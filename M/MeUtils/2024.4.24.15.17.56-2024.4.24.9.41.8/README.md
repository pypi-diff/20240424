# Comparing `tmp/MeUtils-2024.4.24.15.17.56.tar.gz` & `tmp/MeUtils-2024.4.24.9.41.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeUtils-2024.4.24.15.17.56.tar", last modified: Wed Apr 24 07:17:56 2024, max compression
+gzip compressed data, was "MeUtils-2024.4.24.9.41.8.tar", last modified: Wed Apr 24 01:41:08 2024, max compression
```

## Comparing `MeUtils-2024.4.24.15.17.56.tar` & `MeUtils-2024.4.24.9.41.8.tar`

### file list

```diff
@@ -1,446 +1,439 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.395669 MeUtils-2024.4.24.15.17.56/
--rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      331 2023-11-29 08:20:55.000000 MeUtils-2024.4.24.15.17.56/MANIFEST.in
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.295145 MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5961 2024-04-24 07:17:56.000000 MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    13080 2024-04-24 07:17:56.000000 MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-24 07:17:56.000000 MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)      312 2024-04-24 07:17:56.000000 MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1186 2024-04-24 07:17:56.000000 MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)       22 2024-04-24 07:17:56.000000 MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)     5961 2024-04-24 07:17:56.395386 MeUtils-2024.4.24.15.17.56/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2024.4.24.15.17.56/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.295618 MeUtils-2024.4.24.15.17.56/apps/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2024-01-18 04:10:04.000000 MeUtils-2024.4.24.15.17.56/apps/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      462 2024-01-18 04:20:39.000000 MeUtils-2024.4.24.15.17.56/apps/spider.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.301139 MeUtils-2024.4.24.15.17.56/meutils/
--rw-r--r--   0 betterme   (501) staff       (20)      348 2023-08-17 00:48:50.000000 MeUtils-2024.4.24.15.17.56/meutils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2024.4.24.15.17.56/meutils/_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.302482 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-11-21 10:11:16.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/adjusted_audio1.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.303380 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-11-28 10:28:28.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3121 2023-11-28 02:24:07.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/fast_asr.py
--rw-r--r--   0 betterme   (501) staff       (20)      514 2023-12-11 10:44:07.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/openai_asr.py
--rw-r--r--   0 betterme   (501) staff       (20)     7251 2023-12-01 04:06:03.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/xunfei_asr.py
--rw-r--r--   0 betterme   (501) staff       (20)     1226 2023-11-21 06:01:47.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr.py
--rw-r--r--   0 betterme   (501) staff       (20)     2968 2023-11-21 11:25:44.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/fast_asr.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.304332 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts/
--rw-r--r--   0 betterme   (501) staff       (20)     5884 2024-03-27 05:35:42.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts/EdgeTTS.py
--rw-r--r--   0 betterme   (501) staff       (20)      405 2023-12-26 05:42:13.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1755 2024-03-27 06:30:42.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts/openai_tts.py
--rw-r--r--   0 betterme   (501) staff       (20)     4638 2024-03-27 03:35:59.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts/tts_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     2494 2023-11-21 10:39:01.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts.py
--rw-r--r--   0 betterme   (501) staff       (20)     1214 2023-11-28 10:28:28.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_audio/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.305671 MeUtils-2024.4.24.15.17.56/meutils/ai_cv/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_cv/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2684 2023-09-01 11:12:26.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_cv/doc_prompt.py
--rw-r--r--   0 betterme   (501) staff       (20)     1152 2023-11-02 10:12:40.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_cv/latex_ocr.py
--rw-r--r--   0 betterme   (501) staff       (20)      682 2023-10-24 01:58:01.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_cv/ocr.py
--rw-r--r--   0 betterme   (501) staff       (20)     2401 2023-09-25 04:18:07.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_cv/ocr_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.308568 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/
--rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/SplitSentence.py
--rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/Untitled-1(1).py
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/_lda.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.309265 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/_textsplitter/
--rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/_textsplitter/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/_textsplitter/text_split.py
--rw-r--r--   0 betterme   (501) staff       (20)      650 2023-12-12 02:19:51.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      329 2023-10-26 01:47:40.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/epub翻译.py
--rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/lda.py
--rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-07-25 08:50:49.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/ner.py
--rw-r--r--   0 betterme   (501) staff       (20)     1019 2023-12-12 03:58:07.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/text_transformer.py
--rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.311103 MeUtils-2024.4.24.15.17.56/meutils/ai_video/
--rw-r--r--   0 betterme   (501) staff       (20)      254 2020-12-15 11:24:42.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_video/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1143 2023-11-20 10:32:55.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_video/avmerge.py
--rw-r--r--   0 betterme   (501) staff       (20)      881 2023-11-22 09:38:35.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_video/avmerge_.py
--rw-r--r--   0 betterme   (501) staff       (20)     3470 2023-11-24 07:46:38.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_video/scene_detect.py
--rw-r--r--   0 betterme   (501) staff       (20)     1760 2023-11-24 07:57:00.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_video/test.py
--rw-r--r--   0 betterme   (501) staff       (20)     1727 2023-11-24 08:38:38.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_video/video.py
--rw-r--r--   0 betterme   (501) staff       (20)      902 2023-11-17 08:12:46.000000 MeUtils-2024.4.24.15.17.56/meutils/ai_video/xx.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.313242 MeUtils-2024.4.24.15.17.56/meutils/ann/
--rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/ann.py
--rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/ann_faiss.py
--rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/ann_gensim.py
--rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/ann_inmemory.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/ann_qdrant.py
--rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/ann_service.py
--rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/ann_v1.py
--rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/milvus.py
--rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/ann/shake_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.313850 MeUtils-2024.4.24.15.17.56/meutils/api/
--rw-r--r--   0 betterme   (501) staff       (20)      344 2023-12-04 08:54:59.000000 MeUtils-2024.4.24.15.17.56/meutils/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3659 2024-04-18 06:58:56.000000 MeUtils-2024.4.24.15.17.56/meutils/api/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      936 2024-04-24 01:41:03.000000 MeUtils-2024.4.24.15.17.56/meutils/api/deeplx.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.314300 MeUtils-2024.4.24.15.17.56/meutils/async_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      284 2023-08-28 05:10:12.000000 MeUtils-2024.4.24.15.17.56/meutils/async_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1928 2024-04-23 09:00:37.000000 MeUtils-2024.4.24.15.17.56/meutils/async_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     8285 2024-01-20 10:30:04.000000 MeUtils-2024.4.24.15.17.56/meutils/cache_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.316701 MeUtils-2024.4.24.15.17.56/meutils/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4511 2024-01-03 02:50:38.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/browser.py
--rw-r--r--   0 betterme   (501) staff       (20)     3212 2024-02-21 06:58:51.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)      319 2024-01-17 03:02:30.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/cloudflare.py
--rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/cron.py
--rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/gunicorn.conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      731 2023-08-30 03:57:39.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/nesc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1757 2023-12-27 00:56:08.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/notice.py
--rw-r--r--   0 betterme   (501) staff       (20)     2411 2024-02-27 08:32:53.000000 MeUtils-2024.4.24.15.17.56/meutils/clis/server.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.317438 MeUtils-2024.4.24.15.17.56/meutils/cmds/
--rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/cmds/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/cmds/cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/cmds/hdfs_cmd.py
--rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/cmds/subprocess_demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.317731 MeUtils-2024.4.24.15.17.56/meutils/coding/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/coding/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/coding/find132.py
--rw-r--r--   0 betterme   (501) staff       (20)    15339 2024-03-22 01:11:55.000000 MeUtils-2024.4.24.15.17.56/meutils/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.318009 MeUtils-2024.4.24.15.17.56/meutils/comp_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/comp_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/comp_utils/reverse_metric.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.318403 MeUtils-2024.4.24.15.17.56/meutils/config_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2024-04-17 09:00:55.000000 MeUtils-2024.4.24.15.17.56/meutils/config_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1040 2024-04-17 09:06:22.000000 MeUtils-2024.4.24.15.17.56/meutils/config_utils/nacos.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.318636 MeUtils-2024.4.24.15.17.56/meutils/crawlers/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2024-04-19 05:42:51.000000 MeUtils-2024.4.24.15.17.56/meutils/crawlers/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.328841 MeUtils-2024.4.24.15.17.56/meutils/data/
--rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2024.4.24.15.17.56/meutils/data/SimHei.ttf
--rw-r--r--   0 betterme   (501) staff       (20)       19 2024-04-24 07:17:56.000000 MeUtils-2024.4.24.15.17.56/meutils/data/VERSION
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/data/_FLAG
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/data/_SUCCESS
--rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/data/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/data/coordinate.py
--rw-r--r--   0 betterme   (501) staff       (20)     2497 2023-09-07 05:50:11.000000 MeUtils-2024.4.24.15.17.56/meutils/date_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.330669 MeUtils-2024.4.24.15.17.56/meutils/db/
--rw-r--r--   0 betterme   (501) staff       (20)     7637 2024-01-05 00:39:21.000000 MeUtils-2024.4.24.15.17.56/meutils/db/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/db/mongo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/db/neo4j.py
--rw-r--r--   0 betterme   (501) staff       (20)      265 2024-03-26 03:21:15.000000 MeUtils-2024.4.24.15.17.56/meutils/db/redis_db.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.335211 MeUtils-2024.4.24.15.17.56/meutils/decorators/
--rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/__ai.py
--rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2951 2023-12-28 05:10:23.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/cache.py
--rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/catch.py
--rw-r--r--   0 betterme   (501) staff       (20)    10644 2024-03-27 05:09:13.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     1251 2024-01-16 12:50:20.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/contextmanagers.py
--rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/decorator_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      710 2023-12-26 09:35:03.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     1355 2024-01-09 00:35:44.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/fastapi_decorator.py
--rw-r--r--   0 betterme   (501) staff       (20)     3634 2023-08-24 02:55:32.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)     2976 2024-02-27 09:07:28.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/retry.py
--rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     2664 2023-11-06 02:17:41.000000 MeUtils-2024.4.24.15.17.56/meutils/decorators/schedulers.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.335447 MeUtils-2024.4.24.15.17.56/meutils/dependencies/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-02 08:27:24.000000 MeUtils-2024.4.24.15.17.56/meutils/dependencies/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2024.4.24.15.17.56/meutils/dist_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.336609 MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/demo_es.py
--rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/demo_hnsw.py
--rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/in_memory.py
--rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/改造下hnsw.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.337026 MeUtils-2024.4.24.15.17.56/meutils/easy_search/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/easy_search/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2425 2023-08-02 06:36:30.000000 MeUtils-2024.4.24.15.17.56/meutils/easy_search/es.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.339013 MeUtils-2024.4.24.15.17.56/meutils/fileparser/
--rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/PDF抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)      284 2023-07-12 04:10:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2792 2023-08-16 04:33:39.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.340419 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/
--rw-r--r--   0 betterme   (501) staff       (20)      223 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      803 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/__main__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/filetype.py
--rw-r--r--   0 betterme   (501) staff       (20)     2947 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/helpers.py
--rw-r--r--   0 betterme   (501) staff       (20)     3288 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/match.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.342920 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/
--rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      498 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/application.py
--rw-r--r--   0 betterme   (501) staff       (20)    17006 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/archive.py
--rw-r--r--   0 betterme   (501) staff       (20)     4960 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/audio.py
--rw-r--r--   0 betterme   (501) staff       (20)      647 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/base.py
--rw-r--r--   0 betterme   (501) staff       (20)     7513 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/document.py
--rw-r--r--   0 betterme   (501) staff       (20)     2924 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/font.py
--rw-r--r--   0 betterme   (501) staff       (20)     9130 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/image.py
--rw-r--r--   0 betterme   (501) staff       (20)      958 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/isobmff.py
--rw-r--r--   0 betterme   (501) staff       (20)     5371 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/video.py
--rw-r--r--   0 betterme   (501) staff       (20)     2089 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      694 2024-04-22 08:58:46.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype.py
--rw-r--r--   0 betterme   (501) staff       (20)      639 2023-08-10 05:04:53.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4037 2023-07-17 10:15:11.000000 MeUtils-2024.4.24.15.17.56/meutils/fileparser/表格抽取.py
--rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2024.4.24.15.17.56/meutils/hash_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/import_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.343612 MeUtils-2024.4.24.15.17.56/meutils/init/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2024.4.24.15.17.56/meutils/init/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1588 2023-08-07 08:26:31.000000 MeUtils-2024.4.24.15.17.56/meutils/init/evn.py
--rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2024.4.24.15.17.56/meutils/init/oo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.345048 MeUtils-2024.4.24.15.17.56/meutils/io/
--rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2024.4.24.15.17.56/meutils/io/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/io/file.py
--rw-r--r--   0 betterme   (501) staff       (20)     3038 2024-04-22 08:24:23.000000 MeUtils-2024.4.24.15.17.56/meutils/io/image.py
--rw-r--r--   0 betterme   (501) staff       (20)     1274 2024-02-05 09:39:04.000000 MeUtils-2024.4.24.15.17.56/meutils/io/minio_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2024.4.24.15.17.56/meutils/io/tf_io.py
--rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/jinja_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.345526 MeUtils-2024.4.24.15.17.56/meutils/llm/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2024-04-24 05:35:34.000000 MeUtils-2024.4.24.15.17.56/meutils/llm/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3729 2024-04-24 06:55:47.000000 MeUtils-2024.4.24.15.17.56/meutils/llm/demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.345661 MeUtils-2024.4.24.15.17.56/meutils/llm/functions/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2024-04-24 06:06:51.000000 MeUtils-2024.4.24.15.17.56/meutils/llm/functions/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.345804 MeUtils-2024.4.24.15.17.56/meutils/llm/output_parsers/
--rw-r--r--   0 betterme   (501) staff       (20)     3028 2024-04-24 06:13:45.000000 MeUtils-2024.4.24.15.17.56/meutils/llm/output_parsers/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.346752 MeUtils-2024.4.24.15.17.56/meutils/logging/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-15 06:07:38.000000 MeUtils-2024.4.24.15.17.56/meutils/logging/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      701 2023-08-21 08:23:51.000000 MeUtils-2024.4.24.15.17.56/meutils/logging/handlers.py
--rw-r--r--   0 betterme   (501) staff       (20)     2937 2023-08-15 01:04:50.000000 MeUtils-2024.4.24.15.17.56/meutils/logging/log_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6183 2024-02-08 00:37:38.000000 MeUtils-2024.4.24.15.17.56/meutils/logging/logger.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.348874 MeUtils-2024.4.24.15.17.56/meutils/notice/
--rw-r--r--   0 betterme   (501) staff       (20)      248 2023-08-30 03:57:39.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-10-16 09:04:49.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/emails.py
--rw-r--r--   0 betterme   (501) staff       (20)     2411 2024-04-22 11:17:05.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/feishu.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/file_post.py
--rw-r--r--   0 betterme   (501) staff       (20)     7331 2023-09-12 01:53:53.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/load_emailfile - 副本.py
--rw-r--r--   0 betterme   (501) staff       (20)     4207 2024-03-06 06:10:50.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/wechat_.py
--rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/wecom.py
--rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/notice/weekmeet.py
--rw-r--r--   0 betterme   (501) staff       (20)     3559 2023-08-14 09:47:22.000000 MeUtils-2024.4.24.15.17.56/meutils/np_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.349993 MeUtils-2024.4.24.15.17.56/meutils/office_automation/
--rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/office_automation/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2024.4.24.15.17.56/meutils/office_automation/doc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1528 2023-07-25 10:06:46.000000 MeUtils-2024.4.24.15.17.56/meutils/office_automation/pdf.py
--rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2024.4.24.15.17.56/meutils/office_automation/pdm.py
--rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2024.4.24.15.17.56/meutils/office_automation/pdm_run.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.350247 MeUtils-2024.4.24.15.17.56/meutils/office_automation/report/
--rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/office_automation/report/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.350882 MeUtils-2024.4.24.15.17.56/meutils/oss/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2024-03-14 09:54:51.000000 MeUtils-2024.4.24.15.17.56/meutils/oss/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     4500 2024-03-18 03:06:05.000000 MeUtils-2024.4.24.15.17.56/meutils/oss/minio_oss.py
--rw-r--r--   0 betterme   (501) staff       (20)     1274 2024-02-05 09:39:04.000000 MeUtils-2024.4.24.15.17.56/meutils/oss/minio_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.352024 MeUtils-2024.4.24.15.17.56/meutils/other/
--rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2024.4.24.15.17.56/meutils/other/__demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/other/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.353994 MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/
--rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/__version__.py
--rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/core.py
--rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/pool.py
--rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/types.py
--rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/other/besttable.py
--rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2024.4.24.15.17.56/meutils/other/crontab.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.354703 MeUtils-2024.4.24.15.17.56/meutils/pandas_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/pandas_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/pandas_utils/opt.py
--rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/pandas_utils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2024.4.24.15.17.56/meutils/path_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/pd_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)    10133 2023-11-27 09:25:49.000000 MeUtils-2024.4.24.15.17.56/meutils/pipe.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.355494 MeUtils-2024.4.24.15.17.56/meutils/playwright_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      291 2024-01-02 10:44:47.000000 MeUtils-2024.4.24.15.17.56/meutils/playwright_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2024-01-18 03:09:30.000000 MeUtils-2024.4.24.15.17.56/meutils/playwright_utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3145 2024-01-05 03:48:40.000000 MeUtils-2024.4.24.15.17.56/meutils/playwright_utils/reload.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.357954 MeUtils-2024.4.24.15.17.56/meutils/plots/
--rw-r--r--   0 betterme   (501) staff       (20)      276 2023-09-12 02:56:35.000000 MeUtils-2024.4.24.15.17.56/meutils/plots/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2022 2023-09-12 02:59:23.000000 MeUtils-2024.4.24.15.17.56/meutils/plots/common.py
--rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/plots/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/plots/echarts.py
--rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2024.4.24.15.17.56/meutils/plots/embedding_plot.py
--rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2024.4.24.15.17.56/meutils/plots/mecharts.py
--rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/plots/metrics.py
--rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/plots/plot_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.359096 MeUtils-2024.4.24.15.17.56/meutils/queues/
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-07-20 02:35:53.000000 MeUtils-2024.4.24.15.17.56/meutils/queues/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1735 2023-12-06 09:14:18.000000 MeUtils-2024.4.24.15.17.56/meutils/queues/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     1491 2024-03-22 07:55:29.000000 MeUtils-2024.4.24.15.17.56/meutils/queues/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)     3270 2024-04-11 01:15:50.000000 MeUtils-2024.4.24.15.17.56/meutils/queues/smooth_queue.py
--rw-r--r--   0 betterme   (501) staff       (20)     1564 2024-03-22 09:12:23.000000 MeUtils-2024.4.24.15.17.56/meutils/queues/uniform_queue.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.361019 MeUtils-2024.4.24.15.17.56/meutils/request_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     3375 2023-07-27 05:15:39.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-11-03 02:19:03.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/a爬虫.py
--rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/crawler.py
--rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/download.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/results.py
--rw-r--r--   0 betterme   (501) staff       (20)     3057 2023-12-04 10:37:44.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/tiangong.py
--rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/wechat.py
--rw-r--r--   0 betterme   (501) staff       (20)      646 2023-11-22 01:02:28.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/公网ip.py
--rw-r--r--   0 betterme   (501) staff       (20)     1735 2024-01-17 05:19:28.000000 MeUtils-2024.4.24.15.17.56/meutils/request_utils/爬虫.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.361515 MeUtils-2024.4.24.15.17.56/meutils/schemas/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-24 06:44:44.000000 MeUtils-2024.4.24.15.17.56/meutils/schemas/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      484 2023-08-25 03:48:09.000000 MeUtils-2024.4.24.15.17.56/meutils/schemas/baidu_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.362143 MeUtils-2024.4.24.15.17.56/meutils/serving/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/_fastapi.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.364143 MeUtils-2024.4.24.15.17.56/meutils/serving/celery/
--rw-r--r--   0 betterme   (501) staff       (20)      628 2023-08-04 02:38:19.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/celery/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2109 2023-08-04 05:36:36.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/celery/_conf.py
--rw-r--r--   0 betterme   (501) staff       (20)      514 2023-08-04 06:55:40.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/celery/_demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      415 2023-08-04 07:01:12.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/celery/_run_fastapi.py
--rw-r--r--   0 betterme   (501) staff       (20)     1126 2023-11-08 05:27:33.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/celery/router.py
--rw-r--r--   0 betterme   (501) staff       (20)     1465 2023-08-04 07:31:09.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/celery/tasks.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.365226 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.365721 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/__demo/异步任务.py
--rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     3897 2024-01-18 03:22:23.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.366222 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/dependencies/
--rw-r--r--   0 betterme   (501) staff       (20)      272 2023-12-19 09:14:44.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/dependencies/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      369 2023-12-19 09:14:44.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/dependencies/auth.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.366855 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/exceptions/
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/exceptions/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      509 2024-03-14 10:06:19.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/exceptions/http_error.py
--rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/exceptions/validation_error.py
--rw-r--r--   0 betterme   (501) staff       (20)     7791 2024-02-22 02:14:50.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/gunicorn.conf.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.368125 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-09 00:52:27.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      546 2024-01-09 01:09:19.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     1440 2024-01-09 01:03:15.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/scheduler.py
--rw-r--r--   0 betterme   (501) staff       (20)      544 2024-01-09 01:00:29.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/shutdown.py
--rw-r--r--   0 betterme   (501) staff       (20)     1197 2024-01-18 08:10:48.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/spider.py
--rw-r--r--   0 betterme   (501) staff       (20)     2994 2024-03-14 10:39:22.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.369004 MeUtils-2024.4.24.15.17.56/meutils/serving/gui/
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/gui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1690 2024-01-24 01:49:04.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/gui/bar.py
--rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/gui/demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.369255 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.370749 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/client.py
--rw-r--r--   0 betterme   (501) staff       (20)      926 2023-07-24 06:13:28.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/s.py
--rw-r--r--   0 betterme   (501) staff       (20)      953 2023-07-24 06:17:01.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/s2.py
--rw-r--r--   0 betterme   (501) staff       (20)     2113 2023-07-24 06:04:10.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/server.py
--rw-r--r--   0 betterme   (501) staff       (20)     1160 2023-07-19 06:57:16.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/test.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.372054 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/
--rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/SentenceEncoder.py
--rw-r--r--   0 betterme   (501) staff       (20)     1831 2023-07-17 10:23:25.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/SentenceEncoder_.py
--rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-07-24 06:57:00.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/base.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.372605 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/nlp_serving/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/nlp_serving/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/jina/nlp_serving/word_segmentation.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.372937 MeUtils-2024.4.24.15.17.56/meutils/serving/rq/
--rw-r--r--   0 betterme   (501) staff       (20)      321 2023-11-08 05:10:21.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/rq/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.374244 MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-09-20 06:06:45.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      931 2023-12-04 10:19:52.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/_test.py
--rw-r--r--   0 betterme   (501) staff       (20)     3887 2023-11-21 03:52:24.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/chat_latex.py
--rw-r--r--   0 betterme   (501) staff       (20)     6930 2024-03-25 05:38:12.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     1427 2023-11-03 05:24:48.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/demo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.375278 MeUtils-2024.4.24.15.17.56/meutils/serving/webui/
--rw-r--r--   0 betterme   (501) staff       (20)     1757 2023-08-23 04:01:26.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/webui/_2_词性标注与实体识别.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      509 2023-08-23 04:01:26.000000 MeUtils-2024.4.24.15.17.56/meutils/serving/webui/_🏆_主页.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.375979 MeUtils-2024.4.24.15.17.56/meutils/settings/
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-21 06:24:50.000000 MeUtils-2024.4.24.15.17.56/meutils/settings/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      264 2023-08-21 06:29:43.000000 MeUtils-2024.4.24.15.17.56/meutils/settings/base.py
--rw-r--r--   0 betterme   (501) staff       (20)      484 2023-08-21 06:31:48.000000 MeUtils-2024.4.24.15.17.56/meutils/settings/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/sftp.py
--rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/sk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     1400 2023-08-25 08:16:40.000000 MeUtils-2024.4.24.15.17.56/meutils/smooth_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.376185 MeUtils-2024.4.24.15.17.56/meutils/spark/
--rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/spark/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.377097 MeUtils-2024.4.24.15.17.56/meutils/str_utils/
--rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/str_utils/Translator.py
--rw-r--r--   0 betterme   (501) staff       (20)     6697 2023-12-22 01:04:55.000000 MeUtils-2024.4.24.15.17.56/meutils/str_utils/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.377819 MeUtils-2024.4.24.15.17.56/meutils/str_utils/__translater/
--rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/str_utils/__translater/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/str_utils/__translater/tencent.py
--rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/str_utils/__translater/translater.py
--rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/str_utils/__translater/youdao.py
--rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2024.4.24.15.17.56/meutils/str_utils/json_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)     2701 2024-04-23 03:08:58.000000 MeUtils-2024.4.24.15.17.56/meutils/str_utils/regular_expression.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.378271 MeUtils-2024.4.24.15.17.56/meutils/tasks/
--rw-r--r--   0 betterme   (501) staff       (20)      280 2023-11-08 05:13:34.000000 MeUtils-2024.4.24.15.17.56/meutils/tasks/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      627 2023-11-08 05:23:51.000000 MeUtils-2024.4.24.15.17.56/meutils/tasks/common.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.380602 MeUtils-2024.4.24.15.17.56/meutils/templates/
--rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/demo.conf
--rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/demo.j2
--rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/demo.py
--rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/demox.py
--rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/df_html.j2
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.382428 MeUtils-2024.4.24.15.17.56/meutils/templates/dockerfiles/
--rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/dockerfiles/Dockerfile
--rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/dockerfiles/Dockerfile_me
--rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/dockerfiles/Dockerfile_milvus
--rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/dockerfiles/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/dockerfiles/docker_build_push.py
--rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/dockerfiles/docker_push.sh
--rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/hegui.py
--rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/markmap.html
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.382718 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/
--rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/cookiecutter.json
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.386395 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.386556 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
--rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
--rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.388746 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
--rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.388895 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
--rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
--rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
--rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.389216 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.389542 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
--rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.390077 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
--rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/tpl.docx
--rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/x.html
--rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/templates/合规日报模板.docx
--rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2024.4.24.15.17.56/meutils/todo.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 07:17:56.391126 MeUtils-2024.4.24.15.17.56/meutils/tools/
--rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/tools/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/tools/cprint.py
--rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/tools/machine_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/tools/seize.py
--rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/tools/service_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/tools/sys_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)      997 2024-04-22 10:50:36.000000 MeUtils-2024.4.24.15.17.56/meutils/tools/token_monitor.py
--rw-r--r--   0 betterme   (501) staff       (20)     1127 2023-12-11 10:37:26.000000 MeUtils-2024.4.24.15.17.56/meutils/types.py
--rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.15.17.56/meutils/zk_utils.py
--rw-r--r--   0 betterme   (501) staff       (20)       38 2024-04-24 07:17:56.395718 MeUtils-2024.4.24.15.17.56/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     2466 2023-11-29 08:25:30.000000 MeUtils-2024.4.24.15.17.56/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.474005 MeUtils-2024.4.24.9.41.8/
+-rw-r--r--   0 betterme   (501) staff       (20)    11357 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      331 2023-11-29 08:20:55.000000 MeUtils-2024.4.24.9.41.8/MANIFEST.in
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.368677 MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5959 2024-04-24 01:41:08.000000 MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    12963 2024-04-24 01:41:08.000000 MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2024-04-24 01:41:08.000000 MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      312 2024-04-24 01:41:08.000000 MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1186 2024-04-24 01:41:08.000000 MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2024-04-24 01:41:08.000000 MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     5959 2024-04-24 01:41:08.473699 MeUtils-2024.4.24.9.41.8/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1067 2023-05-04 03:00:27.000000 MeUtils-2024.4.24.9.41.8/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.369031 MeUtils-2024.4.24.9.41.8/apps/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2024-01-18 04:10:04.000000 MeUtils-2024.4.24.9.41.8/apps/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      462 2024-01-18 04:20:39.000000 MeUtils-2024.4.24.9.41.8/apps/spider.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.374582 MeUtils-2024.4.24.9.41.8/meutils/
+-rw-r--r--   0 betterme   (501) staff       (20)      348 2023-08-17 00:48:50.000000 MeUtils-2024.4.24.9.41.8/meutils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1850 2023-04-11 05:47:45.000000 MeUtils-2024.4.24.9.41.8/meutils/_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.376141 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 05:51:24.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-11-21 10:11:16.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/adjusted_audio1.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.377128 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-11-28 10:28:28.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3121 2023-11-28 02:24:07.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/fast_asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)      514 2023-12-11 10:44:07.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/openai_asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7251 2023-12-01 04:06:03.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/xunfei_asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1226 2023-11-21 06:01:47.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2968 2023-11-21 11:25:44.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/fast_asr.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.378095 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts/
+-rw-r--r--   0 betterme   (501) staff       (20)     5884 2024-03-27 05:35:42.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts/EdgeTTS.py
+-rw-r--r--   0 betterme   (501) staff       (20)      405 2023-12-26 05:42:13.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1755 2024-03-27 06:30:42.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts/openai_tts.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4638 2024-03-27 03:35:59.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts/tts_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2494 2023-11-21 10:39:01.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1214 2023-11-28 10:28:28.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_audio/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.379376 MeUtils-2024.4.24.9.41.8/meutils/ai_cv/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-18 08:11:56.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_cv/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2684 2023-09-01 11:12:26.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_cv/doc_prompt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1152 2023-11-02 10:12:40.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_cv/latex_ocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)      682 2023-10-24 01:58:01.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_cv/ocr.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2401 2023-09-25 04:18:07.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_cv/ocr_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.382721 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/
+-rw-r--r--   0 betterme   (501) staff       (20)     6927 2023-06-30 13:22:13.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/SplitSentence.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13489 2023-05-21 05:19:20.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/Untitled-1(1).py
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-04-25 06:23:09.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2295 2023-04-10 08:57:58.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/_lda.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.383632 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/_textsplitter/
+-rw-r--r--   0 betterme   (501) staff       (20)      287 2023-05-22 01:52:50.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/_textsplitter/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6673 2023-05-21 05:10:54.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2282 2023-05-21 05:27:40.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/_textsplitter/text_split.py
+-rw-r--r--   0 betterme   (501) staff       (20)      650 2023-12-12 02:19:51.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      329 2023-10-26 01:47:40.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/epub翻译.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1111 2023-06-06 06:44:28.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/lda.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2560 2023-07-25 08:50:49.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/ner.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1019 2023-12-12 03:58:07.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/text_transformer.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2111 2023-06-30 13:18:15.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3542 2023-06-05 05:29:27.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.385467 MeUtils-2024.4.24.9.41.8/meutils/ai_video/
+-rw-r--r--   0 betterme   (501) staff       (20)      254 2020-12-15 11:24:42.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_video/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1143 2023-11-20 10:32:55.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_video/avmerge.py
+-rw-r--r--   0 betterme   (501) staff       (20)      881 2023-11-22 09:38:35.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_video/avmerge_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3470 2023-11-24 07:46:38.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_video/scene_detect.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1760 2023-11-24 07:57:00.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_video/test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1727 2023-11-24 08:38:38.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_video/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)      902 2023-11-17 08:12:46.000000 MeUtils-2024.4.24.9.41.8/meutils/ai_video/xx.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.388331 MeUtils-2024.4.24.9.41.8/meutils/ann/
+-rw-r--r--   0 betterme   (501) staff       (20)      240 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9161 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/ann.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5662 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/ann_faiss.py
+-rw-r--r--   0 betterme   (501) staff       (20)      965 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/ann_gensim.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1002 2023-05-16 06:47:06.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/ann_inmemory.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-05-19 06:06:57.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/ann_qdrant.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1171 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/ann_service.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4743 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/ann_v1.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1927 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      238 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/milvus.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1076 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/ann/shake_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.388947 MeUtils-2024.4.24.9.41.8/meutils/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      344 2023-12-04 08:54:59.000000 MeUtils-2024.4.24.9.41.8/meutils/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3659 2024-04-18 06:58:56.000000 MeUtils-2024.4.24.9.41.8/meutils/api/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      936 2024-04-24 01:41:03.000000 MeUtils-2024.4.24.9.41.8/meutils/api/deeplx.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.389301 MeUtils-2024.4.24.9.41.8/meutils/async_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      284 2023-08-28 05:10:12.000000 MeUtils-2024.4.24.9.41.8/meutils/async_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1928 2024-04-23 09:00:37.000000 MeUtils-2024.4.24.9.41.8/meutils/async_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8285 2024-01-20 10:30:04.000000 MeUtils-2024.4.24.9.41.8/meutils/cache_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.391793 MeUtils-2024.4.24.9.41.8/meutils/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4511 2024-01-03 02:50:38.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/browser.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3212 2024-02-21 06:58:51.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)      319 2024-01-17 03:02:30.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/cloudflare.py
+-rw-r--r--   0 betterme   (501) staff       (20)      738 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2234 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/cron.py
+-rw-r--r--   0 betterme   (501) staff       (20)      595 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1517 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/gunicorn.conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      619 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      731 2023-08-30 03:57:39.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/nesc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1757 2023-12-27 00:56:08.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/notice.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2411 2024-02-27 08:32:53.000000 MeUtils-2024.4.24.9.41.8/meutils/clis/server.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.392550 MeUtils-2024.4.24.9.41.8/meutils/cmds/
+-rw-r--r--   0 betterme   (501) staff       (20)      293 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/cmds/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      458 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/cmds/cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1734 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/cmds/hdfs_cmd.py
+-rw-r--r--   0 betterme   (501) staff       (20)      629 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/cmds/subprocess_demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.392953 MeUtils-2024.4.24.9.41.8/meutils/coding/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/coding/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      942 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/coding/find132.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15339 2024-03-22 01:11:55.000000 MeUtils-2024.4.24.9.41.8/meutils/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.393335 MeUtils-2024.4.24.9.41.8/meutils/comp_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      361 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/comp_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1705 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/comp_utils/reverse_metric.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.393776 MeUtils-2024.4.24.9.41.8/meutils/config_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2024-04-17 09:00:55.000000 MeUtils-2024.4.24.9.41.8/meutils/config_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1040 2024-04-17 09:06:22.000000 MeUtils-2024.4.24.9.41.8/meutils/config_utils/nacos.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.394028 MeUtils-2024.4.24.9.41.8/meutils/crawlers/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2024-04-19 05:42:51.000000 MeUtils-2024.4.24.9.41.8/meutils/crawlers/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.402552 MeUtils-2024.4.24.9.41.8/meutils/data/
+-rw-r--r--   0 betterme   (501) staff       (20) 10062565 2022-11-07 06:01:38.000000 MeUtils-2024.4.24.9.41.8/meutils/data/SimHei.ttf
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2024-04-24 01:41:08.000000 MeUtils-2024.4.24.9.41.8/meutils/data/VERSION
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/data/_FLAG
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/data/_SUCCESS
+-rw-r--r--   0 betterme   (501) staff       (20)      243 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/data/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      600 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/data/coordinate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2497 2023-09-07 05:50:11.000000 MeUtils-2024.4.24.9.41.8/meutils/date_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.406640 MeUtils-2024.4.24.9.41.8/meutils/db/
+-rw-r--r--   0 betterme   (501) staff       (20)     7637 2024-01-05 00:39:21.000000 MeUtils-2024.4.24.9.41.8/meutils/db/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2337 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/db/mongo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2168 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/db/neo4j.py
+-rw-r--r--   0 betterme   (501) staff       (20)      265 2024-03-26 03:21:15.000000 MeUtils-2024.4.24.9.41.8/meutils/db/redis_db.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.410254 MeUtils-2024.4.24.9.41.8/meutils/decorators/
+-rw-r--r--   0 betterme   (501) staff       (20)     1681 2023-05-25 09:49:50.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/__ai.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3284 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2951 2023-12-28 05:10:23.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/cache.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1837 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/catch.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10644 2024-03-27 05:09:13.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1251 2024-01-16 12:50:20.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/contextmanagers.py
+-rw-r--r--   0 betterme   (501) staff       (20)    15570 2023-04-06 06:24:58.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)      754 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/decorator_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      710 2023-12-26 09:35:03.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1355 2024-01-09 00:35:44.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/fastapi_decorator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3634 2023-08-24 02:55:32.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2976 2024-02-27 09:07:28.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/retry.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1678 2023-04-04 15:22:58.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2664 2023-11-06 02:17:41.000000 MeUtils-2024.4.24.9.41.8/meutils/decorators/schedulers.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.410495 MeUtils-2024.4.24.9.41.8/meutils/dependencies/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-02 08:27:24.000000 MeUtils-2024.4.24.9.41.8/meutils/dependencies/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3640 2023-05-15 10:32:24.000000 MeUtils-2024.4.24.9.41.8/meutils/dist_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.411731 MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-18 06:24:19.000000 MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      977 2023-04-21 04:31:21.000000 MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/demo_es.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1341 2023-04-26 13:37:46.000000 MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/demo_hnsw.py
+-rw-r--r--   0 betterme   (501) staff       (20)      985 2023-04-27 02:39:23.000000 MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/in_memory.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1058 2023-04-27 01:04:00.000000 MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/改造下hnsw.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.412204 MeUtils-2024.4.24.9.41.8/meutils/easy_search/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/easy_search/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2425 2023-08-02 06:36:30.000000 MeUtils-2024.4.24.9.41.8/meutils/easy_search/es.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.413870 MeUtils-2024.4.24.9.41.8/meutils/fileparser/
+-rw-r--r--   0 betterme   (501) staff       (20)     1975 2023-05-30 05:34:49.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/PDF抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)      284 2023-07-12 04:10:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2792 2023-08-16 04:33:39.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.415450 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/
+-rw-r--r--   0 betterme   (501) staff       (20)      223 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      803 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/__main__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2122 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/filetype.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2947 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/helpers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3288 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/match.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.417616 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/
+-rw-r--r--   0 betterme   (501) staff       (20)     2085 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      498 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/application.py
+-rw-r--r--   0 betterme   (501) staff       (20)    17006 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/archive.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4960 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/audio.py
+-rw-r--r--   0 betterme   (501) staff       (20)      647 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7513 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/document.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2924 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/font.py
+-rw-r--r--   0 betterme   (501) staff       (20)     9130 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)      958 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/isobmff.py
+-rw-r--r--   0 betterme   (501) staff       (20)     5371 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/video.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2089 2023-05-18 08:40:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      694 2024-04-22 08:58:46.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype.py
+-rw-r--r--   0 betterme   (501) staff       (20)      639 2023-08-10 05:04:53.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4037 2023-07-17 10:15:11.000000 MeUtils-2024.4.24.9.41.8/meutils/fileparser/表格抽取.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2393 2023-04-04 15:30:40.000000 MeUtils-2024.4.24.9.41.8/meutils/hash_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)      969 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/import_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.418306 MeUtils-2024.4.24.9.41.8/meutils/init/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-04-27 08:58:17.000000 MeUtils-2024.4.24.9.41.8/meutils/init/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1588 2023-08-07 08:26:31.000000 MeUtils-2024.4.24.9.41.8/meutils/init/evn.py
+-rw-r--r--   0 betterme   (501) staff       (20)    12884 2023-07-06 01:18:39.000000 MeUtils-2024.4.24.9.41.8/meutils/init/oo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.420050 MeUtils-2024.4.24.9.41.8/meutils/io/
+-rw-r--r--   0 betterme   (501) staff       (20)     2107 2023-04-13 02:51:32.000000 MeUtils-2024.4.24.9.41.8/meutils/io/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      409 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/io/file.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3038 2024-04-22 08:24:23.000000 MeUtils-2024.4.24.9.41.8/meutils/io/image.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1274 2024-02-05 09:39:04.000000 MeUtils-2024.4.24.9.41.8/meutils/io/minio_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8605 2023-06-26 01:26:21.000000 MeUtils-2024.4.24.9.41.8/meutils/io/tf_io.py
+-rw-r--r--   0 betterme   (501) staff       (20)      708 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/jinja_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.421601 MeUtils-2024.4.24.9.41.8/meutils/logging/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-15 06:07:38.000000 MeUtils-2024.4.24.9.41.8/meutils/logging/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      701 2023-08-21 08:23:51.000000 MeUtils-2024.4.24.9.41.8/meutils/logging/handlers.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2937 2023-08-15 01:04:50.000000 MeUtils-2024.4.24.9.41.8/meutils/logging/log_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6183 2024-02-08 00:37:38.000000 MeUtils-2024.4.24.9.41.8/meutils/logging/logger.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.424115 MeUtils-2024.4.24.9.41.8/meutils/notice/
+-rw-r--r--   0 betterme   (501) staff       (20)      248 2023-08-30 03:57:39.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2403 2023-10-16 09:04:49.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/emails.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2411 2024-04-22 11:17:05.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/feishu.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/file_post.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7331 2023-09-12 01:53:53.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/load_emailfile - 副本.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4207 2024-03-06 06:10:50.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3215 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/wechat_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6983 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/wecom.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1102 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/notice/weekmeet.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3559 2023-08-14 09:47:22.000000 MeUtils-2024.4.24.9.41.8/meutils/np_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.425673 MeUtils-2024.4.24.9.41.8/meutils/office_automation/
+-rw-r--r--   0 betterme   (501) staff       (20)      241 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/office_automation/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      508 2023-03-27 04:08:21.000000 MeUtils-2024.4.24.9.41.8/meutils/office_automation/doc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1528 2023-07-25 10:06:46.000000 MeUtils-2024.4.24.9.41.8/meutils/office_automation/pdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11894 2023-03-20 03:17:38.000000 MeUtils-2024.4.24.9.41.8/meutils/office_automation/pdm.py
+-rw-r--r--   0 betterme   (501) staff       (20)    13502 2023-03-21 06:30:39.000000 MeUtils-2024.4.24.9.41.8/meutils/office_automation/pdm_run.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.425953 MeUtils-2024.4.24.9.41.8/meutils/office_automation/report/
+-rw-r--r--   0 betterme   (501) staff       (20)      244 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/office_automation/report/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.426638 MeUtils-2024.4.24.9.41.8/meutils/oss/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2024-03-14 09:54:51.000000 MeUtils-2024.4.24.9.41.8/meutils/oss/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4500 2024-03-18 03:06:05.000000 MeUtils-2024.4.24.9.41.8/meutils/oss/minio_oss.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1274 2024-02-05 09:39:04.000000 MeUtils-2024.4.24.9.41.8/meutils/oss/minio_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.427876 MeUtils-2024.4.24.9.41.8/meutils/other/
+-rw-r--r--   0 betterme   (501) staff       (20)      996 2023-07-04 01:28:59.000000 MeUtils-2024.4.24.9.41.8/meutils/other/__demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/other/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.429805 MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/
+-rw-r--r--   0 betterme   (501) staff       (20)      416 2023-07-04 01:05:39.000000 MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)       22 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/__version__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7835 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/core.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11688 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/pool.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2573 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1037 2023-07-04 01:01:15.000000 MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/types.py
+-rw-r--r--   0 betterme   (501) staff       (20)    23121 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/other/besttable.py
+-rw-r--r--   0 betterme   (501) staff       (20)    44366 2023-03-21 05:16:40.000000 MeUtils-2024.4.24.9.41.8/meutils/other/crontab.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.430519 MeUtils-2024.4.24.9.41.8/meutils/pandas_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/pandas_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1228 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/pandas_utils/opt.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6300 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/pandas_utils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2846 2023-04-13 02:51:32.000000 MeUtils-2024.4.24.9.41.8/meutils/path_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6084 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/pd_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)    10133 2023-11-27 09:25:49.000000 MeUtils-2024.4.24.9.41.8/meutils/pipe.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.431341 MeUtils-2024.4.24.9.41.8/meutils/playwright_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2024-01-02 10:44:47.000000 MeUtils-2024.4.24.9.41.8/meutils/playwright_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2024-01-18 03:09:30.000000 MeUtils-2024.4.24.9.41.8/meutils/playwright_utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3145 2024-01-05 03:48:40.000000 MeUtils-2024.4.24.9.41.8/meutils/playwright_utils/reload.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.433647 MeUtils-2024.4.24.9.41.8/meutils/plots/
+-rw-r--r--   0 betterme   (501) staff       (20)      276 2023-09-12 02:56:35.000000 MeUtils-2024.4.24.9.41.8/meutils/plots/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2022 2023-09-12 02:59:23.000000 MeUtils-2024.4.24.9.41.8/meutils/plots/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)      732 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/plots/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2611 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/plots/echarts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11980 2023-05-09 07:49:05.000000 MeUtils-2024.4.24.9.41.8/meutils/plots/embedding_plot.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3610 2023-04-24 07:54:55.000000 MeUtils-2024.4.24.9.41.8/meutils/plots/mecharts.py
+-rw-r--r--   0 betterme   (501) staff       (20)    19326 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/plots/metrics.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2449 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/plots/plot_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.434850 MeUtils-2024.4.24.9.41.8/meutils/queues/
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-07-20 02:35:53.000000 MeUtils-2024.4.24.9.41.8/meutils/queues/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1735 2023-12-06 09:14:18.000000 MeUtils-2024.4.24.9.41.8/meutils/queues/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1491 2024-03-22 07:55:29.000000 MeUtils-2024.4.24.9.41.8/meutils/queues/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3270 2024-04-11 01:15:50.000000 MeUtils-2024.4.24.9.41.8/meutils/queues/smooth_queue.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1564 2024-03-22 09:12:23.000000 MeUtils-2024.4.24.9.41.8/meutils/queues/uniform_queue.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.437404 MeUtils-2024.4.24.9.41.8/meutils/request_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     3375 2023-07-27 05:15:39.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1894 2023-11-03 02:19:03.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/a爬虫.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1503 2023-04-21 05:45:54.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/crawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1767 2023-03-30 02:00:48.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/download.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/results.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3057 2023-12-04 10:37:44.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/tiangong.py
+-rw-r--r--   0 betterme   (501) staff       (20)      417 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/wechat.py
+-rw-r--r--   0 betterme   (501) staff       (20)      646 2023-11-22 01:02:28.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/公网ip.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1735 2024-01-17 05:19:28.000000 MeUtils-2024.4.24.9.41.8/meutils/request_utils/爬虫.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.437904 MeUtils-2024.4.24.9.41.8/meutils/schemas/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-24 06:44:44.000000 MeUtils-2024.4.24.9.41.8/meutils/schemas/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      484 2023-08-25 03:48:09.000000 MeUtils-2024.4.24.9.41.8/meutils/schemas/baidu_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.438391 MeUtils-2024.4.24.9.41.8/meutils/serving/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 02:50:45.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2478 2023-05-11 08:02:45.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/_fastapi.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.439913 MeUtils-2024.4.24.9.41.8/meutils/serving/celery/
+-rw-r--r--   0 betterme   (501) staff       (20)      628 2023-08-04 02:38:19.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/celery/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2109 2023-08-04 05:36:36.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/celery/_conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      514 2023-08-04 06:55:40.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/celery/_demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      415 2023-08-04 07:01:12.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/celery/_run_fastapi.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1126 2023-11-08 05:27:33.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/celery/router.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1465 2023-08-04 07:31:09.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/celery/tasks.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.441053 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.441534 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-29 01:58:15.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1444 2023-06-01 01:17:23.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/__demo/异步任务.py
+-rw-r--r--   0 betterme   (501) staff       (20)      290 2023-05-26 07:01:26.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3897 2024-01-18 03:22:23.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.442004 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/dependencies/
+-rw-r--r--   0 betterme   (501) staff       (20)      272 2023-12-19 09:14:44.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/dependencies/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      369 2023-12-19 09:14:44.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/dependencies/auth.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.442682 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/exceptions/
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-05-25 10:51:34.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/exceptions/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      509 2024-03-14 10:06:19.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/exceptions/http_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)      825 2023-05-25 10:51:34.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/exceptions/validation_error.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7791 2024-02-22 02:14:50.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/gunicorn.conf.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.444009 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2024-01-09 00:52:27.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      546 2024-01-09 01:09:19.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1440 2024-01-09 01:03:15.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/scheduler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      544 2024-01-09 01:00:29.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/shutdown.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1197 2024-01-18 08:10:48.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/spider.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2994 2024-03-14 10:39:22.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.444753 MeUtils-2024.4.24.9.41.8/meutils/serving/gui/
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-18 07:29:22.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/gui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1690 2024-01-24 01:49:04.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/gui/bar.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1273 2023-04-18 07:21:04.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/gui/demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.445026 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.446822 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      889 2023-06-06 10:44:06.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/client.py
+-rw-r--r--   0 betterme   (501) staff       (20)      926 2023-07-24 06:13:28.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/s.py
+-rw-r--r--   0 betterme   (501) staff       (20)      953 2023-07-24 06:17:01.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/s2.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2113 2023-07-24 06:04:10.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/server.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1160 2023-07-19 06:57:16.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/test.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-16 11:10:26.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.448189 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/
+-rw-r--r--   0 betterme   (501) staff       (20)     1805 2023-06-07 05:33:04.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/SentenceEncoder.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1831 2023-07-17 10:23:25.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/SentenceEncoder_.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1384 2023-06-06 11:14:22.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1093 2023-07-24 06:57:00.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/base.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.448717 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/nlp_serving/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-17 01:14:50.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/nlp_serving/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1079 2023-06-06 07:52:01.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/jina/nlp_serving/word_segmentation.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.448971 MeUtils-2024.4.24.9.41.8/meutils/serving/rq/
+-rw-r--r--   0 betterme   (501) staff       (20)      321 2023-11-08 05:10:21.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/rq/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.450396 MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-09-20 06:06:45.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      931 2023-12-04 10:19:52.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/_test.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3887 2023-11-21 03:52:24.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/chat_latex.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6930 2024-03-25 05:38:12.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1427 2023-11-03 05:24:48.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/demo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.451218 MeUtils-2024.4.24.9.41.8/meutils/serving/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)     1757 2023-08-23 04:01:26.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/webui/_2_词性标注与实体识别.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-05-21 09:09:55.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      509 2023-08-23 04:01:26.000000 MeUtils-2024.4.24.9.41.8/meutils/serving/webui/_🏆_主页.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.451947 MeUtils-2024.4.24.9.41.8/meutils/settings/
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-08-21 06:24:50.000000 MeUtils-2024.4.24.9.41.8/meutils/settings/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      264 2023-08-21 06:29:43.000000 MeUtils-2024.4.24.9.41.8/meutils/settings/base.py
+-rw-r--r--   0 betterme   (501) staff       (20)      484 2023-08-21 06:31:48.000000 MeUtils-2024.4.24.9.41.8/meutils/settings/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      956 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/sftp.py
+-rw-r--r--   0 betterme   (501) staff       (20)      796 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/sk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1400 2023-08-25 08:16:40.000000 MeUtils-2024.4.24.9.41.8/meutils/smooth_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.452150 MeUtils-2024.4.24.9.41.8/meutils/spark/
+-rw-r--r--   0 betterme   (501) staff       (20)      576 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/spark/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.452930 MeUtils-2024.4.24.9.41.8/meutils/str_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)     1258 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/str_utils/Translator.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6697 2023-12-22 01:04:55.000000 MeUtils-2024.4.24.9.41.8/meutils/str_utils/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.453676 MeUtils-2024.4.24.9.41.8/meutils/str_utils/__translater/
+-rw-r--r--   0 betterme   (501) staff       (20)      277 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/str_utils/__translater/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1408 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/str_utils/__translater/tencent.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1238 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/str_utils/__translater/translater.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1168 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/str_utils/__translater/youdao.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1095 2023-06-12 09:51:25.000000 MeUtils-2024.4.24.9.41.8/meutils/str_utils/json_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2701 2024-04-23 03:08:58.000000 MeUtils-2024.4.24.9.41.8/meutils/str_utils/regular_expression.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.454426 MeUtils-2024.4.24.9.41.8/meutils/tasks/
+-rw-r--r--   0 betterme   (501) staff       (20)      280 2023-11-08 05:13:34.000000 MeUtils-2024.4.24.9.41.8/meutils/tasks/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      627 2023-11-08 05:23:51.000000 MeUtils-2024.4.24.9.41.8/meutils/tasks/common.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.458542 MeUtils-2024.4.24.9.41.8/meutils/templates/
+-rw-r--r--   0 betterme   (501) staff       (20)      349 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      291 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      224 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/demo.conf
+-rw-r--r--   0 betterme   (501) staff       (20)      578 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/demo.j2
+-rw-r--r--   0 betterme   (501) staff       (20)      808 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/demo.py
+-rw-r--r--   0 betterme   (501) staff       (20)      536 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/demox.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2416 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/df_html.j2
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.460784 MeUtils-2024.4.24.9.41.8/meutils/templates/dockerfiles/
+-rw-r--r--   0 betterme   (501) staff       (20)      112 2023-03-21 05:16:40.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/dockerfiles/Dockerfile
+-rw-r--r--   0 betterme   (501) staff       (20)      170 2023-03-21 05:16:40.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/dockerfiles/Dockerfile_me
+-rw-r--r--   0 betterme   (501) staff       (20)      217 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/dockerfiles/Dockerfile_milvus
+-rw-r--r--   0 betterme   (501) staff       (20)      245 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/dockerfiles/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      712 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/dockerfiles/docker_build_push.py
+-rwxr-xr-x   0 betterme   (501) staff       (20)      386 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/dockerfiles/docker_push.sh
+-rw-r--r--   0 betterme   (501) staff       (20)     2266 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/hegui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      540 2023-06-29 07:13:14.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/markmap.html
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.460934 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/
+-rw-r--r--   0 betterme   (501) staff       (20)      831 2022-05-05 05:21:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/cookiecutter.json
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.464525 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.editorconfig
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.464700 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/
+-rw-r--r--   0 betterme   (501) staff       (20)      342 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1198 2023-05-31 00:59:56.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      842 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      178 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     4010 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     5987 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      351 2021-09-04 06:53:23.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2516 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      704 2023-04-18 10:20:21.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)     1738 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.466956 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      632 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)      702 2021-09-14 08:44:31.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2022-04-18 06:25:28.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     5157 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      388 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1410 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      829 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      117 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/usage.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.467188 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/
+-rw-r--r--   0 betterme   (501) staff       (20)      234 2021-09-04 07:26:59.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/examples/demo.py
+-rwxr--r--   0 betterme   (501) staff       (20)      244 2022-05-05 05:24:52.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2021-09-01 08:44:34.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/requirements_dev.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      549 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2532 2022-04-19 09:34:52.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.467535 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       61 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2315 2021-09-03 02:32:04.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)      678 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.467930 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2022-04-18 06:39:54.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.468468 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2021-08-31 05:12:27.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2022-04-27 09:56:07.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      591 2022-04-27 09:56:07.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)       19 2021-09-03 02:19:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11496 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/tpl.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      537 2023-06-29 07:15:57.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/x.html
+-rw-r--r--   0 betterme   (501) staff       (20)   172819 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/templates/合规日报模板.docx
+-rw-r--r--   0 betterme   (501) staff       (20)      590 2023-05-08 05:49:55.000000 MeUtils-2024.4.24.9.41.8/meutils/todo.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2024-04-24 01:41:08.469541 MeUtils-2024.4.24.9.41.8/meutils/tools/
+-rw-r--r--   0 betterme   (501) staff       (20)      242 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/tools/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1383 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/tools/cprint.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2392 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/tools/machine_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1064 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/tools/seize.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1255 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/tools/service_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      429 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/tools/sys_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)      997 2024-04-22 10:50:36.000000 MeUtils-2024.4.24.9.41.8/meutils/tools/token_monitor.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1127 2023-12-11 10:37:26.000000 MeUtils-2024.4.24.9.41.8/meutils/types.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2438 2023-03-20 02:44:39.000000 MeUtils-2024.4.24.9.41.8/meutils/zk_utils.py
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2024-04-24 01:41:08.474062 MeUtils-2024.4.24.9.41.8/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     2466 2023-11-29 08:25:30.000000 MeUtils-2024.4.24.9.41.8/setup.py
```

### Comparing `MeUtils-2024.4.24.15.17.56/LICENSE` & `MeUtils-2024.4.24.9.41.8/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/PKG-INFO` & `MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2024.4.24.15.17.56
+Version: 2024.4.24.9.41.8
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
@@ -98,50 +98,50 @@
 Requires-Dist: sqlalchemy; extra == "db"
 Provides-Extra: pd
 Requires-Dist: dataframe_image; extra == "pd"
 Requires-Dist: pandas-profiling[notebook]; extra == "pd"
 Requires-Dist: pandas_summary; extra == "pd"
 Requires-Dist: polars; extra == "pd"
 Provides-Extra: all
+Requires-Dist: sse_starlette; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: fastapi[all]; extra == "all"
-Requires-Dist: iteration_utilities; extra == "all"
-Requires-Dist: pretty_errors; extra == "all"
 Requires-Dist: cachetools; extra == "all"
-Requires-Dist: redis-py-cluster; extra == "all"
-Requires-Dist: fastapi; extra == "all"
-Requires-Dist: thriftpy2; extra == "all"
 Requires-Dist: asyncmy; extra == "all"
-Requires-Dist: faiss-cpu; extra == "all"
-Requires-Dist: pandas-profiling[notebook]; extra == "all"
-Requires-Dist: sse_starlette; extra == "all"
-Requires-Dist: langchain; extra == "all"
-Requires-Dist: schedule; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: thefuck; extra == "all"
-Requires-Dist: dataframe_image; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: jmespath; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: geopy; extra == "all"
 Requires-Dist: streamlit; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: pretty_errors; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
 Requires-Dist: sqlalchemy; extra == "all"
+Requires-Dist: faiss-cpu; extra == "all"
 Requires-Dist: pymysql; extra == "all"
 Requires-Dist: pandas_summary; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: simplejson; extra == "all"
-Requires-Dist: filetype; extra == "all"
+Requires-Dist: dataframe_image; extra == "all"
+Requires-Dist: redis-py-cluster; extra == "all"
+Requires-Dist: missingno; extra == "all"
 Requires-Dist: pymongo; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: reportlab; extra == "all"
-Requires-Dist: geopy; extra == "all"
+Requires-Dist: polars; extra == "all"
+Requires-Dist: filetype; extra == "all"
+Requires-Dist: thriftpy2; extra == "all"
+Requires-Dist: jieba; extra == "all"
 Requires-Dist: pymupd; extra == "all"
-Requires-Dist: missingno; extra == "all"
+Requires-Dist: pandas-profiling[notebook]; extra == "all"
+Requires-Dist: iteration_utilities; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: reportlab; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: simplejson; extra == "all"
 Requires-Dist: gunicorn; extra == "all"
-Requires-Dist: jmespath; extra == "all"
-Requires-Dist: jieba; extra == "all"
-Requires-Dist: polars; extra == "all"
+Requires-Dist: langchain; extra == "all"
+Requires-Dist: fastapi; extra == "all"
 
 [![Downloads](http://pepy.tech/badge/meutils)](http://pepy.tech/project/meutils)
 
 <h1 align = "center">:rocket: 常用工具类 :facepunch:</h1>
 
 ## Install
 ```bash
```

### Comparing `MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/SOURCES.txt` & `MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -166,18 +166,14 @@
 meutils/init/evn.py
 meutils/init/oo.py
 meutils/io/__init__.py
 meutils/io/file.py
 meutils/io/image.py
 meutils/io/minio_utils.py
 meutils/io/tf_io.py
-meutils/llm/__init__.py
-meutils/llm/demo.py
-meutils/llm/functions/__init__.py
-meutils/llm/output_parsers/__init__.py
 meutils/logging/__init__.py
 meutils/logging/handlers.py
 meutils/logging/log_utils.py
 meutils/logging/logger.py
 meutils/notice/__init__.py
 meutils/notice/emails.py
 meutils/notice/feishu.py
```

### Comparing `MeUtils-2024.4.24.15.17.56/MeUtils.egg-info/requires.txt` & `MeUtils-2024.4.24.9.41.8/MeUtils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -35,50 +35,50 @@
 uvicorn
 gunicorn
 sse_starlette
 openai
 langchain
 
 [all]
+sse_starlette
+pyarrow
 fastapi[all]
-iteration_utilities
-pretty_errors
 cachetools
-redis-py-cluster
-fastapi
-thriftpy2
 asyncmy
-faiss-cpu
-pandas-profiling[notebook]
-sse_starlette
-langchain
-schedule
-pyarrow
 thefuck
-dataframe_image
+jinja2
+jmespath
+seaborn
+geopy
 streamlit
+pymilvus
+pretty_errors
+uvicorn
 sqlalchemy
+faiss-cpu
 pymysql
 pandas_summary
-openai
-simplejson
-filetype
+dataframe_image
+redis-py-cluster
+missingno
 pymongo
-seaborn
-uvicorn
-jinja2
-pymilvus
-reportlab
-geopy
+polars
+filetype
+thriftpy2
+jieba
 pymupd
-missingno
+pandas-profiling[notebook]
+iteration_utilities
+openai
+reportlab
+schedule
+simplejson
 gunicorn
-jmespath
-jieba
-polars
+langchain
+fastapi
 
 [ann]
 pymilvus
 faiss-cpu
 
 [app]
 fastapi[all]
```

### Comparing `MeUtils-2024.4.24.15.17.56/PKG-INFO` & `MeUtils-2024.4.24.9.41.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeUtils
-Version: 2024.4.24.15.17.56
+Version: 2024.4.24.9.41.8
 Summary: description
 Home-page: https://github.com/yuanjie-ai/MeUtils
 Author: yuanjie
 Author-email: 313303303@qq.com
 Maintainer: yuanjie
 Maintainer-email: 313303303@qq.com
 License: MIT License
@@ -98,50 +98,50 @@
 Requires-Dist: sqlalchemy; extra == "db"
 Provides-Extra: pd
 Requires-Dist: dataframe_image; extra == "pd"
 Requires-Dist: pandas-profiling[notebook]; extra == "pd"
 Requires-Dist: pandas_summary; extra == "pd"
 Requires-Dist: polars; extra == "pd"
 Provides-Extra: all
+Requires-Dist: sse_starlette; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: fastapi[all]; extra == "all"
-Requires-Dist: iteration_utilities; extra == "all"
-Requires-Dist: pretty_errors; extra == "all"
 Requires-Dist: cachetools; extra == "all"
-Requires-Dist: redis-py-cluster; extra == "all"
-Requires-Dist: fastapi; extra == "all"
-Requires-Dist: thriftpy2; extra == "all"
 Requires-Dist: asyncmy; extra == "all"
-Requires-Dist: faiss-cpu; extra == "all"
-Requires-Dist: pandas-profiling[notebook]; extra == "all"
-Requires-Dist: sse_starlette; extra == "all"
-Requires-Dist: langchain; extra == "all"
-Requires-Dist: schedule; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: thefuck; extra == "all"
-Requires-Dist: dataframe_image; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: jmespath; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: geopy; extra == "all"
 Requires-Dist: streamlit; extra == "all"
+Requires-Dist: pymilvus; extra == "all"
+Requires-Dist: pretty_errors; extra == "all"
+Requires-Dist: uvicorn; extra == "all"
 Requires-Dist: sqlalchemy; extra == "all"
+Requires-Dist: faiss-cpu; extra == "all"
 Requires-Dist: pymysql; extra == "all"
 Requires-Dist: pandas_summary; extra == "all"
-Requires-Dist: openai; extra == "all"
-Requires-Dist: simplejson; extra == "all"
-Requires-Dist: filetype; extra == "all"
+Requires-Dist: dataframe_image; extra == "all"
+Requires-Dist: redis-py-cluster; extra == "all"
+Requires-Dist: missingno; extra == "all"
 Requires-Dist: pymongo; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: uvicorn; extra == "all"
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: pymilvus; extra == "all"
-Requires-Dist: reportlab; extra == "all"
-Requires-Dist: geopy; extra == "all"
+Requires-Dist: polars; extra == "all"
+Requires-Dist: filetype; extra == "all"
+Requires-Dist: thriftpy2; extra == "all"
+Requires-Dist: jieba; extra == "all"
 Requires-Dist: pymupd; extra == "all"
-Requires-Dist: missingno; extra == "all"
+Requires-Dist: pandas-profiling[notebook]; extra == "all"
+Requires-Dist: iteration_utilities; extra == "all"
+Requires-Dist: openai; extra == "all"
+Requires-Dist: reportlab; extra == "all"
+Requires-Dist: schedule; extra == "all"
+Requires-Dist: simplejson; extra == "all"
 Requires-Dist: gunicorn; extra == "all"
-Requires-Dist: jmespath; extra == "all"
-Requires-Dist: jieba; extra == "all"
-Requires-Dist: polars; extra == "all"
+Requires-Dist: langchain; extra == "all"
+Requires-Dist: fastapi; extra == "all"
 
 [![Downloads](http://pepy.tech/badge/meutils)](http://pepy.tech/project/meutils)
 
 <h1 align = "center">:rocket: 常用工具类 :facepunch:</h1>
 
 ## Install
 ```bash
```

### Comparing `MeUtils-2024.4.24.15.17.56/README.md` & `MeUtils-2024.4.24.9.41.8/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/adjusted_audio1.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/adjusted_audio1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/fast_asr.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/fast_asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/openai_asr.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/openai_asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr/xunfei_asr.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr/xunfei_asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/asr.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/fast_asr.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/fast_asr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts/EdgeTTS.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts/EdgeTTS.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts/openai_tts.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts/openai_tts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts/tts_ui.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts/tts_ui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/tts.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/tts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_audio/utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_audio/utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_cv/doc_prompt.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_cv/doc_prompt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_cv/latex_ocr.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_cv/latex_ocr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_cv/ocr.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_cv/ocr.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_cv/ocr_api.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_cv/ocr_api.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/SplitSentence.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/SplitSentence.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/Untitled-1(1).py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/Untitled-1(1).py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/_lda.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/_lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/_textsplitter/chinese_text_splitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/_textsplitter/text_split.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/_textsplitter/text_split.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/lda.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/lda.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/ner.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/ner.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/text_transformer.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/text_transformer.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/textsplitter.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/textsplitter.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_nlp/word_segmentation.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_nlp/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_video/avmerge.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_video/avmerge.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_video/avmerge_.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_video/avmerge_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_video/scene_detect.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_video/scene_detect.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_video/test.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_video/test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_video/video.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_video/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ai_video/xx.py` & `MeUtils-2024.4.24.9.41.8/meutils/ai_video/xx.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ann/ann.py` & `MeUtils-2024.4.24.9.41.8/meutils/ann/ann.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ann/ann_faiss.py` & `MeUtils-2024.4.24.9.41.8/meutils/ann/ann_faiss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ann/ann_gensim.py` & `MeUtils-2024.4.24.9.41.8/meutils/ann/ann_gensim.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ann/ann_inmemory.py` & `MeUtils-2024.4.24.9.41.8/meutils/ann/ann_inmemory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ann/ann_service.py` & `MeUtils-2024.4.24.9.41.8/meutils/ann/ann_service.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ann/ann_v1.py` & `MeUtils-2024.4.24.9.41.8/meutils/ann/ann_v1.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ann/cli.py` & `MeUtils-2024.4.24.9.41.8/meutils/ann/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/ann/shake_demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/ann/shake_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/api/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/api/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/api/deeplx.py` & `MeUtils-2024.4.24.9.41.8/meutils/api/deeplx.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/async_utils/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/async_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/cache_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/cache_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/browser.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/browser.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/cli.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/conf.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/cron.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/cron.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/gunicorn.conf.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/monitor.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/nesc.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/nesc.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/notice.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/notice.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/clis/server.py` & `MeUtils-2024.4.24.9.41.8/meutils/clis/server.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/cmds/hdfs_cmd.py` & `MeUtils-2024.4.24.9.41.8/meutils/cmds/hdfs_cmd.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/cmds/subprocess_demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/cmds/subprocess_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/coding/find132.py` & `MeUtils-2024.4.24.9.41.8/meutils/coding/find132.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/comp_utils/reverse_metric.py` & `MeUtils-2024.4.24.9.41.8/meutils/comp_utils/reverse_metric.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/config_utils/nacos.py` & `MeUtils-2024.4.24.9.41.8/meutils/config_utils/nacos.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/data/SimHei.ttf` & `MeUtils-2024.4.24.9.41.8/meutils/data/SimHei.ttf`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/data/coordinate.py` & `MeUtils-2024.4.24.9.41.8/meutils/data/coordinate.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/date_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/date_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/db/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/db/mongo.py` & `MeUtils-2024.4.24.9.41.8/meutils/db/mongo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/db/neo4j.py` & `MeUtils-2024.4.24.9.41.8/meutils/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/__ai.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/__ai.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/cache.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/cache.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/catch.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/catch.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/contextmanagers.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/decorator.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/decorator_demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/decorator_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/fastapi_decorator.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/fastapi_decorator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/feishu.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/retry.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/retry.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/scheduler.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/decorators/schedulers.py` & `MeUtils-2024.4.24.9.41.8/meutils/decorators/schedulers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/dist_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/dist_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/demo_es.py` & `MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/demo_es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/demo_hnsw.py` & `MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/demo_hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/in_memory.py` & `MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/in_memory.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/docarray_utils/改造下hnsw.py` & `MeUtils-2024.4.24.9.41.8/meutils/docarray_utils/改造下hnsw.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/easy_search/es.py` & `MeUtils-2024.4.24.9.41.8/meutils/easy_search/es.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/PDF抽取.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/PDF抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/__main__.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/__main__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/filetype.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/filetype.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/helpers.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/helpers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/match.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/match.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/archive.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/archive.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/audio.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/audio.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/base.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/document.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/document.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/font.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/font.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/image.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/isobmff.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/isobmff.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/types/video.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/types/video.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype/utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype/utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/filetype.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/filetype.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/pdf.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/fileparser/表格抽取.py` & `MeUtils-2024.4.24.9.41.8/meutils/fileparser/表格抽取.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/hash_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/import_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/import_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/init/evn.py` & `MeUtils-2024.4.24.9.41.8/meutils/init/evn.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/init/oo.py` & `MeUtils-2024.4.24.9.41.8/meutils/init/oo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/io/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/io/image.py` & `MeUtils-2024.4.24.9.41.8/meutils/io/image.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/io/minio_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/io/minio_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/io/tf_io.py` & `MeUtils-2024.4.24.9.41.8/meutils/io/tf_io.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/jinja_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/jinja_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/logging/handlers.py` & `MeUtils-2024.4.24.9.41.8/meutils/logging/handlers.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/logging/log_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/logging/log_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/logging/logger.py` & `MeUtils-2024.4.24.9.41.8/meutils/logging/logger.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/notice/emails.py` & `MeUtils-2024.4.24.9.41.8/meutils/notice/emails.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/notice/feishu.py` & `MeUtils-2024.4.24.9.41.8/meutils/notice/feishu.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/notice/file_post.py` & `MeUtils-2024.4.24.9.41.8/meutils/notice/file_post.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/notice/load_emailfile - 副本.py` & `MeUtils-2024.4.24.9.41.8/meutils/notice/load_emailfile - 副本.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/notice/wechat.py` & `MeUtils-2024.4.24.9.41.8/meutils/notice/wechat.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/notice/wechat_.py` & `MeUtils-2024.4.24.9.41.8/meutils/notice/wechat_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/notice/wecom.py` & `MeUtils-2024.4.24.9.41.8/meutils/notice/wecom.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/notice/weekmeet.py` & `MeUtils-2024.4.24.9.41.8/meutils/notice/weekmeet.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/np_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/np_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/office_automation/pdf.py` & `MeUtils-2024.4.24.9.41.8/meutils/office_automation/pdf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/office_automation/pdm.py` & `MeUtils-2024.4.24.9.41.8/meutils/office_automation/pdm.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/office_automation/pdm_run.py` & `MeUtils-2024.4.24.9.41.8/meutils/office_automation/pdm_run.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/oss/minio_oss.py` & `MeUtils-2024.4.24.9.41.8/meutils/oss/minio_oss.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/oss/minio_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/oss/minio_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/other/__demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/other/__demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/core.py` & `MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/core.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/pool.py` & `MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/pool.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/scheduler.py` & `MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/other/aiomultiprocess/types.py` & `MeUtils-2024.4.24.9.41.8/meutils/other/aiomultiprocess/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/other/besttable.py` & `MeUtils-2024.4.24.9.41.8/meutils/other/besttable.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/other/crontab.py` & `MeUtils-2024.4.24.9.41.8/meutils/other/crontab.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/pandas_utils/opt.py` & `MeUtils-2024.4.24.9.41.8/meutils/pandas_utils/opt.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/pandas_utils/pd_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/pandas_utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/path_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/path_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/pd_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/pipe.py` & `MeUtils-2024.4.24.9.41.8/meutils/pipe.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/playwright_utils/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/playwright_utils/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/playwright_utils/reload.py` & `MeUtils-2024.4.24.9.41.8/meutils/playwright_utils/reload.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/plots/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/plots/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/plots/demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/plots/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/plots/echarts.py` & `MeUtils-2024.4.24.9.41.8/meutils/plots/echarts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/plots/embedding_plot.py` & `MeUtils-2024.4.24.9.41.8/meutils/plots/embedding_plot.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/plots/mecharts.py` & `MeUtils-2024.4.24.9.41.8/meutils/plots/mecharts.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/plots/metrics.py` & `MeUtils-2024.4.24.9.41.8/meutils/plots/metrics.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/plots/plot_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/plots/plot_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/queues/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/queues/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/queues/demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/queues/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/queues/smooth_queue.py` & `MeUtils-2024.4.24.9.41.8/meutils/queues/smooth_queue.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/queues/uniform_queue.py` & `MeUtils-2024.4.24.9.41.8/meutils/queues/uniform_queue.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/request_utils/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/request_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/request_utils/a爬虫.py` & `MeUtils-2024.4.24.9.41.8/meutils/request_utils/a爬虫.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/request_utils/crawler.py` & `MeUtils-2024.4.24.9.41.8/meutils/request_utils/crawler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/request_utils/download.py` & `MeUtils-2024.4.24.9.41.8/meutils/request_utils/download.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/request_utils/results.py` & `MeUtils-2024.4.24.9.41.8/meutils/request_utils/results.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/request_utils/tiangong.py` & `MeUtils-2024.4.24.9.41.8/meutils/request_utils/tiangong.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/request_utils/公网ip.py` & `MeUtils-2024.4.24.9.41.8/meutils/request_utils/公网ip.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/request_utils/爬虫.py` & `MeUtils-2024.4.24.9.41.8/meutils/request_utils/爬虫.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/_fastapi.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/_fastapi.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/celery/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/celery/_conf.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/celery/_conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/celery/_demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/celery/_demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/celery/router.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/celery/router.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/celery/tasks.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/celery/tasks.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/__demo/异步任务.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/__demo/异步任务.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/exceptions/validation_error.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/exceptions/validation_error.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/gunicorn.conf.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/_test.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/scheduler.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/scheduler.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/shutdown.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/shutdown.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/routers/spider.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/routers/spider.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/fastapi/utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/fastapi/utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/gui/bar.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/gui/bar.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/gui/demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/gui/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/client.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/client.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/s.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/s.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/s2.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/s2.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/server.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/server.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/__demo/test.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/__demo/test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/SentenceEncoder.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/SentenceEncoder.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/SentenceEncoder_.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/SentenceEncoder_.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/executors/base.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/executors/base.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/jina/nlp_serving/word_segmentation.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/jina/nlp_serving/word_segmentation.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/_test.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/_test.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/chat_latex.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/chat_latex.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/streamlit/demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/streamlit/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/serving/webui/_2_词性标注与实体识别.py` & `MeUtils-2024.4.24.9.41.8/meutils/serving/webui/_2_词性标注与实体识别.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/sftp.py` & `MeUtils-2024.4.24.9.41.8/meutils/sftp.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/sk_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/sk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/smooth_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/smooth_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/spark/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/spark/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/str_utils/Translator.py` & `MeUtils-2024.4.24.9.41.8/meutils/str_utils/Translator.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/str_utils/__init__.py` & `MeUtils-2024.4.24.9.41.8/meutils/str_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/str_utils/__translater/tencent.py` & `MeUtils-2024.4.24.9.41.8/meutils/str_utils/__translater/tencent.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/str_utils/__translater/translater.py` & `MeUtils-2024.4.24.9.41.8/meutils/str_utils/__translater/translater.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/str_utils/__translater/youdao.py` & `MeUtils-2024.4.24.9.41.8/meutils/str_utils/__translater/youdao.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/str_utils/json_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/str_utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/str_utils/regular_expression.py` & `MeUtils-2024.4.24.9.41.8/meutils/str_utils/regular_expression.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/tasks/common.py` & `MeUtils-2024.4.24.9.41.8/meutils/tasks/common.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/demo.j2` & `MeUtils-2024.4.24.9.41.8/meutils/templates/demo.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/demo.py` & `MeUtils-2024.4.24.9.41.8/meutils/templates/demo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/demox.py` & `MeUtils-2024.4.24.9.41.8/meutils/templates/demox.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/df_html.j2` & `MeUtils-2024.4.24.9.41.8/meutils/templates/df_html.j2`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/dockerfiles/docker_build_push.py` & `MeUtils-2024.4.24.9.41.8/meutils/templates/dockerfiles/docker_build_push.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/hegui.py` & `MeUtils-2024.4.24.9.41.8/meutils/templates/hegui.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/markmap.html` & `MeUtils-2024.4.24.9.41.8/meutils/templates/markmap.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/cookiecutter.json` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/.travis.yml`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/LICENSE`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/README.md`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/docs/make.bat`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.cfg`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tests/test_{{cookiecutter.project_slug}}.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py` & `MeUtils-2024.4.24.9.41.8/meutils/templates/pypackage/{{cookiecutter.project_slug}}/{{cookiecutter.project_slug}}/clis/cli.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/tpl.docx` & `MeUtils-2024.4.24.9.41.8/meutils/templates/tpl.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/x.html` & `MeUtils-2024.4.24.9.41.8/meutils/templates/x.html`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/templates/合规日报模板.docx` & `MeUtils-2024.4.24.9.41.8/meutils/templates/合规日报模板.docx`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/todo.py` & `MeUtils-2024.4.24.9.41.8/meutils/todo.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/tools/cprint.py` & `MeUtils-2024.4.24.9.41.8/meutils/tools/cprint.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/tools/machine_monitor.py` & `MeUtils-2024.4.24.9.41.8/meutils/tools/machine_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/tools/seize.py` & `MeUtils-2024.4.24.9.41.8/meutils/tools/seize.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/tools/service_monitor.py` & `MeUtils-2024.4.24.9.41.8/meutils/tools/service_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/tools/token_monitor.py` & `MeUtils-2024.4.24.9.41.8/meutils/tools/token_monitor.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/types.py` & `MeUtils-2024.4.24.9.41.8/meutils/types.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/meutils/zk_utils.py` & `MeUtils-2024.4.24.9.41.8/meutils/zk_utils.py`

 * *Files identical despite different names*

### Comparing `MeUtils-2024.4.24.15.17.56/setup.py` & `MeUtils-2024.4.24.9.41.8/setup.py`

 * *Files identical despite different names*

