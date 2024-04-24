# Comparing `tmp/byzerllm-0.1.8.tar.gz` & `tmp/byzerllm-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byzerllm-0.1.8.tar", last modified: Sat Oct 14 08:09:41 2023, max compression
+gzip compressed data, was "byzerllm-0.1.9.tar", last modified: Sat Oct 14 14:43:15 2023, max compression
```

## Comparing `byzerllm-0.1.8.tar` & `byzerllm-0.1.9.tar`

### file list

```diff
@@ -1,501 +1,502 @@
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.298790 byzerllm-0.1.8/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      762 2023-10-14 08:09:41.298790 byzerllm-0.1.8/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      449 2023-10-11 00:54:35.000000 byzerllm-0.1.8/README.md
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       38 2023-10-14 08:09:41.298790 byzerllm-0.1.8/setup.cfg
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1254 2023-05-15 03:02:58.000000 byzerllm-0.1.8/setup.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.258790 byzerllm-0.1.8/src/
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.262790 byzerllm-0.1.8/src/byzerllm/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3025 2023-09-11 11:02:01.000000 byzerllm-0.1.8/src/byzerllm/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.262790 byzerllm-0.1.8/src/byzerllm/alpha_moss/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29048 2023-07-07 08:01:34.000000 byzerllm-0.1.8/src/byzerllm/alpha_moss/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.262790 byzerllm-0.1.8/src/byzerllm/apps/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      466 2023-07-04 14:50:28.000000 byzerllm-0.1.8/src/byzerllm/apps/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3942 2023-09-06 06:02:21.000000 byzerllm-0.1.8/src/byzerllm/apps/builder.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3350 2023-09-06 06:06:45.000000 byzerllm-0.1.8/src/byzerllm/apps/client.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6276 2023-09-06 06:07:35.000000 byzerllm-0.1.8/src/byzerllm/apps/qa.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4934 2023-09-01 16:22:38.000000 byzerllm-0.1.8/src/byzerllm/apps/qa_strategy.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1687 2023-09-06 06:19:12.000000 byzerllm-0.1.8/src/byzerllm/apps/vector_db.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.262790 byzerllm-0.1.8/src/byzerllm/auto/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12154 2023-10-04 02:30:28.000000 byzerllm-0.1.8/src/byzerllm/auto/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7577 2023-07-31 02:07:12.000000 byzerllm-0.1.8/src/byzerllm/auto/backend_ds.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.262790 byzerllm-0.1.8/src/byzerllm/baichuan/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4018 2023-09-12 08:55:25.000000 byzerllm-0.1.8/src/byzerllm/baichuan/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.262790 byzerllm-0.1.8/src/byzerllm/bark/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-05-11 02:06:23.000000 byzerllm-0.1.8/src/byzerllm/bark/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4243 2023-05-11 02:06:23.000000 byzerllm-0.1.8/src/byzerllm/bark/api.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.258790 byzerllm-0.1.8/src/byzerllm/bark/assets/
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.274790 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16794 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/announcer.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29060 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20316 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35084 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31724 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    59348 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25116 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22180 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33860 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38124 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21220 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15516 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    13436 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35084 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18980 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35940 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27620 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25436 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27620 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26500 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24420 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34820 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18660 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22660 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30604 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29324 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51084 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31460 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36364 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44044 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43564 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    53908 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33060 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31244 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32580 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23036 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26820 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28684 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33004 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30020 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30180 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    46604 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45268 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    52684 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42764 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34180 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    41268 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29964 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35940 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25220 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44148 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24796 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37964 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22716 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24580 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33380 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    50548 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29540 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24156 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29004 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30500 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22180 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21916 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39780 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26500 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43084 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42284 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42548 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34020 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45324 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37380 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33380 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36364 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32420 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    58492 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35300 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    49004 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34444 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34020 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30284 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    58652 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1943 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/readme.md
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    57852 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24260 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51668 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29164 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27940 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45748 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25380 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42924 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38500 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19620 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21380 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19676 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    54548 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22556 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26020 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24156 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20100 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16100 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29220 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21276 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35724 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.286790 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39620 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27460 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24740 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30660 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23196 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40100 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28524 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51084 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28100 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25220 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26236 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34980 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23780 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24740 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25540 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22716 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23300 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30180 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22020 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25116 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26236 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23780 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25700 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22020 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25436 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19940 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45804 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25700 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    52204 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    50764 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    49908 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45108 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    55932 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32524 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43244 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32100 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32580 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25860 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27780 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29804 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25380 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51404 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29380 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39404 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28740 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33804 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40788 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28740 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30444 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29644 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43724 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42708 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37644 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24420 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31244 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24100 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26716 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40788 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25060 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20260 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31140 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26556 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26340 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19196 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39564 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23140 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23196 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27884 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31140 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23676 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34660 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28580 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    41428 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38180 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38820 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29060 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30980 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27724 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34500 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36844 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26980 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28260 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28100 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28524 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39780 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39884 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29220 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19940 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28204 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44628 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20476 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26020 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39084 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34660 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22076 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28684 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33164 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    17220 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25276 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20260 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28204 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20636 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19836 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21060 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29964 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    17436 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16900 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21060 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19300 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16156 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19620 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21380 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19676 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    54548 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22556 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3759 2023-08-26 08:52:44.000000 byzerllm-0.1.8/src/byzerllm/bark/bark_voice.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33373 2023-05-11 02:06:23.000000 byzerllm-0.1.8/src/byzerllm/bark/generation.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     9139 2023-05-11 02:06:23.000000 byzerllm-0.1.8/src/byzerllm/bark/model.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5955 2023-05-11 02:06:23.000000 byzerllm-0.1.8/src/byzerllm/bark/model_fine.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.286790 byzerllm-0.1.8/src/byzerllm/bge/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1022 2023-09-04 13:38:16.000000 byzerllm-0.1.8/src/byzerllm/bge/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.286790 byzerllm-0.1.8/src/byzerllm/chatglm2/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2108 2023-08-31 04:23:44.000000 byzerllm-0.1.8/src/byzerllm/chatglm2/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.286790 byzerllm-0.1.8/src/byzerllm/chatglm6b/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-04 03:55:05.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8182 2023-04-04 03:55:05.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/arguments.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21286 2023-05-04 08:53:10.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/finetune.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11575 2023-04-04 03:55:05.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/trainer_seq2seq.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.286790 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-05-06 13:50:22.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3000 2023-05-06 13:50:22.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/finetune.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1404 2023-05-12 05:48:30.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/infer.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.286790 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      277 2023-05-06 13:50:22.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16907 2023-05-06 13:50:22.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/common.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7620 2023-05-06 13:50:22.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/config.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6263 2023-05-06 13:50:22.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/other.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11082 2023-05-06 13:50:22.000000 byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/dolly/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-25 12:20:22.000000 byzerllm-0.1.8/src/byzerllm/dolly/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2029 2023-04-25 12:20:22.000000 byzerllm-0.1.8/src/byzerllm/dolly/consts.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1112 2023-04-25 12:45:20.000000 byzerllm-0.1.8/src/byzerllm/dolly/dolly_inference.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10065 2023-04-25 12:44:37.000000 byzerllm-0.1.8/src/byzerllm/dolly/generate.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12156 2023-04-25 12:27:32.000000 byzerllm-0.1.8/src/byzerllm/dolly/trainer.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/falcon/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4080 2023-09-12 08:34:55.000000 byzerllm-0.1.8/src/byzerllm/falcon/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/llama/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6141 2023-09-12 08:34:55.000000 byzerllm-0.1.8/src/byzerllm/llama/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/llama2/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6310 2023-09-12 08:34:55.000000 byzerllm-0.1.8/src/byzerllm/llama2/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/m3e/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      189 2023-07-16 01:34:12.000000 byzerllm-0.1.8/src/byzerllm/m3e/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/moss/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-06 15:03:50.000000 byzerllm-0.1.8/src/byzerllm/moss/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12657 2023-04-23 13:04:50.000000 byzerllm-0.1.8/src/byzerllm/moss/finetune_moss.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/moss/models/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-22 10:54:54.000000 byzerllm-0.1.8/src/byzerllm/moss/models/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5097 2023-05-19 09:07:29.000000 byzerllm-0.1.8/src/byzerllm/moss/models/configuration_moss.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6735 2023-04-23 12:11:45.000000 byzerllm-0.1.8/src/byzerllm/moss/models/custom_autotune.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31351 2023-04-23 12:11:45.000000 byzerllm-0.1.8/src/byzerllm/moss/models/modeling_moss.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18866 2023-04-23 12:11:45.000000 byzerllm-0.1.8/src/byzerllm/moss/models/quantization.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15952 2023-04-23 12:11:45.000000 byzerllm-0.1.8/src/byzerllm/moss/models/tokenization_moss.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16919 2023-06-26 08:47:30.000000 byzerllm-0.1.8/src/byzerllm/moss/moss_inference.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/processor/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      577 2023-08-14 06:44:47.000000 byzerllm-0.1.8/src/byzerllm/processor/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/qwen_vl_chat/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3579 2023-08-26 08:55:00.000000 byzerllm-0.1.8/src/byzerllm/qwen_vl_chat/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/records/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2065 2023-10-12 02:25:36.000000 byzerllm-0.1.8/src/byzerllm/records/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/saas/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-02 02:17:52.000000 byzerllm-0.1.8/src/byzerllm/saas/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/saas/azure_openai/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1724 2023-08-01 03:13:16.000000 byzerllm-0.1.8/src/byzerllm/saas/azure_openai/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/saas/chatglm/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2136 2023-06-27 05:23:44.000000 byzerllm-0.1.8/src/byzerllm/saas/chatglm/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/saas/sparkdesk/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5273 2023-06-27 05:38:38.000000 byzerllm-0.1.8/src/byzerllm/saas/sparkdesk/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6217 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/diffusion/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/diffusion/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/diffusion/pipelines/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/diffusion/pipelines/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4720 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/events/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1701 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/events/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1006 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/events/generation.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/models/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/models/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1260 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/models/diffusion.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      173 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/plugin.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1136 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/config.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3127 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/embeddings.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/networks/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3567 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8214 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/piplines/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/piplines/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31226 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10680 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/upscalers/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/upscalers/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8276 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5247 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3104 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/utils.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      673 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/images.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/lib/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/lib/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/stable_diffusion/lib/diffusers/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/lib/diffusers/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1246 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      434 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/logger.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4681 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/model.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      540 2023-08-16 04:11:49.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/shared.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      928 2023-08-14 15:16:57.000000 byzerllm-0.1.8/src/byzerllm/stable_diffusion/utils.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.290790 byzerllm-0.1.8/src/byzerllm/starcode/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1553 2023-08-10 10:02:48.000000 byzerllm-0.1.8/src/byzerllm/starcode/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2422 2023-09-25 10:15:36.000000 byzerllm-0.1.8/src/byzerllm/store.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4838 2023-10-12 01:43:30.000000 byzerllm-0.1.8/src/byzerllm/utils/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/config/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1059 2023-10-04 03:01:23.000000 byzerllm-0.1.8/src/byzerllm/utils/config/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4042 2023-09-04 13:26:00.000000 byzerllm-0.1.8/src/byzerllm/utils/emb.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/fulltune/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2637 2023-06-30 09:41:26.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/fulltune/base_model/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-28 06:59:34.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/base_model/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2929 2023-07-27 13:14:08.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30037 2023-07-27 13:14:08.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12755 2023-06-30 09:40:41.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/deepspeed_trainner.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4826 2023-06-29 13:00:23.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/launch.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/fulltune/pretrain/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28394 2023-09-19 06:47:44.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/pretrain/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2406 2023-09-20 03:09:31.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6924 2023-06-29 02:54:39.000000 byzerllm-0.1.8/src/byzerllm/utils/fulltune/trainner.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/inference/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3134 2023-07-11 13:03:47.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/inference/models/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10094 2023-07-08 03:06:41.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2699 2023-07-08 03:36:34.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/bloom.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21538 2023-07-08 03:28:59.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/causal_lm.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-08 03:03:28.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34973 2023-07-08 03:29:53.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/bloom_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11952 2023-07-08 03:32:19.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/flash_llama_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12421 2023-07-08 03:35:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/flash_neox_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19256 2023-07-08 03:45:37.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/flash_rw_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15720 2023-07-08 03:35:18.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/flash_santacoder_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44270 2023-07-08 03:35:23.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/mpt_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30556 2023-07-08 03:35:31.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/neox_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33490 2023-07-08 03:35:36.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/opt_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    47248 2023-07-08 03:35:42.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/t5_modeling.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40651 2023-07-10 05:08:26.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_causal_lm.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2405 2023-07-08 03:38:20.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_llama.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2081 2023-07-08 03:38:45.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_neox.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2035 2023-07-08 03:14:25.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_rw.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2584 2023-07-08 03:39:14.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_santacoder.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4457 2023-07-08 08:25:04.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/galactica.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2436 2023-07-08 03:40:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/gpt_neox.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3038 2023-07-08 03:23:26.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/model.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2504 2023-07-08 03:40:50.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/mpt.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2354 2023-07-08 03:41:08.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/opt.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3026 2023-07-08 03:41:14.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/rw.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2186 2023-07-08 03:41:23.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/santacoder.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23774 2023-07-08 03:42:39.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/seq2seq_lm.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2945 2023-07-08 03:43:05.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/t5.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6341 2023-07-11 09:12:44.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/models/types.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.294790 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      886 2023-07-08 05:35:37.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3865 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/convert.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2163 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/dist.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.298790 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/gptq/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-08 08:23:13.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/gptq/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10077 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/gptq/custom_autotune.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12464 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/gptq/quant_linear.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26942 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/gptq/quantize.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6251 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/hub.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    13654 2023-07-08 03:44:02.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/layers.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    14905 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/logits_process.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10645 2023-07-10 05:00:01.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/tokens.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3523 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/watermark.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5731 2023-07-08 03:13:03.000000 byzerllm-0.1.8/src/byzerllm/utils/inference/utils/weights.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.298790 byzerllm-0.1.8/src/byzerllm/utils/metrics/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1216 2023-10-04 02:30:32.000000 byzerllm-0.1.8/src/byzerllm/utils/metrics/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      367 2023-10-09 11:02:19.000000 byzerllm-0.1.8/src/byzerllm/utils/object_store_ref_util.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.298790 byzerllm-0.1.8/src/byzerllm/utils/rayinfer/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4124 2023-07-22 10:08:11.000000 byzerllm-0.1.8/src/byzerllm/utils/rayinfer/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.298790 byzerllm-0.1.8/src/byzerllm/utils/retrieval/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6093 2023-10-14 08:04:57.000000 byzerllm-0.1.8/src/byzerllm/utils/retrieval/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.298790 byzerllm-0.1.8/src/byzerllm/utils/sft/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10052 2023-09-18 01:54:43.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1203 2023-06-26 02:16:27.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/argument.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2029 2023-09-18 01:37:01.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/collator.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3248 2023-09-18 01:39:14.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/dataset.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1614 2023-06-25 10:28:20.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/loss.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2295 2023-09-13 09:14:56.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/merge_lora.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2611 2023-06-25 10:22:30.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/model.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8381 2023-10-03 02:06:56.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/qlora.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3395 2023-06-21 10:59:30.000000 byzerllm-0.1.8/src/byzerllm/utils/sft/trainer.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1288 2023-09-18 08:24:25.000000 byzerllm-0.1.8/src/byzerllm/utils/testing.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7111 2023-09-18 16:23:56.000000 byzerllm-0.1.8/src/byzerllm/utils/text_generator.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       22 2023-10-14 08:09:31.000000 byzerllm-0.1.8/src/byzerllm/version.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.298790 byzerllm-0.1.8/src/byzerllm/visualglm/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2462 2023-07-16 01:34:31.000000 byzerllm-0.1.8/src/byzerllm/visualglm/__init__.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.298790 byzerllm-0.1.8/src/byzerllm/whisper/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-05-11 01:44:23.000000 byzerllm-0.1.8/src/byzerllm/whisper/__init__.py
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1254 2023-05-11 07:07:58.000000 byzerllm-0.1.8/src/byzerllm/whisper/whisper_inference.py
-drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 08:09:41.262790 byzerllm-0.1.8/src/byzerllm.egg-info/
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      762 2023-10-14 08:09:41.000000 byzerllm-0.1.8/src/byzerllm.egg-info/PKG-INFO
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21194 2023-10-14 08:09:41.000000 byzerllm-0.1.8/src/byzerllm.egg-info/SOURCES.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-10-14 08:09:41.000000 byzerllm-0.1.8/src/byzerllm.egg-info/dependency_links.txt
--rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        9 2023-10-14 08:09:41.000000 byzerllm-0.1.8/src/byzerllm.egg-info/top_level.txt
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      762 2023-10-14 14:43:15.219375 byzerllm-0.1.9/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      449 2023-10-11 00:54:35.000000 byzerllm-0.1.9/README.md
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       38 2023-10-14 14:43:15.219375 byzerllm-0.1.9/setup.cfg
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1254 2023-05-15 03:02:58.000000 byzerllm-0.1.9/setup.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.179374 byzerllm-0.1.9/src/
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3025 2023-09-11 11:02:01.000000 byzerllm-0.1.9/src/byzerllm/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/alpha_moss/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29048 2023-07-07 08:01:34.000000 byzerllm-0.1.9/src/byzerllm/alpha_moss/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/apps/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      466 2023-07-04 14:50:28.000000 byzerllm-0.1.9/src/byzerllm/apps/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3942 2023-09-06 06:02:21.000000 byzerllm-0.1.9/src/byzerllm/apps/builder.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3350 2023-09-06 06:06:45.000000 byzerllm-0.1.9/src/byzerllm/apps/client.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6276 2023-09-06 06:07:35.000000 byzerllm-0.1.9/src/byzerllm/apps/qa.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4934 2023-09-01 16:22:38.000000 byzerllm-0.1.9/src/byzerllm/apps/qa_strategy.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1687 2023-09-06 06:19:12.000000 byzerllm-0.1.9/src/byzerllm/apps/vector_db.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/auto/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12154 2023-10-04 02:30:28.000000 byzerllm-0.1.9/src/byzerllm/auto/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7577 2023-07-31 02:07:12.000000 byzerllm-0.1.9/src/byzerllm/auto/backend_ds.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/baichuan/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4018 2023-09-12 08:55:25.000000 byzerllm-0.1.9/src/byzerllm/baichuan/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm/bark/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4243 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/api.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.179374 byzerllm-0.1.9/src/byzerllm/bark/assets/
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.195374 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16794 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/announcer.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20316 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31724 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    59348 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25116 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33860 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38124 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    13436 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18980 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25436 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24420 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34820 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30604 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29324 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36364 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44044 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43564 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    53908 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31244 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23036 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26820 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28684 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33004 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    46604 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45268 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    52684 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    41268 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29964 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44148 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24796 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37964 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22716 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    50548 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29540 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24156 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29004 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21916 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42284 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42548 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45324 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36364 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32420 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    58492 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    49004 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34444 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30284 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    58652 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1943 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/readme.md
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    57852 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24260 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51668 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29164 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45748 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42924 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19676 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    54548 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22556 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24156 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21596 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21276 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    35724 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23196 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28524 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26236 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34980 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25540 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22716 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25116 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26236 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23356 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25700 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25436 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45804 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25700 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    52204 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    50764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    49908 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    45108 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    55932 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32524 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43244 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25860 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29804 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    51404 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39404 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33804 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40788 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30444 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29644 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    43724 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    42708 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    37644 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24420 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31244 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26716 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40788 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20260 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31140 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26556 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26340 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19196 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39564 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23140 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23196 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27884 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31140 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23676 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    41428 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38180 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    38820 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30980 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    27724 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34500 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    36844 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26980 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28260 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30764 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28100 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28524 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39780 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39884 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    56628 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19940 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28204 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44628 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26020 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    39084 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34660 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22076 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24476 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    24956 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28684 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33164 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    17220 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    25276 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20260 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28204 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20636 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19836 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    29964 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    17436 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16900 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21060 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19300 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16156 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19620 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21380 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19460 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    32740 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19676 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    54548 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23516 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    22556 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    20580 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18396 2023-05-11 04:35:06.000000 byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3759 2023-08-26 08:52:44.000000 byzerllm-0.1.9/src/byzerllm/bark/bark_voice.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33373 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/generation.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     9139 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/model.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5955 2023-05-11 02:06:23.000000 byzerllm-0.1.9/src/byzerllm/bark/model_fine.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/bge/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1022 2023-09-04 13:38:16.000000 byzerllm-0.1.9/src/byzerllm/bge/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/chatglm2/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2108 2023-08-31 04:23:44.000000 byzerllm-0.1.9/src/byzerllm/chatglm2/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/chatglm6b/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-04 03:55:05.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8182 2023-04-04 03:55:05.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/arguments.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21286 2023-05-04 08:53:10.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/finetune.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11575 2023-04-04 03:55:05.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/trainer_seq2seq.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3000 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/finetune.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1404 2023-05-12 05:48:30.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/infer.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.207374 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      277 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16907 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/common.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7620 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/config.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6263 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/other.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11082 2023-05-06 13:50:22.000000 byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/dolly/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-25 12:20:22.000000 byzerllm-0.1.9/src/byzerllm/dolly/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2029 2023-04-25 12:20:22.000000 byzerllm-0.1.9/src/byzerllm/dolly/consts.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1112 2023-04-25 12:45:20.000000 byzerllm-0.1.9/src/byzerllm/dolly/dolly_inference.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10065 2023-04-25 12:44:37.000000 byzerllm-0.1.9/src/byzerllm/dolly/generate.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12156 2023-04-25 12:27:32.000000 byzerllm-0.1.9/src/byzerllm/dolly/trainer.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/falcon/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4080 2023-09-12 08:34:55.000000 byzerllm-0.1.9/src/byzerllm/falcon/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/llama/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6141 2023-09-12 08:34:55.000000 byzerllm-0.1.9/src/byzerllm/llama/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/llama2/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6310 2023-09-12 08:34:55.000000 byzerllm-0.1.9/src/byzerllm/llama2/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/m3e/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      189 2023-07-16 01:34:12.000000 byzerllm-0.1.9/src/byzerllm/m3e/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/moss/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-06 15:03:50.000000 byzerllm-0.1.9/src/byzerllm/moss/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12657 2023-04-23 13:04:50.000000 byzerllm-0.1.9/src/byzerllm/moss/finetune_moss.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/moss/models/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-04-22 10:54:54.000000 byzerllm-0.1.9/src/byzerllm/moss/models/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5097 2023-05-19 09:07:29.000000 byzerllm-0.1.9/src/byzerllm/moss/models/configuration_moss.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6735 2023-04-23 12:11:45.000000 byzerllm-0.1.9/src/byzerllm/moss/models/custom_autotune.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31351 2023-04-23 12:11:45.000000 byzerllm-0.1.9/src/byzerllm/moss/models/modeling_moss.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    18866 2023-04-23 12:11:45.000000 byzerllm-0.1.9/src/byzerllm/moss/models/quantization.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15952 2023-04-23 12:11:45.000000 byzerllm-0.1.9/src/byzerllm/moss/models/tokenization_moss.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    16919 2023-06-26 08:47:30.000000 byzerllm-0.1.9/src/byzerllm/moss/moss_inference.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/processor/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      577 2023-08-14 06:44:47.000000 byzerllm-0.1.9/src/byzerllm/processor/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/qwen_vl_chat/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3579 2023-08-26 08:55:00.000000 byzerllm-0.1.9/src/byzerllm/qwen_vl_chat/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/records/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2893 2023-10-14 13:04:39.000000 byzerllm-0.1.9/src/byzerllm/records/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/saas/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-02 02:17:52.000000 byzerllm-0.1.9/src/byzerllm/saas/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/saas/azure_openai/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1724 2023-08-01 03:13:16.000000 byzerllm-0.1.9/src/byzerllm/saas/azure_openai/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/saas/chatglm/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2136 2023-06-27 05:23:44.000000 byzerllm-0.1.9/src/byzerllm/saas/chatglm/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/saas/sparkdesk/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5273 2023-06-27 05:38:38.000000 byzerllm-0.1.9/src/byzerllm/saas/sparkdesk/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6217 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/pipelines/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/pipelines/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4720 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1701 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1006 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/generation.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/models/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/models/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1260 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/models/diffusion.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      173 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/plugin.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1136 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/config.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3127 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/embeddings.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3567 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8214 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    31226 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10680 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8276 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5247 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3104 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/utils.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      673 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/images.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/diffusers/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/diffusers/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1246 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      434 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/logger.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4681 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/model.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      540 2023-08-16 04:11:49.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/shared.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      928 2023-08-14 15:16:57.000000 byzerllm-0.1.9/src/byzerllm/stable_diffusion/utils.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.211374 byzerllm-0.1.9/src/byzerllm/starcode/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1553 2023-08-10 10:02:48.000000 byzerllm-0.1.9/src/byzerllm/starcode/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2422 2023-09-25 10:15:36.000000 byzerllm-0.1.9/src/byzerllm/store.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4838 2023-10-12 01:43:30.000000 byzerllm-0.1.9/src/byzerllm/utils/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/config/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1059 2023-10-04 03:01:23.000000 byzerllm-0.1.9/src/byzerllm/utils/config/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4042 2023-09-04 13:26:00.000000 byzerllm-0.1.9/src/byzerllm/utils/emb.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/fulltune/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2637 2023-06-30 09:41:26.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-06-28 06:59:34.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2929 2023-07-27 13:14:08.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30037 2023-07-27 13:14:08.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12755 2023-06-30 09:40:41.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/deepspeed_trainner.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4826 2023-06-29 13:00:23.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/launch.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    28394 2023-09-19 06:47:44.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2406 2023-09-20 03:09:31.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6924 2023-06-29 02:54:39.000000 byzerllm-0.1.9/src/byzerllm/utils/fulltune/trainner.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/inference/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3134 2023-07-11 13:03:47.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/inference/models/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10094 2023-07-08 03:06:41.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2699 2023-07-08 03:36:34.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/bloom.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21538 2023-07-08 03:28:59.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/causal_lm.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-08 03:03:28.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    34973 2023-07-08 03:29:53.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/bloom_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    11952 2023-07-08 03:32:19.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_llama_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12421 2023-07-08 03:35:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_neox_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    19256 2023-07-08 03:45:37.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_rw_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    15720 2023-07-08 03:35:18.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_santacoder_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    44270 2023-07-08 03:35:23.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/mpt_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    30556 2023-07-08 03:35:31.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/neox_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    33490 2023-07-08 03:35:36.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/opt_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    47248 2023-07-08 03:35:42.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/t5_modeling.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    40651 2023-07-10 05:08:26.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_causal_lm.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2405 2023-07-08 03:38:20.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_llama.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2081 2023-07-08 03:38:45.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_neox.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2035 2023-07-08 03:14:25.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_rw.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2584 2023-07-08 03:39:14.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_santacoder.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4457 2023-07-08 08:25:04.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/galactica.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2436 2023-07-08 03:40:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/gpt_neox.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3038 2023-07-08 03:23:26.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/model.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2504 2023-07-08 03:40:50.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/mpt.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2354 2023-07-08 03:41:08.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/opt.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3026 2023-07-08 03:41:14.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/rw.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2186 2023-07-08 03:41:23.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/santacoder.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    23774 2023-07-08 03:42:39.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/seq2seq_lm.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2945 2023-07-08 03:43:05.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/t5.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6341 2023-07-11 09:12:44.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/models/types.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.215374 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      886 2023-07-08 05:35:37.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3865 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/convert.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2163 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/dist.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-07-08 08:23:13.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10077 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/custom_autotune.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    12464 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/quant_linear.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    26942 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/quantize.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6251 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/hub.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    13654 2023-07-08 03:44:02.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/layers.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    14905 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/logits_process.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10645 2023-07-10 05:00:01.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/tokens.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3523 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/watermark.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     5731 2023-07-08 03:13:03.000000 byzerllm-0.1.9/src/byzerllm/utils/inference/utils/weights.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/metrics/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1216 2023-10-04 02:30:32.000000 byzerllm-0.1.9/src/byzerllm/utils/metrics/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      367 2023-10-09 11:02:19.000000 byzerllm-0.1.9/src/byzerllm/utils/object_store_ref_util.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/rayinfer/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     4124 2023-07-22 10:08:11.000000 byzerllm-0.1.9/src/byzerllm/utils/rayinfer/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/retrieval/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6104 2023-10-14 14:11:39.000000 byzerllm-0.1.9/src/byzerllm/utils/retrieval/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     6019 2023-10-14 14:35:52.000000 byzerllm-0.1.9/src/byzerllm/utils/retrieval/rest.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/utils/sft/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    10052 2023-09-18 01:54:43.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1203 2023-06-26 02:16:27.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/argument.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2029 2023-09-18 01:37:01.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/collator.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3248 2023-09-18 01:39:14.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/dataset.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1614 2023-06-25 10:28:20.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/loss.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2295 2023-09-13 09:14:56.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/merge_lora.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2611 2023-06-25 10:22:30.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/model.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     8381 2023-10-03 02:06:56.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/qlora.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     3395 2023-06-21 10:59:30.000000 byzerllm-0.1.9/src/byzerllm/utils/sft/trainer.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1288 2023-09-18 08:24:25.000000 byzerllm-0.1.9/src/byzerllm/utils/testing.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     7111 2023-09-18 16:23:56.000000 byzerllm-0.1.9/src/byzerllm/utils/text_generator.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)       22 2023-10-14 14:42:41.000000 byzerllm-0.1.9/src/byzerllm/version.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/visualglm/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     2462 2023-07-16 01:34:31.000000 byzerllm-0.1.9/src/byzerllm/visualglm/__init__.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.219375 byzerllm-0.1.9/src/byzerllm/whisper/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        0 2023-05-11 01:44:23.000000 byzerllm-0.1.9/src/byzerllm/whisper/__init__.py
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)     1254 2023-05-11 07:07:58.000000 byzerllm-0.1.9/src/byzerllm/whisper/whisper_inference.py
+drwxrwxr-x   0 winubuntu  (1000) winubuntu  (1000)        0 2023-10-14 14:43:15.183374 byzerllm-0.1.9/src/byzerllm.egg-info/
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)      762 2023-10-14 14:43:15.000000 byzerllm-0.1.9/src/byzerllm.egg-info/PKG-INFO
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)    21231 2023-10-14 14:43:15.000000 byzerllm-0.1.9/src/byzerllm.egg-info/SOURCES.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        1 2023-10-14 14:43:15.000000 byzerllm-0.1.9/src/byzerllm.egg-info/dependency_links.txt
+-rw-rw-r--   0 winubuntu  (1000) winubuntu  (1000)        9 2023-10-14 14:43:15.000000 byzerllm-0.1.9/src/byzerllm.egg-info/top_level.txt
```

### Comparing `byzerllm-0.1.8/PKG-INFO` & `byzerllm-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byzerllm
-Version: 0.1.8
+Version: 0.1.9
 Summary: ByzerLLM: Byzer LLM
 Author: allwefantasy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

### Comparing `byzerllm-0.1.8/setup.py` & `byzerllm-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/__init__.py` & `byzerllm-0.1.9/src/byzerllm/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/alpha_moss/__init__.py` & `byzerllm-0.1.9/src/byzerllm/alpha_moss/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/apps/builder.py` & `byzerllm-0.1.9/src/byzerllm/apps/builder.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/apps/client.py` & `byzerllm-0.1.9/src/byzerllm/apps/client.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/apps/qa.py` & `byzerllm-0.1.9/src/byzerllm/apps/qa.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/apps/qa_strategy.py` & `byzerllm-0.1.9/src/byzerllm/apps/qa_strategy.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/apps/vector_db.py` & `byzerllm-0.1.9/src/byzerllm/apps/vector_db.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/auto/__init__.py` & `byzerllm-0.1.9/src/byzerllm/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/auto/backend_ds.py` & `byzerllm-0.1.9/src/byzerllm/auto/backend_ds.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/baichuan/__init__.py` & `byzerllm-0.1.9/src/byzerllm/baichuan/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/api.py` & `byzerllm-0.1.9/src/byzerllm/bark/api.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/announcer.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/announcer.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/de_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/de_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/en_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/en_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/es_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/es_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/fr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/hi_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/it_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/it_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ja_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ko_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pl_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/pt_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/readme.md` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/readme.md`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/ru_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/tr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/de_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/en_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/es_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/fr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/hi_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/it_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ja_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ko_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pl_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/pt_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/ru_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/tr_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/v2/zh_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_0.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_1.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_2.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_3.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_4.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_5.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_6.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_7.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_8.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz` & `byzerllm-0.1.9/src/byzerllm/bark/assets/prompts/zh_speaker_9.npz`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/bark_voice.py` & `byzerllm-0.1.9/src/byzerllm/bark/bark_voice.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/generation.py` & `byzerllm-0.1.9/src/byzerllm/bark/generation.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/model.py` & `byzerllm-0.1.9/src/byzerllm/bark/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bark/model_fine.py` & `byzerllm-0.1.9/src/byzerllm/bark/model_fine.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/bge/__init__.py` & `byzerllm-0.1.9/src/byzerllm/bge/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm2/__init__.py` & `byzerllm-0.1.9/src/byzerllm/chatglm2/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/arguments.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/arguments.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/finetune.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/trainer_seq2seq.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/finetune.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/finetune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/infer.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/infer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/common.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/common.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/config.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/config.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/other.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/other.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py` & `byzerllm-0.1.9/src/byzerllm/chatglm6b/tunning/utils/seq2seq.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/dolly/consts.py` & `byzerllm-0.1.9/src/byzerllm/dolly/consts.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/dolly/dolly_inference.py` & `byzerllm-0.1.9/src/byzerllm/dolly/dolly_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/dolly/generate.py` & `byzerllm-0.1.9/src/byzerllm/dolly/generate.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/dolly/trainer.py` & `byzerllm-0.1.9/src/byzerllm/dolly/trainer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/falcon/__init__.py` & `byzerllm-0.1.9/src/byzerllm/falcon/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/llama/__init__.py` & `byzerllm-0.1.9/src/byzerllm/llama/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/llama2/__init__.py` & `byzerllm-0.1.9/src/byzerllm/llama2/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/moss/finetune_moss.py` & `byzerllm-0.1.9/src/byzerllm/moss/finetune_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/moss/models/configuration_moss.py` & `byzerllm-0.1.9/src/byzerllm/moss/models/configuration_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/moss/models/custom_autotune.py` & `byzerllm-0.1.9/src/byzerllm/moss/models/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/moss/models/modeling_moss.py` & `byzerllm-0.1.9/src/byzerllm/moss/models/modeling_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/moss/models/quantization.py` & `byzerllm-0.1.9/src/byzerllm/moss/models/quantization.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/moss/models/tokenization_moss.py` & `byzerllm-0.1.9/src/byzerllm/moss/models/tokenization_moss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/moss/moss_inference.py` & `byzerllm-0.1.9/src/byzerllm/moss/moss_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/processor/__init__.py` & `byzerllm-0.1.9/src/byzerllm/processor/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/qwen_vl_chat/__init__.py` & `byzerllm-0.1.9/src/byzerllm/qwen_vl_chat/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/records/__init__.py` & `byzerllm-0.1.9/src/byzerllm/records/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,67 +4,97 @@
 class ClusterSettings:
     def __init__(self, name:str, location:str, numNodes:int):
         self.name = name
         self.location = location 
         self.numNodes = numNodes   
 
     def json(self):
-        return json.dumps(self.__dict__,ensure_ascii=False)        
+        return json.dumps(self.__dict__,ensure_ascii=False) 
+
+    @staticmethod 
+    def from_json(json_str:str):
+        return ClusterSettings(**json.loads(json_str))       
 
 class TableSettings:
     def __init__(self, database:str, table:Optional[str], schema:str, location:Optional[str], num_shards:int):
         self.database = database
         self.table = table
         self.schema = schema
         self.location = location
         self.num_shards = num_shards
 
     def json(self):
-        return json.dumps(self.__dict__,ensure_ascii=False)    
+        return json.dumps(self.__dict__,ensure_ascii=False)
+
+    @staticmethod 
+    def from_json(json_str:str):
+        return TableSettings(**json.loads(json_str))    
 
 
 class EnvSettings:
     def __init__(self, javaHome:str, path:str):
         self.javaHome = javaHome
         self.path = path   
 
     def json(self):
-        return json.dumps(self.__dict__,ensure_ascii=False)  
+        return json.dumps(self.__dict__,ensure_ascii=False) 
+
+    @staticmethod
+    def from_json(json_str:str):
+        return EnvSettings(**json.loads(json_str)) 
 
 
 class ResourceRequirement:
     def __init__(self, name:float, resourceQuantity:float):
         self.name = name
         self.resourceQuantity = resourceQuantity   
 
     def json(self):
         return json.dumps(self.__dict__,ensure_ascii=False)
+    
+    @staticmethod
+    def from_json(json_str:str):
+        return ResourceRequirement(**json.loads(json_str))
+    
 
 
 class ResourceRequirementSettings:
     def __init__(self, resourceRequirements: List[ResourceRequirement]):
         self.resourceRequirements = resourceRequirements
 
     def json(self):
         return json.dumps({"resourceRequirements":[item.__dict__ for item in self.resourceRequirements]},ensure_ascii=False)           
+    
+    @staticmethod
+    def from_json(json_str:str):
+        s = json.loads(json_str)
+        return ResourceRequirementSettings([ResourceRequirement(**s["resourceRequirements"]) ])
 
 
 class JVMSettings:
     def __init__(self, options:list[str]):
         self.options = options   
 
     def json(self):
-        return json.dumps(self.__dict__,ensure_ascii=False)         
+        return json.dumps(self.__dict__,ensure_ascii=False) 
+
+    @staticmethod
+    def from_json(json_str:str):
+        return JVMSettings(**json.loads(json_str))        
 
 
 class SearchQuery:
     def __init__(self, keyword:Optional[str], fields:list[str], vector:list[float], vectorField:Optional[str], limit:int=10):
         self.keyword = keyword
         self.fields = fields
         self.vector = vector
         self.vectorField = vectorField
         self.limit = limit
 
     def json(self):
-        return json.dumps(self.__dict__,ensure_ascii=False)    
+        return json.dumps(self.__dict__,ensure_ascii=False) 
+
+    @staticmethod
+    def from_json(json_str:str):
+        return SearchQuery(**json.loads(json_str))
```

### Comparing `byzerllm-0.1.8/src/byzerllm/saas/azure_openai/__init__.py` & `byzerllm-0.1.9/src/byzerllm/saas/azure_openai/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/saas/chatglm/__init__.py` & `byzerllm-0.1.9/src/byzerllm/saas/chatglm/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/saas/sparkdesk/__init__.py` & `byzerllm-0.1.9/src/byzerllm/saas/sparkdesk/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/__init__.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/diffusion/pipelines/diffusers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/events/__init__.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/events/generation.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/events/generation.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/api/models/diffusion.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/api/models/diffusion.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/config.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/config.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/embeddings.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/embeddings.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/networks/lyco.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/diffusers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/piplines/lpw.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/multidiffusion.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/upscalers/samplers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/diffusion/utils.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/images.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/images.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/lib/diffusers/scheduler.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/model.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/shared.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/shared.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/stable_diffusion/utils.py` & `byzerllm-0.1.9/src/byzerllm/stable_diffusion/utils.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/starcode/__init__.py` & `byzerllm-0.1.9/src/byzerllm/starcode/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/store.py` & `byzerllm-0.1.9/src/byzerllm/store.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/config/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/config/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/emb.py` & `byzerllm-0.1.9/src/byzerllm/utils/emb.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/fulltune/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/fulltune/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py` & `byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/configuration_baichuan.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py` & `byzerllm-0.1.9/src/byzerllm/utils/fulltune/base_model/modeling_baichuan.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/fulltune/deepspeed_trainner.py` & `byzerllm-0.1.9/src/byzerllm/utils/fulltune/deepspeed_trainner.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/fulltune/launch.py` & `byzerllm-0.1.9/src/byzerllm/utils/fulltune/launch.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/fulltune/pretrain/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py` & `byzerllm-0.1.9/src/byzerllm/utils/fulltune/pretrain/convert_to_transformers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/fulltune/trainner.py` & `byzerllm-0.1.9/src/byzerllm/utils/fulltune/trainner.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/bloom.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/bloom.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/causal_lm.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/causal_lm.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/bloom_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/bloom_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/flash_llama_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_llama_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/flash_neox_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_neox_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/flash_rw_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_rw_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/flash_santacoder_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/flash_santacoder_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/mpt_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/mpt_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/neox_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/neox_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/opt_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/opt_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/custom_modeling/t5_modeling.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/custom_modeling/t5_modeling.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_causal_lm.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_causal_lm.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_llama.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_llama.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_neox.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_neox.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_rw.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_rw.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/flash_santacoder.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/flash_santacoder.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/galactica.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/galactica.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/gpt_neox.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/gpt_neox.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/model.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/mpt.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/mpt.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/opt.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/opt.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/rw.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/rw.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/santacoder.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/santacoder.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/seq2seq_lm.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/seq2seq_lm.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/t5.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/t5.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/models/types.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/models/types.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/convert.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/convert.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/dist.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/dist.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/gptq/custom_autotune.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/gptq/quant_linear.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/quant_linear.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/gptq/quantize.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/gptq/quantize.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/hub.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/hub.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/layers.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/layers.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/logits_process.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/logits_process.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/tokens.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/watermark.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/watermark.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/inference/utils/weights.py` & `byzerllm-0.1.9/src/byzerllm/utils/inference/utils/weights.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/metrics/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/rayinfer/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/rayinfer/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/retrieval/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/retrieval/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         retrieval_gateway = ray.get_actor("RetrievalGateway")
         self.launched = True
         self.retrieval_gateway = retrieval_gateway
         return retrieval_gateway  
 
     def gateway(slef) -> ray.actor.ActorHandle:
         return ray.get_actor("RetrievalGateway")
-    
+                 
 
     def start_cluster(self, cluster_settings:ClusterSettings,                       
                       env_settings:EnvSettings, 
                       jvm_settings:JVMSettings,
                       resource_requirement_settings:ResourceRequirementSettings = ResourceRequirementSettings([])) -> bool:                      
         if not self.launched:
             raise Exception("Please launch gateway first")
@@ -136,15 +136,15 @@
     
     def search(self,cluster_name:str, 
                        database:str, 
                        table:str, 
                        search_query: SearchQuery) -> List[Dict[str,Any]]:        
         cluster = self.cluster(cluster_name)
         v = cluster.search.remote(database,table,search_query.json())
-        return json.loads(ray.get(v))    
+        return json.loads(ray.get(v))
```

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/__init__.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/argument.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/argument.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/collator.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/collator.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/dataset.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/dataset.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/loss.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/loss.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/merge_lora.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/merge_lora.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/model.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/model.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/qlora.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/qlora.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/sft/trainer.py` & `byzerllm-0.1.9/src/byzerllm/utils/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/testing.py` & `byzerllm-0.1.9/src/byzerllm/utils/testing.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/utils/text_generator.py` & `byzerllm-0.1.9/src/byzerllm/utils/text_generator.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/visualglm/__init__.py` & `byzerllm-0.1.9/src/byzerllm/visualglm/__init__.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm/whisper/whisper_inference.py` & `byzerllm-0.1.9/src/byzerllm/whisper/whisper_inference.py`

 * *Files identical despite different names*

### Comparing `byzerllm-0.1.8/src/byzerllm.egg-info/PKG-INFO` & `byzerllm-0.1.9/src/byzerllm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byzerllm
-Version: 0.1.8
+Version: 0.1.9
 Summary: ByzerLLM: Byzer LLM
 Author: allwefantasy
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
```

### Comparing `byzerllm-0.1.8/src/byzerllm.egg-info/SOURCES.txt` & `byzerllm-0.1.9/src/byzerllm.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -421,14 +421,15 @@
 src/byzerllm/utils/inference/utils/gptq/__init__.py
 src/byzerllm/utils/inference/utils/gptq/custom_autotune.py
 src/byzerllm/utils/inference/utils/gptq/quant_linear.py
 src/byzerllm/utils/inference/utils/gptq/quantize.py
 src/byzerllm/utils/metrics/__init__.py
 src/byzerllm/utils/rayinfer/__init__.py
 src/byzerllm/utils/retrieval/__init__.py
+src/byzerllm/utils/retrieval/rest.py
 src/byzerllm/utils/sft/__init__.py
 src/byzerllm/utils/sft/argument.py
 src/byzerllm/utils/sft/collator.py
 src/byzerllm/utils/sft/dataset.py
 src/byzerllm/utils/sft/loss.py
 src/byzerllm/utils/sft/merge_lora.py
 src/byzerllm/utils/sft/model.py
```

