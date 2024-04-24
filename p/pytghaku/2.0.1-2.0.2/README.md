# Comparing `tmp/pytghaku-2.0.1.tar.gz` & `tmp/pytghaku-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytghaku-2.0.1.tar", last modified: Wed Apr 24 14:03:05 2024, max compression
+gzip compressed data, was "pytghaku-2.0.2.tar", last modified: Wed Apr 24 14:15:33 2024, max compression
```

## Comparing `pytghaku-2.0.1.tar` & `pytghaku-2.0.2.tar`

### file list

```diff
@@ -1,116 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.259826 pytghaku-2.0.1/
--rw-r--r--   0 root         (0) root         (0)     7652 2024-04-24 14:02:44.000000 pytghaku-2.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)    14319 2024-04-24 14:03:05.259826 pytghaku-2.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3812 2024-04-24 14:02:44.000000 pytghaku-2.0.1/README.md
--rw-r--r--   0 root         (0) root         (0)     1632 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.243826 pytghaku-2.0.1/pytghaku/
--rw-r--r--   0 root         (0) root         (0)      247 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/__init__.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.243826 pytghaku-2.0.1/pytghaku/custom_api/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/custom_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1890 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/custom_api/custom_api.py
--rw-r--r--   0 root         (0) root         (0)     1892 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/environment.py
--rw-r--r--   0 root         (0) root         (0)     4093 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8518 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/ffmpeg.py
--rw-r--r--   0 root         (0) root         (0)     4851 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/filters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.247826 pytghaku-2.0.1/pytghaku/handlers/
--rw-r--r--   0 root         (0) root         (0)       75 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/handlers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/handlers/handlers_holder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.247826 pytghaku-2.0.1/pytghaku/media_devices/
--rw-r--r--   0 root         (0) root         (0)      183 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/media_devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)      489 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/media_devices/device_info.py
--rw-r--r--   0 root         (0) root         (0)     3149 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/media_devices/media_devices.py
--rw-r--r--   0 root         (0) root         (0)     1107 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/media_devices/screen_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.247826 pytghaku-2.0.1/pytghaku/methods/
--rw-r--r--   0 root         (0) root         (0)      217 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.247826 pytghaku-2.0.1/pytghaku/methods/calls/
--rw-r--r--   0 root         (0) root         (0)      214 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/calls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      719 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/calls/change_volume_call.py
--rw-r--r--   0 root         (0) root         (0)      567 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/calls/get_participants.py
--rw-r--r--   0 root         (0) root         (0)     1256 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/calls/leave_call.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.247826 pytghaku-2.0.1/pytghaku/methods/decorators/
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/decorators/on_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.247826 pytghaku-2.0.1/pytghaku/methods/stream/
--rw-r--r--   0 root         (0) root         (0)      343 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)      570 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/stream/mute_stream.py
--rw-r--r--   0 root         (0) root         (0)      573 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/stream/pause_stream.py
--rw-r--r--   0 root         (0) root         (0)     7306 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/stream/play.py
--rw-r--r--   0 root         (0) root         (0)      570 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/stream/played_time.py
--rw-r--r--   0 root         (0) root         (0)      576 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/stream/resume_stream.py
--rw-r--r--   0 root         (0) root         (0)      576 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/stream/unmute_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.251826 pytghaku-2.0.1/pytghaku/methods/utilities/
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      140 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/cache_peer.py
--rw-r--r--   0 root         (0) root         (0)      972 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/call_holder.py
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/compose.py
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/cpu_usage.py
--rw-r--r--   0 root         (0) root         (0)      813 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/idle.py
--rw-r--r--   0 root         (0) root         (0)      244 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/ping.py
--rw-r--r--   0 root         (0) root         (0)      382 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/resolve_chat_id.py
--rw-r--r--   0 root         (0) root         (0)      152 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/run.py
--rw-r--r--   0 root         (0) root         (0)     8922 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/start.py
--rw-r--r--   0 root         (0) root         (0)     1519 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/methods/utilities/stream_params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.251826 pytghaku-2.0.1/pytghaku/mtproto/
--rw-r--r--   0 root         (0) root         (0)      130 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mtproto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4975 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mtproto/bridged_client.py
--rw-r--r--   0 root         (0) root         (0)     5086 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mtproto/client_cache.py
--rw-r--r--   0 root         (0) root         (0)    21093 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mtproto/haku_client.py
--rw-r--r--   0 root         (0) root         (0)    21116 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mtproto/hydrogram_client.py
--rw-r--r--   0 root         (0) root         (0)     6867 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mtproto/mtproto_client.py
--rw-r--r--   0 root         (0) root         (0)    20207 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mtproto/telethon_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mtproto_required.py
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/mutex.py
--rw-r--r--   0 root         (0) root         (0)     1479 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/pytghaku.py
--rw-r--r--   0 root         (0) root         (0)     2716 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/pytghaku_session.py
--rw-r--r--   0 root         (0) root         (0)      958 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/scaffold.py
--rw-r--r--   0 root         (0) root         (0)     3842 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/statictypes.py
--rw-r--r--   0 root         (0) root         (0)     3396 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/sync.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.255826 pytghaku-2.0.1/pytghaku/types/
--rw-r--r--   0 root         (0) root         (0)      910 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9545 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/browsers.py
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/cache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.255826 pytghaku-2.0.1/pytghaku/types/calls/
--rw-r--r--   0 root         (0) root         (0)      346 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/calls/__init__.py
--rw-r--r--   0 root         (0) root         (0)      725 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/calls/call.py
--rw-r--r--   0 root         (0) root         (0)      120 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/calls/call_config.py
--rw-r--r--   0 root         (0) root         (0)      544 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/calls/call_data.py
--rw-r--r--   0 root         (0) root         (0)      408 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/calls/call_protocol.py
--rw-r--r--   0 root         (0) root         (0)      353 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/calls/group_call_config.py
--rw-r--r--   0 root         (0) root         (0)      794 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/calls/raw_call_update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.255826 pytghaku-2.0.1/pytghaku/types/chats/
--rw-r--r--   0 root         (0) root         (0)      261 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/chats/__init__.py
--rw-r--r--   0 root         (0) root         (0)      738 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/chats/chat_update.py
--rw-r--r--   0 root         (0) root         (0)     1018 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/chats/group_call_participant.py
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/chats/updated_group_call_participant.py
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/dict.py
--rw-r--r--   0 root         (0) root         (0)       78 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/list.py
--rw-r--r--   0 root         (0) root         (0)      916 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/participant_list.py
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/py_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.255826 pytghaku-2.0.1/pytghaku/types/raw/
--rw-r--r--   0 root         (0) root         (0)      308 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/raw/__init__.py
--rw-r--r--   0 root         (0) root         (0)      449 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/raw/audio_parameters.py
--rw-r--r--   0 root         (0) root         (0)      476 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/raw/audio_stream.py
--rw-r--r--   0 root         (0) root         (0)      491 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/raw/stream.py
--rw-r--r--   0 root         (0) root         (0)      545 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/raw/video_parameters.py
--rw-r--r--   0 root         (0) root         (0)      433 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/raw/video_stream.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.259826 pytghaku-2.0.1/pytghaku/types/stream/
--rw-r--r--   0 root         (0) root         (0)      338 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/stream/__init__.py
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/stream/audio_quality.py
--rw-r--r--   0 root         (0) root         (0)     8979 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/stream/media_stream.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/stream/stream_audio_ended.py
--rw-r--r--   0 root         (0) root         (0)      164 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/stream/stream_video_ended.py
--rw-r--r--   0 root         (0) root         (0)      231 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/stream/video_quality.py
--rw-r--r--   0 root         (0) root         (0)      157 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/update.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/types/user_agent.py
--rw-r--r--   0 root         (0) root         (0)      296 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/version_manager.py
--rw-r--r--   0 root         (0) root         (0)     2196 2024-04-24 14:02:44.000000 pytghaku-2.0.1/pytghaku/ytdlp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:03:05.259826 pytghaku-2.0.1/pytghaku.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14319 2024-04-24 14:03:05.000000 pytghaku-2.0.1/pytghaku.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3166 2024-04-24 14:03:05.000000 pytghaku-2.0.1/pytghaku.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 14:03:05.000000 pytghaku-2.0.1/pytghaku.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 14:03:05.000000 pytghaku-2.0.1/pytghaku.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      138 2024-04-24 14:03:05.000000 pytghaku-2.0.1/pytghaku.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-24 14:03:05.000000 pytghaku-2.0.1/pytghaku.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 14:03:05.259826 pytghaku-2.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      375 2024-04-24 14:02:44.000000 pytghaku-2.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.663040 pytghaku-2.0.2/
+-rw-r--r--   0 root         (0) root         (0)     7652 2024-04-24 14:15:07.000000 pytghaku-2.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    14319 2024-04-24 14:15:33.663040 pytghaku-2.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3812 2024-04-24 14:15:07.000000 pytghaku-2.0.2/README.md
+-rw-r--r--   0 root         (0) root         (0)     1632 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.643041 pytghaku-2.0.2/pytghaku/
+-rw-r--r--   0 root         (0) root         (0)      247 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.647041 pytghaku-2.0.2/pytghaku/custom_api/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/custom_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1890 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/custom_api/custom_api.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/environment.py
+-rw-r--r--   0 root         (0) root         (0)     4093 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8518 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/ffmpeg.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/filters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.647041 pytghaku-2.0.2/pytghaku/handlers/
+-rw-r--r--   0 root         (0) root         (0)       75 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/handlers/handlers_holder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.647041 pytghaku-2.0.2/pytghaku/media_devices/
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/media_devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      489 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/media_devices/device_info.py
+-rw-r--r--   0 root         (0) root         (0)     3149 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/media_devices/media_devices.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/media_devices/screen_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.647041 pytghaku-2.0.2/pytghaku/methods/
+-rw-r--r--   0 root         (0) root         (0)      217 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.651041 pytghaku-2.0.2/pytghaku/methods/calls/
+-rw-r--r--   0 root         (0) root         (0)      214 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/calls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      719 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/calls/change_volume_call.py
+-rw-r--r--   0 root         (0) root         (0)      567 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/calls/get_participants.py
+-rw-r--r--   0 root         (0) root         (0)     1256 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/calls/leave_call.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.651041 pytghaku-2.0.2/pytghaku/methods/decorators/
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      316 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/decorators/on_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.651041 pytghaku-2.0.2/pytghaku/methods/stream/
+-rw-r--r--   0 root         (0) root         (0)      343 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      570 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/stream/mute_stream.py
+-rw-r--r--   0 root         (0) root         (0)      573 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/stream/pause_stream.py
+-rw-r--r--   0 root         (0) root         (0)     7306 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/stream/play.py
+-rw-r--r--   0 root         (0) root         (0)      570 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/stream/played_time.py
+-rw-r--r--   0 root         (0) root         (0)      576 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/stream/resume_stream.py
+-rw-r--r--   0 root         (0) root         (0)      576 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/stream/unmute_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.655041 pytghaku-2.0.2/pytghaku/methods/utilities/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      140 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/cache_peer.py
+-rw-r--r--   0 root         (0) root         (0)      972 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/call_holder.py
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/compose.py
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/cpu_usage.py
+-rw-r--r--   0 root         (0) root         (0)      813 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/idle.py
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/ping.py
+-rw-r--r--   0 root         (0) root         (0)      382 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/resolve_chat_id.py
+-rw-r--r--   0 root         (0) root         (0)      152 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/run.py
+-rw-r--r--   0 root         (0) root         (0)     8922 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/start.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/methods/utilities/stream_params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.655041 pytghaku-2.0.2/pytghaku/mtproto/
+-rw-r--r--   0 root         (0) root         (0)      130 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mtproto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mtproto/bridged_client.py
+-rw-r--r--   0 root         (0) root         (0)     5086 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mtproto/client_cache.py
+-rw-r--r--   0 root         (0) root         (0)    21093 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mtproto/haku_client.py
+-rw-r--r--   0 root         (0) root         (0)    21116 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mtproto/hydrogram_client.py
+-rw-r--r--   0 root         (0) root         (0)     6867 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mtproto/mtproto_client.py
+-rw-r--r--   0 root         (0) root         (0)    20207 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mtproto/telethon_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mtproto_required.py
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/mutex.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/pytghaku.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/pytghaku_session.py
+-rw-r--r--   0 root         (0) root         (0)      955 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/scaffold.py
+-rw-r--r--   0 root         (0) root         (0)     3842 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/statictypes.py
+-rw-r--r--   0 root         (0) root         (0)     3396 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/sync.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.655041 pytghaku-2.0.2/pytghaku/types/
+-rw-r--r--   0 root         (0) root         (0)      910 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9545 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/browsers.py
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/cache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.659041 pytghaku-2.0.2/pytghaku/types/calls/
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/calls/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      725 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/calls/call.py
+-rw-r--r--   0 root         (0) root         (0)      120 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/calls/call_config.py
+-rw-r--r--   0 root         (0) root         (0)      544 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/calls/call_data.py
+-rw-r--r--   0 root         (0) root         (0)      408 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/calls/call_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      353 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/calls/group_call_config.py
+-rw-r--r--   0 root         (0) root         (0)      794 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/calls/raw_call_update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.659041 pytghaku-2.0.2/pytghaku/types/chats/
+-rw-r--r--   0 root         (0) root         (0)      261 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/chats/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      738 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/chats/chat_update.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/chats/group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)      291 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/chats/updated_group_call_participant.py
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/dict.py
+-rw-r--r--   0 root         (0) root         (0)       78 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/list.py
+-rw-r--r--   0 root         (0) root         (0)      916 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/participant_list.py
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/py_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.659041 pytghaku-2.0.2/pytghaku/types/raw/
+-rw-r--r--   0 root         (0) root         (0)      308 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/raw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      449 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/raw/audio_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/raw/audio_stream.py
+-rw-r--r--   0 root         (0) root         (0)      491 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/raw/stream.py
+-rw-r--r--   0 root         (0) root         (0)      545 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/raw/video_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      433 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/raw/video_stream.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.659041 pytghaku-2.0.2/pytghaku/types/stream/
+-rw-r--r--   0 root         (0) root         (0)      338 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/stream/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/stream/audio_quality.py
+-rw-r--r--   0 root         (0) root         (0)     8979 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/stream/media_stream.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/stream/stream_audio_ended.py
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/stream/stream_video_ended.py
+-rw-r--r--   0 root         (0) root         (0)      231 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/stream/video_quality.py
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/update.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/types/user_agent.py
+-rw-r--r--   0 root         (0) root         (0)      296 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/version_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2196 2024-04-24 14:15:07.000000 pytghaku-2.0.2/pytghaku/ytdlp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 14:15:33.659041 pytghaku-2.0.2/pytghaku.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14319 2024-04-24 14:15:33.000000 pytghaku-2.0.2/pytghaku.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3166 2024-04-24 14:15:33.000000 pytghaku-2.0.2/pytghaku.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 14:15:33.000000 pytghaku-2.0.2/pytghaku.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 14:15:33.000000 pytghaku-2.0.2/pytghaku.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-24 14:15:33.000000 pytghaku-2.0.2/pytghaku.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-24 14:15:33.000000 pytghaku-2.0.2/pytghaku.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-24 14:15:33.663040 pytghaku-2.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      375 2024-04-24 14:15:07.000000 pytghaku-2.0.2/setup.py
```

### Comparing `pytghaku-2.0.1/LICENSE` & `pytghaku-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/PKG-INFO` & `pytghaku-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytghaku
-Version: 2.0.1
+Version: 2.0.2
 Summary: Async client API for the Telegram Calls.
 Author-email: RizalDevs <rizaldaitona@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pytghaku-2.0.1/README.md` & `pytghaku-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pyproject.toml` & `pytghaku-2.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/custom_api/custom_api.py` & `pytghaku-2.0.2/pytghaku/custom_api/custom_api.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/environment.py` & `pytghaku-2.0.2/pytghaku/environment.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/exceptions.py` & `pytghaku-2.0.2/pytghaku/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/ffmpeg.py` & `pytghaku-2.0.2/pytghaku/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/filters.py` & `pytghaku-2.0.2/pytghaku/filters.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/handlers/handlers_holder.py` & `pytghaku-2.0.2/pytghaku/handlers/handlers_holder.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/media_devices/media_devices.py` & `pytghaku-2.0.2/pytghaku/media_devices/media_devices.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/media_devices/screen_info.py` & `pytghaku-2.0.2/pytghaku/media_devices/screen_info.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/calls/change_volume_call.py` & `pytghaku-2.0.2/pytghaku/methods/calls/change_volume_call.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/calls/get_participants.py` & `pytghaku-2.0.2/pytghaku/methods/calls/get_participants.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/calls/leave_call.py` & `pytghaku-2.0.2/pytghaku/methods/calls/leave_call.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/stream/mute_stream.py` & `pytghaku-2.0.2/pytghaku/methods/stream/mute_stream.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/stream/pause_stream.py` & `pytghaku-2.0.2/pytghaku/methods/stream/pause_stream.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/stream/play.py` & `pytghaku-2.0.2/pytghaku/methods/stream/play.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/stream/played_time.py` & `pytghaku-2.0.2/pytghaku/methods/stream/played_time.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/stream/resume_stream.py` & `pytghaku-2.0.2/pytghaku/methods/stream/resume_stream.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/stream/unmute_stream.py` & `pytghaku-2.0.2/pytghaku/methods/stream/unmute_stream.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/utilities/call_holder.py` & `pytghaku-2.0.2/pytghaku/methods/utilities/call_holder.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/utilities/idle.py` & `pytghaku-2.0.2/pytghaku/methods/utilities/idle.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/utilities/start.py` & `pytghaku-2.0.2/pytghaku/methods/utilities/start.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/methods/utilities/stream_params.py` & `pytghaku-2.0.2/pytghaku/methods/utilities/stream_params.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/mtproto/bridged_client.py` & `pytghaku-2.0.2/pytghaku/mtproto/bridged_client.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/mtproto/client_cache.py` & `pytghaku-2.0.2/pytghaku/mtproto/client_cache.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/mtproto/haku_client.py` & `pytghaku-2.0.2/pytghaku/mtproto/haku_client.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/mtproto/hydrogram_client.py` & `pytghaku-2.0.2/pytghaku/mtproto/hydrogram_client.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/mtproto/mtproto_client.py` & `pytghaku-2.0.2/pytghaku/mtproto/mtproto_client.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/mtproto/telethon_client.py` & `pytghaku-2.0.2/pytghaku/mtproto/telethon_client.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/mtproto_required.py` & `pytghaku-2.0.2/pytghaku/mtproto_required.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/pytghaku.py` & `pytghaku-2.0.2/pytghaku/pytghaku.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/pytghaku_session.py` & `pytghaku-2.0.2/pytghaku/pytghaku_session.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/scaffold.py` & `pytghaku-2.0.2/pytghaku/scaffold.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Union
 
 from .handlers import HandlersHolder
 
 
 class Scaffold(HandlersHolder):
-    _REQUIRED_PYROGRAM_VERSION = '1.2.20'
+    _REQUIRED_PYROGRAM_VERSION = '1.0'
     _REQUIRED_TELETHON_VERSION = '1.24.0'
     _REQUIRED_HYDROGRAM_VERSION = '0.1.4'
 
     def __init__(self):
         super().__init__()
         self._app = None
         self._is_running = None
```

### Comparing `pytghaku-2.0.1/pytghaku/statictypes.py` & `pytghaku-2.0.2/pytghaku/statictypes.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/sync.py` & `pytghaku-2.0.2/pytghaku/sync.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/__init__.py` & `pytghaku-2.0.2/pytghaku/types/__init__.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/browsers.py` & `pytghaku-2.0.2/pytghaku/types/browsers.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/cache.py` & `pytghaku-2.0.2/pytghaku/types/cache.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/calls/call.py` & `pytghaku-2.0.2/pytghaku/types/calls/call.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/calls/call_data.py` & `pytghaku-2.0.2/pytghaku/types/calls/call_data.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/calls/raw_call_update.py` & `pytghaku-2.0.2/pytghaku/types/calls/raw_call_update.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/chats/chat_update.py` & `pytghaku-2.0.2/pytghaku/types/chats/chat_update.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/chats/group_call_participant.py` & `pytghaku-2.0.2/pytghaku/types/chats/group_call_participant.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/participant_list.py` & `pytghaku-2.0.2/pytghaku/types/participant_list.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/py_object.py` & `pytghaku-2.0.2/pytghaku/types/py_object.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/raw/video_parameters.py` & `pytghaku-2.0.2/pytghaku/types/raw/video_parameters.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/stream/media_stream.py` & `pytghaku-2.0.2/pytghaku/types/stream/media_stream.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/types/user_agent.py` & `pytghaku-2.0.2/pytghaku/types/user_agent.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku/ytdlp.py` & `pytghaku-2.0.2/pytghaku/ytdlp.py`

 * *Files identical despite different names*

### Comparing `pytghaku-2.0.1/pytghaku.egg-info/PKG-INFO` & `pytghaku-2.0.2/pytghaku.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytghaku
-Version: 2.0.1
+Version: 2.0.2
 Summary: Async client API for the Telegram Calls.
 Author-email: RizalDevs <rizaldaitona@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `pytghaku-2.0.1/pytghaku.egg-info/SOURCES.txt` & `pytghaku-2.0.2/pytghaku.egg-info/SOURCES.txt`

 * *Files identical despite different names*

