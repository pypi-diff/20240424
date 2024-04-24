# Comparing `tmp/animdl2-1.7.28.tar.gz` & `tmp/animdl2-1.7.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "animdl2-1.7.28.tar", max compression
+gzip compressed data, was "animdl2-1.7.29.tar", max compression
```

## Comparing `animdl2-1.7.28.tar` & `animdl2-1.7.29.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0       21 2024-04-24 12:29:07.294592 animdl2-1.7.28/animdl2/__init__.py
--rw-r--r--   0        0        0     3303 2024-04-24 12:44:41.420214 animdl2-1.7.28/animdl2/__main__.py
--rw-r--r--   0        0        0       74 2024-04-24 12:29:07.296592 animdl2-1.7.28/animdl2/core/__init__.py
--rw-r--r--   0        0        0      385 2024-04-24 12:44:41.306688 animdl2-1.7.28/animdl2/core/__version__.py
--rw-r--r--   0        0        0        0 2024-04-24 12:29:07.298592 animdl2-1.7.28/animdl2/core/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 12:29:07.299590 animdl2-1.7.28/animdl2/core/cli/commands/__init__.py
--rw-r--r--   0        0        0     5036 2024-04-24 12:29:07.300594 animdl2-1.7.28/animdl2/core/cli/commands/download.py
--rw-r--r--   0        0        0     1388 2024-04-24 12:29:07.300594 animdl2-1.7.28/animdl2/core/cli/commands/grab.py
--rw-r--r--   0        0        0     3391 2024-04-24 12:29:07.301592 animdl2-1.7.28/animdl2/core/cli/commands/schedule.py
--rw-r--r--   0        0        0     1702 2024-04-24 12:29:07.302591 animdl2-1.7.28/animdl2/core/cli/commands/search.py
--rw-r--r--   0        0        0     8942 2024-04-24 12:29:07.302591 animdl2-1.7.28/animdl2/core/cli/commands/stream.py
--rw-r--r--   0        0        0     3432 2024-04-24 12:29:07.303592 animdl2-1.7.28/animdl2/core/cli/commands/update.py
--rw-r--r--   0        0        0      120 2024-04-24 12:29:07.304593 animdl2-1.7.28/animdl2/core/cli/exit_codes.py
--rw-r--r--   0        0        0     4955 2024-04-24 12:29:07.305590 animdl2-1.7.28/animdl2/core/cli/helpers/__init__.py
--rw-r--r--   0        0        0     1836 2024-04-24 12:29:07.306594 animdl2-1.7.28/animdl2/core/cli/helpers/aniskip.py
--rw-r--r--   0        0        0     2394 2024-04-24 12:29:07.306594 animdl2-1.7.28/animdl2/core/cli/helpers/banner.py
--rw-r--r--   0        0        0      259 2024-04-24 12:29:07.306594 animdl2-1.7.28/animdl2/core/cli/helpers/constants.py
--rw-r--r--   0        0        0     4428 2024-04-24 12:29:07.308099 animdl2-1.7.28/animdl2/core/cli/helpers/decorators.py
--rw-r--r--   0        0        0     1132 2024-04-24 12:29:07.309108 animdl2-1.7.28/animdl2/core/cli/helpers/fuzzysearch.py
--rw-r--r--   0        0        0     9983 2024-04-24 12:44:41.389686 animdl2-1.7.28/animdl2/core/cli/helpers/intelliq.py
--rw-r--r--   0        0        0     2672 2024-04-24 12:29:07.310108 animdl2-1.7.28/animdl2/core/cli/helpers/logger.py
--rw-r--r--   0        0        0     1624 2024-04-24 12:29:07.311109 animdl2-1.7.28/animdl2/core/cli/helpers/player.py
--rw-r--r--   0        0        0      356 2024-04-24 12:29:07.312112 animdl2-1.7.28/animdl2/core/cli/helpers/players/__init__.py
--rw-r--r--   0        0        0      789 2024-04-24 12:29:07.312112 animdl2-1.7.28/animdl2/core/cli/helpers/players/android.py
--rw-r--r--   0        0        0     2171 2024-04-24 12:29:07.313113 animdl2-1.7.28/animdl2/core/cli/helpers/players/base_player.py
--rw-r--r--   0        0        0      751 2024-04-24 12:29:07.314108 animdl2-1.7.28/animdl2/core/cli/helpers/players/ffplay.py
--rw-r--r--   0        0        0     2847 2024-04-24 12:29:07.314108 animdl2-1.7.28/animdl2/core/cli/helpers/players/mpv.py
--rw-r--r--   0        0        0     1813 2024-04-24 12:29:07.315107 animdl2-1.7.28/animdl2/core/cli/helpers/players/vlc.py
--rw-r--r--   0        0        0     1524 2024-04-24 12:29:07.316110 animdl2-1.7.28/animdl2/core/cli/helpers/processors.py
--rw-r--r--   0        0        0     5289 2024-04-24 12:29:07.317105 animdl2-1.7.28/animdl2/core/cli/helpers/prompts.py
--rw-r--r--   0        0        0     3140 2024-04-24 12:29:07.318107 animdl2-1.7.28/animdl2/core/cli/helpers/rpc.py
--rw-r--r--   0        0        0     7053 2024-04-24 12:44:41.430213 animdl2-1.7.28/animdl2/core/cli/helpers/searcher.py
--rw-r--r--   0        0        0     1050 2024-04-24 12:29:07.319108 animdl2-1.7.28/animdl2/core/cli/helpers/special.py
--rw-r--r--   0        0        0     2076 2024-04-24 12:29:07.320109 animdl2-1.7.28/animdl2/core/cli/helpers/stream_handlers.py
--rw-r--r--   0        0        0      575 2024-04-24 12:44:41.316687 animdl2-1.7.28/animdl2/core/cli/http_client.py
--rw-r--r--   0        0        0       27 2024-04-24 12:29:07.321107 animdl2-1.7.28/animdl2/core/codebase/__init__.py
--rw-r--r--   0        0        0       56 2024-04-24 12:29:07.323108 animdl2-1.7.28/animdl2/core/codebase/downloader/__init__.py
--rw-r--r--   0        0        0     7636 2024-04-24 12:29:07.324108 animdl2-1.7.28/animdl2/core/codebase/downloader/ffmpeg.py
--rw-r--r--   0        0        0    12181 2024-04-24 12:44:41.368686 animdl2-1.7.28/animdl2/core/codebase/downloader/handle.py
--rw-r--r--   0        0        0     4995 2024-04-24 12:29:07.325108 animdl2-1.7.28/animdl2/core/codebase/downloader/hls.py
--rw-r--r--   0        0        0     2089 2024-04-24 12:29:07.326107 animdl2-1.7.28/animdl2/core/codebase/downloader/idmanlib.py
--rw-r--r--   0        0        0      451 2024-04-24 12:29:07.326107 animdl2-1.7.28/animdl2/core/codebase/extractors/__init__.py
--rw-r--r--   0        0        0     1425 2024-04-24 12:29:07.328109 animdl2-1.7.28/animdl2/core/codebase/extractors/dailymotion/__init__.py
--rw-r--r--   0        0        0      904 2024-04-24 12:29:07.329108 animdl2-1.7.28/animdl2/core/codebase/extractors/doodstream/__init__.py
--rw-r--r--   0        0        0     2230 2024-04-24 12:29:07.330107 animdl2-1.7.28/animdl2/core/codebase/extractors/gogoplay/__init__.py
--rw-r--r--   0        0        0     1131 2024-04-24 12:29:07.331110 animdl2-1.7.28/animdl2/core/codebase/extractors/mp4upload/__init__.py
--rw-r--r--   0        0        0       33 2024-04-24 12:29:07.332109 animdl2-1.7.28/animdl2/core/codebase/extractors/mycloud/__init__.py
--rw-r--r--   0        0        0     1030 2024-04-24 12:29:07.333108 animdl2-1.7.28/animdl2/core/codebase/extractors/okru/__init__.py
--rw-r--r--   0        0        0     1228 2024-04-24 12:29:07.334107 animdl2-1.7.28/animdl2/core/codebase/extractors/rapidvideo/__init__.py
--rw-r--r--   0        0        0     2202 2024-04-24 12:29:07.335110 animdl2-1.7.28/animdl2/core/codebase/extractors/rapidvideo/polling.py
--rw-r--r--   0        0        0     1111 2024-04-24 12:29:07.335110 animdl2-1.7.28/animdl2/core/codebase/extractors/rapidvideo/utils.py
--rw-r--r--   0        0        0      933 2024-04-24 12:29:07.337109 animdl2-1.7.28/animdl2/core/codebase/extractors/streamlare/__init__.py
--rw-r--r--   0        0        0     1133 2024-04-24 12:29:07.338114 animdl2-1.7.28/animdl2/core/codebase/extractors/streamsb/__init__.py
--rw-r--r--   0        0        0      937 2024-04-24 12:29:07.340110 animdl2-1.7.28/animdl2/core/codebase/extractors/streamtape/__init__.py
--rw-r--r--   0        0        0      391 2024-04-24 12:29:07.341112 animdl2-1.7.28/animdl2/core/codebase/extractors/videobin/__init__.py
--rw-r--r--   0        0        0      909 2024-04-24 12:29:07.343107 animdl2-1.7.28/animdl2/core/codebase/extractors/vidstream/__init__.py
--rw-r--r--   0        0        0     1957 2024-04-24 12:44:41.377688 animdl2-1.7.28/animdl2/core/codebase/helpers/__init__.py
--rw-r--r--   0        0        0     2119 2024-04-24 12:44:41.347689 animdl2-1.7.28/animdl2/core/codebase/helpers/superscrapers.py
--rw-r--r--   0        0        0     2681 2024-04-24 12:29:07.345110 animdl2-1.7.28/animdl2/core/codebase/helpers/uwu.py
--rw-r--r--   0        0        0     1070 2024-04-24 12:29:07.347109 animdl2-1.7.28/animdl2/core/codebase/providers/__init__.py
--rw-r--r--   0        0        0     6396 2024-04-24 12:29:07.348111 animdl2-1.7.28/animdl2/core/codebase/providers/allanime/__init__.py
--rw-r--r--   0        0        0     5594 2024-04-24 12:44:41.337690 animdl2-1.7.28/animdl2/core/codebase/providers/allanime/gql_api.py
--rw-r--r--   0        0        0     2403 2024-04-24 12:29:07.350108 animdl2-1.7.28/animdl2/core/codebase/providers/animekaizoku/__init__.py
--rw-r--r--   0        0        0     2484 2024-04-24 12:29:07.352109 animdl2-1.7.28/animdl2/core/codebase/providers/animeonsen/__init__.py
--rw-r--r--   0        0        0     1808 2024-04-24 12:29:07.353109 animdl2-1.7.28/animdl2/core/codebase/providers/animeout/__init__.py
--rw-r--r--   0        0        0     2841 2024-04-24 12:44:41.326691 animdl2-1.7.28/animdl2/core/codebase/providers/animepahe/__init__.py
--rw-r--r--   0        0        0     1824 2024-04-24 12:29:07.356110 animdl2-1.7.28/animdl2/core/codebase/providers/animepahe/inner/__init__.py
--rw-r--r--   0        0        0     1047 2024-04-24 12:29:07.357109 animdl2-1.7.28/animdl2/core/codebase/providers/animepahe/inner/archive.py
--rw-r--r--   0        0        0     2921 2024-04-24 12:29:07.358108 animdl2-1.7.28/animdl2/core/codebase/providers/animexin/__init__.py
--rw-r--r--   0        0        0      407 2024-04-24 12:29:07.360107 animdl2-1.7.28/animdl2/core/codebase/providers/animixplay/__init__.py
--rw-r--r--   0        0        0     1241 2024-04-24 12:29:07.360107 animdl2-1.7.28/animdl2/core/codebase/providers/animixplay/hardstream.py
--rw-r--r--   0        0        0     2847 2024-04-24 12:29:07.361108 animdl2-1.7.28/animdl2/core/codebase/providers/animixplay/stream_url.py
--rw-r--r--   0        0        0     1913 2024-04-24 12:44:41.357687 animdl2-1.7.28/animdl2/core/codebase/providers/animtime/__init__.py
--rw-r--r--   0        0        0     2959 2024-04-24 12:29:07.364107 animdl2-1.7.28/animdl2/core/codebase/providers/crunchyroll/__init__.py
--rw-r--r--   0        0        0     2336 2024-04-24 12:29:07.365107 animdl2-1.7.28/animdl2/core/codebase/providers/gogoanime/__init__.py
--rw-r--r--   0        0        0     1568 2024-04-24 12:29:07.366109 animdl2-1.7.28/animdl2/core/codebase/providers/hahomoe/__init__.py
--rw-r--r--   0        0        0     2315 2024-04-24 12:29:07.367110 animdl2-1.7.28/animdl2/core/codebase/providers/hentaistream/__init__.py
--rw-r--r--   0        0        0     2920 2024-04-24 12:29:07.368107 animdl2-1.7.28/animdl2/core/codebase/providers/kamyroll/__init__.py
--rw-r--r--   0        0        0     2993 2024-04-24 12:29:07.369108 animdl2-1.7.28/animdl2/core/codebase/providers/kamyroll/api.py
--rw-r--r--   0        0        0     1879 2024-04-24 12:29:07.371113 animdl2-1.7.28/animdl2/core/codebase/providers/kawaiifu/__init__.py
--rw-r--r--   0        0        0     2407 2024-04-24 12:44:41.399697 animdl2-1.7.28/animdl2/core/codebase/providers/marinmoe/__init__.py
--rw-r--r--   0        0        0     2647 2024-04-24 12:29:07.373108 animdl2-1.7.28/animdl2/core/codebase/providers/nineanime/__init__.py
--rw-r--r--   0        0        0     1759 2024-04-24 12:29:07.374107 animdl2-1.7.28/animdl2/core/codebase/providers/nineanime/decipher.py
--rw-r--r--   0        0        0     1303 2024-04-24 12:29:07.375108 animdl2-1.7.28/animdl2/core/codebase/providers/twistmoe/__init__.py
--rw-r--r--   0        0        0     1672 2024-04-24 12:29:07.376108 animdl2-1.7.28/animdl2/core/codebase/providers/twistmoe/stream_url.py
--rw-r--r--   0        0        0     1967 2024-04-24 12:29:07.377107 animdl2-1.7.28/animdl2/core/codebase/providers/yugen/__init__.py
--rw-r--r--   0        0        0     2630 2024-04-24 12:29:07.378108 animdl2-1.7.28/animdl2/core/codebase/providers/zoro/__init__.py
--rw-r--r--   0        0        0     6369 2024-04-24 12:29:07.379109 animdl2-1.7.28/animdl2/core/config/__init__.py
--rw-r--r--   0        0        0     4453 2024-04-24 12:29:07.380108 animdl2-1.7.28/animdl2/core/package_resolver.py
--rw-r--r--   0        0        0      293 2024-04-24 12:29:07.381108 animdl2-1.7.28/animdl2/utils/__init__.py
--rw-r--r--   0        0        0     7529 2024-04-24 12:44:41.409217 animdl2-1.7.28/animdl2/utils/http_caching.py
--rw-r--r--   0        0        0     4093 2024-04-24 12:44:41.439217 animdl2-1.7.28/animdl2/utils/http_client.py
--rw-r--r--   0        0        0     6248 2024-04-24 12:29:07.384107 animdl2-1.7.28/animdl2/utils/media_downloader.py
--rw-r--r--   0        0        0      416 2024-04-24 12:29:07.385108 animdl2-1.7.28/animdl2/utils/optopt.py
--rw-r--r--   0        0        0     1979 2024-04-24 12:29:07.385108 animdl2-1.7.28/animdl2/utils/powertools.py
--rw-r--r--   0        0        0     1837 2024-04-24 12:29:07.386108 animdl2-1.7.28/animdl2/utils/searching.py
--rw-r--r--   0        0        0     1089 2024-04-24 12:29:07.387108 animdl2-1.7.28/animdl2/utils/serverfiles.py
--rw-r--r--   0        0        0    35823 2024-04-24 12:29:07.293631 animdl2-1.7.28/LICENSE
--rw-r--r--   0        0        0     1008 2024-04-24 12:45:18.905820 animdl2-1.7.28/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-24 12:29:07.419628 animdl2-1.7.28/readme.txt
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 animdl2-1.7.28/PKG-INFO
+-rw-r--r--   0        0        0       21 2024-04-24 12:29:07.294592 animdl2-1.7.29/animdl2/__init__.py
+-rw-r--r--   0        0        0     3303 2024-04-24 12:44:41.420214 animdl2-1.7.29/animdl2/__main__.py
+-rw-r--r--   0        0        0       74 2024-04-24 12:29:07.296592 animdl2-1.7.29/animdl2/core/__init__.py
+-rw-r--r--   0        0        0      385 2024-04-24 12:44:41.306688 animdl2-1.7.29/animdl2/core/__version__.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:29:07.298592 animdl2-1.7.29/animdl2/core/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 12:29:07.299590 animdl2-1.7.29/animdl2/core/cli/commands/__init__.py
+-rw-r--r--   0        0        0     5036 2024-04-24 12:29:07.300594 animdl2-1.7.29/animdl2/core/cli/commands/download.py
+-rw-r--r--   0        0        0     1388 2024-04-24 12:29:07.300594 animdl2-1.7.29/animdl2/core/cli/commands/grab.py
+-rw-r--r--   0        0        0     3391 2024-04-24 12:29:07.301592 animdl2-1.7.29/animdl2/core/cli/commands/schedule.py
+-rw-r--r--   0        0        0     1702 2024-04-24 12:29:07.302591 animdl2-1.7.29/animdl2/core/cli/commands/search.py
+-rw-r--r--   0        0        0     8942 2024-04-24 12:29:07.302591 animdl2-1.7.29/animdl2/core/cli/commands/stream.py
+-rw-r--r--   0        0        0     3432 2024-04-24 12:29:07.303592 animdl2-1.7.29/animdl2/core/cli/commands/update.py
+-rw-r--r--   0        0        0      120 2024-04-24 12:29:07.304593 animdl2-1.7.29/animdl2/core/cli/exit_codes.py
+-rw-r--r--   0        0        0     4955 2024-04-24 12:29:07.305590 animdl2-1.7.29/animdl2/core/cli/helpers/__init__.py
+-rw-r--r--   0        0        0     1836 2024-04-24 12:29:07.306594 animdl2-1.7.29/animdl2/core/cli/helpers/aniskip.py
+-rw-r--r--   0        0        0     2394 2024-04-24 12:29:07.306594 animdl2-1.7.29/animdl2/core/cli/helpers/banner.py
+-rw-r--r--   0        0        0      259 2024-04-24 12:29:07.306594 animdl2-1.7.29/animdl2/core/cli/helpers/constants.py
+-rw-r--r--   0        0        0     4428 2024-04-24 12:29:07.308099 animdl2-1.7.29/animdl2/core/cli/helpers/decorators.py
+-rw-r--r--   0        0        0     1132 2024-04-24 12:29:07.309108 animdl2-1.7.29/animdl2/core/cli/helpers/fuzzysearch.py
+-rw-r--r--   0        0        0     9983 2024-04-24 12:44:41.389686 animdl2-1.7.29/animdl2/core/cli/helpers/intelliq.py
+-rw-r--r--   0        0        0     2672 2024-04-24 12:29:07.310108 animdl2-1.7.29/animdl2/core/cli/helpers/logger.py
+-rw-r--r--   0        0        0     1624 2024-04-24 12:29:07.311109 animdl2-1.7.29/animdl2/core/cli/helpers/player.py
+-rw-r--r--   0        0        0      356 2024-04-24 12:29:07.312112 animdl2-1.7.29/animdl2/core/cli/helpers/players/__init__.py
+-rw-r--r--   0        0        0      789 2024-04-24 12:29:07.312112 animdl2-1.7.29/animdl2/core/cli/helpers/players/android.py
+-rw-r--r--   0        0        0     2171 2024-04-24 12:29:07.313113 animdl2-1.7.29/animdl2/core/cli/helpers/players/base_player.py
+-rw-r--r--   0        0        0      751 2024-04-24 12:29:07.314108 animdl2-1.7.29/animdl2/core/cli/helpers/players/ffplay.py
+-rw-r--r--   0        0        0     2847 2024-04-24 12:29:07.314108 animdl2-1.7.29/animdl2/core/cli/helpers/players/mpv.py
+-rw-r--r--   0        0        0     1813 2024-04-24 12:29:07.315107 animdl2-1.7.29/animdl2/core/cli/helpers/players/vlc.py
+-rw-r--r--   0        0        0     1524 2024-04-24 12:29:07.316110 animdl2-1.7.29/animdl2/core/cli/helpers/processors.py
+-rw-r--r--   0        0        0     5289 2024-04-24 12:29:07.317105 animdl2-1.7.29/animdl2/core/cli/helpers/prompts.py
+-rw-r--r--   0        0        0     3140 2024-04-24 12:29:07.318107 animdl2-1.7.29/animdl2/core/cli/helpers/rpc.py
+-rw-r--r--   0        0        0     7053 2024-04-24 12:44:41.430213 animdl2-1.7.29/animdl2/core/cli/helpers/searcher.py
+-rw-r--r--   0        0        0     1050 2024-04-24 12:29:07.319108 animdl2-1.7.29/animdl2/core/cli/helpers/special.py
+-rw-r--r--   0        0        0     2076 2024-04-24 12:29:07.320109 animdl2-1.7.29/animdl2/core/cli/helpers/stream_handlers.py
+-rw-r--r--   0        0        0      575 2024-04-24 12:44:41.316687 animdl2-1.7.29/animdl2/core/cli/http_client.py
+-rw-r--r--   0        0        0       27 2024-04-24 12:29:07.321107 animdl2-1.7.29/animdl2/core/codebase/__init__.py
+-rw-r--r--   0        0        0       56 2024-04-24 12:29:07.323108 animdl2-1.7.29/animdl2/core/codebase/downloader/__init__.py
+-rw-r--r--   0        0        0     7636 2024-04-24 12:29:07.324108 animdl2-1.7.29/animdl2/core/codebase/downloader/ffmpeg.py
+-rw-r--r--   0        0        0    12181 2024-04-24 12:44:41.368686 animdl2-1.7.29/animdl2/core/codebase/downloader/handle.py
+-rw-r--r--   0        0        0     4995 2024-04-24 12:29:07.325108 animdl2-1.7.29/animdl2/core/codebase/downloader/hls.py
+-rw-r--r--   0        0        0     2089 2024-04-24 12:29:07.326107 animdl2-1.7.29/animdl2/core/codebase/downloader/idmanlib.py
+-rw-r--r--   0        0        0      451 2024-04-24 12:29:07.326107 animdl2-1.7.29/animdl2/core/codebase/extractors/__init__.py
+-rw-r--r--   0        0        0     1425 2024-04-24 12:29:07.328109 animdl2-1.7.29/animdl2/core/codebase/extractors/dailymotion/__init__.py
+-rw-r--r--   0        0        0      904 2024-04-24 12:29:07.329108 animdl2-1.7.29/animdl2/core/codebase/extractors/doodstream/__init__.py
+-rw-r--r--   0        0        0     2230 2024-04-24 12:29:07.330107 animdl2-1.7.29/animdl2/core/codebase/extractors/gogoplay/__init__.py
+-rw-r--r--   0        0        0     1131 2024-04-24 12:29:07.331110 animdl2-1.7.29/animdl2/core/codebase/extractors/mp4upload/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-24 12:29:07.332109 animdl2-1.7.29/animdl2/core/codebase/extractors/mycloud/__init__.py
+-rw-r--r--   0        0        0     1030 2024-04-24 12:29:07.333108 animdl2-1.7.29/animdl2/core/codebase/extractors/okru/__init__.py
+-rw-r--r--   0        0        0     1228 2024-04-24 12:29:07.334107 animdl2-1.7.29/animdl2/core/codebase/extractors/rapidvideo/__init__.py
+-rw-r--r--   0        0        0     2202 2024-04-24 12:29:07.335110 animdl2-1.7.29/animdl2/core/codebase/extractors/rapidvideo/polling.py
+-rw-r--r--   0        0        0     1111 2024-04-24 12:29:07.335110 animdl2-1.7.29/animdl2/core/codebase/extractors/rapidvideo/utils.py
+-rw-r--r--   0        0        0      933 2024-04-24 12:29:07.337109 animdl2-1.7.29/animdl2/core/codebase/extractors/streamlare/__init__.py
+-rw-r--r--   0        0        0     1133 2024-04-24 12:29:07.338114 animdl2-1.7.29/animdl2/core/codebase/extractors/streamsb/__init__.py
+-rw-r--r--   0        0        0      937 2024-04-24 12:29:07.340110 animdl2-1.7.29/animdl2/core/codebase/extractors/streamtape/__init__.py
+-rw-r--r--   0        0        0      391 2024-04-24 12:29:07.341112 animdl2-1.7.29/animdl2/core/codebase/extractors/videobin/__init__.py
+-rw-r--r--   0        0        0      909 2024-04-24 12:29:07.343107 animdl2-1.7.29/animdl2/core/codebase/extractors/vidstream/__init__.py
+-rw-r--r--   0        0        0     1957 2024-04-24 12:44:41.377688 animdl2-1.7.29/animdl2/core/codebase/helpers/__init__.py
+-rw-r--r--   0        0        0     2119 2024-04-24 12:44:41.347689 animdl2-1.7.29/animdl2/core/codebase/helpers/superscrapers.py
+-rw-r--r--   0        0        0     2681 2024-04-24 12:29:07.345110 animdl2-1.7.29/animdl2/core/codebase/helpers/uwu.py
+-rw-r--r--   0        0        0     1070 2024-04-24 12:29:07.347109 animdl2-1.7.29/animdl2/core/codebase/providers/__init__.py
+-rw-r--r--   0        0        0     6396 2024-04-24 12:29:07.348111 animdl2-1.7.29/animdl2/core/codebase/providers/allanime/__init__.py
+-rw-r--r--   0        0        0     5594 2024-04-24 12:44:41.337690 animdl2-1.7.29/animdl2/core/codebase/providers/allanime/gql_api.py
+-rw-r--r--   0        0        0     2403 2024-04-24 12:29:07.350108 animdl2-1.7.29/animdl2/core/codebase/providers/animekaizoku/__init__.py
+-rw-r--r--   0        0        0     2484 2024-04-24 12:29:07.352109 animdl2-1.7.29/animdl2/core/codebase/providers/animeonsen/__init__.py
+-rw-r--r--   0        0        0     1808 2024-04-24 12:29:07.353109 animdl2-1.7.29/animdl2/core/codebase/providers/animeout/__init__.py
+-rw-r--r--   0        0        0     2841 2024-04-24 12:44:41.326691 animdl2-1.7.29/animdl2/core/codebase/providers/animepahe/__init__.py
+-rw-r--r--   0        0        0     1824 2024-04-24 12:29:07.356110 animdl2-1.7.29/animdl2/core/codebase/providers/animepahe/inner/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-24 12:29:07.357109 animdl2-1.7.29/animdl2/core/codebase/providers/animepahe/inner/archive.py
+-rw-r--r--   0        0        0     2921 2024-04-24 12:29:07.358108 animdl2-1.7.29/animdl2/core/codebase/providers/animexin/__init__.py
+-rw-r--r--   0        0        0      407 2024-04-24 12:29:07.360107 animdl2-1.7.29/animdl2/core/codebase/providers/animixplay/__init__.py
+-rw-r--r--   0        0        0     1241 2024-04-24 12:29:07.360107 animdl2-1.7.29/animdl2/core/codebase/providers/animixplay/hardstream.py
+-rw-r--r--   0        0        0     2847 2024-04-24 12:29:07.361108 animdl2-1.7.29/animdl2/core/codebase/providers/animixplay/stream_url.py
+-rw-r--r--   0        0        0     1913 2024-04-24 12:44:41.357687 animdl2-1.7.29/animdl2/core/codebase/providers/animtime/__init__.py
+-rw-r--r--   0        0        0     2959 2024-04-24 12:29:07.364107 animdl2-1.7.29/animdl2/core/codebase/providers/crunchyroll/__init__.py
+-rw-r--r--   0        0        0     2336 2024-04-24 12:29:07.365107 animdl2-1.7.29/animdl2/core/codebase/providers/gogoanime/__init__.py
+-rw-r--r--   0        0        0     1568 2024-04-24 12:29:07.366109 animdl2-1.7.29/animdl2/core/codebase/providers/hahomoe/__init__.py
+-rw-r--r--   0        0        0     2315 2024-04-24 12:29:07.367110 animdl2-1.7.29/animdl2/core/codebase/providers/hentaistream/__init__.py
+-rw-r--r--   0        0        0     2920 2024-04-24 12:29:07.368107 animdl2-1.7.29/animdl2/core/codebase/providers/kamyroll/__init__.py
+-rw-r--r--   0        0        0     2993 2024-04-24 12:29:07.369108 animdl2-1.7.29/animdl2/core/codebase/providers/kamyroll/api.py
+-rw-r--r--   0        0        0     1879 2024-04-24 12:29:07.371113 animdl2-1.7.29/animdl2/core/codebase/providers/kawaiifu/__init__.py
+-rw-r--r--   0        0        0     2407 2024-04-24 12:44:41.399697 animdl2-1.7.29/animdl2/core/codebase/providers/marinmoe/__init__.py
+-rw-r--r--   0        0        0     2647 2024-04-24 12:29:07.373108 animdl2-1.7.29/animdl2/core/codebase/providers/nineanime/__init__.py
+-rw-r--r--   0        0        0     1759 2024-04-24 12:29:07.374107 animdl2-1.7.29/animdl2/core/codebase/providers/nineanime/decipher.py
+-rw-r--r--   0        0        0     1303 2024-04-24 12:29:07.375108 animdl2-1.7.29/animdl2/core/codebase/providers/twistmoe/__init__.py
+-rw-r--r--   0        0        0     1672 2024-04-24 12:29:07.376108 animdl2-1.7.29/animdl2/core/codebase/providers/twistmoe/stream_url.py
+-rw-r--r--   0        0        0     1967 2024-04-24 12:29:07.377107 animdl2-1.7.29/animdl2/core/codebase/providers/yugen/__init__.py
+-rw-r--r--   0        0        0     2630 2024-04-24 12:29:07.378108 animdl2-1.7.29/animdl2/core/codebase/providers/zoro/__init__.py
+-rw-r--r--   0        0        0     6369 2024-04-24 12:29:07.379109 animdl2-1.7.29/animdl2/core/config/__init__.py
+-rw-r--r--   0        0        0     4453 2024-04-24 12:29:07.380108 animdl2-1.7.29/animdl2/core/package_resolver.py
+-rw-r--r--   0        0        0      293 2024-04-24 12:29:07.381108 animdl2-1.7.29/animdl2/utils/__init__.py
+-rw-r--r--   0        0        0     7529 2024-04-24 12:44:41.409217 animdl2-1.7.29/animdl2/utils/http_caching.py
+-rw-r--r--   0        0        0     4093 2024-04-24 12:44:41.439217 animdl2-1.7.29/animdl2/utils/http_client.py
+-rw-r--r--   0        0        0     6248 2024-04-24 12:29:07.384107 animdl2-1.7.29/animdl2/utils/media_downloader.py
+-rw-r--r--   0        0        0      416 2024-04-24 12:29:07.385108 animdl2-1.7.29/animdl2/utils/optopt.py
+-rw-r--r--   0        0        0     1979 2024-04-24 12:29:07.385108 animdl2-1.7.29/animdl2/utils/powertools.py
+-rw-r--r--   0        0        0     1837 2024-04-24 12:29:07.386108 animdl2-1.7.29/animdl2/utils/searching.py
+-rw-r--r--   0        0        0     1089 2024-04-24 12:29:07.387108 animdl2-1.7.29/animdl2/utils/serverfiles.py
+-rw-r--r--   0        0        0    35823 2024-04-24 12:29:07.293631 animdl2-1.7.29/LICENSE
+-rw-r--r--   0        0        0     1010 2024-04-24 13:06:23.262612 animdl2-1.7.29/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-24 12:29:07.419628 animdl2-1.7.29/readme.txt
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 animdl2-1.7.29/PKG-INFO
```

### Comparing `animdl2-1.7.28/animdl2/__main__.py` & `animdl2-1.7.29/animdl2/__main__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/commands/download.py` & `animdl2-1.7.29/animdl2/core/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/commands/grab.py` & `animdl2-1.7.29/animdl2/core/cli/commands/grab.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/commands/schedule.py` & `animdl2-1.7.29/animdl2/core/cli/commands/schedule.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/commands/search.py` & `animdl2-1.7.29/animdl2/core/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/commands/stream.py` & `animdl2-1.7.29/animdl2/core/cli/commands/stream.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/commands/update.py` & `animdl2-1.7.29/animdl2/core/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/__init__.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/aniskip.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/aniskip.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/banner.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/banner.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/decorators.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/fuzzysearch.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/fuzzysearch.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/intelliq.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/intelliq.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/logger.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/player.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/player.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/players/android.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/players/android.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/players/base_player.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/players/base_player.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/players/ffplay.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/players/ffplay.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/players/mpv.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/players/mpv.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/players/vlc.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/players/vlc.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/processors.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/processors.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/prompts.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/prompts.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/rpc.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/rpc.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/searcher.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/searcher.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/special.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/special.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/helpers/stream_handlers.py` & `animdl2-1.7.29/animdl2/core/cli/helpers/stream_handlers.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/cli/http_client.py` & `animdl2-1.7.29/animdl2/core/cli/http_client.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/downloader/ffmpeg.py` & `animdl2-1.7.29/animdl2/core/codebase/downloader/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/downloader/handle.py` & `animdl2-1.7.29/animdl2/core/codebase/downloader/handle.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/downloader/hls.py` & `animdl2-1.7.29/animdl2/core/codebase/downloader/hls.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/downloader/idmanlib.py` & `animdl2-1.7.29/animdl2/core/codebase/downloader/idmanlib.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/dailymotion/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/dailymotion/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/doodstream/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/doodstream/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/gogoplay/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/gogoplay/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/mp4upload/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/mp4upload/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/okru/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/okru/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/rapidvideo/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/rapidvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/rapidvideo/polling.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/rapidvideo/polling.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/rapidvideo/utils.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/rapidvideo/utils.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/streamlare/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/streamlare/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/streamsb/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/streamsb/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/streamtape/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/streamtape/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/extractors/vidstream/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/extractors/vidstream/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/helpers/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/helpers/superscrapers.py` & `animdl2-1.7.29/animdl2/core/codebase/helpers/superscrapers.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/helpers/uwu.py` & `animdl2-1.7.29/animdl2/core/codebase/helpers/uwu.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/allanime/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/allanime/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/allanime/gql_api.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/allanime/gql_api.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animekaizoku/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animekaizoku/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animeonsen/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animeonsen/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animeout/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animeout/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animepahe/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animepahe/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animepahe/inner/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animepahe/inner/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animepahe/inner/archive.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animepahe/inner/archive.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animexin/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animexin/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animixplay/hardstream.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animixplay/hardstream.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animixplay/stream_url.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animixplay/stream_url.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/animtime/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/animtime/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/crunchyroll/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/crunchyroll/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/gogoanime/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/gogoanime/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/hahomoe/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/hahomoe/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/hentaistream/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/hentaistream/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/kamyroll/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/kamyroll/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/kamyroll/api.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/kamyroll/api.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/kawaiifu/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/kawaiifu/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/marinmoe/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/marinmoe/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/nineanime/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/nineanime/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/nineanime/decipher.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/nineanime/decipher.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/twistmoe/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/twistmoe/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/twistmoe/stream_url.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/twistmoe/stream_url.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/yugen/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/yugen/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/codebase/providers/zoro/__init__.py` & `animdl2-1.7.29/animdl2/core/codebase/providers/zoro/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/config/__init__.py` & `animdl2-1.7.29/animdl2/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/core/package_resolver.py` & `animdl2-1.7.29/animdl2/core/package_resolver.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/utils/http_caching.py` & `animdl2-1.7.29/animdl2/utils/http_caching.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/utils/http_client.py` & `animdl2-1.7.29/animdl2/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/utils/media_downloader.py` & `animdl2-1.7.29/animdl2/utils/media_downloader.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/utils/powertools.py` & `animdl2-1.7.29/animdl2/utils/powertools.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/utils/searching.py` & `animdl2-1.7.29/animdl2/utils/searching.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/animdl2/utils/serverfiles.py` & `animdl2-1.7.29/animdl2/utils/serverfiles.py`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/LICENSE` & `animdl2-1.7.29/LICENSE`

 * *Files identical despite different names*

### Comparing `animdl2-1.7.28/pyproject.toml` & `animdl2-1.7.29/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "animdl2"
-version = "1.7.28"
+version = "1.7.29"
 description = "A highly efficient, fast, powerful and light-weight anime downloader and streamer for your favorite anime."
 readme = "readme.txt"
 authors = [ "justfoolingaround <kr.justfoolingaround@gmail.com>", "shashstormer <shashstormer@shashstorm.in>" ]
 license = "GPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
@@ -26,12 +26,12 @@
 packaging = ">=22,<24"
 pkginfo = "^1.9.2"
 rich = ">=13.3.1,<13.3.4"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.scripts]
-animdl = "animdl.__main__:__animdl_cli__"
+animdl2 = "animdl2.__main__:__animdl_cli__"
 
 [tool.poetry.dependencies.lxml]
 version = "4.9.1"
 markers = "sys_platform != 'win32'"
```

### Comparing `animdl2-1.7.28/PKG-INFO` & `animdl2-1.7.29/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: animdl2
-Version: 1.7.28
+Version: 1.7.29
 Summary: A highly efficient, fast, powerful and light-weight anime downloader and streamer for your favorite anime.
 License: GPL-3.0-only
 Author: justfoolingaround
 Author-email: kr.justfoolingaround@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

