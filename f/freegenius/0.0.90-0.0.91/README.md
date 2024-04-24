# Comparing `tmp/freegenius-0.0.90.tar.gz` & `tmp/freegenius-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.0.90.tar", last modified: Thu Apr 18 21:38:10 2024, max compression
+gzip compressed data, was "freegenius-0.0.91.tar", last modified: Tue Apr 23 21:23:18 2024, max compression
```

## Comparing `freegenius-0.0.90.tar` & `freegenius-0.0.91.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.515118 freegenius-0.0.90/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    13105 2024-04-18 21:38:10.515118 freegenius-0.0.90/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.471118 freegenius-0.0.90/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10056 2024-04-18 21:38:09.000000 freegenius-0.0.90/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.0.90/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.475118 freegenius-0.0.90/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.0.90/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.0.90/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.0.90/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.0.90/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6646 2024-04-11 14:37:13.000000 freegenius-0.0.90/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.0.90/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10727 2024-04-11 14:37:13.000000 freegenius-0.0.90/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.0.90/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.0.90/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.0.90/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:09.000000 freegenius-0.0.90/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.0.90/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.475118 freegenius-0.0.90/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.0.90/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.0.90/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.0.90/freegenius/geminiprovision.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.475118 freegenius-0.0.90/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.0.90/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.0.90/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.475118 freegenius-0.0.90/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.0.90/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.491118 freegenius-0.0.90/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.0.90/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.0.90/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.0.90/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.0.90/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.0.90/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.0.90/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.499118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.503118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.503118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.503118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.503118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.467118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.503118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.503118 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.0.90/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.0.90/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-18 21:38:09.000000 freegenius-0.0.90/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.0.90/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.511118 freegenius-0.0.90/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.0.90/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-03-25 18:32:07.000000 freegenius-0.0.90/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.0.90/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.0.90/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.0.90/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.0.90/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7429 2024-04-09 10:22:46.000000 freegenius-0.0.90/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.0.90/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4667 2024-04-11 14:37:13.000000 freegenius-0.0.90/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.0.90/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.0.90/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.0.90/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.0.90/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.0.90/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.0.90/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.0.90/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.0.90/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5152 2024-04-11 14:32:24.000000 freegenius-0.0.90/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.0.90/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.0.90/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.0.90/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.0.90/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.0.90/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.0.90/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.0.90/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.0.90/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.0.90/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.0.90/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1325 2024-04-04 08:36:50.000000 freegenius-0.0.90/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.0.90/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.0.90/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.0.90/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8638 2024-04-11 14:37:13.000000 freegenius-0.0.90/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.0.90/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.0.90/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.0.90/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5898 2024-04-10 13:47:59.000000 freegenius-0.0.90/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.0.90/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.0.90/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.0.90/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.0.90/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.0.90/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.0.90/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.0.90/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.0.90/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.0.90/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.0.90/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      779 2024-04-16 16:37:20.000000 freegenius-0.0.90/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1293 2024-04-11 16:00:15.000000 freegenius-0.0.90/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7691 2024-04-16 20:07:13.000000 freegenius-0.0.90/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.511118 freegenius-0.0.90/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.0.90/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.515118 freegenius-0.0.90/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   108133 2024-04-16 22:24:56.000000 freegenius-0.0.90/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29655 2024-04-16 22:14:21.000000 freegenius-0.0.90/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17182 2024-04-16 22:12:03.000000 freegenius-0.0.90/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21560 2024-04-16 22:13:50.000000 freegenius-0.0.90/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7664 2024-04-09 10:22:46.000000 freegenius-0.0.90/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18715 2024-04-16 22:13:24.000000 freegenius-0.0.90/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    16440 2024-04-16 16:48:57.000000 freegenius-0.0.90/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.0.90/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.0.90/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.0.90/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4691 2024-04-18 21:32:51.000000 freegenius-0.0.90/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.0.90/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.0.90/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.0.90/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.0.90/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.0.90/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    42983 2024-04-16 21:59:26.000000 freegenius-0.0.90/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.0.90/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.0.90/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.0.90/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.0.90/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.0.90/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.0.90/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.0.90/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.0.90/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.0.90/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.0.90/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.0.90/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-18 21:38:10.515118 freegenius-0.0.90/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    13105 2024-04-18 21:38:10.000000 freegenius-0.0.90/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5856 2024-04-18 21:38:10.000000 freegenius-0.0.90/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-18 21:38:10.000000 freegenius-0.0.90/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1226 2024-04-18 21:38:10.000000 freegenius-0.0.90/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      780 2024-04-18 21:38:10.000000 freegenius-0.0.90/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-18 21:38:10.000000 freegenius-0.0.90/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-18 21:38:10.515118 freegenius-0.0.90/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10383 2024-04-18 21:35:00.000000 freegenius-0.0.90/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.869455 freegenius-0.0.91/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    13137 2024-04-23 21:23:18.869455 freegenius-0.0.91/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.829455 freegenius-0.0.91/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10056 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.0.91/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.833455 freegenius-0.0.91/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.0.91/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.0.91/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.0.91/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.0.91/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6646 2024-04-11 14:37:13.000000 freegenius-0.0.91/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.0.91/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10727 2024-04-11 14:37:13.000000 freegenius-0.0.91/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.0.91/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.0.91/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.0.91/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.0.91/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.833455 freegenius-0.0.91/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.0.91/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.0.91/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.0.91/freegenius/geminiprovision.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.833455 freegenius-0.0.91/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.0.91/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.0.91/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.833455 freegenius-0.0.91/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.0.91/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.849455 freegenius-0.0.91/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.0.91/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.0.91/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.0.91/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.0.91/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.0.91/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.0.91/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.0.91/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.0.91/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.0.91/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.861455 freegenius-0.0.91/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.0.91/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-03-25 18:32:07.000000 freegenius-0.0.91/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.0.91/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.0.91/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.0.91/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7429 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4667 2024-04-11 14:37:13.000000 freegenius-0.0.91/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.0.91/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.0.91/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.0.91/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.0.91/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.0.91/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5152 2024-04-11 14:32:24.000000 freegenius-0.0.91/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.0.91/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.0.91/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.0.91/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.0.91/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.0.91/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.0.91/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1325 2024-04-04 08:36:50.000000 freegenius-0.0.91/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.0.91/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.0.91/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.0.91/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8638 2024-04-11 14:37:13.000000 freegenius-0.0.91/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.0.91/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.0.91/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5898 2024-04-10 13:47:59.000000 freegenius-0.0.91/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.0.91/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.0.91/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.0.91/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.0.91/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.0.91/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.0.91/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      796 2024-04-21 20:10:23.000000 freegenius-0.0.91/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1293 2024-04-11 16:00:15.000000 freegenius-0.0.91/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7691 2024-04-16 20:07:13.000000 freegenius-0.0.91/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.861455 freegenius-0.0.91/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.0.91/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.869455 freegenius-0.0.91/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   108133 2024-04-16 22:24:56.000000 freegenius-0.0.91/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29582 2024-04-23 21:09:41.000000 freegenius-0.0.91/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17109 2024-04-23 21:09:37.000000 freegenius-0.0.91/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    22215 2024-04-23 21:09:06.000000 freegenius-0.0.91/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7664 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18715 2024-04-16 22:13:24.000000 freegenius-0.0.91/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    16442 2024-04-23 21:03:39.000000 freegenius-0.0.91/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.0.91/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.0.91/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.0.91/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.0.91/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.0.91/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.0.91/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.0.91/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.0.91/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.0.91/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    47445 2024-04-23 21:04:36.000000 freegenius-0.0.91/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.0.91/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.0.91/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.0.91/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.0.91/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.0.91/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.0.91/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.0.91/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.0.91/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.0.91/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.0.91/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.869455 freegenius-0.0.91/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    13137 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5856 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1226 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      797 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-23 21:23:18.869455 freegenius-0.0.91/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10383 2024-04-23 21:23:11.000000 freegenius-0.0.91/setup.py
```

### Comparing `freegenius-0.0.90/PKG-INFO` & `freegenius-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.90
+Version: 0.0.91
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
@@ -77,14 +77,15 @@
 Requires-Dist: llama-cpp-python[server]==0.2.61
 Requires-Dist: huggingface-hub
 Requires-Dist: langchain==0.1.13
 Requires-Dist: pydub
 Requires-Dist: stable-diffusion-cpp-python
 Requires-Dist: pytz
 Requires-Dist: geopy
+Requires-Dist: guidance==0.1.13
 
 # FreeGenius AI
 
 FreeGenius AI is an ambitious project sparked by the pioneering work of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). It's designed with the primary objective of offering a comprehensive suite of AI solutions that mirror the capabilities of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). However, FreeGenius AI is remarkably different in that all core features are completely free, and it doesn't require the use of an OpenAI key.
 
 As with [LetMeDoIt AI](https://github.com/eliranwong/letmedoit), FreeGenius AI is designed to be capable of engaging in intuitive conversations, executing codes, providing up-to-date information, and performing a wide range of tasks. It's designed to learn, adapt, and grow with the user, offering personalized experiences and interactions.
```

### Comparing `freegenius-0.0.90/freegenius/README.md` & `freegenius-0.0.91/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/__init__.py` & `freegenius-0.0.91/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/audio/notification1.mp3` & `freegenius-0.0.91/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/audio/notification1_mild.mp3` & `freegenius-0.0.91/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/audio/notification2.mp3` & `freegenius-0.0.91/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/audio/notification2_mild.mp3` & `freegenius-0.0.91/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/autoassist.py` & `freegenius-0.0.91/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/autobuilder.py` & `freegenius-0.0.91/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/autoretriever.py` & `freegenius-0.0.91/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/chatgpt.py` & `freegenius-0.0.91/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/codey.py` & `freegenius-0.0.91/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/commandprompt.py` & `freegenius-0.0.91/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/eTextEdit.py` & `freegenius-0.0.91/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/geminipro.py` & `freegenius-0.0.91/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/geminiprovision.py` & `freegenius-0.0.91/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/gui/chatgui.py` & `freegenius-0.0.91/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/gui/worker.py` & `freegenius-0.0.91/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/icons/FreeGenius.ico` & `freegenius-0.0.91/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/icons/FreeGenius.png` & `freegenius-0.0.91/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/icons/FreeGenius_original.png` & `freegenius-0.0.91/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/icons/ai.png` & `freegenius-0.0.91/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/icons/ai_original.png` & `freegenius-0.0.91/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/llamacpp.py` & `freegenius-0.0.91/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/main.py` & `freegenius-0.0.91/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/ollamachat.py` & `freegenius-0.0.91/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/palm2.py` & `freegenius-0.0.91/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.0.91/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.0.91/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/000_check_vlc.py` & `freegenius-0.0.91/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/add calendar event.py` & `freegenius-0.0.91/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/aliases.py` & `freegenius-0.0.91/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/analyze audio.py` & `freegenius-0.0.91/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/analyze files.py` & `freegenius-0.0.91/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/analyze images.py` & `freegenius-0.0.91/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/analyze web content.py` & `freegenius-0.0.91/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/auto correct python code.py` & `freegenius-0.0.91/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/awesome prompts.py` & `freegenius-0.0.91/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/character analysis.py` & `freegenius-0.0.91/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/chat.py` & `freegenius-0.0.91/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/contexts.py` & `freegenius-0.0.91/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/counselling.py` & `freegenius-0.0.91/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/create ai assistants.py` & `freegenius-0.0.91/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/create images.py` & `freegenius-0.0.91/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/create maps.py` & `freegenius-0.0.91/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/create qrcode.py` & `freegenius-0.0.91/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/create statistical graphics.py` & `freegenius-0.0.91/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/dates and times.py` & `freegenius-0.0.91/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/download youtube or web content.py` & `freegenius-0.0.91/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/edit text.py` & `freegenius-0.0.91/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/execute computing tasks.py` & `freegenius-0.0.91/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/execute termux command.py` & `freegenius-0.0.91/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/global finance.py` & `freegenius-0.0.91/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/improve British English.py` & `freegenius-0.0.91/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/input suggestions.py` & `freegenius-0.0.91/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/install python package.py` & `freegenius-0.0.91/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/integrate google searches.py` & `freegenius-0.0.91/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/memory.py` & `freegenius-0.0.91/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/modify images.py` & `freegenius-0.0.91/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/open web browser.py` & `freegenius-0.0.91/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/pronounce words.py` & `freegenius-0.0.91/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/remove image background.py` & `freegenius-0.0.91/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/search chat records.py` & `freegenius-0.0.91/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/search financial data.py` & `freegenius-0.0.91/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/search latest news.py` & `freegenius-0.0.91/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/search sqlite.py` & `freegenius-0.0.91/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/search weather info.py` & `freegenius-0.0.91/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/send email.py` & `freegenius-0.0.91/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/send tweet.py` & `freegenius-0.0.91/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.0.91/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.0.91/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/rag.py` & `freegenius-0.0.91/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/requirements.txt` & `freegenius-0.0.91/freegenius/requirements.txt`

 * *Files 14% similar despite different names*

```diff
@@ -52,8 +52,9 @@
 ollama==0.1.8
 llama-cpp-python[server]==0.2.61
 huggingface-hub
 langchain==0.1.13
 pydub
 stable-diffusion-cpp-python
 pytz
-geopy
+geopy
+guidance==0.1.13
```

### Comparing `freegenius-0.0.90/freegenius/servers.py` & `freegenius-0.0.91/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/systemtray.py` & `freegenius-0.0.91/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/assistant.py` & `freegenius-0.0.91/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/call_chatgpt.py` & `freegenius-0.0.91/freegenius/utils/call_chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,16 +359,14 @@
     # Auto Function Call equivalence
 
     @staticmethod
     def runGeniusCall(messages: dict, noFunctionCall: bool = False):
         user_request = messages[-1]["content"]
         if config.intent_screening:
             # 1. Intent Screening
-            if config.developer:
-                print1("screening ...")
             noFunctionCall = True if noFunctionCall else CallChatGPT.screen_user_request(messages=messages)
         if noFunctionCall or config.tool_dependence <= 0.0:
             return CallChatGPT.regularCall(messages)
         else:
             # 2. Tool Selection
             if config.selectedTool and config.selectedTool in config.toolFunctionSchemas:
                 tool_name = config.selectedTool
```

### Comparing `freegenius-0.0.90/freegenius/utils/call_gemini.py` & `freegenius-0.0.91/freegenius/utils/call_gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,16 +202,14 @@
     # Auto Function Call equivalence
 
     @staticmethod
     def runGeniusCall(messages: dict, noFunctionCall: bool = False):
         user_request = messages[-1]["content"]
         if config.intent_screening:
             # 1. Intent Screening
-            if config.developer:
-                print1("screening ...")
             noFunctionCall = True if noFunctionCall else CallGemini.screen_user_request(messages=messages, user_request=user_request)
         if noFunctionCall or config.tool_dependence <= 0.0:
             return CallGemini.regularCall(messages)
         else:
             # 2. Tool Selection
             if config.selectedTool and config.selectedTool in config.toolFunctionSchemas:
                 tool_name = config.selectedTool
```

### Comparing `freegenius-0.0.90/freegenius/utils/call_llamacpp.py` & `freegenius-0.0.91/freegenius/utils/call_llamacpp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from freegenius import config, showErrors, get_or_create_collection, query_vectors, getDeviceInfo, isValidPythodCode, executeToolFunction, toParameterSchema
-from freegenius import print1, print2, print3, selectTool, getPythonFunctionResponse, extractPythonCode, downloadStableDiffusionFiles
+from freegenius import print1, print2, print3, selectTool, getPythonFunctionResponse, extractPythonCode, downloadStableDiffusionFiles, screening
 from typing import Optional
 from llama_cpp import Llama
 from prompt_toolkit import prompt
 from pathlib import Path
 from huggingface_hub import hf_hub_download
 import traceback, json, re, os, pprint, copy, datetime
+from guidance import models
 
 
 class CallLlamaCpp:
 
     @staticmethod
     def checkCompletion():
 
@@ -257,16 +258,14 @@
     # Auto Function call equivalence
 
     @staticmethod
     def runGeniusCall(messages: dict, noFunctionCall: bool = False):
         user_request = messages[-1]["content"]
         if config.intent_screening:
             # 1. Intent Screening
-            if config.developer:
-                print1("screening ...")
             noFunctionCall = True if noFunctionCall else CallLlamaCpp.screen_user_request(messages=messages, user_request=user_request)
         if noFunctionCall or config.tool_dependence <= 0.0:
             return CallLlamaCpp.regularCall(messages)
         else:
             # 2. Tool Selection
             if config.selectedTool and config.selectedTool in config.toolFunctionSchemas:
                 tool_name = config.selectedTool
@@ -349,14 +348,34 @@
                     config.currentMessages.append({"role": "assistant", "content": config.tempContent if config.tempContent else "Done!"})
                     config.tempContent = ""
                     config.conversationStarted = True
                     return None
 
     @staticmethod
     def screen_user_request(messages: dict, user_request: str) -> bool:
+        lm = models.LlamaCpp(
+            config.llamacppMainModel_model_path,
+            echo = False,
+            chat_format="chatml",
+            n_ctx=config.llamacppMainModel_n_ctx,
+            n_batch=config.llamacppMainModel_n_batch,
+            verbose=config.llamacppMainModel_verbose,
+            n_gpu_layers=config.llamacppMainModel_n_gpu_layers,
+            **config.llamacppMainModel_additional_model_options,
+        )
+        try:
+            tool = screening(lm, user_request)
+        except:
+            tool = True
+        lm.reset()
+        del lm
+        return not tool
+
+    @staticmethod
+    def screen_user_request_old(messages: dict, user_request: str) -> bool:
         
         deviceInfo = f"""\n\nMy device information:\n{getDeviceInfo()}""" if config.includeDeviceInfoInContext else ""
         answer = {
             "answer": {
                 "type": "string",
                 "description": """Either 'yes' or 'no':
 - Answer 'no' if you are asked to execute a computing task.
```

### Comparing `freegenius-0.0.90/freegenius/utils/call_llm.py` & `freegenius-0.0.91/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/call_ollama.py` & `freegenius-0.0.91/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/config_essential.py` & `freegenius-0.0.91/freegenius/utils/config_essential.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,23 +67,23 @@
     ('llamacppChatModel_additional_chat_options', {}),
     ('llamacppMainModel_ollama_tag', ''), # selected ollama hosted model to run with llamacpp
     ('llamacppMainModel_model_path', ''), # specify file path of llama.cpp model for general purpose
     ('llamacppMainModel_repo_id', 'CodeLlama-7B-Instruct-GGUF'), # llama.cpp model used for both task execution and conversation, e.g. 'TheBloke/phi-2-GGUF', 'NousResearch/Hermes-2-Pro-Mistral-7B-GGUF', 'NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO-GGUF'
     ('llamacppMainModel_filename', 'codellama-7b-instruct.Q4_K_M.gguf'), # llama.cpp model used for both task execution and conversation, e.g. 'Hermes-2-Pro-Mistral-7B.Q4_K_M.gguf', 'Nous-Hermes-2-Mixtral-8x7B-DPO.Q4_K_M.gguf'
     ('llamacppMainModel_n_ctx', 0), # llama.cpp main model context window
     ('llamacppMainModel_max_tokens', 10000), # llama.cpp main model maximum tokens
-    ('llamacppMainModel_n_gpu_layers', 0), # change to -1 to use GPU acceleration
+    ('llamacppMainModel_n_gpu_layers', -1), # change to -1 to use GPU acceleration
     ('llamacppMainModel_n_batch', 512), # The batch size to use per eval
     ('llamacppChatModel_ollama_tag', ''), # selected ollama hosted model to run with llamacpp
     ('llamacppChatModel_model_path', ''), # specify file path of llama.cpp model for chat
     ('llamacppChatModel_repo_id', 'TheBloke/Mistral-7B-Instruct-v0.2-GGUF'), # llama.cpp model used for chat, e.g. 'TheBloke/CodeLlama-7B-Python-GGUF'
     ('llamacppChatModel_filename', 'mistral-7b-instruct-v0.2.Q4_K_M.gguf'), # llama.cpp model used for chat, e.g. 'codellama-7b-python.Q4_K_M.gguf'
     ('llamacppChatModel_n_ctx', 0), # llama.cpp chat model context window
     ('llamacppChatModel_max_tokens', 10000), # llama.cpp chat model maximum tokens
-    ('llamacppChatModel_n_gpu_layers', 0), # change to -1 to use GPU acceleration
+    ('llamacppChatModel_n_gpu_layers', -1), # change to -1 to use GPU acceleration
     ('llamacppChatModel_n_batch', 512), # The batch size to use per eval
     ('geminipro_max_output_tokens', 8192), # check supported value at https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models
     # common configs as in LetMeDoIt AI
     ('translateToLanguage', ''),
     ('dynamicTokenCount', False),
     ('use_oai_assistant', False), # support OpenAI Assistants API in AutoGen Agent Builder
     ('max_agents', 5), # maximum number of agents build manager can create.
```

### Comparing `freegenius-0.0.90/freegenius/utils/config_tools.py` & `freegenius-0.0.91/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/download.py` & `freegenius-0.0.91/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/get_path_prompt.py` & `freegenius-0.0.91/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/ollama_models.py` & `freegenius-0.0.91/freegenius/utils/ollama_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 ollama_models = (
+    "dolphin-llama3",
+    "dolphin-llama3:8b",
     "llama3",
     "llama3:8b",
     "llama3:8b-text",
     "llama3:70b-instruct",
     "llama3:70b-text",
     "wizardlm2",
     "wizardlm2:7b",
@@ -22,27 +24,34 @@
     "llama2:7b",
     "llama2:13b",
     "llama2:70b",
     "mistral",
     "mistral:7b",
     "mixtral",
     "mixtral:8x7b",
+    "mixtral:instruct",
+    "mixtral:text",
+    "mixtral:8x22b",
+    "mixtral:8x22b-instruct",
+    "mixtral:8x22b-text",
     "neural-chat",
     "dolphin-mixtral",
     "dolphin-mixtral:8x7b",
     "mistral-openorca",
     "mistral-openorca:7b",
     "llama2-uncensored",
     "llama2-uncensored:7b",
     "llama2-uncensored:70b",
     "orca-mini",
     "orca-mini:3b",
     "orca-mini:7b",
     "orca-mini:13b",
     "orca-mini:70b",
+    "phi3",
+    "phi3:3.8b",
     "phi",
     "phi:2.7b",
     "dolphin-mistral",
     "dolphin-mistral:7b",
     "vicuna",
     "vicuna:7b",
     "vicuna:13b",
```

### Comparing `freegenius-0.0.90/freegenius/utils/promptValidator.py` & `freegenius-0.0.91/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.0.91/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.0.91/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/prompts.py` & `freegenius-0.0.91/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/python_utils.py` & `freegenius-0.0.91/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/shared_utils.py` & `freegenius-0.0.91/freegenius/utils/shared_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,22 +12,90 @@
 from vertexai.generative_models import Content, Part
 from pathlib import Path
 from PIL import Image
 from openai import OpenAI
 from huggingface_hub import hf_hub_download
 from bs4 import BeautifulSoup
 from urllib.parse import quote
+from guidance import select, gen
 
 # non-Android only
 if not config.isTermux:
     from autogen.retrieve_utils import TEXT_FORMATS
 
 # a dummy import line to resolve ALSA error display on Linux
 import sounddevice
 
+
+# guidance
+
+def screening(lm, user_input) -> bool:
+    tool = False
+
+    print2("```screening")
+    thought = "Thought: First, I must carefully distinguish whether the given request is formulated like a greeting, a question, a command, a statement, an issue, a description."
+    print3(thought)
+    lm += f"""<|im_start|>user
+Assess the following request and comment whether an additional tool is needed to address it:
+<request>{user_input}</request><|im_end|>
+<|im_start|>assistant
+{thought}
+Observation: The given request is formulated like {select(["a question", "a command", "a statement", "an issue", "a description"], name="question")}.
+"""
+    question = lm.get("question")
+    print3(f"""Observation: The given request is formulated like {question}.""")
+    if question in ("a greeting", "a question", "an issue", "a description"):
+        #thought = "Thought: Next, I need to ascertain the nature of the requested information, determining whether it is static, time-sensitive, changing over time, unchanging over time, published, well-established, common, documented, foundational, historical, technical, prone to periodic updates, subject to changes, evolving, ongoing, location-specific, or unknown." # more categories: "context-specific", "user-dependent", "subject to fluctuation"
+        thought = "Thought: Next, I must carefully distinguish whether the requested information is about greeting, common knowledge, math, translation, published content, acquired knowledge, historical records, programming knowledge, religious knowledge, insights obtainable from literature, textbook material, evolving data, recent updates, latest information, current time, current weather, up-to-date news, information specific to your device, or information unknown to me."
+        print3(thought)
+        lm += f"""{thought}
+Observation: The requested information is about {select(["greeting", "common knowledge", "math", "translation", "published content", "trained knowledge", "historical records", "programming knowledge", "religious knowledge", "insights obtainable from literature", "textbook content", "evolving data", "recent updates", "latest information", "current time", "current weather", "up-to-date news", "information specific to your device", "information unknown to me"], name="information")}.
+"""
+        #Observation: The nature of the requested information is {select(["static", "time-sensitive", "changing over time", "unchanging over time", "published", "well-established", "common", "documented", "foundational", "historical", "technical", "prone to periodic updates", "subject to changes", "evolving", "ongoing", "location-specific", "unknown"], name="information")}.
+        information = lm.get("information")
+        print3(f"""Observation: The requested information is about {information}.""")
+        if information in ("evolving data", "recent updates", "latest information", "current time", "current weather", "up-to-date news", "information specific to your device", "information unknown to me"):
+            tool = True
+    else:
+        thought = "Thought: Next, I must carefully distinguish whether the given request asks for generating a text-response or carrying out a task on your device."
+        print3(thought)
+        lm += f"""{thought}
+Observation: The given request asks for {select(["greeting", "calculation", "translation", "writing a text-response", "carrying out a task on your device"], name="action")}.
+"""
+        action = lm.get("action")
+        print3(f"""Observation: The given request asks for {action}.""")
+        if action in ("carrying out a task on your device",):
+            tool = True
+
+    print3(f"""Comment: Tool may {"" if tool else "not "}be required.""")
+    print2("```")
+
+    return tool
+
+def select_tool(lm, user_input):
+    tool_names = list(config.toolFunctionSchemas.keys())
+    tools = {i:config.toolFunctionSchemas[i]["description"] for i in config.toolFunctionSchemas}
+
+    lm += f"""<|im_start|>user
+Select an action to resolve the request as best you can. You have access only to the following tools:
+
+{tools}
+
+Use the following format:
+
+Request: the input request you must resolve
+Thought: you should always think about what to do
+Action: the action to take, has to be one of {tool_names}<|im_end|>
+<|im_start|>assistant
+Request: {user_input}
+Thought: {gen(stop=".")}.
+Action: {select(tool_names, name="tool")}"""
+    
+    return lm.get("tool")
+
 # local llm
 
 def downloadStableDiffusionFiles():
     # llm directory
     llm_directory = os.path.join(config.localStorage, "LLMs", "stable_diffusion")
     Path(llm_directory).mkdir(parents=True, exist_ok=True)
     filename = "v1-5-pruned-emaonly.safetensors"
```

### Comparing `freegenius-0.0.90/freegenius/utils/shortcuts.py` & `freegenius-0.0.91/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/single_prompt.py` & `freegenius-0.0.91/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.0.91/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/sttLanguages.py` & `freegenius-0.0.91/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.0.91/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.0.91/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/text_utils.py` & `freegenius-0.0.91/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/tool_plugins.py` & `freegenius-0.0.91/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/ttsLanguages.py` & `freegenius-0.0.91/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/tts_utils.py` & `freegenius-0.0.91/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius/utils/vlc_utils.py` & `freegenius-0.0.91/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius.egg-info/PKG-INFO` & `freegenius-0.0.91/freegenius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.90
+Version: 0.0.91
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
@@ -77,14 +77,15 @@
 Requires-Dist: llama-cpp-python[server]==0.2.61
 Requires-Dist: huggingface-hub
 Requires-Dist: langchain==0.1.13
 Requires-Dist: pydub
 Requires-Dist: stable-diffusion-cpp-python
 Requires-Dist: pytz
 Requires-Dist: geopy
+Requires-Dist: guidance==0.1.13
 
 # FreeGenius AI
 
 FreeGenius AI is an ambitious project sparked by the pioneering work of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). It's designed with the primary objective of offering a comprehensive suite of AI solutions that mirror the capabilities of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). However, FreeGenius AI is remarkably different in that all core features are completely free, and it doesn't require the use of an OpenAI key.
 
 As with [LetMeDoIt AI](https://github.com/eliranwong/letmedoit), FreeGenius AI is designed to be capable of engaging in intuitive conversations, executing codes, providing up-to-date information, and performing a wide range of tasks. It's designed to learn, adapt, and grow with the user, offering personalized experiences and interactions.
```

### Comparing `freegenius-0.0.90/freegenius.egg-info/SOURCES.txt` & `freegenius-0.0.91/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius.egg-info/entry_points.txt` & `freegenius-0.0.91/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.90/freegenius.egg-info/requires.txt` & `freegenius-0.0.91/freegenius.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -53,7 +53,8 @@
 llama-cpp-python[server]==0.2.61
 huggingface-hub
 langchain==0.1.13
 pydub
 stable-diffusion-cpp-python
 pytz
 geopy
+guidance==0.1.13
```

### Comparing `freegenius-0.0.90/setup.py` & `freegenius-0.0.91/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.0.90",
+    version="0.0.91",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

