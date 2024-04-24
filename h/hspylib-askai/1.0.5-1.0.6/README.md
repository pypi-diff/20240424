# Comparing `tmp/hspylib-askai-1.0.5.tar.gz` & `tmp/hspylib_askai-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hspylib-askai-1.0.5.tar", last modified: Thu Apr 11 00:23:25 2024, max compression
+gzip compressed data, was "hspylib_askai-1.0.6.tar", last modified: Wed Apr 24 04:27:39 2024, max compression
```

## Comparing `hspylib-askai-1.0.5.tar` & `hspylib_askai-1.0.6.tar`

### file list

```diff
@@ -1,80 +1,82 @@
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.749843 hspylib-askai-1.0.5/
--rw-r--r--   0 hjunior    (501) staff       (20)       49 2024-02-15 22:15:40.000000 hspylib-askai-1.0.5/MANIFEST.in
--rw-r--r--   0 hjunior    (501) staff       (20)     7970 2024-04-11 00:23:25.747825 hspylib-askai-1.0.5/PKG-INFO
--rw-r--r--   0 hjunior    (501) staff       (20)     5933 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/README.md
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.648781 hspylib-askai-1.0.5/askai/
--rw-r--r--   0 hjunior    (501) staff       (20)        6 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/.version
--rw-r--r--   0 hjunior    (501) staff       (20)      800 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/__classpath__.py
--rw-r--r--   0 hjunior    (501) staff       (20)      180 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/__init__.py
--rwxr-xr-x   0 hjunior    (501) staff       (20)     4838 2024-04-09 23:04:09.000000 hspylib-askai-1.0.5/askai/__main__.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.660801 hspylib-askai-1.0.5/askai/core/
--rw-r--r--   0 hjunior    (501) staff       (20)      318 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)    10474 2024-04-10 23:50:17.000000 hspylib-askai-1.0.5/askai/core/askai.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2787 2024-04-08 23:25:38.000000 hspylib-askai-1.0.5/askai/core/askai_configs.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1996 2024-04-04 15:23:06.000000 hspylib-askai-1.0.5/askai/core/askai_events.py
--rw-r--r--   0 hjunior    (501) staff       (20)     5057 2024-04-09 18:31:51.000000 hspylib-askai-1.0.5/askai/core/askai_messages.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1757 2024-04-10 00:17:24.000000 hspylib-askai-1.0.5/askai/core/askai_prompt.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.669932 hspylib-askai-1.0.5/askai/core/component/
--rw-r--r--   0 hjunior    (501) staff       (20)      272 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/component/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3617 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/component/audio_player.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3788 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/component/cache_service.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3001 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/component/geo_location.py
--rw-r--r--   0 hjunior    (501) staff       (20)     6231 2024-04-08 16:43:58.000000 hspylib-askai-1.0.5/askai/core/component/internet_service.py
--rw-r--r--   0 hjunior    (501) staff       (20)     7876 2024-04-10 22:09:33.000000 hspylib-askai-1.0.5/askai/core/component/recorder.py
--rw-r--r--   0 hjunior    (501) staff       (20)     5736 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/component/summarizer.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.673660 hspylib-askai-1.0.5/askai/core/engine/
--rw-r--r--   0 hjunior    (501) staff       (20)      200 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/engine/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2441 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/engine/ai_engine.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1613 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/engine/engine_factory.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.682593 hspylib-askai-1.0.5/askai/core/engine/openai/
--rw-r--r--   0 hjunior    (501) staff       (20)      237 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/engine/openai/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2316 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/engine/openai/openai_configs.py
--rw-r--r--   0 hjunior    (501) staff       (20)     5755 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/engine/openai/openai_engine.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2553 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/engine/openai/openai_model.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2413 2024-04-09 18:52:10.000000 hspylib-askai-1.0.5/askai/core/engine/openai/temperature.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.687202 hspylib-askai-1.0.5/askai/core/features/
--rw-r--r--   0 hjunior    (501) staff       (20)      191 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/features/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     6854 2024-04-09 19:09:30.000000 hspylib-askai-1.0.5/askai/core/features/actions.py
--rw-r--r--   0 hjunior    (501) staff       (20)     5214 2024-04-09 19:26:07.000000 hspylib-askai-1.0.5/askai/core/features/router.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.698101 hspylib-askai-1.0.5/askai/core/features/tools/
--rw-r--r--   0 hjunior    (501) staff       (20)      240 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/features/tools/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2209 2024-04-09 15:46:53.000000 hspylib-askai-1.0.5/askai/core/features/tools/analysis.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2198 2024-04-09 00:47:29.000000 hspylib-askai-1.0.5/askai/core/features/tools/browser.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2076 2024-04-09 23:15:03.000000 hspylib-askai-1.0.5/askai/core/features/tools/general.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2024 2024-04-08 16:43:58.000000 hspylib-askai-1.0.5/askai/core/features/tools/summarization.py
--rw-r--r--   0 hjunior    (501) staff       (20)     4169 2024-04-09 19:37:59.000000 hspylib-askai-1.0.5/askai/core/features/tools/terminal.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.712287 hspylib-askai-1.0.5/askai/core/model/
--rw-r--r--   0 hjunior    (501) staff       (20)      308 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/model/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)      669 2024-03-03 22:13:26.000000 hspylib-askai-1.0.5/askai/core/model/ai_model.py
--rw-r--r--   0 hjunior    (501) staff       (20)      648 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/model/ai_reply.py
--rw-r--r--   0 hjunior    (501) staff       (20)     4173 2024-04-09 00:40:44.000000 hspylib-askai-1.0.5/askai/core/model/chat_context.py
--rw-r--r--   0 hjunior    (501) staff       (20)      479 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/model/query_type.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1020 2024-04-08 16:43:58.000000 hspylib-askai-1.0.5/askai/core/model/rag_response.py
--rw-r--r--   0 hjunior    (501) staff       (20)      854 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/core/model/search_result.py
--rw-r--r--   0 hjunior    (501) staff       (20)      740 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/model/summary_result.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1383 2024-03-25 16:24:17.000000 hspylib-askai-1.0.5/askai/core/model/terminal_command.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.723591 hspylib-askai-1.0.5/askai/core/support/
--rw-r--r--   0 hjunior    (501) staff       (20)      292 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/core/support/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1755 2024-03-25 16:24:18.000000 hspylib-askai-1.0.5/askai/core/support/langchain_support.py
--rw-r--r--   0 hjunior    (501) staff       (20)     4407 2024-03-25 16:24:18.000000 hspylib-askai-1.0.5/askai/core/support/object_mapper.py
--rw-r--r--   0 hjunior    (501) staff       (20)     4943 2024-04-10 15:24:30.000000 hspylib-askai-1.0.5/askai/core/support/presets.py
--rw-r--r--   0 hjunior    (501) staff       (20)     1679 2024-03-25 16:24:18.000000 hspylib-askai-1.0.5/askai/core/support/settings.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3423 2024-04-10 23:54:31.000000 hspylib-askai-1.0.5/askai/core/support/shared_instances.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2992 2024-04-09 15:57:17.000000 hspylib-askai-1.0.5/askai/core/support/text_formatter.py
--rw-r--r--   0 hjunior    (501) staff       (20)     7453 2024-04-09 18:08:30.000000 hspylib-askai-1.0.5/askai/core/support/utilities.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.728358 hspylib-askai-1.0.5/askai/exception/
--rw-r--r--   0 hjunior    (501) staff       (20)      161 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/exception/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     2159 2024-04-05 23:07:33.000000 hspylib-askai-1.0.5/askai/exception/exceptions.py
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.735265 hspylib-askai-1.0.5/askai/language/
--rw-r--r--   0 hjunior    (501) staff       (20)      183 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/askai/language/__init__.py
--rw-r--r--   0 hjunior    (501) staff       (20)     3338 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/language/argos_translator.py
--rw-r--r--   0 hjunior    (501) staff       (20)     8910 2024-04-01 15:07:56.000000 hspylib-askai-1.0.5/askai/language/language.py
--rw-r--r--   0 hjunior    (501) staff       (20)      240 2024-03-03 22:13:26.000000 hspylib-askai-1.0.5/askai/welcome.txt
-drwxr-xr-x   0 hjunior    (501) staff       (20)        0 2024-04-11 00:23:25.745001 hspylib-askai-1.0.5/hspylib_askai.egg-info/
--rw-r--r--   0 hjunior    (501) staff       (20)     7970 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/PKG-INFO
--rw-r--r--   0 hjunior    (501) staff       (20)     2051 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/SOURCES.txt
--rw-r--r--   0 hjunior    (501) staff       (20)        1 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/dependency_links.txt
--rw-r--r--   0 hjunior    (501) staff       (20)      631 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/requires.txt
--rw-r--r--   0 hjunior    (501) staff       (20)       11 2024-04-11 00:23:25.000000 hspylib-askai-1.0.5/hspylib_askai.egg-info/top_level.txt
--rw-r--r--   0 hjunior    (501) staff       (20)       38 2024-04-11 00:23:25.750298 hspylib-askai-1.0.5/setup.cfg
--rw-r--r--   0 hjunior    (501) staff       (20)     1991 2024-04-11 00:23:18.000000 hspylib-askai-1.0.5/setup.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.485142 hspylib_askai-1.0.6/
+-rw-r--r--   0 hugo       (503) staff       (20)       49 2024-04-20 00:03:24.000000 hspylib_askai-1.0.6/MANIFEST.in
+-rw-r--r--   0 hugo       (503) staff       (20)     8142 2024-04-24 04:27:39.484640 hspylib_askai-1.0.6/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)     6006 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/README.md
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.462339 hspylib_askai-1.0.6/askai/
+-rw-r--r--   0 hugo       (503) staff       (20)        6 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/.version
+-rw-r--r--   0 hugo       (503) staff       (20)      799 2024-04-24 00:20:20.000000 hspylib_askai-1.0.6/askai/__classpath__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      180 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/__init__.py
+-rwxr-xr-x   0 hugo       (503) staff       (20)     4942 2024-04-24 01:19:17.000000 hspylib_askai-1.0.6/askai/__main__.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.465034 hspylib_askai-1.0.6/askai/core/
+-rw-r--r--   0 hugo       (503) staff       (20)      341 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)    10896 2024-04-24 03:08:59.000000 hspylib_askai-1.0.6/askai/core/askai.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3599 2024-04-24 04:21:42.000000 hspylib_askai-1.0.6/askai/core/askai_configs.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2384 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/askai_events.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5820 2024-04-24 00:40:38.000000 hspylib_askai-1.0.6/askai/core/askai_messages.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1989 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/askai_prompt.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4280 2024-04-24 04:25:13.000000 hspylib_askai-1.0.6/askai/core/askai_settings.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.467781 hspylib_askai-1.0.6/askai/core/component/
+-rw-r--r--   0 hugo       (503) staff       (20)      272 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/component/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3606 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/component/audio_player.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3778 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/component/cache_service.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3380 2024-04-24 00:42:59.000000 hspylib_askai-1.0.6/askai/core/component/geo_location.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7132 2024-04-24 00:42:59.000000 hspylib_askai-1.0.6/askai/core/component/internet_service.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7125 2024-04-24 03:14:31.000000 hspylib_askai-1.0.6/askai/core/component/recorder.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5727 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/component/summarizer.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.468894 hspylib_askai-1.0.6/askai/core/engine/
+-rw-r--r--   0 hugo       (503) staff       (20)      200 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/engine/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2438 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/engine/ai_engine.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1992 2024-04-24 00:45:20.000000 hspylib_askai-1.0.6/askai/core/engine/engine_factory.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.470636 hspylib_askai-1.0.6/askai/core/engine/openai/
+-rw-r--r--   0 hugo       (503) staff       (20)      237 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/engine/openai/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2304 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/engine/openai/openai_configs.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5752 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/engine/openai/openai_engine.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2550 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/engine/openai/openai_model.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2800 2024-04-24 00:46:00.000000 hspylib_askai-1.0.6/askai/core/engine/openai/temperature.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.471711 hspylib_askai-1.0.6/askai/core/features/
+-rw-r--r--   0 hugo       (503) staff       (20)      191 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/features/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7696 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/actions.py
+-rw-r--r--   0 hugo       (503) staff       (20)     6261 2024-04-24 04:21:02.000000 hspylib_askai-1.0.6/askai/core/features/router.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.474241 hspylib_askai-1.0.6/askai/core/features/tools/
+-rw-r--r--   0 hugo       (503) staff       (20)      259 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/features/tools/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4584 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/analysis.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2347 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/browser.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2535 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/general.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2584 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/generation.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2564 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/summarization.py
+-rw-r--r--   0 hugo       (503) staff       (20)     5140 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/features/tools/terminal.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.477377 hspylib_askai-1.0.6/askai/core/model/
+-rw-r--r--   0 hugo       (503) staff       (20)      307 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/model/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)      774 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/action_plan.py
+-rw-r--r--   0 hugo       (503) staff       (20)      666 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/ai_model.py
+-rw-r--r--   0 hugo       (503) staff       (20)      646 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/ai_reply.py
+-rw-r--r--   0 hugo       (503) staff       (20)      866 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/query_type.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1544 2024-04-24 00:46:35.000000 hspylib_askai-1.0.6/askai/core/model/rag_response.py
+-rw-r--r--   0 hugo       (503) staff       (20)      851 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/search_result.py
+-rw-r--r--   0 hugo       (503) staff       (20)      737 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/summary_result.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1445 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/model/terminal_command.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.480162 hspylib_askai-1.0.6/askai/core/support/
+-rw-r--r--   0 hugo       (503) staff       (20)      296 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/core/support/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4891 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/chat_context.py
+-rw-r--r--   0 hugo       (503) staff       (20)     1612 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/langchain_support.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4397 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/object_mapper.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4940 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/presets.py
+-rw-r--r--   0 hugo       (503) staff       (20)     4802 2024-04-24 00:50:03.000000 hspylib_askai-1.0.6/askai/core/support/shared_instances.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3338 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/text_formatter.py
+-rw-r--r--   0 hugo       (503) staff       (20)     7396 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/core/support/utilities.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.480859 hspylib_askai-1.0.6/askai/exception/
+-rw-r--r--   0 hugo       (503) staff       (20)      161 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/exception/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     2177 2024-04-24 00:40:30.000000 hspylib_askai-1.0.6/askai/exception/exceptions.py
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.481813 hspylib_askai-1.0.6/askai/language/
+-rw-r--r--   0 hugo       (503) staff       (20)      183 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/askai/language/__init__.py
+-rw-r--r--   0 hugo       (503) staff       (20)     3627 2024-04-24 00:40:09.000000 hspylib_askai-1.0.6/askai/language/argos_translator.py
+-rw-r--r--   0 hugo       (503) staff       (20)     9293 2024-04-24 00:40:09.000000 hspylib_askai-1.0.6/askai/language/language.py
+-rw-r--r--   0 hugo       (503) staff       (20)      240 2024-04-20 00:03:24.000000 hspylib_askai-1.0.6/askai/welcome.txt
+drwxr-xr-x   0 hugo       (503) staff       (20)        0 2024-04-24 04:27:39.483935 hspylib_askai-1.0.6/hspylib_askai.egg-info/
+-rw-r--r--   0 hugo       (503) staff       (20)     8142 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/PKG-INFO
+-rw-r--r--   0 hugo       (503) staff       (20)     2123 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/SOURCES.txt
+-rw-r--r--   0 hugo       (503) staff       (20)        1 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/dependency_links.txt
+-rw-r--r--   0 hugo       (503) staff       (20)      685 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/requires.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       11 2024-04-24 04:27:39.000000 hspylib_askai-1.0.6/hspylib_askai.egg-info/top_level.txt
+-rw-r--r--   0 hugo       (503) staff       (20)       38 2024-04-24 04:27:39.485239 hspylib_askai-1.0.6/setup.cfg
+-rw-r--r--   0 hugo       (503) staff       (20)     1988 2024-04-24 04:27:36.000000 hspylib_askai-1.0.6/setup.py
```

### Comparing `hspylib-askai-1.0.5/PKG-INFO` & `hspylib_askai-1.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-askai
-Version: 1.0.5
+Version: 1.0.6
 Summary: HomeSetup - AskAI
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-askai/
@@ -19,28 +19,30 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Terminals
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: hspylib>=1.12.35
-Requires-Dist: hspylib-clitt>=0.9.119
+Requires-Dist: hspylib>=1.12.36
+Requires-Dist: hspylib-clitt>=0.9.122
+Requires-Dist: hspylib-setman>=0.10.34
 Requires-Dist: retry2==0.9.5
 Requires-Dist: pause==0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: argostranslate==1.9.1
 Requires-Dist: protobuf==4.22.1
 Requires-Dist: torch==2.2.0
 Requires-Dist: stanza==1.1.1
 Requires-Dist: soundfile==0.12.1
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: langchain>=0.1.12
 Requires-Dist: langchain-openai==0.0.8
 Requires-Dist: langchain-community==0.0.28
+Requires-Dist: langchainhub
 Requires-Dist: unstructured==0.12.4
 Requires-Dist: unstructured[md]==0.12.4
 Requires-Dist: python-magic-bin==0.4.14
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: html2text==2024.2.26
 Requires-Dist: PyAudio==0.2.14
@@ -50,35 +52,40 @@
 Requires-Dist: openai==1.14.1
 Requires-Dist: chromadb==0.4.24
 Requires-Dist: opentelemetry-api==1.22.0
 Requires-Dist: opentelemetry-sdk==1.22.0
 Requires-Dist: opentelemetry-proto==1.22.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: pytz==2024.1
-Requires-Dist: schedule==1.2.1
+Requires-Dist: bs4==0.0.2
+Requires-Dist: fake_useragent==1.5.1
 
-<img src="https://iili.io/JEatihb.png" width="64" height="64" align="right" />
+<img src="https://iili.io/J8wvc1n.png" width="64" height="64" align="right" />
 
 # AskAI
 >
 > Unleash the Power of AI in Your Terminal
 
 [![Terminal](https://badgen.net/badge/icon/terminal?icon=terminal&label)](https://github.com/yorevs/homesetup)
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v1.0.5/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v1.0.6/gray)](docs/CHANGELOG.md#unreleased)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 [![build-and-test](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml)
 
-<img src="https://iili.io/JGv7BTP.png)" width="360" height="360" align="right" />
+<img src="https://iili.io/J8vkAYX.png" width="100%" height="100%" />
+
+---
+
+<img src="https://iili.io/J8wrBSe.png" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
 
 At the heart of AskAI lies its innovative integration of Speech-to-Text and Text-to-Speech technologies, offering a seamless experience for both visually and hearing impaired users. Through these cutting-edge features, individuals can interact with their computers using their natural voice, transcending the barriers imposed by traditional input methods. Moreover, AskAI introduces a unique push-to-talk input mechanism, enabling users to issue commands effortlessly, enhancing the fluidity and ease of interaction.
 
-<img src="https://iili.io/JMWbjf4.jpg)" style="padding-right: 10px" width="258" height="170" align="left" />
+<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="238" height="170" align="left" />
 
 Furthermore, AskAI embraces diversity by breaking language barriers, ensuring that no matter the tongue spoken, users can communicate effectively with their systems. Its adaptive language capabilities ensure that commands are understood and executed accurately, regardless of linguistic nuances. By championing inclusivity on all fronts, AskAI redefines the landscape of computing accessibility, empowering individuals with disabilities to navigate the digital realm with confidence and autonomy.
 
 
 > The world speaks many languages. AskAI understands them all.
 
 The see a brief demo about AskAI feature check our asciinema video.
```

### Comparing `hspylib-askai-1.0.5/README.md` & `hspylib_askai-1.0.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-<img src="https://iili.io/JEatihb.png" width="64" height="64" align="right" />
+<img src="https://iili.io/J8wvc1n.png" width="64" height="64" align="right" />
 
 # AskAI
 >
 > Unleash the Power of AI in Your Terminal
 
 [![Terminal](https://badgen.net/badge/icon/terminal?icon=terminal&label)](https://github.com/yorevs/homesetup)
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v1.0.5/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v1.0.6/gray)](docs/CHANGELOG.md#unreleased)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 [![build-and-test](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml)
 
-<img src="https://iili.io/JGv7BTP.png)" width="360" height="360" align="right" />
+<img src="https://iili.io/J8vkAYX.png" width="100%" height="100%" />
+
+---
+
+<img src="https://iili.io/J8wrBSe.png" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
 
 At the heart of AskAI lies its innovative integration of Speech-to-Text and Text-to-Speech technologies, offering a seamless experience for both visually and hearing impaired users. Through these cutting-edge features, individuals can interact with their computers using their natural voice, transcending the barriers imposed by traditional input methods. Moreover, AskAI introduces a unique push-to-talk input mechanism, enabling users to issue commands effortlessly, enhancing the fluidity and ease of interaction.
 
-<img src="https://iili.io/JMWbjf4.jpg)" style="padding-right: 10px" width="258" height="170" align="left" />
+<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="238" height="170" align="left" />
 
 Furthermore, AskAI embraces diversity by breaking language barriers, ensuring that no matter the tongue spoken, users can communicate effectively with their systems. Its adaptive language capabilities ensure that commands are understood and executed accurately, regardless of linguistic nuances. By championing inclusivity on all fronts, AskAI redefines the landscape of computing accessibility, empowering individuals with disabilities to navigate the digital realm with confidence and autonomy.
 
 
 > The world speaks many languages. AskAI understands them all.
 
 The see a brief demo about AskAI feature check our asciinema video.
```

### Comparing `hspylib-askai-1.0.5/askai/__classpath__.py` & `hspylib_askai-1.0.6/askai/__classpath__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,15 +6,15 @@
    @package: askai
       @file: __classpath__.py
    @created: Fri, 5 Jan 2024
     @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
       @site: "https://github.com/yorevs/hspylib")
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 
 from hspylib.core.metaclass.classpath import Classpath
 from hspylib.core.tools.commons import get_path, run_dir
 
 
 class _Classpath(Classpath):
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/__main__.py` & `hspylib_askai-1.0.6/askai/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,61 +3,62 @@
 
 """
    @project: hspylib
    @package: hspylib
       @file: __main__.py
    @created: Fri, 5 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 
 import logging as log
 import sys
+from textwrap import dedent
 from typing import Any, Optional
 
+from askai.__classpath__ import classpath
+from askai.core.askai import AskAi
 from clitt.core.term.commons import is_a_tty
-
-if not is_a_tty():
-    log.getLogger().setLevel(log.ERROR)
-
-from textwrap import dedent
-
 from clitt.core.tui.tui_application import TUIApplication
 from hspylib.core.enums.charset import Charset
+from hspylib.core.tools.commons import to_bool
 from hspylib.core.tools.dict_tools import get_or_default
 from hspylib.core.zoned_datetime import now
 from hspylib.modules.application.argparse.parser_action import ParserAction
 from hspylib.modules.application.exit_status import ExitStatus
 from hspylib.modules.application.version import Version
 
-from askai.__classpath__ import classpath
-from askai.core.askai import AskAi
+if not is_a_tty():
+    log.getLogger().setLevel(log.ERROR)
 
 
 class Main(TUIApplication):
     """HomeSetup Ask-AI - Unleash the Power of AI in Your Terminal."""
 
     # The welcome message
     DESCRIPTION = classpath.get_source("welcome.txt").read_text(encoding=Charset.UTF_8.val)
 
     # Location of the .version file
     VERSION = Version.load(load_dir=classpath.source_path())
 
     # The resources folder
     RESOURCE_DIR = str(classpath.resource_path())
 
+    INSTANCE: "Main"
+
     def __init__(self, app_name: str):
         super().__init__(app_name, self.VERSION, self.DESCRIPTION.format(self.VERSION), resource_dir=self.RESOURCE_DIR)
-        self._askai = None
+        self._askai: AskAi
 
     def _setup_arguments(self) -> None:
         """Initialize application parameters and options."""
+
         # fmt: off
         self._with_options() \
             .option(
                 "interactive", "i", "interactive",
                 "whether you would like to run the program in an interactive mode.",
                 nargs="?", action=ParserAction.STORE_TRUE, default=False)\
             .option(
@@ -72,15 +73,15 @@
                 "tempo", "t", "tempo",
                 "specifies the playback and streaming speed.",
                 choices=['1', '2', '3'],
                 nargs=1, default='1')\
             .option(
                 "prompt", "p", "prompt",
                 "specifies the query prompt file (not useful with interactive mode).",
-                nargs=1, default='qstring-prompt')\
+                nargs=1, default='qstring')\
             .option(
                 "engine", "e", "engine",
                 "specifies which AI engine to use. If not provided, the default engine wil be used.",
                 choices=['openai', 'palm'],
                 nargs=1, default='openai')\
             .option(
                 "model", "m", "model",
@@ -89,22 +90,22 @@
         self._with_arguments() \
             .argument("query_string", "what to ask to the AI engine", nargs="*")
         # fmt: on
 
     def _main(self, *params, **kwargs) -> ExitStatus:
         """Run the application with the command line arguments."""
         self._askai = AskAi(
-            self.get_arg("interactive"),
-            self.get_arg("quiet"),
-            self.get_arg("debug"),
-            int(self._get_argument("tempo")),
+            to_bool(self.get_arg("interactive")),
+            to_bool(self.get_arg("quiet")),
+            to_bool(self.get_arg("debug")),
+            int(self._get_argument("tempo") or 1),
             str(self._get_argument("prompt")),
-            self.get_arg("engine"),
-            self.get_arg("model"),
-            self.get_arg("query_string"),
+            str(self.get_arg("engine")),
+            str(self.get_arg("model")),
+            str(self.get_arg("query_string")),
         )
 
         log.info(
             dedent(
                 f"""
         {self._app_name} v{self._app_version}
 
@@ -124,17 +125,17 @@
 
     def _get_argument(self, arg_name: str) -> Optional[Any]:
         """TODO"""
         if arg := self.get_arg(arg_name):
             if isinstance(arg, str):
                 return arg
             elif isinstance(arg, list):
-                return get_or_default(arg, 0, '')
+                return get_or_default(arg, 0, "")
             else:
                 raise TypeError("Argument '' has an invalid type: ''", arg, type(arg))
         else:
-            return ''
+            return ""
 
 
 # Application entry point
 if __name__ == "__main__":
     Main("AskAI").INSTANCE.run(sys.argv[1:])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/askai.py` & `hspylib_askai-1.0.6/askai/core/askai.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,75 +3,78 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core
       @file: askai.py
    @created: Fri, 5 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 import logging as log
 import os
 import sys
 from functools import partial
+from pathlib import Path
 from threading import Thread
 from typing import List, Optional
 
 import nltk
 import pause
-from clitt.core.term.cursor import cursor
-from clitt.core.term.screen import screen
-from clitt.core.term.terminal import terminal
-from hspylib.core.enums.charset import Charset
-from hspylib.core.tools.commons import sysout, is_debugging
-from hspylib.modules.application.exit_status import ExitStatus
-from hspylib.modules.eventbus.event import Event
-from langchain_core.prompts import PromptTemplate
-
 from askai.__classpath__ import classpath
 from askai.core.askai_configs import configs
 from askai.core.askai_events import ASKAI_BUS_NAME, AskAiEvents, REPLY_ERROR_EVENT, REPLY_EVENT
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
 from askai.core.component.audio_player import player
 from askai.core.component.cache_service import cache, CACHE_DIR
+from askai.core.component.geo_location import geo_location
 from askai.core.component.recorder import recorder
 from askai.core.engine.ai_engine import AIEngine
 from askai.core.engine.openai.temperature import Temperature
 from askai.core.features.router import router
-from askai.core.model.chat_context import ChatContext
+from askai.core.support.chat_context import ChatContext
 from askai.core.support.langchain_support import lc_llm
 from askai.core.support.shared_instances import shared
 from askai.core.support.utilities import display_text, read_stdin
-from askai.exception.exceptions import ImpossibleQuery, UnintelligibleQuery, TerminatingQuery, MaxInteractionsReached, \
-    InaccurateResponse
+from askai.exception.exceptions import ImpossibleQuery, InaccurateResponse, MaxInteractionsReached, TerminatingQuery
+from clitt.core.term.cursor import cursor
+from clitt.core.term.screen import screen
+from clitt.core.term.terminal import terminal
+from hspylib.core.enums.charset import Charset
+from hspylib.core.tools.commons import is_debugging, sysout
+from hspylib.core.tools.text_tools import elide_text
+from hspylib.modules.application.exit_status import ExitStatus
+from hspylib.modules.application.version import Version
+from hspylib.modules.eventbus.event import Event
+from langchain_core.prompts import PromptTemplate
 
 
 class AskAi:
     """Responsible for the OpenAI functionalities."""
 
     SPLASH = classpath.get_resource("splash.txt").read_text(encoding=Charset.UTF_8.val)
 
     @staticmethod
     def _abort():
         """Abort the execution and exit."""
         sys.exit(ExitStatus.FAILED.val)
 
     def __init__(
-        self, interactive: bool,
+        self,
+        interactive: bool,
         quiet: bool,
         debug: bool,
         tempo: int,
         query_prompt: str,
         engine_name: str,
         model_name: str,
-        query: str | List[str]
+        query: str | List[str],
     ):
         self._interactive: bool = interactive
         self._ready: bool = False
         self._processing: Optional[bool] = None
         self._query_string: str | None = None
         self._question: str | None = None
         self._query_prompt: str | None = query_prompt
@@ -82,25 +85,29 @@
         configs.is_speak = not quiet
         configs.is_debug = is_debugging() or debug
         configs.tempo = tempo
         configs.is_interactive = interactive
 
     def __str__(self) -> str:
         device_info = f"{recorder.input_device[1].title()}" if recorder.input_device else ""
+        dtm = f" {geo_location.datetime} "
+        cur_dir = elide_text(str(Path(os.curdir).absolute()), 67, "…")
         return (
             f"%GREEN%"
-            f"{'-=' * 40} %EOL%"
+            f"AskAI v{Version.load(load_dir=classpath.source_path())} %EOL%"
+            f"{dtm.center(80, '=')} %EOL%"
             f"     Engine: {self.engine} %EOL%"
             f"   Language: {configs.language} %EOL%"
-            f"{'-+' * 40} %EOL%"
+            f"    WorkDir: {cur_dir} %EOL%"
+            f"{'-' * 80} %EOL%"
             f" Microphone: {device_info or '%RED%Undetected'} %GREEN%%EOL%"
             f"  Debugging: {'ON' if self.is_debugging else '%RED%OFF'} %GREEN%%EOL%"
             f"   Speaking: {'ON, tempo: ' + str(configs.tempo) if self.is_speak else '%RED%OFF'} %GREEN%%EOL%"
             f"    Caching: {'ON, TTL: ' + configs.ttl if cache.is_cache_enabled() else '%RED%OFF'} %GREEN%%EOL%"
-            f"{'-=' * 40} %EOL%%NC%"
+            f"{'=' * 80}%EOL%%NC%"
         )
 
     @property
     def engine(self) -> AIEngine:
         return self._engine
 
     @property
@@ -181,15 +188,15 @@
         :param ev: The reply event.
         :param error: Whether the event is an error not not.
         """
         if error:
             self.reply_error(ev.args.message)
         else:
             verbose = ev.args.verbosity.lower()
-            if verbose == 'normal' or self.is_debugging:
+            if verbose == "normal" or self.is_debugging:
                 if ev.args.erase_last:
                     cursor.erase_line()
                 self.reply(ev.args.message)
 
     def _splash(self) -> None:
         """Display the AskAI splash screen."""
         splash_interval = 1000
@@ -205,21 +212,21 @@
         """Initialize the application."""
         askai_bus = AskAiEvents.get_bus(ASKAI_BUS_NAME)
         askai_bus.subscribe(REPLY_EVENT, self._cb_reply_event)
         askai_bus.subscribe(REPLY_ERROR_EVENT, partial(self._cb_reply_event, error=True))
         if self.is_interactive:
             splash_thread: Thread = Thread(daemon=True, target=self._splash)
             splash_thread.start()
-            recorder.setup()
             nltk.download("averaged_perceptron_tagger", quiet=True, download_dir=CACHE_DIR)
             cache.set_cache_enable(self.cache_enabled)
             cache.read_query_history()
             player.start_delay()
             self._ready = True
             splash_thread.join()
+            recorder.setup()
             display_text(self, markdown=False)
             self.reply(msg.welcome(os.getenv("USER", "you")))
         else:
             recorder.setup()
             player.start_delay()
         log.info("AskAI is ready to use!")
 
@@ -245,17 +252,17 @@
                 log.debug('Response not found for "%s" in cache. Querying from %s.', question, self.engine.nickname())
                 AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.wait())
                 if output := router.process(question):
                     self.reply(output)
             else:
                 log.debug("Reply found for '%s' in cache.", question)
                 self.reply(reply)
-        except (NotImplementedError, ImpossibleQuery, UnintelligibleQuery) as err:
+        except (NotImplementedError, ImpossibleQuery) as err:
             self.reply_error(str(err))
-        except (MaxInteractionsReached, InaccurateResponse) as err:
+        except (MaxInteractionsReached, InaccurateResponse, ValueError) as err:
             self.reply_error(msg.unprocessable(str(err)))
         except TerminatingQuery:
             status = False
 
         return status
 
     def _get_query_string(self, interactive: bool, query_arg: str | list[str]) -> None:
@@ -265,14 +272,15 @@
         """
         query: str = str(" ".join(query_arg) if isinstance(query_arg, list) else query_arg)
         self._question = query
         dir_name, file_name = os.path.split(self._query_prompt)
         if not interactive:
             stdin_args = read_stdin()
             template = PromptTemplate(
-                input_variables=['context', 'question'],
-                template=prompt.read_prompt(file_name, dir_name.replace('~', os.getenv('HOME'))))
+                input_variables=["context", "question"],
+                template=prompt.read_prompt(file_name, dir_name.replace("~", os.getenv("HOME"))),
+            )
             final_prompt = template.format(context=stdin_args, question=self._question)
             self._query_string = final_prompt if query else stdin_args
             self._question = self._question or self._query_string
         else:
             self._query_string = query
```

### Comparing `hspylib-askai-1.0.5/askai/core/askai_configs.py` & `hspylib_askai-1.0.6/askai/core/askai_configs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,99 +1,120 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HsPyLib-AskAI
-   @package: askai.core
+   @package: askai.core.askai_configs
       @file: askai_configs.py
    @created: Fri, 5 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 import os
 from shutil import which
 
-from hspylib.core.config.app_config import AppConfigs
-from hspylib.core.enums.charset import Charset
-from hspylib.core.metaclass.singleton import Singleton
-
 from askai.__classpath__ import classpath
+from askai.core.askai_settings import settings
 from askai.language.language import Language
+from hspylib.core.enums.charset import Charset
+from hspylib.core.metaclass.singleton import Singleton
 
 
 class AskAiConfigs(metaclass=Singleton):
     """Provides access to AskAI configurations."""
 
-    INSTANCE: "AskAiConfigs" = None
+    INSTANCE: "AskAiConfigs"
 
     # The resources folder
     RESOURCE_DIR = str(classpath.resource_path())
 
     def __init__(self):
-        self._configs = AppConfigs.INSTANCE or AppConfigs(self.RESOURCE_DIR)
-        self._is_interactive = self._configs.get_bool("askai.interactive.enabled")
-        self._is_speak = self._configs.get_bool("askai.speak.enabled")
-        self._is_debug = self._configs.get_bool("askai.debug.enabled")
-        self._is_cache = self._configs.get_bool("askai.cache.enabled")
-        self._ttl = self._configs.get_int("askai.cache.ttl.minutes")
-        self._tempo = self._configs.get_int("askai.speech.tempo")
-        self._language = Language.of_locale(
+        self._language: Language = Language.of_locale(
             os.getenv("LC_ALL", os.getenv("LC_TYPE", os.getenv("LANG", os.getenv("LANGUAGE", "en_US.UTF-8"))))
         )
+        self._recorder_devices: list[str] = settings.get_list("askai.recorder.devices")
 
     @property
-    def is_cache(self) -> bool:
-        return self._is_cache
-
-    @is_cache.setter
-    def is_cache(self, value: bool) -> None:
-        self._is_cache = value
-
-    @property
-    def tempo(self) -> int:
-        return self._tempo
+    def is_interactive(self) -> bool:
+        return settings.get_bool("askai.interactive.enabled")
 
-    @tempo.setter
-    def tempo(self, value: int) -> None:
-        self._tempo = value
+    @is_interactive.setter
+    def is_interactive(self, value: bool) -> None:
+        settings.put("askai.interactive.enabled", value)
 
     @property
     def is_speak(self) -> bool:
-        return which("ffplay") and self._is_speak
+        return which("ffplay") and settings.get_bool("askai.speak.enabled")
 
     @is_speak.setter
     def is_speak(self, value: bool) -> None:
-        self._is_speak = which("ffplay") and value
+        settings.put("askai.speak.enabled", which("ffplay") and value)
 
     @property
     def is_debug(self) -> bool:
-        return self._is_debug
+        return settings.get_bool("askai.debug.enabled")
 
     @is_debug.setter
     def is_debug(self, value: bool) -> None:
-        self._is_debug = value
+        settings.put("askai.debug.enabled", value)
 
     @property
-    def is_interactive(self) -> bool:
-        return self._is_interactive
+    def is_cache(self) -> bool:
+        return settings.get_bool("askai.cache.enabled")
 
-    @is_interactive.setter
-    def is_interactive(self, value: bool) -> None:
-        self._is_interactive = value
+    @is_cache.setter
+    def is_cache(self, value: bool) -> None:
+        settings.put("askai.cache.enabled", value)
+
+    @property
+    def tempo(self) -> int:
+        return settings.get_int("askai.speech.tempo")
+
+    @tempo.setter
+    def tempo(self, value: int) -> None:
+        settings.get_int("askai.speech.tempo", value)
 
     @property
     def language(self) -> Language:
         return self._language
 
     @property
     def encoding(self) -> Charset:
         return self.language.encoding
 
     @property
     def ttl(self) -> int:
-        return self._ttl
+        return settings.get_int("askai.cache.ttl.minutes")
+
+    @property
+    def max_iteractions(self) -> int:
+        return settings.get_int("askai.max.iteractions")
+
+    @property
+    def max_context_size(self) -> int:
+        return settings.get_int("askai.max.context.size")
+
+    @property
+    def max_router_retries(self) -> int:
+        return settings.get_int("askai.max.router.retries")
+
+    @property
+    def max_agent_execution_time_seconds(self) -> int:
+        return settings.get_int("askai.max.agent.execution.time.seconds")
+
+    @property
+    def recorder_devices(self) -> list[str]:
+        return self._recorder_devices
+
+    def add_device(self, device_name: str) -> None:
+        self._recorder_devices.append(device_name)
+        settings.put("askai.recorder.devices", ', '.join(self._recorder_devices))
+
+    def remove_device(self, device_name: str) -> None:
+        self._recorder_devices.remove(device_name)
+        settings.put("askai.recorder.devices", ', '.join(self._recorder_devices))
 
 
 assert (configs := AskAiConfigs().INSTANCE) is not None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/askai_events.py` & `hspylib_askai-1.0.6/askai/core/askai_events.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.core.askai_events
+      @file: askai_events.py
+   @created: Fri, 5 Jan 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
+
 from functools import partial
 from hspylib.core.enums.enumeration import Enumeration
 from hspylib.core.namespace import Namespace
 from hspylib.modules.eventbus.eventbus import emit, EventBus
 from typing import Optional
 
 ASKAI_BUS_NAME: str = "askai-reply-bus"
```

### Comparing `hspylib-askai-1.0.5/askai/core/askai_messages.py` & `hspylib_askai-1.0.6/askai/core/askai_messages.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,43 @@
-from functools import lru_cache
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.core.askai_messages
+      @file: askai_messages.py
+   @created: Fri, 5 Jan 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
+from functools import cached_property, lru_cache
 
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.modules.application.exit_status import ExitStatus
 
 from askai.core.askai_configs import configs
 from askai.language.argos_translator import ArgosTranslator
 from askai.language.language import Language
 
 
 class AskAiMessages(metaclass=Singleton):
     """Provide access to static 'translated' messages."""
 
-    INSTANCE: "AskAiMessages" = None
+    INSTANCE: "AskAiMessages"
 
     def __init__(self):
         self._translator = ArgosTranslator(Language.EN_US, configs.language)
+        self._accurate_responses: list[str] = [self.welcome_back()]
+
+    @cached_property
+    def accurate_responses(self) -> list[str]:
+        return self._accurate_responses
 
     @lru_cache
     def translate(self, text: str) -> str:
         """Translate text using the configured language."""
         return self._translator.translate(text)
 
     # Informational
@@ -45,25 +64,29 @@
 
     @lru_cache
     def goodbye(self) -> str:
         return self.translate("Goodbye, have a nice day !")
 
     @lru_cache
     def executing(self, command_line: str) -> str:
-        return self.translate(f"Executing `{command_line}`…")
+        return self.translate(f"> Executing `{command_line}`…")
 
     @lru_cache
     def cmd_success(self, command_line: str, exit_code: ExitStatus) -> str:
         return self.translate(f"OK, command `{command_line}` executed with {str(exit_code).lower()}")
 
     @lru_cache
     def searching(self) -> str:
         return self.translate(f"Searching on the internet…")
 
     @lru_cache
+    def scrapping(self) -> str:
+        return self.translate(f"Scrapping web site…")
+
+    @lru_cache
     def summarizing(self, path: str) -> str:
         return self.translate(f"Summarizing docs at:'{path}' …")
 
     @lru_cache
     def enter_qna(self) -> str:
         return self.translate("You have entered the Summarization Q & A")
 
@@ -76,34 +99,38 @@
         return self.translate("What specific information are you seeking about the content ?")
 
     @lru_cache
     def press_esc_enter(self) -> str:
         return self.translate("Press [Esc or Enter] to leave")
 
     @lru_cache
-    def analysis(self) -> str:
-        return self.translate(f"Analysing the output…")
+    def analysis(self, result: str) -> str:
+        return self.translate(f"Analysis result: `{result}`")
 
     @lru_cache
-    def assert_acc(self, ai_response: str, result: str) -> str:
-        return self.translate(f"Accuracy check: `{ai_response.strip()}` -> **{result.strip()}**")
+    def assert_acc(self, result: str) -> str:
+        return self.translate(f"! Accuracy check: `{result}`")
 
     @lru_cache
     def action_plan(self, plan_text: str) -> str:
-        return self.translate(f"Action plan: `{plan_text.strip()}`")
+        return self.translate(f"@ Action plan: `{plan_text}`")
+
+    @lru_cache
+    def x_reference(self) -> str:
+        return self.translate(f"> Looking for **X-References**…")
 
     # Warnings and alerts
 
     @lru_cache
     def search_empty(self) -> str:
         return self.translate("The search didn't return an output !")
 
     @lru_cache
     def access_grant(self) -> str:
-        return self.translate("Do you approve executing this command on you terminal (yes/[no])?")
+        return self.translate("Do you approve executing this command on you terminal (**yes/[no]**)?")
 
     # Failures
 
     @lru_cache
     def no_query_string(self) -> str:
         return self.translate("No query string was provided in non-interactive mode !")
```

### Comparing `hspylib-askai-1.0.5/askai/core/askai_prompt.py` & `hspylib_askai-1.0.6/askai/core/askai_prompt.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HsPyLib-AskAI
-   @package: askai.utils
+   @package: askai.core.askai_prompt
       @file: askai_prompt.py
    @created: Mon, 22 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
-from functools import lru_cache
-
-from hspylib.core.metaclass.singleton import Singleton
-
 from askai.__classpath__ import classpath
 from askai.core.askai_configs import configs
 from askai.core.model.terminal_command import get_os, get_shell, get_user, SupportedPlatforms, SupportedShells
 from askai.core.support.utilities import read_resource
+from functools import lru_cache
+from hspylib.core.metaclass.singleton import Singleton
+from langchain import hub
+from langchain_core.prompts import ChatPromptTemplate
 
 
 class AskAiPrompt(metaclass=Singleton):
     """Provide the prompts used by the AskAi."""
 
-    INSTANCE: "AskAiPrompt" = None
+    INSTANCE: "AskAiPrompt"
 
     # AI Prompts directory.
     PROMPT_DIR = str(classpath.resource_path()) + "/assets/prompts"
 
     def __init__(self):
         self._shell: SupportedShells = get_shell()
         self._os_type: SupportedPlatforms = get_os()
@@ -52,9 +52,13 @@
         return f"{configs.language.name} ({configs.language.country})"
 
     @lru_cache
     def read_prompt(self, template_file: str, prompt_dir: str = None) -> str:
         """Read a processor prompt template and set its persona."""
         return read_resource(prompt_dir or self.PROMPT_DIR, template_file)
 
+    def hub(self, owner_repo_commit) -> ChatPromptTemplate:
+        """Read a prompt from LangChain hub."""
+        return hub.pull(owner_repo_commit)
+
 
 assert (prompt := AskAiPrompt().INSTANCE) is not None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/component/audio_player.py` & `hspylib_askai-1.0.6/askai/core/component/audio_player.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,39 +3,38 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.component
       @file: audio_player.py
    @created: Wed, 22 Feb 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
-import logging as log
-import time
-from functools import lru_cache
-from shutil import which
-from typing import Literal
-
+from askai.__classpath__ import classpath
 from clitt.core.term.terminal import Terminal
+from functools import lru_cache
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_argument
 from hspylib.core.tools.commons import file_is_not_empty
 from hspylib.core.tools.text_tools import ensure_endswith
 from hspylib.modules.application.exit_status import ExitStatus
+from shutil import which
+from typing import Literal
 
-from askai.__classpath__ import classpath
+import logging as log
+import time
 
 
 class AudioPlayer(metaclass=Singleton):
     """Provide an interface to play audio using the default speaker device."""
 
-    INSTANCE: "AudioPlayer" = None
+    INSTANCE: "AudioPlayer"
 
     # Sound effects directory.
     SFX_DIR = str(classpath.resource_path()) + "/assets/sound-fx"
 
     @staticmethod
     def play_audio_file(path_to_audio_file: str, tempo: int = 1) -> bool:
         """Play the specified mp3 file using ffplay (ffmpeg) application.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/component/cache_service.py` & `hspylib_askai-1.0.6/askai/core/component/cache_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.component
       @file: cache_service.py
    @created: Tue, 16 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 from askai.core.support.utilities import hash_text
 from clitt.core.tui.line_input.keyboard_input import KeyboardInput
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.commons import file_is_not_empty
 from hspylib.modules.cache.ttl_cache import TTLCache
 from pathlib import Path
@@ -39,15 +39,15 @@
 if not PERSIST_DIR.exists():
     PERSIST_DIR.mkdir(parents=True, exist_ok=True)
 
 
 class CacheService(metaclass=Singleton):
     """Provide a cache service for previously used queries, audio generation, etc..."""
 
-    INSTANCE: "CacheService" = None
+    INSTANCE: "CacheService"
 
     ASKAI_INPUT_CACHE_KEY = "askai-input-history"
 
     DISABLE_CACHE = True
 
     _TTL_CACHE: TTLCache[str] = TTLCache(ttl_minutes=30)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/component/internet_service.py` & `hspylib_askai-1.0.6/askai/core/component/internet_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,79 +2,63 @@
 # -*- coding: utf-8 -*-
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.component
       @file: internet_service.py
    @created: Sun, 10 Mar 2024
-    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 import logging as log
 import re
 from functools import lru_cache
-from typing import List, Optional
+from typing import List
 
+import bs4
 from googleapiclient.errors import HttpError
 from hspylib.core.metaclass.singleton import Singleton
 from langchain.chains.combine_documents import create_stuff_documents_chain
-from langchain.chains.retrieval_qa.base import RetrievalQA
-from langchain_community.document_loaders.async_html import AsyncHtmlLoader
+from langchain_community.document_loaders.web_base import WebBaseLoader
 from langchain_community.utilities import GoogleSearchAPIWrapper
 from langchain_community.vectorstores.chroma import Chroma
 from langchain_core.documents import Document
+from langchain_core.output_parsers import StrOutputParser
 from langchain_core.prompts import ChatPromptTemplate, PromptTemplate
+from langchain_core.runnables import RunnablePassthrough
+from langchain_core.runnables.utils import Output
 from langchain_core.tools import Tool
 from langchain_text_splitters import RecursiveCharacterTextSplitter
 
 from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
-from askai.core.component.cache_service import PERSIST_DIR
 from askai.core.component.geo_location import geo_location
 from askai.core.component.summarizer import summarizer
 from askai.core.engine.openai.temperature import Temperature
 from askai.core.model.search_result import SearchResult
-from askai.core.support.langchain_support import lc_llm, load_document
+from askai.core.support.langchain_support import lc_llm
 from askai.core.support.shared_instances import shared
 
 
 class InternetService(metaclass=Singleton):
     """Provide a internet search service to complete queries that require realtime data."""
 
-    INSTANCE: "InternetService" = None
+    INSTANCE: "InternetService"
 
     ASKAI_INTERNET_DATA_KEY = "askai-internet-data"
 
     @staticmethod
-    def scrap_sites(search: SearchResult) -> Optional[str]:
-        """Scrap a web page and summarize it's contents.
+    def _build_google_query(search: SearchResult) -> str:
+        """Build a Google Search query from search parameters.
         :param search: The AI search parameters.
         """
-        AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.searching())
-        if len(search.sites) > 0:
-            query = "+".join(search.keywords)
-            log.info("Scrapping sites: '%s'", str(", ".join(search.sites)))
-            documents: List[Document] = load_document(AsyncHtmlLoader, list(search.sites))
-            if len(documents) > 0:
-                texts: List[Document] = summarizer.text_splitter.split_documents(documents)
-                v_store = Chroma.from_documents(texts, lc_llm.create_embeddings(), persist_directory=str(PERSIST_DIR))
-                retriever = RetrievalQA.from_chain_type(
-                    llm=lc_llm.create_model(), chain_type="stuff", retriever=v_store.as_retriever()
-                )
-                search_results = retriever.invoke({"query": query})
-                return search_results["result"]
-        return None
-
-    @staticmethod
-    def _build_query(search: SearchResult) -> str:
-        """TODO"""
         query = ""
         # Gather the sites to be used in te search.
         if search.sites:
             query += f" {' OR '.join(['site:' + url for url in search.sites])}"
         # Weather is a filter that does not require any other search parameter.
         if search.filters and any(f.find("weather:") >= 0 for f in search.filters):
             return re.sub(r"^weather:(.*)", r'weather:"\1"', " AND ".join(search.filters))
@@ -85,51 +69,91 @@
         if search.keywords:
             query += f" {' + '.join(search.keywords)} "
         return query
 
     def __init__(self):
         self._google = GoogleSearchAPIWrapper()
         self._tool = Tool(name="google_search", description="Search Google for recent results.", func=self._google.run)
-        self._text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=25)
-
-    @lru_cache
-    def template(self) -> str:
-        return prompt.read_prompt("search-prompt")
+        self._text_splitter = RecursiveCharacterTextSplitter(chunk_size=2000, chunk_overlap=200)
 
     @lru_cache
     def refine_template(self) -> str:
-        return prompt.read_prompt("refine-prompt")
+        return prompt.read_prompt("refine-search")
 
-    def search_google(self, search: SearchResult) -> Optional[str]:
+    def search_google(self, search: SearchResult) -> str:
         """Search the web using google search API.
         Google search operators: https://ahrefs.com/blog/google-advanced-search-operators/
         :param search: The AI search parameters.
         """
         AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.searching())
-        search.sites = search.sites if len(search.sites) > 0 else ['google.com', 'bing.com']
+        search.sites = search.sites if len(search.sites) > 0 else ["google.com", "bing.com"]
         try:
-            query = self._build_query(search).strip()
+            query = self._build_google_query(search).strip()
             log.info("Searching Google for '%s'", query)
             ctx = str(self._tool.run(query))
             llm_prompt = ChatPromptTemplate.from_messages([("system", "{query}\n\n{context}")])
             context: List[Document] = [Document(ctx)]
-            chain = create_stuff_documents_chain(lc_llm.create_chat_model(
-                temperature=Temperature.DATA_ANALYSIS.temp), llm_prompt)
+            chain = create_stuff_documents_chain(
+                lc_llm.create_chat_model(temperature=Temperature.DATA_ANALYSIS.temp), llm_prompt
+            )
             output = chain.invoke({"query": search.question, "context": context})
         except HttpError as err:
             output = msg.fail_to_search(str(err))
 
-        return self.refine_text(search.question, output, search.sites) if output else None
+        return self.refine_search(search.question, output, search.sites)
 
-    def refine_text(self, question: str, context: str, sites: list[str]) -> Optional[str]:
-        """Refines the text retrieved by the search engine."""
+    def scrap_sites(self, search: SearchResult) -> str:
+        """Scrap a web page and summarize it's contents.
+        :param search: The AI search parameters.
+        """
+        AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.scrapping())
+        if len(search.sites) > 0:
+            log.info("Scrapping sites: '%s'", str(", ".join(search.sites)))
+            loader = WebBaseLoader(
+                web_paths=search.sites,
+                bs_kwargs=dict(parse_only=bs4.SoupStrainer(["article", "span", "div", "h1", "h2", "h3"])),
+            )
+            if (page_content := loader.load()) and len(page_content) > 0:
+                splits: List[Document] = summarizer.text_splitter.split_documents(page_content)
+                v_store = Chroma.from_documents(splits, lc_llm.create_embeddings())
+                retriever = v_store.as_retriever()
+                scrap_prompt = PromptTemplate(input_variables=["context", "question"], template=prompt.read_prompt("qstring"))
+
+                def format_docs(docs):
+                    return "\n\n".join(doc.page_content for doc in docs)
+
+                rag_chain = (
+                    {"context": retriever | format_docs, "question": RunnablePassthrough()}
+                    | scrap_prompt
+                    | lc_llm.create_model()
+                    | StrOutputParser()
+                )
+
+                output: Output = rag_chain.invoke(search.question)
+                # cleanup
+                v_store.delete_collection()
+                log.info("Scrapping sites retuned: '%s'", str(output))
+
+                return self.refine_search(search.question, str(output), search.sites)
+        return msg.search_empty()
+
+    def refine_search(self, question: str, context: str, sites: list[str]) -> str:
+        """Refines the text retrieved by the search engine.
+        :param question: The user question, used to refine the context.
+        :param context: The context to refine.
+        :param sites: The list of source sites used on the search.
+        """
         refine_prompt = PromptTemplate.from_template(self.refine_template()).format(
-            idiom=shared.idiom, sources=sites, location=geo_location.location,
-            context=context, question=question)
+            idiom=shared.idiom,
+            sources=sites,
+            location=geo_location.location,
+            datetime=geo_location.datetime,
+            context=context,
+            question=question,
+        )
         log.info("STT::[QUESTION] '%s'", context)
         llm = lc_llm.create_chat_model(temperature=Temperature.CREATIVE_WRITING.temp)
-        output = llm.predict(refine_prompt)
 
-        return output
+        return llm.invoke(refine_prompt).content
 
 
 assert (internet := InternetService().INSTANCE) is not None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/component/recorder.py` & `hspylib_askai-1.0.6/askai/core/component/recorder.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,50 +3,43 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.components
       @file: recorder.py
    @created: Wed, 22 Feb 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 import logging as log
-import os
 from pathlib import Path
 from typing import Callable, List, Optional, Tuple
 
 import pause
-from clitt.core.term.cursor import cursor
-from clitt.core.tui.mselect.mselect import mselect
-from hspylib.core.enums.enumeration import Enumeration
-from hspylib.core.metaclass.singleton import Singleton
-from hspylib.core.tools.commons import file_is_not_empty
-from hspylib.core.zoned_datetime import now_ms
-from speech_recognition import AudioData, Microphone, Recognizer, RequestError, UnknownValueError, WaitTimeoutError
-
+from askai.core.askai_configs import configs
 from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
 from askai.core.component.cache_service import REC_DIR
-from askai.core.support.settings import Settings
 from askai.core.support.utilities import display_text
 from askai.exception.exceptions import IntelligibleAudioError, InvalidInputDevice, InvalidRecognitionApiError
 from askai.language.language import Language
+from clitt.core.term.cursor import cursor
+from clitt.core.tui.mselect.mselect import mselect
+from hspylib.core.enums.enumeration import Enumeration
+from hspylib.core.metaclass.singleton import Singleton
+from hspylib.core.zoned_datetime import now_ms
+from speech_recognition import AudioData, Microphone, Recognizer, RequestError, UnknownValueError, WaitTimeoutError
 
 
 class Recorder(metaclass=Singleton):
     """Provide an interface to record voice using the microphone device."""
 
-    INSTANCE: "Recorder" = None
-
-    ASKAI_SETTINGS_DIR: str = f'{os.getenv("HHS_DIR", os.getenv("TEMP", "/tmp"))}'
-
-    ASKAI_SETTINGS_FILE: str = ".askai.properties"
+    INSTANCE: "Recorder"
 
     class RecognitionApi(Enumeration):
         # fmt: off
         OPEN_AI = 'recognize_whisper'
         GOOGLE = 'recognize_google'
         # fmt: on
 
@@ -56,16 +49,15 @@
         devices = []
         for index, name in enumerate(Microphone.list_microphone_names()):
             devices.append((index, name))
         return devices
 
     def __init__(self):
         self._rec: Recognizer = Recognizer()
-        self._settings: Settings = Settings(self.ASKAI_SETTINGS_FILE, load_dir=self.ASKAI_SETTINGS_DIR)
-        self._devices = []
+        self._devices: list[tuple[int, str]] = []
         self._device_index = None
         self._input_device = None
         self._rec_phrase_limit_s = 10
         self._rec_wait_timeout_s = 0.8
 
     def setup(self) -> None:
         """Setup the recorder."""
@@ -91,15 +83,16 @@
         """
         audio_path = Path(f"{REC_DIR}/askai-stt-{now_ms()}.wav")
         with Microphone(device_index=self._device_index) as source:
             try:
                 self._detect_noise()
                 AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.listening())
                 audio: AudioData = self._rec.listen(
-                    source, phrase_time_limit=self._rec_phrase_limit_s, timeout=self._rec_wait_timeout_s)
+                    source, phrase_time_limit=self._rec_phrase_limit_s, timeout=self._rec_wait_timeout_s
+                )
                 AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.transcribing(), erase_last=True)
                 with open(audio_path, "wb") as f_rec:
                     f_rec.write(audio.get_wav_data())
                     log.debug("Voice recorded and saved as %s", audio_path)
                 if api := getattr(self._rec, recognition_api.value):
                     log.debug("Recognizing voice using %s", recognition_api)
                     assert isinstance(api, Callable)
@@ -129,38 +122,31 @@
                 self._rec.adjust_for_ambient_noise(source, duration=interval)
             except UnknownValueError as err:
                 raise IntelligibleAudioError(f"Unable to detect noise => {str(err)}") from err
 
     def _select_device(self) -> Optional[int]:
         """Select device for recording."""
         done = False
-        filepath: str = f"{self.ASKAI_SETTINGS_DIR}/{self.ASKAI_SETTINGS_FILE}"
-        if not file_is_not_empty(filepath):
-            self._settings.set("askai.recorder.devices", None)
-            self._settings.set("askai.recorder.silence-timeout_ms", 1500)
-            self._settings.set("askai.recorder.phrase.limit_ms", 0)
         available: List[str] = list(
-            filter(lambda d: d, map(str.strip, eval(self._settings.get("askai.recorder.devices") or "[]")))
+            filter(lambda d: d, map(str.strip, configs.recorder_devices))
         )
         while not done:
             if available:
                 for idx, device in self.devices:
                     if device in available and self._test_device(idx):
-                        self._settings.save()
                         return idx
             # Choose device from list
             idx_device: Tuple[int, str] = mselect(
                 self.devices, f"{'-=' * 40}%EOL%AskAI::Select the Input device%EOL%{'=-' * 40}%EOL%"
             )
             if not idx_device:
                 break
             elif self._test_device(idx_device[0]):
                 available.append(idx_device[1])
-                self._settings.set("askai.recorder.devices", available)
-                self._settings.save()
+                configs.add_device(idx_device[1])
                 return idx_device[0]
 
             display_text(f"%HOM%%ED2%Error:{idx_device[1]} does not support INPUTS !%NC%")
             self._devices.remove(idx_device)
             pause.seconds(2)
 
         return None
```

### Comparing `hspylib-askai-1.0.5/askai/core/component/summarizer.py` & `hspylib_askai-1.0.6/askai/core/component/summarizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.component
       @file: summarizer.py
    @created: Mon, 11 Mar 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
 from askai.core.component.cache_service import PERSIST_DIR
 from askai.core.model.summary_result import SummaryResult
 from askai.core.support.langchain_support import lc_llm
 from askai.core.support.utilities import hash_text
@@ -33,15 +33,15 @@
 import logging as log
 import os
 
 
 class Summarizer(metaclass=Singleton):
     """Provide a summarization service to complete queries that require summarization."""
 
-    INSTANCE: "Summarizer" = None
+    INSTANCE: "Summarizer"
 
     ASKAI_SUMMARY_DATA_KEY = "askai-summary-data"
 
     @staticmethod
     def _extract_result(result: dict) -> Tuple[str, str]:
         """Extract the question and answer from the summarization result."""
         question = result["query"] if "query" in result else result["question"]
@@ -55,15 +55,15 @@
         return Path(f"{PERSIST_DIR}/{summary_hash}").exists()
 
     def __init__(self):
         self._retriever = None
         self._folder = None
         self._glob = None
         self._chat_history = None
-        self._text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=25)
+        self._text_splitter = RecursiveCharacterTextSplitter(chunk_size=1000, chunk_overlap=100)
 
     @property
     def persist_dir(self) -> Path:
         summary_hash = hash_text(self.sum_path)
         return Path(f"{PERSIST_DIR}/{summary_hash}")
 
     @property
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/engine/ai_engine.py` & `hspylib_askai-1.0.6/askai/core/engine/ai_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.model
       @file: ai_engine.py
    @created: Fri, 5 May 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 from askai.core.model.ai_model import AIModel
 from askai.core.model.ai_reply import AIReply
 from langchain_core.language_models import BaseChatModel, BaseLLM
 from typing import Any, List, Optional, Protocol
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/engine/engine_factory.py` & `hspylib_askai-1.0.6/askai/core/engine/engine_factory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,37 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.core.engine
+      @file: engine_factory.py
+   @created: Tue, 23 Apr 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
+
+from typing import List
+
+from hspylib.core.metaclass.singleton import Singleton
+from hspylib.core.preconditions import check_not_none
+
 from askai.core.engine.ai_engine import AIEngine
 from askai.core.engine.openai.openai_engine import OpenAIEngine
 from askai.core.engine.openai.openai_model import OpenAIModel
 from askai.exception.exceptions import NoSuchEngineError
-from hspylib.core.metaclass.singleton import Singleton
-from hspylib.core.preconditions import check_not_none
-from typing import List
 
 
 class EngineFactory(metaclass=Singleton):
     """TODO"""
 
-    INSTANCE: "EngineFactory" = None
+    INSTANCE: "EngineFactory"
 
     _ACTIVE_AI_ENGINE: AIEngine = None
 
     @classmethod
     def create_engine(cls, engine_name: str | List[str], engine_model: str | List[str]) -> AIEngine:
         """Find the suitable AI engine according to the provided engine name.
         :param engine_name: the AI engine name.
```

### Comparing `hspylib-askai-1.0.5/askai/core/engine/openai/openai_configs.py` & `hspylib_askai-1.0.6/askai/core/engine/openai/openai_configs.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,32 +3,30 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.engine.openai
       @file: openai_configs.py
    @created: Fri, 12 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
-from typing import Literal
-
-from hspylib.core.config.app_config import AppConfigs
-from hspylib.core.metaclass.singleton import Singleton
-
 from askai.__classpath__ import classpath
 from askai.core.askai_configs import AskAiConfigs
+from hspylib.core.config.app_config import AppConfigs
+from hspylib.core.metaclass.singleton import Singleton
+from typing import Literal
 
 
 class OpenAiConfigs(AskAiConfigs, metaclass=Singleton):
     """Provides access to OpenAI configurations."""
 
-    INSTANCE: "OpenAiConfigs" = None
+    INSTANCE: "OpenAiConfigs"
 
     # The resources folder
     RESOURCE_DIR = str(classpath.resource_path())
 
     def __init__(self):
         super().__init__()
         self._configs = AppConfigs.INSTANCE or AppConfigs(self.RESOURCE_DIR)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/engine/openai/openai_engine.py` & `hspylib_askai-1.0.6/askai/core/engine/openai/openai_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.engine.openai
       @file: openai_engine.py
    @created: Fri, 12 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 
 from askai.core.component.audio_player import AudioPlayer
 from askai.core.component.cache_service import CacheService
 from askai.core.component.recorder import Recorder
 from askai.core.engine.openai.openai_configs import OpenAiConfigs
 from askai.core.engine.openai.openai_model import OpenAIModel
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/engine/openai/openai_model.py` & `hspylib_askai-1.0.6/askai/core/engine/openai/openai_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.engine.openai
       @file: openai_model.py
    @created: Fri, 12 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 from askai.core.model.ai_model import AIModel
 from hspylib.core.enums.enumeration import Enumeration
 from hspylib.core.preconditions import check_not_none
 from typing import List
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/engine/openai/temperature.py` & `hspylib_askai-1.0.6/askai/core/engine/openai/temperature.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.core.engine.openai
+      @file: temperature.py
+   @created: Tue, 23 Apr 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
+
 from hspylib.core.enums.enumeration import Enumeration
 
 
 class Temperature(Enumeration):
     """Provide some recommended temperature x top_p combinations for ChatGPT prompts.
     Ref:. https://community.openai.com/t/cheat-sheet-mastering-temperature-and-top-p-in-chatgpt-api/172683
 
@@ -51,8 +66,7 @@
     @property
     def temp(self) -> float:
         return self.value[0]
 
     @property
     def top_p(self) -> float:
         return self.value[1]
-
```

### Comparing `hspylib-askai-1.0.5/askai/core/features/tools/analysis.py` & `hspylib_askai-1.0.6/askai/core/features/tools/browser.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,53 +1,62 @@
-import logging as log
-from typing import Optional
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 
-from langchain_core.prompts import PromptTemplate
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.core.features.tools.browser
+      @file: browser.py
+   @created: Mon, 01 Apr 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
 
-from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
 from askai.core.askai_prompt import prompt
+from askai.core.component.cache_service import cache
+from askai.core.component.geo_location import geo_location
+from askai.core.component.internet_service import internet
 from askai.core.engine.openai.temperature import Temperature
+from askai.core.model.search_result import SearchResult
 from askai.core.support.langchain_support import lc_llm
+from askai.core.support.object_mapper import object_mapper
 from askai.core.support.shared_instances import shared
-from askai.core.support.text_formatter import text_formatter
+from langchain_core.prompts import PromptTemplate
+from typing import Optional
+
+import logging as log
 
 
-def check_output(question: str, context: str) -> Optional[str]:
-    """Handle 'Text analysis', invoking: analyze(question: str). Analyze the context and answer the question.
-    :param question: The question about the content to be analyzed.
-    :param context: The context of the question.
+def browse(query: str) -> Optional[str]:
+    """Fetch the information from the Internet.
+    :param query: The search query.
     """
-    log.info("Analysis::[QUESTION] '%s'  context=%s", question, context)
-    llm = lc_llm.create_chat_model(Temperature.CREATIVE_WRITING.temp)
     template = PromptTemplate(
-        input_variables=['context', 'question'],
-        template=prompt.read_prompt('analysis-prompt'))
-    final_prompt = template.format(context=context, question=question)
-
-    if output := llm.predict(final_prompt):
-        shared.context.push("CONTEXT", question)
-        shared.context.push("CONTEXT", output, 'assistant')
-        AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.analysis(), verbosity='debug')
-
-    return text_formatter.ensure_ln(output)
-
-
-def stt(question: str, context: str) -> str:
-    """Process the given context according to STT rules.
-    :param question: The question about the content to be summarized.
-    :param context: The context of the question.
-    """
-    template = PromptTemplate(input_variables=[
-        'idiom', 'context', 'question'
-    ], template=prompt.read_prompt('stt-prompt'))
-    final_prompt = template.format(
-        idiom=shared.idiom, context=context, question=question
+        input_variables=["idiom", "datetime", "location", "question"], template=prompt.read_prompt("search-builder")
     )
-    log.info("STT::[QUESTION] '%s'", context)
-    llm = lc_llm.create_chat_model(temperature=Temperature.CREATIVE_WRITING.temp)
-
-    if output := llm.predict(final_prompt):
-        shared.context.push("CONTEXT", question)
-        shared.context.push("CONTEXT", output, 'assistant')
+    final_prompt: str = template.format(
+        idiom=shared.idiom, datetime=geo_location.datetime, location=geo_location.location, question=query
+    )
+    log.info("Browser::[QUESTION] '%s'  context=''", final_prompt)
+    llm = lc_llm.create_chat_model(Temperature.DATA_ANALYSIS.temp)
+    response: str = llm.invoke(final_prompt).content
+
+    if response and shared.UNCERTAIN_ID not in response:
+        search: SearchResult = object_mapper.of_json(response, SearchResult)
+        if not isinstance(search, SearchResult):
+            log.error(msg.invalid_response(search))
+            output = response.strip()
+        else:
+            output = internet.search_google(search)
+            if output:
+                shared.context.push("HISTORY", query)
+                shared.context.push("HISTORY", output, "assistant")
+                cache.save_reply(query, output)
+            else:
+                output = msg.search_empty()
+    else:
+        output = msg.translate("Sorry, I don't know.")
 
-    return text_formatter.ensure_ln(output)
+    return output
```

### Comparing `hspylib-askai-1.0.5/askai/core/features/tools/summarization.py` & `hspylib_askai-1.0.6/askai/core/features/tools/summarization.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,49 @@
-import logging as log
-import os
-from typing import Optional
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
 
-from hspylib.core.tools.text_tools import ensure_startswith
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.core.features.tools.summarization
+      @file: summarization.py
+   @created: Mon, 01 Apr 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
 
 from askai.core.askai_events import AskAiEvents
 from askai.core.askai_messages import msg
 from askai.core.component.summarizer import summarizer
 from askai.core.support.shared_instances import shared
 from askai.core.support.utilities import display_text
 from askai.exception.exceptions import DocumentsNotFound
+from hspylib.core.tools.text_tools import ensure_startswith
+from typing import Optional
 
+import logging as log
+import os
 
-def summarize(folder: str, glob: str) -> Optional[str]:
-    """Summarize files and folders."""
+
+def summarize(base_folder: str, glob: str) -> Optional[str]:
+    """Summarize files and folders.
+    :param base_folder: The base folder to be summarized.
+    :param glob: The glob to match the files to be summarized.
+    """
     try:
-        glob = ensure_startswith(glob, '**/')
-        if not summarizer.exists(folder, glob):
-            if not summarizer.generate(folder, glob):
+        glob = ensure_startswith(glob, "**/")
+        if not summarizer.exists(base_folder, glob):
+            if not summarizer.generate(base_folder, glob):
                 return msg.summary_not_possible()
         else:
-            summarizer.folder = folder
+            summarizer.folder = base_folder
             summarizer.glob = glob
-            log.info("Reusing persisted summarized content: '%s/%s'", folder, glob)
+            log.info("Reusing persisted summarized content: '%s/%s'", base_folder, glob)
         output = _qna()
     except (FileNotFoundError, ValueError, DocumentsNotFound) as err:
         output = msg.summary_not_possible(err)
 
     return output
 
 
@@ -39,17 +56,15 @@
         output = os.linesep.join([r.answer for r in results]).strip()
     return output
 
 
 def _qna() -> str:
     """Questions and Answers about the summarized content."""
     display_text(
-        f"# {msg.enter_qna()} %EOL%"
-        f"> Content:  {summarizer.sum_path} %EOL%%EOL%"
-        f"`{msg.press_esc_enter()}` %EOL%"
+        f"# {msg.enter_qna()} %EOL%" f"> Content:  {summarizer.sum_path} %EOL%%EOL%" f"`{msg.press_esc_enter()}` %EOL%"
     )
     AskAiEvents.ASKAI_BUS.events.reply.emit(message=msg.qna_welcome())
     while question := shared.input_text(f"{shared.username}: %GREEN%"):
         if not (output := _ask_and_reply(question)):
             break
         AskAiEvents.ASKAI_BUS.events.reply.emit(message=f"{output}")
     display_text(f"# {msg.leave_qna()} %EOL%")
```

### Comparing `hspylib-askai-1.0.5/askai/core/model/ai_model.py` & `hspylib_askai-1.0.6/askai/core/model/ai_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.model
       @file: ai_model.py
    @created: Fri, 5 May 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 from typing import Protocol
 
 
 class AIModel(Protocol):
     """Provide an interface for AI models."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/model/ai_reply.py` & `hspylib_askai-1.0.6/askai/core/model/ai_reply.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.engine.model
       @file: ai_reply.py
    @created: Fri, 12 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
+
 from dataclasses import dataclass
 
 
 @dataclass
 class AIReply:
     """Data class that represent AI replies."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/model/chat_context.py` & `hspylib_askai-1.0.6/askai/core/support/chat_context.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,109 +1,120 @@
 """
    @project: HsPyLib-AskAI
-   @package: askai.core.model
+   @package: askai.core.support.chat_context
       @file: chat_context.py
    @created: Fri, 28 Feb 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 
-import os
-from collections import defaultdict, namedtuple
-from functools import reduce
-from typing import Any, List, Literal, Optional, TypeAlias
-
+from askai.exception.exceptions import TokenLengthExceeded
+from collections import defaultdict, deque, namedtuple
+from functools import partial, reduce
 from hspylib.core.zoned_datetime import now
+from langchain_community.chat_message_histories.in_memory import ChatMessageHistory
+from langchain_core.messages import AIMessage, HumanMessage, SystemMessage
+from typing import Any, Literal, Optional, TypeAlias
 
-from askai.exception.exceptions import TokenLengthExceeded
+import os
 
 ChatRoles: TypeAlias = Literal["system", "human", "assistant"]
 
 ContextRaw: TypeAlias = list[dict[str, str]]
 
 LangChainContext: TypeAlias = list[tuple[str, str]]
 
-ContextEntry = namedtuple("ContextEntry", ["created_at", "role", "content"], rename=False)
+ContextEntry = namedtuple("ContextEntry", ["created_at", "role", "content"])
 
 
 class ChatContext:
     """Provide a chat context helper for AI engines."""
 
-    def __init__(self, token_limit: int):
-        self._context: dict[Any, list] = defaultdict(list)
+    LANGCHAIN_ROLE_MAP: dict = {"human": HumanMessage, "system": SystemMessage, "assistant": AIMessage}
+
+    def __init__(self, token_limit: int, max_context_length: int):
+        self._store: dict[Any, deque] = defaultdict(partial(deque, maxlen=max_context_length))
         self._token_limit: int = token_limit * 1024  # The limit is given in KB
 
     def __str__(self):
-        return os.linesep.join(f"'{k}': '{v}'" for k, v in self._context.items())
+        return os.linesep.join(f"'{k}': '{v}'" for k, v in self._store.items())
 
-    def __getitem__(self, key) -> List[ContextEntry]:
-        return self._context[key]
+    def __getitem__(self, key) -> deque[ContextEntry]:
+        return self._store[key]
 
     def push(self, key: str, content: Any, role: ChatRoles = "human") -> ContextRaw:
         """Push a context message to the chat with the provided role."""
         entry = ContextEntry(now(), role, str(content))
-        ctx = self._context[key]
+        ctx = self._store[key]
         token_length = reduce(lambda total, e: total + len(e.content), ctx, 0) if len(ctx) > 0 else 0
         if (token_length := token_length + len(content)) > self._token_limit:
             raise TokenLengthExceeded(f"Required token length={token_length}  limit={self._token_limit}")
         ctx.append(entry)
         return self.get(key)
 
     def set(self, key: str, content: Any, role: ChatRoles = "human") -> ContextRaw:
         """Set the context to the chat with the provided role."""
         self.clear(key)
         return self.push(key, content, role)
 
     def remove(self, key: str, index: int) -> Optional[str]:
         """Remove a context message from the chat at the provided index."""
         val = None
-        if ctx := self._context[key]:
+        if ctx := self._store[key]:
             if index < len(ctx):
                 val = ctx[index]
                 del ctx[index]
         return val
 
     def get(self, key: str) -> ContextRaw:
         """Retrieve a context from the specified by key."""
-        return [{"role": ctx.role, "content": ctx.content} for ctx in self._context[key]] or []
+        return [{"role": ctx.role, "content": ctx.content} for ctx in self._store[key]] or []
 
     def join(self, *keys: str) -> LangChainContext:
         """Join contexts specified by keys."""
         context: LangChainContext = []
         token_length = 0
         for key in keys:
             ctx: ContextRaw = self.get(key)
-            content: str = os.linesep.join([tk['content'] for tk in ctx])
+            content: str = os.linesep.join([tk["content"] for tk in ctx])
             token_length += len(content or "")
             if token_length > self._token_limit:
                 raise TokenLengthExceeded(f"Required token length={token_length}k  limit={self._token_limit}k")
             if content and ctx not in context:
-                list(map(context.append, [(t['role'], t['content']) for t in ctx]))
+                list(map(context.append, [(t["role"], t["content"]) for t in ctx]))
         return context
 
-    def flat(self, *keys: str) -> str:
+    def flat(self, *keys: str) -> ChatMessageHistory:
         """Flatten contexts specified by keys."""
-        return os.linesep.join([f"\n{ctx[0].upper()}\n{ctx[1]}" for ctx in self.join(*keys)])
+        history = ChatMessageHistory()
+        flatten: LangChainContext = self.join(*keys)
+        for ctx_entry in flatten:
+            mtype = self.LANGCHAIN_ROLE_MAP[ctx_entry[0]]
+            history.add_message(mtype(ctx_entry[1]))
+        return history
 
     def clear(self, *keys: str) -> int:
         """Clear the all the chat context specified by key."""
         for key in keys:
-            if self._context[key]:
-                del self._context[key]
-        return len(self._context)
+            if self._store[key]:
+                del self._store[key]
+        return len(self._store)
 
     def forget(self) -> None:
         """Forget all entries pushed to the chat context."""
-        del self._context
-        self._context = defaultdict(list)
+        del self._store
+        self._store = defaultdict(list)
 
 
-if __name__ == '__main__':
-    c = ChatContext(1000)
-    c.push("TESTE", 'What is the size of the moon?')
-    c.push("TESTE", 'What is the size of the moon?', 'assistant')
-    c.push("TESTE", 'Who are you?')
-    c.push("TESTE", "I'm Taius, you digital assistant", 'assistant')
-    print(c.join("TESTE"))
+if __name__ == "__main__":
+    c = ChatContext(1000, 5)
+    c.push("TESTE", "1 What is the size of the moon?")
+    c.push("TESTE", "2 What is the size of the moon?", "assistant")
+    c.push("TESTE", "3 Who are you?")
+    c.push("TESTE", "4 I'm Taius, you digital assistant", "assistant")
+    c.push("TESTE", "5 I'm Taius, you digital assistant", "assistant")
+    c.push("TESTE", "6 I'm Taius, you digital assistant", "assistant")
+    c.push("TESTE", "7 I'm Taius, you digital assistant", "assistant")
+    print(c.flat("TESTE"))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/model/search_result.py` & `hspylib_askai-1.0.6/askai/core/model/search_result.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.model
       @file: search_result.py
    @created: Sun, 12 Mar 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 from dataclasses import dataclass
 from typing import List
 
 import json
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/model/summary_result.py` & `hspylib_askai-1.0.6/askai/core/model/summary_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.model
       @file: summary_result.py
    @created: Sun, 10 Mar 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 from dataclasses import dataclass
 
 import json
 
 
 @dataclass
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/model/terminal_command.py` & `hspylib_askai-1.0.6/askai/core/model/terminal_command.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 """
    @project: HsPyLib-AskAI
    @package: askai.core.model
       @file: terminal_command.py
    @created: Thu, 29 Feb 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 
 from dataclasses import dataclass
+from functools import lru_cache
 from os.path import basename
 from typing import Literal, TypeAlias
 
 import json
 import os
 import platform
 
 SupportedPlatforms: TypeAlias = Literal["linux", "windows", "darwin"] | None
 
 SupportedShells: TypeAlias = Literal["bash", "csh", "dash", "ksh", "tcsh", "zsh", "sh"] | None
 
 
+@lru_cache
 def get_os() -> SupportedPlatforms:
     os_name = platform.system().lower()
     return os_name if os_name and os_name in ["linux", "windows", "darwin"] else None
 
 
+@lru_cache
 def get_shell() -> SupportedShells:
     shell = basename(os.getenv("SHELL", "bash")).lower()
     return shell if shell and shell in ["bash", "csh", "dash", "ksh", "tcsh", "zsh", "sh"] else None
 
 
+@lru_cache
 def get_user() -> str:
     return os.getenv("USER", "user")
 
 
 @dataclass
 class TerminalCommand:
     """Keep track of the executed terminal commands."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/support/langchain_support.py` & `hspylib_askai-1.0.6/askai/core/support/langchain_support.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-from askai.core.model.chat_context import ChatContext
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.core.support.langchain_support
+      @file: langchain_support.py
+   @created: Fri, 28 Feb 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
+
 from askai.core.support.shared_instances import shared
 from functools import lru_cache
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_not_none
 from langchain_core.documents import Document
-from langchain_core.messages import AIMessage, HumanMessage, SystemMessage
-from typing import Any, Dict, List, Type
+from typing import Any, List, Type
 
 
 def load_document(loader_type: Type, url: str | List[str]) -> List[Document]:
     """TODO"""
     return loader_type(url).load()
 
 
 class LangChainSupport(metaclass=Singleton):
     """TODO"""
 
-    INSTANCE: "" = None
-
-    LANGCHAIN_ROLE_MAP: Dict = {"user": HumanMessage, "system": SystemMessage, "assistant": AIMessage}
+    INSTANCE: ""
 
     @staticmethod
     @lru_cache
     def create_model(temperature: float = 0.0, top_p: float = 0.0) -> Any:
         """TODO"""
         check_not_none(shared.engine, "AI Engine was not created yet!")
         return shared.engine.lc_model(temperature, top_p)
@@ -37,16 +45,9 @@
     @staticmethod
     @lru_cache
     def create_embeddings() -> Any:
         """TODO"""
         check_not_none(shared.engine, "AI Engine was not created yet!")
         return shared.engine.lc_embeddings()
 
-    @classmethod
-    @lru_cache
-    def get_context(cls, key: str) -> List:
-        """TODO"""
-        context: List[ChatContext.ContextEntry] = shared.context[key]
-        return [cls.LANGCHAIN_ROLE_MAP[c.role](content=c.content) for c in context] or []
-
 
 assert (lc_llm := LangChainSupport().INSTANCE) is not None
```

### Comparing `hspylib-askai-1.0.5/askai/core/support/object_mapper.py` & `hspylib_askai-1.0.6/askai/core/support/object_mapper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """
    @project: HsPyLib-AskAI
    @package: askai.core.component
       @file: object_mapper.py
    @created: Fri, 28 Feb 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 
 from askai.exception.exceptions import InvalidJsonMapping, InvalidMapping
 from hspylib.core.enums.enumeration import Enumeration
 from hspylib.core.metaclass.singleton import Singleton
 from inspect import isclass
 from json import JSONDecodeError
@@ -23,15 +23,15 @@
 
 FnConverter: TypeAlias = Callable[[Any, Type], Any]
 
 
 class ObjectMapper(metaclass=Singleton):
     """Provide a utility class to convert one object into the other, and vice-versa."""
 
-    INSTANCE: "ObjectMapper" = None
+    INSTANCE: "ObjectMapper"
 
     class ConversionMode(Enumeration):
         """TODO"""
 
         # fmt: off
         STANDARD    = '_standard_converter'
         STRICT      = '_strict_converter'
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/support/presets.py` & `hspylib_askai-1.0.6/askai/core/support/presets.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
    @project: HsPyLib-AskAI
    @package: askai.core.support
       @file: presets.py
    @created: Tue, 16 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 from functools import lru_cache
 from string import Template
 from textwrap import dedent
 
 
 class Presets:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/core/support/shared_instances.py` & `hspylib_askai-1.0.6/askai/core/support/shared_instances.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,59 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""
+   @project: "askai"
+   @package: "askai".main.askai.core.support
+      @file: shared_instances.py
+   @created: Tue, 23 Apr 2024
+    @author: "<B>H</B>ugo <B>S</B>aporetti <B>J</B>unior")"
+      @site: "https://github.com/yorevs/askai")
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
+
+from functools import lru_cache
 from typing import Optional
 
 from clitt.core.term.terminal import terminal
 from clitt.core.tui.line_input.line_input import line_input
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.preconditions import check_state
 from hspylib.modules.cli.keyboard import Keyboard
+from langchain.memory import ConversationBufferWindowMemory
+from langchain.memory.chat_memory import BaseChatMemory
 
 from askai.core.askai_configs import configs
 from askai.core.askai_prompt import prompt
 from askai.core.engine.ai_engine import AIEngine
 from askai.core.engine.engine_factory import EngineFactory
-from askai.core.model.chat_context import ChatContext
+from askai.core.support.chat_context import ChatContext
 from askai.core.support.utilities import display_text
 
 
 class SharedInstances(metaclass=Singleton):
-    """TODO"""
+    """Provides access to shared instances."""
 
-    INSTANCE: "SharedInstances" = None
+    INSTANCE: "SharedInstances"
 
     # This is the uuid used in the prompts to indicate that the AI does not know the answer.
     UNCERTAIN_ID: str = "bde6f44d-c1a0-4b0c-bd74-8278e468e50c"
 
+    # This is the uuid used in the prompts to indicate that the response is negative.
+    NEGATIVE_ID: str = "1b11b759-e50e-44de-b5b2-4879354fd9cf"
+
     def __init__(self) -> None:
-        self._engine: Optional[AIEngine] = None
-        self._context: Optional[ChatContext] = None
+        self._engine: AIEngine | None = None
+        self._context: ChatContext | None = None
+        self._memory: BaseChatMemory | None = None
         self._idiom: str = configs.language.idiom
+        self._max_context_size: int = configs.max_context_size
+        self._max_iteractions: int = configs.max_iteractions
 
     @property
     def engine(self) -> Optional[AIEngine]:
         return self._engine
 
     @engine.setter
     def engine(self, value: AIEngine) -> None:
@@ -53,26 +77,41 @@
     def username(self) -> str:
         return f"%WHITE%  {prompt.user.title()}%NC%"
 
     @property
     def idiom(self) -> str:
         return self._idiom
 
+    @property
+    def max_context_size(self) -> int:
+        return self._max_context_size
+
+    @property
+    def max_iteractions(self) -> int:
+        return self._max_iteractions
+
     def create_engine(self, engine_name: str, model_name: str) -> AIEngine:
         """TODO"""
         if self._engine is None:
             self._engine = EngineFactory.create_engine(engine_name, model_name)
         return self._engine
 
     def create_context(self, token_limit: int) -> ChatContext:
         """TODO"""
         if self._context is None:
-            self._context = ChatContext(token_limit)
+            self._context = ChatContext(token_limit, self.max_context_size)
         return self._context
 
+    @lru_cache
+    def create_chat_memory(self) -> BaseChatMemory:
+        """TODO"""
+        if self._memory is None:
+            self._memory = ConversationBufferWindowMemory(memory_key="chat_history", k=self.max_context_size, return_messages=True)
+        return self._memory
+
     def input_text(self, input_prompt: str) -> Optional[str]:
         """Prompt for user input.
         :param input_prompt: The prompt to display to the user.
         """
         ret = None
         while ret is None:
             if (ret := line_input(input_prompt)) == Keyboard.VK_CTRL_L:  # Use STT as input method.
```

### Comparing `hspylib-askai-1.0.5/askai/core/support/text_formatter.py` & `hspylib_askai-1.0.6/askai/core/support/text_formatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,37 @@
-import os
-import re
-from textwrap import dedent
-from typing import Any
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.core.support.text_formatter
+      @file: text_formatter.py
+   @created: Fri, 28 Feb 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
 
 from hspylib.core.metaclass.singleton import Singleton
 from hspylib.core.tools.text_tools import ensure_endswith, ensure_startswith
 from hspylib.modules.cli.vt100.vt_code import VtCode
 from hspylib.modules.cli.vt100.vt_color import VtColor
 from rich.console import Console
 from rich.markdown import Markdown
 from rich.text import Text
+from textwrap import dedent
+from typing import Any
+
+import os
+import re
 
 
 class TextFormatter(metaclass=Singleton):
     """TODO"""
 
-    INSTANCE: "TextFormatter" = None
+    INSTANCE: "TextFormatter"
 
     CHAT_ICONS = {
         "": "\n%RED%  Error: ",
         "": "\n>   *TIP:* ",
         "": "\n>   *Analysis:* ",
         "": "\n>   *Summary:* ",
         "": "\n>   *Joke:* ",
```

### Comparing `hspylib-askai-1.0.5/askai/core/support/utilities.py` & `hspylib_askai-1.0.6/askai/core/support/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HsPyLib-AskAI
-   @package: askai.core.support
+   @package: askai.core.support.utilities
       @file: utilities.py
    @created: Wed, 10 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
-import hashlib
-import mimetypes
-import os
-import re
-import sys
-from os.path import basename, dirname
-from pathlib import Path
-from typing import Any, Optional, Tuple
-
-import pause
+from askai.core.support.presets import Presets
+from askai.core.support.text_formatter import text_formatter
+from askai.language.language import Language
 from clitt.core.term.cursor import Cursor
 from hspylib.core.enums.charset import Charset
 from hspylib.core.preconditions import check_argument
 from hspylib.core.tools.commons import file_is_not_empty, sysout
 from hspylib.core.tools.text_tools import ensure_endswith
 from hspylib.modules.cli.vt100.vt_color import VtColor
+from os.path import basename, dirname
+from pathlib import Path
+from typing import Any, Optional, Tuple
 
-from askai.core.support.presets import Presets
-from askai.core.support.text_formatter import text_formatter
-from askai.language.language import Language
+import hashlib
+import mimetypes
+import os
+import pause
+import re
+import sys
 
 
 def read_stdin() -> Optional[str]:
     """TODO"""
     if not sys.stdin.isatty():
         return sys.stdin.read()
     return None
@@ -154,32 +153,33 @@
     if command_line and (cmd_path := re.search(re_path, command_line, flags)):
         if (extracted := cmd_path.group(1).strip().replace("\\ ", " ")) and (_path_ := Path(extracted)).exists():
             if _path_.is_dir() or (extracted := dirname(extracted)):
                 return extracted if extracted and Path(extracted).is_dir() else None
     return None
 
 
-def extract_command(markdown_text: str, flags: int = re.IGNORECASE | re.MULTILINE) -> Optional[Tuple[str, str]]:
-    """Extract command from the markdown code block formatted text.
-    :param markdown_text: The markdown formatted command line text.
-    :param flags: Regex match flags.
+def extract_codeblock(text: str) -> Tuple[Optional[str], str]:
+    """Extract language and actual code from a markdown multi-line code block.
+    :param text: The markdown formatted text.
     """
+    flags: int = re.IGNORECASE | re.MULTILINE
     # Match a terminal command formatted in a markdown code block.
     re_command = r"^`{3}((\w+)\s*)?(.+)\s*?`{3}$"
-    if markdown_text and (mat := re.search(re_command, markdown_text.replace("\n", " ").strip(), flags)):
+    if text and (mat := re.search(re_command, text.replace("\n", " ").strip(), flags)):
         if mat and len(mat.groups()) == 3:
-            shell, cmd = mat.group(1) or "", mat.group(3) or ""
-            return shell.strip(), cmd.strip()
-    return None
+            lang, code = mat.group(1) or "", mat.group(3) or ""
+            return lang.strip(), code.strip()
+
+    return None, text
 
 
 def media_type_of(pathname: str) -> Optional[tuple[str, ...]] | None:
     """Return the file media type, or none is guessing was not possible.
     :param pathname: The file path to check.
     """
     mimetypes.init()
     mtype, _ = mimetypes.guess_type(basename(pathname))
 
     if mtype is not None:
-        return tuple(mtype.split('/'))
+        return tuple(mtype.split("/"))
 
     return None
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/exception/exceptions.py` & `hspylib_askai-1.0.6/askai/exception/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 """
    @project: HsPyLib-CFMan
-   @package: askai.exception
+   @package: askai.exception.exceptions
       @file: exceptions.py
    @created: Fri, 12 May 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 """
 
 from hspylib.core.exception.exceptions import HSBaseException
 
 
 class NoSuchEngineError(HSBaseException):
     """Raised when the provided engine does not exist"""
@@ -64,14 +64,12 @@
     """Raised when the number of executed actions exceeded the limit."""
 
 
 class ImpossibleQuery(HSBaseException):
     """Raised when tracing or executing an action plan is/was not possible."""
 
 
-class UnintelligibleQuery(HSBaseException):
-    """Raised when received an intelligible question."""
-
-
 class TerminatingQuery(HSBaseException):
     """Raised when received a terminating question."""
 
+class InvalidStructuredResponse(HSBaseException):
+    """Raised when received an invalid structured response."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `hspylib-askai-1.0.5/askai/language/argos_translator.py` & `hspylib_askai-1.0.6/askai/language/argos_translator.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,33 @@
-from argostranslate import package, translate
-from argostranslate.translate import ITranslation
-from askai.core.component.cache_service import CACHE_DIR
-from askai.exception.exceptions import TranslationPackageError
-from askai.language.language import Language
-from functools import lru_cache
-from hspylib.core.metaclass.singleton import Singleton
-from typing import Optional
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.language.argos_translator
+      @file: argos_translator.py
+   @created: Fri, 5 Jan 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
 
 import logging as log
 import os
 import sys
+from functools import lru_cache
+from typing import Optional
+
+from argostranslate import package, translate
+from argostranslate.translate import ITranslation
+
+from askai.exception.exceptions import TranslationPackageError
+from askai.language.language import Language
 
 
 class ArgosTranslator:
     """Provides a multilingual offline translation engine.
     Language packages are downloaded at: ~/.local/share/argos-translate/packages
     """
```

### Comparing `hspylib-askai-1.0.5/askai/language/language.py` & `hspylib_askai-1.0.6/askai/language/language.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,28 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+"""
+   @project: HsPyLib-AskAI
+   @package: askai.language.language
+      @file: language.py
+   @created: Fri, 5 Jan 2024
+    @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior
+      @site: https://github.com/yorevs/askai
+   @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
+
+   Copyright (c) 2024, HomeSetup
+"""
+
+import re
+from typing import Tuple
+
 from hspylib.core.enums.charset import Charset
 from hspylib.core.enums.enumeration import Enumeration
 from hspylib.core.tools.dict_tools import get_or_default
-from typing import Tuple
-
-import re
 
 
 class Language(Enumeration):
     """Enumeration to wrap all standard languages.
     Ref:. https://docs.oracle.com/cd/E23824_01/html/E26033/glset.html
     """
```

### Comparing `hspylib-askai-1.0.5/hspylib_askai.egg-info/PKG-INFO` & `hspylib_askai-1.0.6/hspylib_askai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hspylib-askai
-Version: 1.0.5
+Version: 1.0.6
 Summary: HomeSetup - AskAI
 Home-page: https://github.com/yorevs/hspylib
 Author: Hugo Saporetti Junior
 Author-email: yorevs@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/yorevs/hspylib
 Project-URL: PyPi, https://pypi.org/project/hspylib-askai/
@@ -19,28 +19,30 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Terminals
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Requires-Dist: hspylib>=1.12.35
-Requires-Dist: hspylib-clitt>=0.9.119
+Requires-Dist: hspylib>=1.12.36
+Requires-Dist: hspylib-clitt>=0.9.122
+Requires-Dist: hspylib-setman>=0.10.34
 Requires-Dist: retry2==0.9.5
 Requires-Dist: pause==0.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: argostranslate==1.9.1
 Requires-Dist: protobuf==4.22.1
 Requires-Dist: torch==2.2.0
 Requires-Dist: stanza==1.1.1
 Requires-Dist: soundfile==0.12.1
 Requires-Dist: urllib3==1.26.18
 Requires-Dist: langchain>=0.1.12
 Requires-Dist: langchain-openai==0.0.8
 Requires-Dist: langchain-community==0.0.28
+Requires-Dist: langchainhub
 Requires-Dist: unstructured==0.12.4
 Requires-Dist: unstructured[md]==0.12.4
 Requires-Dist: python-magic-bin==0.4.14
 Requires-Dist: tiktoken==0.6.0
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: html2text==2024.2.26
 Requires-Dist: PyAudio==0.2.14
@@ -50,35 +52,40 @@
 Requires-Dist: openai==1.14.1
 Requires-Dist: chromadb==0.4.24
 Requires-Dist: opentelemetry-api==1.22.0
 Requires-Dist: opentelemetry-sdk==1.22.0
 Requires-Dist: opentelemetry-proto==1.22.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: pytz==2024.1
-Requires-Dist: schedule==1.2.1
+Requires-Dist: bs4==0.0.2
+Requires-Dist: fake_useragent==1.5.1
 
-<img src="https://iili.io/JEatihb.png" width="64" height="64" align="right" />
+<img src="https://iili.io/J8wvc1n.png" width="64" height="64" align="right" />
 
 # AskAI
 >
 > Unleash the Power of AI in Your Terminal
 
 [![Terminal](https://badgen.net/badge/icon/terminal?icon=terminal&label)](https://github.com/yorevs/homesetup)
 [![License](https://badgen.net/badge/license/MIT/gray)](LICENSE.md)
-[![Release](https://badgen.net/badge/release/v1.0.5/gray)](docs/CHANGELOG.md#unreleased)
+[![Release](https://badgen.net/badge/release/v1.0.6/gray)](docs/CHANGELOG.md#unreleased)
 [![Donate](https://badgen.net/badge/paypal/donate/yellow)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=J5CDEFLF6M3H4)
 [![build-and-test](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml/badge.svg)](https://github.com/yorevs/askai/actions/workflows/build-and-test.yml)
 
-<img src="https://iili.io/JGv7BTP.png)" width="360" height="360" align="right" />
+<img src="https://iili.io/J8vkAYX.png" width="100%" height="100%" />
+
+---
+
+<img src="https://iili.io/J8wrBSe.png" width="360" height="360" align="right" />
 
 Born from the idea of empowering individuals with disabilities to navigate the digital world effortlessly, AskAI stands as a beacon of accessibility in the realm of computing. It emerges as a revolutionary solution, harnessing the prowess of AI to bridge the gap between users and the terminal interface. With its intuitive design, AskAI welcomes users of all abilities, eliminating the need for extensive familiarity with shells like bash or zsh. Now, individuals with disabilities can effortlessly command their machines, whether it involves listing files and folders, summarizing documents, accessing real-time data, or delving into a myriad of other functions.
 
 At the heart of AskAI lies its innovative integration of Speech-to-Text and Text-to-Speech technologies, offering a seamless experience for both visually and hearing impaired users. Through these cutting-edge features, individuals can interact with their computers using their natural voice, transcending the barriers imposed by traditional input methods. Moreover, AskAI introduces a unique push-to-talk input mechanism, enabling users to issue commands effortlessly, enhancing the fluidity and ease of interaction.
 
-<img src="https://iili.io/JMWbjf4.jpg)" style="padding-right: 10px" width="258" height="170" align="left" />
+<img src="https://iili.io/J8wiCqQ.png" style="padding-right: 10px" width="238" height="170" align="left" />
 
 Furthermore, AskAI embraces diversity by breaking language barriers, ensuring that no matter the tongue spoken, users can communicate effectively with their systems. Its adaptive language capabilities ensure that commands are understood and executed accurately, regardless of linguistic nuances. By championing inclusivity on all fronts, AskAI redefines the landscape of computing accessibility, empowering individuals with disabilities to navigate the digital realm with confidence and autonomy.
 
 
 > The world speaks many languages. AskAI understands them all.
 
 The see a brief demo about AskAI feature check our asciinema video.
```

### Comparing `hspylib-askai-1.0.5/hspylib_askai.egg-info/SOURCES.txt` & `hspylib_askai-1.0.6/hspylib_askai.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 askai/welcome.txt
 askai/core/__init__.py
 askai/core/askai.py
 askai/core/askai_configs.py
 askai/core/askai_events.py
 askai/core/askai_messages.py
 askai/core/askai_prompt.py
+askai/core/askai_settings.py
 askai/core/component/__init__.py
 askai/core/component/audio_player.py
 askai/core/component/cache_service.py
 askai/core/component/geo_location.py
 askai/core/component/internet_service.py
 askai/core/component/recorder.py
 askai/core/component/summarizer.py
@@ -30,30 +31,31 @@
 askai/core/features/__init__.py
 askai/core/features/actions.py
 askai/core/features/router.py
 askai/core/features/tools/__init__.py
 askai/core/features/tools/analysis.py
 askai/core/features/tools/browser.py
 askai/core/features/tools/general.py
+askai/core/features/tools/generation.py
 askai/core/features/tools/summarization.py
 askai/core/features/tools/terminal.py
 askai/core/model/__init__.py
+askai/core/model/action_plan.py
 askai/core/model/ai_model.py
 askai/core/model/ai_reply.py
-askai/core/model/chat_context.py
 askai/core/model/query_type.py
 askai/core/model/rag_response.py
 askai/core/model/search_result.py
 askai/core/model/summary_result.py
 askai/core/model/terminal_command.py
 askai/core/support/__init__.py
+askai/core/support/chat_context.py
 askai/core/support/langchain_support.py
 askai/core/support/object_mapper.py
 askai/core/support/presets.py
-askai/core/support/settings.py
 askai/core/support/shared_instances.py
 askai/core/support/text_formatter.py
 askai/core/support/utilities.py
 askai/exception/__init__.py
 askai/exception/exceptions.py
 askai/language/__init__.py
 askai/language/argos_translator.py
```

### Comparing `hspylib-askai-1.0.5/hspylib_askai.egg-info/requires.txt` & `hspylib_askai-1.0.6/hspylib_askai.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-hspylib>=1.12.35
-hspylib-clitt>=0.9.119
+hspylib>=1.12.36
+hspylib-clitt>=0.9.122
+hspylib-setman>=0.10.34
 retry2==0.9.5
 pause==0.3
 requests==2.31.0
 argostranslate==1.9.1
 protobuf==4.22.1
 torch==2.2.0
 stanza==1.1.1
 soundfile==0.12.1
 urllib3==1.26.18
 langchain>=0.1.12
 langchain-openai==0.0.8
 langchain-community==0.0.28
+langchainhub
 unstructured==0.12.4
 unstructured[md]==0.12.4
 python-magic-bin==0.4.14
 tiktoken==0.6.0
 aiohttp==3.9.3
 html2text==2024.2.26
 PyAudio==0.2.14
@@ -25,8 +27,9 @@
 openai==1.14.1
 chromadb==0.4.24
 opentelemetry-api==1.22.0
 opentelemetry-sdk==1.22.0
 opentelemetry-proto==1.22.0
 rich==13.7.1
 pytz==2024.1
-schedule==1.2.1
+bs4==0.0.2
+fake_useragent==1.5.1
```

### Comparing `hspylib-askai-1.0.5/setup.py` & `hspylib_askai-1.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 # -*- coding: utf-8 -*-
 
 """
    @project: HsPyLib-AskAI
       @file: setup.py
    @created: Tue, 2 Jan 2024
     @author: <B>H</B>ugo <B>S</B>aporetti <B>J</B>unior"
-      @site: https://github.com/yorevs/hspylib
+      @site: https://github.com/yorevs/askai
    @license: MIT - Please refer to <https://opensource.org/licenses/MIT>
 
-   Copyright·(c)·2024,·HSPyLib
+   Copyright (c) 2024, HomeSetup
 
    Reference: https://setuptools.pypa.io/en/latest/references/keywords.html
 """
 
 import pathlib
 import setuptools
 
@@ -27,15 +27,15 @@
 
 # The package requirements
 REQUIREMENTS = list(filter(None, (HERE / "requirements.txt").read_text().splitlines()))
 
 # This call to setup() does all the work
 setuptools.setup(
     name="hspylib-askai",
-    version="1.0.5",
+    version="1.0.6",
     description="HomeSetup - AskAI",
     author="Hugo Saporetti Junior",
     author_email="yorevs@hotmail.com",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/yorevs/hspylib",
     project_urls={"GitHub": "https://github.com/yorevs/hspylib", "PyPi": "https://pypi.org/project/hspylib-askai/"},
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

