# Comparing `tmp/freegenius-0.0.94.tar.gz` & `tmp/freegenius-0.0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.0.94.tar", last modified: Wed Apr 24 18:10:01 2024, max compression
+gzip compressed data, was "freegenius-0.0.95.tar", last modified: Thu Apr 25 10:18:44 2024, max compression
```

## Comparing `freegenius-0.0.94.tar` & `freegenius-0.0.95.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.434954 freegenius-0.0.94/
--rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-24 18:10:01.434708 freegenius-0.0.94/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.390663 freegenius-0.0.94/freegenius/
--rw-r--r--   0 admin      (501) staff       (20)    10056 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius/README.md
--rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.392218 freegenius-0.0.94/freegenius/audio/
--rw-r--r--   0 admin      (501) staff       (20)    15588 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/audio/notification1.mp3
--rw-r--r--   0 admin      (501) staff       (20)     2925 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/audio/notification1_mild.mp3
--rw-r--r--   0 admin      (501) staff       (20)    19428 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/audio/notification2.mp3
--rw-r--r--   0 admin      (501) staff       (20)     3693 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/audio/notification2_mild.mp3
--rw-r--r--   0 admin      (501) staff       (20)     6646 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/autoassist.py
--rw-r--r--   0 admin      (501) staff       (20)     9421 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/autobuilder.py
--rw-r--r--   0 admin      (501) staff       (20)    10727 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/autoretriever.py
--rw-r--r--   0 admin      (501) staff       (20)     6933 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)     7037 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/codey.py
--rw-r--r--   0 admin      (501) staff       (20)      833 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/commandprompt.py
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius/config.py
--rw-r--r--   0 admin      (501) staff       (20)    29583 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/eTextEdit.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.392372 freegenius-0.0.94/freegenius/files/
--rw-r--r--   0 admin      (501) staff       (20)       31 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/files/Readme.md
--rw-r--r--   0 admin      (501) staff       (20)    11372 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/geminipro.py
--rw-r--r--   0 admin      (501) staff       (20)     7838 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/geminiprovision.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.392814 freegenius-0.0.94/freegenius/gui/
--rw-r--r--   0 admin      (501) staff       (20)     9741 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/gui/chatgui.py
--rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/gui/worker.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.392978 freegenius-0.0.94/freegenius/history/
--rw-r--r--   0 admin      (501) staff       (20)       29 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/history/Readme.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.406928 freegenius-0.0.94/freegenius/icons/
--rw-r--r--   0 admin      (501) staff       (20)   158655 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/icons/FreeGenius.ico
--rw-r--r--   0 admin      (501) staff       (20)  2549036 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/icons/FreeGenius.png
--rw-r--r--   0 admin      (501) staff       (20)  3162696 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/icons/FreeGenius_original.png
--rw-r--r--   0 admin      (501) staff       (20)  3141194 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/icons/ai.png
--rw-r--r--   0 admin      (501) staff       (20)  2390858 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/icons/ai_original.png
--rw-r--r--   0 admin      (501) staff       (20)     8119 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/llamacpp.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.385452 freegenius-0.0.94/freegenius/macOS_service/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.384244 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.411587 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      644 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.413446 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5680 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.384407 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.414044 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.414216 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5679 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.384562 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.414651 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      635 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.414810 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4100 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5684 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.384734 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.415113 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      649 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.415273 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.384930 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.415600 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      643 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.415738 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.385121 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.416031 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      640 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.416207 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5656 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.385326 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.416545 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.416711 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.385492 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.417053 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.417253 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5692 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-r--r--   0 admin      (501) staff       (20)     7320 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/main.py
--rw-r--r--   0 admin      (501) staff       (20)    10959 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/ollamachat.py
--rw-r--r--   0 admin      (501) staff       (20)       10 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius/package_name.txt
--rw-r--r--   0 admin      (501) staff       (20)     7573 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/palm2.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.424617 freegenius-0.0.94/freegenius/plugins/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/000_check_ffmpeg.py
--rw-r--r--   0 admin      (501) staff       (20)     1616 2024-04-24 12:46:57.000000 freegenius-0.0.94/freegenius/plugins/000_check_pyaudio.py
--rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/000_check_vlc.py
--rw-r--r--   0 admin      (501) staff       (20)      115 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/Readme.md
--rw-r--r--   0 admin      (501) staff       (20)     6812 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/add calendar event.py
--rw-r--r--   0 admin      (501) staff       (20)     3358 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/aliases.py
--rw-r--r--   0 admin      (501) staff       (20)     7429 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/analyze audio.py
--rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/analyze files.py
--rw-r--r--   0 admin      (501) staff       (20)     4667 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/analyze images.py
--rw-r--r--   0 admin      (501) staff       (20)     2316 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/analyze web content.py
--rw-r--r--   0 admin      (501) staff       (20)     2559 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/auto correct python code.py
--rw-r--r--   0 admin      (501) staff       (20)     1860 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/awesome prompts.py
--rw-r--r--   0 admin      (501) staff       (20)     5876 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/character analysis.py
--rw-r--r--   0 admin      (501) staff       (20)      654 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/chat.py
--rw-r--r--   0 admin      (501) staff       (20)      762 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/contexts.py
--rw-r--r--   0 admin      (501) staff       (20)     7220 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/counselling.py
--rw-r--r--   0 admin      (501) staff       (20)     1688 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/create ai assistants.py
--rw-r--r--   0 admin      (501) staff       (20)     5152 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/create images.py
--rw-r--r--   0 admin      (501) staff       (20)     1262 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/create maps.py
--rw-r--r--   0 admin      (501) staff       (20)     1520 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/create qrcode.py
--rw-r--r--   0 admin      (501) staff       (20)     1522 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/create statistical graphics.py
--rw-r--r--   0 admin      (501) staff       (20)     1211 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/dates and times.py
--rw-r--r--   0 admin      (501) staff       (20)     3950 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/download youtube or web content.py
--rw-r--r--   0 admin      (501) staff       (20)     1862 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/edit text.py
--rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/execute computing tasks.py
--rw-r--r--   0 admin      (501) staff       (20)     4213 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/execute termux command.py
--rw-r--r--   0 admin      (501) staff       (20)     6940 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/global finance.py
--rw-r--r--   0 admin      (501) staff       (20)      975 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/improve British English.py
--rw-r--r--   0 admin      (501) staff       (20)     2315 2024-04-24 18:08:35.000000 freegenius-0.0.94/freegenius/plugins/input suggestions.py
--rw-r--r--   0 admin      (501) staff       (20)     1077 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/install python package.py
--rw-r--r--   0 admin      (501) staff       (20)     1670 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/integrate google searches.py
--rw-r--r--   0 admin      (501) staff       (20)     4606 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/memory.py
--rw-r--r--   0 admin      (501) staff       (20)     8638 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/modify images.py
--rw-r--r--   0 admin      (501) staff       (20)      944 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/open web browser.py
--rw-r--r--   0 admin      (501) staff       (20)     1296 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/pronounce words.py
--rw-r--r--   0 admin      (501) staff       (20)     2409 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/remove image background.py
--rw-r--r--   0 admin      (501) staff       (20)     5898 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/search chat records.py
--rw-r--r--   0 admin      (501) staff       (20)     1156 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/search financial data.py
--rw-r--r--   0 admin      (501) staff       (20)     1966 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/search latest news.py
--rw-r--r--   0 admin      (501) staff       (20)     3479 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/search sqlite.py
--rw-r--r--   0 admin      (501) staff       (20)     1539 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/search weather info.py
--rw-r--r--   0 admin      (501) staff       (20)     3987 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/send email.py
--rw-r--r--   0 admin      (501) staff       (20)      898 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/send tweet.py
--rw-r--r--   0 admin      (501) staff       (20)     1280 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/send whatsapp messages.py
--rw-r--r--   0 admin      (501) staff       (20)      528 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-r--r--   0 admin      (501) staff       (20)      242 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/qt.py
--rw-r--r--   0 admin      (501) staff       (20)     9711 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/rag.py
--rw-r--r--   0 admin      (501) staff       (20)      796 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/requirements.txt
--rw-r--r--   0 admin      (501) staff       (20)     1293 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/servers.py
--rw-r--r--   0 admin      (501) staff       (20)     7691 2024-04-24 16:18:44.000000 freegenius-0.0.94/freegenius/systemtray.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.424780 freegenius-0.0.94/freegenius/temp/
--rw-r--r--   0 admin      (501) staff       (20)       36 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/temp/Readme.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.434359 freegenius-0.0.94/freegenius/utils/
--rw-r--r--   0 admin      (501) staff       (20)   108133 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/assistant.py
--rw-r--r--   0 admin      (501) staff       (20)    29582 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/call_chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)    17109 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/call_gemini.py
--rw-r--r--   0 admin      (501) staff       (20)    22247 2024-04-24 12:03:40.000000 freegenius-0.0.94/freegenius/utils/call_llamacpp.py
--rw-r--r--   0 admin      (501) staff       (20)     7664 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/call_llm.py
--rw-r--r--   0 admin      (501) staff       (20)    18715 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/call_ollama.py
--rw-r--r--   0 admin      (501) staff       (20)    16451 2024-04-24 12:02:43.000000 freegenius-0.0.94/freegenius/utils/config_essential.py
--rw-r--r--   0 admin      (501) staff       (20)     2616 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/config_tools.py
--rw-r--r--   0 admin      (501) staff       (20)     1368 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/download.py
--rw-r--r--   0 admin      (501) staff       (20)    14296 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/get_path_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)     4888 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/ollama_models.py
--rw-r--r--   0 admin      (501) staff       (20)     3872 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/promptValidator.py
--rw-r--r--   0 admin      (501) staff       (20)     6973 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-r--r--   0 admin      (501) staff       (20)     7880 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/prompt_shared_key_bindings.py
--rw-r--r--   0 admin      (501) staff       (20)    21592 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/prompts.py
--rw-r--r--   0 admin      (501) staff       (20)     1681 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/python_utils.py
--rw-r--r--   0 admin      (501) staff       (20)    47445 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/shared_utils.py
--rw-r--r--   0 admin      (501) staff       (20)    21476 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/shortcuts.py
--rw-r--r--   0 admin      (501) staff       (20)     8558 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/single_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)     7936 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/streaming_word_wrapper.py
--rw-r--r--   0 admin      (501) staff       (20)     7580 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/sttLanguages.py
--rw-r--r--   0 admin      (501) staff       (20)     4781 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/terminal_mode_dialogs.py
--rwxr-xr-x   0 admin      (501) staff       (20)     9891 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/terminal_system_command_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)    23917 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/text_utils.py
--rw-r--r--   0 admin      (501) staff       (20)     4352 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/tool_plugins.py
--rw-r--r--   0 admin      (501) staff       (20)     7640 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/ttsLanguages.py
--rw-r--r--   0 admin      (501) staff       (20)     8563 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/tts_utils.py
--rw-r--r--   0 admin      (501) staff       (20)     4651 2024-04-24 10:05:32.000000 freegenius-0.0.94/freegenius/utils/vlc_utils.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-24 18:10:01.391346 freegenius-0.0.94/freegenius.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     5856 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)     1226 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)      797 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       11 2024-04-24 18:10:01.000000 freegenius-0.0.94/freegenius.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-24 18:10:01.435003 freegenius-0.0.94/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)    10383 2024-04-24 18:09:57.000000 freegenius-0.0.94/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.544555 freegenius-0.0.95/
+-rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-25 10:18:44.544295 freegenius-0.0.95/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.505484 freegenius-0.0.95/freegenius/
+-rw-r--r--   0 admin      (501) staff       (20)    10056 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius/README.md
+-rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.507321 freegenius-0.0.95/freegenius/audio/
+-rw-r--r--   0 admin      (501) staff       (20)    15588 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/audio/notification1.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     2925 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/audio/notification1_mild.mp3
+-rw-r--r--   0 admin      (501) staff       (20)    19428 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/audio/notification2.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     3693 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/audio/notification2_mild.mp3
+-rw-r--r--   0 admin      (501) staff       (20)     6646 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/autoassist.py
+-rw-r--r--   0 admin      (501) staff       (20)     9421 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/autobuilder.py
+-rw-r--r--   0 admin      (501) staff       (20)    10727 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/autoretriever.py
+-rw-r--r--   0 admin      (501) staff       (20)     6933 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)     7037 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/codey.py
+-rw-r--r--   0 admin      (501) staff       (20)      833 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/commandprompt.py
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius/config.py
+-rw-r--r--   0 admin      (501) staff       (20)    29583 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/eTextEdit.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.507459 freegenius-0.0.95/freegenius/files/
+-rw-r--r--   0 admin      (501) staff       (20)       31 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/files/Readme.md
+-rw-r--r--   0 admin      (501) staff       (20)    11372 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/geminipro.py
+-rw-r--r--   0 admin      (501) staff       (20)     7838 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/geminiprovision.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.507857 freegenius-0.0.95/freegenius/gui/
+-rw-r--r--   0 admin      (501) staff       (20)     9741 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/gui/chatgui.py
+-rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/gui/worker.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.508002 freegenius-0.0.95/freegenius/history/
+-rw-r--r--   0 admin      (501) staff       (20)       29 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/history/Readme.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.521084 freegenius-0.0.95/freegenius/icons/
+-rw-r--r--   0 admin      (501) staff       (20)   158655 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/FreeGenius.ico
+-rw-r--r--   0 admin      (501) staff       (20)  2549036 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/FreeGenius.png
+-rw-r--r--   0 admin      (501) staff       (20)  3162696 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/FreeGenius_original.png
+-rw-r--r--   0 admin      (501) staff       (20)  3141194 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/ai.png
+-rw-r--r--   0 admin      (501) staff       (20)  2390858 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/ai_original.png
+-rw-r--r--   0 admin      (501) staff       (20)     8119 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/llamacpp.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.499498 freegenius-0.0.95/freegenius/macOS_service/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498216 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.525368 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      644 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.525580 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5680 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498384 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.526064 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.526202 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5679 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498612 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.526590 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      635 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.526777 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4100 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5684 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498804 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.527096 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      649 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.527282 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498965 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.527570 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      643 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.527707 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.499121 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528013 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      640 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528148 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5656 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.499332 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528409 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528546 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.499565 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528824 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528979 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-r--r--   0 admin      (501) staff       (20)     5692 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-r--r--   0 admin      (501) staff       (20)     7320 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/main.py
+-rw-r--r--   0 admin      (501) staff       (20)    10959 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/ollamachat.py
+-rw-r--r--   0 admin      (501) staff       (20)       10 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius/package_name.txt
+-rw-r--r--   0 admin      (501) staff       (20)     7573 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/palm2.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.536131 freegenius-0.0.95/freegenius/plugins/
+-rw-r--r--   0 admin      (501) staff       (20)     1326 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/000_check_ffmpeg.py
+-rw-r--r--   0 admin      (501) staff       (20)     1616 2024-04-24 12:46:57.000000 freegenius-0.0.95/freegenius/plugins/000_check_pyaudio.py
+-rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/000_check_vlc.py
+-rw-r--r--   0 admin      (501) staff       (20)      115 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/Readme.md
+-rw-r--r--   0 admin      (501) staff       (20)     6812 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/add calendar event.py
+-rw-r--r--   0 admin      (501) staff       (20)     3358 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/aliases.py
+-rw-r--r--   0 admin      (501) staff       (20)     7429 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/analyze audio.py
+-rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/analyze files.py
+-rw-r--r--   0 admin      (501) staff       (20)     4667 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/analyze images.py
+-rw-r--r--   0 admin      (501) staff       (20)     2316 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/analyze web content.py
+-rw-r--r--   0 admin      (501) staff       (20)     2559 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/auto correct python code.py
+-rw-r--r--   0 admin      (501) staff       (20)     1860 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/awesome prompts.py
+-rw-r--r--   0 admin      (501) staff       (20)     5876 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/character analysis.py
+-rw-r--r--   0 admin      (501) staff       (20)      654 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/chat.py
+-rw-r--r--   0 admin      (501) staff       (20)      762 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/contexts.py
+-rw-r--r--   0 admin      (501) staff       (20)     7220 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/counselling.py
+-rw-r--r--   0 admin      (501) staff       (20)     1688 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create ai assistants.py
+-rw-r--r--   0 admin      (501) staff       (20)     5152 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create images.py
+-rw-r--r--   0 admin      (501) staff       (20)     1262 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create maps.py
+-rw-r--r--   0 admin      (501) staff       (20)     1520 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create qrcode.py
+-rw-r--r--   0 admin      (501) staff       (20)     1522 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create statistical graphics.py
+-rw-r--r--   0 admin      (501) staff       (20)     1211 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/dates and times.py
+-rw-r--r--   0 admin      (501) staff       (20)     3950 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/download youtube or web content.py
+-rw-r--r--   0 admin      (501) staff       (20)     1862 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/edit text.py
+-rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/execute computing tasks.py
+-rw-r--r--   0 admin      (501) staff       (20)     4213 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/execute termux command.py
+-rw-r--r--   0 admin      (501) staff       (20)     6940 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/global finance.py
+-rw-r--r--   0 admin      (501) staff       (20)      975 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/improve British English.py
+-rw-r--r--   0 admin      (501) staff       (20)     2315 2024-04-24 18:08:35.000000 freegenius-0.0.95/freegenius/plugins/input suggestions.py
+-rw-r--r--   0 admin      (501) staff       (20)     1077 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/install python package.py
+-rw-r--r--   0 admin      (501) staff       (20)     1670 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/integrate google searches.py
+-rw-r--r--   0 admin      (501) staff       (20)     4606 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/memory.py
+-rw-r--r--   0 admin      (501) staff       (20)     8638 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/modify images.py
+-rw-r--r--   0 admin      (501) staff       (20)      944 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/open web browser.py
+-rw-r--r--   0 admin      (501) staff       (20)     1296 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/pronounce words.py
+-rw-r--r--   0 admin      (501) staff       (20)     2409 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/remove image background.py
+-rw-r--r--   0 admin      (501) staff       (20)     5898 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search chat records.py
+-rw-r--r--   0 admin      (501) staff       (20)     1156 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search financial data.py
+-rw-r--r--   0 admin      (501) staff       (20)     1966 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search latest news.py
+-rw-r--r--   0 admin      (501) staff       (20)     3479 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search sqlite.py
+-rw-r--r--   0 admin      (501) staff       (20)     1539 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search weather info.py
+-rw-r--r--   0 admin      (501) staff       (20)     3987 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/send email.py
+-rw-r--r--   0 admin      (501) staff       (20)      898 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/send tweet.py
+-rw-r--r--   0 admin      (501) staff       (20)     1280 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/send whatsapp messages.py
+-rw-r--r--   0 admin      (501) staff       (20)      528 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-r--r--   0 admin      (501) staff       (20)      242 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/qt.py
+-rw-r--r--   0 admin      (501) staff       (20)     9711 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/rag.py
+-rw-r--r--   0 admin      (501) staff       (20)      796 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/requirements.txt
+-rw-r--r--   0 admin      (501) staff       (20)     1293 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/servers.py
+-rw-r--r--   0 admin      (501) staff       (20)     7691 2024-04-24 16:18:44.000000 freegenius-0.0.95/freegenius/systemtray.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.536259 freegenius-0.0.95/freegenius/temp/
+-rw-r--r--   0 admin      (501) staff       (20)       36 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/temp/Readme.md
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.543837 freegenius-0.0.95/freegenius/utils/
+-rw-r--r--   0 admin      (501) staff       (20)   108133 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/assistant.py
+-rw-r--r--   0 admin      (501) staff       (20)    29582 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/call_chatgpt.py
+-rw-r--r--   0 admin      (501) staff       (20)    17109 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/call_gemini.py
+-rw-r--r--   0 admin      (501) staff       (20)    22247 2024-04-25 09:02:38.000000 freegenius-0.0.95/freegenius/utils/call_llamacpp.py
+-rw-r--r--   0 admin      (501) staff       (20)     7664 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/call_llm.py
+-rw-r--r--   0 admin      (501) staff       (20)    18715 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/call_ollama.py
+-rw-r--r--   0 admin      (501) staff       (20)    16449 2024-04-25 09:58:59.000000 freegenius-0.0.95/freegenius/utils/config_essential.py
+-rw-r--r--   0 admin      (501) staff       (20)     2616 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/config_tools.py
+-rw-r--r--   0 admin      (501) staff       (20)     1368 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/download.py
+-rw-r--r--   0 admin      (501) staff       (20)    14296 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/get_path_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)     4888 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/ollama_models.py
+-rw-r--r--   0 admin      (501) staff       (20)     3872 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/promptValidator.py
+-rw-r--r--   0 admin      (501) staff       (20)     6973 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-r--r--   0 admin      (501) staff       (20)     7880 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/prompt_shared_key_bindings.py
+-rw-r--r--   0 admin      (501) staff       (20)    21592 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/prompts.py
+-rw-r--r--   0 admin      (501) staff       (20)     1681 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/python_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)    48047 2024-04-25 10:17:59.000000 freegenius-0.0.95/freegenius/utils/shared_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)    21476 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/shortcuts.py
+-rw-r--r--   0 admin      (501) staff       (20)     8558 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/single_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)     7936 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/streaming_word_wrapper.py
+-rw-r--r--   0 admin      (501) staff       (20)     7580 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/sttLanguages.py
+-rw-r--r--   0 admin      (501) staff       (20)     4781 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/terminal_mode_dialogs.py
+-rwxr-xr-x   0 admin      (501) staff       (20)     9891 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/terminal_system_command_prompt.py
+-rw-r--r--   0 admin      (501) staff       (20)    23917 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/text_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     4352 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/tool_plugins.py
+-rw-r--r--   0 admin      (501) staff       (20)     7640 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/ttsLanguages.py
+-rw-r--r--   0 admin      (501) staff       (20)     8563 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/tts_utils.py
+-rw-r--r--   0 admin      (501) staff       (20)     4651 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/vlc_utils.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.506422 freegenius-0.0.95/freegenius.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     5856 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)     1226 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/entry_points.txt
+-rw-r--r--   0 admin      (501) staff       (20)      797 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)       11 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-25 10:18:44.544600 freegenius-0.0.95/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)    10383 2024-04-25 10:18:09.000000 freegenius-0.0.95/setup.py
```

### Comparing `freegenius-0.0.94/PKG-INFO` & `freegenius-0.0.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.94
+Version: 0.0.95
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.0.94/freegenius/README.md` & `freegenius-0.0.95/freegenius/README.md`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/__init__.py` & `freegenius-0.0.95/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/audio/notification1.mp3` & `freegenius-0.0.95/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/audio/notification1_mild.mp3` & `freegenius-0.0.95/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/audio/notification2.mp3` & `freegenius-0.0.95/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/audio/notification2_mild.mp3` & `freegenius-0.0.95/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/autoassist.py` & `freegenius-0.0.95/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/autobuilder.py` & `freegenius-0.0.95/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/autoretriever.py` & `freegenius-0.0.95/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/chatgpt.py` & `freegenius-0.0.95/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/codey.py` & `freegenius-0.0.95/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/commandprompt.py` & `freegenius-0.0.95/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/eTextEdit.py` & `freegenius-0.0.95/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/geminipro.py` & `freegenius-0.0.95/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/geminiprovision.py` & `freegenius-0.0.95/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/gui/chatgui.py` & `freegenius-0.0.95/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/gui/worker.py` & `freegenius-0.0.95/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/icons/FreeGenius.ico` & `freegenius-0.0.95/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/icons/FreeGenius.png` & `freegenius-0.0.95/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/icons/FreeGenius_original.png` & `freegenius-0.0.95/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/icons/ai.png` & `freegenius-0.0.95/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/icons/ai_original.png` & `freegenius-0.0.95/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/llamacpp.py` & `freegenius-0.0.95/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/main.py` & `freegenius-0.0.95/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/ollamachat.py` & `freegenius-0.0.95/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/palm2.py` & `freegenius-0.0.95/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.0.95/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.0.95/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/000_check_vlc.py` & `freegenius-0.0.95/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/add calendar event.py` & `freegenius-0.0.95/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/aliases.py` & `freegenius-0.0.95/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/analyze audio.py` & `freegenius-0.0.95/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/analyze files.py` & `freegenius-0.0.95/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/analyze images.py` & `freegenius-0.0.95/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/analyze web content.py` & `freegenius-0.0.95/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/auto correct python code.py` & `freegenius-0.0.95/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/awesome prompts.py` & `freegenius-0.0.95/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/character analysis.py` & `freegenius-0.0.95/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/chat.py` & `freegenius-0.0.95/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/contexts.py` & `freegenius-0.0.95/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/counselling.py` & `freegenius-0.0.95/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/create ai assistants.py` & `freegenius-0.0.95/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/create images.py` & `freegenius-0.0.95/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/create maps.py` & `freegenius-0.0.95/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/create qrcode.py` & `freegenius-0.0.95/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/create statistical graphics.py` & `freegenius-0.0.95/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/dates and times.py` & `freegenius-0.0.95/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/download youtube or web content.py` & `freegenius-0.0.95/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/edit text.py` & `freegenius-0.0.95/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/execute computing tasks.py` & `freegenius-0.0.95/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/execute termux command.py` & `freegenius-0.0.95/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/global finance.py` & `freegenius-0.0.95/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/improve British English.py` & `freegenius-0.0.95/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/input suggestions.py` & `freegenius-0.0.95/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/install python package.py` & `freegenius-0.0.95/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/integrate google searches.py` & `freegenius-0.0.95/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/memory.py` & `freegenius-0.0.95/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/modify images.py` & `freegenius-0.0.95/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/open web browser.py` & `freegenius-0.0.95/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/pronounce words.py` & `freegenius-0.0.95/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/remove image background.py` & `freegenius-0.0.95/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/search chat records.py` & `freegenius-0.0.95/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/search financial data.py` & `freegenius-0.0.95/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/search latest news.py` & `freegenius-0.0.95/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/search sqlite.py` & `freegenius-0.0.95/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/search weather info.py` & `freegenius-0.0.95/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/send email.py` & `freegenius-0.0.95/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/send tweet.py` & `freegenius-0.0.95/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.0.95/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.0.95/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/rag.py` & `freegenius-0.0.95/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/requirements.txt` & `freegenius-0.0.95/freegenius/requirements.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/servers.py` & `freegenius-0.0.95/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/systemtray.py` & `freegenius-0.0.95/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/assistant.py` & `freegenius-0.0.95/freegenius/utils/assistant.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/call_chatgpt.py` & `freegenius-0.0.95/freegenius/utils/call_chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/call_gemini.py` & `freegenius-0.0.95/freegenius/utils/call_gemini.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/call_llamacpp.py` & `freegenius-0.0.95/freegenius/utils/call_llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/call_llm.py` & `freegenius-0.0.95/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/call_ollama.py` & `freegenius-0.0.95/freegenius/utils/call_ollama.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/config_essential.py` & `freegenius-0.0.95/freegenius/utils/config_essential.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,23 +67,23 @@
     ('llamacppChatModel_additional_chat_options', {}),
     ('llamacppMainModel_ollama_tag', ''), # selected ollama hosted model to run with llamacpp
     ('llamacppMainModel_model_path', ''), # specify file path of llama.cpp model for general purpose
     ('llamacppMainModel_repo_id', 'TheBloke/CodeLlama-7B-Instruct-GGUF'), # llama.cpp model used for both task execution and conversation, e.g. 'TheBloke/phi-2-GGUF', 'NousResearch/Hermes-2-Pro-Mistral-7B-GGUF', 'NousResearch/Nous-Hermes-2-Mixtral-8x7B-DPO-GGUF'
     ('llamacppMainModel_filename', 'codellama-7b-instruct.Q4_K_M.gguf'), # llama.cpp model used for both task execution and conversation, e.g. 'Hermes-2-Pro-Mistral-7B.Q4_K_M.gguf', 'Nous-Hermes-2-Mixtral-8x7B-DPO.Q4_K_M.gguf'
     ('llamacppMainModel_n_ctx', 0), # llama.cpp main model context window
     ('llamacppMainModel_max_tokens', 10000), # llama.cpp main model maximum tokens
-    ('llamacppMainModel_n_gpu_layers', -1), # change to -1 to use GPU acceleration
+    ('llamacppMainModel_n_gpu_layers', 0), # change to -1 to use GPU acceleration
     ('llamacppMainModel_n_batch', 512), # The batch size to use per eval
     ('llamacppChatModel_ollama_tag', ''), # selected ollama hosted model to run with llamacpp
     ('llamacppChatModel_model_path', ''), # specify file path of llama.cpp model for chat
     ('llamacppChatModel_repo_id', 'TheBloke/Mistral-7B-Instruct-v0.2-GGUF'), # llama.cpp model used for chat, e.g. 'TheBloke/CodeLlama-7B-Python-GGUF'
     ('llamacppChatModel_filename', 'mistral-7b-instruct-v0.2.Q4_K_M.gguf'), # llama.cpp model used for chat, e.g. 'codellama-7b-python.Q4_K_M.gguf'
     ('llamacppChatModel_n_ctx', 0), # llama.cpp chat model context window
     ('llamacppChatModel_max_tokens', 10000), # llama.cpp chat model maximum tokens
-    ('llamacppChatModel_n_gpu_layers', -1), # change to -1 to use GPU acceleration
+    ('llamacppChatModel_n_gpu_layers', 0), # change to -1 to use GPU acceleration
     ('llamacppChatModel_n_batch', 512), # The batch size to use per eval
     ('geminipro_max_output_tokens', 8192), # check supported value at https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models
     # common configs as in LetMeDoIt AI
     ('translateToLanguage', ''),
     ('dynamicTokenCount', False),
     ('use_oai_assistant', False), # support OpenAI Assistants API in AutoGen Agent Builder
     ('max_agents', 5), # maximum number of agents build manager can create.
```

### Comparing `freegenius-0.0.94/freegenius/utils/config_tools.py` & `freegenius-0.0.95/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/download.py` & `freegenius-0.0.95/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/get_path_prompt.py` & `freegenius-0.0.95/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/ollama_models.py` & `freegenius-0.0.95/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/promptValidator.py` & `freegenius-0.0.95/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.0.95/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.0.95/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/prompts.py` & `freegenius-0.0.95/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/python_utils.py` & `freegenius-0.0.95/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/shared_utils.py` & `freegenius-0.0.95/freegenius/utils/shared_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from pathlib import Path
 from PIL import Image
 from openai import OpenAI
 from huggingface_hub import hf_hub_download
 from bs4 import BeautifulSoup
 from urllib.parse import quote
 from guidance import select, gen
+from typing import Union
 
 # non-Android only
 if not config.isTermux:
     from autogen.retrieve_utils import TEXT_FORMATS
 
 # a dummy import line to resolve ALSA error display on Linux
 import sounddevice
@@ -28,53 +29,91 @@
 
 # guidance
 
 def screening(lm, user_input) -> bool:
     tool = False
 
     print2("```screening")
-    thought = "Thought: First, I must carefully distinguish whether the given request is formulated like a greeting, a question, a command, a statement, an issue, a description."
+    thought = "Question: Is the given request formulated like a greeting, a question, a command, a statement, an issue, a description?"
     print3(thought)
     lm += f"""<|im_start|>user
-Assess the following request and comment whether an additional tool is needed to address it:
-<request>{user_input}</request><|im_end|>
+Please answer my questions with regards to the following request:
+<request>{user_input}</request>
+<|im_end|>
 <|im_start|>assistant
+Certainly! Please provide me with the questions.
+<|im_end|>
+<|im_start|>user
 {thought}
-Observation: The given request is formulated like {select(["a question", "a command", "a statement", "an issue", "a description"], name="question")}.
+Answer: The given request is formulated like {select(["a question", "a command", "a statement", "an issue", "a description"], name="question")}.
+<|im_end|>
 """
     question = lm.get("question")
-    print3(f"""Observation: The given request is formulated like {question}.""")
+    print3(f"""Answer: The given request is formulated like {question}.""")
     if question in ("a greeting", "a question", "an issue", "a description"):
-        #thought = "Thought: Next, I need to ascertain the nature of the requested information, determining whether it is static, time-sensitive, changing over time, unchanging over time, published, well-established, common, documented, foundational, historical, technical, prone to periodic updates, subject to changes, evolving, ongoing, location-specific, or unknown." # more categories: "context-specific", "user-dependent", "subject to fluctuation"
-        thought = "Thought: Next, I must carefully distinguish whether the requested information is about greeting, common knowledge, math, translation, published content, acquired knowledge, historical records, programming knowledge, religious knowledge, insights obtainable from literature, textbook material, evolving data, recent updates, latest information, current time, current weather, up-to-date news, information specific to your device, or information unknown to me."
+        thought = "Question: What is the request about?"
         print3(thought)
-        lm += f"""{thought}
-Observation: The requested information is about {select(["greeting", "common knowledge", "math", "translation", "published content", "trained knowledge", "historical records", "programming knowledge", "religious knowledge", "insights obtainable from literature", "textbook content", "evolving data", "recent updates", "latest information", "current time", "current weather", "up-to-date news", "information specific to your device", "information unknown to me"], name="information")}.
+        lm += f"""<|im_start|>assistant
+{thought}
+<|im_end|>
+<|im_start|>user
+Answer: The request is about {select(["greeting", "common knowledge", "math", "published content", "trained knowledge", "historical records", "programming knowledge", "religious knowledge", "insights obtainable from literature", "textbook content", "evolving data", "recent updates", "latest information", "current time", "current weather", "up-to-date news", "information specific to your device", "information unknown to me"], name="information")}.
+<|im_end|>
 """
-        #Observation: The nature of the requested information is {select(["static", "time-sensitive", "changing over time", "unchanging over time", "published", "well-established", "common", "documented", "foundational", "historical", "technical", "prone to periodic updates", "subject to changes", "evolving", "ongoing", "location-specific", "unknown"], name="information")}.
         information = lm.get("information")
-        print3(f"""Observation: The requested information is about {information}.""")
+        print3(f"""Answer: The request is about {information}.""")
         if information in ("evolving data", "recent updates", "latest information", "current time", "current weather", "up-to-date news", "information specific to your device", "information unknown to me"):
             tool = True
     else:
-        thought = "Thought: Next, I must carefully distinguish whether the given request asks for generating a text-response or carrying out a task on your device."
+        thought = "Question: Does the given request ask for generating a text-response or carrying out a task on your device?"
         print3(thought)
-        lm += f"""{thought}
-Observation: The given request asks for {select(["greeting", "calculation", "translation", "writing a text-response", "carrying out a task on your device"], name="action")}.
+        lm += f"""<|im_start|>assistant
+{thought}
+<|im_end|>
+<|im_start|>user
+Answer: The given request asks for {select(["greeting", "calculation", "translation", "writing a text-response", "carrying out a task on your device"], name="action")}.
+<|im_end|>
 """
         action = lm.get("action")
-        print3(f"""Observation: The given request asks for {action}.""")
+        print3(f"""Answer: The given request asks for {action}.""")
         if action in ("carrying out a task on your device",):
             tool = True
 
     print3(f"""Comment: Tool may {"" if tool else "not "}be required.""")
     print2("```")
 
     return tool
 
+def outputStructuredData(lm, schema: dict, json_output: bool=False, messages: list = [], use_system_message: bool=True, request: str="", temperature: Optional[float]=None, max_tokens: Optional[int]=None, **kwargs) -> Union[dict, str]:
+    properties = toParameterSchema(schema)["properties"]
+    lm += toChatml(messages, use_system_message=use_system_message).rstrip()
+    lm += f"""<|im_start|>assistant.
+I am answering your questions based on the content in our conversation given above, particularly related to the following request:
+{request}
+<|im_end|>
+"""
+    for key, value in properties.items():
+        description = value["description"].replace("\n", " ")
+        if "enum" in value:
+            options = value["enum"]
+            options_str = "', '".join(value["enum"])
+            description += f" Its value must be one of these options: '{options_str}'"
+        lm += f'''<|im_start|>user
+Question: {description}
+<|im_end|>
+<|im_start|>assistant
+Answer: {select(options, name=key) if "enum" in value else gen(name=key, stop="<")}
+<|im_end|>
+'''
+
+    response = {}
+    for i in properties:
+        response[i] = lm.get(i, "").rstrip()
+    return json.dumps(response) if json_output else response
+
 def select_tool(lm, user_input):
     tool_names = list(config.toolFunctionSchemas.keys())
     tools = {i:config.toolFunctionSchemas[i]["description"] for i in config.toolFunctionSchemas}
 
     lm += f"""<|im_start|>user
 Select an action to resolve the request as best you can. You have access only to the following tools:
 
@@ -454,14 +493,28 @@
     """
     extract parameter schema from full schema
     """
     if "parameters" in schema:
         return schema["parameters"]
     return schema
 
+def toChatml(messages: dict=[], use_system_message=True) -> str:
+    messages_str = ""
+    roles = {
+        "user": "<|im_start|>user\n{content}\n<|im_end|>\n",
+        "assistant": "<|im_start|>assistant\n{content}\n<|im_end|>\n",
+    }
+    if use_system_message:
+        roles["system"] = "<|im_start|>system\n{content}\n<|im_end|>\n"
+    for message in messages:
+        role, content = message.get("role", ""), message.get("content", "")
+        if role and role in roles and content:
+            messages_str += roles[role].format(content=content)
+    return messages_str.rstrip()
+
 def toGeminiMessages(messages: dict=[]) -> Optional[list]:
     systemMessage = ""
     lastUserMessage = ""
     if messages:
         history = []
         for i in messages:
             role = i.get("role", "")
```

### Comparing `freegenius-0.0.94/freegenius/utils/shortcuts.py` & `freegenius-0.0.95/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/single_prompt.py` & `freegenius-0.0.95/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.0.95/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/sttLanguages.py` & `freegenius-0.0.95/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.0.95/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.0.95/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/text_utils.py` & `freegenius-0.0.95/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/tool_plugins.py` & `freegenius-0.0.95/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/ttsLanguages.py` & `freegenius-0.0.95/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/tts_utils.py` & `freegenius-0.0.95/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius/utils/vlc_utils.py` & `freegenius-0.0.95/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius.egg-info/PKG-INFO` & `freegenius-0.0.95/freegenius.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.94
+Version: 0.0.95
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
```

### Comparing `freegenius-0.0.94/freegenius.egg-info/SOURCES.txt` & `freegenius-0.0.95/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius.egg-info/entry_points.txt` & `freegenius-0.0.95/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/freegenius.egg-info/requires.txt` & `freegenius-0.0.95/freegenius.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.94/setup.py` & `freegenius-0.0.95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.0.94",
+    version="0.0.95",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

