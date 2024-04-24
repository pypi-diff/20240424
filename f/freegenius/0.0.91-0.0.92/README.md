# Comparing `tmp/freegenius-0.0.91.tar.gz` & `tmp/freegenius-0.0.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.0.91.tar", last modified: Tue Apr 23 21:23:18 2024, max compression
+gzip compressed data, was "freegenius-0.0.92.tar", last modified: Wed Apr 24 12:14:03 2024, max compression
```

## Comparing `freegenius-0.0.91.tar` & `freegenius-0.0.92.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.869455 freegenius-0.0.91/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    13137 2024-04-23 21:23:18.869455 freegenius-0.0.91/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.829455 freegenius-0.0.91/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10056 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.0.91/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.833455 freegenius-0.0.91/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.0.91/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.0.91/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.0.91/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.0.91/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6646 2024-04-11 14:37:13.000000 freegenius-0.0.91/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.0.91/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10727 2024-04-11 14:37:13.000000 freegenius-0.0.91/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.0.91/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.0.91/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.0.91/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.0.91/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.833455 freegenius-0.0.91/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.0.91/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.0.91/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.0.91/freegenius/geminiprovision.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.833455 freegenius-0.0.91/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.0.91/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.0.91/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.833455 freegenius-0.0.91/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.0.91/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.849455 freegenius-0.0.91/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.0.91/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.0.91/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.0.91/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.0.91/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.0.91/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.0.91/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.853455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.825456 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.857455 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.0.91/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.0.91/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.0.91/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.861455 freegenius-0.0.91/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.0.91/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-03-25 18:32:07.000000 freegenius-0.0.91/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.0.91/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.0.91/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.0.91/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7429 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4667 2024-04-11 14:37:13.000000 freegenius-0.0.91/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.0.91/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.0.91/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.0.91/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.0.91/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.0.91/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5152 2024-04-11 14:32:24.000000 freegenius-0.0.91/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.0.91/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.0.91/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.0.91/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.0.91/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.0.91/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.0.91/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1325 2024-04-04 08:36:50.000000 freegenius-0.0.91/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.0.91/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.0.91/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.0.91/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8638 2024-04-11 14:37:13.000000 freegenius-0.0.91/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.0.91/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.0.91/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5898 2024-04-10 13:47:59.000000 freegenius-0.0.91/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.0.91/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.0.91/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.0.91/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.0.91/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.0.91/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.0.91/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.0.91/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.0.91/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      796 2024-04-21 20:10:23.000000 freegenius-0.0.91/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1293 2024-04-11 16:00:15.000000 freegenius-0.0.91/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7691 2024-04-16 20:07:13.000000 freegenius-0.0.91/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.861455 freegenius-0.0.91/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.0.91/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.869455 freegenius-0.0.91/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   108133 2024-04-16 22:24:56.000000 freegenius-0.0.91/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29582 2024-04-23 21:09:41.000000 freegenius-0.0.91/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17109 2024-04-23 21:09:37.000000 freegenius-0.0.91/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    22215 2024-04-23 21:09:06.000000 freegenius-0.0.91/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7664 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18715 2024-04-16 22:13:24.000000 freegenius-0.0.91/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    16442 2024-04-23 21:03:39.000000 freegenius-0.0.91/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.0.91/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.0.91/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.0.91/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.0.91/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.0.91/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.0.91/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.0.91/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.0.91/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.0.91/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    47445 2024-04-23 21:04:36.000000 freegenius-0.0.91/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.0.91/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.0.91/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.0.91/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.0.91/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.0.91/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.0.91/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.0.91/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.0.91/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.0.91/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.0.91/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.0.91/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-23 21:23:18.869455 freegenius-0.0.91/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    13137 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5856 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1226 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      797 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-23 21:23:18.000000 freegenius-0.0.91/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-23 21:23:18.869455 freegenius-0.0.91/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10383 2024-04-23 21:23:11.000000 freegenius-0.0.91/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.697394 freegenius-0.0.92/
+-rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-24 12:14:03.697153 freegenius-0.0.92/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.668412 freegenius-0.0.92/freegenius/
+-rw-r--r--   0 admin      (501) staff       (20)    10056 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius/README.md
+-rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.670103 freegenius-0.0.92/freegenius/audio/
+-rw-r--r--   0 admin      (501) staff       (20)    15588 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/audio/notification1.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     2925 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/audio/notification1_mild.mp3
+-rw-r--r--   0 admin      (501) staff       (20)    19428 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/audio/notification2.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     3693 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/audio/notification2_mild.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     6646 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/autoassist.py
+-rw-r--r--   0 admin      (501) staff       (20)     9421 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/autobuilder.py
+-rw-r--r--   0 admin      (501) staff       (20)    10727 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/autoretriever.py
+-rw-r--r--   0 admin      (501) staff       (20)     6933 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)     7037 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/codey.py
+-rw-r--r--   0 admin      (501) staff       (20)      833 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/commandprompt.py
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius/config.py
+-rw-r--r--   0 admin      (501) staff       (20)    29583 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/eTextEdit.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.670242 freegenius-0.0.92/freegenius/files/
+-rw-r--r--   0 admin      (501) staff       (20)       31 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/files/Readme.md
+-rw-r--r--   0 admin      (501) staff       (20)    11372 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/geminipro.py
+-rw-r--r--   0 admin      (501) staff       (20)     7838 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/geminiprovision.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.670681 freegenius-0.0.92/freegenius/gui/
+-rw-r--r--   0 admin      (501) staff       (20)     9741 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/gui/chatgui.py
+-rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/gui/worker.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.670851 freegenius-0.0.92/freegenius/history/
+-rw-r--r--   0 admin      (501) staff       (20)       29 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/history/Readme.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.675908 freegenius-0.0.92/freegenius/icons/
+-rw-r--r--   0 admin      (501) staff       (20)   158655 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/FreeGenius.ico
+-rw-r--r--   0 admin      (501) staff       (20)  2549036 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/FreeGenius.png
+-rw-r--r--   0 admin      (501) staff       (20)  3162696 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/FreeGenius_original.png
+-rw-r--r--   0 admin      (501) staff       (20)  3141194 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/ai.png
+-rw-r--r--   0 admin      (501) staff       (20)  2390858 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/ai_original.png
+-rw-r--r--   0 admin      (501) staff       (20)     8119 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/llamacpp.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.663122 freegenius-0.0.92/freegenius/macOS_service/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662005 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.678957 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      644 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679097 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5680 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662167 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679412 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679561 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5679 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662320 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679849 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      635 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679979 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4100 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5684 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662480 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.680282 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      649 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.680420 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662651 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.680686 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      643 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.680820 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662816 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.681122 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      640 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.681302 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5656 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662997 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.681600 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.681737 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.663163 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.682029 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.682198 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5692 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-r--r--   0 admin      (501) staff       (20)     7320 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/main.py
+-rw-r--r--   0 admin      (501) staff       (20)    10959 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/ollamachat.py
+-rw-r--r--   0 admin      (501) staff       (20)       10 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius/package_name.txt
+-rw-r--r--   0 admin      (501) staff       (20)     7573 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/palm2.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.689403 freegenius-0.0.92/freegenius/plugins/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/000_check_ffmpeg.py
+-rw-r--r--   0 admin      (501) staff       (20)     1616 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/000_check_pyaudio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/000_check_vlc.py
+-rw-r--r--   0 admin      (501) staff       (20)      115 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/Readme.md
+-rw-r--r--   0 admin      (501) staff       (20)     6812 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/add calendar event.py
+-rw-r--r--   0 admin      (501) staff       (20)     3358 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/aliases.py
+-rw-r--r--   0 admin      (501) staff       (20)     7429 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/analyze audio.py
+-rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/analyze files.py
+-rw-r--r--   0 admin      (501) staff       (20)     4667 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/analyze images.py
+-rw-r--r--   0 admin      (501) staff       (20)     2316 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/analyze web content.py
+-rw-r--r--   0 admin      (501) staff       (20)     2559 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/auto correct python code.py
+-rw-r--r--   0 admin      (501) staff       (20)     1860 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/awesome prompts.py
+-rw-r--r--   0 admin      (501) staff       (20)     5876 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/character analysis.py
+-rw-r--r--   0 admin      (501) staff       (20)      654 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/chat.py
+-rw-r--r--   0 admin      (501) staff       (20)      762 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/contexts.py
+-rw-r--r--   0 admin      (501) staff       (20)     7220 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/counselling.py
+-rw-r--r--   0 admin      (501) staff       (20)     1688 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create ai assistants.py
+-rw-r--r--   0 admin      (501) staff       (20)     5152 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create images.py
+-rw-r--r--   0 admin      (501) staff       (20)     1262 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create maps.py
+-rw-r--r--   0 admin      (501) staff       (20)     1520 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create qrcode.py
+-rw-r--r--   0 admin      (501) staff       (20)     1522 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create statistical graphics.py
+-rw-r--r--   0 admin      (501) staff       (20)     1211 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/dates and times.py
+-rw-r--r--   0 admin      (501) staff       (20)     3950 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/download youtube or web content.py
+-rw-r--r--   0 admin      (501) staff       (20)     1862 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/edit text.py
+-rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/execute computing tasks.py
+-rw-r--r--   0 admin      (501) staff       (20)     4213 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/execute termux command.py
+-rw-r--r--   0 admin      (501) staff       (20)     6940 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/global finance.py
+-rw-r--r--   0 admin      (501) staff       (20)      975 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/improve British English.py
+-rw-r--r--   0 admin      (501) staff       (20)     1325 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/input suggestions.py
+-rw-r--r--   0 admin      (501) staff       (20)     1077 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/install python package.py
+-rw-r--r--   0 admin      (501) staff       (20)     1670 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/integrate google searches.py
+-rw-r--r--   0 admin      (501) staff       (20)     4606 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/memory.py
+-rw-r--r--   0 admin      (501) staff       (20)     8638 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/modify images.py
+-rw-r--r--   0 admin      (501) staff       (20)      944 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/open web browser.py
+-rw-r--r--   0 admin      (501) staff       (20)     1296 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/pronounce words.py
+-rw-r--r--   0 admin      (501) staff       (20)     2409 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/remove image background.py
+-rw-r--r--   0 admin      (501) staff       (20)     5898 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search chat records.py
+-rw-r--r--   0 admin      (501) staff       (20)     1156 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search financial data.py
+-rw-r--r--   0 admin      (501) staff       (20)     1966 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search latest news.py
+-rw-r--r--   0 admin      (501) staff       (20)     3479 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search sqlite.py
+-rw-r--r--   0 admin      (501) staff       (20)     1539 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search weather info.py
+-rw-r--r--   0 admin      (501) staff       (20)     3987 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/send email.py
+-rw-r--r--   0 admin      (501) staff       (20)      898 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/send tweet.py
+-rw-r--r--   0 admin      (501) staff       (20)     1280 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/send whatsapp messages.py
+-rw-r--r--   0 admin      (501) staff       (20)      528 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-r--r--   0 admin      (501) staff       (20)      242 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/qt.py
+-rw-r--r--   0 admin      (501) staff       (20)     9711 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/rag.py
+-rw-r--r--   0 admin      (501) staff       (20)      796 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/requirements.txt
+-rw-r--r--   0 admin      (501) staff       (20)     1293 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/servers.py
+-rw-r--r--   0 admin      (501) staff       (20)     7691 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/systemtray.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.689553 freegenius-0.0.92/freegenius/temp/
+-rw-r--r--   0 admin      (501) staff       (20)       36 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/temp/Readme.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.696833 freegenius-0.0.92/freegenius/utils/
+-rw-r--r--   0 admin      (501) staff       (20)   108133 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/assistant.py
+-rw-r--r--   0 admin      (501) staff       (20)    29582 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/call_chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)    17109 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/call_gemini.py
+-rw-r--r--   0 admin      (501) staff       (20)    22247 2024-04-24 12:03:40.000000 freegenius-0.0.92/freegenius/utils/call_llamacpp.py
+-rw-r--r--   0 admin      (501) staff       (20)     7664 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/call_llm.py
+-rw-r--r--   0 admin      (501) staff       (20)    18715 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/call_ollama.py
+-rw-r--r--   0 admin      (501) staff       (20)    16451 2024-04-24 12:02:43.000000 freegenius-0.0.92/freegenius/utils/config_essential.py
+-rw-r--r--   0 admin      (501) staff       (20)     2616 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/config_tools.py
+-rw-r--r--   0 admin      (501) staff       (20)     1368 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/download.py
+-rw-r--r--   0 admin      (501) staff       (20)    14296 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/get_path_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)     4888 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/ollama_models.py
+-rw-r--r--   0 admin      (501) staff       (20)     3872 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/promptValidator.py
+-rw-r--r--   0 admin      (501) staff       (20)     6973 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-r--r--   0 admin      (501) staff       (20)     7880 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/prompt_shared_key_bindings.py
+-rw-r--r--   0 admin      (501) staff       (20)    21592 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/prompts.py
+-rw-r--r--   0 admin      (501) staff       (20)     1681 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/python_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)    47445 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/shared_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)    21476 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/shortcuts.py
+-rw-r--r--   0 admin      (501) staff       (20)     8558 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/single_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)     7936 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/streaming_word_wrapper.py
+-rw-r--r--   0 admin      (501) staff       (20)     7580 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/sttLanguages.py
+-rw-r--r--   0 admin      (501) staff       (20)     4781 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/terminal_mode_dialogs.py
+-rwxr-xr-x   0 admin      (501) staff       (20)     9891 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/terminal_system_command_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)    23917 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/text_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     4352 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/tool_plugins.py
+-rw-r--r--   0 admin      (501) staff       (20)     7640 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/ttsLanguages.py
+-rw-r--r--   0 admin      (501) staff       (20)     8563 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/tts_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     4651 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/vlc_utils.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.669125 freegenius-0.0.92/freegenius.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     5856 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)     1226 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)      797 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       11 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-24 12:14:03.697433 freegenius-0.0.92/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)    10383 2024-04-24 12:04:04.000000 freegenius-0.0.92/setup.py
```

### Comparing `freegenius-0.0.91/PKG-INFO` & `freegenius-0.0.92/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.91
+Version: 0.0.92
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
@@ -18,74 +18,14 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
-Requires-Dist: openai==1.19.0
-Requires-Dist: requests
-Requires-Dist: argparse
-Requires-Dist: pendulum
-Requires-Dist: folium
-Requires-Dist: seaborn[stats]
-Requires-Dist: sympy
-Requires-Dist: numpy
-Requires-Dist: prompt_toolkit
-Requires-Dist: Pygments
-Requires-Dist: datetime
-Requires-Dist: netifaces
-Requires-Dist: geocoder
-Requires-Dist: googlesearch-python
-Requires-Dist: art
-Requires-Dist: apsw
-Requires-Dist: gTTS
-Requires-Dist: google-cloud-speech
-Requires-Dist: google-cloud-texttospeech
-Requires-Dist: google-cloud-aiplatform==1.47.0
-Requires-Dist: pywhatkit
-Requires-Dist: yt-dlp
-Requires-Dist: rembg
-Requires-Dist: qrcode
-Requires-Dist: pyperclip
-Requires-Dist: colorama
-Requires-Dist: pillow
-Requires-Dist: docker
-Requires-Dist: einops
-Requires-Dist: transformers
-Requires-Dist: torch==2.2.2
-Requires-Dist: torchvision==0.17.2
-Requires-Dist: sentence-transformers
-Requires-Dist: chromadb==0.4.24
-Requires-Dist: unstructured[all-docs]
-Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.24
-Requires-Dist: autogenstudio==0.0.56
-Requires-Dist: tiktoken
-Requires-Dist: pygame
-Requires-Dist: PySide6
-Requires-Dist: feedparser
-Requires-Dist: html2text
-Requires-Dist: pypdf
-Requires-Dist: PyMuPDF
-Requires-Dist: yfinance
-Requires-Dist: setuptools-rust
-Requires-Dist: SpeechRecognition
-Requires-Dist: openai-whisper
-Requires-Dist: soundfile==0.12.1
-Requires-Dist: sounddevice==0.4.6
-Requires-Dist: elevenlabs==1.0.3
-Requires-Dist: ollama==0.1.8
-Requires-Dist: llama-cpp-python[server]==0.2.61
-Requires-Dist: huggingface-hub
-Requires-Dist: langchain==0.1.13
-Requires-Dist: pydub
-Requires-Dist: stable-diffusion-cpp-python
-Requires-Dist: pytz
-Requires-Dist: geopy
-Requires-Dist: guidance==0.1.13
 
 # FreeGenius AI
 
 FreeGenius AI is an ambitious project sparked by the pioneering work of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). It's designed with the primary objective of offering a comprehensive suite of AI solutions that mirror the capabilities of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). However, FreeGenius AI is remarkably different in that all core features are completely free, and it doesn't require the use of an OpenAI key.
 
 As with [LetMeDoIt AI](https://github.com/eliranwong/letmedoit), FreeGenius AI is designed to be capable of engaging in intuitive conversations, executing codes, providing up-to-date information, and performing a wide range of tasks. It's designed to learn, adapt, and grow with the user, offering personalized experiences and interactions.
```

### Comparing `freegenius-0.0.91/freegenius/README.md` & `freegenius-0.0.92/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/__init__.py` & `freegenius-0.0.92/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/audio/notification1.mp3` & `freegenius-0.0.92/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/audio/notification1_mild.mp3` & `freegenius-0.0.92/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/audio/notification2.mp3` & `freegenius-0.0.92/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/audio/notification2_mild.mp3` & `freegenius-0.0.92/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/autoassist.py` & `freegenius-0.0.92/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/autobuilder.py` & `freegenius-0.0.92/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/autoretriever.py` & `freegenius-0.0.92/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/chatgpt.py` & `freegenius-0.0.92/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/codey.py` & `freegenius-0.0.92/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/commandprompt.py` & `freegenius-0.0.92/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/eTextEdit.py` & `freegenius-0.0.92/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/geminipro.py` & `freegenius-0.0.92/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/geminiprovision.py` & `freegenius-0.0.92/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/gui/chatgui.py` & `freegenius-0.0.92/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/gui/worker.py` & `freegenius-0.0.92/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/icons/FreeGenius.ico` & `freegenius-0.0.92/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/icons/FreeGenius.png` & `freegenius-0.0.92/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/icons/FreeGenius_original.png` & `freegenius-0.0.92/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/icons/ai.png` & `freegenius-0.0.92/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/icons/ai_original.png` & `freegenius-0.0.92/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/llamacpp.py` & `freegenius-0.0.92/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/main.py` & `freegenius-0.0.92/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/ollamachat.py` & `freegenius-0.0.92/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/palm2.py` & `freegenius-0.0.92/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.0.92/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.0.92/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/000_check_vlc.py` & `freegenius-0.0.92/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/add calendar event.py` & `freegenius-0.0.92/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/aliases.py` & `freegenius-0.0.92/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/analyze audio.py` & `freegenius-0.0.92/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/analyze files.py` & `freegenius-0.0.92/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/analyze images.py` & `freegenius-0.0.92/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/analyze web content.py` & `freegenius-0.0.92/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/auto correct python code.py` & `freegenius-0.0.92/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/awesome prompts.py` & `freegenius-0.0.92/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/character analysis.py` & `freegenius-0.0.92/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/chat.py` & `freegenius-0.0.92/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/contexts.py` & `freegenius-0.0.92/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/counselling.py` & `freegenius-0.0.92/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/create ai assistants.py` & `freegenius-0.0.92/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/create images.py` & `freegenius-0.0.92/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/create maps.py` & `freegenius-0.0.92/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/create qrcode.py` & `freegenius-0.0.92/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/create statistical graphics.py` & `freegenius-0.0.92/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/dates and times.py` & `freegenius-0.0.92/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/download youtube or web content.py` & `freegenius-0.0.92/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/edit text.py` & `freegenius-0.0.92/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/execute computing tasks.py` & `freegenius-0.0.92/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/execute termux command.py` & `freegenius-0.0.92/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/global finance.py` & `freegenius-0.0.92/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/improve British English.py` & `freegenius-0.0.92/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/input suggestions.py` & `freegenius-0.0.92/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/install python package.py` & `freegenius-0.0.92/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/integrate google searches.py` & `freegenius-0.0.92/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/memory.py` & `freegenius-0.0.92/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/modify images.py` & `freegenius-0.0.92/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/open web browser.py` & `freegenius-0.0.92/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/pronounce words.py` & `freegenius-0.0.92/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/remove image background.py` & `freegenius-0.0.92/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/search chat records.py` & `freegenius-0.0.92/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/search financial data.py` & `freegenius-0.0.92/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/search latest news.py` & `freegenius-0.0.92/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/search sqlite.py` & `freegenius-0.0.92/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/search weather info.py` & `freegenius-0.0.92/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/send email.py` & `freegenius-0.0.92/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/send tweet.py` & `freegenius-0.0.92/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.0.92/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.0.92/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/rag.py` & `freegenius-0.0.92/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/requirements.txt` & `freegenius-0.0.92/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/servers.py` & `freegenius-0.0.92/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/systemtray.py` & `freegenius-0.0.92/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/assistant.py` & `freegenius-0.0.92/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/call_chatgpt.py` & `freegenius-0.0.92/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/call_gemini.py` & `freegenius-0.0.92/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/call_llamacpp.py` & `freegenius-0.0.92/freegenius/utils/call_llamacpp.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,27 +60,27 @@
         try:
             loadMainModel()
         except:
             # restore default config
             print2("Errors! Restoring default main model!")
             config.llamacppMainModel_ollama_tag = ""
             config.llamacppMainModel_model_path = ""
-            config.llamacppMainModel_repo_id = "TheBloke/Mistral-7B-Instruct-v0.2-GGUF"
-            config.llamacppMainModel_filename = "mistral-7b-instruct-v0.2.Q4_K_M.gguf"
+            config.llamacppMainModel_repo_id = "TheBloke/CodeLlama-7B-Instruct-GGUF"
+            config.llamacppMainModel_filename = "codellama-7b-instruct.Q4_K_M.gguf"
             loadMainModel()
 
         try:
             downloadChatModel()
         except:
             # restore default config
             print2("Errors! Restoring default chat model!")
             config.llamacppChatModel_ollama_tag = ""
             config.llamacppChatModel_model_path = ""
-            config.llamacppChatModel_repo_id = "TheBloke/phi-2-GGUF"
-            config.llamacppChatModel_filename = "phi-2.Q4_K_M.gguf"
+            config.llamacppChatModel_repo_id = "TheBloke/Mistral-7B-Instruct-v0.2-GGUF"
+            config.llamacppChatModel_filename = "mistral-7b-instruct-v0.2.Q4_K_M.gguf"
             downloadChatModel()
 
         # Download vision model
         filename = "ggml-model-q4_k.gguf"
         llamacppVisionModel_model_path = os.path.join(llm_directory, filename)
         if not config.llamacppVisionModel_model_path or not os.path.isfile(config.llamacppVisionModel_model_path):
             config.llamacppVisionModel_model_path = llamacppVisionModel_model_path
```

### Comparing `freegenius-0.0.91/freegenius/utils/call_llm.py` & `freegenius-0.0.92/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/call_ollama.py` & `freegenius-0.0.92/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/config_essential.py` & `freegenius-0.0.92/freegenius/utils/config_essential.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     ('llamacppVisionModel_additional_options', ''),
     ('llamacppMainModel_additional_model_options', {}),
     ('llamacppMainModel_additional_chat_options', {}),
     ('llamacppChatModel_additional_model_options', {}),
     ('llamacppChatModel_additional_chat_options', {}),
     ('llamacppMainModel_ollama_tag', ''), # selected ollama hosted model to run with llamacpp
     ('llamacppMainModel_model_path', ''), # specify file path of llama.cpp model for general purpose
-    ('llamacppMainModel_repo_id', 'CodeLlama-7B-Instruct-GGUF'), # llama.cpp model used for both task execution and conversation, e.g. 'TheBloke/phi-2-GGUF', 'NousResearch/Hermes-2-Pro-Mistral-7B-GGUF', 'NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO-GGUF'
+    ('llamacppMainModel_repo_id', 'TheBloke/CodeLlama-7B-Instruct-GGUF'), # llama.cpp model used for both task execution and conversation, e.g. 'TheBloke/phi-2-GGUF', 'NousResearch/Hermes-2-Pro-Mistral-7B-GGUF', 'NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO-GGUF'
     ('llamacppMainModel_filename', 'codellama-7b-instruct.Q4_K_M.gguf'), # llama.cpp model used for both task execution and conversation, e.g. 'Hermes-2-Pro-Mistral-7B.Q4_K_M.gguf', 'Nous-Hermes-2-Mixtral-8x7B-DPO.Q4_K_M.gguf'
     ('llamacppMainModel_n_ctx', 0), # llama.cpp main model context window
     ('llamacppMainModel_max_tokens', 10000), # llama.cpp main model maximum tokens
     ('llamacppMainModel_n_gpu_layers', -1), # change to -1 to use GPU acceleration
     ('llamacppMainModel_n_batch', 512), # The batch size to use per eval
     ('llamacppChatModel_ollama_tag', ''), # selected ollama hosted model to run with llamacpp
     ('llamacppChatModel_model_path', ''), # specify file path of llama.cpp model for chat
```

### Comparing `freegenius-0.0.91/freegenius/utils/config_tools.py` & `freegenius-0.0.92/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/download.py` & `freegenius-0.0.92/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/get_path_prompt.py` & `freegenius-0.0.92/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/ollama_models.py` & `freegenius-0.0.92/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/promptValidator.py` & `freegenius-0.0.92/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.0.92/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.0.92/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/prompts.py` & `freegenius-0.0.92/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/python_utils.py` & `freegenius-0.0.92/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/shared_utils.py` & `freegenius-0.0.92/freegenius/utils/shared_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/shortcuts.py` & `freegenius-0.0.92/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/single_prompt.py` & `freegenius-0.0.92/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.0.92/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/sttLanguages.py` & `freegenius-0.0.92/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.0.92/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.0.92/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/text_utils.py` & `freegenius-0.0.92/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/tool_plugins.py` & `freegenius-0.0.92/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/ttsLanguages.py` & `freegenius-0.0.92/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/tts_utils.py` & `freegenius-0.0.92/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius/utils/vlc_utils.py` & `freegenius-0.0.92/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius.egg-info/PKG-INFO` & `freegenius-0.0.92/freegenius.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.91
+Version: 0.0.92
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
@@ -18,74 +18,14 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
-Requires-Dist: openai==1.19.0
-Requires-Dist: requests
-Requires-Dist: argparse
-Requires-Dist: pendulum
-Requires-Dist: folium
-Requires-Dist: seaborn[stats]
-Requires-Dist: sympy
-Requires-Dist: numpy
-Requires-Dist: prompt_toolkit
-Requires-Dist: Pygments
-Requires-Dist: datetime
-Requires-Dist: netifaces
-Requires-Dist: geocoder
-Requires-Dist: googlesearch-python
-Requires-Dist: art
-Requires-Dist: apsw
-Requires-Dist: gTTS
-Requires-Dist: google-cloud-speech
-Requires-Dist: google-cloud-texttospeech
-Requires-Dist: google-cloud-aiplatform==1.47.0
-Requires-Dist: pywhatkit
-Requires-Dist: yt-dlp
-Requires-Dist: rembg
-Requires-Dist: qrcode
-Requires-Dist: pyperclip
-Requires-Dist: colorama
-Requires-Dist: pillow
-Requires-Dist: docker
-Requires-Dist: einops
-Requires-Dist: transformers
-Requires-Dist: torch==2.2.2
-Requires-Dist: torchvision==0.17.2
-Requires-Dist: sentence-transformers
-Requires-Dist: chromadb==0.4.24
-Requires-Dist: unstructured[all-docs]
-Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.24
-Requires-Dist: autogenstudio==0.0.56
-Requires-Dist: tiktoken
-Requires-Dist: pygame
-Requires-Dist: PySide6
-Requires-Dist: feedparser
-Requires-Dist: html2text
-Requires-Dist: pypdf
-Requires-Dist: PyMuPDF
-Requires-Dist: yfinance
-Requires-Dist: setuptools-rust
-Requires-Dist: SpeechRecognition
-Requires-Dist: openai-whisper
-Requires-Dist: soundfile==0.12.1
-Requires-Dist: sounddevice==0.4.6
-Requires-Dist: elevenlabs==1.0.3
-Requires-Dist: ollama==0.1.8
-Requires-Dist: llama-cpp-python[server]==0.2.61
-Requires-Dist: huggingface-hub
-Requires-Dist: langchain==0.1.13
-Requires-Dist: pydub
-Requires-Dist: stable-diffusion-cpp-python
-Requires-Dist: pytz
-Requires-Dist: geopy
-Requires-Dist: guidance==0.1.13
 
 # FreeGenius AI
 
 FreeGenius AI is an ambitious project sparked by the pioneering work of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). It's designed with the primary objective of offering a comprehensive suite of AI solutions that mirror the capabilities of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). However, FreeGenius AI is remarkably different in that all core features are completely free, and it doesn't require the use of an OpenAI key.
 
 As with [LetMeDoIt AI](https://github.com/eliranwong/letmedoit), FreeGenius AI is designed to be capable of engaging in intuitive conversations, executing codes, providing up-to-date information, and performing a wide range of tasks. It's designed to learn, adapt, and grow with the user, offering personalized experiences and interactions.
```

### Comparing `freegenius-0.0.91/freegenius.egg-info/SOURCES.txt` & `freegenius-0.0.92/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius.egg-info/entry_points.txt` & `freegenius-0.0.92/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/freegenius.egg-info/requires.txt` & `freegenius-0.0.92/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.91/setup.py` & `freegenius-0.0.92/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.0.91",
+    version="0.0.92",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

