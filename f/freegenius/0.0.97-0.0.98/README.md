# Comparing `tmp/freegenius-0.0.97.tar.gz` & `tmp/freegenius-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.0.97.tar", last modified: Thu Apr 25 15:50:35 2024, max compression
+gzip compressed data, was "freegenius-0.0.98.tar", last modified: Thu Apr 25 20:48:54 2024, max compression
```

## Comparing `freegenius-0.0.97.tar` & `freegenius-0.0.98.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.866748 freegenius-0.0.97/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    13438 2024-04-25 15:50:35.866748 freegenius-0.0.97/PKG-INFO
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10310 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius/README.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.0.97/freegenius/__init__.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/audio/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.0.97/freegenius/audio/notification1.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.0.97/freegenius/audio/notification1_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.0.97/freegenius/audio/notification2.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.0.97/freegenius/audio/notification2_mild.mp3
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6646 2024-04-11 14:37:13.000000 freegenius-0.0.97/freegenius/autoassist.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.0.97/freegenius/autobuilder.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10727 2024-04-11 14:37:13.000000 freegenius-0.0.97/freegenius/autoretriever.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.0.97/freegenius/chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.0.97/freegenius/codey.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.0.97/freegenius/commandprompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius/config.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.0.97/freegenius/eTextEdit.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/files/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.0.97/freegenius/files/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.0.97/freegenius/geminipro.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.0.97/freegenius/geminiprovision.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/gui/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.0.97/freegenius/gui/chatgui.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.0.97/freegenius/gui/worker.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/history/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.0.97/freegenius/history/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.842748 freegenius-0.0.97/freegenius/icons/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.0.97/freegenius/icons/FreeGenius.ico
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.0.97/freegenius/icons/FreeGenius.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.0.97/freegenius/icons/FreeGenius_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.0.97/freegenius/icons/ai.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.0.97/freegenius/icons/ai_original.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.0.97/freegenius/llamacpp.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.814748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.846748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.846748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.814748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.846748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.854748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.854748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.0.97/freegenius/main.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.0.97/freegenius/ollamachat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius/package_name.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.0.97/freegenius/palm2.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.858748 freegenius-0.0.97/freegenius/plugins/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.0.97/freegenius/plugins/000_check_ffmpeg.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.0.97/freegenius/plugins/000_check_pyaudio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.0.97/freegenius/plugins/000_check_vlc.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.0.97/freegenius/plugins/Readme.md
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.0.97/freegenius/plugins/add calendar event.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/aliases.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7429 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/plugins/analyze audio.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/plugins/analyze files.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4667 2024-04-11 14:37:13.000000 freegenius-0.0.97/freegenius/plugins/analyze images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.0.97/freegenius/plugins/analyze web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.0.97/freegenius/plugins/auto correct python code.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/awesome prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/character analysis.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.0.97/freegenius/plugins/chat.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.0.97/freegenius/plugins/contexts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/counselling.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.0.97/freegenius/plugins/create ai assistants.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5152 2024-04-11 14:32:24.000000 freegenius-0.0.97/freegenius/plugins/create images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/create maps.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.0.97/freegenius/plugins/create qrcode.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/create statistical graphics.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.0.97/freegenius/plugins/dates and times.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.0.97/freegenius/plugins/download youtube or web content.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.0.97/freegenius/plugins/edit text.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.0.97/freegenius/plugins/execute computing tasks.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.0.97/freegenius/plugins/execute termux command.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/global finance.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/improve British English.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.0.97/freegenius/plugins/input suggestions.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.0.97/freegenius/plugins/install python package.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.0.97/freegenius/plugins/integrate google searches.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.0.97/freegenius/plugins/memory.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8638 2024-04-11 14:37:13.000000 freegenius-0.0.97/freegenius/plugins/modify images.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.0.97/freegenius/plugins/open web browser.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.0.97/freegenius/plugins/pronounce words.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/remove image background.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5898 2024-04-10 13:47:59.000000 freegenius-0.0.97/freegenius/plugins/search chat records.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/search financial data.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.0.97/freegenius/plugins/search latest news.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.0.97/freegenius/plugins/search sqlite.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/search weather info.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.0.97/freegenius/plugins/send email.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.0.97/freegenius/plugins/send tweet.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.0.97/freegenius/plugins/send whatsapp messages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.0.97/freegenius/qt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/rag.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      828 2024-04-25 15:49:57.000000 freegenius-0.0.97/freegenius/requirements.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1293 2024-04-11 16:00:15.000000 freegenius-0.0.97/freegenius/servers.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7691 2024-04-16 20:07:13.000000 freegenius-0.0.97/freegenius/systemtray.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.858748 freegenius-0.0.97/freegenius/temp/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.0.97/freegenius/temp/Readme.md
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.862748 freegenius-0.0.97/freegenius/utils/
--rw-rw-r--   0 eliran    (1000) eliran    (1000)   108994 2024-04-25 15:33:09.000000 freegenius-0.0.97/freegenius/utils/assistant.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    29718 2024-04-25 13:47:07.000000 freegenius-0.0.97/freegenius/utils/call_chatgpt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17236 2024-04-25 13:53:07.000000 freegenius-0.0.97/freegenius/utils/call_gemini.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    22590 2024-04-25 13:45:00.000000 freegenius-0.0.97/freegenius/utils/call_llamacpp.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7664 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/utils/call_llm.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    18680 2024-04-25 13:45:52.000000 freegenius-0.0.97/freegenius/utils/call_ollama.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    17552 2024-04-25 15:16:21.000000 freegenius-0.0.97/freegenius/utils/config_essential.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.0.97/freegenius/utils/config_tools.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.0.97/freegenius/utils/download.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.0.97/freegenius/utils/get_path_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.0.97/freegenius/utils/ollama_models.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.0.97/freegenius/utils/promptValidator.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.0.97/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.0.97/freegenius/utils/prompt_shared_key_bindings.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.0.97/freegenius/utils/prompts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.0.97/freegenius/utils/python_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    49430 2024-04-25 15:16:34.000000 freegenius-0.0.97/freegenius/utils/shared_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.0.97/freegenius/utils/shortcuts.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.0.97/freegenius/utils/single_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/utils/streaming_word_wrapper.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.0.97/freegenius/utils/sttLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.0.97/freegenius/utils/terminal_mode_dialogs.py
--rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.0.97/freegenius/utils/terminal_system_command_prompt.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.0.97/freegenius/utils/text_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.0.97/freegenius/utils/tool_plugins.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.0.97/freegenius/utils/ttsLanguages.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.0.97/freegenius/utils/tts_utils.py
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.0.97/freegenius/utils/vlc_utils.py
-drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.862748 freegenius-0.0.97/freegenius.egg-info/
--rw-r--r--   0 eliran    (1000) eliran    (1000)    13438 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/PKG-INFO
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     5856 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/SOURCES.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/dependency_links.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)     1226 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/entry_points.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)      829 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/requires.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/top_level.txt
--rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-25 15:50:35.866748 freegenius-0.0.97/setup.cfg
--rw-rw-r--   0 eliran    (1000) eliran    (1000)    10383 2024-04-25 15:19:09.000000 freegenius-0.0.97/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.897642 freegenius-0.0.98/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    13438 2024-04-25 20:48:54.897642 freegenius-0.0.98/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.865643 freegenius-0.0.98/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10310 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.0.98/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.865643 freegenius-0.0.98/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.0.98/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.0.98/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.0.98/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.0.98/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6646 2024-04-11 14:37:13.000000 freegenius-0.0.98/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.0.98/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10727 2024-04-11 14:37:13.000000 freegenius-0.0.98/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.0.98/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.0.98/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.0.98/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.0.98/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.865643 freegenius-0.0.98/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.0.98/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.0.98/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.0.98/freegenius/geminiprovision.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.865643 freegenius-0.0.98/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.0.98/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.0.98/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.865643 freegenius-0.0.98/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.0.98/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.877643 freegenius-0.0.98/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.0.98/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.0.98/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.0.98/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.0.98/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.0.98/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.0.98/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.881643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.885643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.885643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.885643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.885643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.861643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.885643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.885643 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.0.98/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.0.98/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.0.98/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.889643 freegenius-0.0.98/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.0.98/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.0.98/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.0.98/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.0.98/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.0.98/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.0.98/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7429 2024-04-09 10:22:46.000000 freegenius-0.0.98/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.0.98/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4667 2024-04-11 14:37:13.000000 freegenius-0.0.98/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.0.98/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.0.98/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.0.98/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.0.98/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.0.98/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.0.98/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.0.98/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.0.98/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5152 2024-04-11 14:32:24.000000 freegenius-0.0.98/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.0.98/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.0.98/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.0.98/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.0.98/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.0.98/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.0.98/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.0.98/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.0.98/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.0.98/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.0.98/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.0.98/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.0.98/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.0.98/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.0.98/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8638 2024-04-11 14:37:13.000000 freegenius-0.0.98/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.0.98/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.0.98/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.0.98/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5898 2024-04-10 13:47:59.000000 freegenius-0.0.98/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.0.98/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.0.98/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.0.98/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.0.98/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.0.98/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.0.98/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.0.98/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.0.98/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.0.98/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.0.98/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      828 2024-04-25 15:49:57.000000 freegenius-0.0.98/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1359 2024-04-25 20:30:31.000000 freegenius-0.0.98/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7691 2024-04-16 20:07:13.000000 freegenius-0.0.98/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.889643 freegenius-0.0.98/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.0.98/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.893643 freegenius-0.0.98/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   108994 2024-04-25 15:33:09.000000 freegenius-0.0.98/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29718 2024-04-25 13:47:07.000000 freegenius-0.0.98/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17236 2024-04-25 13:53:07.000000 freegenius-0.0.98/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    24579 2024-04-25 20:41:47.000000 freegenius-0.0.98/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7664 2024-04-09 10:22:46.000000 freegenius-0.0.98/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18680 2024-04-25 13:45:52.000000 freegenius-0.0.98/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17977 2024-04-25 20:25:22.000000 freegenius-0.0.98/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.0.98/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.0.98/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.0.98/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.0.98/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.0.98/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.0.98/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.0.98/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.0.98/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.0.98/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    49508 2024-04-25 20:30:07.000000 freegenius-0.0.98/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.0.98/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.0.98/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.0.98/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.0.98/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.0.98/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.0.98/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.0.98/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.0.98/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.0.98/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.0.98/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.0.98/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 20:48:54.897642 freegenius-0.0.98/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    13438 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5856 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1226 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      829 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-25 20:48:54.000000 freegenius-0.0.98/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-25 20:48:54.897642 freegenius-0.0.98/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10383 2024-04-25 20:47:58.000000 freegenius-0.0.98/setup.py
```

### Comparing `freegenius-0.0.97/PKG-INFO` & `freegenius-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.97
+Version: 0.0.98
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.0.97/freegenius/README.md` & `freegenius-0.0.98/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/__init__.py` & `freegenius-0.0.98/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/audio/notification1.mp3` & `freegenius-0.0.98/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/audio/notification1_mild.mp3` & `freegenius-0.0.98/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/audio/notification2.mp3` & `freegenius-0.0.98/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/audio/notification2_mild.mp3` & `freegenius-0.0.98/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/autoassist.py` & `freegenius-0.0.98/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/autobuilder.py` & `freegenius-0.0.98/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/autoretriever.py` & `freegenius-0.0.98/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/chatgpt.py` & `freegenius-0.0.98/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/codey.py` & `freegenius-0.0.98/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/commandprompt.py` & `freegenius-0.0.98/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/eTextEdit.py` & `freegenius-0.0.98/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/geminipro.py` & `freegenius-0.0.98/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/geminiprovision.py` & `freegenius-0.0.98/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/gui/chatgui.py` & `freegenius-0.0.98/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/gui/worker.py` & `freegenius-0.0.98/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/icons/FreeGenius.ico` & `freegenius-0.0.98/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/icons/FreeGenius.png` & `freegenius-0.0.98/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/icons/FreeGenius_original.png` & `freegenius-0.0.98/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/icons/ai.png` & `freegenius-0.0.98/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/icons/ai_original.png` & `freegenius-0.0.98/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/llamacpp.py` & `freegenius-0.0.98/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.0.98/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/main.py` & `freegenius-0.0.98/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/ollamachat.py` & `freegenius-0.0.98/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/palm2.py` & `freegenius-0.0.98/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.0.98/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.0.98/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/000_check_vlc.py` & `freegenius-0.0.98/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/add calendar event.py` & `freegenius-0.0.98/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/aliases.py` & `freegenius-0.0.98/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/analyze audio.py` & `freegenius-0.0.98/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/analyze files.py` & `freegenius-0.0.98/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/analyze images.py` & `freegenius-0.0.98/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/analyze web content.py` & `freegenius-0.0.98/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/auto correct python code.py` & `freegenius-0.0.98/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/awesome prompts.py` & `freegenius-0.0.98/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/character analysis.py` & `freegenius-0.0.98/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/chat.py` & `freegenius-0.0.98/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/contexts.py` & `freegenius-0.0.98/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/counselling.py` & `freegenius-0.0.98/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/create ai assistants.py` & `freegenius-0.0.98/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/create images.py` & `freegenius-0.0.98/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/create maps.py` & `freegenius-0.0.98/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/create qrcode.py` & `freegenius-0.0.98/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/create statistical graphics.py` & `freegenius-0.0.98/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/dates and times.py` & `freegenius-0.0.98/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/download youtube or web content.py` & `freegenius-0.0.98/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/edit text.py` & `freegenius-0.0.98/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/execute computing tasks.py` & `freegenius-0.0.98/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/execute termux command.py` & `freegenius-0.0.98/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/global finance.py` & `freegenius-0.0.98/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/improve British English.py` & `freegenius-0.0.98/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/input suggestions.py` & `freegenius-0.0.98/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/install python package.py` & `freegenius-0.0.98/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/integrate google searches.py` & `freegenius-0.0.98/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/memory.py` & `freegenius-0.0.98/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/modify images.py` & `freegenius-0.0.98/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/open web browser.py` & `freegenius-0.0.98/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/pronounce words.py` & `freegenius-0.0.98/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/remove image background.py` & `freegenius-0.0.98/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/search chat records.py` & `freegenius-0.0.98/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/search financial data.py` & `freegenius-0.0.98/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/search latest news.py` & `freegenius-0.0.98/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/search sqlite.py` & `freegenius-0.0.98/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/search weather info.py` & `freegenius-0.0.98/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/send email.py` & `freegenius-0.0.98/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/send tweet.py` & `freegenius-0.0.98/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.0.98/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.0.98/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/rag.py` & `freegenius-0.0.98/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/requirements.txt` & `freegenius-0.0.98/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/servers.py` & `freegenius-0.0.98/freegenius/servers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from freegenius import config, isServerAlive, print2
 import os, sys
 
 def chat():
     if isServerAlive("127.0.0.1", config.llamacppMainModel_server_port):
         print2(f"A service is already running at 127.0.0.1:{config.llamacppMainModel_server_port}!")
         return None
-    cmd = f"""{sys.executable} -m llama_cpp.server --port {config.llamacppMainModel_server_port} --model "{config.llamacppMainModel_model_path}" --verbose True --chat_format chatml --n_ctx {config.llamacppMainModel_n_ctx} --n_gpu_layers {config.llamacppMainModel_n_gpu_layers} --n_batch {config.llamacppMainModel_n_batch}"""
+    cmd = f"""{sys.executable} -m llama_cpp.server --port {config.llamacppMainModel_server_port} --model "{config.llamacppMainModel_model_path}" --verbose True --chat_format chatml --n_ctx {config.llamacppMainModel_n_ctx} --n_gpu_layers {config.llamacppMainModel_n_gpu_layers} --n_batch {config.llamacppMainModel_n_batch} {config.llamacppMainModel_additional_server_options}"""
     os.system(cmd)
 
 def vision():
     if isServerAlive("127.0.0.1", config.llamacppVisionModel_server_port):
         print2(f"A service is already running at 127.0.0.1:{config.llamacppVisionModel_server_port}!")
         return None
-    cmd = f"""{sys.executable} -m llama_cpp.server --port {config.llamacppVisionModel_server_port} --model "{config.llamacppVisionModel_model_path}" --clip_model_path {config.llamacppVisionModel_clip_model_path} --verbose True --chat_format llava-1-5 --n_ctx {config.llamacppMainModel_n_ctx} --n_gpu_layers {config.llamacppMainModel_n_gpu_layers} --n_batch {config.llamacppMainModel_n_batch} {config.llamacppVisionModel_additional_options}"""
+    cmd = f"""{sys.executable} -m llama_cpp.server --port {config.llamacppVisionModel_server_port} --model "{config.llamacppVisionModel_model_path}" --clip_model_path {config.llamacppVisionModel_clip_model_path} --verbose True --chat_format llava-1-5 --n_ctx {config.llamacppVisionModel_n_ctx} --n_gpu_layers {config.llamacppVisionModel_n_gpu_layers} --n_batch {config.llamacppVisionModel_n_batch} {config.llamacppVisionModel_additional_server_options}"""
     os.system(cmd)
```

### Comparing `freegenius-0.0.97/freegenius/systemtray.py` & `freegenius-0.0.98/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/assistant.py` & `freegenius-0.0.98/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/call_chatgpt.py` & `freegenius-0.0.98/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/call_gemini.py` & `freegenius-0.0.98/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/call_llamacpp.py` & `freegenius-0.0.98/freegenius/utils/call_llamacpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from freegenius import config, showErrors, get_or_create_collection, query_vectors, getDeviceInfo, isValidPythodCode, executeToolFunction, toParameterSchema
-from freegenius import print1, print2, print3, selectTool, getPythonFunctionResponse, extractPythonCode, downloadStableDiffusionFiles, screening, isToolRequired
+from freegenius import print1, print2, print3, selectTool, getPythonFunctionResponse, extractPythonCode, downloadStableDiffusionFiles, isToolRequired, encode_image
 from typing import Optional
 from llama_cpp import Llama
+from llama_cpp.llama_chat_format import Llava15ChatHandler
 from prompt_toolkit import prompt
 from pathlib import Path
 from huggingface_hub import hf_hub_download
 import traceback, json, re, os, pprint, copy, datetime
 
 
 class CallLlamaCpp:
@@ -183,14 +184,56 @@
             temperature=temperature if temperature is not None else config.llmTemperature,
             max_tokens=max_tokens if max_tokens is not None else config.llamacppMainModel_max_tokens,
             stream=True,
             **config.llamacppMainModel_additional_chat_options,
         )
 
     @staticmethod
+    def img_to_txt(file_path: str, query: str="Describe this image in detail please.", temperature: Optional[float]=None, max_tokens: Optional[int]=None, messages: Optional[list]=None):
+        chat_handler = Llava15ChatHandler(clip_model_path=config.llamacppVisionModel_clip_model_path)
+        llm = Llama(
+            model_path=config.llamacppVisionModel_model_path,
+            chat_handler=chat_handler,
+            logits_all=True, # needed to make llava work
+            n_ctx=config.llamacppVisionModel_n_ctx, # n_ctx should be increased to accomodate the image embedding
+            n_batch=config.llamacppVisionModel_n_batch,
+            verbose=config.llamacppVisionModel_verbose,
+            n_gpu_layers=config.llamacppVisionModel_n_gpu_layers,
+            **config.llamacppVisionModel_additional_model_options,
+        )
+        # update messages
+        if messages is None:
+            messages = [
+                {
+                    "role": "system",
+                    "content": "You are an assistant who perfectly describes images.",
+                },
+            ]
+        messages.append(
+            {
+                "role": "user",
+                "content": [
+                    {"type": "image_url", "image_url": {"url": encode_image(file_path)}},
+                    {"type" : "text", "text": query},
+                ]
+            }
+        )
+        try:
+            completion = llm.create_chat_completion(
+                messages=messages,
+                temperature=temperature if temperature is not None else config.llmTemperature,
+                max_tokens=max_tokens if max_tokens is not None else config.llamacppVisionModel_max_tokens,
+                stream=False,
+                **config.llamacppVisionModel_additional_chat_options,
+            )
+            return completion["choices"][0]["message"].get("content", "")
+        except:
+            return ""
+
+    @staticmethod
     def getResponseDict(messages: list, schema: dict={}, temperature: Optional[float]=None, max_tokens: Optional[int]=None) -> dict:
         schema = toParameterSchema(schema)
         try:
             completion = config.llamacppMainModel.create_chat_completion(
                 messages=messages,
                 response_format={"type": "json_object", "schema": schema} if schema else {"type": "json_object"},
                 temperature=temperature if temperature is not None else config.llmTemperature,
```

### Comparing `freegenius-0.0.97/freegenius/utils/call_llm.py` & `freegenius-0.0.98/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/call_ollama.py` & `freegenius-0.0.98/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/config_essential.py` & `freegenius-0.0.98/freegenius/utils/config_essential.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,15 +64,22 @@
     ('llamacppMainModel_verbose', False),
     ('llamacppChatModel_verbose', False),
     ('llamacppVisionModel_verbose', False),
     ('llamacppMainModel_server_port', 8000),
     ('llamacppVisionModel_server_port', 8001),
     ('llamacppVisionModel_model_path', ''), # specify file path of llama.cpp model for vision
     ('llamacppVisionModel_clip_model_path', ''), # specify file path of llama.cpp clip model for vision
-    ('llamacppVisionModel_additional_options', ''),
+    ('llamacppVisionModel_additional_server_options', ''),
+    ('llamacppVisionModel_additional_model_options', {}),
+    ('llamacppVisionModel_additional_chat_options', {}),
+    ('llamacppVisionModel_max_tokens', 10000), # llama.cpp vision model maximum tokens
+    ('llamacppVisionModel_n_gpu_layers', 0), # -1 automatic if gpu is in place
+    ('llamacppVisionModel_n_batch', 512),
+    ('llamacppVisionModel_n_ctx', 0),
+    ('llamacppMainModel_additional_server_options', ''),
     ('llamacppMainModel_additional_model_options', {}),
     ('llamacppMainModel_additional_chat_options', {}),
     ('llamacppChatModel_additional_model_options', {}),
     ('llamacppChatModel_additional_chat_options', {}),
     ('llamacppMainModel_ollama_tag', ''), # selected ollama hosted model to run with llamacpp
     ('llamacppMainModel_model_path', ''), # specify file path of llama.cpp model for general purpose
     ('llamacppMainModel_repo_id', 'TheBloke/CodeLlama-7B-Instruct-GGUF'), # llama.cpp model used for both task execution and conversation, e.g. 'TheBloke/phi-2-GGUF', 'NousResearch/Hermes-2-Pro-Mistral-7B-GGUF', 'NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO-GGUF'
```

### Comparing `freegenius-0.0.97/freegenius/utils/config_tools.py` & `freegenius-0.0.98/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/download.py` & `freegenius-0.0.98/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/get_path_prompt.py` & `freegenius-0.0.98/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/ollama_models.py` & `freegenius-0.0.98/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/promptValidator.py` & `freegenius-0.0.98/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.0.98/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.0.98/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/prompts.py` & `freegenius-0.0.98/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/python_utils.py` & `freegenius-0.0.98/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/shared_utils.py` & `freegenius-0.0.98/freegenius/utils/shared_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         config.autogenstudioServer = None
 
 def startLlamacppServer():
     try:
         if not hasattr(config, "llamacppServer") or config.llamacppServer is None:
             config.llamacppServer = None
             print2("Running llama.cpp chat server ...")
-            cmd = f"""{sys.executable} -m llama_cpp.server --port {config.llamacppMainModel_server_port} --model "{config.llamacppMainModel_model_path}" --verbose {config.llamacppMainModel_verbose} --chat_format chatml --n_ctx {config.llamacppMainModel_n_ctx} --n_gpu_layers {config.llamacppMainModel_n_gpu_layers} --n_batch {config.llamacppMainModel_n_batch}"""
+            cmd = f"""{sys.executable} -m llama_cpp.server --port {config.llamacppMainModel_server_port} --model "{config.llamacppMainModel_model_path}" --verbose {config.llamacppMainModel_verbose} --chat_format chatml --n_ctx {config.llamacppMainModel_n_ctx} --n_gpu_layers {config.llamacppMainModel_n_gpu_layers} --n_batch {config.llamacppMainModel_n_batch} {config.llamacppMainModel_additional_server_options}"""
             config.llamacppServer = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, preexec_fn=os.setsid)
             while not isServerAlive("127.0.0.1", config.llamacppMainModel_server_port):
                 # wait til the server is up
                 ...
     except:
         print2(f'''Failed to run llama.cpp server at "localhost:{config.llamacppMainModel_server_port}"!''')
         config.llamacppServer = None
@@ -250,15 +250,15 @@
 
 def startLlamacppVisionServer():
     try:
         if not hasattr(config, "llamacppVisionServer") or config.llamacppVisionServer is None:
             if os.path.isfile(config.llamacppVisionModel_model_path) and os.path.isfile(config.llamacppVisionModel_clip_model_path):
                 config.llamacppVisionServer = None
                 print2("Running llama.cpp vision server ...")
-                cmd = f"""{sys.executable} -m llama_cpp.server --port {config.llamacppVisionModel_server_port} --model "{config.llamacppVisionModel_model_path}" --clip_model_path {config.llamacppVisionModel_clip_model_path} --verbose {config.llamacppVisionModel_verbose} --chat_format llava-1-5 --n_ctx {config.llamacppMainModel_n_ctx} --n_gpu_layers {config.llamacppMainModel_n_gpu_layers} --n_batch {config.llamacppMainModel_n_batch} {config.llamacppVisionModel_additional_options}"""
+                cmd = f"""{sys.executable} -m llama_cpp.server --port {config.llamacppVisionModel_server_port} --model "{config.llamacppVisionModel_model_path}" --clip_model_path {config.llamacppVisionModel_clip_model_path} --verbose {config.llamacppVisionModel_verbose} --chat_format llava-1-5 --n_ctx {config.llamacppVisionModel_n_ctx} --n_gpu_layers {config.llamacppVisionModel_n_gpu_layers} --n_batch {config.llamacppVisionModel_n_batch} {config.llamacppVisionModel_additional_server_options}"""
                 config.llamacppVisionServer = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE, shell=True, preexec_fn=os.setsid)
                 while not isServerAlive("127.0.0.1", config.llamacppVisionModel_server_port):
                     # wait til the server is up
                     ...
             else:
                 print1("Error! Clip model or vision model is missing!")
     except:
@@ -477,16 +477,16 @@
         return os.path.join(config.freeGeniusAIFolder, "files")
 
 # image
 
 def encode_image(image_path):
     with open(image_path, "rb") as image_file:
         base64_image = base64.b64encode(image_file.read()).decode('utf-8')
-    os.path.splitext(os.path.basename(image_path))[1]
-    return f"data:image/png;base64,{base64_image}"
+    ext = os.path.splitext(os.path.basename(image_path))[1][1:]
+    return f"data:image/{ext};base64,{base64_image}"
 
 def is_valid_image_url(url): 
     try: 
         response = requests.head(url, timeout=30)
         content_type = response.headers['content-type'] 
         if 'image' in content_type: 
             return True
```

### Comparing `freegenius-0.0.97/freegenius/utils/shortcuts.py` & `freegenius-0.0.98/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/single_prompt.py` & `freegenius-0.0.98/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.0.98/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/sttLanguages.py` & `freegenius-0.0.98/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.0.98/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.0.98/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/text_utils.py` & `freegenius-0.0.98/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/tool_plugins.py` & `freegenius-0.0.98/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/ttsLanguages.py` & `freegenius-0.0.98/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/tts_utils.py` & `freegenius-0.0.98/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius/utils/vlc_utils.py` & `freegenius-0.0.98/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius.egg-info/PKG-INFO` & `freegenius-0.0.98/freegenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.97
+Version: 0.0.98
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.0.97/freegenius.egg-info/SOURCES.txt` & `freegenius-0.0.98/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius.egg-info/entry_points.txt` & `freegenius-0.0.98/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/freegenius.egg-info/requires.txt` & `freegenius-0.0.98/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.97/setup.py` & `freegenius-0.0.98/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.0.97",
+    version="0.0.98",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

