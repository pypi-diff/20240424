# Comparing `tmp/freegenius-0.0.92.tar.gz` & `tmp/freegenius-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.0.92.tar", last modified: Wed Apr 24 12:14:03 2024, max compression
+gzip compressed data, was "freegenius-0.0.93.tar", last modified: Wed Apr 24 12:49:09 2024, max compression
```

## Comparing `freegenius-0.0.92.tar` & `freegenius-0.0.93.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.697394 freegenius-0.0.92/
--rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-24 12:14:03.697153 freegenius-0.0.92/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.668412 freegenius-0.0.92/freegenius/
--rw-r--r--   0 admin      (501) staff       (20)    10056 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius/README.md
--rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.670103 freegenius-0.0.92/freegenius/audio/
--rw-r--r--   0 admin      (501) staff       (20)    15588 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/audio/notification1.mp3
--rw-r--r--   0 admin      (501) staff       (20)     2925 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/audio/notification1_mild.mp3
--rw-r--r--   0 admin      (501) staff       (20)    19428 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/audio/notification2.mp3
--rw-r--r--   0 admin      (501) staff       (20)     3693 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/audio/notification2_mild.mp3
--rw-r--r--   0 admin      (501) staff       (20)     6646 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/autoassist.py
--rw-r--r--   0 admin      (501) staff       (20)     9421 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/autobuilder.py
--rw-r--r--   0 admin      (501) staff       (20)    10727 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/autoretriever.py
--rw-r--r--   0 admin      (501) staff       (20)     6933 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)     7037 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/codey.py
--rw-r--r--   0 admin      (501) staff       (20)      833 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/commandprompt.py
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius/config.py
--rw-r--r--   0 admin      (501) staff       (20)    29583 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/eTextEdit.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.670242 freegenius-0.0.92/freegenius/files/
--rw-r--r--   0 admin      (501) staff       (20)       31 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/files/Readme.md
--rw-r--r--   0 admin      (501) staff       (20)    11372 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/geminipro.py
--rw-r--r--   0 admin      (501) staff       (20)     7838 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/geminiprovision.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.670681 freegenius-0.0.92/freegenius/gui/
--rw-r--r--   0 admin      (501) staff       (20)     9741 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/gui/chatgui.py
--rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/gui/worker.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.670851 freegenius-0.0.92/freegenius/history/
--rw-r--r--   0 admin      (501) staff       (20)       29 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/history/Readme.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.675908 freegenius-0.0.92/freegenius/icons/
--rw-r--r--   0 admin      (501) staff       (20)   158655 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/FreeGenius.ico
--rw-r--r--   0 admin      (501) staff       (20)  2549036 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/FreeGenius.png
--rw-r--r--   0 admin      (501) staff       (20)  3162696 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/FreeGenius_original.png
--rw-r--r--   0 admin      (501) staff       (20)  3141194 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/ai.png
--rw-r--r--   0 admin      (501) staff       (20)  2390858 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/icons/ai_original.png
--rw-r--r--   0 admin      (501) staff       (20)     8119 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/llamacpp.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.663122 freegenius-0.0.92/freegenius/macOS_service/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662005 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.678957 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      644 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679097 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5680 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662167 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679412 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679561 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5679 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662320 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679849 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      635 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.679979 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4100 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5684 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662480 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.680282 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      649 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.680420 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662651 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.680686 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      643 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.680820 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662816 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.681122 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      640 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.681302 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5656 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.662997 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.681600 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.681737 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.663163 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.682029 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.682198 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5692 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-r--r--   0 admin      (501) staff       (20)     7320 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/main.py
--rw-r--r--   0 admin      (501) staff       (20)    10959 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/ollamachat.py
--rw-r--r--   0 admin      (501) staff       (20)       10 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius/package_name.txt
--rw-r--r--   0 admin      (501) staff       (20)     7573 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/palm2.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.689403 freegenius-0.0.92/freegenius/plugins/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/000_check_ffmpeg.py
--rw-r--r--   0 admin      (501) staff       (20)     1616 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/000_check_pyaudio.py
--rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/000_check_vlc.py
--rw-r--r--   0 admin      (501) staff       (20)      115 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/Readme.md
--rw-r--r--   0 admin      (501) staff       (20)     6812 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/add calendar event.py
--rw-r--r--   0 admin      (501) staff       (20)     3358 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/aliases.py
--rw-r--r--   0 admin      (501) staff       (20)     7429 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/analyze audio.py
--rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/analyze files.py
--rw-r--r--   0 admin      (501) staff       (20)     4667 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/analyze images.py
--rw-r--r--   0 admin      (501) staff       (20)     2316 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/analyze web content.py
--rw-r--r--   0 admin      (501) staff       (20)     2559 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/auto correct python code.py
--rw-r--r--   0 admin      (501) staff       (20)     1860 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/awesome prompts.py
--rw-r--r--   0 admin      (501) staff       (20)     5876 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/character analysis.py
--rw-r--r--   0 admin      (501) staff       (20)      654 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/chat.py
--rw-r--r--   0 admin      (501) staff       (20)      762 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/contexts.py
--rw-r--r--   0 admin      (501) staff       (20)     7220 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/counselling.py
--rw-r--r--   0 admin      (501) staff       (20)     1688 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create ai assistants.py
--rw-r--r--   0 admin      (501) staff       (20)     5152 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create images.py
--rw-r--r--   0 admin      (501) staff       (20)     1262 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create maps.py
--rw-r--r--   0 admin      (501) staff       (20)     1520 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create qrcode.py
--rw-r--r--   0 admin      (501) staff       (20)     1522 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/create statistical graphics.py
--rw-r--r--   0 admin      (501) staff       (20)     1211 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/dates and times.py
--rw-r--r--   0 admin      (501) staff       (20)     3950 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/download youtube or web content.py
--rw-r--r--   0 admin      (501) staff       (20)     1862 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/edit text.py
--rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/execute computing tasks.py
--rw-r--r--   0 admin      (501) staff       (20)     4213 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/execute termux command.py
--rw-r--r--   0 admin      (501) staff       (20)     6940 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/global finance.py
--rw-r--r--   0 admin      (501) staff       (20)      975 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/improve British English.py
--rw-r--r--   0 admin      (501) staff       (20)     1325 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/input suggestions.py
--rw-r--r--   0 admin      (501) staff       (20)     1077 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/install python package.py
--rw-r--r--   0 admin      (501) staff       (20)     1670 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/integrate google searches.py
--rw-r--r--   0 admin      (501) staff       (20)     4606 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/memory.py
--rw-r--r--   0 admin      (501) staff       (20)     8638 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/modify images.py
--rw-r--r--   0 admin      (501) staff       (20)      944 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/open web browser.py
--rw-r--r--   0 admin      (501) staff       (20)     1296 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/pronounce words.py
--rw-r--r--   0 admin      (501) staff       (20)     2409 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/remove image background.py
--rw-r--r--   0 admin      (501) staff       (20)     5898 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search chat records.py
--rw-r--r--   0 admin      (501) staff       (20)     1156 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search financial data.py
--rw-r--r--   0 admin      (501) staff       (20)     1966 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search latest news.py
--rw-r--r--   0 admin      (501) staff       (20)     3479 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search sqlite.py
--rw-r--r--   0 admin      (501) staff       (20)     1539 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/search weather info.py
--rw-r--r--   0 admin      (501) staff       (20)     3987 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/send email.py
--rw-r--r--   0 admin      (501) staff       (20)      898 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/send tweet.py
--rw-r--r--   0 admin      (501) staff       (20)     1280 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/send whatsapp messages.py
--rw-r--r--   0 admin      (501) staff       (20)      528 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-r--r--   0 admin      (501) staff       (20)      242 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/qt.py
--rw-r--r--   0 admin      (501) staff       (20)     9711 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/rag.py
--rw-r--r--   0 admin      (501) staff       (20)      796 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/requirements.txt
--rw-r--r--   0 admin      (501) staff       (20)     1293 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/servers.py
--rw-r--r--   0 admin      (501) staff       (20)     7691 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/systemtray.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.689553 freegenius-0.0.92/freegenius/temp/
--rw-r--r--   0 admin      (501) staff       (20)       36 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/temp/Readme.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.696833 freegenius-0.0.92/freegenius/utils/
--rw-r--r--   0 admin      (501) staff       (20)   108133 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/assistant.py
--rw-r--r--   0 admin      (501) staff       (20)    29582 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/call_chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)    17109 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/call_gemini.py
--rw-r--r--   0 admin      (501) staff       (20)    22247 2024-04-24 12:03:40.000000 freegenius-0.0.92/freegenius/utils/call_llamacpp.py
--rw-r--r--   0 admin      (501) staff       (20)     7664 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/call_llm.py
--rw-r--r--   0 admin      (501) staff       (20)    18715 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/call_ollama.py
--rw-r--r--   0 admin      (501) staff       (20)    16451 2024-04-24 12:02:43.000000 freegenius-0.0.92/freegenius/utils/config_essential.py
--rw-r--r--   0 admin      (501) staff       (20)     2616 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/config_tools.py
--rw-r--r--   0 admin      (501) staff       (20)     1368 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/download.py
--rw-r--r--   0 admin      (501) staff       (20)    14296 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/get_path_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)     4888 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/ollama_models.py
--rw-r--r--   0 admin      (501) staff       (20)     3872 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/promptValidator.py
--rw-r--r--   0 admin      (501) staff       (20)     6973 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-r--r--   0 admin      (501) staff       (20)     7880 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/prompt_shared_key_bindings.py
--rw-r--r--   0 admin      (501) staff       (20)    21592 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/prompts.py
--rw-r--r--   0 admin      (501) staff       (20)     1681 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/python_utils.py
--rw-r--r--   0 admin      (501) staff       (20)    47445 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/shared_utils.py
--rw-r--r--   0 admin      (501) staff       (20)    21476 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/shortcuts.py
--rw-r--r--   0 admin      (501) staff       (20)     8558 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/single_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)     7936 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/streaming_word_wrapper.py
--rw-r--r--   0 admin      (501) staff       (20)     7580 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/sttLanguages.py
--rw-r--r--   0 admin      (501) staff       (20)     4781 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/terminal_mode_dialogs.py
--rwxr-xr-x   0 admin      (501) staff       (20)     9891 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/terminal_system_command_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)    23917 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/text_utils.py
--rw-r--r--   0 admin      (501) staff       (20)     4352 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/tool_plugins.py
--rw-r--r--   0 admin      (501) staff       (20)     7640 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/ttsLanguages.py
--rw-r--r--   0 admin      (501) staff       (20)     8563 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/tts_utils.py
--rw-r--r--   0 admin      (501) staff       (20)     4651 2024-04-24 10:05:32.000000 freegenius-0.0.92/freegenius/utils/vlc_utils.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:14:03.669125 freegenius-0.0.92/freegenius.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     5856 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)     1226 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)      797 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       11 2024-04-24 12:14:03.000000 freegenius-0.0.92/freegenius.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-24 12:14:03.697433 freegenius-0.0.92/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)    10383 2024-04-24 12:04:04.000000 freegenius-0.0.92/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.548614 freegenius-0.0.93/
+-rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-24 12:49:09.548326 freegenius-0.0.93/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.512951 freegenius-0.0.93/freegenius/
+-rw-r--r--   0 admin      (501) staff       (20)    10056 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius/README.md
+-rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.514832 freegenius-0.0.93/freegenius/audio/
+-rw-r--r--   0 admin      (501) staff       (20)    15588 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/audio/notification1.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     2925 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/audio/notification1_mild.mp3
+-rw-r--r--   0 admin      (501) staff       (20)    19428 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/audio/notification2.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     3693 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/audio/notification2_mild.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     6646 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/autoassist.py
+-rw-r--r--   0 admin      (501) staff       (20)     9421 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/autobuilder.py
+-rw-r--r--   0 admin      (501) staff       (20)    10727 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/autoretriever.py
+-rw-r--r--   0 admin      (501) staff       (20)     6933 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)     7037 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/codey.py
+-rw-r--r--   0 admin      (501) staff       (20)      833 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/commandprompt.py
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius/config.py
+-rw-r--r--   0 admin      (501) staff       (20)    29583 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/eTextEdit.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.515115 freegenius-0.0.93/freegenius/files/
+-rw-r--r--   0 admin      (501) staff       (20)       31 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/files/Readme.md
+-rw-r--r--   0 admin      (501) staff       (20)    11372 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/geminipro.py
+-rw-r--r--   0 admin      (501) staff       (20)     7838 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/geminiprovision.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.515591 freegenius-0.0.93/freegenius/gui/
+-rw-r--r--   0 admin      (501) staff       (20)     9741 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/gui/chatgui.py
+-rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/gui/worker.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.515703 freegenius-0.0.93/freegenius/history/
+-rw-r--r--   0 admin      (501) staff       (20)       29 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/history/Readme.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.528612 freegenius-0.0.93/freegenius/icons/
+-rw-r--r--   0 admin      (501) staff       (20)   158655 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/icons/FreeGenius.ico
+-rw-r--r--   0 admin      (501) staff       (20)  2549036 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/icons/FreeGenius.png
+-rw-r--r--   0 admin      (501) staff       (20)  3162696 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/icons/FreeGenius_original.png
+-rw-r--r--   0 admin      (501) staff       (20)  3141194 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/icons/ai.png
+-rw-r--r--   0 admin      (501) staff       (20)  2390858 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/icons/ai_original.png
+-rw-r--r--   0 admin      (501) staff       (20)     8119 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/llamacpp.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.508455 freegenius-0.0.93/freegenius/macOS_service/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.507344 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.533079 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      644 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.534826 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5680 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.507506 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.535391 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.535551 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5679 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.507669 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.535922 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      635 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.536085 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4100 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5684 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.507840 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.536383 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      649 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.536522 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.507998 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.536790 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      643 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.536927 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.508144 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.537195 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      640 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.537337 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5656 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.508302 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.537625 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.537768 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.508498 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.538061 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.538231 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5692 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-r--r--   0 admin      (501) staff       (20)     7320 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/main.py
+-rw-r--r--   0 admin      (501) staff       (20)    10959 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/ollamachat.py
+-rw-r--r--   0 admin      (501) staff       (20)       10 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius/package_name.txt
+-rw-r--r--   0 admin      (501) staff       (20)     7573 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/palm2.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.544111 freegenius-0.0.93/freegenius/plugins/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/000_check_ffmpeg.py
+-rw-r--r--   0 admin      (501) staff       (20)     1616 2024-04-24 12:46:57.000000 freegenius-0.0.93/freegenius/plugins/000_check_pyaudio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/000_check_vlc.py
+-rw-r--r--   0 admin      (501) staff       (20)      115 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/Readme.md
+-rw-r--r--   0 admin      (501) staff       (20)     6812 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/add calendar event.py
+-rw-r--r--   0 admin      (501) staff       (20)     3358 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/aliases.py
+-rw-r--r--   0 admin      (501) staff       (20)     7429 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/analyze audio.py
+-rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/analyze files.py
+-rw-r--r--   0 admin      (501) staff       (20)     4667 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/analyze images.py
+-rw-r--r--   0 admin      (501) staff       (20)     2316 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/analyze web content.py
+-rw-r--r--   0 admin      (501) staff       (20)     2559 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/auto correct python code.py
+-rw-r--r--   0 admin      (501) staff       (20)     1860 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/awesome prompts.py
+-rw-r--r--   0 admin      (501) staff       (20)     5876 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/character analysis.py
+-rw-r--r--   0 admin      (501) staff       (20)      654 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/chat.py
+-rw-r--r--   0 admin      (501) staff       (20)      762 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/contexts.py
+-rw-r--r--   0 admin      (501) staff       (20)     7220 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/counselling.py
+-rw-r--r--   0 admin      (501) staff       (20)     1688 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/create ai assistants.py
+-rw-r--r--   0 admin      (501) staff       (20)     5152 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/create images.py
+-rw-r--r--   0 admin      (501) staff       (20)     1262 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/create maps.py
+-rw-r--r--   0 admin      (501) staff       (20)     1520 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/create qrcode.py
+-rw-r--r--   0 admin      (501) staff       (20)     1522 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/create statistical graphics.py
+-rw-r--r--   0 admin      (501) staff       (20)     1211 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/dates and times.py
+-rw-r--r--   0 admin      (501) staff       (20)     3950 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/download youtube or web content.py
+-rw-r--r--   0 admin      (501) staff       (20)     1862 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/edit text.py
+-rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/execute computing tasks.py
+-rw-r--r--   0 admin      (501) staff       (20)     4213 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/execute termux command.py
+-rw-r--r--   0 admin      (501) staff       (20)     6940 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/global finance.py
+-rw-r--r--   0 admin      (501) staff       (20)      975 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/improve British English.py
+-rw-r--r--   0 admin      (501) staff       (20)     1325 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/input suggestions.py
+-rw-r--r--   0 admin      (501) staff       (20)     1077 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/install python package.py
+-rw-r--r--   0 admin      (501) staff       (20)     1670 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/integrate google searches.py
+-rw-r--r--   0 admin      (501) staff       (20)     4606 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/memory.py
+-rw-r--r--   0 admin      (501) staff       (20)     8638 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/modify images.py
+-rw-r--r--   0 admin      (501) staff       (20)      944 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/open web browser.py
+-rw-r--r--   0 admin      (501) staff       (20)     1296 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/pronounce words.py
+-rw-r--r--   0 admin      (501) staff       (20)     2409 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/remove image background.py
+-rw-r--r--   0 admin      (501) staff       (20)     5898 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/search chat records.py
+-rw-r--r--   0 admin      (501) staff       (20)     1156 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/search financial data.py
+-rw-r--r--   0 admin      (501) staff       (20)     1966 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/search latest news.py
+-rw-r--r--   0 admin      (501) staff       (20)     3479 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/search sqlite.py
+-rw-r--r--   0 admin      (501) staff       (20)     1539 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/search weather info.py
+-rw-r--r--   0 admin      (501) staff       (20)     3987 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/send email.py
+-rw-r--r--   0 admin      (501) staff       (20)      898 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/send tweet.py
+-rw-r--r--   0 admin      (501) staff       (20)     1280 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/send whatsapp messages.py
+-rw-r--r--   0 admin      (501) staff       (20)      528 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-r--r--   0 admin      (501) staff       (20)      242 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/qt.py
+-rw-r--r--   0 admin      (501) staff       (20)     9711 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/rag.py
+-rw-r--r--   0 admin      (501) staff       (20)      796 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/requirements.txt
+-rw-r--r--   0 admin      (501) staff       (20)     1293 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/servers.py
+-rw-r--r--   0 admin      (501) staff       (20)     7691 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/systemtray.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.544235 freegenius-0.0.93/freegenius/temp/
+-rw-r--r--   0 admin      (501) staff       (20)       36 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/temp/Readme.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.547999 freegenius-0.0.93/freegenius/utils/
+-rw-r--r--   0 admin      (501) staff       (20)   108133 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/assistant.py
+-rw-r--r--   0 admin      (501) staff       (20)    29582 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/call_chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)    17109 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/call_gemini.py
+-rw-r--r--   0 admin      (501) staff       (20)    22247 2024-04-24 12:03:40.000000 freegenius-0.0.93/freegenius/utils/call_llamacpp.py
+-rw-r--r--   0 admin      (501) staff       (20)     7664 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/call_llm.py
+-rw-r--r--   0 admin      (501) staff       (20)    18715 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/call_ollama.py
+-rw-r--r--   0 admin      (501) staff       (20)    16451 2024-04-24 12:02:43.000000 freegenius-0.0.93/freegenius/utils/config_essential.py
+-rw-r--r--   0 admin      (501) staff       (20)     2616 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/config_tools.py
+-rw-r--r--   0 admin      (501) staff       (20)     1368 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/download.py
+-rw-r--r--   0 admin      (501) staff       (20)    14296 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/get_path_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)     4888 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/ollama_models.py
+-rw-r--r--   0 admin      (501) staff       (20)     3872 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/promptValidator.py
+-rw-r--r--   0 admin      (501) staff       (20)     6973 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-r--r--   0 admin      (501) staff       (20)     7880 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/prompt_shared_key_bindings.py
+-rw-r--r--   0 admin      (501) staff       (20)    21592 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/prompts.py
+-rw-r--r--   0 admin      (501) staff       (20)     1681 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/python_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)    47445 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/shared_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)    21476 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/shortcuts.py
+-rw-r--r--   0 admin      (501) staff       (20)     8558 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/single_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)     7936 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/streaming_word_wrapper.py
+-rw-r--r--   0 admin      (501) staff       (20)     7580 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/sttLanguages.py
+-rw-r--r--   0 admin      (501) staff       (20)     4781 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/terminal_mode_dialogs.py
+-rwxr-xr-x   0 admin      (501) staff       (20)     9891 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/terminal_system_command_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)    23917 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/text_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     4352 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/tool_plugins.py
+-rw-r--r--   0 admin      (501) staff       (20)     7640 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/ttsLanguages.py
+-rw-r--r--   0 admin      (501) staff       (20)     8563 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/tts_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     4651 2024-04-24 10:05:32.000000 freegenius-0.0.93/freegenius/utils/vlc_utils.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 12:49:09.513698 freegenius-0.0.93/freegenius.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     5856 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)     1226 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)      797 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       11 2024-04-24 12:49:09.000000 freegenius-0.0.93/freegenius.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-24 12:49:09.548662 freegenius-0.0.93/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)    10383 2024-04-24 12:47:13.000000 freegenius-0.0.93/setup.py
```

### Comparing `freegenius-0.0.92/PKG-INFO` & `freegenius-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.92
+Version: 0.0.93
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.0.92/freegenius/README.md` & `freegenius-0.0.93/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/__init__.py` & `freegenius-0.0.93/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/audio/notification1.mp3` & `freegenius-0.0.93/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/audio/notification1_mild.mp3` & `freegenius-0.0.93/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/audio/notification2.mp3` & `freegenius-0.0.93/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/audio/notification2_mild.mp3` & `freegenius-0.0.93/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/autoassist.py` & `freegenius-0.0.93/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/autobuilder.py` & `freegenius-0.0.93/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/autoretriever.py` & `freegenius-0.0.93/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/chatgpt.py` & `freegenius-0.0.93/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/codey.py` & `freegenius-0.0.93/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/commandprompt.py` & `freegenius-0.0.93/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/eTextEdit.py` & `freegenius-0.0.93/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/geminipro.py` & `freegenius-0.0.93/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/geminiprovision.py` & `freegenius-0.0.93/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/gui/chatgui.py` & `freegenius-0.0.93/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/gui/worker.py` & `freegenius-0.0.93/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/icons/FreeGenius.ico` & `freegenius-0.0.93/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/icons/FreeGenius.png` & `freegenius-0.0.93/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/icons/FreeGenius_original.png` & `freegenius-0.0.93/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/icons/ai.png` & `freegenius-0.0.93/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/icons/ai_original.png` & `freegenius-0.0.93/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/llamacpp.py` & `freegenius-0.0.93/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.0.93/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/main.py` & `freegenius-0.0.93/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/ollamachat.py` & `freegenius-0.0.93/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/palm2.py` & `freegenius-0.0.93/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.0.93/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.0.93/freegenius/plugins/000_check_pyaudio.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,25 +13,25 @@
     config.pyaudioInstalled = True
 except:
     if config.isTermux:
         config.pyaudioInstalled = False
         #print2("Installing 'portaudio' and 'Pyaudio' ...")
         #os.system("pkg install portaudio")
         #config.pyaudioInstalled = True if installPipPackage("--upgrade PyAudio") else False
+    elif isCommandInstalled("brew"):
+        print2("Installing 'portaudio' and 'Pyaudio' ...")
+        os.system("brew install portaudio")
+        config.pyaudioInstalled = True if installPipPackage("--upgrade PyAudio") else False
     elif isCommandInstalled("apt"):
         print2("Installing 'portaudio19-dev' and 'Pyaudio' ...")
         os.system("sudo apt update && sudo apt install portaudio19-dev")
         config.pyaudioInstalled = True if installPipPackage("--upgrade PyAudio") else False
     elif isCommandInstalled("dnf"):
         print2("Installing 'portaudio-devel' and 'Pyaudio' ...")
         os.system("sudo dnf update && sudo dnf install portaudio-devel")
         config.pyaudioInstalled = True if installPipPackage("--upgrade PyAudio") else False
-    elif isCommandInstalled("brew"):
-        print2("Installing 'portaudio' and 'Pyaudio' ...")
-        os.system("brew install portaudio")
-        config.pyaudioInstalled = True if installPipPackage("--upgrade PyAudio") else False
     else:
         config.pyaudioInstalled = False
 
 if not config.pyaudioInstalled:
     print3("Note: 'ffmpeg' is not installed.")
     print1("It is essential for built-in voice typing feature.")
```

### Comparing `freegenius-0.0.92/freegenius/plugins/000_check_vlc.py` & `freegenius-0.0.93/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/add calendar event.py` & `freegenius-0.0.93/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/aliases.py` & `freegenius-0.0.93/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/analyze audio.py` & `freegenius-0.0.93/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/analyze files.py` & `freegenius-0.0.93/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/analyze images.py` & `freegenius-0.0.93/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/analyze web content.py` & `freegenius-0.0.93/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/auto correct python code.py` & `freegenius-0.0.93/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/awesome prompts.py` & `freegenius-0.0.93/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/character analysis.py` & `freegenius-0.0.93/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/chat.py` & `freegenius-0.0.93/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/contexts.py` & `freegenius-0.0.93/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/counselling.py` & `freegenius-0.0.93/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/create ai assistants.py` & `freegenius-0.0.93/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/create images.py` & `freegenius-0.0.93/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/create maps.py` & `freegenius-0.0.93/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/create qrcode.py` & `freegenius-0.0.93/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/create statistical graphics.py` & `freegenius-0.0.93/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/dates and times.py` & `freegenius-0.0.93/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/download youtube or web content.py` & `freegenius-0.0.93/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/edit text.py` & `freegenius-0.0.93/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/execute computing tasks.py` & `freegenius-0.0.93/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/execute termux command.py` & `freegenius-0.0.93/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/global finance.py` & `freegenius-0.0.93/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/improve British English.py` & `freegenius-0.0.93/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/input suggestions.py` & `freegenius-0.0.93/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/install python package.py` & `freegenius-0.0.93/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/integrate google searches.py` & `freegenius-0.0.93/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/memory.py` & `freegenius-0.0.93/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/modify images.py` & `freegenius-0.0.93/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/open web browser.py` & `freegenius-0.0.93/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/pronounce words.py` & `freegenius-0.0.93/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/remove image background.py` & `freegenius-0.0.93/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/search chat records.py` & `freegenius-0.0.93/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/search financial data.py` & `freegenius-0.0.93/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/search latest news.py` & `freegenius-0.0.93/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/search sqlite.py` & `freegenius-0.0.93/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/search weather info.py` & `freegenius-0.0.93/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/send email.py` & `freegenius-0.0.93/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/send tweet.py` & `freegenius-0.0.93/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.0.93/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.0.93/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/rag.py` & `freegenius-0.0.93/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/requirements.txt` & `freegenius-0.0.93/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/servers.py` & `freegenius-0.0.93/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/systemtray.py` & `freegenius-0.0.93/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/assistant.py` & `freegenius-0.0.93/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/call_chatgpt.py` & `freegenius-0.0.93/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/call_gemini.py` & `freegenius-0.0.93/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/call_llamacpp.py` & `freegenius-0.0.93/freegenius/utils/call_llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/call_llm.py` & `freegenius-0.0.93/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/call_ollama.py` & `freegenius-0.0.93/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/config_essential.py` & `freegenius-0.0.93/freegenius/utils/config_essential.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/config_tools.py` & `freegenius-0.0.93/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/download.py` & `freegenius-0.0.93/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/get_path_prompt.py` & `freegenius-0.0.93/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/ollama_models.py` & `freegenius-0.0.93/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/promptValidator.py` & `freegenius-0.0.93/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.0.93/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.0.93/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/prompts.py` & `freegenius-0.0.93/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/python_utils.py` & `freegenius-0.0.93/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/shared_utils.py` & `freegenius-0.0.93/freegenius/utils/shared_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/shortcuts.py` & `freegenius-0.0.93/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/single_prompt.py` & `freegenius-0.0.93/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.0.93/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/sttLanguages.py` & `freegenius-0.0.93/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.0.93/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.0.93/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/text_utils.py` & `freegenius-0.0.93/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/tool_plugins.py` & `freegenius-0.0.93/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/ttsLanguages.py` & `freegenius-0.0.93/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/tts_utils.py` & `freegenius-0.0.93/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius/utils/vlc_utils.py` & `freegenius-0.0.93/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius.egg-info/PKG-INFO` & `freegenius-0.0.93/freegenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.92
+Version: 0.0.93
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.0.92/freegenius.egg-info/SOURCES.txt` & `freegenius-0.0.93/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius.egg-info/entry_points.txt` & `freegenius-0.0.93/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/freegenius.egg-info/requires.txt` & `freegenius-0.0.93/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.92/setup.py` & `freegenius-0.0.93/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.0.92",
+    version="0.0.93",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

