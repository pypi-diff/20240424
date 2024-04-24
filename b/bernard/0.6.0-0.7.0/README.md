# Comparing `tmp/bernard-0.6.0.tar.gz` & `tmp/bernard-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bernard-0.6.0.tar", max compression
+gzip compressed data, was "bernard-0.7.0.tar", max compression
```

## Comparing `bernard-0.6.0.tar` & `bernard-0.7.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
--rw-r--r--   0        0        0    34279 2024-02-29 12:00:16.309143 bernard-0.6.0/LICENSE.md
--rw-r--r--   0        0        0    34520 2024-02-29 12:00:16.309143 bernard-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     1671 2024-02-29 12:00:16.309143 bernard-0.6.0/README.md
--rw-r--r--   0        0        0     1340 2024-02-29 12:00:41.305427 bernard-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/__init__.py
--rw-r--r--   0        0        0       32 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/analytics/__init__.py
--rw-r--r--   0        0        0      954 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/analytics/_helpers.py
--rw-r--r--   0        0        0     1752 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/analytics/base.py
--rw-r--r--   0        0        0       33 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/analytics/ga/__init__.py
--rw-r--r--   0        0        0     1683 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/analytics/ga/_ga.py
--rw-r--r--   0        0        0       24 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/cli/__init__.py
--rw-r--r--   0        0        0     1490 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/cli/_base.py
--rw-r--r--   0        0        0     3117 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/cli/_live_reload.py
--rw-r--r--   0        0        0      657 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/conf/__init__.py
--rw-r--r--   0        0        0     4672 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/conf/default_settings.py
--rw-r--r--   0        0        0     3136 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/conf/loader.py
--rw-r--r--   0        0        0     1238 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/conf/utils.py
--rw-r--r--   0        0        0        0 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/core/__init__.py
--rw-r--r--   0        0        0      374 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/core/health_check.py
--rw-r--r--   0        0        0       70 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/engine/__init__.py
--rw-r--r--   0        0        0    11191 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/engine/fsm.py
--rw-r--r--   0        0        0     6267 2024-02-29 12:00:16.313143 bernard-0.6.0/src/bernard/engine/platform.py
--rw-r--r--   0        0        0     6878 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/engine/request.py
--rw-r--r--   0        0        0     2448 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/engine/responder.py
--rw-r--r--   0        0        0     3179 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/engine/state.py
--rw-r--r--   0        0        0     2595 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/engine/transition.py
--rw-r--r--   0        0        0     9772 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/engine/triggers.py
--rw-r--r--   0        0        0      163 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/i18n/__init__.py
--rw-r--r--   0        0        0     3155 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/i18n/_formatter.py
--rw-r--r--   0        0        0     3004 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/i18n/intents.py
--rw-r--r--   0        0        0     7654 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/i18n/loaders.py
--rw-r--r--   0        0        0    16258 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/i18n/translator.py
--rw-r--r--   0        0        0     2831 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/i18n/utils.py
--rw-r--r--   0        0        0      235 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/layers/__init__.py
--rw-r--r--   0        0        0     6711 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/layers/definitions.py
--rw-r--r--   0        0        0     4614 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/layers/stack.py
--rw-r--r--   0        0        0       27 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/media/__init__.py
--rw-r--r--   0        0        0      773 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/media/base.py
--rw-r--r--   0        0        0       99 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/middleware/__init__.py
--rw-r--r--   0        0        0     5224 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/middleware/_builtins.py
--rw-r--r--   0        0        0     4825 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/middleware/_manager.py
--rw-r--r--   0        0        0        0 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/__init__.py
--rw-r--r--   0        0        0       24 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/main/__init__.py
--rw-r--r--   0        0        0     2074 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/main/_base.py
--rw-r--r--   0        0        0       41 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/sheet_sync/__init__.py
--rw-r--r--   0        0        0     3657 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/sheet_sync/_base.py
--rw-r--r--   0        0        0       24 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/__init__.py
--rw-r--r--   0        0        0     3986 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/_base.py
--rw-r--r--   0        0        0      178 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/.editorconfig
--rw-r--r--   0        0        0       63 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/.gitignore
--rw-r--r--   0        0        0      258 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/README.md
--rw-r--r--   0        0        0      478 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/env
--rw-r--r--   0        0        0       33 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/i18n/en/intents.csv
--rw-r--r--   0        0        0      144 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/i18n/en/responses.csv
--rw-r--r--   0        0        0      574 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/manage.py
--rw-r--r--   0        0        0        8 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/requirements.txt
--rw-r--r--   0        0        0        0 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/src/__project_name_snake__/__init__.py
--rw-r--r--   0        0        0     5335 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/src/__project_name_snake__/settings.py
--rw-r--r--   0        0        0     1487 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/src/__project_name_snake__/states.py
--rw-r--r--   0        0        0      235 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/misc/start_project/files/src/__project_name_snake__/transitions.py
--rw-r--r--   0        0        0      444 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/__init__.py
--rw-r--r--   0        0        0        0 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/facebook/__init__.py
--rw-r--r--   0        0        0    10405 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/facebook/helpers.py
--rw-r--r--   0        0        0     8851 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/facebook/layers.py
--rw-r--r--   0        0        0    28612 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/facebook/platform.py
--rw-r--r--   0        0        0     6057 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/management.py
--rw-r--r--   0        0        0        0 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/telegram/__init__.py
--rw-r--r--   0        0        0     1053 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/telegram/_utils.py
--rw-r--r--   0        0        0    15971 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/telegram/layers.py
--rw-r--r--   0        0        0      702 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/telegram/media.py
--rw-r--r--   0        0        0    19730 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/telegram/platform.py
--rw-r--r--   0        0        0       50 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/test/__init__.py
--rw-r--r--   0        0        0     4199 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/platforms/test/platform.py
--rw-r--r--   0        0        0       22 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/server/__init__.py
--rw-r--r--   0        0        0      433 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/server/http.py
--rw-r--r--   0        0        0     3959 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/server/views.py
--rw-r--r--   0        0        0        0 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/storage/__init__.py
--rw-r--r--   0        0        0       94 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/storage/context/__init__.py
--rw-r--r--   0        0        0     6105 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/storage/context/base.py
--rw-r--r--   0        0        0      647 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/storage/context/redis.py
--rw-r--r--   0        0        0     1364 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/storage/redis.py
--rw-r--r--   0        0        0      165 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/storage/register/__init__.py
--rw-r--r--   0        0        0     4017 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/storage/register/base.py
--rw-r--r--   0        0        0     1929 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/storage/register/redis.py
--rw-r--r--   0        0        0     4041 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/trigram.py
--rw-r--r--   0        0        0     6069 2024-02-29 12:00:16.317143 bernard-0.6.0/src/bernard/utils.py
--rw-r--r--   0        0        0     2876 1970-01-01 00:00:00.000000 bernard-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    34279 2024-04-24 11:18:15.564919 bernard-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0    34520 2024-04-24 11:18:15.564919 bernard-0.7.0/LICENSE.txt
+-rw-r--r--   0        0        0     1671 2024-04-24 11:18:15.564919 bernard-0.7.0/README.md
+-rw-r--r--   0        0        0     2658 2024-04-24 11:18:31.649115 bernard-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/__init__.py
+-rw-r--r--   0        0        0       40 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/analytics/__init__.py
+-rw-r--r--   0        0        0      954 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/analytics/_helpers.py
+-rw-r--r--   0        0        0     1863 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/analytics/base.py
+-rw-r--r--   0        0        0       41 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/analytics/ga/__init__.py
+-rw-r--r--   0        0        0     1687 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/analytics/ga/_ga.py
+-rw-r--r--   0        0        0       32 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/cli/__init__.py
+-rw-r--r--   0        0        0     1877 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/cli/_base.py
+-rw-r--r--   0        0        0     4053 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/cli/_live_reload.py
+-rw-r--r--   0        0        0      703 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/conf/__init__.py
+-rw-r--r--   0        0        0     4686 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/conf/default_settings.py
+-rw-r--r--   0        0        0     3242 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/conf/loader.py
+-rw-r--r--   0        0        0     1345 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/conf/utils.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/core/__init__.py
+-rw-r--r--   0        0        0      366 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/core/health_check.py
+-rw-r--r--   0        0        0       86 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/engine/__init__.py
+-rw-r--r--   0        0        0    11358 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/engine/fsm.py
+-rw-r--r--   0        0        0     6338 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/engine/platform.py
+-rw-r--r--   0        0        0     6842 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/engine/request.py
+-rw-r--r--   0        0        0     2419 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/engine/responder.py
+-rw-r--r--   0        0        0     3118 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/engine/state.py
+-rw-r--r--   0        0        0     2622 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/engine/transition.py
+-rw-r--r--   0        0        0    10313 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/engine/triggers.py
+-rw-r--r--   0        0        0      171 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/i18n/__init__.py
+-rw-r--r--   0        0        0     3139 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/i18n/_formatter.py
+-rw-r--r--   0        0        0     3368 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/i18n/intents.py
+-rw-r--r--   0        0        0     8153 2024-04-24 11:18:15.568919 bernard-0.7.0/src/bernard/i18n/loaders.py
+-rw-r--r--   0        0        0    16703 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/i18n/translator.py
+-rw-r--r--   0        0        0     2812 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/i18n/utils.py
+-rw-r--r--   0        0        0      355 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/layers/__init__.py
+-rw-r--r--   0        0        0     6636 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/layers/definitions.py
+-rw-r--r--   0        0        0     4593 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/layers/stack.py
+-rw-r--r--   0        0        0       35 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/media/__init__.py
+-rw-r--r--   0        0        0      753 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/media/base.py
+-rw-r--r--   0        0        0      115 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/middleware/__init__.py
+-rw-r--r--   0        0        0     5188 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/middleware/_builtins.py
+-rw-r--r--   0        0        0     4759 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/middleware/_manager.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/main/__init__.py
+-rw-r--r--   0        0        0     1361 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/main/_base.py
+-rw-r--r--   0        0        0       49 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/sheet_sync/__init__.py
+-rw-r--r--   0        0        0     2945 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/sheet_sync/_base.py
+-rw-r--r--   0        0        0       32 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/__init__.py
+-rw-r--r--   0        0        0     3904 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/_base.py
+-rw-r--r--   0        0        0      178 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/.editorconfig
+-rw-r--r--   0        0        0       63 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/.gitignore
+-rw-r--r--   0        0        0      258 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/README.md
+-rw-r--r--   0        0        0      478 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/env
+-rw-r--r--   0        0        0       33 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/i18n/en/intents.csv
+-rw-r--r--   0        0        0      144 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/i18n/en/responses.csv
+-rwxr-xr-x   0        0        0      596 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/manage.py
+-rw-r--r--   0        0        0        8 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/requirements.txt
+-rw-r--r--   0        0        0        0 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/src/__project_name_snake__/__init__.py
+-rw-r--r--   0        0        0     5329 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/src/__project_name_snake__/settings.py
+-rw-r--r--   0        0        0     1485 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/src/__project_name_snake__/states.py
+-rw-r--r--   0        0        0      239 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/misc/start_project/files/src/__project_name_snake__/transitions.py
+-rw-r--r--   0        0        0      475 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/facebook/__init__.py
+-rw-r--r--   0        0        0    10280 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/facebook/helpers.py
+-rw-r--r--   0        0        0     8727 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/facebook/layers.py
+-rw-r--r--   0        0        0    29072 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/facebook/platform.py
+-rw-r--r--   0        0        0     6019 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/management.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/telegram/__init__.py
+-rw-r--r--   0        0        0     1052 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/telegram/_utils.py
+-rw-r--r--   0        0        0    15552 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/telegram/layers.py
+-rw-r--r--   0        0        0      691 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/telegram/media.py
+-rw-r--r--   0        0        0    23619 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/telegram/platform.py
+-rw-r--r--   0        0        0       58 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/test/__init__.py
+-rw-r--r--   0        0        0     4116 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/platforms/test/platform.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/py.typed
+-rw-r--r--   0        0        0       30 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/server/__init__.py
+-rw-r--r--   0        0        0      381 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/server/http.py
+-rw-r--r--   0        0        0     3991 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/server/views.py
+-rw-r--r--   0        0        0        0 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/storage/__init__.py
+-rw-r--r--   0        0        0      110 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/storage/context/__init__.py
+-rw-r--r--   0        0        0     6049 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/storage/context/base.py
+-rw-r--r--   0        0        0      623 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/storage/context/redis.py
+-rw-r--r--   0        0        0     1307 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/storage/redis.py
+-rw-r--r--   0        0        0      197 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/storage/register/__init__.py
+-rw-r--r--   0        0        0     3961 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/storage/register/base.py
+-rw-r--r--   0        0        0     1897 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/storage/register/redis.py
+-rw-r--r--   0        0        0     4020 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/trigram.py
+-rw-r--r--   0        0        0     5704 2024-04-24 11:18:15.572919 bernard-0.7.0/src/bernard/utils.py
+-rw-r--r--   0        0        0     2796 1970-01-01 00:00:00.000000 bernard-0.7.0/PKG-INFO
```

### Comparing `bernard-0.6.0/LICENSE.md` & `bernard-0.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bernard-0.6.0/LICENSE.txt` & `bernard-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bernard-0.6.0/README.md` & `bernard-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bernard-0.6.0/src/bernard/analytics/_helpers.py` & `bernard-0.7.0/src/bernard/analytics/_helpers.py`

 * *Files identical despite different names*

### Comparing `bernard-0.6.0/src/bernard/analytics/base.py` & `bernard-0.7.0/src/bernard/analytics/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,68 +1,70 @@
 from asyncio import get_event_loop
 from functools import wraps
 from hashlib import sha256
-from typing import Any, Dict, Tuple
+from typing import Any, ClassVar
 
 from bernard.conf import settings
 from bernard.utils import import_class
 
 
-class BaseAnalytics(object):
+class BaseAnalytics:
     """
     Standard interface for analytics tracking. If your platform doesn't support
     some operations, either adapt the concept, either make make the function
     empty and document it.
     """
 
-    _instances: Dict[Tuple[Any, ...], "BaseAnalytics"] = {}
+    _instances: ClassVar[dict[tuple[Any, ...], "BaseAnalytics"]] = {}
 
     async def async_init(self):
         pass
 
     async def page_view(
         self, url: str, title: str, user_id: str, user_lang: str = ""
     ) -> None:
         """
         Track the view of a page
         """
-
         raise NotImplementedError
 
     def hash_user_id(self, user_id: str) -> str:
         """
         As per the law, anonymize user identifier before sending it.
         """
-
         h = sha256()
         h.update(user_id.encode())
         return h.hexdigest()
 
     @classmethod
     async def instance(cls, *args) -> "BaseAnalytics":
         if args not in cls._instances:
             cls._instances[args] = cls(*args)
             await cls._instances[args].async_init()
         return cls._instances[args]
 
 
+_pending_t = set()
+
+
 def new_task(func):
     """
     Runs the decorated function in a new task
     """
 
     @wraps(func)
     async def wrapper(self, *args, **kwargs):
         loop = get_event_loop()
-        loop.create_task(func(self, *args, **kwargs))
+        t = loop.create_task(func(self, *args, **kwargs))
+        _pending_t.add(t)
+        t.add_done_callback(_pending_t.discard)
 
     return wrapper
 
 
 async def providers():
     """
     Iterates over all instances of analytics provider found in configuration
     """
-
     for provider in settings.ANALYTICS_PROVIDERS:
-        cls: BaseAnalytics = import_class(provider["class"])
+        cls: BaseAnalytics = import_class(provider["class"])  # type: ignore
         yield await cls.instance(*provider["args"])
```

### Comparing `bernard-0.6.0/src/bernard/analytics/ga/_ga.py` & `bernard-0.7.0/src/bernard/analytics/ga/_ga.py`

 * *Files 10% similar despite different names*

```diff
@@ -55,10 +55,10 @@
             args["ul"] = user_lang
 
         logger.debug("GA settings = %s", urlencode(args))
 
         r = await self.session.post(ga_url, data=args)
 
         if r.status_code == 200:
-            logger.debug(f"Sent to GA {url} ({title}) for user {user_id}")
+            logger.debug("Sent to GA %s (%s) for user %s", url, title, user_id)
         else:
-            logger.warning(f"Could not contact GA")
+            logger.warning("Could not contact GA")
```

### Comparing `bernard-0.6.0/src/bernard/cli/_base.py` & `bernard-0.7.0/src/bernard/cli/_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,84 @@
 import logging
 
-logger = logging.getLogger("bernard.cli")
-
-
-def init_uvloop():
-    import asyncio
+from rich.logging import RichHandler
 
-    import uvloop
-
-    asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
+logger = logging.getLogger("bernard.cli")
+_tasks = set()
 
 
 def init_logger():
     import logging
 
     logging.basicConfig(
-        level=logging.DEBUG,
+        level=logging.WARNING,
+        format=r"[bold cyan]\[%(name)s][/] %(message)s",
+        datefmt="[%X]",
+        handlers=[RichHandler(markup=True)],
     )
+    logging.getLogger("watchdog.observers").setLevel(logging.WARNING)
+    logging.getLogger("httpcore").setLevel(logging.WARNING)
+    logging.getLogger("httpx").setLevel(logging.WARNING)
 
 
-def init_live_reload(run):
+async def init_live_reload(run):
     """
     Start the live reload task
 
     :param run: run the task inside of this function or just create it
     """
     from asyncio import get_event_loop
 
     from ._live_reload import start_child
 
     loop = get_event_loop()
 
     if run:
-        loop.run_until_complete(start_child())
+        await start_child()
     else:
-        get_event_loop().create_task(start_child())
+        t = loop.create_task(start_child())
+        _tasks.add(t)
+        t.add_done_callback(_tasks.discard)
+
+
+async def run_core():
+    import asyncio
+
+    from aiohttp import web
+
+    from bernard.conf import settings
+    from bernard.platforms import start_all
+    from bernard.server import app
+
+    try:
+        await start_all()
+
+        web_t = asyncio.create_task(web._run_app(app, **settings.SERVER_BIND))
+
+        if settings.CODE_LIVE_RELOAD:
+            await init_live_reload(False)
+
+        await web_t
+    except Exception:
+        logger.exception("Error while running core")
+
+        if settings.CODE_LIVE_RELOAD:
+            await init_live_reload(True)
 
 
 def main():
     init_logger()
-    init_uvloop()
 
+    import asyncio
     from os import getenv
 
     from bernard.conf import settings
 
+    if settings.DEBUG:
+        logging.root.setLevel(logging.DEBUG)
+
     if settings.CODE_LIVE_RELOAD and getenv("_IN_CHILD") != "yes":
         from ._live_reload import start_parent
 
         return start_parent()
 
-    # noinspection PyBroadException
-    try:
-        from aiohttp import web
-
-        from bernard.platforms import start_all
-        from bernard.server import app
-        from bernard.utils import run
-
-        run(start_all())
-
-        if settings.CODE_LIVE_RELOAD:
-            init_live_reload(False)
-    except Exception:
-        logger.exception("Something bad happened while bootstraping")
-
-        if settings.CODE_LIVE_RELOAD:
-            init_live_reload(True)
-    else:
-        # noinspection PyArgumentList
-        web.run_app(app, **settings.SERVER_BIND)
+    asyncio.run(run_core())
```

### Comparing `bernard-0.6.0/src/bernard/conf/__init__.py` & `bernard-0.7.0/src/bernard/conf/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 """
 Settings management.
 
 This module is really inspired by the Django and the Sanic config systems,
 thanks to their teams.
 """
+
 import os
-from typing import List, Text
+from pathlib import Path
+from typing import List
 
 from .loader import LazySettings
 
 ENVIRONMENT_VARIABLE = "BERNARD_SETTINGS_FILE"
 
 
-def list_config_files() -> List[Text]:
+def list_config_files() -> List[Path]:
     """
     This function returns the list of configuration files to load.
 
     This is a callable so the configuration can be reloaded with files that
     changed in between.
     """
 
-    return [
-        os.path.join(os.path.dirname(__file__), "default_settings.py"),
-        os.getenv(ENVIRONMENT_VARIABLE, ""),
-    ]
+    out = [Path(__file__).parent / "default_settings.py"]
+
+    if env_path := os.getenv(ENVIRONMENT_VARIABLE):
+        out.append(Path(env_path))
+
+    return out
 
 
 settings = LazySettings(list_config_files)
```

### Comparing `bernard-0.6.0/src/bernard/conf/default_settings.py` & `bernard-0.7.0/src/bernard/conf/default_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 # set properly.
 WEBVIEW_SECRET_KEY = None
 
 # JWT algorithm
 WEBVIEW_JWT_ALGORITHM = "HS256"
 
 # Where to store the webview token
-WEBVIEW_TOKEN_KEY = "_b"
+WEBVIEW_TOKEN_KEY = "_b"  # noqa: S105
 
 # What is the header name
 WEBVIEW_HEADER_NAME = "X-BERNARD-AUTH"
 
 # Webviews are supposed to send a message when they close. However, it can
 # happen on some shitty devices (follow my eyes) that connections are not
 # closed properly. In this case, if we receive no heartbeat for X seconds then
```

### Comparing `bernard-0.6.0/src/bernard/conf/loader.py` & `bernard-0.7.0/src/bernard/conf/loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,68 +1,72 @@
 import re
 import types
-from typing import Any, Text
+from pathlib import Path
+from typing import Any
 
 CONFIG_ATTR = re.compile(r"^[A-Z](?:_?[A-Z0-9]+)*$")
 
 
 class Settings(dict):
     """
     This object handles settings loaded from a pure Python file.
     """
 
-    def __getattr__(self, attr: Text) -> Any:
+    def __getattr__(self, attr: str) -> Any:
         """
         Return a config value. Get it from the internal dict.
 
         :param attr: Name of the config value you want
         """
         try:
             return self[attr]
         except KeyError as ke:
-            raise AttributeError("Config has no '{}'".format(ke.args[0]))
+            msg = f"Config has no '{ke.args[0]}'"
+            raise AttributeError(msg) from None
 
-    def __setattr__(self, attr: Text, value: Any) -> None:
+    def __setattr__(self, attr: str, value: Any) -> None:
         """
         Define a configuration value. Internally, it is stored as a dictionary
         entry.
 
         :param attr: Key to save
         :param value: Value to put
         """
         self[attr] = value
 
-    def _load(self, file_path: Text) -> None:
+    def _load(self, file_path: str | Path) -> None:
         """
         Load the configuration from a plain Python file. This file is executed
         on its own.
 
         Only keys matching the CONFIG_ATTR will be loaded. Basically, it's
         CONFIG_KEYS_LIKE_THIS.
 
         :param file_path: Path to the file to load
         """
-
         # noinspection PyUnresolvedReferences
         module_ = types.ModuleType("settings")
         module_.__file__ = file_path
 
         try:
-            with open(file_path, encoding="utf-8") as f:
-                exec(compile(f.read(), file_path, "exec"), module_.__dict__)
-        except IOError as e:
-            e.strerror = "Unable to load configuration file ({})".format(e.strerror)
+            with Path(file_path).open(encoding="utf-8") as f:
+                exec(  # noqa: S102
+                    compile(f.read(), file_path, "exec"),
+                    module_.__dict__,
+                )
+        except OSError as e:
+            e.strerror = f"Unable to load configuration file ({e.strerror})"
             raise
 
         for key in dir(module_):
             if CONFIG_ATTR.match(key):
                 self[key] = getattr(module_, key)
 
 
-class LazySettings(object):
+class LazySettings:
     """
     This object lazily loads the settings at first access.
 
     It works like `Settings`, except that instead of calling the `_load()`
     method, specify a list of files to load as argument.
     """
 
@@ -92,18 +96,18 @@
 
     def _reload(self) -> None:
         """
         Delete the inner settings object so it gets reloaded.
         """
         self.__dict__["__settings"] = None
 
-    def __getattr__(self, key: Text) -> Any:
+    def __getattr__(self, key: str) -> Any:
         """
         Proxy to `Settings.__getattr__`
         """
         return getattr(self._settings, key)
 
-    def __setattr__(self, key: Text, value: Any) -> None:
+    def __setattr__(self, key: str, value: Any) -> None:
         """
         Proxy to `Settings.__setattr__`
         """
         return setattr(self._settings, key, value)
```

### Comparing `bernard-0.6.0/src/bernard/conf/utils.py` & `bernard-0.7.0/src/bernard/conf/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 from contextlib import contextmanager
+from pathlib import Path
 from sys import modules
 
 from bernard.conf import settings
 
 from ..conf import ENVIRONMENT_VARIABLE
 
 
 def reload_config() -> None:
     """
     Reload the whole configuration.
     """
-
     # noinspection PyProtectedMember
     settings._reload()
 
 
 # noinspection PyProtectedMember
 @contextmanager
 def patch_conf(settings_patch=None, settings_file=None):
@@ -26,18 +26,20 @@
     Then the specified patch is applied.
 
     This is for unit tests only!
 
     :param settings_patch: Custom configuration values to insert
     :param settings_file: Custom settings file to read
     """
-
     if settings_patch is None:
         settings_patch = {}
 
+    if isinstance(settings_file, Path):
+        settings_file = str(settings_file)
+
     reload_config()
     os.environ[ENVIRONMENT_VARIABLE] = settings_file if settings_file else ""
 
     from bernard.conf import settings as l_settings
 
     # noinspection PyProtectedMember
     r_settings = l_settings._settings
```

### Comparing `bernard-0.6.0/src/bernard/engine/fsm.py` & `bernard-0.7.0/src/bernard/engine/fsm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
 import importlib
 import logging
-from typing import Dict, Iterator, List, Optional, Text, Tuple, Type
+from typing import AsyncIterator, Dict, Iterator, List, Optional, Tuple, Type
 
 import sentry_sdk
 
 from bernard.conf import settings
 from bernard.core.health_check import HealthCheckFail
 from bernard.i18n.translator import MissingTranslationError
 from bernard.layers import RawText
@@ -30,15 +30,18 @@
 
 class MaxInternalJump(FsmError):
     """
     That's when the max number of internal jumps is reached
     """
 
 
-class FSM(object):
+_pending_t = set()
+
+
+class FSM:
     """
     The FSM is the core of the engine. FSM as in "Finite-State Machine".
 
     Bots are represented as a FSM: states are the various states of the but,
     and each state handler sends messages to the user. Transitions are
     triggered by events from the user (or crons, or whatever).
 
@@ -49,33 +52,32 @@
     """
 
     def __init__(self):
         self.register = self._make_register()
         self.transitions = self._make_transitions()
         self._allowed_states = set(self._make_allowed_states())
 
-    async def health_check(self) -> Iterator[HealthCheckFail]:
+    async def health_check(self) -> AsyncIterator[HealthCheckFail]:
         """
         Perform the checks. So far:
 
         - Make a list of the unique destination states from the transitions
           list, then check the health of each of them.
         """
-
         ds_class = getattr(settings, "DEFAULT_STATE", "")
         forbidden_defaults = [None, "", "bernard.engine.state.DefaultState"]
 
         if ds_class in forbidden_defaults:
             yield HealthCheckFail(
                 "00005",
-                f"Default state (`DEFAULT_STATE` in settings) is not set. "
-                f"You need to set it to your own implementation. Please refer "
-                f"yourself to the doc. See "
-                f"https://github.com/BernardFW/bernard/blob/develop/doc/"
-                f"get_started.md#statespy",
+                "Default state (`DEFAULT_STATE` in settings) is not set. "
+                "You need to set it to your own implementation. Please refer "
+                "yourself to the doc. See "
+                "https://github.com/BernardFW/bernard/blob/develop/doc/"
+                "get_started.md#statespy",
             )
 
         try:
             import_class(ds_class)
         except (ImportError, KeyError, AttributeError, TypeError):
             yield HealthCheckFail(
                 "00005",
@@ -85,64 +87,63 @@
                 f" to `DEFAULT_STATE` is wrong. You need to provide a default"
                 f" state class for this framework to work. Please refer"
                 f" yourself to the documentation for more information. See"
                 f" https://github.com/BernardFW/bernard/blob/develop/doc/"
                 f"get_started.md#statespy",
             )
 
-        states = set(t.dest for t in self.transitions)
+        states = {t.dest for t in self.transitions}
 
         for state in states:
             async for check in state.health_check():
                 yield check
 
     async def async_init(self):
         """
         THe register might need to be initialized in a loop
         """
-
         await self.register.async_init()
 
     def _make_register(self) -> BaseRegisterStore:
         """
         Make the register storage.
         """
-
         s = settings.REGISTER_STORE
         store_class = import_class(s["class"])
         return store_class(**s["params"])
 
     def _make_transitions(self) -> List[Transition]:
         """
         Load the transitions file.
         """
-
         module_name = settings.TRANSITIONS_MODULE
         module_ = importlib.import_module(module_name)
         return module_.transitions
 
-    def _make_allowed_states(self) -> Iterator[Text]:
+    def _make_allowed_states(self) -> Iterator[str]:
         """
         Sometimes we load states from the database. In order to avoid loading
         an arbitrary class, we list here the state classes that are allowed.
         """
-
         for trans in self.transitions:
             yield trans.dest.name()
 
             if trans.origin:
                 yield trans.origin.name()
 
     async def _find_trigger(
-        self, request: Request, origin: Optional[Text] = None, internal: bool = False
-    ) -> Tuple[Optional[BaseTrigger], Optional[Type[BaseState]], Optional[bool],]:
+        self, request: Request, origin: Optional[str] = None, internal: bool = False
+    ) -> Tuple[
+        Optional[BaseTrigger],
+        Optional[Type[BaseState]],
+        Optional[bool],
+    ]:
         """
         Find the best trigger for this request, or go away.
         """
-
         reg = request.register
 
         if not origin:
             origin = reg.get(Register.STATE)
             logger.debug("From state: %s", origin)
 
         results = await asyncio.gather(
@@ -162,32 +163,34 @@
         return None, None, None
 
     # noinspection PyTypeChecker
     def _confused_state(self, request: Request) -> Type[BaseState]:
         """
         If we're confused, find which state to call.
         """
-
         origin = request.register.get(Register.STATE)
 
         if origin in self._allowed_states:
             try:
                 return import_class(origin)
             except (AttributeError, ImportError):
                 pass
 
         return import_class(settings.DEFAULT_STATE)
 
     async def _build_state(
         self, request: Request, message: BaseMessage, responder: Responder
-    ) -> Tuple[Optional[BaseState], Optional[BaseTrigger], Optional[bool],]:
+    ) -> Tuple[
+        Optional[BaseState],
+        Optional[BaseTrigger],
+        Optional[bool],
+    ]:
         """
         Build the state for this request.
         """
-
         trigger, state_class, dnr = await self._find_trigger(request)
 
         if trigger is None:
             if not message.should_confuse():
                 return None, None, None
             state_class = self._confused_state(request)
             logger.debug("Next state: %s (confused)", state_class.name())
@@ -197,15 +200,14 @@
         state = state_class(request, responder, trigger, trigger)
         return state, trigger, dnr
 
     async def _run_state(self, responder, state, trigger, request) -> BaseState:
         """
         Execute the state, or if execution fails handle it.
         """
-
         user_trigger = trigger
 
         # noinspection PyBroadException
         try:
             if trigger:
                 await state.handle()
             else:
@@ -239,15 +241,14 @@
         """
         Build the next register to store.
 
             - The state is the name of the current state
             - The transition is made by all successive layers present in the
               response.
         """
-
         return {
             Register.STATE: state.name(),
             Register.TRANSITION: await responder.make_transition_register(request),
         }
 
     async def _handle_message(
         self, message: BaseMessage, responder: Responder
@@ -265,37 +266,37 @@
         reg_manager = self.register.work_on_register(message.get_conversation().id)
 
         async with reg_manager as reg:
             request = Request(message, reg)
             await request.transform()
 
             if not request.stack.layers:
-                return
+                return None
 
             logger.debug("Incoming message: %s", request.stack)
             await mm.get("pre_handle", noop)(request, responder)
 
             # noinspection PyBroadException
             try:
                 state, trigger, dnr = await self._build_state(
                     request, message, responder
                 )
             except Exception as e:
                 logger.exception(
                     "Error while finding a transition from %s", reg.get(Register.STATE)
                 )
                 sentry_sdk.capture_exception(e)
-                return
+                return None
 
             if state is None:
                 logger.debug(
                     'No next state found but "%s" is not confusing, stopping',
                     request.message,
                 )
-                return
+                return None
 
             state = await self._run_state(responder, state, trigger, request)
 
             # noinspection PyBroadException
             try:
                 await responder.flush(request)
             except MissingTranslationError as e:
@@ -326,15 +327,16 @@
             - A message from the platform
             - A responder from the platform
 
         If `create_task` is true, them the task will automatically be added to
         the loop. However, if it is not, the coroutine will be returned and it
         will be the responsibility of the caller to run/start the task.
         """
-
         coro = self._handle_message(message, responder)
 
         if create_task:
             loop = asyncio.get_event_loop()
-            loop.create_task(coro)
+            t = loop.create_task(coro)
+            _pending_t.add(t)
+            t.add_done_callback(_pending_t.discard)
         else:
             return coro
```

### Comparing `bernard-0.6.0/src/bernard/engine/platform.py` & `bernard-0.7.0/src/bernard/engine/platform.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import asyncio
-from typing import Any, Callable, List, Optional, Text
+from typing import Any, Callable, ClassVar, Optional
 
 import httpx
 from aiohttp.web_urldispatcher import UrlDispatcher
 
 from bernard.engine.request import Request
 from bernard.engine.responder import Responder, UnacceptableStack
 from bernard.layers import Stack
@@ -11,15 +11,15 @@
 from bernard.utils import import_class
 
 from .request import BaseMessage
 
 MessageCallback = Callable[[BaseMessage, Responder, bool], None]
 
 
-class Platform(object):
+class Platform:
     """
     Base class for the platforms. You need to overload it in order to create
     your own platform.
 
     To create a new platform, you need two things:
 
         - Call `_notify()` when you receive a message from the platform
@@ -47,39 +47,36 @@
 
     @classmethod
     def settings(cls):
         """
         Find the settings for the current class inside the platforms
         configuration.
         """
-
         from bernard.platforms.management import get_platform_settings
 
         for platform in get_platform_settings():
             candidate = import_class(platform["class"])
             if candidate == cls:
                 return platform.get("settings", {})
 
     @property
     def id(self):
         """
         Allows to get several instances of the same class, using a custom
         `name` attribute in the platform configuration.
         """
-
         if self._id:
             return self._id
 
         return self.NAME
 
     def on_message(self, cb: MessageCallback):
         """
         Register a callback to listen for incoming messages.
         """
-
         self._listeners.append(cb)
 
     async def _notify(self, message: BaseMessage, responder: Responder):
         """
         Notify all callbacks that a message was received.
         """
         for cb in self._listeners:
@@ -111,100 +108,100 @@
         raise NotImplementedError
 
     @classmethod
     async def self_check(cls):
         """
         Run the self health-check. This one is a dummy one.
         """
-
-        for i in []:
+        for _ in []:
             yield
 
     def hook_up(self, router: UrlDispatcher):
         """
         This is where the platform can register its routes (for the hooks and
         so on).
         """
-
         pass
 
     async def message_from_token(
-        self, token: Text, payload: Any
+        self, token: str, payload: Any
     ) -> Optional[BaseMessage]:
         """
         Given a token and a payload, create a message for this platform with
         a Postback layer holding the payload.
         """
-
         raise NotImplementedError
 
     async def inject_message(self, message: BaseMessage) -> None:
         """
         Injects a message into the platform and handles it in the FSM
         """
-
         raise NotImplementedError
 
 
+_running_t = set()
+
+
 class SimplePlatform(Platform):
-    PATTERNS = {}
+    PATTERNS: ClassVar[dict] = {}
 
     def __init__(self):
-        super(SimplePlatform, self).__init__()
+        super().__init__()
         self.session = None
 
     async def async_init(self):
         """
-        During async init we just need to create a HTTP session so we can keep
-        outgoing connexions to the platform alive.
+        During async init we just need to create an HTTP session, so we can
+        keep outgoing connexions to the platform alive.
         """
         self.session = httpx.AsyncClient()
-        _ = asyncio.get_event_loop().create_task(self._deferred_init())
+
+        t = asyncio.get_event_loop().create_task(self._deferred_init())
+        _running_t.add(t)
+        t.add_done_callback(_running_t.discard)
 
     async def _deferred_init(self):
         """
-        Run those things in a sepearate tasks as they are not required for the
-        bot to work and they take a lot of time to run.
+        Run those things in a separate tasks as they are not required for the
+        bot to work, and they take a lot of time to run.
         """
         raise NotImplementedError
 
     def accept(self, stack: Stack):
         """
         Checks that the stack can be accepted according to the `PATTERNS`.
 
         If the pattern is found, then its name is stored in the `annotation`
         attribute of the stack.
         """
-
         for name, pattern in self.PATTERNS.items():
             if stack.match_exp(pattern):
                 stack.annotation = name
                 return True
         return False
 
     async def send(self, request: Request, stack: Stack):
         """
         Send a stack to the platform.
 
         Actually this will delegate to one of the `_send_*` functions depending
         on what the stack looks like.
         """
-
-        if stack.annotation not in self.PATTERNS:
-            if not self.accept(stack):
-                raise UnacceptableStack("Cannot accept stack {}".format(stack))
+        if stack.annotation not in self.PATTERNS and not self.accept(stack):
+            msg = f"Cannot accept stack {stack}"
+            raise UnacceptableStack(msg)
 
         func = getattr(self, "_send_" + stack.annotation)
         return await func(request, stack)
 
     def ensure_usable_media(self, media: BaseMedia) -> BaseMedia:
         raise NotImplementedError
 
     async def message_from_token(
-        self, token: Text, payload: Any
+        self, token: str, payload: Any
     ) -> Optional[BaseMessage]:
         raise NotImplementedError
 
     async def inject_message(self, message: BaseMessage) -> None:
         raise NotImplementedError
```

### Comparing `bernard-0.6.0/src/bernard/engine/request.py` & `bernard-0.7.0/src/bernard/engine/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from datetime import tzinfo
 from enum import Enum
-from typing import TYPE_CHECKING, Any, List, Optional, Text, Type
+from typing import TYPE_CHECKING, Any, List, Optional, Type
 from urllib.parse import quote, urlparse, urlunparse
 
 from bernard.conf import settings
 from bernard.layers import BaseLayer, Stack
 from bernard.layers.stack import L
 from bernard.storage.register import Register
 from bernard.utils import patch_qs
 
 if TYPE_CHECKING:
     from bernard.i18n.translator import Flags
 
 
-class Conversation(object):
+class Conversation:
     """
     Abstract representation of a conversation.
     """
 
     def __init__(self, id_):
         self.id = id_
 
 
-class User(object):
+class User:
     """
     Abstract representation of a user.
     """
 
     class Gender(Enum):
         """
         Represents the gender of a person. Unknown is to be used either when
@@ -43,60 +43,60 @@
 
     async def get_gender(self) -> Gender:
         """
         Returns the gender of the person if known
         """
         return self.Gender.unknown
 
-    async def get_friendly_name(self) -> Text:
+    async def get_friendly_name(self) -> str:
         """
         Computes a friendly name (like in "Hi Rémy")
         """
         raise NotImplementedError
 
-    async def get_formal_name(self) -> Text:
+    async def get_formal_name(self) -> str:
         """
         Computes a formal name (like in "Howdy Mr Sanchez")
         """
         raise NotImplementedError
 
-    async def get_full_name(self) -> Text:
+    async def get_full_name(self) -> str:
         """
         Computes an administrative full name (like "Name: Rémy Sanchez")
         """
         raise NotImplementedError
 
     async def get_timezone(self) -> Optional[tzinfo]:
         """
         Return the current time zone of the user
         """
         raise NotImplementedError
 
-    async def get_locale(self) -> Text:
+    async def get_locale(self) -> str:
         """
         Returns a locale-descripting string
         """
         raise NotImplementedError
 
 
-class BaseMessage(object):
+class BaseMessage:
     """
     This class represents a message received by the platform. It is in charge
     of implementing the following abstract methods from what the platform
     can provide.
 
     The methods here should, in principle, only get called once. Though it's
     not guaranteed.
     """
 
     def __repr__(self):
         stack = Stack(self.get_layers())
         return f"{self.__class__.__name__}({stack})"
 
-    def get_platform(self) -> Text:
+    def get_platform(self) -> str:
         """
         Return a static string indicating the name of the platform that this
         message comes from.
         """
         raise NotImplementedError
 
     def get_user(self) -> User:
@@ -120,28 +120,27 @@
     def should_confuse(self) -> bool:
         """
         If this returns "True" then the message should trigger a confused state
         when not understood.
 
         Otherwise, it is simply ignored.
         """
-
         return True
 
-    async def get_token(self) -> Text:
+    async def get_token(self) -> str:
         """
         Returns an authentication token that can be understood by the platform.
         """
         raise NotImplementedError
 
 
-class Request(object):
+class Request:
     """
     The request object is generated after each message. Its goal is to provide
-    a comprehensive access to the received message and its context to be used
+    comprehensive access to the received message and its context to be used
     by the transitions and the handlers.
     """
 
     QUERY = "query"
     HASH = "hash"
 
     def __init__(self, message: BaseMessage, register: Register):
@@ -154,23 +153,22 @@
         self.custom_content = {}
 
         self._locale_override = None
 
     async def transform(self):
         await self.stack.transform(self)
 
-    def get_trans_reg(self, name: Text, default: Any = None) -> Any:
+    def get_trans_reg(self, name: str, default: Any = None) -> Any:
         """
         Convenience function to access the transition register of a specific
         kind.
 
         :param name: Name of the register you want to see
         :param default: What to return by default
         """
-
         tr = self.register.get(Register.TRANSITION, {})
         return tr.get(name, default)
 
     def has_layer(self, class_: Type[L], became: bool = True) -> bool:
         """
         Proxy to stack
         """
@@ -184,62 +182,57 @@
 
     def get_layers(self, class_: Type[L], became: bool = True) -> List[L]:
         """
         Proxy to stack
         """
         return self.stack.get_layers(class_, became)
 
-    def set_locale_override(self, locale: Text) -> None:
+    def set_locale_override(self, locale: str) -> None:
         """
         This allows to override manually the locale that will be used in
         replies.
 
         :param locale: Name of the locale (format 'fr' or 'fr_FR')
         """
-
         self._locale_override = locale
 
-    async def get_locale(self) -> Text:
+    async def get_locale(self) -> str:
         """
         Get the locale to use for this request. It's either the overridden
         locale or the locale provided by the platform.
 
         :return: Locale to use for this request
         """
-
         if self._locale_override:
             return self._locale_override
         else:
             return await self.user.get_locale()
 
     async def get_trans_flags(self) -> "Flags":
         """
         Gives a chance to middlewares to make the translation flags
         """
-
         from bernard.middleware import MiddlewareManager
 
         async def make_flags(request: Request) -> "Flags":
             return {}
 
         mf = MiddlewareManager.instance().get("make_trans_flags", make_flags)
         return await mf(self)
 
-    async def get_token(self) -> Text:
+    async def get_token(self) -> str:
         """
         Returns the auth token from the message
         """
-
         return await self.message.get_token()
 
     async def sign_url(self, url, method=HASH):
         """
-        Sign an URL with this request's auth token
+        Sign a URL with this request's auth token
         """
-
         token = await self.get_token()
 
         if method == self.QUERY:
             return patch_qs(
                 url,
                 {
                     settings.WEBVIEW_TOKEN_KEY: token,
@@ -247,8 +240,9 @@
             )
         elif method == self.HASH:
             hash_id = 5
             p = list(urlparse(url))
             p[hash_id] = quote(token)
             return urlunparse(p)
         else:
-            raise ValueError(f'Invalid signing method "{method}"')
+            msg = f'Invalid signing method "{method}"'
+            raise ValueError(msg)
```

### Comparing `bernard-0.6.0/src/bernard/engine/responder.py` & `bernard-0.7.0/src/bernard/engine/responder.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     """
     Base responder exception
     """
 
 
 class UnacceptableStack(ResponderError):
     """
-    The stack you're tryping to send can't be accepted by the platform
+    The stack you're trying to send can't be accepted by the platform
     """
 
 
-class Responder(object):
+class Responder:
     """
     The responder is the abstract object that allows to talk back to the
     conversation.
 
     If you implement a platform, you can overload this class but you probably
     won't need to change anything.
     """
@@ -35,30 +35,27 @@
         self.platform = platform
         self._stacks = []  # type: List[Stack]
 
     def send(self, stack: Layers):
         """
         Add a message stack to the send list.
         """
-
         if not isinstance(stack, Stack):
             stack = Stack(stack)
 
         if not self.platform.accept(stack):
-            raise UnacceptableStack(
-                'The platform does not allow "{}"'.format(stack.describe())
-            )
+            msg = f'The platform does not allow "{stack.describe()}"'
+            raise UnacceptableStack(msg)
 
         self._stacks.append(stack)
 
     def clear(self):
         """
         Reset the send list.
         """
-
         self._stacks = []
 
     async def flush(self, request: "Request"):
         """
         Send all queued messages.
 
         The first step is to convert all media in the stacked layers then the
@@ -73,22 +70,20 @@
         await func(request, self._stacks)
 
     async def _flush(self, request: "Request", stacks: List[Stack]):
         """
         Perform the actual sending to platform. This is separated from
         `flush()` since it needs to be inside a middleware call.
         """
-
         for stack in stacks:
             await self.platform.send(request, stack)
 
     async def make_transition_register(self, request: "Request"):
         """
         Use all underlying stacks to generate the next transition register.
         """
-
         register = {}
 
         for stack in self._stacks:
             register = await stack.patch_register(register, request)
 
         return register
```

### Comparing `bernard-0.6.0/src/bernard/engine/state.py` & `bernard-0.7.0/src/bernard/engine/state.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from bernard.engine.triggers import BaseTrigger
 from bernard.layers import BaseLayer, Text
 
 from .request import Request
 from .responder import Responder
 
 
-class BaseState(object):
+class BaseState:
     """
     This is the base state interface. When implementing a bot, you need to
     implement it.
 
     What is advised is to create your own base class for your bot, so it can
     have a default `error()` and `confused()` behaviour, and then inherit
     this class from everywhere. This base subclass can then become the
@@ -33,64 +33,55 @@
 
     @classmethod
     def name(cls):
         """
         Generate a unique name for this state based on its fully qualified
         name.
         """
-
-        return "{}.{}".format(
-            cls.__module__,
-            cls.__qualname__,
-        )
+        return f"{cls.__module__}.{cls.__qualname__}"
 
     @classmethod
     async def health_check(cls) -> Iterator[HealthCheckFail]:
         """
         Perform checks of the state itself. So far:
 
         - For each method of the class, check for the presence of a
           health_check() method. If the method is present then call it. This is
           used to allow the context decorator to make some checks on the
           structure of the class.
         """
-
-        for k, v in cls.__dict__.items():
+        for v in cls.__dict__.values():
             if hasattr(v, "health_check") and callable(v.health_check):
                 async for check in v.health_check(cls):
                     yield check
 
     async def error(self) -> None:
         """
         This is what happens when the code screws up (aka error 500).
         """
-
         raise NotImplementedError
 
     async def confused(self) -> None:
         """
         This is called when a good state cannot be found.
         """
-
         raise NotImplementedError
 
     async def handle(self) -> None:
         """
         That's the regular state handling method that gets called when all
         goes well. You need to overload this one and reply your things to the
         user.
         """
-
         raise NotImplementedError
 
     def send(self, *stack: BaseLayer):
         """
         Shortcut method to send a reply.
         """
-
         self.responder.send(list(stack))
 
 
 class DefaultState(BaseState):
     """
     That's the default default state. You really need to make your own default
     state but this one here is created so not everything crashes if you forget
```

### Comparing `bernard-0.6.0/src/bernard/engine/transition.py` & `bernard-0.7.0/src/bernard/engine/transition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from typing import Optional, Text, Tuple, Type
+from typing import Optional, Tuple, Type
 
 from bernard.conf import settings
 from bernard.utils import run_or_return
 
 from .state import BaseState
 from .triggers import BaseTrigger
 
 
-class Transition(object):
+class Transition:
     """
     Describes a specific transition from one state to the other, with the
     trigger in charge.
     """
 
     def __init__(
         self,
         dest: Type[BaseState],
         factory,
-        origin: Type[BaseState] = None,
+        origin: Type[BaseState] | None = None,
         weight: float = 1.0,
-        desc: Text = "",
+        desc: str = "",
         internal: bool = False,
         do_not_register: bool = False,
     ):
         """
         Create the transition.
 
         :param dest: Destination state
@@ -32,15 +32,14 @@
         :param weight: Weight of the transition (1 by default, can be reduced)
         :param desc: A textual description for documentation
         :param internal: That transition is an internal jump (eg it is only
                          triggered right after handling another state).
         :param do_not_register: The transition won't be saved into the
                                 register.
         """
-
         self.origin = origin
         self.dest = dest
         self.factory = factory
         self.weight = weight
         self.desc = desc
         self.internal = internal
         self.do_not_register = do_not_register
@@ -54,26 +53,30 @@
         return "{} -[{}]-> {}".format(
             self.origin.__name__ if self.origin else "(init)",
             getattr(self.factory, "trigger_name", "???"),
             self.dest.__name__,
         )
 
     async def rank(
-        self, request, origin: Optional[Text]
-    ) -> Tuple[float, Optional[BaseTrigger], Optional[type], Optional[bool],]:
+        self, request, origin: Optional[str]
+    ) -> Tuple[
+        float,
+        Optional[BaseTrigger],
+        Optional[type],
+        Optional[bool],
+    ]:
         """
         Computes the rank of this transition for a given request.
 
         It returns (in order):
 
             - The score (from 0 to 1)
             - The trigger instance (if it matched)
             - The class of the destination state (if matched)
         """
-
         if self.origin_name == origin:
             score = 1.0
         elif self.origin_name is None:
             score = settings.JUMPING_TRIGGER_PENALTY
         else:
             return 0.0, None, None, None
```

### Comparing `bernard-0.6.0/src/bernard/engine/triggers.py` & `bernard-0.7.0/src/bernard/engine/triggers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import asyncio
-from typing import Any, Callable, List, Optional
-from typing import Text as TextT
-from typing import Type
+from typing import Any, Callable, List, Optional, Type
 
 from bernard import layers as l
 from bernard.engine.request import Request
 from bernard.i18n import intents, render
 from bernard.i18n.intents import Intent
 from bernard.trigram import Matcher, Trigram
 from bernard.utils import run_or_return
 
 
-class BaseTrigger(object):
+class BaseTrigger:
     def __init__(self, request: Request):
         self.request = request
 
     @classmethod
     def builder(cls, *args, **kwargs) -> Callable[[Request], "BaseTrigger"]:
         def factory(request: Request):
             return cls(request, *args, **kwargs)
@@ -48,79 +46,71 @@
     """
 
     @classmethod
     def name(cls) -> str:
         """
         Computes a unique name for this class
         """
-
         return f"{cls.__module__}.{cls.__qualname__}"
 
     @property
     def content_key(self) -> str:
         """
         That's the key used to store the content in the request
         """
-
         return f"{self.name()}::content"
 
     @property
     def lock_key(self) -> str:
         """
         That's the key to store the lock of this trigger
         """
-
         return f"{self.name()}::lock"
 
     @property
     def lock(self) -> asyncio.Lock:
         """
         Return and generate if required the lock for this request.
         """
-
         if self.lock_key not in self.request.custom_content:
             self.request.custom_content[self.lock_key] = asyncio.Lock()
 
         return self.request.custom_content[self.lock_key]
 
     async def call_api(self) -> Any:
         """
         You need to implement here the call to your API. The value it returns
         will be passed to `compute_rank()` later on.
         """
-
         raise NotImplementedError
 
     async def compute_rank(self, value: Any) -> Optional[float]:
         """
         Compute the rank from the cached value from the API call.
         """
-
         raise NotImplementedError
 
     async def get_value(self):
         """
         Get the value from the API. Make sure to use a lock in order not to
         fetch the value twice at the same time.
         """
-
         cc = self.request.custom_content
 
         async with self.lock:
             if self.content_key not in cc:
                 cc[self.content_key] = await self.call_api()
 
         return cc[self.content_key]
 
     async def rank(self):
         """
         Compute the rank based on the (cached) value and on the overriden
         rank computation function.
         """
-
         return await self.compute_rank(await self.get_value())
 
 
 class Anything(BaseTrigger):
     """
     A trigger that will always match
     """
@@ -134,25 +124,24 @@
 
 class Text(BaseTrigger):
     """
     A trigger that will match an intent in a text message
     """
 
     def __init__(self, request: Request, intent: Intent):
-        super(Text, self).__init__(request)
+        super().__init__(request)
         self.intent = intent
 
     async def rank(self) -> Optional[float]:
         """
         If there is a text layer inside the request, try to find a matching
         text in the specified intent.
         """
-
         if not self.request.has_layer(l.RawText):
-            return
+            return None
 
         tl = self.request.get_layer(l.RawText)
         matcher = Matcher(
             [
                 tuple(Trigram(y) for y in x)
                 for x in await self.intent.strings(self.request)
             ]
@@ -169,16 +158,16 @@
 
     This trigger has two attributes: `slug` is the slug of choice made and
     `chosen` is the meta-info about this choice (text and intent).
 
     The optional `when` argument allows to limit matching to a single choice.
     """
 
-    def __init__(self, request: Request, when: Optional[TextT] = None):
-        super(Choice, self).__init__(request)
+    def __init__(self, request: Request, when: Optional[str] = None):
+        super().__init__(request)
         self.when = when
         self.slug = None
         self.chosen = None
 
     # noinspection PyUnresolvedReferences
     def _rank_qr(self, choices):
         """
@@ -196,15 +185,14 @@
         except KeyError:
             pass
 
     async def _rank_text(self, choices):
         """
         Try to match the TextLayer with choice's intents.
         """
-
         tl = self.request.get_layer(l.RawText)
         best = 0.0
 
         for slug, params in choices.items():
             strings = []
 
             if params["intent"]:
@@ -234,30 +222,30 @@
         - Otherwise, try to match each choice with its intent
         """
         from bernard.platforms.facebook import layers as fbl
 
         choices = self.request.get_trans_reg("choices")
 
         if not choices:
-            return
+            return None
 
         if self.request.has_layer(fbl.QuickReply):
             return self._rank_qr(choices)
         elif self.request.has_layer(l.RawText):
             return await self._rank_text(choices)
 
 
 class Action(BaseTrigger):
     """
     Triggered by "actions". An action is a postback message with a "action"
     field in its payload. This trigger simply matches actions on text.
     """
 
-    def __init__(self, request: Request, action: TextT):
-        super(Action, self).__init__(request)
+    def __init__(self, request: Request, action: str):
+        super().__init__(request)
         self.action = action
 
     # noinspection PyUnresolvedReferences
     def rank(self) -> Optional[float]:
         if self.request.has_layer(l.Postback):
             pb = self.request.get_layer(l.Postback)
 
@@ -270,59 +258,57 @@
 
 class Layer(BaseTrigger):
     """
     Gets triggered when the message contains a specific layer
     """
 
     def __init__(self, request: Request, layer_type: Type[l.BaseLayer]):
-        super(Layer, self).__init__(request)
+        super().__init__(request)
         self.layer_type = layer_type
 
     def rank(self) -> Optional[float]:
         """
         Simply test the presence of layer type
         """
-
         return 1.0 if self.request.has_layer(self.layer_type) else 0.0
 
 
 class BaseSlugTrigger(BaseTrigger):
     """
     Common type for slug-based classes that would have exactly the same code
     otherwise.
     """
 
     LAYER_TYPE = None
 
     def __init__(self, request: Request, slug: Optional[Text] = None):
-        super(BaseSlugTrigger, self).__init__(request)
+        super().__init__(request)
         self.slug = slug
 
     def rank(self) -> Optional[float]:
-        if self.request.has_layer(self.LAYER_TYPE):
-            if (
-                self.request.get_layer(self.LAYER_TYPE).slug == self.slug
-                or self.slug is None
-            ):
-                return 1.0
+        if self.request.has_layer(self.LAYER_TYPE) and (
+            self.request.get_layer(self.LAYER_TYPE).slug == self.slug
+            or self.slug is None
+        ):
+            return 1.0
 
 
 class Worst(BaseTrigger):
     """
     Run several triggers and only keep the worst one. Queries are not made
     in parallel, and execution stops when 0.0 is reached.
 
     This allows to put simple conditions first before doing more expensive
     tests.
     """
 
     def __init__(
         self, request: Request, triggers: List[Callable[[Request], "BaseTrigger"]]
     ):
-        super(Worst, self).__init__(request)
+        super().__init__(request)
         self.triggers = triggers
 
     async def rank(self):
         m = 1.0
 
         for t in self.triggers:
             r = await run_or_return(t(self.request).rank())
@@ -344,12 +330,40 @@
     def __init__(self, request: Request, layer: l.BaseLayer):
         super().__init__(request)
         self.layer = layer
 
     def rank(self):
         try:
             other = self.request.get_layer(self.layer.__class__)
-            assert self.layer == other
         except (KeyError, AssertionError):
             return 0.0
         else:
+            if self.layer == other:
+                return 1.0
+            else:
+                return 0.0
+
+
+class Command(BaseTrigger):
+    """
+    Gets triggered when the message contains a specific command
+    """
+
+    def __init__(self, request: Request, command: str):
+        super().__init__(request)
+        self.command = command
+        self.remainder = ""
+
+    def rank(self) -> Optional[float]:
+        """
+        Simply test the presence of a command
+        """
+        if not self.request.has_layer(l.RawText):
+            return 0.0
+
+        text = self.request.get_layer(l.RawText).text
+
+        if text.startswith(self.command):
+            self.remainder = text[len(self.command) :].strip()
             return 1.0
+        else:
+            return 0.0
```

### Comparing `bernard-0.6.0/src/bernard/i18n/_formatter.py` & `bernard-0.7.0/src/bernard/i18n/_formatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 import string
 from datetime import date, datetime, tzinfo
-from typing import Text, Union
+from typing import Union
 
 from babel import dates, numbers
 from dateutil.parser import parse as parse_date
 
 
-def make_date(obj: Union[date, datetime, Text], timezone: tzinfo = None):
+def make_date(obj: Union[date, datetime, str], timezone: tzinfo | None = None):
     """
     A flexible method to get a date object.
 
     It accepts either an ISO 8601 date/time string, either a Python `datetime`,
     either a Python `date`.
 
     If the input is a date/time and a timezone is specified, the resulting
     date object will be in the specified time zone.
     """
-
     if isinstance(obj, datetime):
         if hasattr(obj, "astimezone") and timezone:
             obj = obj.astimezone(timezone)
         return obj.date()
     elif isinstance(obj, date):
         return obj
     elif isinstance(obj, str):
         return make_date(parse_date(obj), timezone)
 
 
-def make_datetime(obj: Union[datetime, Text], timezone: tzinfo = None):
+def make_datetime(obj: Union[datetime, str], timezone: tzinfo | None = None):
     """
     A flexible method to get a date object.
 
     It accepts either an ISO 8601 date/time string, either a Python `datetime`,
     either a Python `date`.
 
     If the input is a date/time and a timezone is specified, the resulting
     date object will be in the specified time zone.
     """
-
     if isinstance(obj, datetime):
         if hasattr(obj, "astimezone") and timezone:
             obj = obj.astimezone(timezone)
         return obj
     elif isinstance(obj, str):
         return make_date(parse_date(obj), timezone)
 
@@ -84,18 +82,17 @@
         """
         return numbers.format_number(value, locale=self.lang)
 
     def format_field(self, value, spec):
         """
         Provide the additional formatters for localization.
         """
-
         if spec.startswith("date:"):
             _, format_ = spec.split(":", 1)
             return self.format_date(value, format_)
         elif spec.startswith("datetime:"):
             _, format_ = spec.split(":", 1)
             return self.format_datetime(value, format_)
         elif spec == "number":
             return self.format_number(value)
         else:
-            return super(I18nFormatter, self).format_field(value, spec)
+            return super().format_field(value, spec)
```

### Comparing `bernard-0.6.0/src/bernard/i18n/intents.py` & `bernard-0.7.0/src/bernard/i18n/intents.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,96 +1,108 @@
-# config: utf-8
-from typing import TYPE_CHECKING, List, Optional, Text, Tuple
+import asyncio
+import logging
+from typing import TYPE_CHECKING, List, Optional, Tuple
 
 from bernard.conf import settings
-from bernard.utils import import_class, run
+from bernard.utils import import_class
 
 from .loaders import BaseIntentsLoader, IntentDict
 from .utils import LocalesFlatDict
 
 if TYPE_CHECKING:
     from bernard.engine.request import Request
 
 
+logger = logging.getLogger(__name__)
+
+
 class IntentsDb(LocalesFlatDict):
     """
     Database of intents. In the future it will handle different langs but right
     now it only handles one.
     """
 
     def __init__(self):
-        super(IntentsDb, self).__init__()
-        self.loaders = []  # type: List[BaseIntentsLoader]
-        self._init_loaders()
+        super().__init__()
+        self.loaders: List[BaseIntentsLoader] = []
+        self._init_t = None
+
+    async def ensure_loaded(self):
+        if not self._init_t:
+            logger.info("Loading intents")
+            self._init_t = asyncio.get_running_loop().create_task(self._init_loaders())
 
-    def _init_loaders(self) -> None:
+        await self._init_t
+
+    async def _init_loaders(self) -> None:
         """
         Gets loaders from conf, make instances and subscribe to them.
         """
-
         for loader in settings.I18N_INTENTS_LOADERS:
             loader_class = import_class(loader["loader"])
             instance = loader_class()
             instance.on_update(self.update)
-            run(instance.load(**loader["params"]))
+            await instance.load(**loader["params"])
 
     def update(self, new_data: IntentDict):
         """
         Receive an update from the loaders.
         """
-
         for locale, data in new_data.items():
             if locale not in self.dict:
                 self.dict[locale] = {}
 
             self.dict[locale].update(data)
 
-    def get(self, key: Text, locale: Optional[Text]) -> List[Tuple[Text, ...]]:
+    async def get(self, key: str, locale: Optional[str]) -> List[Tuple[str, ...]]:
         """
         Get a single set of intents.
         """
+        await self.ensure_loaded()
 
         locale = self.choose_locale(locale)
+        logger.info("Getting intent %s for locale %s", key, locale)
 
         return self.dict[locale][key]
 
 
-class Intent(object):
+class Intent:
     """
     Represents an intent to be resolved later.
     """
 
-    def __init__(self, db: Optional[IntentsDb], key: Text):
+    def __init__(self, db: Optional[IntentsDb], key: str):
         self.db = db
         self.key = key
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.key == other.key
 
     def __repr__(self):
-        return "Intent({})".format(repr(self.key))
+        return f"Intent({self.key!r})"
 
     # noinspection PyUnusedLocal
     async def strings(
         self, request: Optional["Request"] = None
-    ) -> List[Tuple[Text, ...]]:
+    ) -> List[Tuple[str, ...]]:
         """
         For the given request, find the list of strings of that intent. If the
         intent does not exist, it will raise a KeyError.
         """
+        await self.db.ensure_loaded()
 
         if request:
             locale = await request.get_locale()
         else:
             locale = None
 
-        return self.db.get(self.key, locale)
+        return await self.db.get(self.key, locale)
 
 
-class IntentsMaker(object):
+class IntentsMaker:
     """
     Utility class to be used as singleton and produce Intents objects easily
     from anywhere in the code.
     """
 
     def __init__(self, db: IntentsDb = None):
         self.db = db
@@ -98,19 +110,17 @@
         if not self.db:
             self._refresh_intents_db()
 
     def _refresh_intents_db(self):
         """
         Re-read the config and re-generate the intents DB.
         """
-
         self.db = IntentsDb()
 
-    def __getattr__(self, key: Text) -> Intent:
+    def __getattr__(self, key: str) -> Intent:
         """
         Generate an intent. Use it this way:
 
         >>> i = IntentsMaker()
         >>> print(await i.FOO.strings())
         """
-
         return Intent(self.db, key)
```

### Comparing `bernard-0.6.0/src/bernard/i18n/translator.py` & `bernard-0.7.0/src/bernard/i18n/translator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,41 @@
+import asyncio
+import logging
 from collections import defaultdict
 from itertools import zip_longest
 from random import SystemRandom
 from string import Formatter
 from typing import (
     TYPE_CHECKING,
     Any,
     Dict,
     List,
     Mapping,
     NamedTuple,
     Optional,
-    Text,
     Tuple,
     Union,
 )
 
 from bernard.conf import settings
-from bernard.i18n.loaders import TransDict
-from bernard.utils import import_class, run
+from bernard.i18n.loaders import BaseTranslationLoader, TransDict
+from bernard.utils import import_class
 
 from ._formatter import I18nFormatter
-from .loaders import BaseTranslationLoader
 from .utils import LocalesDict
 
 if TYPE_CHECKING:
     from bernard.engine.request import Request
 
 
 random = SystemRandom()
+logger = logging.getLogger(__name__)
 
 
-Flags = Dict[Text, Text]
+Flags = Dict[str, str]
 
 
 class TranslationError(Exception):
     """
     That is the base translation error class
     """
 
@@ -49,77 +50,75 @@
     """
     Raised if a translation needs parameters that can't be found
     """
 
 
 class TransItem(NamedTuple):
     """
-    This is a single "item of translation". Typically it comes from the CSV.
+    This is a single "item of translation". Typically, it comes from the CSV.
 
     It's a de-normalized representation of translations. There is 3 properties
-    today but it might become more in the future.
+    today, but it might become more in the future.
 
     - `key` is the translation key
-    - `index` is the number of the message in case you're doing a multi-part
+    - `index` is the number of the message in case you're doing a multipart
       message (from 1 to the infinite)
     - `value` is the raw text value
     - `flags` are key/values that will be compared to the translation context
       for the current request. Translations will be chosen between items of
       equal flag "score".
     """
 
-    key: Text
+    key: str
     index: int
-    value: Text
+    value: str
     flags: Flags
 
     def score(self, flags: Flags) -> int:
         """
         Counts how many of the flags can be matched
         """
-
         score = 0
 
         for k, v in flags.items():
             if self.flags.get(k) == v:
                 score += 1
 
         return score
 
 
-class Sentence(object):
+class Sentence:
     """
     A single sentence. The main goal of this class is to provide an easy way to
     get a random sentence from the list and to see if the list is valid.
     """
 
     def __init__(self):
         self.items: List[TransItem] = []
 
     def best_for_flags(self, flags: Flags) -> List[TransItem]:
         """
         Given `flags`, find all items of this sentence that have an equal
         matching score and put them in a list.
         """
-
         best_score: int = 0
         best_list: List[TransItem] = []
 
         for item in self.items:
             score = item.score(flags)
 
             if score == best_score:
                 best_list.append(item)
             elif score > best_score:
                 best_list = [item]
                 best_score = score
 
         return best_list
 
-    def render(self, flags: Flags) -> Text:
+    def render(self, flags: Flags) -> str:
         """
         Chooses a random sentence from the list and returns it.
         """
         return random.choice(self.best_for_flags(flags)).value
 
     def append(self, item: TransItem):
         """
@@ -135,50 +134,48 @@
         return bool(self.items)
 
     def update(self, new: "Sentence", flags: Flags):
         """
         Erase items with the specified flags and insert the new items from
         the other sentence instead.
         """
-
         items = [i for i in self.items if i.flags != flags]
         items.extend(new.items)
         self.items = items
 
 
-class SentenceGroup(object):
+class SentenceGroup:
     """
     That's a group of sentences, aka a "step" in a conversation that might get
     split into several messages at the will of the translator.
 
     It will automatically group items into sentences of the same index, however
     you need at least one item for each sentence. In other words, if you try
     to add FOO+1 and FOO+3 it won't work.
 
     Order of insertion does not matter.
     """
 
     def __init__(self):
         self.sentences: List[Sentence] = []
 
-    def render(self, flags: Flags) -> List[Text]:
+    def render(self, flags: Flags) -> List[str]:
         """
         Returns a list of randomly chosen outcomes for each sentence of the
         list.
         """
         return [x.render(flags) for x in self.sentences]
 
     def append(self, item: TransItem):
         """
         Append an item to the list. If there is not enough sentences in the
         list, then the list is extended as needed.
 
         There is no control made to make sure that the key is consistent.
         """
-
         if not (1 <= item.index <= settings.I18N_MAX_SENTENCES_PER_GROUP):
             return
 
         if len(self.sentences) < item.index:
             for _ in range(len(self.sentences), item.index):
                 self.sentences.append(Sentence())
 
@@ -189,15 +186,14 @@
 
     def update(self, group: "SentenceGroup", flags: Flags) -> None:
         """
         This object is considered to be a "global" sentence group while the
         other one is flags-specific. All data related to the specified flags
         will be overwritten by the content of the specified group.
         """
-
         to_append = []
 
         for old, new in zip_longest(self.sentences, group.sentences):
             if old is None:
                 old = Sentence()
                 to_append.append(old)
 
@@ -205,101 +201,103 @@
                 new = Sentence()
 
             old.update(new, flags)
 
         self.sentences.extend(to_append)
 
 
-class SortingDict(object):
+class SortingDict:
     """
     A validating and sorting dictionary for translation items. The intended use
     is to append all your values to it and then to extract it to get only the
     valid keys out. Then you can discard this object.
     """
 
     def __init__(self):
-        self.data: Dict[Text, SentenceGroup] = defaultdict(lambda: SentenceGroup())
+        self.data: Dict[str, SentenceGroup] = defaultdict(lambda: SentenceGroup())
 
     def extract(self):
         """
         Extract only the valid sentence groups into a dictionary.
         """
-
         out = {}
 
         for key, group in self.data.items():
             out[key] = group
 
         return out
 
     def append(self, item: TransItem):
         """
         Append an item to the internal dictionary.
         """
-
         self.data[item.key].append(item)
 
 
 class WordDictionary(LocalesDict):
     """
     That's where the actual translation happens. It stores all translations in
     memory, puts the parameters in place and so on.
     """
 
     def __init__(self):
-        super(WordDictionary, self).__init__()
-        self.loaders = []  # type: List[BaseTranslationLoader]
-        self._init_loaders()
+        super().__init__()
+        self.loaders: list[BaseTranslationLoader] = []
+        self._init_t = None
+
+    async def ensure_loaded(self):
+        if not self._init_t:
+            logger.info("Loading translations")
+            self._init_t = asyncio.get_running_loop().create_task(self._init_loaders())
 
-    def _init_loaders(self) -> None:
+        await self._init_t
+
+    async def _init_loaders(self) -> None:
         """
         This creates the loaders instances and subscribes to their updates.
         """
-
         for loader in settings.I18N_TRANSLATION_LOADERS:
             loader_class = import_class(loader["loader"])
             instance = loader_class()
             instance.on_update(self.update)
-            run(instance.load(**loader["params"]))
+            await instance.load(**loader["params"])
 
     def parse_item(self, key, value, flags: Flags) -> Optional[TransItem]:
         """
         Parse an item (and more specifically its key).
         """
-
         parts = key.split("+")
         pure_key = parts[0]
 
         try:
             if len(parts) == 2:
                 index = int(parts[1])
             elif len(parts) > 2:
-                return
+                return None
             else:
                 index = 1
         except (ValueError, TypeError):
-            return
+            return None
 
         if index < 1:
-            return
+            return None
 
         return TransItem(
             key=pure_key,
             index=index,
             value=value,
             flags=flags,
         )
 
     def update_lang(
-        self, lang: Optional[Text], data: List[Tuple[Text, Text]], flags: Flags
+        self, lang: Optional[str], data: List[Tuple[str, str]], flags: Flags
     ):
         """
         Update translations for one specific lang
         """
-
         sd = SortingDict()
 
         for item in (self.parse_item(x[0], x[1], flags) for x in data):
             if item:
                 sd.append(item)
 
         if lang not in self.dict:
@@ -313,82 +311,83 @@
 
             d[k].update(v, flags)
 
     def update(self, data: TransDict, flags: Flags):
         """
         Update all langs at once
         """
-
         for lang, lang_data in data.items():
             self.update_lang(lang, lang_data, flags)
 
-    def get(
+    async def get(
         self,
-        key: Text,
+        key: str,
         count: Optional[int] = None,
-        formatter: Formatter = None,
-        locale: Text = None,
-        params: Optional[Dict[Text, Any]] = None,
+        formatter: Formatter | None = None,
+        locale: str | None = None,
+        params: Optional[Dict[str, Any]] = None,
         flags: Optional[Flags] = None,
-    ) -> List[Text]:
+    ) -> List[str]:
         """
         Get the appropriate translation given the specified parameters.
 
         :param key: Translation key
         :param count: Count for plurals
         :param formatter: Optional string formatter to use
-        :param locale: Prefered locale to get the string from
+        :param locale: Preferred locale to get the string from
         :param params: Params to be substituted
         :param flags: Flags to help choosing one version or the other
         """
-
         if params is None:
             params = {}
 
         if count is not None:
-            raise TranslationError("Count parameter is not supported yet")
+            msg = "Count parameter is not supported yet"
+            raise TranslationError(msg)
+
+        await self.ensure_loaded()
 
         locale = self.choose_locale(locale)
 
         try:
             group: SentenceGroup = self.dict[locale][key]
         except KeyError:
-            raise MissingTranslationError('Translation "{}" does not exist'.format(key))
+            msg = f'Translation "{key}" does not exist'
+            raise MissingTranslationError(msg) from None
 
         try:
             trans = group.render(flags or {})
             out = []
 
             for line in trans:
                 if not formatter:
                     out.append(line.format(**params))
                 else:
                     out.append(formatter.format(line, **params))
         except KeyError as e:
-            raise MissingParamError(
-                'Parameter "{}" missing to translate "{}"'.format(e.args[0], key)
-            )
+            msg = f'Parameter "{e.args[0]}" missing to translate "{key}"'
+            raise MissingParamError(msg) from None
         else:
             return out
 
 
-class StringToTranslate(object):
+class StringToTranslate:
     """
     That's a string to translate. It holds the parameters until it gets
     rendered.
     """
 
     LINE_SEPARATOR = "\n"
 
     def __init__(
         self,
         wd: WordDictionary,
-        key: Text,
-        count: Optional[int] = None,
-        params: Dict[Text, Any] = None,
+        key: str,
+        count: int | None = None,
+        params: dict[str, Any] | None = None,
     ):
         if params is None:
             params = {}
 
         self.wd = wd
         self.key = key
         self.count = count
@@ -405,26 +404,25 @@
     def __repr__(self):
         parts = [repr(self.key)]
 
         if self.count is not None:
             parts.append(repr(self.count))
 
         for k, v in self.params.items():
-            parts.append("{}={}".format(k, repr(v)))
+            parts.append(f"{k}={v!r}")
 
         return "t({})".format(", ".join(parts))
 
     async def _resolve_params(
-        self, params: Dict[Text, Any], request: Optional["Request"]
+        self, params: Dict[str, Any], request: Optional["Request"]
     ):
         """
         If any StringToTranslate was passed as parameter then it is rendered
         at this moment.
         """
-
         out = {}
 
         for k, v in params.items():
             if isinstance(v, StringToTranslate):
                 out[k] = await render(v, request)
             else:
                 out[k] = v
@@ -435,27 +433,28 @@
         """
         Render the translation for the specified request. If no request is
         specified, do as good as possible.
 
         :param request: Bot request. No one knows what it's going to look like
                         so far.
         """
-
         return self.LINE_SEPARATOR.join(await self.render_list(request))
 
     # noinspection PyUnusedLocal
-    async def render_list(self, request=None) -> List[Text]:
+    async def render_list(self, request=None) -> List[str]:
         """
         Render the translation as a list if there is multiple strings for this
         single key.
 
         :param request: Bot request.
         """
         from bernard.middleware import MiddlewareManager
 
+        await self.wd.ensure_loaded()
+
         if request:
             tz = await request.user.get_timezone()
             locale = await request.get_locale()
             flags = await request.get_trans_flags()
         else:
             tz = None
             locale = self.wd.list_locales()[0]
@@ -464,143 +463,143 @@
         rp = MiddlewareManager.instance().get(
             "resolve_trans_params", self._resolve_params
         )
 
         resolved_params = await rp(self.params, request)
 
         f = I18nFormatter(self.wd.choose_locale(locale), tz)
-        return self.wd.get(
+        return await self.wd.get(
             self.key,
             self.count,
             f,
             locale,
             resolved_params,
             flags,
         )
 
 
-class Translator(object):
+class Translator:
     """
     That's the basic object that you use to produce translations.
     """
 
     def __init__(self, wd: Optional[WordDictionary] = None):
         """
         We need the word dictionary here in order to pass it to the string to
         translate when it will get rendered.
 
         :param wd: a configured WordDictionary
         """
-
         self.wd = wd  # type: WordDictionary
 
         if not self.wd:
             self._regenerate_word_dict()
 
     def _regenerate_word_dict(self):
         """
         Re-generate the word dict, if you need to.
         """
-
         self.wd = WordDictionary()
 
-    def __getattr__(self, key: Text) -> StringToTranslate:
+    def __getattr__(self, key: str) -> StringToTranslate:
         """
         Allow the `t.FOO` style.
 
         :param key: Key to get
         """
-
         return self(key)
 
     def __call__(
-        self, key: Text, count: Optional[int] = None, **params
+        self, key: str, count: Optional[int] = None, **params
     ) -> StringToTranslate:
         """
         Allow the `t('FOO')` style.
 
         :param key: Key to translate
         :param count: Count for plurals
         :param params: Params to substitute
         """
-
         return StringToTranslate(self.wd, key, count, params)
 
 
-TransText = Union[StringToTranslate, Text]
+TransText = Union[StringToTranslate, str]
 
 
 def serialize(text: TransText):
     """
     Takes as input either a string to translate either an actual string and
     transforms it into a JSON-serializable structure that can be reconstructed
     using `unserialize()`.
     """
-
     if isinstance(text, str):
         return {
             "type": "string",
             "value": text,
         }
     elif isinstance(text, StringToTranslate):
         return {
             "type": "trans",
             "key": text.key,
             "count": text.count,
             "params": text.params,
         }
     else:
-        raise ValueError('Cannot accept type "{}"'.format(text.__class__.__name__))
+        msg = f'Cannot accept type "{text.__class__.__name__}"'
+        raise ValueError(msg)
 
 
 def unserialize(wd: WordDictionary, text: Dict):
     """
     Transforms back a serialized value of `serialize()`
     """
-
     if not isinstance(text, Mapping):
-        raise ValueError("Text has not the right format")
+        msg = "Text has not the right format"
+        raise ValueError(msg)
 
     try:
         t = text["type"]
 
         if t == "string":
             return text["value"]
         elif t == "trans":
             if not isinstance(text["params"], Mapping):
-                raise ValueError("Params should be a dictionary")
+                msg = "Params should be a dictionary"
+                raise ValueError(msg)
 
             for param in text["params"]:
                 if not isinstance(param, str):
-                    raise ValueError("Params are not all text-keys")
+                    msg = "Params are not all text-keys"
+                    raise ValueError(msg)
 
             return StringToTranslate(
                 wd=wd,
                 key=text["key"],
                 count=text["count"],
                 params=text["params"],
             )
         else:
-            raise ValueError('Unknown type "{}"'.format(t))
+            msg = f'Unknown type "{t}"'
+            raise ValueError(msg)
     except KeyError:
-        raise ValueError("Not enough information to unserialize")
+        msg = "Not enough information to unserialize"
+        raise ValueError(msg) from None
 
 
 async def render(
     text: TransText, request: Optional["Request"], multi_line=False
-) -> Union[Text, List[Text]]:
+) -> Union[str, List[str]]:
     """
     Render either a normal string either a string to translate into an actual
     string for the specified request.
     """
-
     if isinstance(text, str):
         out = [text]
     elif isinstance(text, StringToTranslate):
         out = await text.render_list(request)
     else:
-        raise TypeError("Provided text cannot be rendered")
+        msg = "Provided text cannot be rendered"
+        raise TypeError(msg)
 
     if multi_line:
         return out
     else:
         return " ".join(out)
```

### Comparing `bernard-0.6.0/src/bernard/i18n/utils.py` & `bernard-0.7.0/src/bernard/i18n/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import re
 from collections import OrderedDict
-from typing import Dict, List, Optional, Text, Tuple
+from typing import Dict, List, Optional, Tuple
 
 
-def split_locale(locale: Text) -> Tuple[Text, Optional[Text]]:
+def split_locale(locale: str) -> Tuple[str, Optional[str]]:
     """
     Decompose the locale into a normalized tuple.
 
     The first item is the locale (as lowercase letters) while the second item
     is either the country as lower case either None if no country was supplied.
     """
-
-    items = re.split(r"[_\-]", locale.lower(), 1)
+    items = re.split(r"[_\-]", locale.lower(), maxsplit=1)
 
     try:
         return items[0], items[1]
     except IndexError:
         return items[0], None
 
 
@@ -23,15 +22,14 @@
     """
     Compares two locales to find the level of compatibility
 
     :param a: First locale
     :param b: Second locale
     :return: 2 full match, 1 lang match, 0 no match
     """
-
     if a is None or b is None:
         if a == b:
             return 2
         else:
             return 0
 
     a = split_locale(a)
@@ -41,41 +39,39 @@
         return 2
     elif a[0] == b[0]:
         return 1
     else:
         return 0
 
 
-class LocalesDict(object):
+class LocalesDict:
     def __init__(self):
         self.dict = OrderedDict()
         self._choice_cache = {}
 
-    def list_locales(self) -> List[Optional[Text]]:
+    def list_locales(self) -> List[Optional[str]]:
         """
         Returns the list of available locales. The first locale is the default
         locale to be used. If no locales are known, then `None` will be the
         first item.
         """
-
         locales = list(self.dict.keys())
 
         if not locales:
             locales.append(None)
 
         return locales
 
-    def choose_locale(self, locale: Text) -> Text:
+    def choose_locale(self, locale: str) -> str:
         """
         Returns the best matching locale in what is available.
 
         :param locale: Locale to match
         :return: Locale to use
         """
-
         if locale not in self._choice_cache:
             locales = self.list_locales()
 
             best_choice = locales[0]
             best_level = 0
 
             for candidate in locales:
@@ -94,19 +90,18 @@
     """
     That used to be in LocalesDict but the children diverged and now this
     method is alone. It could have gone directly into the intents loader but
     it feels like it'll have to go outside again, so for now it stays in this
     class.
     """
 
-    def update(self, new_data: Dict[Text, Dict[Text, Text]]):
+    def update(self, new_data: Dict[str, Dict[str, str]]):
         """
         Receive an update from a loader.
 
         :param new_data: New translation data from the loader
         """
-
         for locale, data in new_data.items():
             if locale not in self.dict:
                 self.dict[locale] = {}
 
             self.dict[locale].update(data)
```

### Comparing `bernard-0.6.0/src/bernard/layers/definitions.py` & `bernard-0.7.0/src/bernard/layers/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from typing import TYPE_CHECKING, Dict, NamedTuple, Optional
-from typing import Text as TextT
-from typing import Type, TypeVar
+from typing import TYPE_CHECKING, Dict, NamedTuple, Type, TypeVar
 
 from bernard.i18n import TransText, render
 
 if TYPE_CHECKING:
     from bernard.engine.platform import Platform
     from bernard.engine.request import BaseMessage, Request
 
 
 L = TypeVar("L")
 
 
-class BaseLayer(object):
+class BaseLayer:
     def __eq__(self, other):
         raise NotImplementedError
 
     def __repr__(self):
         return "{}({})".format(
             self.__class__.__name__,
             ",".join(repr(x) for x in self._repr_arguments()),
@@ -26,15 +24,15 @@
         raise NotImplementedError
 
     async def patch_register(self, register: Dict, request: "Request") -> Dict:
         """
         If you want to put a value in the transition register, you can overload
         this function and patch the provided register.
 
-        Keys match different operations. By example, for quick replies:
+        Keys match different operations. For example, for quick replies:
 
         >>> {
         >>>     'choices': {
         >>>         'yes': {
         >>>             'intents': 'YES',
         >>>         },
         >>>         'no': {
@@ -47,30 +45,29 @@
         for this register.
 
         This function will be called in the order of layers. The implementation
         can choose to add information to what previous layers inserted or to
         overwrite it completely. That is why the previous output is provided
         as argument.
         """
-
         return register
 
     def can_become(self):
         """
         This indicates other layer classes that you can transform this layer
         into from a request.
         """
         return []
 
     async def become(self, layer_type: Type[L], request: "Request") -> L:
         """
         Transform this layer into another layer type
         """
-
-        raise ValueError('Cannot become "{}"'.format(layer_type.__name__))
+        msg = f'Cannot become "{layer_type.__name__}"'
+        raise ValueError(msg)
 
     async def convert_media(self, platform: "Platform") -> None:
         """
         Convert this layer's media if needed
         """
         pass
 
@@ -97,15 +94,15 @@
 
     async def become(self, layer_type: Type[L], request: "Request"):
         """
         Transforms the translatable string into an actual string and put it
         inside a RawText.
         """
         if layer_type != RawText:
-            super(Text, self).become(layer_type, request)
+            await super().become(layer_type, request)
 
         return RawText(await render(self.text, request))
 
 
 class MultiText(Text):
     """
     That's exactly like a Text layer but which can output several messages at
@@ -114,30 +111,30 @@
 
 
 class RawText(BaseLayer):
     """
     That is a text message that warranties it will never have to be translated.
     """
 
-    def __init__(self, text: TextT):
+    def __init__(self, text: str):
         self.text = text
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.text == other.text
 
     def _repr_arguments(self):
         return [self.text]
 
 
 class Markdown(BaseLayer):
     """
     Like the Text but for Markdown.
     """
 
-    def __init__(self, text: TextT):
+    def __init__(self, text: str):
         self.text = text
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.text == other.text
 
     def _repr_arguments(self):
         if len(self.text) > 15:
@@ -259,15 +256,15 @@
     def __init__(self, message: "BaseMessage"):
         from bernard.layers import Stack
 
         self.message = message
         self.stack: Stack = Stack(message.get_layers())
 
     def _repr_arguments(self):
-        return [x for x in self.stack.layers]
+        return list(self.stack.layers)
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.stack == other.stack
 
 
 class Typing(BaseLayer):
     """
```

### Comparing `bernard-0.6.0/src/bernard/layers/stack.py` & `bernard-0.7.0/src/bernard/layers/stack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import TYPE_CHECKING, Dict, List, Text, Type, TypeVar
+from typing import TYPE_CHECKING, Dict, List, Type, TypeVar
 
 from bernard.utils import ClassExp, RoList
 
 from .definitions import BaseLayer
 
 if TYPE_CHECKING:
     from bernard.engine.platform import Platform
     from bernard.engine.request import Request
 
 
 L = TypeVar("L")
 
 
-class Stack(object):
+class Stack:
     """
     The stack holds several layers and allows quick access to specific content.
     This is useful by example for transitions to check if they have anything
     interesting to find.
 
     This stack has a .layers attribute that you can read to get the list of
     layers. However, if you want to change that list, you must set it all at
@@ -61,52 +61,49 @@
         self._transformed = {}
 
     def _make_index(self):
         """
         Perform the index computation. It groups layers by type into a
         dictionary, to allow quick access.
         """
-
         out = {}
 
         for layer in self._layers:
             cls = layer.__class__
-            out[cls] = out.get(cls, []) + [layer]
+            out[cls] = [*out.get(cls, []), layer]
 
         return out
 
     async def transform(self, request):
         out = {}
 
         for layer in self._layers:  # type: BaseLayer
             for become in layer.can_become():
                 b_layer = await layer.become(become, request)
-                out[become] = out.get(become, []) + [b_layer]
+                out[become] = [*out.get(become, []), b_layer]
 
         self._transformed = out
 
     def has_layer(self, class_: Type[L], became: bool = True) -> bool:
         """
         Test the presence of a given layer type.
 
         :param class_: Layer class you're interested in.
         :param became: Allow transformed layers in results
         """
-
         return class_ in self._index or (became and class_ in self._transformed)
 
     def get_layer(self, class_: Type[L], became: bool = True) -> L:
         """
         Return the first layer of a given class. If that layer is not present,
         then raise a KeyError.
 
         :param class_: class of the expected layer
         :param became: Allow transformed layers in results
         """
-
         try:
             return self._index[class_][0]
         except KeyError:
             if became:
                 return self._transformed[class_][0]
             else:
                 raise
@@ -115,38 +112,36 @@
         """
         Returns the list of layers of a given class. If no layers are present
         then the list will be empty.
 
         :param class_: class of the expected layers
         :param became: Allow transformed layers in results
         """
-
         out = self._index.get(class_, [])
 
         if became:
             out += self._transformed.get(class_, [])
 
         return out
 
-    def describe(self) -> Text:
+    def describe(self) -> str:
         return ", ".join(s.__class__.__name__ for s in self._layers)
 
     async def patch_register(self, register: Dict, request: "Request"):
         for layer in self._layers:  # type: BaseLayer
             register = await layer.patch_register(register, request)
         return register
 
-    def match_exp(self, expression: Text):
+    def match_exp(self, expression: str):
         e = ClassExp(expression)
         return e.match(self._layers)
 
     async def convert_media(self, platform: "Platform") -> None:
         """
         Polls all the layers to convert the media inside.
         """
-
         for layer in self.layers:
             await layer.convert_media(platform)
 
 
 def stack(*layers: BaseLayer):
     return Stack(list(layers))
```

### Comparing `bernard-0.6.0/src/bernard/media/base.py` & `bernard-0.7.0/src/bernard/media/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-class BaseMedia(object):
+class BaseMedia:
     """
     Different platforms have different ways of representing medias. The goal
     of this object is to provide a way to know which platform the media came
     from and a way to convert it into a media that can be sent to another
     platform.
     """
 
@@ -22,8 +22,8 @@
     def __init__(self, url):
         self.url = url
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.url == other.url
 
     def __repr__(self):
-        return "UrlMedia({})".format(repr(self.url))
+        return f"UrlMedia({self.url!r})"
```

### Comparing `bernard-0.6.0/src/bernard/middleware/_builtins.py` & `bernard-0.7.0/src/bernard/middleware/_builtins.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,66 @@
 import re
 from typing import TYPE_CHECKING, List
-from typing import Text as TextT
 
 from bernard import layers as lyr
 from bernard.conf import settings
 from bernard.engine.request import Request
 from bernard.i18n import render
 from bernard.layers import BaseLayer, Stack
 
 if TYPE_CHECKING:
     from bernard.engine.responder import Responder
 
 
-class BaseMiddleware(object):
+class BaseMiddleware:
     """
     Base class for middlewares. It's just useful to get the `self.next`
     automatically.
     """
 
     def __init__(self, next_):
         self.next = next_
 
 
 class AutoSleep(BaseMiddleware):
     """
-    Automatically add sleep between text messages so the user has some time to
+    Automatically add sleep between text messages so the user has some time
     to read.
     """
 
     async def flush(self, request: Request, stacks: List[Stack]):
         """
         For all stacks to be sent, append a pause after each text layer.
         """
-
         ns = await self.expand_stacks(request, stacks)
         ns = self.split_stacks(ns)
         ns = self.clean_stacks(ns)
 
         await self.next(request, [Stack(x) for x in ns])
 
     async def expand_stacks(self, request: Request, stacks: List[Stack]):
         ns = []
 
         for stack in stacks:
             s = []
 
             for layer in stack.layers:
                 async for sub_layer in self.expand(request, layer):
-                    s.append(sub_layer)
+                    s.append(sub_layer)  # noqa: PERF402
 
             ns.append(s)
 
         return ns
 
     def split_stacks(self, stacks: List[List[BaseLayer]]) -> List[List[BaseLayer]]:
         """
         First step of the stacks cleanup process. We consider that if inside
         a stack there's a text layer showing up then it's the beginning of a
         new stack and split upon that.
         """
-
         ns: List[List[BaseLayer]] = []
 
         for stack in stacks:
             cur: List[BaseLayer] = []
 
             for layer in stack:
                 if cur and isinstance(layer, lyr.RawText):
@@ -76,19 +73,18 @@
                 ns.append(cur)
 
         return ns
 
     def clean_stacks(self, stacks: List[List[BaseLayer]]) -> List[List[BaseLayer]]:
         """
         Two cases: if a stack finishes by a sleep then let's keep it (it means
-        that there was nothing after the text). However if the stack finishes
+        that there was nothing after the text). However, if the stack finishes
         with something else (like a quick reply) then we don't risk an
         is preserved.
         """
-
         ns: List[List[BaseLayer]] = []
 
         for stack in stacks:
             if isinstance(stack[-1], lyr.Sleep):
                 ns.extend([x] for x in stack)
             else:
                 ns.append([x for x in stack if not isinstance(x, lyr.Sleep)])
@@ -102,15 +98,14 @@
         else:
             return ns
 
     async def expand(self, request: Request, layer: BaseLayer):
         """
         Expand a layer into a list of layers including the pauses.
         """
-
         if isinstance(layer, lyr.RawText):
             t = self.reading_time(layer.text)
             yield layer
             yield lyr.Sleep(t)
 
         elif isinstance(layer, lyr.MultiText):
             texts = await render(layer.text, request, True)
@@ -125,20 +120,19 @@
             t = self.reading_time(text)
             yield lyr.RawText(text)
             yield lyr.Sleep(t)
 
         else:
             yield layer
 
-    def reading_time(self, text: TextT):
+    def reading_time(self, text: str):
         """
         Computes the time in seconds that the user will need to read a bubble
         containing the text passed as parameter.
         """
-
         wc = re.findall(r"\w+", text)
         period = 60.0 / settings.USERS_READING_SPEED
         return float(len(wc)) * period + settings.USERS_READING_BUBBLE_START
 
 
 class AutoType(BaseMiddleware):
     """
@@ -146,39 +140,36 @@
     the last message.
     """
 
     async def flush(self, request: Request, stacks: List[Stack]):
         """
         Add a typing stack after each stack.
         """
-
         ns: List[Stack] = []
 
         for stack in stacks:
             ns.extend(self.typify(stack))
 
         if len(ns) > 1 and ns[-1] == Stack([lyr.Typing()]):
             ns[-1].get_layer(lyr.Typing).active = False
 
         await self.next(request, ns)
 
     async def pre_handle(self, request: Request, responder: "Responder"):
         """
         Start typing right when the message is received.
         """
-
         responder.send([lyr.Typing()])
         await responder.flush(request)
         responder.clear()
 
         await self.next(request, responder)
 
     def typify(self, stack: Stack) -> List[Stack]:
         """
         Appends a typing stack after the given stack, but only if required
         (aka don't have two typing layers following each other).
         """
-
         if len(stack.layers) == 1 and isinstance(stack.layers[0], lyr.Typing):
             return [stack]
 
         return [stack, Stack([lyr.Typing()])]
```

### Comparing `bernard-0.6.0/src/bernard/middleware/_manager.py` & `bernard-0.7.0/src/bernard/middleware/_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,93 +1,89 @@
-from typing import Callable, List, Text, Type, TypeVar
+import contextlib
+from typing import Callable, List, Type, TypeVar
 
 from bernard.conf import settings
 from bernard.core.health_check import HealthCheckFail
 from bernard.utils import import_class
 
 from ._builtins import BaseMiddleware
 
 C = TypeVar("C")
 
 
-class Caller(object):
+class Caller:
     """
     This object allows to create functions which can call each other
     recursively without knowing in advance the list of functions to call.
 
     It's useful to stack middlewares.
     """
 
     def __init__(
-        self, manager: "MiddlewareManager", name: Text, final: Callable
+        self, manager: "MiddlewareManager", name: str, final: Callable
     ) -> None:
         """
         Save attributes and generate the proper stack of calls.
 
         `manager` is the middleware manager from which the stack is built
         `name` is the name of the function to call
         `final` is the final function to call, which will end the recursion
         """
-
         self.manager = manager
         self.name = name
         self.final = final
         self._stack = self._build_stack()
         self._pos = 0
         self._complete = False
 
     def _build_stack(self) -> List[Callable]:
         """
         Generates the stack of functions to call. It looks at the ordered list
         of all middlewares and only keeps those which have the method we're
         trying to call.
         """
-
         stack = []
 
         for m in self.manager.middlewares:
-            try:
+            with contextlib.suppress(AttributeError):
                 stack.append(getattr(m(self), self.name))
-            except AttributeError:
-                pass
 
         return stack
 
     async def __call__(self, *args, **kwargs):
         """
         Calls the next function in the stack.
         """
-
         if self._pos == 0:
             is_root = True
         else:
             is_root = False
 
         if self._pos < len(self._stack):
             func = self._stack[self._pos]
             self._pos += 1
             out = await func(*args, **kwargs)
         elif self._pos == len(self._stack):
             self._pos += 1
             out = await self.final(*args, **kwargs)
             self._complete = True
         else:
-            raise ValueError("A caller cannot be called twice")
+            msg = "A caller cannot be called twice"
+            raise ValueError(msg)
 
         if is_root and not self._complete:
             # noinspection PyUnresolvedReferences
             faulty = self._stack[self._pos - 1].__qualname__
-            raise TypeError(
-                f'"{faulty}" did not call `self.next()`, or ' f"forgot to await it"
-            )
+            msg = f'"{faulty}" did not call `self.next()`, or ' f"forgot to await it"
+            raise TypeError(msg)
 
         return out
 
 
-class MiddlewareManager(object):
+class MiddlewareManager:
     """
     Manages the middlewares and allows to run them.
 
     Typical use:
 
     >>> async def do_something(x):
     >>>     return x + 1
@@ -98,38 +94,34 @@
 
     _instance = None
 
     def __init__(self):
         """
         Don't call directly, use `instance()` instead.
         """
-
-        self._middlewares_classes: List[Text] = settings.MIDDLEWARES
+        self._middlewares_classes: List[str] = settings.MIDDLEWARES
         self.middlewares: List[Type[BaseMiddleware]] = []
 
     @classmethod
     def instance(cls) -> "MiddlewareManager":
         """
         Creates, initializes and returns a unique MiddlewareManager instance.
         """
-
         if cls._instance is None:
             cls._instance = cls()
             cls._instance.init()
         return cls._instance
 
     @classmethod
     def health_check(cls):
         """
         Checks that the configuration makes sense.
         """
 
-        try:
-            assert isinstance(settings.MIDDLEWARES, list)
-        except AssertionError:
+        if not isinstance(settings.MIDDLEWARES, list):
             yield HealthCheckFail(
                 "00005",
                 'The "MIDDLEWARES" configuration key should be assigned ' "to a list",
             )
             return
 
         for m in settings.MIDDLEWARES:
@@ -147,22 +139,20 @@
                         f'Middleware "{m}" does not implement ' f'"BaseMiddleware"',
                     )
 
     def init(self):
         """
         Imports and caches all middleware classes.
         """
-
         self.middlewares = [import_class(c) for c in self._middlewares_classes]
 
-    def get(self, name: Text, final: C) -> C:
+    def get(self, name: str, final: C) -> C:
         """
         Get the function to call which will run all middlewares.
 
         :param name: Name of the function to be called
         :param final: Function to call at the bottom of the stack (that's the
                       one provided by the implementer).
         :return:
         """
-
         # noinspection PyTypeChecker
         return Caller(self, name, final)
```

### Comparing `bernard-0.6.0/src/bernard/misc/start_project/_base.py` & `bernard-0.7.0/src/bernard/misc/start_project/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,158 +1,147 @@
 import re
-from os import chmod, makedirs, path, scandir, walk
+from pathlib import Path
 from random import SystemRandom
 from sys import stderr
-from typing import Text
 
 
 def fail(msg):
     """
     In case of failure, display a message and exit(1)
     """
-
-    print(msg, file=stderr)
+    print(msg, file=stderr)  # noqa: T201
     exit(1)
 
 
-def vary_name(name: Text):
+def vary_name(name: str):
     """
     Validates the name and creates variations
     """
-
     snake = re.match(r"^[a-z][a-z0-9]*(?:_[a-z0-9]+)*$", name)
 
     if not snake:
         fail("The project name is not a valid snake-case Python variable name")
 
     camel = [x[0].upper() + x[1:] for x in name.split("_")]
 
     return {
         "project_name_snake": name,
         "project_name_camel": "".join(camel),
         "project_name_readable": " ".join(camel),
     }
 
 
-def make_random_key() -> Text:
+def make_random_key() -> str:
     """
     Generates a secure random string
     """
-
     r = SystemRandom()
     allowed = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789_+/[]"
 
     return "".join([r.choice(allowed) for _ in range(0, 50)])
 
 
-def make_dir_path(project_dir, root, project_name):
+def make_dir_path(project_dir, root, project_name) -> Path:
     """
     Generates the target path for a directory
     """
+    root = str(root).replace("__project_name_snake__", project_name)
+    real_dir = Path(project_dir).absolute()
+    return real_dir / root
 
-    root = root.replace("__project_name_snake__", project_name)
-    real_dir = path.realpath(project_dir)
-    return path.join(real_dir, root)
 
-
-def make_file_path(project_dir, project_name, root, name):
+def make_file_path(project_dir, project_name, root, name) -> Path:
     """
     Generates the target path for a file
     """
-
-    return path.join(make_dir_path(project_dir, root, project_name), name)
+    return make_dir_path(project_dir, root, project_name) / name
 
 
 def generate_vars(project_name, project_dir):
     """
     Generates the variables to replace in files
     """
-
     out = vary_name(project_name)
     out["random_key"] = make_random_key()
     out["settings_file"] = make_file_path(
         project_dir,
         project_name,
-        path.join("src", project_name),
+        Path("src") / project_name,
         "settings.py",
     )
 
     return out
 
 
 def get_files():
     """
     Read all the template's files
     """
+    files_root = Path(__file__).parent / "files"
 
-    files_root = path.join(path.dirname(__file__), "files")
-
-    for root, dirs, files in walk(files_root):
-        rel_root = path.relpath(root, files_root)
+    for file_path in files_root.rglob("*"):
+        if file_path.is_file():
+            rel_path = file_path.relative_to(files_root)
+            rel_root = rel_path.parent
+            file_name = rel_path.name
 
-        for file_name in files:
             try:
-                f = open(path.join(root, file_name), "r", encoding="utf-8")
-                with f:
+                with file_path.open(encoding="utf-8") as f:
                     yield rel_root, file_name, f.read(), True
             except UnicodeError:
-                f = open(path.join(root, file_name), "rb")
-                with f:
+                with file_path.open("rb") as f:
                     yield rel_root, file_name, f.read(), False
 
 
 def check_target(target_path):
     """
     Checks that the target path is not empty
     """
-
-    if not path.exists(target_path):
+    target = Path(target_path)
+    if not target.exists():
         return
 
-    with scandir(target_path) as d:
-        for entry in d:
-            if not entry.name.startswith("."):
-                fail(f'Target directory "{target_path}" is not empty')
+    for entry in target.iterdir():
+        if not entry.name.startswith("."):
+            fail(f'Target directory "{target_path}" is not empty')
 
 
 def replace_content(content, project_vars):
     """
     Replaces variables inside the content.
     """
-
     for k, v in project_vars.items():
-        content = content.replace(f"__{k}__", v)
+        content = content.replace(f"__{k}__", str(v))
 
     return content
 
 
 def copy_files(project_vars, project_dir, files):
     """
     Copies files from the template into their target location. Unicode files
     get their variables replaced here and files with a shebang are set to be
     executable.
     """
-
     for root, name, content, is_unicode in files:
         project_name = project_vars["project_name_snake"]
 
         if is_unicode:
             content = replace_content(content, project_vars)
 
         file_path = make_file_path(project_dir, project_name, root, name)
-        makedirs(make_dir_path(project_dir, root, project_name), exist_ok=True)
+        make_dir_path(project_dir, root, project_name).mkdir(
+            parents=True, exist_ok=True
+        )
 
         if is_unicode:
-            with open(file_path, "w") as f:
-                f.write(content)
+            file_path.write_text(content, encoding="utf-8")
 
             if content.startswith("#!"):
-                chmod(file_path, 0o755)
+                file_path.chmod(0o755)
         else:
-            with open(file_path, "wb") as f:
-                f.write(content)
+            file_path.write_bytes(content)
 
 
 def main(args):
     project_vars = generate_vars(args.project_name, args.dir)
     check_target(args.dir)
     copy_files(project_vars, args.dir, get_files())
```

### Comparing `bernard-0.6.0/src/bernard/misc/start_project/files/manage.py` & `bernard-0.7.0/src/bernard/misc/start_project/files/manage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 #!/usr/bin/env python3
 
-from os import environ, path
+from os import environ
+from pathlib import Path
 from sys import path as py_path
 from sys import stderr
 
-ROOT = path.dirname(__file__)
+ROOT = Path(__file__).parent
 
 environ.setdefault(
     "BERNARD_SETTINGS_FILE",
-    path.join(ROOT, "src/__project_name_snake__/settings.py"),
+    str(ROOT / "src/__project_name_snake__/settings.py"),
 )
 
 
 if __name__ == "__main__":
     try:
-        py_path.append(path.join(ROOT, "src"))
+        py_path.append(str(ROOT / "src"))
         from bernard.misc.main import main
 
         main()
     except ImportError:
-        print(
+        print(  # noqa: T201
             "Could not import BERNARD. Is your environment correctly " "configured?",
             file=stderr,
         )
         exit(1)
```

### Comparing `bernard-0.6.0/src/bernard/misc/start_project/files/src/__project_name_snake__/settings.py` & `bernard-0.7.0/src/bernard/misc/start_project/files/src/__project_name_snake__/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,40 @@
-from os import getenv, path
+from os import getenv
+from pathlib import Path
 from urllib.parse import urlparse
 
 
 def extract_domain(var_name, output):
     """
     Extracts just the domain name from an URL and adds it to a list
     """
-
     var = getenv(var_name)
 
     if var:
         p = urlparse(var)
         output.append(p.hostname)
 
 
 def make_whitelist():
     """
     Generates the list of whitelisted domains for webviews. This is especially
     useful when you create your Facebook Messenger configuration.
 
     Don't hesitate to change this function to add more domains if you need it.
     """
-
     out = []
     extract_domain("BERNARD_BASE_URL", out)
     return out
 
 
-def i18n_root(lang):
+def i18n_root(lang) -> Path:
     """
     Computes the root to a given lang's root directory
     """
-
-    return path.join(path.dirname(__file__), "../../i18n", lang)
+    return Path(__file__).parent / "../../i18n" / lang
 
 
 # --- Starting points ---
 
 # This module contains the transitions and is loaded to generate the FSM.
 TRANSITIONS_MODULE = "__project_name_snake__.transitions"
 
@@ -137,26 +135,26 @@
 # --- Natural language understanding/generation ---
 
 # List of intents loaders, typically CSV files with intents.
 I18N_INTENTS_LOADERS = [
     {
         "loader": "bernard.i18n.loaders.CsvIntentsLoader",
         "params": {
-            "file_path": path.join(i18n_root("en"), "intents.csv"),
+            "file_path": i18n_root("en") / "intents.csv",
             "locale": "en",
         },
     },
 ]
 
 # List of translation loaders, typically CSV files with translations.
 I18N_TRANSLATION_LOADERS = [
     {
         "loader": "bernard.i18n.loaders.CsvTranslationLoader",
         "params": {
-            "file_path": path.join(i18n_root("en"), "responses.csv"),
+            "file_path": i18n_root("en") / "responses.csv",
             "locale": "fr",
         },
     },
 ]
 
 
 # --- Middlewares ---
```

### Comparing `bernard-0.6.0/src/bernard/misc/start_project/files/src/__project_name_snake__/states.py` & `bernard-0.7.0/src/bernard/misc/start_project/files/src/__project_name_snake__/states.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,24 +15,22 @@
 
     @page_view("/bot/error")
     async def error(self) -> None:
         """
         This happens when something goes wrong (it's the equivalent of the
         HTTP error 500).
         """
-
         self.send(lyr.Text(t.ERROR))
 
     @page_view("/bot/confused")
     async def confused(self) -> None:
         """
         This is called when the user sends a message that triggers no
         transitions.
         """
-
         self.send(lyr.Text(t.CONFUSED))
 
     async def handle(self) -> None:
         raise NotImplementedError
 
 
 class Hello(__project_name_camel__State):
```

### Comparing `bernard-0.6.0/src/bernard/platforms/facebook/helpers.py` & `bernard-0.7.0/src/bernard/platforms/facebook/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Text
-from urllib.parse import urljoin
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
-import jwt
-import ujson
+import orjson
 
-from bernard.conf import settings
 from bernard.i18n import TransText, render
 from bernard.media.base import BaseMedia, UrlMedia
-from bernard.utils import patch_qs
 
 if TYPE_CHECKING:
     from bernard.engine.platform import Platform
     from bernard.engine.request import Request
 
     from .layers import GenericTemplate
 
@@ -23,20 +19,20 @@
     """
 
     full = "full"
     tall = "tall"
     compact = "compact"
 
 
-class BaseButton(object):
+class BaseButton:
     """
     Base utility class and interface for Facebook buttons.
     """
 
-    def __init__(self, title: Text):
+    def __init__(self, title: str):
         self.title = title
 
     def __eq__(self, other):
         raise NotImplementedError
 
     def __repr__(self):
         raise NotImplementedError
@@ -46,33 +42,33 @@
         Transforms the object into a JSON-serializable structure
         """
         raise NotImplementedError
 
     def is_sharable(self):
         """
         Returns True if the button holds no sensitive (aka authentication)
-        information. If it has, it will automatically disable the shareability
+        information. If it has, it will automatically disable the share-ability
         of the template that holds that button.
         """
         return True
 
 
 class UrlButton(BaseButton):
     """
-    That's an URL button. It has quite a lot of options, see the init doc.
+    That's a URL button. It has quite a lot of options, see the init doc.
     """
 
     def __init__(
         self,
         title: TransText,
-        url: Text,
+        url: str,
         sign_webview: bool = False,
         webview_height_ratio: Optional[WebviewRatio] = None,
         messenger_extensions: Optional[bool] = None,
-        fallback_url: Optional[Text] = None,
+        fallback_url: Optional[str] = None,
         hide_share: Optional[bool] = None,
     ):
         """
         Please refer to the FB doc for more info.
 
         :param title: Title that will be displayed
         :param url: URL to send the user to
@@ -102,21 +98,20 @@
             and self.webview_height_ratio == other.webview_height_ratio
             and self.messenger_extensions == other.messenger_exteions
             and self.fallback_url == other.fallback_url
             and self.hide_share == other.hide_share
         )
 
     def __repr__(self):
-        return "Url({}, {})".format(repr(self.title), repr(self.url))
+        return f"Url({self.title!r}, {self.url!r})"
 
-    async def _make_url(self, url: Text, request: "Request") -> Text:
+    async def _make_url(self, url: str, request: "Request") -> str:
         """
         Signs the URL if needed
         """
-
         if self.sign_webview:
             return await request.sign_url(url)
 
         return url
 
     async def serialize(self, request: "Request") -> Dict:
         out = {
@@ -137,15 +132,15 @@
         if self.hide_share or self.sign_webview:
             out["webview_share_button"] = "hide"
 
         return out
 
     def is_sharable(self):
         """
-        This button can be shared only if it is naive, eg it does not track
+        This button can be shared only if it is naive, e.g. it does not track
         URLs and does not embed an auto-connect code.
         """
         return not self.sign_webview
 
 
 class PostbackButton(BaseButton):
     """
@@ -157,31 +152,31 @@
         super().__init__(title)
         self.payload = payload
 
     async def serialize(self, request: "Request"):
         return {
             "type": "postback",
             "title": await render(self.title, request),
-            "payload": ujson.dumps(self.payload),
+            "payload": orjson.dumps(self.payload).decode(),
         }
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.payload == other.payload
 
     def __repr__(self):
-        return "Postback({}, {})".format(repr(self.title), repr(self.payload))
+        return f"Postback({self.title!r}, {self.payload!r})"
 
 
 class CallButton(BaseButton):
     """
     A button to trigger a phone call. The phone number must be in the format
     "+123456789"
     """
 
-    def __init__(self, title: TransText, phone_number: Text):
+    def __init__(self, title: TransText, phone_number: str):
         super().__init__(title)
         self.phone_number = phone_number
 
     async def serialize(self, request: "Request"):
         return {
             "type": "phone_number",
             "title": await render(self.title, request),
@@ -191,44 +186,44 @@
     def __eq__(self, other):
         return (
             self.__class__ == other.__class__
             and self.phone_number == other.phone_number
         )
 
     def __repr__(self):
-        return "Postback({}, {})".format(repr(self.title), repr(self.phone_number))
+        return f"Postback({self.title!r}, {self.phone_number!r})"
 
 
 class CardAction(UrlButton):
     """
     That is a simili-button that behaves like a URL button when the user clicks
     on a card.
     """
 
     def __init__(
         self,
-        url: Text,
+        url: str,
         sign_webview: bool = False,
         webview_height_ratio: Optional[WebviewRatio] = None,
         messenger_extensions: Optional[bool] = None,
-        fallback_url: Optional[Text] = None,
+        fallback_url: Optional[str] = None,
         hide_share: Optional[bool] = None,
     ):
-        super(CardAction, self).__init__(
+        super().__init__(
             "",
             url,
             sign_webview,
             webview_height_ratio,
             messenger_extensions,
             fallback_url,
             hide_share,
         )
 
     def __repr__(self):
-        return "CardAction({})".format(repr(self.url))
+        return f"CardAction({self.url!r})"
 
     def __eq__(self, other):
         return (
             self.__class__ == other.__class__
             and self.url == other.url
             and self.sign_webview == other.sign_webview
             and self.webview_height_ratio == other.webview_height_ratio
@@ -239,15 +234,15 @@
 
     async def serialize(self, request: "Request"):
         out = await super().serialize(request)
         del out["title"]
         return out
 
 
-class Card(object):
+class Card:
     """
     A Facebook Card for the Generic Template.
     """
 
     def __init__(
         self,
         title: TransText,
@@ -269,28 +264,30 @@
             and self.subtitle == other.subtitle
             and list(self.buttons) == list(other.buttons)
             and self.image == other.image
             and self.default_action == other.default_action
         )
 
     def __repr__(self):
-        return "Card({})".format(repr(self.title))
+        return f"Card({self.title!r})"
 
     async def convert_media(self, platform: "Platform"):
         if self.image:
             self.image = await platform.ensure_usable_media(self.image)
 
     async def serialize(self, request: "Request"):
         out = {"title": await render(self.title, request)}
 
         if self.subtitle:
             out["subtitle"] = await render(self.subtitle, request)
 
         if self.image:
-            assert isinstance(self.image, UrlMedia)
+            if not isinstance(self.image, UrlMedia):
+                msg = "Only URL media is supported for cards"
+                raise ValueError(msg)
             out["image_url"] = self.image.url
 
         if self.buttons:
             out["buttons"] = [await b.serialize(request) for b in self.buttons]
 
         if self.default_action:
             out["default_action"] = self.default_action.serialize(request)
@@ -308,15 +305,15 @@
                 and self.default_action.is_sharable()
             )
 
 
 class ShareButton(BaseButton):
     """
     That's a Facebook Share button. When the user clicks on it, the FbCard
-    is share to an other user who can go to the bot.
+    is share to another user who can go to the bot.
 
     Parameter share_content define what will be share and must be a generic
     template.
     """
 
     def __init__(self, share_content: Optional["GenericTemplate"] = None):
         super().__init__("")
```

### Comparing `bernard-0.6.0/src/bernard/platforms/facebook/layers.py` & `bernard-0.7.0/src/bernard/platforms/facebook/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import TYPE_CHECKING, Dict, List, Optional, Text
+from typing import TYPE_CHECKING, Dict, List, Optional
 
 from bernard.i18n import TransText, render
 from bernard.i18n.intents import Intent
 from bernard.layers import BaseLayer
 
 from .helpers import BaseButton, Card
 
@@ -57,18 +57,19 @@
             response,
             update,
             tag,
             subscription,
         ]
 
         if self._args.count(None) != 3:
-            raise ValueError(
+            msg = (
                 "You need to specify exactly one argument when "
                 "creating a MessagingType() layer."
             )
+            raise ValueError(msg)
 
     def __eq__(self, other):
         return (
             self.__class__ == other.__class__
             and self.response == other.response
             and self.update == other.update
             and self.subscription == other.subscription
@@ -87,15 +88,14 @@
         if self.subscription is not None:
             return ["subscription"]
 
     def serialize(self):
         """
         Generates the messaging-type-related part of the message dictionary.
         """
-
         if self.response is not None:
             return {"messaging_type": "RESPONSE"}
 
         if self.update is not None:
             return {"messaging_type": "UPDATE"}
 
         if self.tag is not None:
@@ -110,48 +110,44 @@
 
 class QuickRepliesList(BaseLayer):
     """
     This layer is a bunch of quick replies options that will be presented to
     the user.
     """
 
-    class BaseOption(object):
+    class BaseOption:
         """
         Base object for a quick reply option
         """
 
         type = None
 
     class TextOption(BaseOption):
         """
         A quick reply that will trigger a text response (with a QuickReply
         layer).
         """
 
         type = "text"
 
-        def __init__(
-            self, slug: Text, text: TransText, intent: Optional[Intent] = None
-        ):
+        def __init__(self, slug: str, text: TransText, intent: Optional[Intent] = None):
             self.slug = slug
             self.text = text
             self.intent = intent
 
         def __eq__(self, other):
             return (
                 self.__class__ == other.__class__
                 and self.slug == other.slug
                 and self.text == other.text
                 and self.intent == other.intent
             )
 
         def __repr__(self):
-            return "Text({}, {}, {})".format(
-                repr(self.slug), repr(self.text), repr(self.intent)
-            )
+            return f"Text({self.slug!r}, {self.text!r}, {self.intent!r})"
 
     class LocationOption(BaseOption):
         """
         A quick reply that will generate a location response (with a Location
         layer).
         """
 
@@ -172,31 +168,26 @@
     def __eq__(self, other):
         if self.__class__ != other.__class__:
             return False
 
         if len(self.options) != len(other.options):
             return False
 
-        for o1, o2 in zip(self.options, other.options):
-            if o1 != o2:
-                return False
-
-        return True
+        return all(o1 == o2 for o1, o2 in zip(self.options, other.options))
 
     def _repr_arguments(self):
         return self.options
 
     async def patch_register(self, register: Dict, request: "Request"):
         """
         Store all options in the "choices" sub-register. We store both the
         text and the potential intent, in order to match both regular
         quick reply clicks but also the user typing stuff on his keyboard that
         matches more or less the content of quick replies.
         """
-
         register["choices"] = {
             o.slug: {
                 "intent": o.intent.key if o.intent else None,
                 "text": await render(o.text, request),
             }
             for o in self.options
             if isinstance(o, QuickRepliesList.TextOption)
```

### Comparing `bernard-0.6.0/src/bernard/platforms/facebook/platform.py` & `bernard-0.7.0/src/bernard/platforms/facebook/platform.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,124 +1,134 @@
 import asyncio
 import hmac
 import logging
 from datetime import tzinfo
 from hashlib import sha1, sha256
 from textwrap import wrap
-from typing import Any, ByteString, Dict, List, Optional, Set, Text, Tuple
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    ByteString,
+    ClassVar,
+    Dict,
+    List,
+    Optional,
+    Set,
+    Tuple,
+)
 from urllib.parse import urljoin
 
 import httpx
 import jwt
+import orjson
 import sentry_sdk
-import ujson
 from aiohttp.web import Request as HttpRequest
 from aiohttp.web_response import Response, json_response
 from aiohttp.web_urldispatcher import UrlDispatcher
 from dateutil import tz
 from facepy import SignedRequest, SignedRequestError
 
 from bernard import layers as lyr
 from bernard.conf import settings
 from bernard.core.health_check import HealthCheckFail
 from bernard.engine.platform import PlatformOperationError, SimplePlatform
 from bernard.engine.request import BaseMessage, Conversation, Request, User
 from bernard.engine.responder import Responder
 from bernard.i18n.translator import render
 from bernard.layers import BaseLayer, Stack
-from bernard.layers.definitions import BaseMediaLayer
 from bernard.media.base import BaseMedia, UrlMedia
 from bernard.utils import dict_is_subset
 
 from .layers import (
     ButtonTemplate,
     GenericTemplate,
     MessagingType,
     OptIn,
     QuickRepliesList,
     QuickReply,
 )
 
+if TYPE_CHECKING:
+    from bernard.layers.definitions import BaseMediaLayer
+
 FB_API = "2.12"
 MESSAGES_ENDPOINT = f"https://graph.facebook.com/v{FB_API}/me/messages"
 PROFILE_ENDPOINT = f"https://graph.facebook.com/v{FB_API}/me/messenger_profile"
 GRAPH_ENDPOINT = f'https://graph.facebook.com/v{FB_API}/{"{}"}'
 
 
 logger = logging.getLogger("bernard.platform.facebook")
 
 
-def sign_message(body: ByteString, secret: Text) -> Text:
+def sign_message(body: ByteString, secret: str) -> str:
     """
     Compute a message's signature.
     """
-
-    return "sha1={}".format(hmac.new(secret.encode(), body, sha1).hexdigest())
+    return f"sha1={hmac.new(secret.encode(), body, sha1).hexdigest()}"
 
 
 class FacebookUser(User):
     """
     That is the Facebook user class. So far it just computes the unique user
     ID.
     """
 
     def __init__(
         self,
-        fbid: Text,
-        page_id: Text,
+        fbid: str,
+        page_id: str,
         facebook: "Facebook",
         message: "FacebookMessage",
     ):
         self.fbid = fbid
         self.page_id = page_id
         self.facebook = facebook
         self.message = message
         self._cache = None
-        super(FacebookUser, self).__init__(self._fbid_to_id(fbid))
+        super().__init__(self._fbid_to_id(fbid))
 
-    def _fbid_to_id(self, fbid: Text):
+    def _fbid_to_id(self, fbid: str):
         """
         Transforms a Facebook user ID into a unique user ID.
         """
-        return "facebook:user:{}".format(fbid)
+        return f"facebook:user:{fbid}"
 
     async def _get_user(self):
         """
         Get the user dict from cache or query it from the platform if missing.
         """
-
         if self._cache is None:
             try:
                 self._cache = await self.facebook.get_user(self.fbid, self.page_id)
             except PlatformOperationError:
                 self._cache = {}
         return self._cache
 
-    async def get_full_name(self) -> Text:
+    async def get_full_name(self) -> str:
         """
         Let's implement this later
         """
         raise NotImplementedError
 
-    async def get_formal_name(self) -> Text:
+    async def get_formal_name(self) -> str:
         """
         Let's implement this later
         """
         raise NotImplementedError
 
-    async def get_friendly_name(self) -> Text:
+    async def get_friendly_name(self) -> str:
         """
         The friendly name is mapped to Facebook's first name. If the first
         name is missing, use the last name.
         """
         u = await self._get_user()
-        f = u.get("first_name", "").strip()
-        l = u.get("last_name", "").strip()
+        first_name = u.get("first_name", "").strip()
+        last_name = u.get("last_name", "").strip()
 
-        return f or l
+        return first_name or last_name
 
     async def get_gender(self) -> User.Gender:
         """
         Get the gender from Facebook.
         """
         u = await self._get_user()
 
@@ -129,54 +139,53 @@
 
     async def get_timezone(self) -> Optional[tzinfo]:
         """
         We can't exactly know the time zone of the user from what Facebook
         gives (fucking morons) but we can still give something that'll work
         until next DST.
         """
-
         u = await self._get_user()
         diff = float(u.get("timezone", 0)) * 3600.0
 
         return tz.tzoffset("ITC", diff)
 
-    async def get_locale(self) -> Text:
+    async def get_locale(self) -> str:
         u = await self._get_user()
         return u.get("locale", "")
 
 
 class FacebookConversation(Conversation):
     """
     That is a Facebook conversation. Some idea as the user.
     """
 
-    def __init__(self, fbid: Text):
+    def __init__(self, fbid: str):
         self.fbid = fbid
-        super(FacebookConversation, self).__init__(self._fbid_to_id(fbid))
+        super().__init__(self._fbid_to_id(fbid))
 
-    def _fbid_to_id(self, fbid: Text):
+    def _fbid_to_id(self, fbid: str):
         """
         Facebook ID into conversation ID. So far we just handle user-to-bot
         cases, but who knows it might change in the future.
         """
-        return "facebook:conversation:user:{}".format(fbid)
+        return f"facebook:conversation:user:{fbid}"
 
 
 class FacebookMessage(BaseMessage):
     """
     Decodes the raw JSON sent by Facebook and allow to extract the user and the
     accompanying layers.
     """
 
     def __init__(self, event, facebook, confusing=True):
         self._event = event
         self._facebook = facebook
         self._confusing = confusing
 
-    def get_platform(self) -> Text:
+    def get_platform(self) -> str:
         """
         The platform is always Facebook
         """
         return "facebook"
 
     def get_user(self) -> FacebookUser:
         """
@@ -199,61 +208,76 @@
         """
         Return all layers that can be found in the message.
         """
         out = []
         msg = self._event.get("message", {})
 
         if "text" in msg:
-            out.append(lyr.RawText(msg["text"]))
+            self._get_layers_text(msg, out)
 
         for attachment in msg.get("attachments") or []:
-            if attachment["type"] == "image":
-                out.append(lyr.Image(UrlMedia(attachment["payload"]["url"])))
-            elif attachment["type"] == "audio":
-                out.append(lyr.Audio(UrlMedia(attachment["payload"]["url"])))
-            elif attachment["type"] == "file":
-                out.append(lyr.File(UrlMedia(attachment["payload"]["url"])))
-            elif attachment["type"] == "video":
-                out.append(lyr.Video(UrlMedia(attachment["payload"]["url"])))
-            elif attachment["type"] == "location":
-                # noinspection PyArgumentList
-                out.append(
-                    lyr.Location(
-                        lyr.Location.Point(
-                            lat=attachment["payload"]["coordinates"]["lat"],
-                            lon=attachment["payload"]["coordinates"]["long"],
-                        )
-                    )
-                )
+            self._get_layers_attachment(attachment, out)
 
         if "quick_reply" in msg:
-            out.append(QuickReply(msg["quick_reply"]["payload"]))
+            self._get_layers_quick_reply(msg, out)
 
         if "postback" in self._event:
-            payload = ujson.loads(self._event["postback"]["payload"])
-            out.append(lyr.Postback(payload))
+            self._get_layers_postback(out)
 
         if "optin" in self._event:
-            out.append(OptIn(self._event["optin"]["ref"]))
+            self._get_layers_optin(out)
 
         return out
 
-    def get_page_id(self) -> Text:
+    def _get_layers_text(self, msg, out):
+        out.append(lyr.RawText(msg["text"]))
+
+    def _get_layers_attachment(self, attachment, out):
+        if attachment["type"] == "image":
+            out.append(lyr.Image(UrlMedia(attachment["payload"]["url"])))
+        elif attachment["type"] == "audio":
+            out.append(lyr.Audio(UrlMedia(attachment["payload"]["url"])))
+        elif attachment["type"] == "file":
+            out.append(lyr.File(UrlMedia(attachment["payload"]["url"])))
+        elif attachment["type"] == "video":
+            out.append(lyr.Video(UrlMedia(attachment["payload"]["url"])))
+        elif attachment["type"] == "location":
+            # noinspection PyArgumentList
+            out.append(
+                lyr.Location(
+                    lyr.Location.Point(
+                        lat=attachment["payload"]["coordinates"]["lat"],
+                        lon=attachment["payload"]["coordinates"]["long"],
+                    )
+                )
+            )
+
+    def _get_layers_quick_reply(self, msg, out):
+        out.append(QuickReply(msg["quick_reply"]["payload"]))
+
+    def _get_layers_postback(self, out):
+        payload = orjson.loads(self._event["postback"]["payload"])
+        out.append(lyr.Postback(payload))
+
+    def _get_layers_optin(self, out):
+        out.append(OptIn(self._event["optin"]["ref"]))
+
+    def get_page_id(self) -> str:
         """
         That's for internal use, extract the Facebook page ID.
         """
         return self._event["recipient"]["id"]
 
     def should_confuse(self) -> bool:
         """
         The message is marked confusing or not at init
         """
         return self._confusing
 
-    async def get_token(self) -> Text:
+    async def get_token(self) -> str:
         user = self.get_user()
 
         return jwt.encode(
             {
                 "fb_psid": user.fbid,
                 "fb_pid": user.page_id,
             },
@@ -267,15 +291,15 @@
     Not much to do here
     """
 
 
 class Facebook(SimplePlatform):
     NAME = "facebook"
 
-    PATTERNS = {
+    PATTERNS: ClassVar[dict[str, str]] = {
         "text": "^(Text|RawText|MultiText)+ QuickRepliesList? MessagingType?$",
         "generic_template": "^GenericTemplate QuickRepliesList? " "MessagingType?$",
         "button_template": "^ButtonTemplate QuickRepliesList? " "MessagingType?$",
         "attachment": "^(Image|Audio|Video|File) QuickRepliesList? " "MessagingType?$",
         "sleep": "^Sleep$",
         "typing": "^Typing$",
     }
@@ -284,19 +308,18 @@
     async def self_check(cls):
         """
         Check that the configuration is correct
 
         - Presence of "BERNARD_BASE_URL" in the global configuration
         - Presence of a "WEBVIEW_SECRET_KEY"
         """
-
         async for check in super().self_check():
             yield check
 
-        s = cls.settings()
+        cls.settings()
 
         if not hasattr(settings, "BERNARD_BASE_URL"):
             yield HealthCheckFail(
                 "00005",
                 '"BERNARD_BASE_URL" cannot be found in the configuration. The'
                 "Telegram platform needs it because it uses it to "
                 "automatically register its hook.",
@@ -311,57 +334,51 @@
             )
 
     @property
     def app_access_token(self):
         """
         App token to access app configuration API
         """
-
         page = self.settings()
         return f"{page['app_id']}|{page['app_secret']}"
 
     @property
     def verify_token(self):
         """
         Automatically generated secure verify token
         """
-
         h = sha256()
         h.update(self.app_access_token.encode())
         return h.hexdigest()
 
     @property
     def webhook_path(self):
         """
         Path to the webhook
         """
-
         return f"/hooks/{self.id}"
 
     @property
     def webhook_url(self):
         """
         Full URL to the hook
         """
-
         return urljoin(settings.BERNARD_BASE_URL, self.webhook_path)
 
     def hook_up(self, router: UrlDispatcher):
         """
         Dynamically hooks the right webhook paths
         """
-
         router.add_get(self.webhook_path, self.check_hook)
         router.add_post(self.webhook_path, self.receive_events)
 
     async def check_hook(self, request: HttpRequest):
         """
         Called when Facebook checks the hook
         """
-
         verify_token = request.query.get("hub.verify_token")
 
         if not verify_token:
             return json_response(
                 {
                     "error": "No verification token was provided",
                 },
@@ -377,20 +394,19 @@
             }
         )
 
     async def receive_events(self, request: HttpRequest):
         """
         Events received from Facebook
         """
-
         body = await request.read()
         s = self.settings()
 
         try:
-            content = ujson.loads(body)
+            content = orjson.loads(body)
         except ValueError:
             return json_response(
                 {"error": True, "message": "Cannot decode body"}, status=400
             )
 
         secret = s["app_secret"]
         actual_sig = request.headers["X-Hub-Signature"]
@@ -417,28 +433,26 @@
         )
 
     async def _deferred_init(self):
         """
         Run those things in a sepearate tasks as they are not required for the
         bot to work and they take a lot of time to run.
         """
-
         await self._check_subscriptions()
         await self._set_whitelist()
         await self._set_get_started()
         await self._set_greeting_text()
         await self._set_persistent_menu()
 
-    async def _get_messenger_profile(self, page, fields: List[Text]):
+    async def _get_messenger_profile(self, page, fields: List[str]):
         """
         Fetch the value of specified fields in order to avoid setting the same
         field twice at the same value (since Facebook engineers are not able
         to make menus that keep on working if set again).
         """
-
         params = {
             "access_token": page["page_token"],
             "fields": ",".join(fields),
         }
 
         r = await self.session.get(PROFILE_ENDPOINT, params=params)
         await self._handle_fb_response(r)
@@ -454,15 +468,14 @@
         """
         The messenger profile API handles all meta-information about the bot,
         like the menu. This allows to submit data to this API endpoint.
 
         :param page: page dict from the configuration
         :param content: content to be sent to Facebook (as dict)
         """
-
         log_name = ", ".join(repr(x) for x in content.keys())
         page_id = page["page_id"]
 
         current = await self._get_messenger_profile(page, content.keys())
 
         if dict_is_subset(content, current):
             logger.info("Page %s: %s is already up to date", page_id, log_name)
@@ -473,15 +486,18 @@
         }
 
         headers = {
             "content-type": "application/json",
         }
 
         r = await self.session.post(
-            PROFILE_ENDPOINT, params=params, headers=headers, data=ujson.dumps(content)
+            PROFILE_ENDPOINT,
+            params=params,
+            headers=headers,
+            json=content,
         )
 
         # noinspection PyBroadException
         try:
             await self._handle_fb_response(r)
         except Exception as e:
             logger.exception("Page %s: %s could not be set", page_id, log_name)
@@ -489,38 +505,36 @@
         else:
             logger.info("Page %s: %s was updated", page_id, log_name)
 
     async def _set_get_started(self):
         """
         Set the "get started" action for all configured pages.
         """
-
         page = self.settings()
 
         if "get_started" in page:
             payload = page["get_started"]
         else:
             payload = {"action": "get_started"}
 
         await self._send_to_messenger_profile(
             page,
             {
                 "get_started": {
-                    "payload": ujson.dumps(payload),
+                    "payload": orjson.dumps(payload).decode(),
                 },
             },
         )
 
         logger.info("Get started set for page %s", page["page_id"])
 
     async def _set_greeting_text(self):
         """
         Set the greeting text of the page
         """
-
         page = self.settings()
 
         if "greeting" in page:
             await self._send_to_messenger_profile(
                 page,
                 {
                     "greeting": page["greeting"],
@@ -529,15 +543,14 @@
 
             logger.info("Greeting text set for page %s", page["page_id"])
 
     async def _set_persistent_menu(self):
         """
         Define the persistent menu for all pages
         """
-
         page = self.settings()
 
         if "menu" in page:
             await self._send_to_messenger_profile(
                 page,
                 {
                     "persistent_menu": page["menu"],
@@ -546,15 +559,14 @@
 
             logger.info("Set menu for page %s", page["page_id"])
 
     async def _set_whitelist(self):
         """
         Whitelist domains for the messenger extensions
         """
-
         page = self.settings()
 
         if "whitelist" in page:
             await self._send_to_messenger_profile(
                 page,
                 {
                     "whitelisted_domains": page["whitelist"],
@@ -565,52 +577,49 @@
                 "Whitelisted %s for page %s", page["whitelist"], page["page_id"]
             )
 
     def _get_subscriptions_endpoint(self):
         """
         Generates the URL and tokens for the subscriptions endpoint
         """
-
         s = self.settings()
 
         params = {
             "access_token": self.app_access_token,
         }
 
         return (
             GRAPH_ENDPOINT.format(f'{s["app_id"]}/subscriptions'),
             params,
         )
 
-    async def _get_subscriptions(self) -> Tuple[Set[Text], Text]:
+    async def _get_subscriptions(self) -> Tuple[Set[str], str]:
         """
         List the subscriptions currently active
         """
-
         url, params = self._get_subscriptions_endpoint()
 
         r = await self.session.get(url, params=params)
 
         await self._handle_fb_response(r)
         data = r.json()
 
         for scope in data["data"]:
             if scope["object"] == "page":
                 return (
-                    set(x["name"] for x in scope["fields"]),
+                    {x["name"] for x in scope["fields"]},
                     scope["callback_url"],
                 )
 
         return set(), ""
 
     async def _set_subscriptions(self, subscriptions):
         """
         Set the subscriptions to a specific list of values
         """
-
         url, params = self._get_subscriptions_endpoint()
 
         data = {
             "object": "page",
             "callback_url": self.webhook_url,
             "fields": ", ".join(subscriptions),
             "verify_token": self.verify_token,
@@ -619,26 +628,25 @@
         headers = {
             "Content-Type": "application/json",
         }
 
         r = await self.session.post(
             url,
             params=params,
-            data=ujson.dumps(data),
+            json=data,
             headers=headers,
         )
 
         await self._handle_fb_response(r)
         data = r.json()
 
     async def _check_subscriptions(self):
         """
         Checks that all subscriptions are subscribed
         """
-
         subscribed, url = await self._get_subscriptions()
         expect = set(settings.FACEBOOK_SUBSCRIPTIONS)
 
         if (expect - subscribed) or url != self.webhook_url:
             await self._set_subscriptions(expect | subscribed)
             logger.info("Updated webhook subscriptions")
         else:
@@ -647,38 +655,37 @@
     async def handle_event(self, event: FacebookMessage):
         """
         Handle an incoming message from Facebook.
         """
         responder = FacebookResponder(self)
         await self._notify(event, responder)
 
-    def _access_token(self, request: Request = None, page_id: Text = ""):
+    def _access_token(self, request: Request = None, page_id: str = ""):
         """
         Guess the access token for that specific request.
         """
-
         if not page_id:
-            msg = request.message  # type: FacebookMessage
+            msg: FacebookMessage = request.message  # type: ignore
             page_id = msg.get_page_id()
 
         page = self.settings()
 
         if page["page_id"] == page_id:
             return page["page_token"]
 
-        raise PlatformOperationError(
+        error_msg = (
             "Trying to get access token of the "
-            'page "{}", which is not configured.'.format(page_id)
+            + f'page "{page_id}", which is not configured.'
         )
+        raise PlatformOperationError(error_msg)
 
     async def _make_qr(self, qr: QuickRepliesList.BaseOption, request: Request):
         """
         Generate a single quick reply's content.
         """
-
         if isinstance(qr, QuickRepliesList.TextOption):
             return {
                 "content_type": "text",
                 "title": await render(qr.text, request),
                 "payload": qr.slug,
             }
         elif isinstance(qr, QuickRepliesList.LocationOption):
@@ -699,27 +706,24 @@
         """
         Send text layers to the user. Each layer will go in its own bubble.
 
         Also, Facebook limits messages to 320 chars, so if any message is
         longer than that it will be split into as many messages as needed to
         be accepted by Facebook.
         """
-
         parts = []
 
         for layer in stack.layers:
             if isinstance(layer, lyr.MultiText):
                 lines = await render(layer.text, request, multi_line=True)
                 for line in lines:
-                    for part in wrap(line, 320):
-                        parts.append(part)
+                    parts.extend(wrap(line, 320))
             elif isinstance(layer, (lyr.Text, lyr.RawText)):
                 text = await render(layer.text, request)
-                for part in wrap(text, 320):
-                    parts.append(part)
+                parts.extend(wrap(text, 320))
 
         for part in parts[:-1]:
             await self._send(
                 request,
                 {
                     "text": part,
                 },
@@ -735,28 +739,26 @@
         await self._add_qr(stack, msg, request)
         await self._send(request, msg, stack)
 
     async def _send_generic_template(self, request: Request, stack: Stack):
         """
         Generates and send a generic template.
         """
-
         gt = stack.get_layer(GenericTemplate)
         payload = await gt.serialize(request)
 
         msg = {"attachment": {"type": "template", "payload": payload}}
 
         await self._add_qr(stack, msg, request)
         await self._send(request, msg, stack)
 
     async def _send_button_template(self, request: Request, stack: Stack):
         """
         Generates and send a button template.
         """
-
         gt = stack.get_layer(ButtonTemplate)
 
         payload = {
             "template_type": "button",
             "text": await render(gt.text, request),
             "buttons": [await b.serialize(request) for b in gt.buttons],
         }
@@ -770,46 +772,44 @@
         types = {
             lyr.Image: "image",
             lyr.Audio: "audio",
             lyr.File: "file",
             lyr.Video: "video",
         }
 
-        l: BaseMediaLayer = stack.layers[0]
-        media = await self.ensure_usable_media(l.media)
+        layer: BaseMediaLayer = stack.layers[0]
+        media = await self.ensure_usable_media(layer.media)
 
         # noinspection PyTypeChecker
         msg = {
             "attachment": {
-                "type": types[l.__class__],
+                "type": types[layer.__class__],
                 "payload": {
                     "url": media.url,
                 },
             },
         }
 
         await self._add_qr(stack, msg, request)
         await self._send(request, msg, stack)
 
     async def _send_sleep(self, request: Request, stack: Stack):
         """
         Sleep for the amount of time specified in the Sleep layer
         """
-
         duration = stack.get_layer(lyr.Sleep).duration
         await asyncio.sleep(duration)
 
     async def _send_typing(self, request: Request, stack: Stack):
         """
         Send to Facebook typing indications
         """
-
         active = stack.get_layer(lyr.Typing).active
 
-        msg = ujson.dumps(
+        msg = orjson.dumps(
             {
                 "recipient": {
                     "id": request.conversation.fbid,
                 },
                 "sender_action": "typing_on" if active else "typing_off",
             }
         )
@@ -821,83 +821,80 @@
         params = {
             "access_token": self._access_token(request),
         }
 
         r = await self.session.post(
             MESSAGES_ENDPOINT,
             params=params,
-            data=msg,
+            json=msg,
             headers=headers,
         )
 
         logger.debug("Sending: %s", msg)
 
         await self._handle_fb_response(r)
 
     async def _handle_fb_response(self, response: httpx.Response):
         """
         Check that Facebook was OK with the API call we just made and raise
         an exception if it failed.
         """
-
         ok = response.status_code == 200
 
         if not ok:
             # noinspection PyBroadException
             try:
                 error = (response.json())["error"]["message"]
             except Exception:
                 error = "(nothing)"
 
-            raise PlatformOperationError('Facebook says: "{}"'.format(error))
+            msg = f'Facebook says: "{error}"'
+            raise PlatformOperationError(msg)
 
-    async def _send(self, request: Request, content: Dict[Text, Any], stack: Stack):
+    async def _send(self, request: Request, content: Dict[str, Any], stack: Stack):
         """
         Actually proceed to sending the message to the Facebook API.
         """
-
         msg = {
             "recipient": {
                 "id": request.conversation.fbid,
             },
             "message": content,
         }
 
         if stack and stack.has_layer(MessagingType):
             mt = stack.get_layer(MessagingType)
         else:
             mt = MessagingType(response=True)
 
         msg.update(mt.serialize())
-        msg_json = ujson.dumps(msg)
 
         headers = {
             "content-type": "application/json",
         }
 
         params = {
             "access_token": self._access_token(request),
         }
 
         r = await self.session.post(
             MESSAGES_ENDPOINT,
             params=params,
-            data=msg_json,
+            json=msg,
             headers=headers,
         )
 
-        logger.debug("Sending: %s", msg_json)
+        logger.debug("Sending: %s", msg)
 
         await self._handle_fb_response(r)
 
     async def get_user(self, user_id, page_id):
         """
         Query a user from the API and return its JSON
         """
-
         access_token = self._access_token(page_id=page_id)
 
         params = {
             "fields": "first_name,last_name,profile_pic,locale,timezone" ",gender",
             "access_token": access_token,
         }
 
@@ -908,88 +905,89 @@
         return r.json()
 
     async def ensure_usable_media(self, media: BaseMedia) -> UrlMedia:
         """
         So far, let's just accept URL media. We'll see in the future how it
         goes.
         """
-
         if not isinstance(media, UrlMedia):
-            raise ValueError("Facebook platform only accepts URL media")
+            msg = "Facebook platform only accepts URL media"
+            raise ValueError(msg)
 
         return media
 
     def _make_fake_message(self, user_id, page_id, payload):
         """
         Creates a fake message for the given user_id. It contains a postback
         with the given payload.
         """
-
         event = {
             "sender": {
                 "id": user_id,
             },
             "recipient": {
                 "id": page_id,
             },
             "postback": {
-                "payload": ujson.dumps(payload),
+                "payload": orjson.dumps(payload).decode(),
             },
         }
 
         return FacebookMessage(event, self, False)
 
-    def _message_from_sr(self, token: Text, payload: Any) -> Optional[BaseMessage]:
+    def _message_from_sr(self, token: str, payload: Any) -> Optional[BaseMessage]:
         """
         Tries to verify the signed request
         """
-
         page = self.settings()
         secret = page["app_secret"]
 
         try:
             sr_data = SignedRequest.parse(token, secret)
-        except (TypeError, ValueError, SignedRequestError) as e:
-            return
+        except (TypeError, ValueError, SignedRequestError):
+            return None
 
         return self._make_fake_message(
             sr_data["psid"],
             page["page_id"],
             payload,
         )
 
-    def _message_from_token(self, token: Text, payload: Any) -> Optional[BaseMessage]:
+    def _message_from_token(self, token: str, payload: Any) -> Optional[BaseMessage]:
         """
         Analyzes a signed token and generates the matching message
         """
-
         try:
             tk = jwt.decode(token, settings.WEBVIEW_SECRET_KEY)
         except jwt.InvalidTokenError:
-            return
+            return None
 
         try:
             user_id = tk["fb_psid"]
-            assert isinstance(user_id, Text)
+
+            if not isinstance(user_id, str):
+                raise AssertionError
+
             page_id = tk["fb_pid"]
-            assert isinstance(page_id, Text)
+
+            if not isinstance(page_id, str):
+                raise AssertionError
         except (KeyError, AssertionError):
-            return
+            return None
 
         if self.settings()["page_id"] == page_id:
             return self._make_fake_message(user_id, page_id, payload)
 
     async def message_from_token(
-        self, token: Text, payload: Any
+        self, token: str, payload: Any
     ) -> Optional[BaseMessage]:
         """
         There is two ways of getting a FB user: either with a signed request or
         either with a platform token. Both are tried out.
         """
-
         methods = [
             self._message_from_sr,
             self._message_from_token,
         ]
 
         for method in methods:
             msg = method(token, payload)
```

### Comparing `bernard-0.6.0/src/bernard/platforms/management.py` & `bernard-0.7.0/src/bernard/platforms/management.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, AsyncIterator, Dict, Optional, Text, Tuple, Type
+from typing import Any, AsyncIterator, Dict, Optional, Tuple, Type
 
 from bernard.conf import settings
 from bernard.core.health_check import HealthCheckFail
 from bernard.engine.fsm import FSM
 from bernard.engine.platform import Platform, PlatformDoesNotExist
 from bernard.engine.request import BaseMessage
 from bernard.middleware import MiddlewareManager
@@ -18,29 +18,28 @@
 
     The platforms settings was created to stay compatible with the old way of
     declaring the FB configuration, in order not to break production bots. This
     function will convert the legacy configuration into the new configuration
     if required. As a result, it should be the only used way to access the
     platform configuration.
     """
-
     s = settings.PLATFORMS
 
     if hasattr(settings, "FACEBOOK") and settings.FACEBOOK:
         s.append(
             {
                 "class": "bernard.platforms.facebook.platform.Facebook",
                 "settings": settings.FACEBOOK,
             }
         )
 
     return s
 
 
-class PlatformManager(object):
+class PlatformManager:
     """
     That is the core of the system. This class has the responsibilities to:
 
         - Create the platform instances
         - Create the FSM
         - Hook the platforms to the FSM
 
@@ -84,29 +83,27 @@
 
         self.platforms = {}
 
     async def run_checks(self):
         """
         Run checks on itself and on the FSM
         """
-
         async for check in self.fsm.health_check():
             yield check
 
         async for check in self.self_check():
             yield check
 
         for check in MiddlewareManager.health_check():
             yield check
 
     async def self_check(self):
         """
         Checks that the platforms configuration is all right.
         """
-
         platforms = set()
 
         for platform in get_platform_settings():
             try:
                 name = platform["class"]
                 cls: Type[Platform] = import_class(name)
             except KeyError:
@@ -122,19 +119,18 @@
                     )
                 platforms.add(cls)
 
                 # noinspection PyTypeChecker
                 async for check in cls.self_check():
                     yield check
 
-    def _index_classes(self) -> Dict[Text, Type[Platform]]:
+    def _index_classes(self) -> Dict[str, Type[Platform]]:
         """
         Build a name index for all platform classes
         """
-
         out = {}
 
         for p in get_platform_settings():
             cls: Type[Platform] = import_class(p["class"])
 
             if "name" in p:
                 out[p["name"]] = cls
@@ -143,15 +139,14 @@
 
         return out
 
     async def build_platform(self, cls: Type[Platform], custom_id):
         """
         Build the Facebook platform. Nothing fancy.
         """
-
         from bernard.server.http import router
 
         p = cls()
 
         if custom_id:
             p._id = custom_id
 
@@ -160,54 +155,49 @@
         p.hook_up(router)
         return p
 
     def get_class(self, platform) -> Type[Platform]:
         """
         For a given platform name, gets the matching class
         """
-
         if platform in self._classes:
             return self._classes[platform]
 
-        raise PlatformDoesNotExist(
-            'Platform "{}" is not in configuration'.format(platform)
-        )
+        msg = f'Platform "{platform}" is not in configuration'
+        raise PlatformDoesNotExist(msg)
 
-    async def get_platform(self, name: Text):
+    async def get_platform(self, name: str):
         """
         Get a valid instance of the specified platform. Do not cache this
         object, it might change with configuration changes.
         """
-
         if not self._is_init:
             await self.init()
 
         if name not in self.platforms:
             self.platforms[name] = await self.build_platform(self.get_class(name), name)
 
         return self.platforms[name]
 
     async def get_all_platforms(self) -> AsyncIterator[Platform]:
         """
         Returns all platform instances
         """
-
         for name in self._classes.keys():
             yield await self.get_platform(name)
 
     async def message_from_token(
-        self, token: Text, payload: Any
+        self, token: str, payload: Any
     ) -> Tuple[Optional[BaseMessage], Optional[Platform]]:
         """
         Given an authentication token, find the right platform that can
         recognize this token and create a message for this platform.
 
         The payload will be inserted into a Postback layer.
         """
-
         async for platform in self.get_all_platforms():
             m = await platform.message_from_token(token, payload)
 
             if m:
                 return m, platform
 
         return None, None
```

### Comparing `bernard-0.6.0/src/bernard/platforms/telegram/_utils.py` & `bernard-0.7.0/src/bernard/platforms/telegram/_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     """
     Add the "reply markup" to a message from the layers
 
     :param msg: Message dictionary
     :param request: Current request being replied
     :param stack: Stack to analyze
     """
-
     from bernard.platforms.telegram.layers import (
         InlineKeyboard,
         ReplyKeyboard,
         ReplyKeyboardRemove,
     )
 
     try:
```

### Comparing `bernard-0.6.0/src/bernard/platforms/telegram/layers.py` & `bernard-0.7.0/src/bernard/platforms/telegram/layers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from hashlib import md5
-from typing import Any, Dict, List, Optional, Text
+from typing import Any, Dict, List, Optional
 
-import ujson
+import orjson
 
 from bernard.engine.request import Request
 from bernard.i18n.intents import Intent
 from bernard.i18n.translator import TransText, render
 from bernard.layers import Markdown, Stack
 from bernard.layers import Text as TextLayer
 from bernard.layers.definitions import BaseLayer
 from bernard.utils import patch_dict
 
 from ._utils import set_reply_markup
 
 
-class InlineKeyboardButton(object):
+class InlineKeyboardButton:
     """
     Represents an inline keyboard button
     """
 
     def __init__(self, text: TransText):
         """
         See https://core.telegram.org/bots/api#inlinekeyboardmarkup
         """
-
         self.text = text
 
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return {
             "text": await render(self.text, request),
         }
 
@@ -35,80 +34,78 @@
         return self.text
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.text == other.text
 
 
 class InlineKeyboardUrlButton(InlineKeyboardButton):
-    def __init__(self, text: TransText, url: Text, sign_webview: bool = False):
-        super(InlineKeyboardUrlButton, self).__init__(text)
+    def __init__(self, text: TransText, url: str, sign_webview: bool = False):
+        super().__init__(text)
         self.url = url
         self.sign_webview = sign_webview
 
     async def make_url(self, request: Optional[Request]):
         if request and self.sign_webview:
             return await request.sign_url(self.url)
 
         return self.url
 
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return patch_dict(
-            await super(InlineKeyboardUrlButton, self).serialize(request),
+            await super().serialize(request),
             url=await self.make_url(request),
         )
 
     def __eq__(self, other):
         return (
             self.__class__ == other.__class__
             and self.text == other.text
             and self.url == other.url
         )
 
 
 class InlineKeyboardCallbackButton(InlineKeyboardButton):
     def __init__(self, text: TransText, payload: Any):
-        super(InlineKeyboardCallbackButton, self).__init__(text)
+        super().__init__(text)
         self.payload = payload
 
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return patch_dict(
-            await super(InlineKeyboardCallbackButton, self).serialize(request),
-            callback_data=ujson.dumps(self.payload),
+            await super().serialize(request),
+            callback_data=orjson.dumps(self.payload).decode(),
         )
 
     def __eq__(self, other):
         return (
             self.__class__ == other.__class__
             and self.text == other.text
             and self.payload == other.payload
         )
 
 
 class InlineKeyboardSwitchInlineQueryButton(InlineKeyboardButton):
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return patch_dict(
-            await super(InlineKeyboardSwitchInlineQueryButton, self).serialize(request),
+            await super().serialize(request),
             switch_inline_query=True,
         )
 
 
 class InlineKeyboardSwitchInlineQueryCurrentChatButton(InlineKeyboardButton):
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return patch_dict(
-            await super(
-                InlineKeyboardSwitchInlineQueryCurrentChatButton, self
-            ).serialize(request),
+            await super().serialize(request),
             switch_inline_query_current_chat=True,
         )
 
 
 class InlineKeyboardPayButton(InlineKeyboardButton):
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return patch_dict(
-            await super(InlineKeyboardPayButton, self).serialize(request),
+            await super().serialize(request),
             pay=True,
         )
 
 
 class InlineKeyboard(BaseLayer):
     def __init__(self, rows: List[List[InlineKeyboardButton]]):
         self.rows = rows
@@ -116,15 +113,15 @@
     async def serialize(self, request: Optional[Request] = None):
         out = []
 
         for row in self.rows:
             row_ser = []
 
             for button in row:
-                row_ser.append(await button.serialize(request))
+                row_ser.append(await button.serialize(request))  # noqa: PERF401
 
             out.append(row_ser)
 
         return {
             "inline_keyboard": out,
         }
 
@@ -141,26 +138,26 @@
     generate an empty AnswerCallbackQuery when a callback query is sent, but
     if you place one in the answer then it will be sent in place of the default
     one.
     """
 
     def __init__(
         self,
-        text: Optional[Text] = None,
+        text: Optional[str] = None,
         show_alert: Optional[bool] = None,
-        url: Optional[Text] = None,
+        url: Optional[str] = None,
         cache_time: Optional[int] = None,
     ):
         self.text = text
         self.show_alert = show_alert
         self.url = url
         self.cache_time = cache_time
 
     async def serialize(
-        self, callback_query_id: Text, request: Optional[Request] = None
+        self, callback_query_id: str, request: Optional[Request] = None
     ) -> Dict:
         out = {
             "callback_query_id": callback_query_id,
         }
 
         if self.text:
             out["text"] = await render(self.text, request)
@@ -221,52 +218,52 @@
     def __eq__(self, other):
         return self.__class__ == other.__class__
 
     def _repr_arguments(self):
         return []
 
 
-class KeyboardButton(object):
+class KeyboardButton:
     def __init__(
         self,
         text: TransText,
-        choice: Optional[Text] = None,
+        choice: Optional[str] = None,
         intent: Optional[Intent] = None,
     ) -> None:
         self.text = text
         self.choice = choice
         self.intent = intent
         self._chosen_text = None
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.text == other.text
 
-    async def get_chosen_text(self, request: Optional[Request] = None) -> Text:
+    async def get_chosen_text(self, request: Optional[Request] = None) -> str:
         if self._chosen_text is None:
             self._chosen_text = await render(self.text, request)
         return self._chosen_text
 
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return {
             "text": await self.get_chosen_text(request),
         }
 
 
 class ContactKeyboardButton(KeyboardButton):
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return patch_dict(
-            await super(ContactKeyboardButton, self).serialize(request),
+            await super().serialize(request),
             request_contact=True,
         )
 
 
 class LocationKeyboardButton(KeyboardButton):
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         return patch_dict(
-            await super(LocationKeyboardButton, self).serialize(request),
+            await super().serialize(request),
             request_location=True,
         )
 
 
 class ReplyKeyboard(BaseLayer):
     def __init__(
         self,
@@ -274,15 +271,14 @@
         resize_keyboard: Optional[bool] = None,
         one_time_keyboard: Optional[bool] = None,
         selective: Optional[bool] = None,
     ) -> None:
         """
         See https://core.telegram.org/bots/api#replykeyboardmarkup
         """
-
         self.keyboard = keyboard
         self.resize_keyboard = resize_keyboard
         self.one_time_keyboard = one_time_keyboard
         self.selective = selective
 
     def __eq__(self, other):
         return (
@@ -299,15 +295,15 @@
     async def serialize(self, request: Optional[Request] = None) -> Dict:
         out = {"keyboard": []}
 
         for row in self.keyboard:
             row_ser = []
 
             for button in row:
-                row_ser.append(await button.serialize(request))
+                row_ser.append(await button.serialize(request))  # noqa: PERF401
 
             out["keyboard"].append(row_ser)
 
         if self.resize_keyboard is not None:
             out["resize_keyboard"] = self.resize_keyboard
 
         if self.one_time_keyboard is not None:
@@ -378,24 +374,24 @@
             and self.inline_query == other.inline_query
         )
 
     def _repr_arguments(self):
         return [self.query]
 
 
-class InlineQueryResult(object):
+class InlineQueryResult:
     TYPE = None
 
     def __init__(self, identifiers: Dict, input_stack: Stack):
         self.identifiers = identifiers
         self.input_stack = input_stack
 
     @property
     def unique_id(self):
-        h = md5()
+        h = md5()  # noqa: S324
 
         for k in sorted(self.identifiers.keys()):
             h.update(f"{k}={self.identifiers[k]}".encode())
 
         return h.hexdigest()
 
     def __eq__(self, other):
@@ -432,33 +428,33 @@
     TYPE = "article"
 
     def __init__(
         self,
         identifiers: Dict,
         input_stack: Stack,
         title: TransText,
-        url: Optional[Text] = None,
+        url: Optional[str] = None,
         hide_url: Optional[bool] = None,
-        description: Optional[Text] = None,
-        thumb_url: Optional[Text] = None,
+        description: Optional[str] = None,
+        thumb_url: Optional[str] = None,
         thumb_width: Optional[int] = None,
         thumb_height: Optional[int] = None,
     ):
-        super(InlineQueryResultArticle, self).__init__(identifiers, input_stack)
+        super().__init__(identifiers, input_stack)
 
         self.title = title
         self.url = url
         self.hide_url = hide_url
         self.description = description
         self.thumb_url = thumb_url
         self.thumb_width = thumb_width
         self.thumb_height = thumb_height
 
     async def serialize(self, request: Optional[Request] = None):
-        out = await super(InlineQueryResultArticle, self).serialize(request)
+        out = await super().serialize(request)
 
         out["title"] = await render(self.title, request)
         fields = [
             "url",
             "hide_url",
             "description",
             "thumb_url",
@@ -511,18 +507,15 @@
             and self.is_personal == other.is_personal
         )
 
     def _repr_arguments(self):
         return self.results
 
     async def serialize(self, request: Optional[Request] = None):
-        results = []
-
-        for result in self.results:
-            results.append(await result.serialize(request))
+        results = [await result.serialize(request) for result in self.results]
 
         out = {
             "inline_query_id": self.inline_query_id,
             "results": results,
         }
 
         if self.cache_time is not None:
@@ -547,15 +540,15 @@
 
 
 class BotCommand(BaseLayer):
     """
     That is when the user sends a command to the bot
     """
 
-    def __init__(self, command: Text):
+    def __init__(self, command: str):
         self.command = command
 
     def _repr_arguments(self):
         return [self.command]
 
     def __eq__(self, other):
         return self.__class__ == other.__class__ and self.command == other.command
```

### Comparing `bernard-0.6.0/src/bernard/platforms/telegram/media.py` & `bernard-0.7.0/src/bernard/platforms/telegram/media.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional, Text
+from typing import Dict, List, Optional
 
 from bernard.media.base import BaseMedia
 
 
 class Photo(BaseMedia):
     """
     Abstract object over a Telegram photo object
@@ -16,13 +16,13 @@
             [
                 self.__class__ == other.__class__,
                 self.files == other.files,
             ]
         )
 
     def __repr__(self):
-        return f"Photo({repr(self.largest_id())})"
+        return f"Photo({self.largest_id()!r})"
 
-    def largest_id(self) -> Optional[Text]:
+    def largest_id(self) -> Optional[str]:
         # noinspection PyTypeChecker
         largest = max(self.files, key=lambda f: f["file_size"], default=None)
         return largest["file_id"]
```

### Comparing `bernard-0.6.0/src/bernard/platforms/telegram/platform.py` & `bernard-0.7.0/src/bernard/platforms/telegram/platform.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+import asyncio
 import logging
+import time
 from asyncio import Lock, sleep
 from datetime import tzinfo
 from hashlib import sha256
-from typing import Any, Dict, List, Optional, Set, Text
+from typing import Any, ClassVar, Dict, List, Literal, Optional
 from urllib.parse import quote, urljoin
 
+import httpx
 import jwt
-import ujson
+import orjson
 from aiohttp.web_request import Request
 from aiohttp.web_response import json_response
 from aiohttp.web_urldispatcher import UrlDispatcher
+from sentry_sdk import capture_exception
 
 from bernard import layers as lyr
 from bernard.conf import settings
 from bernard.core.health_check import HealthCheckFail
 from bernard.engine.platform import PlatformOperationError
-from bernard.engine.request import BaseMessage, Conversation
+from bernard.engine.request import BaseMessage, Conversation, User
 from bernard.engine.request import Request as BernardRequest
-from bernard.engine.request import User
 from bernard.engine.responder import Layers, Responder
 from bernard.i18n import render
 from bernard.layers import BaseLayer, Stack
 from bernard.media.base import BaseMedia
-from bernard.utils import patch_dict, patch_qs
+from bernard.utils import patch_dict
 
 from ...platforms import SimplePlatform
 from ._utils import set_reply_markup
 from .layers import (
     AnswerCallbackQuery,
     AnswerInlineQuery,
     BotCommand,
@@ -45,15 +48,15 @@
 class TelegramConversation(Conversation):
     """
     Matches the Telegram "chat" concept
     """
 
     def __init__(self, chat):
         self._chat = chat
-        super(TelegramConversation, self).__init__(self._make_id())
+        super().__init__(self._make_id())
 
     def _make_id(self):
         if "is_inline_query" in self._chat:
             return f'telegram:inline_query:{self._chat["id"]}'
         else:
             return f'telegram:conversation:{self._chat["id"]}'
 
@@ -61,15 +64,15 @@
 class TelegramUser(User):
     def __init__(self, user, chat, telegram: "Telegram"):
         self._user = user
         self._chat = chat
         self._telegram = telegram
         self._full_user = None
         self._lock = Lock()
-        super(TelegramUser, self).__init__(self._make_id())
+        super().__init__(self._make_id())
 
     def _make_id(self):
         return f'telegram:user:{self._user["id"]}'
 
     async def _get_full_user(self) -> Dict:
         """
         Sometimes Telegram does not provide all the user info with the message.
@@ -77,59 +80,57 @@
         call this method which will make sure that the full User object is
         loaded.
 
         The result is cached for the lifetime of the object, so if the function
         is called multiple times it will only fetch the user once. There is
         a locking mechanism around the cache to allow concurrent calls.
         """
-
         if "language_code" in self._user:
             return self._user
 
         async with self._lock:
             if self._full_user is None:
                 cm = await self._telegram.call(
                     "getChatMember",
                     user_id=self._user["id"],
                     chat_id=self._chat["id"],
                 )
                 self._full_user = cm["result"]["user"]
 
             return self._full_user
 
-    async def get_friendly_name(self) -> Text:
+    async def get_friendly_name(self) -> str:
         """
         Let's use the first name of the user as friendly name. In some cases
         the user object is incomplete, and in those cases the full user is
         fetched.
         """
-
         if "first_name" not in self._user:
             user = await self._get_full_user()
         else:
             user = self._user
 
         return user.get("first_name")
 
-    async def get_locale(self) -> Text:
+    async def get_locale(self) -> str:
         user = await self._get_full_user()
-        return user.get("language_code", None)
+        return user.get("language_code", "")
 
-    async def get_formal_name(self) -> Text:
+    async def get_formal_name(self) -> str:
         parts = [
             self._user.get("first_name"),
             self._user.get("last_name"),
         ]
 
         return " ".join(x for x in parts if x)
 
     async def get_timezone(self) -> Optional[tzinfo]:
         return None
 
-    async def get_full_name(self) -> Text:
+    async def get_full_name(self) -> str:
         return await self.get_formal_name()
 
 
 class TelegramMessage(BaseMessage):
     def __init__(self, update: Dict, telegram: "Telegram"):
         self._update = update
         self._telegram = telegram
@@ -142,16 +143,16 @@
 
             if "text" in msg:
                 text = msg["text"]
                 out.append(lyr.RawText(text))
 
                 for entity in msg.get("entities") or []:
                     o = entity["offset"]
-                    l = entity["length"]
-                    entity_text = text[o : o + l]
+                    ln = entity["length"]
+                    entity_text = text[o : o + ln]
 
                     if entity["type"] == "bot_command":
                         out.append(BotCommand(entity_text))
 
             if "reply_to_message" in msg:
                 sub_msg = TelegramMessage(
                     {"message": msg["reply_to_message"]},
@@ -161,37 +162,36 @@
 
             if "photo" in msg:
                 media = Photo(msg["photo"])
                 out.append(lyr.Image(media))
 
         if "callback_query" in self._update:
             payload = self._update["callback_query"]["data"]
-            out.append(lyr.Postback(ujson.loads(payload)))
+            out.append(lyr.Postback(orjson.loads(payload)))
             out.append(InlineMessage())
 
             sub_msg = TelegramMessage(
                 self._update["callback_query"],
                 self._telegram,
             )
             out.append(lyr.Message(sub_msg))
 
         if "inline_query" in self._update:
             out.append(InlineQuery(self._update["inline_query"]))
 
         return out
 
-    def get_platform(self) -> Text:
+    def get_platform(self) -> str:
         return self._telegram.NAME
 
     def _get_chat(self) -> Dict:
         """
         As Telegram changes where the chat object is located in the response,
         this method tries to be smart about finding it in the right place.
         """
-
         if "callback_query" in self._update:
             query = self._update["callback_query"]
             if "message" in query:
                 return query["message"]["chat"]
             else:
                 return {"id": query["chat_instance"]}
         elif "inline_query" in self._update:
@@ -203,32 +203,31 @@
             return self._update["message"]["chat"]
 
     def _get_user(self) -> Dict:
         """
         Same thing as for `_get_chat()` but for the user related to the
         message.
         """
-
         if "callback_query" in self._update:
             return self._update["callback_query"]["from"]
         elif "inline_query" in self._update:
             return self._update["inline_query"]["from"]
         elif "message" in self._update:
             return self._update["message"]["from"]
 
     def get_conversation(self) -> Conversation:
         return TelegramConversation(self._get_chat())
 
     def get_user(self) -> User:
         return TelegramUser(self._get_user(), self._get_chat(), self._telegram)
 
-    def get_chat_id(self) -> Text:
+    def get_chat_id(self) -> str:
         return self._get_chat()["id"]
 
-    async def get_token(self) -> Text:
+    async def get_token(self) -> str:
         user = self.get_user()
         # noinspection PyUnresolvedReferences,PyProtectedMember
         user_id = user._user["id"]
         # noinspection PyUnresolvedReferences,PyProtectedMember
         chat_id = user._chat["id"]
 
         return jwt.encode(
@@ -243,119 +242,139 @@
 
 class TelegramResponder(Responder):
     """
     This responder handles most of the magic behind Telegram messages
     acknowledgements and so on.
     """
 
+    platform: "Telegram"
+
     def __init__(self, update, platform):
-        super(TelegramResponder, self).__init__(platform)
+        super().__init__(platform)
 
         self._update = update
 
         if "callback_query" in update:
             self._acq = AnswerCallbackQuery()
         else:
             self._acq = None
 
     def send(self, stack: Layers):
         """
         Intercept any potential "AnswerCallbackQuery" before adding the stack
         to the output buffer.
         """
-
         if not isinstance(stack, Stack):
             stack = Stack(stack)
 
+        self._send_update(stack)
+        stack = self._send_answer(stack)
+        self._send_reply(stack)
+        self._send_inline_query(stack)
+
+        if stack.layers:
+            return super().send(stack)
+
+    def _send_update(self, stack):
         if "callback_query" in self._update and stack.has_layer(Update):
             layer = stack.get_layer(Update)
 
             try:
                 msg = self._update["callback_query"]["message"]
             except KeyError:
                 layer.inline_message_id = self._update["callback_query"][
                     "inline_message_id"
                 ]
             else:
                 layer.chat_id = msg["chat"]["id"]
                 layer.message_id = msg["message_id"]
 
+    def _send_answer(self, stack):
         if stack.has_layer(AnswerCallbackQuery):
             self._acq = stack.get_layer(AnswerCallbackQuery)
+
             stack = Stack(
-                [l for l in stack.layers if not isinstance(l, AnswerCallbackQuery)]
+                [
+                    layer
+                    for layer in stack.layers
+                    if not isinstance(layer, AnswerCallbackQuery)
+                ]
             )
 
+        return stack
+
+    def _send_reply(self, stack):
         if stack.has_layer(Reply):
             layer = stack.get_layer(Reply)
 
             if "message" in self._update:
                 layer.message = self._update["message"]
             elif "callback_query" in self._update:
                 layer.message = self._update["callback_query"]["message"]
 
+    def _send_inline_query(self, stack):
         if "inline_query" in self._update and stack.has_layer(AnswerInlineQuery):
             a = stack.get_layer(AnswerInlineQuery)
             a.inline_query_id = self._update["inline_query"]["id"]
 
-        if stack.layers:
-            return super(TelegramResponder, self).send(stack)
-
     async def flush(self, request: BernardRequest):
         """
         If there's a AnswerCallbackQuery scheduled for reply, place the call
         before actually flushing the buffer.
         """
-
         if self._acq and "callback_query" in self._update:
             try:
                 cbq_id = self._update["callback_query"]["id"]
             except KeyError:
                 pass
             else:
                 await self.platform.call(
                     "answerCallbackQuery", **(await self._acq.serialize(cbq_id))
                 )
 
-        return await super(TelegramResponder, self).flush(request)
+        return await super().flush(request)
 
 
 class Telegram(SimplePlatform):
     NAME = "telegram"
-    PATTERNS = {
-        "plain_text": "^(Text|RawText)+ "
+    PATTERNS: ClassVar[dict[str, str]] = {
+        "plain_text": "^(Text|RawText|MultiText)+ "
         "(InlineKeyboard|ReplyKeyboard|ReplyKeyboardRemove)? "
         "Reply?$"
         "|^(Text|RawText) InlineKeyboard? Reply? Update$",
         "inline_answer": "^AnswerInlineQuery$",
         "markdown": "^Markdown+ "
         "(InlineKeyboard|ReplyKeyboard|ReplyKeyboardRemove)? "
         "Reply?$"
         "|^Markdown InlineKeyboard? Reply? Update$",
         "sleep": "^Sleep$",
         "typing": "^Typing$",
     }
 
+    def __init__(self):
+        super().__init__()
+        self._polling_t = None
+
     @classmethod
     async def self_check(cls):
         """
         Check that the configuration is correct
 
         - Presence of "token" in the settings
         - Presence of "BERNARD_BASE_URL" in the global configuration
         """
-
         # noinspection PyTypeChecker
-        async for check in super(Telegram, cls).self_check():
+        async for check in super().self_check():
             yield check
 
         s = cls.settings()
 
         try:
-            assert isinstance(s["token"], str)
+            if not isinstance(s["token"], str):
+                raise AssertionError
         except (KeyError, TypeError, AssertionError):
             yield HealthCheckFail(
                 "00005",
                 'Missing "token" for Telegram platform. You can obtain one by'
                 "registering your bot in Telegram.",
             )
 
@@ -371,26 +390,89 @@
             yield HealthCheckFail(
                 "00005",
                 '"WEBVIEW_SECRET_KEY" cannot be found in the configuration. '
                 "It is required in order to be able to create secure postback "
                 "URLs.",
             )
 
+    @property
+    def telegram_update_mode(self) -> Literal["polling", "webhook"]:
+        """Determining from settings how we are supposed to receive updates.
+
+        Telegram supports two modes: either the webhook, which calls an HTTP
+        hook on your behalf, which is good at scale if you want to have several
+        servers answer requests etc. But this framework is pretty lightweight,
+        so before you need to scale horizontally there is probably a lot of
+        time that will pass.
+
+        Instead, the recommended way for most people is to use the polling
+        method. The huge advantage of it is that you don't need a public URL
+        for your bot, so it's ideal for development environments. The only
+        drawback is that you can't scale horizontally with it.
+        """
+
+        return self.settings().get("update_mode", "polling")
+
     def hook_up(self, router: UrlDispatcher):
-        router.add_post(self.make_hook_path(), self.receive_updates)
+        if self.telegram_update_mode == "webhook":
+            router.add_post(self.make_hook_path(), self.receive_updates)
+
+    async def _poll_updates(self):
+        """Using the poll method for Telegram updates.
+
+        It's very simple, you just call the same endpoint repeatedly until you
+        get an answer, this forever and ever.
+        """
+
+        min_time = 1
+        offset = 0
+
+        while True:
+            time_start = time.time()
+
+            try:
+                updates = await self.call(
+                    "getUpdates",
+                    _log=False,
+                    offset=offset,
+                    timeout=5,
+                    allowed_updates=[
+                        "message",
+                        "callback_query",
+                        "inline_query",
+                    ],
+                )
+
+                for update in updates["result"]:
+                    message = TelegramMessage(update, self)
+                    responder = TelegramResponder(update, self)
+                    await self._notify(message, responder)
+
+                if updates["result"]:
+                    offset = max(x["update_id"] for x in updates["result"]) + 1
+            except httpx.ReadTimeout:
+                pass
+            except Exception as e:
+                capture_exception(e)
+                logger.exception("Error while polling Telegram: %s")
+
+            time_end = time.time()
+            time_diff = time_end - time_start
+
+            if time_diff < min_time:
+                await sleep(min_time - time_diff)
 
     async def receive_updates(self, request: Request):
         """
         Handle updates from Telegram
         """
-
         body = await request.read()
 
         try:
-            content = ujson.loads(body)
+            content = orjson.loads(body)
         except ValueError:
             return json_response(
                 {
                     "error": True,
                     "message": "Cannot decode body",
                 },
                 status=400,
@@ -405,164 +487,187 @@
         return json_response(
             {
                 "error": False,
             }
         )
 
     async def message_from_token(
-        self, token: Text, payload: Any
+        self, token: str, payload: Any
     ) -> Optional[BaseMessage]:
         try:
             tk = jwt.decode(token, settings.WEBVIEW_SECRET_KEY)
         except jwt.InvalidTokenError:
-            return
+            return None
 
         try:
             user_id = tk["telegram_user_id"]
-            assert isinstance(user_id, int)
+
+            if not isinstance(user_id, int):
+                raise AssertionError
+
             chat_id = tk["telegram_chat_id"]
-            assert isinstance(chat_id, int)
+
+            if not isinstance(chat_id, int):
+                raise AssertionError
         except (KeyError, AssertionError):
-            return
+            return None
 
         fake_message = {
             "callback_query": {
                 "from": {
                     "id": user_id,
                 },
                 "message": {
                     "chat": {
                         "id": chat_id,
                     },
                 },
-                "data": ujson.dumps(payload),
+                "data": orjson.dumps(payload).decode(),
             }
         }
 
         return TelegramMessage(fake_message, self)
 
     async def inject_message(self, message: TelegramMessage) -> None:
         # noinspection PyProtectedMember
         responder = TelegramResponder(message._update, self)
         await self._notify(message, responder)
 
-        return json_response(
-            {
-                "error": False,
-            }
-        )
-
     def make_url(self, method):
         """
         Generate a Telegram URL for this bot.
         """
-
         token = self.settings()["token"]
 
         return TELEGRAM_URL.format(
             token=quote(token),
             method=quote(method),
         )
 
-    async def call(self, method: Text, _ignore: Set[Text] = None, **params: Any):
+    async def call(
+        self,
+        method: str,
+        _ignore: set[str] | None = None,
+        _log: bool = True,
+        **params: Any,
+    ):
         """
         Call a telegram method
 
         :param _ignore: List of reasons to ignore
+        :param _log: Whether to log the call or not
         :param method: Name of the method to call
         :param params: Dictionary of the parameters to send
 
         :return: Returns the API response
         """
-
-        logger.debug("Calling Telegram %s(%s)", method, params)
+        if _log:
+            logger.debug("Calling Telegram %s(%s)", method, params)
 
         url = self.make_url(method)
 
         headers = {
             "content-type": "application/json",
         }
 
-        post = self.session.post(
-            url,
-            data=ujson.dumps(params),
-            headers=headers,
-        )
-
-        async with post as r:
+        async with httpx.AsyncClient() as client:
+            r = await client.post(
+                url,
+                json=params,
+                headers=headers,
+            )
             out = await self._handle_telegram_response(r, _ignore)
-            logger.debug("Telegram replied: %s", out)
+
+            if _log:
+                logger.debug("Telegram replied: %s", out)
+
             return out
 
-    async def _handle_telegram_response(self, response, ignore=None):
+    async def _handle_telegram_response(self, response: httpx.Response, ignore=None):
         """
         Parse a response from Telegram. If there's an error, an exception will
         be raised with an explicative message.
 
         :param response: Response to parse
         :return: Data
         """
-
         if ignore is None:
             ignore = set()
 
-        ok = response.status == 200
+        ok = response.status_code == 200
 
         try:
-            data = await response.json()
+            data = response.json()
 
             if not ok:
                 desc = data["description"]
 
                 if desc in ignore:
-                    return
+                    return None
 
-                raise PlatformOperationError(
-                    "Telegram replied with an error: {}".format(desc)
-                )
+                msg = f"Telegram replied with an error: {desc}"
+                raise PlatformOperationError(msg)
         except (ValueError, TypeError, KeyError):
-            raise PlatformOperationError("An unknown Telegram error occurred")
+            msg = "An unknown Telegram error occurred"
+            raise PlatformOperationError(msg) from None
 
         return data
 
     def make_hook_path(self):
         """
         Compute the path to the hook URL
         """
-
         token = self.settings()["token"]
         h = sha256()
         h.update(token.encode())
         key = str(h.hexdigest())
         return f"/hooks/telegram/{key}"
 
     async def _deferred_init(self):
         """
-        Register the web hook onto which Telegram should send its messages.
-        """
+        Make sure that the webhook is in the required state. In case of polling
+        the webhook is disabled and a polling task is started, in case of
+        webhook the webhook is set.
+        """
+        if self.telegram_update_mode == "webhook":
+            hook_path = self.make_hook_path()
+            url = urljoin(settings.BERNARD_BASE_URL, hook_path)
+            await self.call("setWebhook", url=url)
+            logger.info('Setting Telegram webhook to "%s"', url)
+        else:
+            info = await self.call("getWebhookInfo")
 
-        hook_path = self.make_hook_path()
-        url = urljoin(settings.BERNARD_BASE_URL, hook_path)
-        await self.call("setWebhook", url=url)
-        logger.info('Setting Telegram webhook to "%s"', url)
+            if url := info["result"]["url"]:
+                logger.info(
+                    (
+                        'Telegram webhook is set to "%s", disabling it '
+                        "because polling is enabled"
+                    ),
+                    url,
+                )
+                await self.call("deleteWebhook")
+
+            self._polling_t = asyncio.create_task(self._poll_updates())
 
     async def _send_text(
-        self, request: Request, stack: Stack, parse_mode: Optional[Text] = None
+        self, request: Request, stack: Stack, parse_mode: Optional[str] = None
     ):
         """
         Base function for sending text
         """
-
         parts = []
         chat_id = request.message.get_chat_id()
 
         for layer in stack.layers:
             if isinstance(layer, (lyr.Text, lyr.RawText, lyr.Markdown)):
                 text = await render(layer.text, request)
                 parts.append(text)
+            elif isinstance(layer, lyr.MultiText):
+                lines = await render(layer.text, request, multi_line=True)
+                parts.extend(lines)
 
         for part in parts[:-1]:
             await self.call(
                 "sendMessage",
                 text=part,
                 chat_id=chat_id,
             )
@@ -597,44 +702,40 @@
         else:
             await self.call("sendMessage", **msg)
 
     async def _send_plain_text(self, request: Request, stack: Stack):
         """
         Sends plain text using `_send_text()`.
         """
-
         await self._send_text(request, stack, None)
 
     async def _send_markdown(self, request: Request, stack: Stack):
         """
         Sends Markdown using `_send_text()`
         """
-
         await self._send_text(request, stack, "Markdown")
 
     async def _send_sleep(self, request: Request, stack: Stack):
         """
         Sleep for the amount of time specified in the Sleep layer
         """
-
         duration = stack.get_layer(lyr.Sleep).duration
         await sleep(duration)
 
     async def _send_inline_answer(self, request: Request, stack: Stack):
         aiq = stack.get_layer(AnswerInlineQuery)
         answer = await aiq.serialize(request)
         await self.call("answerInlineQuery", **answer)
 
     async def _send_typing(self, request: Request, stack: Stack):
         """
         In telegram, the typing stops when the message is received. Thus, there
         is no "typing stops" messages to send. The API is only called when
         typing must start.
         """
-
         t = stack.get_layer(lyr.Typing)
 
         if t.active:
             await self.call(
                 "sendChatAction",
                 chat_id=request.message.get_chat_id(),
                 action="typing",
```

### Comparing `bernard-0.6.0/src/bernard/platforms/test/platform.py` & `bernard-0.7.0/src/bernard/platforms/test/platform.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,31 @@
-from typing import List, Text, Tuple, Type
+from typing import Tuple, Type
 
 from bernard.engine.fsm import FSM
 from bernard.engine.platform import Platform
 from bernard.engine.request import BaseMessage, Conversation, Request, User
 from bernard.engine.responder import Responder
 from bernard.engine.state import BaseState
 from bernard.layers import BaseLayer, Stack
 from bernard.media.base import BaseMedia
 from bernard.storage.register import Register
-from bernard.utils import run
 
 
 class TestUser(User):
     """
     Mock user object
     """
 
-    def get_friendly_name(self) -> Text:
+    def get_friendly_name(self) -> str:
         return "Test"
 
-    def get_formal_name(self) -> Text:
+    def get_formal_name(self) -> str:
         return "Formal Test"
 
-    def get_full_name(self) -> Text:
+    def get_full_name(self) -> str:
         return "Full Test"
 
     async def get_timezone(self):
         return None
 
     async def get_locale(self):
         return None
@@ -94,15 +93,15 @@
     """
 
     NAME = "test"
 
     fsm_creates_task = False
 
     def __init__(self):
-        super(TestPlatform, self).__init__()
+        super().__init__()
         self.sent = []  # type: List[Stack]
 
     async def send(self, request: Request, stack: Stack):
         """
         Store the message to be sent for later analysis
         """
         self.sent.append(stack)
@@ -110,60 +109,56 @@
     def accept(self, stack: Stack):
         """
         So far we accept anything, it's up to the test to test that things sent
         are the right ones.
         """
         return True
 
-    def handle(self, *layers: BaseLayer):
+    async def handle(self, *layers: BaseLayer):
         """
-        Call this method to send a test message. Call it OUTSIDE the async
-        loop. It will return when the message is fully handled.
+        Call this method to send a test message. It will return when the
+        message is fully handled.
         """
-
         self.sent = []
         stack = Stack(list(layers))
         message = TestMessage(stack)
         responder = TestResponder(self)
 
-        run(self._notify(message, responder))
+        await self._notify(message, responder)
 
     def assert_sent(self, *stacks: Stack):
         """
         Assert that the sent stacks are identical to the ones provided as
         argument here.
         """
-
         assert len(stacks) == len(self.sent)
 
         for s1, s2 in zip(stacks, self.sent):
             assert s1 == s2
 
     def assert_state(self, state_class: Type[BaseState]):
         """
         Assert that the state returned in the register is the one passed as
         argument.
         """
-
         assert self._register
         assert Register.STATE in self._register
         assert self._register[Register.STATE] == state_class.name()
 
     def ensure_usable_media(self, media: BaseMedia) -> BaseMedia:
         return media
 
 
-def make_test_fsm() -> Tuple[FSM, TestPlatform]:
+async def make_test_fsm() -> Tuple[FSM, TestPlatform]:
     """
-    Generate both a FSM and a test platform for unit testing purposes.
+    Generate both an FSM and a test platform for unit testing purposes.
 
-    The will use the current configuration to load stories and transitions.
+    They will use the current configuration to load stories and transitions.
     """
-
     fsm = FSM()
-    run(fsm.async_init())
+    await fsm.async_init()
 
     platform = TestPlatform()
     # noinspection PyTypeChecker
     platform.on_message(fsm.handle_message)
 
     return fsm, platform
```

### Comparing `bernard-0.6.0/src/bernard/server/views.py` & `bernard-0.7.0/src/bernard/server/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,33 +83,33 @@
 
 
 @bernard_auth
 async def postback_send(msg: BaseMessage, platform: Platform) -> Response:
     """
     Injects the POST body into the FSM as a Postback message.
     """
-
     await platform.inject_message(msg)
 
     return json_response(
         {
             "status": "ok",
         }
     )
 
 
 @bernard_auth
 async def postback_analytics(msg: BaseMessage, platform: Platform) -> Response:
     """
     Makes a call to an analytics function.
     """
-
     try:
         pb = msg.get_layers()[0]
-        assert isinstance(pb, Postback)
+
+        if not isinstance(pb, Postback):
+            raise AssertionError
 
         user = msg.get_user()
         user_lang = await user.get_locale()
         user_id = user.id
 
         if pb.payload["event"] == "page_view":
             func = "page_view"
@@ -139,13 +139,12 @@
         )
 
 
 async def health_check(request: Request) -> Response:
     """
     A simple non-authenticated endpoint to check the health of the process.
     """
-
     return json_response(
         {
             "status": "ok",
         }
     )
```

### Comparing `bernard-0.6.0/src/bernard/storage/context/base.py` & `bernard-0.7.0/src/bernard/storage/context/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from functools import wraps
-from typing import Any, Dict, Iterator, List, Optional, Text, Union
+from typing import Any, Dict, Iterator, List, Optional, Union
 
 from bernard.conf import settings
 from bernard.core.health_check import HealthCheckFail
 from bernard.engine.state import BaseState
 from bernard.engine.triggers import BaseTrigger
 from bernard.utils import import_class
 
-Context = Dict[Text, Any]
+Context = Dict[str, Any]
 
 
 def create_context_store(
     name="default", ttl=settings.CONTEXT_DEFAULT_TTL, store=settings.CONTEXT_STORE
 ) -> "BaseContextStore":
     """
     Create a context store. By default using the default configured context
@@ -38,20 +38,19 @@
     >>>         self.send(lyr.Text('`foo` is not in context'))
 
     This requires that `foo` is present in the context in order to enter the
     handler.
 
     See `BaseContextStore.inject()` for more info.
     """
-
     store_class = import_class(store["class"])
     return store_class(name=name, ttl=ttl, **store["params"])
 
 
-class BaseContextStore(object):
+class BaseContextStore:
     """
     Defines the interface of a context store.
 
     The context store stores a dictionary object in whichever way it wants (by
     example in a Redis database). Each context is a plain dictionary object.
     Each context is created for one conversation and expires after X seconds.
 
@@ -59,57 +58,56 @@
     method.
 
     For a user of this class, the main entry point is `inject()`.
     """
 
     def __init__(self, name, ttl, **kwargs):
         # noinspection PyArgumentList
-        super(BaseContextStore, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
         self.name = name
         self.ttl = ttl
         self._init_done = False
 
     async def async_init(self) -> None:
         pass
 
     async def ensure_async_init(self) -> None:
         """
         This allows to lazily do the async init
         """
-
         if not self._init_done:
             await self.async_init()
             self._init_done = True
 
-    async def _get(self, key: Text) -> Context:
+    async def _get(self, key: str) -> Context:
         """
         Implement this as a method to get the context for the given key.
         """
         raise NotImplementedError
 
-    async def _set(self, key: Text, data: Context) -> None:
+    async def _set(self, key: str, data: Context) -> None:
         """
         Implement this as a method to set the context at the given key.
         """
         raise NotImplementedError
 
-    def open(self, key: Text) -> "ContextContextManager":
+    def open(self, key: str) -> "ContextContextManager":
         """
         Opens a context using the a Python context manager.
 
         The `key` is the arbitrary key identifying the context.
         """
         return ContextContextManager(key, self)
 
     def inject(
         self,
-        require: Optional[List[Text]] = None,
-        fail: Text = "missing_context",
-        var_name: Text = "context",
+        require: Optional[List[str]] = None,
+        fail: str = "missing_context",
+        var_name: str = "context",
     ):
         """
         This is a decorator intended to be used on states (and actually only
         work on state handlers).
 
         The `require` argument is a list of keys to be checked in the context.
         If at least one of them is missing, then instead of calling the handler
@@ -152,35 +150,33 @@
 
             return wrapper
 
         return decorator
 
 
 # noinspection PyProtectedMember
-class ContextContextManager(object):
+class ContextContextManager:
     """
     A (Python) context manager to handle the opening and saving/closing of the
     (Bernard) context.
     """
 
-    def __init__(self, key: Text, store: BaseContextStore):
+    def __init__(self, key: str, store: BaseContextStore):
         self.key = key
         self.data = None
         self.store = store
 
     async def __aenter__(self):
         """
         When we enter the (Python) context, we load the (Bernard) context into
         a plain dictionary and return it.
         """
-
         await self.store.ensure_async_init()
         self.data = await self.store._get(self.key)
         return self.data
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         """
         When leaving the (Python) context, the (Bernard) context is sent back
         to the storage for saving.
         """
-
         await self.store._set(self.key, self.data)
```

### Comparing `bernard-0.6.0/src/bernard/storage/context/redis.py` & `bernard-0.7.0/src/bernard/storage/context/redis.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-from typing import Text
-
-import ujson
+import orjson
 
 from ..redis import BaseRedisStore
 from .base import BaseContextStore, Context
 
 
 class RedisContextStore(BaseRedisStore, BaseContextStore):
     """
     Store the context as a serialized JSON inside Redis. It's made to be
     compatible with the register storage, if using the same Redis DB.
     """
 
-    async def _get(self, key: Text) -> Context:
+    async def _get(self, key: str) -> Context:
         try:
-            return ujson.loads(await self.redis.get(key))
+            return orjson.loads(await self.redis.get(key))
         except (ValueError, TypeError):
             return {}
 
-    async def _set(self, key: Text, data: Context) -> None:
-        await self.redis.set(key, ujson.dumps(data), ex=self.ttl)
+    async def _set(self, key: str, data: Context) -> None:
+        await self.redis.set(key, orjson.dumps(data), ex=self.ttl)
```

### Comparing `bernard-0.6.0/src/bernard/storage/redis.py` & `bernard-0.7.0/src/bernard/storage/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from typing import Text
-
 from redis import asyncio as aioredis
 
 
-class BaseRedisStore(object):
+class BaseRedisStore:
     def __init__(
         self,
-        protocol: Text = "redis",
-        host: Text = "localhost",
+        protocol: str = "redis",
+        host: str = "localhost",
         port: int = 6379,
         db_id: int = 0,
         min_pool_size: int = 5,
         max_pool_size: int = 10,
         **kwargs,
     ):
         """
@@ -22,27 +20,25 @@
 
         :param host: IP/DNS host
         :param port: TCP port
         :param db_id: ID of the DB
         :param min_pool_size: minimum number of connections alive
         :param max_pool_size: maximum number of connections alive
         """
-
         # noinspection PyArgumentList
-        super(BaseRedisStore, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
         self.protocol = protocol
         self.host = host
         self.port = port
         self.db_id = db_id
         self.min_pool_size = min_pool_size
         self.max_pool_size = max_pool_size
         self.redis = None
 
     async def async_init(self):
         """
         Handle here the asynchronous part of the init.
         """
-
         self.redis = await aioredis.from_url(
             f"{self.protocol}://{self.host}:{self.port}/{self.db_id}"
         )
```

### Comparing `bernard-0.6.0/src/bernard/storage/register/base.py` & `bernard-0.7.0/src/bernard/storage/register/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Dict, Optional, Text
+from typing import Any, Dict
 
 from bernard.utils import RoDict
 
 logger = logging.getLogger("bernard.storage.register")
 
 
 class Register(RoDict):
@@ -16,19 +16,19 @@
     STATE = "state"
 
     def __init__(self, *args, **kwargs):
         """
         Create a "replacement" member, that external classes can read to see
         if there is some replacement data ready.
         """
-        super(Register, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.replacement = None  # type: Optional[Dict[Text, Any]]
 
 
-class BaseRegisterStore(object):
+class BaseRegisterStore:
     """
     Interface for register storage.
 
     The register is atomic: you read it all at once, lock out other readers
     and then save it all at once.
 
     You can use it like this:
@@ -49,78 +49,76 @@
 
     async def async_init(self):
         """
         This is just a placeholder in case a subclass needs to overload it.
         """
         pass
 
-    def work_on_register(self, key: Text) -> "RegisterContextManager":
+    def work_on_register(self, key: str) -> "RegisterContextManager":
         """
         Create the context manager
         """
         return RegisterContextManager(key, self)
 
-    async def _start(self, key: Text) -> None:
+    async def _start(self, key: str) -> None:
         """
         That's when you start working on a key. You should start locking here.
         """
         raise NotImplementedError
 
-    async def _get(self, key: Text) -> Dict[Text, Any]:
+    async def _get(self, key: str) -> Dict[str, Any]:
         """
         There you fetch the data of the register.
         """
         raise NotImplementedError
 
-    async def _replace(self, key: Text, data: Dict[Text, Any]) -> None:
+    async def _replace(self, key: str, data: Dict[str, Any]) -> None:
         """
         This function will be called if there is a replacement in order to
         store it into the register. This will be called only once by the
         context manager, even if the replacement was set several times (only
         the last value counts).
         """
         raise NotImplementedError
 
-    async def _finish(self, key: Text) -> None:
+    async def _finish(self, key: str) -> None:
         """
         This is called when everything is done. You should release the lock
         here. This will get called even if the replace failed.
         """
         raise NotImplementedError
 
 
 # noinspection PyProtectedMember
-class RegisterContextManager(object):
+class RegisterContextManager:
     """
     Handles the context of the register: call the right methods of the storage
     at the right time and provide the register.
     """
 
-    def __init__(self, key: Text, store: BaseRegisterStore):
+    def __init__(self, key: str, store: BaseRegisterStore):
         self.key = key
         self.register = None
         self.store = store
 
     async def __aenter__(self):
         """
         Start the lock and fetch data from the store in order to provide it.
         """
-
         await self.store._start(self.key)
         data = await self.store._get(self.key)
         self.register = Register(data)
 
         logger.debug("Restored register: %s", self.register._data)
         return self.register
 
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         """
         Whatever happened, if there is a replacement we'll store it. And even
         if that fails, the lock is lifted afterwards.
         """
-
         try:
             if self.register.replacement is not None:
                 logger.debug("Saving register: %s", self.register.replacement)
                 await self.store._replace(self.key, self.register.replacement)
         finally:
             await self.store._finish(self.key)
```

### Comparing `bernard-0.6.0/src/bernard/storage/register/redis.py` & `bernard-0.7.0/src/bernard/storage/register/redis.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import asyncio
-from typing import Any, Dict, Text
+from typing import Any, Dict
 
-import ujson
+import orjson
 
 from bernard.conf import settings
 
 from ..redis import BaseRedisStore
 from .base import BaseRegisterStore
 
 
@@ -13,57 +13,54 @@
     """
     Store the register in Redis.
 
     So far it is quite basic, especially regarding the locking mechanism which
     is just the bare minimum. This should seriously be improved in the future.
     """
 
-    def lock_key(self, key: Text) -> Text:
+    def lock_key(self, key: str) -> str:
         """
         Compute the internal lock key for the specified key
         """
-        return "register::lock:{}".format(key)
+        return f"register::lock:{key}"
 
-    def register_key(self, key: Text) -> Text:
+    def register_key(self, key: str) -> str:
         """
         Compute the internal register content key for the specified key
         """
-        return "register::content:{}".format(key)
+        return f"register::content:{key}"
 
-    async def _start(self, key: Text) -> None:
+    async def _start(self, key: str) -> None:
         """
         Start the lock.
 
         Here we use a SETNX-based algorithm. It's quite shitty, change it.
         """
         for _ in range(0, 1000):
             just_set = await self.redis.setnx(self.lock_key(key), "")
 
             if just_set:
                 break
 
             await asyncio.sleep(settings.REDIS_POLL_INTERVAL)
 
-    async def _finish(self, key: Text) -> None:
+    async def _finish(self, key: str) -> None:
         """
         Remove the lock.
         """
-
         await self.redis.delete(self.lock_key(key))
 
-    async def _get(self, key: Text) -> Dict[Text, Any]:
+    async def _get(self, key: str) -> Dict[str, Any]:
         """
         Get the value for the key. It is automatically deserialized from JSON
         and returns an empty dictionary by default.
         """
-
         try:
-            return ujson.loads(await self.redis.get(self.register_key(key)))
+            return orjson.loads(await self.redis.get(self.register_key(key)))
         except (ValueError, TypeError):
             return {}
 
-    async def _replace(self, key: Text, data: Dict[Text, Any]) -> None:
+    async def _replace(self, key: str, data: Dict[str, Any]) -> None:
         """
         Replace the register with a new value.
         """
-
-        await self.redis.set(self.register_key(key), ujson.dumps(data))
+        await self.redis.set(self.register_key(key), orjson.dumps(data))
```

### Comparing `bernard-0.6.0/src/bernard/trigram.py` & `bernard-0.7.0/src/bernard/trigram.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """
 Trigram computation utils. Although the algorithm are pretty different, the
 code here is inspired from PostgreSQL's pg_trgm module and should give similar
 or identical results.
 """
+
 import re
 from collections import deque
-from typing import Iterable, List, Optional, Text, Tuple, TypeVar, Union
+from typing import Iterable, List, Optional, Tuple, TypeVar, Union
 
 from unidecode import unidecode
 
 RE_WHITESPACES = re.compile(r'[\W.,;?!\'"«»\-_\s]+')
 
 T = TypeVar("T")
 
 
-def normalize(string: Text) -> Text:
+def normalize(string: str) -> str:
     """
     Normalizes a string to encompass various things humans tend to get wrong:
 
     - Put everything lowercase
     - Drop accents
     - Transform all whitespaces sequences into a single space
     - Remove spaces before and after punctuation
     """
-
     string = string.lower()
     string = unidecode(string)
     string = RE_WHITESPACES.sub(" ", string).strip()
 
     return string
 
 
-def make_words(string: Text) -> List[Text]:
+def make_words(string: str) -> List[str]:
     return string.split(" ")
 
 
 def make_trigrams(
     i: Iterable[T],
 ) -> Iterable[Tuple[Optional[T], Optional[T], Optional[T]]]:
     """
@@ -47,36 +47,36 @@
     q = deque([None, None, None])
 
     def nxt():
         q.append(x)
         q.popleft()
         return tuple(c if c is not None else " " for c in q)
 
-    for x in i:
+    for x in i:  # noqa: B007
         yield nxt()
 
     if q[-1] is not None:
         x = None
         yield nxt()
 
 
-class Trigram(object):
+class Trigram:
     """
     This represents a "compiled" trigram object. It is able to compute its
     similarity with other trigram objects.
     """
 
     def __init__(self, string):
         self._string = string
         self._norm = normalize(string)
         self._words = make_words(self._norm)
-        self._trigrams = set(t for w in self._words for t in make_trigrams(w))
+        self._trigrams = {t for w in self._words for t in make_trigrams(w)}
 
     def __repr__(self):
-        return f"Trigram({repr(self._norm)})"
+        return f"Trigram({self._norm!r})"
 
     def similarity(self, other: "Trigram") -> float:
         """
         Compute the similarity with the provided other trigram.
         """
         if not len(self._trigrams) or not len(other._trigrams):
             return 0
@@ -90,28 +90,27 @@
     def __mod__(self, other: "Trigram") -> float:
         """
         Shortcut notation using modulo symbol.
         """
         return self.similarity(other)
 
 
-class Matcher(object):
+class Matcher:
     """
     Allows to match several trigrams at once. This is useful to detect intents.
     """
 
     def __init__(self, trigrams: List[Union[Trigram, Tuple[Trigram, ...]]]):
         self.trigrams = [(t,) if isinstance(t, Trigram) else t for t in trigrams]
 
     def _match(self, local: Tuple[Trigram, ...], other: Trigram) -> float:
         """
         Match a trigram with another one. If the negative matching wins,
         returns an inverted matching.
         """
-
         pos = local[0] % other
         neg = max((x % other for x in local[1:]), default=0)
 
         if neg > pos:
             return 0.0
 
         return pos
@@ -128,25 +127,24 @@
         """
         return self.similarity(other)
 
 
 L = TypeVar("L")
 
 
-class LabelMatcher(object):
+class LabelMatcher:
     """
     Allows to match trigrams and associate an arbitrary label to them. When
     matching, the label will be returned along with the score.
     """
 
     def __init__(self, trigrams: List[Tuple[Trigram, L]]):
         self.trigrams = trigrams
 
     def similarity(self, other: Trigram) -> Tuple[float, L]:
         """
         Returns the best matching score and the associated label.
         """
-
         return max(
-            ((t % other, l) for t, l in self.trigrams),
+            ((t % other, label) for t, label in self.trigrams),
             key=lambda x: x[0],
         )
```

### Comparing `bernard-0.6.0/src/bernard/utils.py` & `bernard-0.7.0/src/bernard/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,43 @@
-import asyncio
 import importlib
 import re
 from asyncio import iscoroutine
 from itertools import chain
 from typing import (
     Any,
     Coroutine,
     Dict,
     Iterator,
     List,
     Mapping,
     Sequence,
-    Text,
-    Tuple,
     Type,
     Union,
 )
 from urllib.parse import parse_qsl, urlencode, urlparse, urlunparse
 
 
-def import_class(name: Text) -> Type:
+def import_class(name: str) -> Type:
     """
     Import a class based on its full name.
 
     :param name: name of the class
     """
-
     parts = name.split(".")
     module_name = parts[:-1]
     class_name = parts[-1]
     module_ = importlib.import_module(".".join(module_name))
     return getattr(module_, class_name)
 
 
-def run(task: Coroutine) -> Any:
-    """
-    Run a task in the default asyncio look.
-
-    :param task: Task to run
-    """
-
-    return asyncio.get_event_loop().run_until_complete(task)
-
-
 async def run_or_return(task: Union[Coroutine, Any]):
     """
     If the specified task is a coroutine then await it, otherwise return
     directly.
     """
-
     if iscoroutine(task):
         return await task
     else:
         return task
 
 
 class RoList(Sequence):
@@ -81,82 +66,74 @@
 
 
 class RoDict(Mapping):
     """
     Wrapper around a dict to make it read-only.
     """
 
-    def __init__(self, data: Dict[Text, Any], forgive_type=False):
+    def __init__(self, data: Dict[str, Any], forgive_type=False):
         self._data = data
         self._forgive_type = forgive_type
 
-    def __getitem__(self, key: Text) -> Any:
+    def __getitem__(self, key: str) -> Any:
         """
         Gets the item from data while making it read-only first
         """
-
         return make_ro(self._data[key], self._forgive_type)
 
     def __len__(self) -> int:
         """
         Proxy to data's length
         """
-
         return len(self._data)
 
     def __iter__(self) -> Iterator[Any]:
         """
         Proxy to data's iterator
         """
-
         return iter(self._data)
 
 
 # noinspection PyTypeChecker
 def make_ro(obj: Any, forgive_type=False):
     """
     Make a json-serializable type recursively read-only
 
     :param obj: Any json-serializable type
     :param forgive_type: If you can forgive a type to be unknown (instead of
                          raising an exception)
     """
-
     if isinstance(obj, (str, bytes, int, float, bool, RoDict, RoList)) or obj is None:
         return obj
     elif isinstance(obj, Mapping):
         return RoDict(obj, forgive_type)
     elif isinstance(obj, Sequence):
         return RoList(obj, forgive_type)
     elif forgive_type:
         return obj
     else:
-        raise ValueError(
-            'Trying to make read-only an object of type "{}"'.format(
-                obj.__class__.__name__
-            )
-        )
+        msg = f'Trying to make read-only an object of type "{obj.__class__.__name__}"'
+        raise ValueError(msg)
 
 
 def make_rw(obj: Any):
     """
     Copy a RO object into a RW structure made with standard Python classes.
 
     WARNING there is no protection against recursion.
     """
-
     if isinstance(obj, RoDict):
         return {k: make_rw(v) for k, v in obj.items()}
     elif isinstance(obj, RoList):
         return [make_rw(x) for x in obj]
     else:
         return obj
 
 
-class ClassExp(object):
+class ClassExp:
     """
     Perform regular expression matching on list of classes.
     """
 
     RE_SPACES = re.compile(r"\s+")
     RE_PYTHON_VAR = re.compile(r"([A-Za-z_][A-Za-z_0-9]*)")
 
@@ -164,48 +141,44 @@
         self._initial_expression = expression
         self._compiled_expression = self._compile(expression)
 
     def _compile(self, expression):
         """
         Transform a class exp into an actual regex
         """
-
         x = self.RE_PYTHON_VAR.sub("(?:\\1,)", expression)
         x = self.RE_SPACES.sub("", x)
         return re.compile(x)
 
-    def _make_string(self, objects: List[Any]) -> Text:
+    def _make_string(self, objects: List[Any]) -> str:
         """
         Transforms a list of objects into a matchable string
         """
-
         return "".join(x.__class__.__name__ + "," for x in objects)
 
     def match(self, objects: List[Any]) -> bool:
         """
         Return True if the list of objects matches the expression.
         """
-
         s = self._make_string(objects)
         m = self._compiled_expression.match(s)
         return m is not None
 
 
-def patch_qs(url: Text, data: Dict[Text, Text]) -> Text:
+def patch_qs(url: str, data: Dict[str, str]) -> str:
     """
-    Given an URL, change the query string to include the values specified in
+    Given a URL, change the query string to include the values specified in
     the dictionary.
 
     If the keys of the dictionary can be found in the query string of the URL,
     then they will be removed.
 
     It is guaranteed that all other values of the query string will keep their
     order.
     """
-
     qs_id = 4
     p = list(urlparse(url))
     qs = parse_qsl(p[qs_id])  # type: List[Tuple[Text, Text]]
     patched_qs = list(
         chain(
             filter(lambda x: x[0] not in data, qs),
             data.items(),
@@ -225,27 +198,21 @@
 
 def dict_is_subset(subset: Any, full_set: Any) -> bool:
     """
     Checks that all keys present in `subset` are present and have the same
     value in `full_set`. If a key is in `full_set` but not in `subset` then
     True will be returned anyways.
     """
-
     if not isinstance(subset, full_set.__class__):
         return False
     elif isinstance(subset, dict):
         for k, v in subset.items():
             if k not in full_set or not dict_is_subset(v, full_set[k]):
                 return False
 
         return True
     elif isinstance(subset, list):
-        if len(subset) != len(full_set):
-            return False
-
-        for a, b in zip(subset, full_set):
-            if not dict_is_subset(a, b):
-                return False
-
-        return True
+        return len(subset) == len(full_set) and all(
+            dict_is_subset(a, b) for a, b in zip(subset, full_set)
+        )
     else:
         return subset == full_set
```

### Comparing `bernard-0.6.0/PKG-INFO` & `bernard-0.7.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: bernard
-Version: 0.6.0
+Version: 0.7.0
 Summary: Bot Engine Responding Naturally At Requests Detection
 License: AGPL-3.0-or-later
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
-Requires-Dist: aionotify (>=0.2.0,<0.3.0)
-Requires-Dist: babel (>=2.14.0,<3.0.0)
-Requires-Dist: facepy (>=1.0.12,<2.0.0)
-Requires-Dist: google-api-python-client (>=2.119.0,<3.0.0)
-Requires-Dist: httpx (>=0.27.0,<0.28.0)
-Requires-Dist: oauth2client (>=4.1.3,<5.0.0)
-Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: pytz (>=2022.6,<2023.0)
-Requires-Dist: redis (>=5.0.1,<6.0.0)
-Requires-Dist: sentry-sdk (>=1.40.6,<2.0.0)
-Requires-Dist: ujson (>=5.9.0,<6.0.0)
-Requires-Dist: unidecode (>=1.3.8,<2.0.0)
-Requires-Dist: uvloop (>=0.19.0,<0.20.0)
+Requires-Dist: aiohttp (>=3.0,<4.0)
+Requires-Dist: babel (>=2.0,<3.0)
+Requires-Dist: facepy (>=1.0,<2.0)
+Requires-Dist: google-api-python-client
+Requires-Dist: google-auth (>=2.0,<3.0)
+Requires-Dist: google-auth-oauthlib (>=1.0,<2.0)
+Requires-Dist: httpx
+Requires-Dist: keyring
+Requires-Dist: orjson (>=3.0,<4.0)
+Requires-Dist: pyjwt (>=2.0,<3.0)
+Requires-Dist: python-dateutil (>=2.0,<3.0)
+Requires-Dist: pytz
+Requires-Dist: redis (>=4.2.0rc1)
+Requires-Dist: rich
+Requires-Dist: sentry-sdk
+Requires-Dist: unidecode (>=1.0,<2.0)
+Requires-Dist: watchdog
 Description-Content-Type: text/markdown
 
 BERNARD
 =======
 
 [![Build Status](https://travis-ci.org/BernardFW/bernard.svg?branch=develop)](https://travis-ci.org/BernardFW/bernard)
```

