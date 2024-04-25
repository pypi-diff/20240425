# Comparing `tmp/freegenius-0.0.95.tar.gz` & `tmp/freegenius-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freegenius-0.0.95.tar", last modified: Thu Apr 25 10:18:44 2024, max compression
+gzip compressed data, was "freegenius-0.0.97.tar", last modified: Thu Apr 25 15:50:35 2024, max compression
```

## Comparing `freegenius-0.0.95.tar` & `freegenius-0.0.97.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.544555 freegenius-0.0.95/
--rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-25 10:18:44.544295 freegenius-0.0.95/PKG-INFO
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.505484 freegenius-0.0.95/freegenius/
--rw-r--r--   0 admin      (501) staff       (20)    10056 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius/README.md
--rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.507321 freegenius-0.0.95/freegenius/audio/
--rw-r--r--   0 admin      (501) staff       (20)    15588 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/audio/notification1.mp3
--rw-r--r--   0 admin      (501) staff       (20)     2925 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/audio/notification1_mild.mp3
--rw-r--r--   0 admin      (501) staff       (20)    19428 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/audio/notification2.mp3
--rw-r--r--   0 admin      (501) staff       (20)     3693 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/audio/notification2_mild.mp3
--rw-r--r--   0 admin      (501) staff       (20)     6646 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/autoassist.py
--rw-r--r--   0 admin      (501) staff       (20)     9421 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/autobuilder.py
--rw-r--r--   0 admin      (501) staff       (20)    10727 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/autoretriever.py
--rw-r--r--   0 admin      (501) staff       (20)     6933 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)     7037 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/codey.py
--rw-r--r--   0 admin      (501) staff       (20)      833 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/commandprompt.py
--rw-r--r--   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius/config.py
--rw-r--r--   0 admin      (501) staff       (20)    29583 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/eTextEdit.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.507459 freegenius-0.0.95/freegenius/files/
--rw-r--r--   0 admin      (501) staff       (20)       31 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/files/Readme.md
--rw-r--r--   0 admin      (501) staff       (20)    11372 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/geminipro.py
--rw-r--r--   0 admin      (501) staff       (20)     7838 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/geminiprovision.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.507857 freegenius-0.0.95/freegenius/gui/
--rw-r--r--   0 admin      (501) staff       (20)     9741 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/gui/chatgui.py
--rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/gui/worker.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.508002 freegenius-0.0.95/freegenius/history/
--rw-r--r--   0 admin      (501) staff       (20)       29 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/history/Readme.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.521084 freegenius-0.0.95/freegenius/icons/
--rw-r--r--   0 admin      (501) staff       (20)   158655 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/FreeGenius.ico
--rw-r--r--   0 admin      (501) staff       (20)  2549036 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/FreeGenius.png
--rw-r--r--   0 admin      (501) staff       (20)  3162696 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/FreeGenius_original.png
--rw-r--r--   0 admin      (501) staff       (20)  3141194 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/ai.png
--rw-r--r--   0 admin      (501) staff       (20)  2390858 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/icons/ai_original.png
--rw-r--r--   0 admin      (501) staff       (20)     8119 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/llamacpp.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.499498 freegenius-0.0.95/freegenius/macOS_service/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498216 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.525368 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      644 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.525580 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5680 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498384 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.526064 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.526202 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5679 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498612 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.526590 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      635 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.526777 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4100 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5684 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498804 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.527096 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      649 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.527282 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.498965 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.527570 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      643 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.527707 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.499121 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528013 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      640 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528148 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5656 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.499332 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528409 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528546 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5681 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.499565 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528824 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
--rw-r--r--   0 admin      (501) staff       (20)      647 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.528979 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
--rw-r--r--   0 admin      (501) staff       (20)     4273 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
--rw-r--r--   0 admin      (501) staff       (20)     5692 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
--rw-r--r--   0 admin      (501) staff       (20)     7320 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/main.py
--rw-r--r--   0 admin      (501) staff       (20)    10959 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/ollamachat.py
--rw-r--r--   0 admin      (501) staff       (20)       10 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius/package_name.txt
--rw-r--r--   0 admin      (501) staff       (20)     7573 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/palm2.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.536131 freegenius-0.0.95/freegenius/plugins/
--rw-r--r--   0 admin      (501) staff       (20)     1326 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/000_check_ffmpeg.py
--rw-r--r--   0 admin      (501) staff       (20)     1616 2024-04-24 12:46:57.000000 freegenius-0.0.95/freegenius/plugins/000_check_pyaudio.py
--rw-r--r--   0 admin      (501) staff       (20)     1465 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/000_check_vlc.py
--rw-r--r--   0 admin      (501) staff       (20)      115 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/Readme.md
--rw-r--r--   0 admin      (501) staff       (20)     6812 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/add calendar event.py
--rw-r--r--   0 admin      (501) staff       (20)     3358 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/aliases.py
--rw-r--r--   0 admin      (501) staff       (20)     7429 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/analyze audio.py
--rw-r--r--   0 admin      (501) staff       (20)     2154 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/analyze files.py
--rw-r--r--   0 admin      (501) staff       (20)     4667 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/analyze images.py
--rw-r--r--   0 admin      (501) staff       (20)     2316 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/analyze web content.py
--rw-r--r--   0 admin      (501) staff       (20)     2559 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/auto correct python code.py
--rw-r--r--   0 admin      (501) staff       (20)     1860 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/awesome prompts.py
--rw-r--r--   0 admin      (501) staff       (20)     5876 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/character analysis.py
--rw-r--r--   0 admin      (501) staff       (20)      654 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/chat.py
--rw-r--r--   0 admin      (501) staff       (20)      762 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/contexts.py
--rw-r--r--   0 admin      (501) staff       (20)     7220 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/counselling.py
--rw-r--r--   0 admin      (501) staff       (20)     1688 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create ai assistants.py
--rw-r--r--   0 admin      (501) staff       (20)     5152 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create images.py
--rw-r--r--   0 admin      (501) staff       (20)     1262 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create maps.py
--rw-r--r--   0 admin      (501) staff       (20)     1520 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create qrcode.py
--rw-r--r--   0 admin      (501) staff       (20)     1522 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/create statistical graphics.py
--rw-r--r--   0 admin      (501) staff       (20)     1211 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/dates and times.py
--rw-r--r--   0 admin      (501) staff       (20)     3950 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/download youtube or web content.py
--rw-r--r--   0 admin      (501) staff       (20)     1862 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/edit text.py
--rw-r--r--   0 admin      (501) staff       (20)     3316 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/execute computing tasks.py
--rw-r--r--   0 admin      (501) staff       (20)     4213 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/execute termux command.py
--rw-r--r--   0 admin      (501) staff       (20)     6940 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/global finance.py
--rw-r--r--   0 admin      (501) staff       (20)      975 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/improve British English.py
--rw-r--r--   0 admin      (501) staff       (20)     2315 2024-04-24 18:08:35.000000 freegenius-0.0.95/freegenius/plugins/input suggestions.py
--rw-r--r--   0 admin      (501) staff       (20)     1077 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/install python package.py
--rw-r--r--   0 admin      (501) staff       (20)     1670 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/integrate google searches.py
--rw-r--r--   0 admin      (501) staff       (20)     4606 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/memory.py
--rw-r--r--   0 admin      (501) staff       (20)     8638 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/modify images.py
--rw-r--r--   0 admin      (501) staff       (20)      944 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/open web browser.py
--rw-r--r--   0 admin      (501) staff       (20)     1296 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/pronounce words.py
--rw-r--r--   0 admin      (501) staff       (20)     2409 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/remove image background.py
--rw-r--r--   0 admin      (501) staff       (20)     5898 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search chat records.py
--rw-r--r--   0 admin      (501) staff       (20)     1156 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search financial data.py
--rw-r--r--   0 admin      (501) staff       (20)     1966 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search latest news.py
--rw-r--r--   0 admin      (501) staff       (20)     3479 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search sqlite.py
--rw-r--r--   0 admin      (501) staff       (20)     1539 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/search weather info.py
--rw-r--r--   0 admin      (501) staff       (20)     3987 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/send email.py
--rw-r--r--   0 admin      (501) staff       (20)      898 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/send tweet.py
--rw-r--r--   0 admin      (501) staff       (20)     1280 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/send whatsapp messages.py
--rw-r--r--   0 admin      (501) staff       (20)      528 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/plugins/simplified Chinese to traditional Chinese.py
--rw-r--r--   0 admin      (501) staff       (20)      242 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/qt.py
--rw-r--r--   0 admin      (501) staff       (20)     9711 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/rag.py
--rw-r--r--   0 admin      (501) staff       (20)      796 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/requirements.txt
--rw-r--r--   0 admin      (501) staff       (20)     1293 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/servers.py
--rw-r--r--   0 admin      (501) staff       (20)     7691 2024-04-24 16:18:44.000000 freegenius-0.0.95/freegenius/systemtray.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.536259 freegenius-0.0.95/freegenius/temp/
--rw-r--r--   0 admin      (501) staff       (20)       36 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/temp/Readme.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.543837 freegenius-0.0.95/freegenius/utils/
--rw-r--r--   0 admin      (501) staff       (20)   108133 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/assistant.py
--rw-r--r--   0 admin      (501) staff       (20)    29582 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/call_chatgpt.py
--rw-r--r--   0 admin      (501) staff       (20)    17109 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/call_gemini.py
--rw-r--r--   0 admin      (501) staff       (20)    22247 2024-04-25 09:02:38.000000 freegenius-0.0.95/freegenius/utils/call_llamacpp.py
--rw-r--r--   0 admin      (501) staff       (20)     7664 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/call_llm.py
--rw-r--r--   0 admin      (501) staff       (20)    18715 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/call_ollama.py
--rw-r--r--   0 admin      (501) staff       (20)    16449 2024-04-25 09:58:59.000000 freegenius-0.0.95/freegenius/utils/config_essential.py
--rw-r--r--   0 admin      (501) staff       (20)     2616 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/config_tools.py
--rw-r--r--   0 admin      (501) staff       (20)     1368 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/download.py
--rw-r--r--   0 admin      (501) staff       (20)    14296 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/get_path_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)     4888 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/ollama_models.py
--rw-r--r--   0 admin      (501) staff       (20)     3872 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/promptValidator.py
--rw-r--r--   0 admin      (501) staff       (20)     6973 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/prompt_multiline_shared_key_bindings.py
--rw-r--r--   0 admin      (501) staff       (20)     7880 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/prompt_shared_key_bindings.py
--rw-r--r--   0 admin      (501) staff       (20)    21592 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/prompts.py
--rw-r--r--   0 admin      (501) staff       (20)     1681 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/python_utils.py
--rw-r--r--   0 admin      (501) staff       (20)    48047 2024-04-25 10:17:59.000000 freegenius-0.0.95/freegenius/utils/shared_utils.py
--rw-r--r--   0 admin      (501) staff       (20)    21476 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/shortcuts.py
--rw-r--r--   0 admin      (501) staff       (20)     8558 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/single_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)     7936 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/streaming_word_wrapper.py
--rw-r--r--   0 admin      (501) staff       (20)     7580 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/sttLanguages.py
--rw-r--r--   0 admin      (501) staff       (20)     4781 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/terminal_mode_dialogs.py
--rwxr-xr-x   0 admin      (501) staff       (20)     9891 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/terminal_system_command_prompt.py
--rw-r--r--   0 admin      (501) staff       (20)    23917 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/text_utils.py
--rw-r--r--   0 admin      (501) staff       (20)     4352 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/tool_plugins.py
--rw-r--r--   0 admin      (501) staff       (20)     7640 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/ttsLanguages.py
--rw-r--r--   0 admin      (501) staff       (20)     8563 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/tts_utils.py
--rw-r--r--   0 admin      (501) staff       (20)     4651 2024-04-24 10:05:32.000000 freegenius-0.0.95/freegenius/utils/vlc_utils.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-04-25 10:18:44.506422 freegenius-0.0.95/freegenius.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)    11440 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)     5856 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)     1226 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/entry_points.txt
--rw-r--r--   0 admin      (501) staff       (20)      797 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)       11 2024-04-25 10:18:44.000000 freegenius-0.0.95/freegenius.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2024-04-25 10:18:44.544600 freegenius-0.0.95/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)    10383 2024-04-25 10:18:09.000000 freegenius-0.0.95/setup.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.866748 freegenius-0.0.97/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    13438 2024-04-25 15:50:35.866748 freegenius-0.0.97/PKG-INFO
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10310 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius/README.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-11 08:45:18.000000 freegenius-0.0.97/freegenius/__init__.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/audio/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    15588 2024-02-18 17:53:14.000000 freegenius-0.0.97/freegenius/audio/notification1.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2925 2024-02-20 11:12:21.000000 freegenius-0.0.97/freegenius/audio/notification1_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    19428 2024-02-18 17:51:50.000000 freegenius-0.0.97/freegenius/audio/notification2.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3693 2024-02-20 11:18:40.000000 freegenius-0.0.97/freegenius/audio/notification2_mild.mp3
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6646 2024-04-11 14:37:13.000000 freegenius-0.0.97/freegenius/autoassist.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9421 2024-04-13 20:55:38.000000 freegenius-0.0.97/freegenius/autobuilder.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10727 2024-04-11 14:37:13.000000 freegenius-0.0.97/freegenius/autoretriever.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6933 2024-04-03 20:55:06.000000 freegenius-0.0.97/freegenius/chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7037 2024-04-03 20:55:57.000000 freegenius-0.0.97/freegenius/codey.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      833 2024-03-25 21:25:36.000000 freegenius-0.0.97/freegenius/commandprompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius/config.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29583 2023-12-02 22:39:56.000000 freegenius-0.0.97/freegenius/eTextEdit.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/files/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       31 2023-11-28 12:28:19.000000 freegenius-0.0.97/freegenius/files/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    11372 2024-04-16 20:22:58.000000 freegenius-0.0.97/freegenius/geminipro.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7838 2024-04-16 20:22:58.000000 freegenius-0.0.97/freegenius/geminiprovision.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/gui/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9741 2024-04-09 22:46:08.000000 freegenius-0.0.97/freegenius/gui/chatgui.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-03-12 11:57:01.000000 freegenius-0.0.97/freegenius/gui/worker.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.822748 freegenius-0.0.97/freegenius/history/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       29 2023-11-28 12:28:19.000000 freegenius-0.0.97/freegenius/history/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.842748 freegenius-0.0.97/freegenius/icons/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   158655 2024-04-10 10:01:55.000000 freegenius-0.0.97/freegenius/icons/FreeGenius.ico
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2549036 2024-04-10 09:49:32.000000 freegenius-0.0.97/freegenius/icons/FreeGenius.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3162696 2024-04-10 09:20:11.000000 freegenius-0.0.97/freegenius/icons/FreeGenius_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  3141194 2024-04-10 09:41:18.000000 freegenius-0.0.97/freegenius/icons/ai.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)  2390858 2024-04-10 09:27:35.000000 freegenius-0.0.97/freegenius/icons/ai_original.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8119 2024-04-11 14:34:40.000000 freegenius-0.0.97/freegenius/llamacpp.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.814748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.846748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      644 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.846748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5680 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.814748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.846748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5679 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      635 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4100 2023-12-01 10:53:39.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5684 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      649 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      643 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)      640 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-01 10:53:44.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5656 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.850748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-07 18:59:13.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5681 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.818748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.854748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      647 2024-04-06 16:47:12.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.854748 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4273 2023-12-09 18:05:15.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5692 2024-04-06 16:46:45.000000 freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7320 2024-04-10 10:50:28.000000 freegenius-0.0.97/freegenius/main.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10959 2024-04-07 18:24:27.000000 freegenius-0.0.97/freegenius/ollamachat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       10 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius/package_name.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7573 2024-04-03 20:57:58.000000 freegenius-0.0.97/freegenius/palm2.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.858748 freegenius-0.0.97/freegenius/plugins/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1326 2024-03-25 18:25:44.000000 freegenius-0.0.97/freegenius/plugins/000_check_ffmpeg.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1616 2024-04-25 10:21:23.000000 freegenius-0.0.97/freegenius/plugins/000_check_pyaudio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1465 2024-03-25 18:26:33.000000 freegenius-0.0.97/freegenius/plugins/000_check_vlc.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      115 2023-11-28 12:28:19.000000 freegenius-0.0.97/freegenius/plugins/Readme.md
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6812 2024-04-12 22:35:03.000000 freegenius-0.0.97/freegenius/plugins/add calendar event.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3358 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/aliases.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7429 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/plugins/analyze audio.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2154 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/plugins/analyze files.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4667 2024-04-11 14:37:13.000000 freegenius-0.0.97/freegenius/plugins/analyze images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2316 2024-04-09 22:27:35.000000 freegenius-0.0.97/freegenius/plugins/analyze web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2559 2024-04-14 22:20:21.000000 freegenius-0.0.97/freegenius/plugins/auto correct python code.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1860 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/awesome prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5876 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/character analysis.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      654 2024-04-04 22:28:27.000000 freegenius-0.0.97/freegenius/plugins/chat.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      762 2024-04-04 08:36:50.000000 freegenius-0.0.97/freegenius/plugins/contexts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7220 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/counselling.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1688 2024-04-04 22:11:59.000000 freegenius-0.0.97/freegenius/plugins/create ai assistants.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5152 2024-04-11 14:32:24.000000 freegenius-0.0.97/freegenius/plugins/create images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1262 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/create maps.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1520 2024-04-04 22:15:17.000000 freegenius-0.0.97/freegenius/plugins/create qrcode.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1522 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/create statistical graphics.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1211 2024-04-13 22:43:22.000000 freegenius-0.0.97/freegenius/plugins/dates and times.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3950 2024-04-09 22:27:52.000000 freegenius-0.0.97/freegenius/plugins/download youtube or web content.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1862 2024-04-05 11:08:57.000000 freegenius-0.0.97/freegenius/plugins/edit text.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3316 2024-04-13 22:42:39.000000 freegenius-0.0.97/freegenius/plugins/execute computing tasks.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4213 2024-04-09 22:24:00.000000 freegenius-0.0.97/freegenius/plugins/execute termux command.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6940 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/global finance.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      975 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/improve British English.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2315 2024-04-25 10:21:23.000000 freegenius-0.0.97/freegenius/plugins/input suggestions.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1077 2024-04-07 19:39:31.000000 freegenius-0.0.97/freegenius/plugins/install python package.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1670 2024-04-04 22:36:17.000000 freegenius-0.0.97/freegenius/plugins/integrate google searches.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4606 2024-04-11 22:17:28.000000 freegenius-0.0.97/freegenius/plugins/memory.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8638 2024-04-11 14:37:13.000000 freegenius-0.0.97/freegenius/plugins/modify images.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      944 2024-04-09 22:25:30.000000 freegenius-0.0.97/freegenius/plugins/open web browser.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1296 2024-04-05 11:14:34.000000 freegenius-0.0.97/freegenius/plugins/pronounce words.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2409 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/remove image background.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5898 2024-04-10 13:47:59.000000 freegenius-0.0.97/freegenius/plugins/search chat records.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1156 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/search financial data.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1966 2024-04-04 22:42:40.000000 freegenius-0.0.97/freegenius/plugins/search latest news.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3479 2024-04-11 22:13:56.000000 freegenius-0.0.97/freegenius/plugins/search sqlite.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1539 2024-04-10 07:42:48.000000 freegenius-0.0.97/freegenius/plugins/search weather info.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3987 2024-04-09 22:25:48.000000 freegenius-0.0.97/freegenius/plugins/send email.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      898 2024-04-09 22:26:03.000000 freegenius-0.0.97/freegenius/plugins/send tweet.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1280 2024-04-05 11:15:56.000000 freegenius-0.0.97/freegenius/plugins/send whatsapp messages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      528 2024-04-02 21:37:01.000000 freegenius-0.0.97/freegenius/plugins/simplified Chinese to traditional Chinese.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      242 2024-03-25 12:56:42.000000 freegenius-0.0.97/freegenius/qt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     9711 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/rag.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      828 2024-04-25 15:49:57.000000 freegenius-0.0.97/freegenius/requirements.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1293 2024-04-11 16:00:15.000000 freegenius-0.0.97/freegenius/servers.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7691 2024-04-16 20:07:13.000000 freegenius-0.0.97/freegenius/systemtray.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.858748 freegenius-0.0.97/freegenius/temp/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       36 2023-11-28 12:28:19.000000 freegenius-0.0.97/freegenius/temp/Readme.md
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.862748 freegenius-0.0.97/freegenius/utils/
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)   108994 2024-04-25 15:33:09.000000 freegenius-0.0.97/freegenius/utils/assistant.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    29718 2024-04-25 13:47:07.000000 freegenius-0.0.97/freegenius/utils/call_chatgpt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17236 2024-04-25 13:53:07.000000 freegenius-0.0.97/freegenius/utils/call_gemini.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    22590 2024-04-25 13:45:00.000000 freegenius-0.0.97/freegenius/utils/call_llamacpp.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7664 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/utils/call_llm.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    18680 2024-04-25 13:45:52.000000 freegenius-0.0.97/freegenius/utils/call_ollama.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    17552 2024-04-25 15:16:21.000000 freegenius-0.0.97/freegenius/utils/config_essential.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     2616 2024-04-03 21:01:16.000000 freegenius-0.0.97/freegenius/utils/config_tools.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1368 2024-03-27 21:22:10.000000 freegenius-0.0.97/freegenius/utils/download.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    14296 2024-04-03 21:01:58.000000 freegenius-0.0.97/freegenius/utils/get_path_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4888 2024-04-23 21:13:11.000000 freegenius-0.0.97/freegenius/utils/ollama_models.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     3872 2024-04-09 22:46:08.000000 freegenius-0.0.97/freegenius/utils/promptValidator.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     6973 2024-03-25 11:20:01.000000 freegenius-0.0.97/freegenius/utils/prompt_multiline_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7880 2024-04-09 22:40:12.000000 freegenius-0.0.97/freegenius/utils/prompt_shared_key_bindings.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21592 2024-04-09 22:46:08.000000 freegenius-0.0.97/freegenius/utils/prompts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1681 2024-04-12 23:13:01.000000 freegenius-0.0.97/freegenius/utils/python_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    49430 2024-04-25 15:16:34.000000 freegenius-0.0.97/freegenius/utils/shared_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    21476 2024-04-10 11:33:28.000000 freegenius-0.0.97/freegenius/utils/shortcuts.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8558 2024-04-04 08:45:13.000000 freegenius-0.0.97/freegenius/utils/single_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7936 2024-04-09 10:22:46.000000 freegenius-0.0.97/freegenius/utils/streaming_word_wrapper.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7580 2024-02-22 12:18:47.000000 freegenius-0.0.97/freegenius/utils/sttLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4781 2024-03-26 19:39:22.000000 freegenius-0.0.97/freegenius/utils/terminal_mode_dialogs.py
+-rwxrwxr-x   0 eliran    (1000) eliran    (1000)     9891 2024-04-03 21:02:14.000000 freegenius-0.0.97/freegenius/utils/terminal_system_command_prompt.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    23917 2024-03-12 11:57:01.000000 freegenius-0.0.97/freegenius/utils/text_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4352 2024-04-12 22:26:19.000000 freegenius-0.0.97/freegenius/utils/tool_plugins.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     7640 2024-02-22 00:47:05.000000 freegenius-0.0.97/freegenius/utils/ttsLanguages.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     8563 2024-03-28 23:38:45.000000 freegenius-0.0.97/freegenius/utils/tts_utils.py
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     4651 2024-04-09 22:46:08.000000 freegenius-0.0.97/freegenius/utils/vlc_utils.py
+drwxrwxr-x   0 eliran    (1000) eliran    (1000)        0 2024-04-25 15:50:35.862748 freegenius-0.0.97/freegenius.egg-info/
+-rw-r--r--   0 eliran    (1000) eliran    (1000)    13438 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/PKG-INFO
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     5856 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/SOURCES.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)        1 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/dependency_links.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)     1226 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/entry_points.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)      829 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/requires.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       11 2024-04-25 15:50:35.000000 freegenius-0.0.97/freegenius.egg-info/top_level.txt
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)       38 2024-04-25 15:50:35.866748 freegenius-0.0.97/setup.cfg
+-rw-rw-r--   0 eliran    (1000) eliran    (1000)    10383 2024-04-25 15:19:09.000000 freegenius-0.0.97/setup.py
```

### Comparing `freegenius-0.0.95/PKG-INFO` & `freegenius-0.0.97/freegenius/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,15 @@
-Metadata-Version: 2.1
-Name: freegenius
-Version: 0.0.95
-Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
-Home-page: https://letmedoit.ai
-Author: Eliran Wong
-Author-email: support@letmedoit.ai
-License: GNU General Public License (GPL)
-Project-URL: Source, https://github.com/eliranwong/letmedoit
-Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
-Project-URL: Documentation, https://github.com/eliranwong/letmedoit/wiki
-Project-URL: Funding, https://www.paypal.me/letmedoitai
-Keywords: ai assistant ollama llama llamacpp openai chatgpt gemini autogen rag agent stable-diffusion
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Topic :: Utilities
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8, <3.12
-
 # FreeGenius AI
 
 FreeGenius AI is an ambitious project sparked by the pioneering work of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). It's designed with the primary objective of offering a comprehensive suite of AI solutions that mirror the capabilities of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). However, FreeGenius AI is remarkably different in that all core features are completely free, and it doesn't require the use of an OpenAI key.
 
 As with [LetMeDoIt AI](https://github.com/eliranwong/letmedoit), FreeGenius AI is designed to be capable of engaging in intuitive conversations, executing codes, providing up-to-date information, and performing a wide range of tasks. It's designed to learn, adapt, and grow with the user, offering personalized experiences and interactions.
 
+![freegenius_ai_screenshot](https://github.com/eliranwong/freegenius/assets/25262722/1e9dd18e-aa4b-4e2c-8d76-386af7ba00ea)
+
 # Beyond LetMeDoIt AI
 
 https://github.com/eliranwong/freegenius/wiki/Beyond-LetMeDoIt-AI
 
 # Goals
 
 The author aims to equip FreeGenius AI, as an AI suite that is able to:
@@ -96,14 +73,18 @@
 ## Speech-to-Text Options
 
 1. Google Text-to-Speech (Generic)
 2. Google Text-to-Speech (API)
 3. Elevenlabs (API)
 4. Custom system commands
 
+# Highly Customizable
+
+![plugins](https://github.com/eliranwong/freegenius/assets/25262722/6bb4b2f6-5684-42c1-95e3-7b12c3a38db6)
+
 # Installation
 
 Install FreeGenius AI, by running:
 
 To set up virtual environment (recommended):
 
 > mkdir -p ~/apps/freegenius
@@ -355,8 +336,8 @@
 
 * joining the development collaboratively
 
 * donations to show support and invest for the future
 
 Support link: https://www.paypal.me/letmedoitai
 
-Please kindly report of any issues at https://github.com/eliranwong/freegenius/issues
+Please kindly report of any issues at https://github.com/eliranwong/freegenius/issues
```

### Comparing `freegenius-0.0.95/freegenius/__init__.py` & `freegenius-0.0.97/freegenius/__init__.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/audio/notification1.mp3` & `freegenius-0.0.97/freegenius/audio/notification1.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/audio/notification1_mild.mp3` & `freegenius-0.0.97/freegenius/audio/notification1_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/audio/notification2.mp3` & `freegenius-0.0.97/freegenius/audio/notification2.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/audio/notification2_mild.mp3` & `freegenius-0.0.97/freegenius/audio/notification2_mild.mp3`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/autoassist.py` & `freegenius-0.0.97/freegenius/autoassist.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/autobuilder.py` & `freegenius-0.0.97/freegenius/autobuilder.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/autoretriever.py` & `freegenius-0.0.97/freegenius/autoretriever.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/chatgpt.py` & `freegenius-0.0.97/freegenius/chatgpt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/codey.py` & `freegenius-0.0.97/freegenius/codey.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/commandprompt.py` & `freegenius-0.0.97/freegenius/commandprompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/eTextEdit.py` & `freegenius-0.0.97/freegenius/eTextEdit.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/geminipro.py` & `freegenius-0.0.97/freegenius/geminipro.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/geminiprovision.py` & `freegenius-0.0.97/freegenius/geminiprovision.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/gui/chatgui.py` & `freegenius-0.0.97/freegenius/gui/chatgui.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/gui/worker.py` & `freegenius-0.0.97/freegenius/gui/worker.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/icons/FreeGenius.ico` & `freegenius-0.0.97/freegenius/icons/FreeGenius.ico`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/icons/FreeGenius.png` & `freegenius-0.0.97/freegenius/icons/FreeGenius.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/icons/FreeGenius_original.png` & `freegenius-0.0.97/freegenius/icons/FreeGenius_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/icons/ai.png` & `freegenius-0.0.97/freegenius/icons/ai.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/icons/ai_original.png` & `freegenius-0.0.97/freegenius/icons/ai_original.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/llamacpp.py` & `freegenius-0.0.97/freegenius/llamacpp.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Download_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Explanation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Files_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Pronounce_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Summary_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Text_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_Translation_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/QuickLook/Thumbnail.png`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow` & `freegenius-0.0.97/freegenius/macOS_service/FreeGenius_YoutubeMP3_workflow/Contents/document.wflow`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/main.py` & `freegenius-0.0.97/freegenius/main.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/ollamachat.py` & `freegenius-0.0.97/freegenius/ollamachat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/palm2.py` & `freegenius-0.0.97/freegenius/palm2.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/000_check_ffmpeg.py` & `freegenius-0.0.97/freegenius/plugins/000_check_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/000_check_pyaudio.py` & `freegenius-0.0.97/freegenius/plugins/000_check_pyaudio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/000_check_vlc.py` & `freegenius-0.0.97/freegenius/plugins/000_check_vlc.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/add calendar event.py` & `freegenius-0.0.97/freegenius/plugins/add calendar event.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/aliases.py` & `freegenius-0.0.97/freegenius/plugins/aliases.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/analyze audio.py` & `freegenius-0.0.97/freegenius/plugins/analyze audio.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/analyze files.py` & `freegenius-0.0.97/freegenius/plugins/analyze files.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/analyze images.py` & `freegenius-0.0.97/freegenius/plugins/analyze images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/analyze web content.py` & `freegenius-0.0.97/freegenius/plugins/analyze web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/auto correct python code.py` & `freegenius-0.0.97/freegenius/plugins/auto correct python code.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/awesome prompts.py` & `freegenius-0.0.97/freegenius/plugins/awesome prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/character analysis.py` & `freegenius-0.0.97/freegenius/plugins/character analysis.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/chat.py` & `freegenius-0.0.97/freegenius/plugins/chat.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/contexts.py` & `freegenius-0.0.97/freegenius/plugins/contexts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/counselling.py` & `freegenius-0.0.97/freegenius/plugins/counselling.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/create ai assistants.py` & `freegenius-0.0.97/freegenius/plugins/create ai assistants.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/create images.py` & `freegenius-0.0.97/freegenius/plugins/create images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/create maps.py` & `freegenius-0.0.97/freegenius/plugins/create maps.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/create qrcode.py` & `freegenius-0.0.97/freegenius/plugins/create qrcode.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/create statistical graphics.py` & `freegenius-0.0.97/freegenius/plugins/create statistical graphics.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/dates and times.py` & `freegenius-0.0.97/freegenius/plugins/dates and times.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/download youtube or web content.py` & `freegenius-0.0.97/freegenius/plugins/download youtube or web content.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/edit text.py` & `freegenius-0.0.97/freegenius/plugins/edit text.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/execute computing tasks.py` & `freegenius-0.0.97/freegenius/plugins/execute computing tasks.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/execute termux command.py` & `freegenius-0.0.97/freegenius/plugins/execute termux command.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/global finance.py` & `freegenius-0.0.97/freegenius/plugins/global finance.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/improve British English.py` & `freegenius-0.0.97/freegenius/plugins/improve British English.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/input suggestions.py` & `freegenius-0.0.97/freegenius/plugins/input suggestions.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/install python package.py` & `freegenius-0.0.97/freegenius/plugins/install python package.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/integrate google searches.py` & `freegenius-0.0.97/freegenius/plugins/integrate google searches.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/memory.py` & `freegenius-0.0.97/freegenius/plugins/memory.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/modify images.py` & `freegenius-0.0.97/freegenius/plugins/modify images.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/open web browser.py` & `freegenius-0.0.97/freegenius/plugins/open web browser.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/pronounce words.py` & `freegenius-0.0.97/freegenius/plugins/pronounce words.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/remove image background.py` & `freegenius-0.0.97/freegenius/plugins/remove image background.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/search chat records.py` & `freegenius-0.0.97/freegenius/plugins/search chat records.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/search financial data.py` & `freegenius-0.0.97/freegenius/plugins/search financial data.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/search latest news.py` & `freegenius-0.0.97/freegenius/plugins/search latest news.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/search sqlite.py` & `freegenius-0.0.97/freegenius/plugins/search sqlite.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/search weather info.py` & `freegenius-0.0.97/freegenius/plugins/search weather info.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/send email.py` & `freegenius-0.0.97/freegenius/plugins/send email.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/send tweet.py` & `freegenius-0.0.97/freegenius/plugins/send tweet.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/send whatsapp messages.py` & `freegenius-0.0.97/freegenius/plugins/send whatsapp messages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/plugins/simplified Chinese to traditional Chinese.py` & `freegenius-0.0.97/freegenius/plugins/simplified Chinese to traditional Chinese.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/rag.py` & `freegenius-0.0.97/freegenius/rag.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/requirements.txt` & `freegenius-0.0.97/freegenius/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 rembg
 qrcode
 pyperclip
 colorama
 pillow
 docker
 einops
-transformers
+transformers==4.40.1
 torch==2.2.2
 torchvision==0.17.2
 sentence-transformers
 chromadb==0.4.24
 unstructured[all-docs]
 pyautogen[retrievechat,autobuild]==0.2.24
 autogenstudio==0.0.56
@@ -49,12 +49,13 @@
 soundfile==0.12.1
 sounddevice==0.4.6
 elevenlabs==1.0.3
 ollama==0.1.8
 llama-cpp-python[server]==0.2.61
 huggingface-hub
 langchain==0.1.13
+langchain_openai==0.1.3
 pydub
 stable-diffusion-cpp-python
 pytz
 geopy
 guidance==0.1.13
```

### Comparing `freegenius-0.0.95/freegenius/servers.py` & `freegenius-0.0.97/freegenius/servers.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/systemtray.py` & `freegenius-0.0.97/freegenius/systemtray.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/assistant.py` & `freegenius-0.0.97/freegenius/utils/assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -2983,3777 +2983,3831 @@
 0000ba60: 3d3d 2022 7965 7322 3a0a 2020 2020 2020  == "yes":.      
 0000ba70: 2020 2020 2020 2020 2020 636f 6e66 6967            config
 0000ba80: 2e75 7365 4164 6469 7469 6f6e 616c 4368  .useAdditionalCh
 0000ba90: 6174 4d6f 6465 6c20 3d20 5472 7565 0a20  atModel = True. 
 0000baa0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
 0000bab0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
 0000bac0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-0000bad0: 6c73 650a 0a20 2020 2020 2020 2063 7572  lse..        cur
-0000bae0: 7265 6e74 4c6c 6d49 6e74 6572 6661 6365  rentLlmInterface
-0000baf0: 203d 2063 6f6e 6669 672e 6c6c 6d49 6e74   = config.llmInt
-0000bb00: 6572 6661 6365 0a20 2020 2020 2020 2073  erface.        s
-0000bb10: 656c 662e 7365 6c65 6374 4c6c 6d50 6c61  elf.selectLlmPla
-0000bb20: 7466 6f72 6d28 290a 0a20 2020 2020 2020  tform()..       
-0000bb30: 2070 7269 6e74 3128 2253 656c 6563 7420   print1("Select 
-0000bb40: 6d6f 6465 6c73 202e 2e2e 2229 0a20 2020  models ...").   
-0000bb50: 2020 2020 2069 6620 636f 6e66 6967 2e6c       if config.l
-0000bb60: 6c6d 496e 7465 7266 6163 6520 3d3d 2022  lmInterface == "
-0000bb70: 6f6c 6c61 6d61 223a 0a20 2020 2020 2020  ollama":.       
-0000bb80: 2020 2020 2070 7269 6e74 3228 2223 204d       print2("# M
-0000bb90: 6169 6e20 4d6f 6465 6c20 2d20 666f 7220  ain Model - for 
-0000bba0: 626f 7468 2074 6173 6b20 6578 6563 7574  both task execut
-0000bbb0: 696f 6e20 616e 6420 636f 6e76 6572 7361  ion and conversa
-0000bbc0: 7469 6f6e 2229 0a20 2020 2020 2020 2020  tion").         
-0000bbd0: 2020 2073 656c 662e 7365 744c 6c6d 4d6f     self.setLlmMo
-0000bbe0: 6465 6c5f 6f6c 6c61 6d61 2829 0a20 2020  del_ollama().   
-0000bbf0: 2020 2020 2020 2020 2069 6620 6173 6b41           if askA
-0000bc00: 6464 6974 696f 6e61 6c43 6861 744d 6f64  dditionalChatMod
-0000bc10: 656c 2829 3a0a 2020 2020 2020 2020 2020  el():.          
-0000bc20: 2020 2020 2020 7072 696e 7432 2822 2320        print2("# 
-0000bc30: 4368 6174 204d 6f64 656c 202d 2066 6f72  Chat Model - for
-0000bc40: 2063 6f6e 7665 7273 6174 696f 6e20 6f6e   conversation on
-0000bc50: 6c79 2229 0a20 2020 2020 2020 2020 2020  ly").           
-0000bc60: 2020 2020 2073 656c 662e 7365 744c 6c6d       self.setLlm
-0000bc70: 4d6f 6465 6c5f 6f6c 6c61 6d61 2822 636f  Model_ollama("co
-0000bc80: 6465 2229 0a20 2020 2020 2020 2065 6c69  de").        eli
-0000bc90: 6620 636f 6e66 6967 2e6c 6c6d 496e 7465  f config.llmInte
-0000bca0: 7266 6163 6520 3d3d 2022 6c6c 616d 6163  rface == "llamac
-0000bcb0: 7070 223a 0a20 2020 2020 2020 2020 2020  pp":.           
-0000bcc0: 2070 7269 6e74 3228 2223 204d 6169 6e20   print2("# Main 
-0000bcd0: 4d6f 6465 6c20 2d20 666f 7220 626f 7468  Model - for both
-0000bce0: 2074 6173 6b20 6578 6563 7574 696f 6e20   task execution 
-0000bcf0: 616e 6420 636f 6e76 6572 7361 7469 6f6e  and conversation
-0000bd00: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
-0000bd10: 656c 662e 7365 744c 6c6d 4d6f 6465 6c5f  elf.setLlmModel_
-0000bd20: 6c6c 616d 6163 7070 2829 0a20 2020 2020  llamacpp().     
-0000bd30: 2020 2020 2020 2069 6620 6173 6b41 6464         if askAdd
-0000bd40: 6974 696f 6e61 6c43 6861 744d 6f64 656c  itionalChatModel
-0000bd50: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-0000bd60: 2020 2020 7072 696e 7432 2822 2320 4368      print2("# Ch
-0000bd70: 6174 204d 6f64 656c 202d 2066 6f72 2063  at Model - for c
-0000bd80: 6f6e 7665 7273 6174 696f 6e20 6f6e 6c79  onversation only
-0000bd90: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000bda0: 2020 2073 656c 662e 7365 744c 6c6d 4d6f     self.setLlmMo
-0000bdb0: 6465 6c5f 6c6c 616d 6163 7070 2822 636f  del_llamacpp("co
-0000bdc0: 6465 2229 0a20 2020 2020 2020 2065 6c69  de").        eli
-0000bdd0: 6620 636f 6e66 6967 2e6c 6c6d 496e 7465  f config.llmInte
-0000bde0: 7266 6163 6520 3d3d 2022 6765 6d69 6e69  rface == "gemini
-0000bdf0: 223a 0a20 2020 2020 2020 2020 2020 2070  ":.            p
-0000be00: 7269 6e74 3328 224d 6f64 656c 2073 656c  rint3("Model sel
-0000be10: 6563 7465 643a 2047 6f6f 676c 6520 4765  ected: Google Ge
-0000be20: 6d69 6e69 2050 726f 2229 0a20 2020 2020  mini Pro").     
-0000be30: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000be40: 2020 2020 2073 656c 662e 7365 744c 6c6d       self.setLlm
-0000be50: 4d6f 6465 6c5f 6368 6174 6770 7428 290a  Model_chatgpt().
-0000be60: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
-0000be70: 6176 6543 6f6e 6669 6728 290a 2020 2020  aveConfig().    
-0000be80: 2020 2020 6966 206e 6f74 2063 6f6e 6669      if not confi
-0000be90: 672e 6c6c 6d49 6e74 6572 6661 6365 203d  g.llmInterface =
-0000bea0: 3d20 6375 7272 656e 744c 6c6d 496e 7465  = currentLlmInte
-0000beb0: 7266 6163 653a 0a20 2020 2020 2020 2020  rface:.         
-0000bec0: 2020 2070 7269 6e74 3228 224c 4c4d 2049     print2("LLM I
-0000bed0: 6e74 6572 6661 6365 2063 6861 6e67 6564  nterface changed
-0000bee0: 2120 5374 6172 7469 6e67 2061 206e 6577  ! Starting a new
-0000bef0: 2063 6861 7420 7365 7373 696f 6e20 2e2e   chat session ..
-0000bf00: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-0000bf10: 636f 6e66 6967 2e64 6566 6175 6c74 456e  config.defaultEn
-0000bf20: 7472 7920 3d20 222e 6e65 7722 0a20 2020  try = ".new".   
-0000bf30: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-0000bf40: 6163 6365 7074 5f64 6566 6175 6c74 203d  accept_default =
-0000bf50: 2054 7275 650a 0a20 2020 2064 6566 2073   True..    def s
-0000bf60: 656c 6563 744f 6c6c 616d 614d 6f64 656c  electOllamaModel
-0000bf70: 2873 656c 662c 206d 6573 7361 6765 3d22  (self, message="
-0000bf80: 5365 6c65 6374 2061 206d 6f64 656c 2066  Select a model f
-0000bf90: 726f 6d20 4f6c 6c61 6d61 204c 6962 7261  rom Ollama Libra
-0000bfa0: 7279 3a22 2c20 6665 6174 7572 653d 2264  ry:", feature="d
-0000bfb0: 6566 6175 6c74 2229 202d 3e20 7374 723a  efault") -> str:
-0000bfc0: 0a20 2020 2020 2020 2023 2068 6973 746f  .        # histo
-0000bfd0: 7279 2073 6573 7369 6f6e 0a20 2020 2020  ry session.     
-0000bfe0: 2020 2068 6973 746f 7279 466f 6c64 6572     historyFolder
-0000bff0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
-0000c000: 636f 6e66 6967 2e6c 6f63 616c 5374 6f72  config.localStor
-0000c010: 6167 652c 2022 6869 7374 6f72 7922 290a  age, "history").
-0000c020: 2020 2020 2020 2020 5061 7468 2868 6973          Path(his
-0000c030: 746f 7279 466f 6c64 6572 292e 6d6b 6469  toryFolder).mkdi
-0000c040: 7228 7061 7265 6e74 733d 5472 7565 2c20  r(parents=True, 
-0000c050: 6578 6973 745f 6f6b 3d54 7275 6529 0a20  exist_ok=True). 
-0000c060: 2020 2020 2020 206d 6f64 656c 5f68 6973         model_his
-0000c070: 746f 7279 203d 206f 732e 7061 7468 2e6a  tory = os.path.j
-0000c080: 6f69 6e28 6869 7374 6f72 7946 6f6c 6465  oin(historyFolde
-0000c090: 722c 2022 6f6c 6c61 6d61 5f63 6f64 6522  r, "ollama_code"
-0000c0a0: 2069 6620 6665 6174 7572 6520 3d3d 2022   if feature == "
-0000c0b0: 636f 6465 2220 656c 7365 2022 6f6c 6c61  code" else "olla
-0000c0c0: 6d61 5f64 6566 6175 6c74 2229 0a20 2020  ma_default").   
-0000c0d0: 2020 2020 206d 6f64 656c 5f73 6573 7369       model_sessi
-0000c0e0: 6f6e 203d 2050 726f 6d70 7453 6573 7369  on = PromptSessi
-0000c0f0: 6f6e 2868 6973 746f 7279 3d46 696c 6548  on(history=FileH
-0000c100: 6973 746f 7279 286d 6f64 656c 5f68 6973  istory(model_his
-0000c110: 746f 7279 2929 0a20 2020 2020 2020 2063  tory)).        c
-0000c120: 6f6d 706c 6574 6572 203d 2046 757a 7a79  ompleter = Fuzzy
-0000c130: 436f 6d70 6c65 7465 7228 576f 7264 436f  Completer(WordCo
-0000c140: 6d70 6c65 7465 7228 736f 7274 6564 286f  mpleter(sorted(o
-0000c150: 6c6c 616d 615f 6d6f 6465 6c73 292c 2069  llama_models), i
-0000c160: 676e 6f72 655f 6361 7365 3d54 7275 6529  gnore_case=True)
-0000c170: 290a 2020 2020 2020 2020 626f 7474 6f6d  ).        bottom
-0000c180: 5f74 6f6f 6c62 6172 203d 2066 2222 2220  _toolbar = f""" 
-0000c190: 7b73 7472 2863 6f6e 6669 672e 686f 746b  {str(config.hotk
-0000c1a0: 6579 5f65 7869 7429 2e72 6570 6c61 6365  ey_exit).replace
-0000c1b0: 2822 2722 2c20 2222 297d 207b 636f 6e66  ("'", "")} {conf
-0000c1c0: 6967 2e65 7869 745f 656e 7472 797d 2222  ig.exit_entry}""
-0000c1d0: 220a 2020 2020 2020 2020 6465 6661 756c  ".        defaul
-0000c1e0: 7420 3d20 636f 6e66 6967 2e6f 6c6c 616d  t = config.ollam
-0000c1f0: 6143 6861 744d 6f64 656c 2069 6620 6665  aChatModel if fe
-0000c200: 6174 7572 6520 3d3d 2022 636f 6465 2220  ature == "code" 
-0000c210: 656c 7365 2063 6f6e 6669 672e 6f6c 6c61  else config.olla
-0000c220: 6d61 4d61 696e 4d6f 6465 6c0a 2020 2020  maMainModel.    
-0000c230: 2020 2020 6966 2063 6f6e 6669 672e 6c6c      if config.ll
-0000c240: 6d49 6e74 6572 6661 6365 203d 3d20 226c  mInterface == "l
-0000c250: 6c61 6d61 6370 7022 3a0a 2020 2020 2020  lamacpp":.      
-0000c260: 2020 2020 2020 6966 2066 6561 7475 7265        if feature
-0000c270: 203d 3d20 2264 6566 6175 6c74 2220 616e   == "default" an
-0000c280: 6420 636f 6e66 6967 2e6c 6c61 6d61 6370  d config.llamacp
-0000c290: 704d 6169 6e4d 6f64 656c 5f6f 6c6c 616d  pMainModel_ollam
-0000c2a0: 615f 7461 673a 0a20 2020 2020 2020 2020  a_tag:.         
-0000c2b0: 2020 2020 2020 2064 6566 6175 6c74 203d         default =
-0000c2c0: 2063 6f6e 6669 672e 6c6c 616d 6163 7070   config.llamacpp
-0000c2d0: 4d61 696e 4d6f 6465 6c5f 6f6c 6c61 6d61  MainModel_ollama
-0000c2e0: 5f74 6167 0a20 2020 2020 2020 2020 2020  _tag.           
-0000c2f0: 2065 6c69 6620 6665 6174 7572 6520 3d3d   elif feature ==
-0000c300: 2022 636f 6465 2220 616e 6420 636f 6e66   "code" and conf
-0000c310: 6967 2e6c 6c61 6d61 6370 7043 6861 744d  ig.llamacppChatM
-0000c320: 6f64 656c 5f6f 6c6c 616d 615f 7461 673a  odel_ollama_tag:
-0000c330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c340: 2064 6566 6175 6c74 203d 2063 6f6e 6669   default = confi
-0000c350: 672e 6c6c 616d 6163 7070 4368 6174 4d6f  g.llamacppChatMo
-0000c360: 6465 6c5f 6f6c 6c61 6d61 5f74 6167 0a20  del_ollama_tag. 
-0000c370: 2020 2020 2020 2023 2070 726f 6d70 740a         # prompt.
-0000c380: 2020 2020 2020 2020 7072 696e 7431 286d          print1(m
-0000c390: 6573 7361 6765 290a 2020 2020 2020 2020  essage).        
-0000c3a0: 7072 696e 7431 2822 2846 6f72 2064 6574  print1("(For det
-0000c3b0: 6169 6c73 2c20 7669 7369 7420 6874 7470  ails, visit http
-0000c3c0: 733a 2f2f 6f6c 6c61 6d61 2e63 6f6d 2f6c  s://ollama.com/l
-0000c3d0: 6962 7261 7279 2922 290a 2020 2020 2020  ibrary)").      
-0000c3e0: 2020 6d6f 6465 6c20 3d20 7365 6c66 2e70    model = self.p
-0000c3f0: 726f 6d70 7473 2e73 696d 706c 6550 726f  rompts.simplePro
-0000c400: 6d70 7428 7374 796c 653d 7365 6c66 2e70  mpt(style=self.p
-0000c410: 726f 6d70 7473 2e70 726f 6d70 7453 7479  rompts.promptSty
-0000c420: 6c65 322c 2070 726f 6d70 7453 6573 7369  le2, promptSessi
-0000c430: 6f6e 3d6d 6f64 656c 5f73 6573 7369 6f6e  on=model_session
-0000c440: 2c20 626f 7474 6f6d 5f74 6f6f 6c62 6172  , bottom_toolbar
-0000c450: 3d62 6f74 746f 6d5f 746f 6f6c 6261 722c  =bottom_toolbar,
-0000c460: 2064 6566 6175 6c74 3d64 6566 6175 6c74   default=default
-0000c470: 2c20 636f 6d70 6c65 7465 723d 636f 6d70  , completer=comp
-0000c480: 6c65 7465 7229 0a20 2020 2020 2020 2069  leter).        i
-0000c490: 6620 6d6f 6465 6c20 616e 6420 6e6f 7420  f model and not 
-0000c4a0: 6d6f 6465 6c2e 6c6f 7765 7228 2920 3d3d  model.lower() ==
-0000c4b0: 2063 6f6e 6669 672e 6578 6974 5f65 6e74   config.exit_ent
-0000c4c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000c4d0: 7265 7475 726e 206d 6f64 656c 0a20 2020  return model.   
-0000c4e0: 2020 2020 2072 6574 7572 6e20 2222 0a0a       return ""..
-0000c4f0: 2020 2020 6465 6620 7365 744c 6c6d 4d6f      def setLlmMo
-0000c500: 6465 6c5f 6f6c 6c61 6d61 2873 656c 662c  del_ollama(self,
-0000c510: 2066 6561 7475 7265 3d22 6465 6661 756c   feature="defaul
-0000c520: 7422 293a 0a20 2020 2020 2020 206d 6f64  t"):.        mod
-0000c530: 656c 203d 2073 656c 662e 7365 6c65 6374  el = self.select
-0000c540: 4f6c 6c61 6d61 4d6f 6465 6c28 6665 6174  OllamaModel(feat
-0000c550: 7572 653d 6665 6174 7572 6529 0a20 2020  ure=feature).   
-0000c560: 2020 2020 2069 6620 6d6f 6465 6c3a 0a20       if model:. 
-0000c570: 2020 2020 2020 2020 2020 2064 6f77 6e6c             downl
-0000c580: 6f61 6465 644f 6c6c 616d 614d 6f64 656c  oadedOllamaModel
-0000c590: 7320 3d20 6765 7444 6f77 6e6c 6f61 6465  s = getDownloade
-0000c5a0: 644f 6c6c 616d 614d 6f64 656c 7328 290a  dOllamaModels().
-0000c5b0: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-0000c5c0: 6f64 656c 2069 6e20 646f 776e 6c6f 6164  odel in download
-0000c5d0: 6564 4f6c 6c61 6d61 4d6f 6465 6c73 3a0a  edOllamaModels:.
-0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5f0: 6966 2066 6561 7475 7265 203d 3d20 2264  if feature == "d
-0000c600: 6566 6175 6c74 223a 0a20 2020 2020 2020  efault":.       
-0000c610: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000c620: 6669 672e 6f6c 6c61 6d61 4d61 696e 4d6f  fig.ollamaMainMo
-0000c630: 6465 6c20 3d20 6d6f 6465 6c0a 2020 2020  del = model.    
-0000c640: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-0000c650: 2066 6561 7475 7265 203d 3d20 2263 6f64   feature == "cod
-0000c660: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
-0000c670: 2020 2020 2020 2020 636f 6e66 6967 2e6f          config.o
-0000c680: 6c6c 616d 6143 6861 744d 6f64 656c 203d  llamaChatModel =
-0000c690: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
-0000c6a0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000c6b0: 2020 2020 2020 2020 2069 6620 7368 7574           if shut
-0000c6c0: 696c 2e77 6869 6368 2822 6f6c 6c61 6d61  il.which("ollama
-0000c6d0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-0000c6e0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-0000c6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c700: 2020 2020 2044 6f77 6e6c 6f61 6465 722e       Downloader.
-0000c710: 646f 776e 6c6f 6164 4f6c 6c61 6d61 4d6f  downloadOllamaMo
-0000c720: 6465 6c28 6d6f 6465 6c2c 2054 7275 6529  del(model, True)
-0000c730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c740: 2020 2020 2020 2020 2069 6620 6665 6174           if feat
-0000c750: 7572 6520 3d3d 2022 6465 6661 756c 7422  ure == "default"
-0000c760: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000c770: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000c780: 6e66 6967 2e6f 6c6c 616d 614d 6169 6e4d  nfig.ollamaMainM
-0000c790: 6f64 656c 203d 206d 6f64 656c 0a20 2020  odel = model.   
-0000c7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7b0: 2020 2020 2065 6c69 6620 6665 6174 7572       elif featur
-0000c7c0: 6520 3d3d 2022 636f 6465 223a 0a20 2020  e == "code":.   
-0000c7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7e0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-0000c7f0: 6f6c 6c61 6d61 4368 6174 4d6f 6465 6c20  ollamaChatModel 
-0000c800: 3d20 6d6f 6465 6c0a 2020 2020 2020 2020  = model.        
-0000c810: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-0000c820: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-0000c830: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0000c840: 7432 2866 2246 6169 6c65 6420 746f 2064  t2(f"Failed to d
-0000c850: 6f77 6e6c 6f61 6420 277b 6d6f 6465 6c7d  ownload '{model}
-0000c860: 2721 2050 6c65 6173 6520 6d61 6b65 2073  '! Please make s
-0000c870: 7572 6520 796f 7520 656e 7465 7220 6120  ure you enter a 
-0000c880: 7661 6c69 6420 6d6f 6465 6c20 6e61 6d65  valid model name
-0000c890: 206f 7220 7461 672e 2229 0a20 2020 2020   or tag.").     
-0000c8a0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000c8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c8c0: 2020 2020 2070 7269 6e74 2822 4f6c 6c61       print("Olla
-0000c8d0: 6d61 206e 6f74 2066 6f75 6e64 2120 496e  ma not found! In
-0000c8e0: 7374 616c 6c20 4f6c 6c61 6d61 2066 6972  stall Ollama fir
-0000c8f0: 7374 2074 6f20 7573 6520 4f6c 6c61 6d61  st to use Ollama
-0000c900: 206d 6f64 656c 206c 6962 7261 7279 2122   model library!"
-0000c910: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c920: 2020 2020 2020 7072 696e 7428 2254 6f20        print("To 
-0000c930: 696e 7374 616c 6c20 4f6c 6c61 6d61 2c20  install Ollama, 
-0000c940: 7669 7369 7420 6874 7470 733a 2f2f 6f6c  visit https://ol
-0000c950: 6c61 6d61 2e63 6f6d 2229 0a0a 2020 2020  lama.com")..    
-0000c960: 6465 6620 7365 744c 6c6d 4d6f 6465 6c5f  def setLlmModel_
-0000c970: 6c6c 616d 6163 7070 2873 656c 662c 2066  llamacpp(self, f
-0000c980: 6561 7475 7265 3d22 6465 6661 756c 7422  eature="default"
-0000c990: 293a 0a20 2020 2020 2020 206c 6962 7261  ):.        libra
-0000c9a0: 7279 203d 2073 656c 662e 6469 616c 6f67  ry = self.dialog
-0000c9b0: 732e 6765 7456 616c 6964 4f70 7469 6f6e  s.getValidOption
-0000c9c0: 7328 0a20 2020 2020 2020 2020 2020 206f  s(.            o
-0000c9d0: 7074 696f 6e73 3d28 224f 6c6c 616d 6120  ptions=("Ollama 
-0000c9e0: 4c69 6272 6172 7922 2c20 2248 7567 6769  Library", "Huggi
-0000c9f0: 6e67 6661 6365 2048 7562 222c 2022 4375  ngface Hub", "Cu
-0000ca00: 7374 6f6d 2047 4755 4622 292c 0a20 2020  stom GGUF"),.   
-0000ca10: 2020 2020 2020 2020 2074 6974 6c65 3d22           title="
-0000ca20: 4d6f 6465 6c20 4c69 6272 6172 7922 2c0a  Model Library",.
-0000ca30: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-0000ca40: 756c 743d 224f 6c6c 616d 6120 4c69 6272  ult="Ollama Libr
-0000ca50: 6172 7922 2069 6620 7368 7574 696c 2e77  ary" if shutil.w
-0000ca60: 6869 6368 2822 6f6c 6c61 6d61 2229 2065  hich("ollama") e
-0000ca70: 6c73 6520 2248 7567 6769 6e67 6661 6365  lse "Huggingface
-0000ca80: 2048 7562 222c 0a20 2020 2020 2020 2020   Hub",.         
-0000ca90: 2020 2074 6578 743d 2253 656c 6563 7420     text="Select 
-0000caa0: 6120 6d6f 6465 6c20 6c69 6272 6172 793a  a model library:
-0000cab0: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
-0000cac0: 2020 2020 2069 6620 6c69 6272 6172 793a       if library:
-0000cad0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000cae0: 6c69 6272 6172 7920 3d3d 2022 4f6c 6c61  library == "Olla
-0000caf0: 6d61 204c 6962 7261 7279 223a 0a20 2020  ma Library":.   
-0000cb00: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-0000cb10: 656c 203d 2073 656c 662e 7365 6c65 6374  el = self.select
-0000cb20: 4f6c 6c61 6d61 4d6f 6465 6c28 6665 6174  OllamaModel(feat
-0000cb30: 7572 653d 6665 6174 7572 6529 0a20 2020  ure=feature).   
-0000cb40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000cb50: 6d6f 6465 6c3a 0a20 2020 2020 2020 2020  model:.         
-0000cb60: 2020 2020 2020 2020 2020 2064 6f77 6e6c             downl
-0000cb70: 6f61 6465 644f 6c6c 616d 614d 6f64 656c  oadedOllamaModel
-0000cb80: 7320 3d20 6765 7444 6f77 6e6c 6f61 6465  s = getDownloade
-0000cb90: 644f 6c6c 616d 614d 6f64 656c 7328 290a  dOllamaModels().
-0000cba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbb0: 2020 2020 6966 206d 6f64 656c 2069 6e20      if model in 
-0000cbc0: 646f 776e 6c6f 6164 6564 4f6c 6c61 6d61  downloadedOllama
-0000cbd0: 4d6f 6465 6c73 3a0a 2020 2020 2020 2020  Models:.        
-0000cbe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cbf0: 6966 2066 6561 7475 7265 203d 3d20 2264  if feature == "d
-0000cc00: 6566 6175 6c74 223a 0a20 2020 2020 2020  efault":.       
+0000bad0: 6c73 650a 2020 2020 2020 2020 6465 6620  lse.        def 
+0000bae0: 6173 6b49 6e74 656e 7453 6372 6565 6e69  askIntentScreeni
+0000baf0: 6e67 2829 202d 3e20 626f 6f6c 3a0a 2020  ng() -> bool:.  
+0000bb00: 2020 2020 2020 2020 2020 6f70 7469 6f6e            option
+0000bb10: 7320 3d20 2822 7965 7322 2c20 226e 6f22  s = ("yes", "no"
+0000bb20: 290a 2020 2020 2020 2020 2020 2020 7175  ).            qu
+0000bb30: 6573 7469 6f6e 203d 2022 446f 2079 6f75  estion = "Do you
+0000bb40: 2077 616e 7420 746f 2063 6865 636b 2065   want to check e
+0000bb50: 6163 6820 7265 7175 6573 7420 746f 2073  ach request to s
+0000bb60: 6565 2069 6620 6120 746f 6f6c 2069 7320  ee if a tool is 
+0000bb70: 7265 7175 6972 6564 3f22 0a20 2020 2020  required?".     
+0000bb80: 2020 2020 2020 2070 7269 6e74 3128 7175         print1(qu
+0000bb90: 6573 7469 6f6e 290a 2020 2020 2020 2020  estion).        
+0000bba0: 2020 2020 696e 7465 6e74 5f73 6372 6565      intent_scree
+0000bbb0: 6e69 6e67 203d 2073 656c 662e 6469 616c  ning = self.dial
+0000bbc0: 6f67 732e 6765 7456 616c 6964 4f70 7469  ogs.getValidOpti
+0000bbd0: 6f6e 7328 0a20 2020 2020 2020 2020 2020  ons(.           
+0000bbe0: 2020 2020 206f 7074 696f 6e73 3d6f 7074       options=opt
+0000bbf0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
+0000bc00: 2020 2020 2020 7469 746c 653d 2249 6e74        title="Int
+0000bc10: 656e 7420 5363 7265 656e 696e 6722 2c0a  ent Screening",.
+0000bc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc30: 6465 6661 756c 743d 2279 6573 2220 6966  default="yes" if
+0000bc40: 2063 6f6e 6669 672e 696e 7465 6e74 5f73   config.intent_s
+0000bc50: 6372 6565 6e69 6e67 2065 6c73 6520 226e  creening else "n
+0000bc60: 6f22 2c0a 2020 2020 2020 2020 2020 2020  o",.            
+0000bc70: 2020 2020 7465 7874 3d71 7565 7374 696f      text=questio
+0000bc80: 6e2c 0a20 2020 2020 2020 2020 2020 2029  n,.            )
+0000bc90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bca0: 696e 7465 6e74 5f73 6372 6565 6e69 6e67  intent_screening
+0000bcb0: 2061 6e64 2069 6e74 656e 745f 7363 7265   and intent_scre
+0000bcc0: 656e 696e 6720 3d3d 2022 7965 7322 3a0a  ening == "yes":.
+0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bce0: 636f 6e66 6967 2e69 6e74 656e 745f 7363  config.intent_sc
+0000bcf0: 7265 656e 696e 6720 3d20 5472 7565 0a20  reening = True. 
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000bd10: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+0000bd20: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0000bd30: 6c73 650a 0a20 2020 2020 2020 2063 7572  lse..        cur
+0000bd40: 7265 6e74 4c6c 6d49 6e74 6572 6661 6365  rentLlmInterface
+0000bd50: 203d 2063 6f6e 6669 672e 6c6c 6d49 6e74   = config.llmInt
+0000bd60: 6572 6661 6365 0a20 2020 2020 2020 2073  erface.        s
+0000bd70: 656c 662e 7365 6c65 6374 4c6c 6d50 6c61  elf.selectLlmPla
+0000bd80: 7466 6f72 6d28 290a 0a20 2020 2020 2020  tform()..       
+0000bd90: 2070 7269 6e74 3128 2253 656c 6563 7420   print1("Select 
+0000bda0: 6d6f 6465 6c73 202e 2e2e 2229 0a20 2020  models ...").   
+0000bdb0: 2020 2020 2069 6620 636f 6e66 6967 2e6c       if config.l
+0000bdc0: 6c6d 496e 7465 7266 6163 6520 3d3d 2022  lmInterface == "
+0000bdd0: 6f6c 6c61 6d61 223a 0a20 2020 2020 2020  ollama":.       
+0000bde0: 2020 2020 2070 7269 6e74 3228 2223 204d       print2("# M
+0000bdf0: 6169 6e20 4d6f 6465 6c20 2d20 666f 7220  ain Model - for 
+0000be00: 626f 7468 2074 6173 6b20 6578 6563 7574  both task execut
+0000be10: 696f 6e20 616e 6420 636f 6e76 6572 7361  ion and conversa
+0000be20: 7469 6f6e 2229 0a20 2020 2020 2020 2020  tion").         
+0000be30: 2020 2073 656c 662e 7365 744c 6c6d 4d6f     self.setLlmMo
+0000be40: 6465 6c5f 6f6c 6c61 6d61 2829 0a20 2020  del_ollama().   
+0000be50: 2020 2020 2020 2020 2061 736b 496e 7465           askInte
+0000be60: 6e74 5363 7265 656e 696e 6728 290a 2020  ntScreening().  
+0000be70: 2020 2020 2020 2020 2020 6966 2061 736b            if ask
+0000be80: 4164 6469 7469 6f6e 616c 4368 6174 4d6f  AdditionalChatMo
+0000be90: 6465 6c28 293a 0a20 2020 2020 2020 2020  del():.         
+0000bea0: 2020 2020 2020 2070 7269 6e74 3228 2223         print2("#
+0000beb0: 2043 6861 7420 4d6f 6465 6c20 2d20 666f   Chat Model - fo
+0000bec0: 7220 636f 6e76 6572 7361 7469 6f6e 206f  r conversation o
+0000bed0: 6e6c 7922 290a 2020 2020 2020 2020 2020  nly").          
+0000bee0: 2020 2020 2020 7365 6c66 2e73 6574 4c6c        self.setLl
+0000bef0: 6d4d 6f64 656c 5f6f 6c6c 616d 6128 2263  mModel_ollama("c
+0000bf00: 6f64 6522 290a 2020 2020 2020 2020 656c  ode").        el
+0000bf10: 6966 2063 6f6e 6669 672e 6c6c 6d49 6e74  if config.llmInt
+0000bf20: 6572 6661 6365 203d 3d20 226c 6c61 6d61  erface == "llama
+0000bf30: 6370 7022 3a0a 2020 2020 2020 2020 2020  cpp":.          
+0000bf40: 2020 7072 696e 7432 2822 2320 4d61 696e    print2("# Main
+0000bf50: 204d 6f64 656c 202d 2066 6f72 2062 6f74   Model - for bot
+0000bf60: 6820 7461 736b 2065 7865 6375 7469 6f6e  h task execution
+0000bf70: 2061 6e64 2063 6f6e 7665 7273 6174 696f   and conversatio
+0000bf80: 6e22 290a 2020 2020 2020 2020 2020 2020  n").            
+0000bf90: 7365 6c66 2e73 6574 4c6c 6d4d 6f64 656c  self.setLlmModel
+0000bfa0: 5f6c 6c61 6d61 6370 7028 290a 2020 2020  _llamacpp().    
+0000bfb0: 2020 2020 2020 2020 6173 6b49 6e74 656e          askInten
+0000bfc0: 7453 6372 6565 6e69 6e67 2829 0a20 2020  tScreening().   
+0000bfd0: 2020 2020 2020 2020 2069 6620 6173 6b41           if askA
+0000bfe0: 6464 6974 696f 6e61 6c43 6861 744d 6f64  dditionalChatMod
+0000bff0: 656c 2829 3a0a 2020 2020 2020 2020 2020  el():.          
+0000c000: 2020 2020 2020 7072 696e 7432 2822 2320        print2("# 
+0000c010: 4368 6174 204d 6f64 656c 202d 2066 6f72  Chat Model - for
+0000c020: 2063 6f6e 7665 7273 6174 696f 6e20 6f6e   conversation on
+0000c030: 6c79 2229 0a20 2020 2020 2020 2020 2020  ly").           
+0000c040: 2020 2020 2073 656c 662e 7365 744c 6c6d       self.setLlm
+0000c050: 4d6f 6465 6c5f 6c6c 616d 6163 7070 2822  Model_llamacpp("
+0000c060: 636f 6465 2229 0a20 2020 2020 2020 2065  code").        e
+0000c070: 6c69 6620 636f 6e66 6967 2e6c 6c6d 496e  lif config.llmIn
+0000c080: 7465 7266 6163 6520 3d3d 2022 6765 6d69  terface == "gemi
+0000c090: 6e69 223a 0a20 2020 2020 2020 2020 2020  ni":.           
+0000c0a0: 2070 7269 6e74 3328 224d 6f64 656c 2073   print3("Model s
+0000c0b0: 656c 6563 7465 643a 2047 6f6f 676c 6520  elected: Google 
+0000c0c0: 4765 6d69 6e69 2050 726f 2229 0a20 2020  Gemini Pro").   
+0000c0d0: 2020 2020 2020 2020 2061 736b 496e 7465           askInte
+0000c0e0: 6e74 5363 7265 656e 696e 6728 290a 2020  ntScreening().  
+0000c0f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000c100: 2020 2020 2020 2020 6966 2063 6f6e 6669          if confi
+0000c110: 672e 6c6c 6d49 6e74 6572 6661 6365 203d  g.llmInterface =
+0000c120: 3d20 2263 6861 7467 7074 223a 0a20 2020  = "chatgpt":.   
+0000c130: 2020 2020 2020 2020 2020 2020 2023 2069               # i
+0000c140: 6e74 656e 7420 7363 7265 656e 696e 6720  ntent screening 
+0000c150: 646f 6573 206e 6f74 2061 7070 6c79 2074  does not apply t
+0000c160: 6f20 6c65 746d 6564 6f69 7420 6d6f 6465  o letmedoit mode
+0000c170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c180: 2061 736b 496e 7465 6e74 5363 7265 656e   askIntentScreen
+0000c190: 696e 6728 290a 2020 2020 2020 2020 2020  ing().          
+0000c1a0: 2020 7365 6c66 2e73 6574 4c6c 6d4d 6f64    self.setLlmMod
+0000c1b0: 656c 5f63 6861 7467 7074 2829 0a20 2020  el_chatgpt().   
+0000c1c0: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
+0000c1d0: 436f 6e66 6967 2829 0a20 2020 2020 2020  Config().       
+0000c1e0: 2069 6620 6e6f 7420 636f 6e66 6967 2e6c   if not config.l
+0000c1f0: 6c6d 496e 7465 7266 6163 6520 3d3d 2063  lmInterface == c
+0000c200: 7572 7265 6e74 4c6c 6d49 6e74 6572 6661  urrentLlmInterfa
+0000c210: 6365 3a0a 2020 2020 2020 2020 2020 2020  ce:.            
+0000c220: 7072 696e 7432 2822 4c4c 4d20 496e 7465  print2("LLM Inte
+0000c230: 7266 6163 6520 6368 616e 6765 6421 2053  rface changed! S
+0000c240: 7461 7274 696e 6720 6120 6e65 7720 6368  tarting a new ch
+0000c250: 6174 2073 6573 7369 6f6e 202e 2e2e 2229  at session ...")
+0000c260: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+0000c270: 6669 672e 6465 6661 756c 7445 6e74 7279  fig.defaultEntry
+0000c280: 203d 2022 2e6e 6577 220a 2020 2020 2020   = ".new".      
+0000c290: 2020 2020 2020 636f 6e66 6967 2e61 6363        config.acc
+0000c2a0: 6570 745f 6465 6661 756c 7420 3d20 5472  ept_default = Tr
+0000c2b0: 7565 0a0a 2020 2020 6465 6620 7365 6c65  ue..    def sele
+0000c2c0: 6374 4f6c 6c61 6d61 4d6f 6465 6c28 7365  ctOllamaModel(se
+0000c2d0: 6c66 2c20 6d65 7373 6167 653d 2253 656c  lf, message="Sel
+0000c2e0: 6563 7420 6120 6d6f 6465 6c20 6672 6f6d  ect a model from
+0000c2f0: 204f 6c6c 616d 6120 4c69 6272 6172 793a   Ollama Library:
+0000c300: 222c 2066 6561 7475 7265 3d22 6465 6661  ", feature="defa
+0000c310: 756c 7422 2920 2d3e 2073 7472 3a0a 2020  ult") -> str:.  
+0000c320: 2020 2020 2020 2320 6869 7374 6f72 7920        # history 
+0000c330: 7365 7373 696f 6e0a 2020 2020 2020 2020  session.        
+0000c340: 6869 7374 6f72 7946 6f6c 6465 7220 3d20  historyFolder = 
+0000c350: 6f73 2e70 6174 682e 6a6f 696e 2863 6f6e  os.path.join(con
+0000c360: 6669 672e 6c6f 6361 6c53 746f 7261 6765  fig.localStorage
+0000c370: 2c20 2268 6973 746f 7279 2229 0a20 2020  , "history").   
+0000c380: 2020 2020 2050 6174 6828 6869 7374 6f72       Path(histor
+0000c390: 7946 6f6c 6465 7229 2e6d 6b64 6972 2870  yFolder).mkdir(p
+0000c3a0: 6172 656e 7473 3d54 7275 652c 2065 7869  arents=True, exi
+0000c3b0: 7374 5f6f 6b3d 5472 7565 290a 2020 2020  st_ok=True).    
+0000c3c0: 2020 2020 6d6f 6465 6c5f 6869 7374 6f72      model_histor
+0000c3d0: 7920 3d20 6f73 2e70 6174 682e 6a6f 696e  y = os.path.join
+0000c3e0: 2868 6973 746f 7279 466f 6c64 6572 2c20  (historyFolder, 
+0000c3f0: 226f 6c6c 616d 615f 636f 6465 2220 6966  "ollama_code" if
+0000c400: 2066 6561 7475 7265 203d 3d20 2263 6f64   feature == "cod
+0000c410: 6522 2065 6c73 6520 226f 6c6c 616d 615f  e" else "ollama_
+0000c420: 6465 6661 756c 7422 290a 2020 2020 2020  default").      
+0000c430: 2020 6d6f 6465 6c5f 7365 7373 696f 6e20    model_session 
+0000c440: 3d20 5072 6f6d 7074 5365 7373 696f 6e28  = PromptSession(
+0000c450: 6869 7374 6f72 793d 4669 6c65 4869 7374  history=FileHist
+0000c460: 6f72 7928 6d6f 6465 6c5f 6869 7374 6f72  ory(model_histor
+0000c470: 7929 290a 2020 2020 2020 2020 636f 6d70  y)).        comp
+0000c480: 6c65 7465 7220 3d20 4675 7a7a 7943 6f6d  leter = FuzzyCom
+0000c490: 706c 6574 6572 2857 6f72 6443 6f6d 706c  pleter(WordCompl
+0000c4a0: 6574 6572 2873 6f72 7465 6428 6f6c 6c61  eter(sorted(olla
+0000c4b0: 6d61 5f6d 6f64 656c 7329 2c20 6967 6e6f  ma_models), igno
+0000c4c0: 7265 5f63 6173 653d 5472 7565 2929 0a20  re_case=True)). 
+0000c4d0: 2020 2020 2020 2062 6f74 746f 6d5f 746f         bottom_to
+0000c4e0: 6f6c 6261 7220 3d20 6622 2222 207b 7374  olbar = f""" {st
+0000c4f0: 7228 636f 6e66 6967 2e68 6f74 6b65 795f  r(config.hotkey_
+0000c500: 6578 6974 292e 7265 706c 6163 6528 2227  exit).replace("'
+0000c510: 222c 2022 2229 7d20 7b63 6f6e 6669 672e  ", "")} {config.
+0000c520: 6578 6974 5f65 6e74 7279 7d22 2222 0a20  exit_entry}""". 
+0000c530: 2020 2020 2020 2064 6566 6175 6c74 203d         default =
+0000c540: 2063 6f6e 6669 672e 6f6c 6c61 6d61 4368   config.ollamaCh
+0000c550: 6174 4d6f 6465 6c20 6966 2066 6561 7475  atModel if featu
+0000c560: 7265 203d 3d20 2263 6f64 6522 2065 6c73  re == "code" els
+0000c570: 6520 636f 6e66 6967 2e6f 6c6c 616d 614d  e config.ollamaM
+0000c580: 6169 6e4d 6f64 656c 0a20 2020 2020 2020  ainModel.       
+0000c590: 2069 6620 636f 6e66 6967 2e6c 6c6d 496e   if config.llmIn
+0000c5a0: 7465 7266 6163 6520 3d3d 2022 6c6c 616d  terface == "llam
+0000c5b0: 6163 7070 223a 0a20 2020 2020 2020 2020  acpp":.         
+0000c5c0: 2020 2069 6620 6665 6174 7572 6520 3d3d     if feature ==
+0000c5d0: 2022 6465 6661 756c 7422 2061 6e64 2063   "default" and c
+0000c5e0: 6f6e 6669 672e 6c6c 616d 6163 7070 4d61  onfig.llamacppMa
+0000c5f0: 696e 4d6f 6465 6c5f 6f6c 6c61 6d61 5f74  inModel_ollama_t
+0000c600: 6167 3a0a 2020 2020 2020 2020 2020 2020  ag:.            
+0000c610: 2020 2020 6465 6661 756c 7420 3d20 636f      default = co
+0000c620: 6e66 6967 2e6c 6c61 6d61 6370 704d 6169  nfig.llamacppMai
+0000c630: 6e4d 6f64 656c 5f6f 6c6c 616d 615f 7461  nModel_ollama_ta
+0000c640: 670a 2020 2020 2020 2020 2020 2020 656c  g.            el
+0000c650: 6966 2066 6561 7475 7265 203d 3d20 2263  if feature == "c
+0000c660: 6f64 6522 2061 6e64 2063 6f6e 6669 672e  ode" and config.
+0000c670: 6c6c 616d 6163 7070 4368 6174 4d6f 6465  llamacppChatMode
+0000c680: 6c5f 6f6c 6c61 6d61 5f74 6167 3a0a 2020  l_ollama_tag:.  
+0000c690: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000c6a0: 6661 756c 7420 3d20 636f 6e66 6967 2e6c  fault = config.l
+0000c6b0: 6c61 6d61 6370 7043 6861 744d 6f64 656c  lamacppChatModel
+0000c6c0: 5f6f 6c6c 616d 615f 7461 670a 2020 2020  _ollama_tag.    
+0000c6d0: 2020 2020 2320 7072 6f6d 7074 0a20 2020      # prompt.   
+0000c6e0: 2020 2020 2070 7269 6e74 3128 6d65 7373       print1(mess
+0000c6f0: 6167 6529 0a20 2020 2020 2020 2070 7269  age).        pri
+0000c700: 6e74 3128 2228 466f 7220 6465 7461 696c  nt1("(For detail
+0000c710: 732c 2076 6973 6974 2068 7474 7073 3a2f  s, visit https:/
+0000c720: 2f6f 6c6c 616d 612e 636f 6d2f 6c69 6272  /ollama.com/libr
+0000c730: 6172 7929 2229 0a20 2020 2020 2020 206d  ary)").        m
+0000c740: 6f64 656c 203d 2073 656c 662e 7072 6f6d  odel = self.prom
+0000c750: 7074 732e 7369 6d70 6c65 5072 6f6d 7074  pts.simplePrompt
+0000c760: 2873 7479 6c65 3d73 656c 662e 7072 6f6d  (style=self.prom
+0000c770: 7074 732e 7072 6f6d 7074 5374 796c 6532  pts.promptStyle2
+0000c780: 2c20 7072 6f6d 7074 5365 7373 696f 6e3d  , promptSession=
+0000c790: 6d6f 6465 6c5f 7365 7373 696f 6e2c 2062  model_session, b
+0000c7a0: 6f74 746f 6d5f 746f 6f6c 6261 723d 626f  ottom_toolbar=bo
+0000c7b0: 7474 6f6d 5f74 6f6f 6c62 6172 2c20 6465  ttom_toolbar, de
+0000c7c0: 6661 756c 743d 6465 6661 756c 742c 2063  fault=default, c
+0000c7d0: 6f6d 706c 6574 6572 3d63 6f6d 706c 6574  ompleter=complet
+0000c7e0: 6572 290a 2020 2020 2020 2020 6966 206d  er).        if m
+0000c7f0: 6f64 656c 2061 6e64 206e 6f74 206d 6f64  odel and not mod
+0000c800: 656c 2e6c 6f77 6572 2829 203d 3d20 636f  el.lower() == co
+0000c810: 6e66 6967 2e65 7869 745f 656e 7472 793a  nfig.exit_entry:
+0000c820: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000c830: 7572 6e20 6d6f 6465 6c0a 2020 2020 2020  urn model.      
+0000c840: 2020 7265 7475 726e 2022 220a 0a20 2020    return ""..   
+0000c850: 2064 6566 2073 6574 4c6c 6d4d 6f64 656c   def setLlmModel
+0000c860: 5f6f 6c6c 616d 6128 7365 6c66 2c20 6665  _ollama(self, fe
+0000c870: 6174 7572 653d 2264 6566 6175 6c74 2229  ature="default")
+0000c880: 3a0a 2020 2020 2020 2020 6d6f 6465 6c20  :.        model 
+0000c890: 3d20 7365 6c66 2e73 656c 6563 744f 6c6c  = self.selectOll
+0000c8a0: 616d 614d 6f64 656c 2866 6561 7475 7265  amaModel(feature
+0000c8b0: 3d66 6561 7475 7265 290a 2020 2020 2020  =feature).      
+0000c8c0: 2020 6966 206d 6f64 656c 3a0a 2020 2020    if model:.    
+0000c8d0: 2020 2020 2020 2020 646f 776e 6c6f 6164          download
+0000c8e0: 6564 4f6c 6c61 6d61 4d6f 6465 6c73 203d  edOllamaModels =
+0000c8f0: 2067 6574 446f 776e 6c6f 6164 6564 4f6c   getDownloadedOl
+0000c900: 6c61 6d61 4d6f 6465 6c73 2829 0a20 2020  lamaModels().   
+0000c910: 2020 2020 2020 2020 2069 6620 6d6f 6465           if mode
+0000c920: 6c20 696e 2064 6f77 6e6c 6f61 6465 644f  l in downloadedO
+0000c930: 6c6c 616d 614d 6f64 656c 733a 0a20 2020  llamaModels:.   
+0000c940: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000c950: 6665 6174 7572 6520 3d3d 2022 6465 6661  feature == "defa
+0000c960: 756c 7422 3a0a 2020 2020 2020 2020 2020  ult":.          
+0000c970: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0000c980: 2e6f 6c6c 616d 614d 6169 6e4d 6f64 656c  .ollamaMainModel
+0000c990: 203d 206d 6f64 656c 0a20 2020 2020 2020   = model.       
+0000c9a0: 2020 2020 2020 2020 2065 6c69 6620 6665           elif fe
+0000c9b0: 6174 7572 6520 3d3d 2022 636f 6465 223a  ature == "code":
+0000c9c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c9d0: 2020 2020 2063 6f6e 6669 672e 6f6c 6c61       config.olla
+0000c9e0: 6d61 4368 6174 4d6f 6465 6c20 3d20 6d6f  maChatModel = mo
+0000c9f0: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
+0000ca00: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000ca10: 2020 2020 2020 6966 2073 6875 7469 6c2e        if shutil.
+0000ca20: 7768 6963 6828 226f 6c6c 616d 6122 293a  which("ollama"):
+0000ca30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ca40: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000ca50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ca60: 2020 446f 776e 6c6f 6164 6572 2e64 6f77    Downloader.dow
+0000ca70: 6e6c 6f61 644f 6c6c 616d 614d 6f64 656c  nloadOllamaModel
+0000ca80: 286d 6f64 656c 2c20 5472 7565 290a 2020  (model, True).  
+0000ca90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000caa0: 2020 2020 2020 6966 2066 6561 7475 7265        if feature
+0000cab0: 203d 3d20 2264 6566 6175 6c74 223a 0a20   == "default":. 
+0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cad0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+0000cae0: 672e 6f6c 6c61 6d61 4d61 696e 4d6f 6465  g.ollamaMainMode
+0000caf0: 6c20 3d20 6d6f 6465 6c0a 2020 2020 2020  l = model.      
+0000cb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb10: 2020 656c 6966 2066 6561 7475 7265 203d    elif feature =
+0000cb20: 3d20 2263 6f64 6522 3a0a 2020 2020 2020  = "code":.      
+0000cb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cb40: 2020 2020 2020 636f 6e66 6967 2e6f 6c6c        config.oll
+0000cb50: 616d 6143 6861 744d 6f64 656c 203d 206d  amaChatModel = m
+0000cb60: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
+0000cb70: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+0000cb80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cb90: 2020 2020 2020 2020 2070 7269 6e74 3228           print2(
+0000cba0: 6622 4661 696c 6564 2074 6f20 646f 776e  f"Failed to down
+0000cbb0: 6c6f 6164 2027 7b6d 6f64 656c 7d27 2120  load '{model}'! 
+0000cbc0: 506c 6561 7365 206d 616b 6520 7375 7265  Please make sure
+0000cbd0: 2079 6f75 2065 6e74 6572 2061 2076 616c   you enter a val
+0000cbe0: 6964 206d 6f64 656c 206e 616d 6520 6f72  id model name or
+0000cbf0: 2074 6167 2e22 290a 2020 2020 2020 2020   tag.").        
+0000cc00: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc20: 2020 2020 2063 6f6e 6669 672e 6c6c 616d       config.llam
-0000cc30: 6163 7070 4d61 696e 4d6f 6465 6c5f 6d6f  acppMainModel_mo
-0000cc40: 6465 6c5f 7061 7468 203d 2064 6f77 6e6c  del_path = downl
-0000cc50: 6f61 6465 644f 6c6c 616d 614d 6f64 656c  oadedOllamaModel
-0000cc60: 735b 6d6f 6465 6c5d 0a20 2020 2020 2020  s[model].       
+0000cc20: 2020 7072 696e 7428 224f 6c6c 616d 6120    print("Ollama 
+0000cc30: 6e6f 7420 666f 756e 6421 2049 6e73 7461  not found! Insta
+0000cc40: 6c6c 204f 6c6c 616d 6120 6669 7273 7420  ll Ollama first 
+0000cc50: 746f 2075 7365 204f 6c6c 616d 6120 6d6f  to use Ollama mo
+0000cc60: 6465 6c20 6c69 6272 6172 7921 2229 0a20  del library!"). 
 0000cc70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc80: 2065 6c69 6620 6665 6174 7572 6520 3d3d   elif feature ==
-0000cc90: 2022 636f 6465 223a 0a20 2020 2020 2020   "code":.       
-0000cca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ccb0: 2020 2020 2063 6f6e 6669 672e 6c6c 616d       config.llam
-0000ccc0: 6163 7070 4368 6174 4d6f 6465 6c5f 6d6f  acppChatModel_mo
-0000ccd0: 6465 6c5f 7061 7468 203d 2064 6f77 6e6c  del_path = downl
-0000cce0: 6f61 6465 644f 6c6c 616d 614d 6f64 656c  oadedOllamaModel
-0000ccf0: 735b 6d6f 6465 6c5d 0a20 2020 2020 2020  s[model].       
-0000cd00: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000cd10: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000cd20: 2020 2020 2020 2020 2020 2069 6620 7368             if sh
-0000cd30: 7574 696c 2e77 6869 6368 2822 6f6c 6c61  util.which("olla
-0000cd40: 6d61 2229 3a0a 2020 2020 2020 2020 2020  ma"):.          
-0000cd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd60: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-0000cd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd80: 2020 2020 2020 2044 6f77 6e6c 6f61 6465         Downloade
-0000cd90: 722e 646f 776e 6c6f 6164 4f6c 6c61 6d61  r.downloadOllama
-0000cda0: 4d6f 6465 6c28 6d6f 6465 6c2c 2054 7275  Model(model, Tru
-0000cdb0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdd0: 2020 2023 2072 6566 7265 7368 2064 6f77     # refresh dow
-0000cde0: 6e6c 6f61 6420 6c69 7374 0a20 2020 2020  nload list.     
-0000cdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce00: 2020 2020 2020 2020 2020 2064 6f77 6e6c             downl
-0000ce10: 6f61 6465 644f 6c6c 616d 614d 6f64 656c  oadedOllamaModel
-0000ce20: 7320 3d20 6765 7444 6f77 6e6c 6f61 6465  s = getDownloade
-0000ce30: 644f 6c6c 616d 614d 6f64 656c 7328 290a  dOllamaModels().
-0000ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce60: 6966 2066 6561 7475 7265 203d 3d20 2264  if feature == "d
-0000ce70: 6566 6175 6c74 223a 0a20 2020 2020 2020  efault":.       
-0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce90: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000cea0: 6669 672e 6c6c 616d 6163 7070 4d61 696e  fig.llamacppMain
-0000ceb0: 4d6f 6465 6c5f 6d6f 6465 6c5f 7061 7468  Model_model_path
-0000cec0: 203d 2064 6f77 6e6c 6f61 6465 644f 6c6c   = downloadedOll
-0000ced0: 616d 614d 6f64 656c 735b 6d6f 6465 6c5d  amaModels[model]
-0000cee0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf00: 2065 6c69 6620 6665 6174 7572 6520 3d3d   elif feature ==
-0000cf10: 2022 636f 6465 223a 0a20 2020 2020 2020   "code":.       
-0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf30: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000cf40: 6669 672e 6c6c 616d 6163 7070 4368 6174  fig.llamacppChat
-0000cf50: 4d6f 6465 6c5f 6d6f 6465 6c5f 7061 7468  Model_model_path
-0000cf60: 203d 2064 6f77 6e6c 6f61 6465 644f 6c6c   = downloadedOll
-0000cf70: 616d 614d 6f64 656c 735b 6d6f 6465 6c5d  amaModels[model]
-0000cf80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cf90: 2020 2020 2020 2020 2020 2020 2065 7863               exc
-0000cfa0: 6570 743a 0a20 2020 2020 2020 2020 2020  ept:.           
-0000cfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfc0: 2020 2020 2070 7269 6e74 3228 6622 4661       print2(f"Fa
-0000cfd0: 696c 6564 2074 6f20 646f 776e 6c6f 6164  iled to download
-0000cfe0: 2027 7b6d 6f64 656c 7d27 2120 506c 6561   '{model}'! Plea
-0000cff0: 7365 206d 616b 6520 7375 7265 2079 6f75  se make sure you
-0000d000: 2065 6e74 6572 2061 2076 616c 6964 206d   enter a valid m
-0000d010: 6f64 656c 206e 616d 6520 6f72 2074 6167  odel name or tag
-0000d020: 2e22 290a 2020 2020 2020 2020 2020 2020  .").            
-0000d030: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000d040: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d050: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000d060: 696e 7428 224f 6c6c 616d 6120 6e6f 7420  int("Ollama not 
-0000d070: 666f 756e 6421 2049 6e73 7461 6c6c 204f  found! Install O
-0000d080: 6c6c 616d 6120 6669 7273 7420 746f 2075  llama first to u
-0000d090: 7365 204f 6c6c 616d 6120 6d6f 6465 6c20  se Ollama model 
-0000d0a0: 6c69 6272 6172 7921 2229 0a20 2020 2020  library!").     
-0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0c0: 2020 2020 2020 2070 7269 6e74 2822 546f         print("To
-0000d0d0: 2069 6e73 7461 6c6c 204f 6c6c 616d 612c   install Ollama,
-0000d0e0: 2076 6973 6974 2068 7474 7073 3a2f 2f6f   visit https://o
-0000d0f0: 6c6c 616d 612e 636f 6d22 290a 2020 2020  llama.com").    
-0000d100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d110: 6966 2066 6561 7475 7265 203d 3d20 2264  if feature == "d
-0000d120: 6566 6175 6c74 223a 0a20 2020 2020 2020  efault":.       
-0000d130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d140: 2063 6f6e 6669 672e 6c6c 616d 6163 7070   config.llamacpp
-0000d150: 4d61 696e 4d6f 6465 6c5f 6f6c 6c61 6d61  MainModel_ollama
-0000d160: 5f74 6167 203d 206d 6f64 656c 0a20 2020  _tag = model.   
-0000d170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d180: 2065 6c69 6620 6665 6174 7572 6520 3d3d   elif feature ==
-0000d190: 2022 636f 6465 223a 0a20 2020 2020 2020   "code":.       
+0000cc80: 2020 2070 7269 6e74 2822 546f 2069 6e73     print("To ins
+0000cc90: 7461 6c6c 204f 6c6c 616d 612c 2076 6973  tall Ollama, vis
+0000cca0: 6974 2068 7474 7073 3a2f 2f6f 6c6c 616d  it https://ollam
+0000ccb0: 612e 636f 6d22 290a 0a20 2020 2064 6566  a.com")..    def
+0000ccc0: 2073 6574 4c6c 6d4d 6f64 656c 5f6c 6c61   setLlmModel_lla
+0000ccd0: 6d61 6370 7028 7365 6c66 2c20 6665 6174  macpp(self, feat
+0000cce0: 7572 653d 2264 6566 6175 6c74 2229 3a0a  ure="default"):.
+0000ccf0: 2020 2020 2020 2020 6c69 6272 6172 7920          library 
+0000cd00: 3d20 7365 6c66 2e64 6961 6c6f 6773 2e67  = self.dialogs.g
+0000cd10: 6574 5661 6c69 644f 7074 696f 6e73 280a  etValidOptions(.
+0000cd20: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+0000cd30: 6f6e 733d 2822 4f6c 6c61 6d61 204c 6962  ons=("Ollama Lib
+0000cd40: 7261 7279 222c 2022 4875 6767 696e 6766  rary", "Huggingf
+0000cd50: 6163 6520 4875 6222 2c20 2243 7573 746f  ace Hub", "Custo
+0000cd60: 6d20 4747 5546 2229 2c0a 2020 2020 2020  m GGUF"),.      
+0000cd70: 2020 2020 2020 7469 746c 653d 224d 6f64        title="Mod
+0000cd80: 656c 204c 6962 7261 7279 222c 0a20 2020  el Library",.   
+0000cd90: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+0000cda0: 3d22 4f6c 6c61 6d61 204c 6962 7261 7279  ="Ollama Library
+0000cdb0: 2220 6966 2073 6875 7469 6c2e 7768 6963  " if shutil.whic
+0000cdc0: 6828 226f 6c6c 616d 6122 2920 656c 7365  h("ollama") else
+0000cdd0: 2022 4875 6767 696e 6766 6163 6520 4875   "Huggingface Hu
+0000cde0: 6222 2c0a 2020 2020 2020 2020 2020 2020  b",.            
+0000cdf0: 7465 7874 3d22 5365 6c65 6374 2061 206d  text="Select a m
+0000ce00: 6f64 656c 206c 6962 7261 7279 3a22 2c0a  odel library:",.
+0000ce10: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000ce20: 2020 6966 206c 6962 7261 7279 3a0a 2020    if library:.  
+0000ce30: 2020 2020 2020 2020 2020 6966 206c 6962            if lib
+0000ce40: 7261 7279 203d 3d20 224f 6c6c 616d 6120  rary == "Ollama 
+0000ce50: 4c69 6272 6172 7922 3a0a 2020 2020 2020  Library":.      
+0000ce60: 2020 2020 2020 2020 2020 6d6f 6465 6c20            model 
+0000ce70: 3d20 7365 6c66 2e73 656c 6563 744f 6c6c  = self.selectOll
+0000ce80: 616d 614d 6f64 656c 2866 6561 7475 7265  amaModel(feature
+0000ce90: 3d66 6561 7475 7265 290a 2020 2020 2020  =feature).      
+0000cea0: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
+0000ceb0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+0000cec0: 2020 2020 2020 2020 646f 776e 6c6f 6164          download
+0000ced0: 6564 4f6c 6c61 6d61 4d6f 6465 6c73 203d  edOllamaModels =
+0000cee0: 2067 6574 446f 776e 6c6f 6164 6564 4f6c   getDownloadedOl
+0000cef0: 6c61 6d61 4d6f 6465 6c73 2829 0a20 2020  lamaModels().   
+0000cf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf10: 2069 6620 6d6f 6465 6c20 696e 2064 6f77   if model in dow
+0000cf20: 6e6c 6f61 6465 644f 6c6c 616d 614d 6f64  nloadedOllamaMod
+0000cf30: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+0000cf40: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000cf50: 6665 6174 7572 6520 3d3d 2022 6465 6661  feature == "defa
+0000cf60: 756c 7422 3a0a 2020 2020 2020 2020 2020  ult":.          
+0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf80: 2020 636f 6e66 6967 2e6c 6c61 6d61 6370    config.llamacp
+0000cf90: 704d 6169 6e4d 6f64 656c 5f6d 6f64 656c  pMainModel_model
+0000cfa0: 5f70 6174 6820 3d20 646f 776e 6c6f 6164  _path = download
+0000cfb0: 6564 4f6c 6c61 6d61 4d6f 6465 6c73 5b6d  edOllamaModels[m
+0000cfc0: 6f64 656c 5d0a 2020 2020 2020 2020 2020  odel].          
+0000cfd0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000cfe0: 6966 2066 6561 7475 7265 203d 3d20 2263  if feature == "c
+0000cff0: 6f64 6522 3a0a 2020 2020 2020 2020 2020  ode":.          
+0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d010: 2020 636f 6e66 6967 2e6c 6c61 6d61 6370    config.llamacp
+0000d020: 7043 6861 744d 6f64 656c 5f6d 6f64 656c  pChatModel_model
+0000d030: 5f70 6174 6820 3d20 646f 776e 6c6f 6164  _path = download
+0000d040: 6564 4f6c 6c61 6d61 4d6f 6465 6c73 5b6d  edOllamaModels[m
+0000d050: 6f64 656c 5d0a 2020 2020 2020 2020 2020  odel].          
+0000d060: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 2020 2020 2020 2020 6966 2073 6875 7469          if shuti
+0000d090: 6c2e 7768 6963 6828 226f 6c6c 616d 6122  l.which("ollama"
+0000d0a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000d0b0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000d0c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0e0: 2020 2020 446f 776e 6c6f 6164 6572 2e64      Downloader.d
+0000d0f0: 6f77 6e6c 6f61 644f 6c6c 616d 614d 6f64  ownloadOllamaMod
+0000d100: 656c 286d 6f64 656c 2c20 5472 7565 290a  el(model, True).
+0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d130: 2320 7265 6672 6573 6820 646f 776e 6c6f  # refresh downlo
+0000d140: 6164 206c 6973 740a 2020 2020 2020 2020  ad list.        
+0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d160: 2020 2020 2020 2020 646f 776e 6c6f 6164          download
+0000d170: 6564 4f6c 6c61 6d61 4d6f 6465 6c73 203d  edOllamaModels =
+0000d180: 2067 6574 446f 776e 6c6f 6164 6564 4f6c   getDownloadedOl
+0000d190: 6c61 6d61 4d6f 6465 6c73 2829 0a20 2020  lamaModels().   
 0000d1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d1b0: 2063 6f6e 6669 672e 6c6c 616d 6163 7070   config.llamacpp
-0000d1c0: 4368 6174 4d6f 6465 6c5f 6f6c 6c61 6d61  ChatModel_ollama
-0000d1d0: 5f74 6167 203d 206d 6f64 656c 0a20 2020  _tag = model.   
-0000d1e0: 2020 2020 2020 2020 2065 6c69 6620 6c69           elif li
-0000d1f0: 6272 6172 7920 3d3d 2022 4875 6767 696e  brary == "Huggin
-0000d200: 6766 6163 6520 4875 6222 3a0a 2020 2020  gface Hub":.    
-0000d210: 2020 2020 2020 2020 2020 2020 646f 776e              down
-0000d220: 6c6f 6164 6564 4767 7566 4d6f 6465 6c73  loadedGgufModels
-0000d230: 203d 2067 6574 446f 776e 6c6f 6164 6564   = getDownloaded
-0000d240: 4767 7566 4d6f 6465 6c73 2829 0a20 2020  GgufModels().   
-0000d250: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000d260: 6e6f 7420 646f 776e 6c6f 6164 6564 4767  not downloadedGg
-0000d270: 7566 4d6f 6465 6c73 3a0a 2020 2020 2020  ufModels:.      
-0000d280: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d290: 6c66 2e73 6574 4375 7374 6f6d 4875 6767  lf.setCustomHugg
-0000d2a0: 696e 6766 6163 654d 6f64 656c 2866 6561  ingfaceModel(fea
-0000d2b0: 7475 7265 3d66 6561 7475 7265 290a 2020  ture=feature).  
-0000d2c0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000d2d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000d2e0: 2020 2020 2020 2020 6d6f 6465 6c20 3d20          model = 
-0000d2f0: 7365 6c66 2e64 6961 6c6f 6773 2e67 6574  self.dialogs.get
-0000d300: 5661 6c69 644f 7074 696f 6e73 280a 2020  ValidOptions(.  
+0000d1b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d1c0: 6665 6174 7572 6520 3d3d 2022 6465 6661  feature == "defa
+0000d1d0: 756c 7422 3a0a 2020 2020 2020 2020 2020  ult":.          
+0000d1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d1f0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0000d200: 2e6c 6c61 6d61 6370 704d 6169 6e4d 6f64  .llamacppMainMod
+0000d210: 656c 5f6d 6f64 656c 5f70 6174 6820 3d20  el_model_path = 
+0000d220: 646f 776e 6c6f 6164 6564 4f6c 6c61 6d61  downloadedOllama
+0000d230: 4d6f 6465 6c73 5b6d 6f64 656c 5d0a 2020  Models[model].  
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000d260: 6966 2066 6561 7475 7265 203d 3d20 2263  if feature == "c
+0000d270: 6f64 6522 3a0a 2020 2020 2020 2020 2020  ode":.          
+0000d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d290: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0000d2a0: 2e6c 6c61 6d61 6370 7043 6861 744d 6f64  .llamacppChatMod
+0000d2b0: 656c 5f6d 6f64 656c 5f70 6174 6820 3d20  el_model_path = 
+0000d2c0: 646f 776e 6c6f 6164 6564 4f6c 6c61 6d61  downloadedOllama
+0000d2d0: 4d6f 6465 6c73 5b6d 6f64 656c 5d0a 2020  Models[model].  
+0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2f0: 2020 2020 2020 2020 2020 6578 6365 7074            except
+0000d300: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
 0000d310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d320: 2020 2020 2020 6f70 7469 6f6e 733d 6c69        options=li
-0000d330: 7374 2864 6f77 6e6c 6f61 6465 6447 6775  st(downloadedGgu
-0000d340: 664d 6f64 656c 732e 6b65 7973 2829 2920  fModels.keys()) 
-0000d350: 2b20 5b22 4f74 6865 7273 202e 2e2e 225d  + ["Others ..."]
-0000d360: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d370: 2020 2020 2020 2020 2020 7469 746c 653d            title=
-0000d380: 2248 7567 6769 6e67 6661 6365 2048 7562  "Huggingface Hub
-0000d390: 204d 6f64 656c 222c 0a20 2020 2020 2020   Model",.       
+0000d320: 2020 7072 696e 7432 2866 2246 6169 6c65    print2(f"Faile
+0000d330: 6420 746f 2064 6f77 6e6c 6f61 6420 277b  d to download '{
+0000d340: 6d6f 6465 6c7d 2721 2050 6c65 6173 6520  model}'! Please 
+0000d350: 6d61 6b65 2073 7572 6520 796f 7520 656e  make sure you en
+0000d360: 7465 7220 6120 7661 6c69 6420 6d6f 6465  ter a valid mode
+0000d370: 6c20 6e61 6d65 206f 7220 7461 672e 2229  l name or tag.")
+0000d380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d390: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
 0000d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3b0: 2064 6566 6175 6c74 3d22 2220 6966 202e   default="" if .
-0000d3c0: 2e2e 2065 6c73 6520 2222 2c0a 2020 2020  .. else "",.    
-0000d3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d3e0: 2020 2020 7465 7874 3d22 5365 6c65 6374      text="Select
-0000d3f0: 2061 2068 7567 6769 6e67 6661 6365 206d   a huggingface m
-0000d400: 6f64 656c 3a22 2c0a 2020 2020 2020 2020  odel:",.        
-0000d410: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-0000d420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d430: 2020 6966 206d 6f64 656c 3a0a 2020 2020    if model:.    
-0000d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d450: 2020 2020 6966 206d 6f64 656c 203d 3d20      if model == 
-0000d460: 224f 7468 6572 7320 2e2e 2e22 3a0a 2020  "Others ...":.  
-0000d470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d480: 2020 2020 2020 2020 2020 7365 6c66 2e73            self.s
-0000d490: 6574 4375 7374 6f6d 4875 6767 696e 6766  etCustomHuggingf
-0000d4a0: 6163 654d 6f64 656c 2866 6561 7475 7265  aceModel(feature
-0000d4b0: 3d66 6561 7475 7265 290a 2020 2020 2020  =feature).      
-0000d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4d0: 2020 656c 6966 2066 6561 7475 7265 203d    elif feature =
-0000d4e0: 3d20 2264 6566 6175 6c74 223a 0a20 2020  = "default":.   
-0000d4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d500: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-0000d510: 6c6c 616d 6163 7070 4d61 696e 4d6f 6465  llamacppMainMode
-0000d520: 6c5f 6d6f 6465 6c5f 7061 7468 203d 2064  l_model_path = d
-0000d530: 6f77 6e6c 6f61 6465 6447 6775 664d 6f64  ownloadedGgufMod
-0000d540: 656c 735b 6d6f 6465 6c5d 0a20 2020 2020  els[model].     
-0000d550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d560: 2020 2065 6c69 6620 6665 6174 7572 6520     elif feature 
-0000d570: 3d3d 2022 636f 6465 223a 0a20 2020 2020  == "code":.     
-0000d580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d590: 2020 2020 2020 2063 6f6e 6669 672e 6c6c         config.ll
-0000d5a0: 616d 6163 7070 4368 6174 4d6f 6465 6c5f  amacppChatModel_
-0000d5b0: 6d6f 6465 6c5f 7061 7468 203d 2064 6f77  model_path = dow
-0000d5c0: 6e6c 6f61 6465 6447 6775 664d 6f64 656c  nloadedGgufModel
-0000d5d0: 735b 6d6f 6465 6c5d 0a20 2020 2020 2020  s[model].       
-0000d5e0: 2020 2020 2065 6c69 6620 6c69 6272 6172       elif librar
-0000d5f0: 7920 3d3d 2022 4375 7374 6f6d 2047 4755  y == "Custom GGU
-0000d600: 4622 3a0a 2020 2020 2020 2020 2020 2020  F":.            
-0000d610: 2020 2020 7365 6c66 2e73 6574 4375 7374      self.setCust
-0000d620: 6f6d 4d6f 6465 6c50 6174 6828 6665 6174  omModelPath(feat
-0000d630: 7572 653d 6665 6174 7572 6529 0a0a 2020  ure=feature)..  
-0000d640: 2020 6465 6620 7365 7443 7573 746f 6d4d    def setCustomM
-0000d650: 6f64 656c 5061 7468 2873 656c 662c 2066  odelPath(self, f
-0000d660: 6561 7475 7265 3d22 6465 6661 756c 7422  eature="default"
-0000d670: 293a 0a20 2020 2020 2020 206d 6f64 656c  ):.        model
-0000d680: 5f70 6174 6820 3d20 7365 6c66 2e67 6574  _path = self.get
-0000d690: 5061 7468 2e67 6574 4669 6c65 5061 7468  Path.getFilePath
-0000d6a0: 280a 2020 2020 2020 2020 2020 2020 6368  (.            ch
-0000d6b0: 6563 6b5f 6973 6669 6c65 3d54 7275 652c  eck_isfile=True,
-0000d6c0: 0a20 2020 2020 2020 2020 2020 2065 6d70  .            emp
-0000d6d0: 7479 5f74 6f5f 6361 6e63 656c 3d54 7275  ty_to_cancel=Tru
-0000d6e0: 652c 0a20 2020 2020 2020 2020 2020 206c  e,.            l
-0000d6f0: 6973 745f 636f 6e74 656e 745f 6f6e 5f64  ist_content_on_d
-0000d700: 6972 6563 746f 7279 5f63 6861 6e67 653d  irectory_change=
-0000d710: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000d720: 2020 6b65 6570 5f73 7461 7274 7570 5f64    keep_startup_d
-0000d730: 6972 6563 746f 7279 3d54 7275 652c 0a20  irectory=True,. 
-0000d740: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0000d750: 6765 3d22 456e 7465 7220 6120 6375 7374  ge="Enter a cust
-0000d760: 6f6d 206d 6f64 656c 2070 6174 683a 222c  om model path:",
-0000d770: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
-0000d780: 6175 6c74 3d63 6f6e 6669 672e 6c6c 616d  ault=config.llam
-0000d790: 6163 7070 4368 6174 4d6f 6465 6c5f 6d6f  acppChatModel_mo
-0000d7a0: 6465 6c5f 7061 7468 2069 6620 6665 6174  del_path if feat
-0000d7b0: 7572 6520 3d3d 2022 636f 6465 2220 656c  ure == "code" el
-0000d7c0: 7365 2063 6f6e 6669 672e 6c6c 616d 6163  se config.llamac
-0000d7d0: 7070 4d61 696e 4d6f 6465 6c5f 6d6f 6465  ppMainModel_mode
-0000d7e0: 6c5f 7061 7468 2c0a 2020 2020 2020 2020  l_path,.        
-0000d7f0: 290a 2020 2020 2020 2020 6966 206d 6f64  ).        if mod
-0000d800: 656c 5f70 6174 6820 616e 6420 6f73 2e70  el_path and os.p
-0000d810: 6174 682e 6973 6669 6c65 286d 6f64 656c  ath.isfile(model
-0000d820: 5f70 6174 6829 3a0a 2020 2020 2020 2020  _path):.        
-0000d830: 2020 2020 6966 2066 6561 7475 7265 203d      if feature =
-0000d840: 3d20 2264 6566 6175 6c74 223a 0a20 2020  = "default":.   
-0000d850: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0000d860: 6669 672e 6c6c 616d 6163 7070 4d61 696e  fig.llamacppMain
-0000d870: 4d6f 6465 6c5f 6d6f 6465 6c5f 7061 7468  Model_model_path
-0000d880: 203d 206d 6f64 656c 5f70 6174 680a 2020   = model_path.  
-0000d890: 2020 2020 2020 2020 2020 656c 6966 2066            elif f
-0000d8a0: 6561 7475 7265 203d 3d20 2263 6f64 6522  eature == "code"
-0000d8b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d8c0: 2020 636f 6e66 6967 2e6c 6c61 6d61 6370    config.llamacp
-0000d8d0: 7043 6861 744d 6f64 656c 5f6d 6f64 656c  pChatModel_model
-0000d8e0: 5f70 6174 6820 3d20 6d6f 6465 6c5f 7061  _path = model_pa
-0000d8f0: 7468 0a0a 2020 2020 6465 6620 7365 7443  th..    def setC
-0000d900: 7573 746f 6d48 7567 6769 6e67 6661 6365  ustomHuggingface
-0000d910: 4d6f 6465 6c28 7365 6c66 2c20 6665 6174  Model(self, feat
-0000d920: 7572 653d 2264 6566 6175 6c74 2229 3a0a  ure="default"):.
-0000d930: 2020 2020 2020 2020 6869 7374 6f72 7946          historyF
-0000d940: 6f6c 6465 7220 3d20 6f73 2e70 6174 682e  older = os.path.
-0000d950: 6a6f 696e 2863 6f6e 6669 672e 6c6f 6361  join(config.loca
-0000d960: 6c53 746f 7261 6765 2c20 2268 6973 746f  lStorage, "histo
-0000d970: 7279 2229 0a20 2020 2020 2020 2050 6174  ry").        Pat
-0000d980: 6828 6869 7374 6f72 7946 6f6c 6465 7229  h(historyFolder)
-0000d990: 2e6d 6b64 6972 2870 6172 656e 7473 3d54  .mkdir(parents=T
-0000d9a0: 7275 652c 2065 7869 7374 5f6f 6b3d 5472  rue, exist_ok=Tr
-0000d9b0: 7565 290a 2020 2020 2020 2020 7265 706f  ue).        repo
-0000d9c0: 5f69 645f 6869 7374 6f72 7920 3d20 6f73  _id_history = os
-0000d9d0: 2e70 6174 682e 6a6f 696e 2868 6973 746f  .path.join(histo
-0000d9e0: 7279 466f 6c64 6572 2c20 226c 6c61 6d61  ryFolder, "llama
-0000d9f0: 6370 705f 636f 6465 5f72 6570 6f5f 6964  cpp_code_repo_id
-0000da00: 2220 6966 2066 6561 7475 7265 203d 3d20  " if feature == 
-0000da10: 2263 6f64 6522 2065 6c73 6520 226c 6c61  "code" else "lla
-0000da20: 6d61 6370 705f 6465 6661 756c 745f 7265  macpp_default_re
-0000da30: 706f 5f69 6422 290a 2020 2020 2020 2020  po_id").        
-0000da40: 7265 706f 5f69 645f 7365 7373 696f 6e20  repo_id_session 
-0000da50: 3d20 5072 6f6d 7074 5365 7373 696f 6e28  = PromptSession(
-0000da60: 6869 7374 6f72 793d 4669 6c65 4869 7374  history=FileHist
-0000da70: 6f72 7928 7265 706f 5f69 645f 6869 7374  ory(repo_id_hist
-0000da80: 6f72 7929 290a 2020 2020 2020 2020 6669  ory)).        fi
-0000da90: 6c65 6e61 6d65 5f68 6973 746f 7279 203d  lename_history =
-0000daa0: 206f 732e 7061 7468 2e6a 6f69 6e28 6869   os.path.join(hi
-0000dab0: 7374 6f72 7946 6f6c 6465 722c 2022 6c6c  storyFolder, "ll
-0000dac0: 616d 6163 7070 5f63 6f64 655f 6669 6c65  amacpp_code_file
-0000dad0: 6e61 6d65 2220 6966 2066 6561 7475 7265  name" if feature
-0000dae0: 203d 3d20 2263 6f64 6522 2065 6c73 6520   == "code" else 
-0000daf0: 226c 6c61 6d61 6370 705f 6465 6661 756c  "llamacpp_defaul
-0000db00: 745f 6669 6c65 6e61 6d65 2229 0a20 2020  t_filename").   
-0000db10: 2020 2020 2066 696c 656e 616d 655f 7365       filename_se
-0000db20: 7373 696f 6e20 3d20 5072 6f6d 7074 5365  ssion = PromptSe
-0000db30: 7373 696f 6e28 6869 7374 6f72 793d 4669  ssion(history=Fi
-0000db40: 6c65 4869 7374 6f72 7928 6669 6c65 6e61  leHistory(filena
-0000db50: 6d65 5f68 6973 746f 7279 2929 0a20 2020  me_history)).   
-0000db60: 2020 2020 2062 6f74 746f 6d5f 746f 6f6c       bottom_tool
-0000db70: 6261 7220 3d20 6622 2222 207b 7374 7228  bar = f""" {str(
-0000db80: 636f 6e66 6967 2e68 6f74 6b65 795f 6578  config.hotkey_ex
-0000db90: 6974 292e 7265 706c 6163 6528 2227 222c  it).replace("'",
-0000dba0: 2022 2229 7d20 7b63 6f6e 6669 672e 6578   "")} {config.ex
-0000dbb0: 6974 5f65 6e74 7279 7d22 2222 0a20 2020  it_entry}""".   
-0000dbc0: 2020 2020 2070 7269 6e74 3128 2250 6c65       print1("Ple
-0000dbd0: 6173 6520 7370 6563 6966 7920 7468 6520  ase specify the 
-0000dbe0: 6875 6767 696e 6766 6163 6520 7265 706f  huggingface repo
-0000dbf0: 2069 6420 6f66 2061 202a 2e67 6775 6620   id of a *.gguf 
-0000dc00: 6d6f 6465 6c3a 2229 0a20 2020 2020 2020  model:").       
-0000dc10: 2072 6570 6f5f 6964 203d 2073 656c 662e   repo_id = self.
-0000dc20: 7072 6f6d 7074 732e 7369 6d70 6c65 5072  prompts.simplePr
-0000dc30: 6f6d 7074 2873 7479 6c65 3d73 656c 662e  ompt(style=self.
-0000dc40: 7072 6f6d 7074 732e 7072 6f6d 7074 5374  prompts.promptSt
-0000dc50: 796c 6532 2c20 7072 6f6d 7074 5365 7373  yle2, promptSess
-0000dc60: 696f 6e3d 7265 706f 5f69 645f 7365 7373  ion=repo_id_sess
-0000dc70: 696f 6e2c 2062 6f74 746f 6d5f 746f 6f6c  ion, bottom_tool
-0000dc80: 6261 723d 626f 7474 6f6d 5f74 6f6f 6c62  bar=bottom_toolb
-0000dc90: 6172 2c20 6465 6661 756c 743d 636f 6e66  ar, default=conf
-0000dca0: 6967 2e6c 6c61 6d61 6370 7043 6861 744d  ig.llamacppChatM
-0000dcb0: 6f64 656c 5f72 6570 6f5f 6964 2069 6620  odel_repo_id if 
-0000dcc0: 6665 6174 7572 6520 3d3d 2022 636f 6465  feature == "code
-0000dcd0: 2220 656c 7365 2063 6f6e 6669 672e 6c6c  " else config.ll
-0000dce0: 616d 6163 7070 4d61 696e 4d6f 6465 6c5f  amacppMainModel_
-0000dcf0: 7265 706f 5f69 6429 0a20 2020 2020 2020  repo_id).       
-0000dd00: 2070 7269 6e74 3228 2250 6c65 6173 6520   print2("Please 
-0000dd10: 7370 6563 6966 7920 6120 6669 6c65 6e61  specify a filena
-0000dd20: 6d65 206f 7220 676c 6f62 2070 6174 7465  me or glob patte
-0000dd30: 726e 2074 6f20 6d61 7463 6820 7468 6520  rn to match the 
-0000dd40: 6d6f 6465 6c20 6669 6c65 2069 6e20 7468  model file in th
-0000dd50: 6520 7265 706f 3a22 290a 2020 2020 2020  e repo:").      
-0000dd60: 2020 6669 6c65 6e61 6d65 203d 2073 656c    filename = sel
-0000dd70: 662e 7072 6f6d 7074 732e 7369 6d70 6c65  f.prompts.simple
-0000dd80: 5072 6f6d 7074 2873 7479 6c65 3d73 656c  Prompt(style=sel
-0000dd90: 662e 7072 6f6d 7074 732e 7072 6f6d 7074  f.prompts.prompt
-0000dda0: 5374 796c 6532 2c20 7072 6f6d 7074 5365  Style2, promptSe
-0000ddb0: 7373 696f 6e3d 6669 6c65 6e61 6d65 5f73  ssion=filename_s
-0000ddc0: 6573 7369 6f6e 2c20 626f 7474 6f6d 5f74  ession, bottom_t
-0000ddd0: 6f6f 6c62 6172 3d62 6f74 746f 6d5f 746f  oolbar=bottom_to
-0000dde0: 6f6c 6261 722c 2064 6566 6175 6c74 3d63  olbar, default=c
-0000ddf0: 6f6e 6669 672e 6c6c 616d 6163 7070 4368  onfig.llamacppCh
-0000de00: 6174 4d6f 6465 6c5f 6669 6c65 6e61 6d65  atModel_filename
-0000de10: 2069 6620 6665 6174 7572 6520 3d3d 2022   if feature == "
-0000de20: 636f 6465 2220 656c 7365 2063 6f6e 6669  code" else confi
-0000de30: 672e 6c6c 616d 6163 7070 4d61 696e 4d6f  g.llamacppMainMo
-0000de40: 6465 6c5f 6669 6c65 6e61 6d65 290a 2020  del_filename).  
-0000de50: 2020 2020 2020 6966 2028 7265 706f 5f69        if (repo_i
-0000de60: 6420 616e 6420 6e6f 7420 7265 706f 5f69  d and not repo_i
-0000de70: 642e 6c6f 7765 7228 2920 3d3d 2063 6f6e  d.lower() == con
-0000de80: 6669 672e 6578 6974 5f65 6e74 7279 2920  fig.exit_entry) 
-0000de90: 616e 6420 2866 696c 656e 616d 6520 616e  and (filename an
-0000dea0: 6420 6e6f 7420 6669 6c65 6e61 6d65 2e6c  d not filename.l
-0000deb0: 6f77 6572 2829 203d 3d20 636f 6e66 6967  ower() == config
-0000dec0: 2e65 7869 745f 656e 7472 7929 3a0a 2020  .exit_entry):.  
-0000ded0: 2020 2020 2020 2020 2020 6966 2066 6561            if fea
-0000dee0: 7475 7265 203d 3d20 2264 6566 6175 6c74  ture == "default
-0000def0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-0000df00: 2020 2063 6f6e 6669 672e 6c6c 616d 6163     config.llamac
-0000df10: 7070 4d61 696e 4d6f 6465 6c5f 7265 706f  ppMainModel_repo
-0000df20: 5f69 6420 3d20 7265 706f 5f69 640a 2020  _id = repo_id.  
-0000df30: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000df40: 6e66 6967 2e6c 6c61 6d61 6370 704d 6169  nfig.llamacppMai
-0000df50: 6e4d 6f64 656c 5f66 696c 656e 616d 6520  nModel_filename 
-0000df60: 3d20 6669 6c65 6e61 6d65 0a20 2020 2020  = filename.     
-0000df70: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-0000df80: 672e 6c6c 616d 6163 7070 4d61 696e 4d6f  g.llamacppMainMo
-0000df90: 6465 6c5f 6d6f 6465 6c5f 7061 7468 203d  del_model_path =
-0000dfa0: 2022 220a 2020 2020 2020 2020 2020 2020   "".            
-0000dfb0: 656c 6966 2066 6561 7475 7265 203d 3d20  elif feature == 
-0000dfc0: 2263 6f64 6522 3a0a 2020 2020 2020 2020  "code":.        
-0000dfd0: 2020 2020 2020 2020 636f 6e66 6967 2e6c          config.l
-0000dfe0: 6c61 6d61 6370 7043 6861 744d 6f64 656c  lamacppChatModel
-0000dff0: 5f72 6570 6f5f 6964 203d 2072 6570 6f5f  _repo_id = repo_
-0000e000: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
-0000e010: 2020 2063 6f6e 6669 672e 6c6c 616d 6163     config.llamac
-0000e020: 7070 4368 6174 4d6f 6465 6c5f 6669 6c65  ppChatModel_file
-0000e030: 6e61 6d65 203d 2066 696c 656e 616d 650a  name = filename.
-0000e040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e050: 636f 6e66 6967 2e6c 6c61 6d61 6370 7043  config.llamacppC
-0000e060: 6861 744d 6f64 656c 5f6d 6f64 656c 5f70  hatModel_model_p
-0000e070: 6174 6820 3d20 2222 0a20 2020 2020 2020  ath = "".       
-0000e080: 2020 2020 2043 616c 6c4c 4c4d 2e63 6865       CallLLM.che
-0000e090: 636b 436f 6d70 6c65 7469 6f6e 2829 0a20  ckCompletion(). 
-0000e0a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000e0b0: 2020 2020 2020 2020 2070 7269 6e74 3228           print2(
-0000e0c0: 2241 6374 696f 6e20 6361 6e63 656c 6c65  "Action cancelle
-0000e0d0: 6420 6475 6520 746f 2069 6e73 7566 6669  d due to insuffi
-0000e0e0: 6369 656e 7420 696e 666f 726d 6174 696f  cient informatio
-0000e0f0: 6e21 2229 0a0a 2020 2020 6465 6620 7365  n!")..    def se
-0000e100: 744c 6c6d 4d6f 6465 6c5f 6368 6174 6770  tLlmModel_chatgp
-0000e110: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
-0000e120: 206d 6f64 656c 203d 2073 656c 662e 6469   model = self.di
-0000e130: 616c 6f67 732e 6765 7456 616c 6964 4f70  alogs.getValidOp
-0000e140: 7469 6f6e 7328 0a20 2020 2020 2020 2020  tions(.         
-0000e150: 2020 206f 7074 696f 6e73 3d73 656c 662e     options=self.
-0000e160: 6d6f 6465 6c73 2c0a 2020 2020 2020 2020  models,.        
-0000e170: 2020 2020 7469 746c 653d 2246 756e 6374      title="Funct
-0000e180: 696f 6e20 4361 6c6c 696e 6720 4d6f 6465  ion Calling Mode
-0000e190: 6c22 2c0a 2020 2020 2020 2020 2020 2020  l",.            
-0000e1a0: 6465 6661 756c 743d 636f 6e66 6967 2e63  default=config.c
-0000e1b0: 6861 7447 5054 4170 694d 6f64 656c 2069  hatGPTApiModel i
-0000e1c0: 6620 636f 6e66 6967 2e63 6861 7447 5054  f config.chatGPT
-0000e1d0: 4170 694d 6f64 656c 2069 6e20 7365 6c66  ApiModel in self
-0000e1e0: 2e6d 6f64 656c 7320 656c 7365 2073 656c  .models else sel
-0000e1f0: 662e 6d6f 6465 6c73 5b30 5d2c 0a20 2020  f.models[0],.   
-0000e200: 2020 2020 2020 2020 2074 6578 743d 2253           text="S
-0000e210: 656c 6563 7420 6120 6675 6e63 7469 6f6e  elect a function
-0000e220: 2063 616c 6c20 6d6f 6465 6c3a 5c6e 2866   call model:\n(f
-0000e230: 6f72 2062 6f74 6820 6368 6174 2061 6e64  or both chat and
-0000e240: 2074 6173 6b20 6578 6563 7574 696f 6e29   task execution)
-0000e250: 222c 0a20 2020 2020 2020 2029 0a20 2020  ",.        ).   
-0000e260: 2020 2020 2069 6620 6d6f 6465 6c3a 0a20       if model:. 
-0000e270: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-0000e280: 672e 6368 6174 4750 5441 7069 4d6f 6465  g.chatGPTApiMode
-0000e290: 6c20 3d20 6d6f 6465 6c0a 2020 2020 2020  l = model.      
-0000e2a0: 2020 2020 2020 7072 696e 7433 2866 2243        print3(f"C
-0000e2b0: 6861 7447 5054 206d 6f64 656c 3a20 7b6d  hatGPT model: {m
-0000e2c0: 6f64 656c 7d22 290a 2020 2020 2020 2020  odel}").        
-0000e2d0: 2020 2020 2320 7365 7420 6d61 7820 746f      # set max to
-0000e2e0: 6b65 6e73 0a20 2020 2020 2020 2020 2020  kens.           
-0000e2f0: 2063 6f6e 6669 672e 6368 6174 4750 5441   config.chatGPTA
-0000e300: 7069 4d61 7854 6f6b 656e 7320 3d20 7365  piMaxTokens = se
-0000e310: 6c66 2e67 6574 4d61 7854 6f6b 656e 7328  lf.getMaxTokens(
-0000e320: 295b 2d31 5d0a 2020 2020 2020 2020 2020  )[-1].          
-0000e330: 2020 7072 696e 7433 2866 224d 6178 696d    print3(f"Maxim
-0000e340: 756d 206f 7574 7075 7420 746f 6b65 6e73  um output tokens
-0000e350: 3a20 7b63 6f6e 6669 672e 6368 6174 4750  : {config.chatGP
-0000e360: 5441 7069 4d61 7854 6f6b 656e 737d 2229  TApiMaxTokens}")
-0000e370: 0a0a 2020 2020 6465 6620 7365 7443 6861  ..    def setCha
-0000e380: 7462 6f74 2873 656c 6629 3a0a 2020 2020  tbot(self):.    
-0000e390: 2020 2020 6d6f 6465 6c20 3d20 7365 6c66      model = self
-0000e3a0: 2e64 6961 6c6f 6773 2e67 6574 5661 6c69  .dialogs.getVali
-0000e3b0: 644f 7074 696f 6e73 280a 2020 2020 2020  dOptions(.      
-0000e3c0: 2020 2020 2020 6f70 7469 6f6e 733d 2822        options=("
-0000e3d0: 6368 6174 6770 7422 2c20 2267 656d 696e  chatgpt", "gemin
-0000e3e0: 6970 726f 222c 2022 7061 6c6d 3222 2c20  ipro", "palm2", 
-0000e3f0: 2263 6f64 6579 2229 2c0a 2020 2020 2020  "codey"),.      
-0000e400: 2020 2020 2020 7469 746c 653d 2243 6861        title="Cha
-0000e410: 742d 6f6e 6c79 206d 6f64 656c 222c 0a20  t-only model",. 
-0000e420: 2020 2020 2020 2020 2020 2064 6566 6175             defau
-0000e430: 6c74 3d63 6f6e 6669 672e 6368 6174 626f  lt=config.chatbo
-0000e440: 742c 0a20 2020 2020 2020 2020 2020 2074  t,.            t
-0000e450: 6578 743d 2253 656c 6563 7420 6465 6661  ext="Select defa
-0000e460: 756c 7420 6368 6174 2d6f 6e6c 7920 6d6f  ult chat-only mo
-0000e470: 6465 6c3a 5c6e 2844 6566 6175 6c74 206d  del:\n(Default m
-0000e480: 6f64 656c 2069 7320 6c6f 6164 6564 2077  odel is loaded w
-0000e490: 6865 6e20 796f 7520 696e 636c 7564 6520  hen you include 
-0000e4a0: 275b 4348 4154 5d27 2069 6e20 796f 7572  '[CHAT]' in your
-0000e4b0: 2069 6e70 7574 2922 2c0a 2020 2020 2020   input)",.      
-0000e4c0: 2020 290a 2020 2020 2020 2020 6966 206d    ).        if m
-0000e4d0: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
-0000e4e0: 2020 636f 6e66 6967 2e63 6861 7462 6f74    config.chatbot
-0000e4f0: 203d 206d 6f64 656c 0a20 2020 2020 2020   = model.       
-0000e500: 2020 2020 2070 7269 6e74 3328 6622 4368       print3(f"Ch
-0000e510: 6174 2d6f 6e6c 7920 6d6f 6465 6c3a 207b  at-only model: {
-0000e520: 6d6f 6465 6c7d 2229 0a0a 2020 2020 6465  model}")..    de
-0000e530: 6620 7365 7445 6d62 6564 6469 6e67 4d6f  f setEmbeddingMo
-0000e540: 6465 6c28 7365 6c66 293a 0a20 2020 2020  del(self):.     
-0000e550: 2020 206f 6c64 456d 6265 6464 696e 674d     oldEmbeddingM
-0000e560: 6f64 656c 203d 2063 6f6e 6669 672e 656d  odel = config.em
-0000e570: 6265 6464 696e 674d 6f64 656c 0a20 2020  beddingModel.   
-0000e580: 2020 2020 206d 6f64 656c 203d 2073 656c       model = sel
-0000e590: 662e 6469 616c 6f67 732e 6765 7456 616c  f.dialogs.getVal
-0000e5a0: 6964 4f70 7469 6f6e 7328 0a20 2020 2020  idOptions(.     
-0000e5b0: 2020 2020 2020 206f 7074 696f 6e73 3d28         options=(
-0000e5c0: 2274 6578 742d 656d 6265 6464 696e 672d  "text-embedding-
-0000e5d0: 332d 6c61 7267 6522 2c20 2274 6578 742d  3-large", "text-
-0000e5e0: 656d 6265 6464 696e 672d 332d 736d 616c  embedding-3-smal
-0000e5f0: 6c22 2c20 2274 6578 742d 656d 6265 6464  l", "text-embedd
-0000e600: 696e 672d 6164 612d 3030 3222 2c20 2270  ing-ada-002", "p
-0000e610: 6172 6170 6872 6173 652d 6d75 6c74 696c  araphrase-multil
-0000e620: 696e 6775 616c 2d6d 706e 6574 2d62 6173  ingual-mpnet-bas
-0000e630: 652d 7632 222c 2022 616c 6c2d 6d70 6e65  e-v2", "all-mpne
-0000e640: 742d 6261 7365 2d76 3222 2c20 2261 6c6c  t-base-v2", "all
-0000e650: 2d4d 696e 694c 4d2d 4c36 2d76 3222 2c20  -MiniLM-L6-v2", 
-0000e660: 2263 7573 746f 6d22 292c 0a20 2020 2020  "custom"),.     
-0000e670: 2020 2020 2020 2074 6974 6c65 3d22 456d         title="Em
-0000e680: 6265 6464 696e 6720 6d6f 6465 6c22 2c0a  bedding model",.
-0000e690: 2020 2020 2020 2020 2020 2020 6465 6661              defa
-0000e6a0: 756c 743d 636f 6e66 6967 2e65 6d62 6564  ult=config.embed
-0000e6b0: 6469 6e67 4d6f 6465 6c2c 0a20 2020 2020  dingModel,.     
-0000e6c0: 2020 2020 2020 2074 6578 743d 2253 656c         text="Sel
-0000e6d0: 6563 7420 616e 2065 6d62 6564 6469 6e67  ect an embedding
-0000e6e0: 206d 6f64 656c 3a22 2c0a 2020 2020 2020   model:",.      
-0000e6f0: 2020 290a 2020 2020 2020 2020 6966 206d    ).        if m
-0000e700: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
-0000e710: 2020 6966 206d 6f64 656c 203d 3d20 2263    if model == "c
-0000e720: 7573 746f 6d22 3a0a 2020 2020 2020 2020  ustom":.        
-0000e730: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
-0000e740: 456e 7465 7220 4f70 656e 4149 206f 7220  Enter OpenAI or 
-0000e750: 5365 6e74 656e 6365 2054 7261 6e73 666f  Sentence Transfo
-0000e760: 726d 6572 2045 6d62 6564 6469 6e67 206d  rmer Embedding m
-0000e770: 6f64 656c 3a22 290a 2020 2020 2020 2020  odel:").        
-0000e780: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
-0000e790: 5265 6164 206d 6f72 6520 6174 3a20 6874  Read more at: ht
-0000e7a0: 7470 733a 2f2f 7777 772e 7362 6572 742e  tps://www.sbert.
-0000e7b0: 6e65 742f 646f 6373 2f70 7265 7472 6169  net/docs/pretrai
-0000e7c0: 6e65 645f 6d6f 6465 6c73 2e68 746d 6c22  ned_models.html"
-0000e7d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000e7e0: 2020 6375 7374 6f6d 4d6f 6465 6c20 3d20    customModel = 
-0000e7f0: 7365 6c66 2e70 726f 6d70 7473 2e73 696d  self.prompts.sim
-0000e800: 706c 6550 726f 6d70 7428 7374 796c 653d  plePrompt(style=
-0000e810: 7365 6c66 2e70 726f 6d70 7473 2e70 726f  self.prompts.pro
-0000e820: 6d70 7453 7479 6c65 322c 2064 6566 6175  mptStyle2, defau
-0000e830: 6c74 3d63 6f6e 6669 672e 656d 6265 6464  lt=config.embedd
-0000e840: 696e 674d 6f64 656c 290a 2020 2020 2020  ingModel).      
-0000e850: 2020 2020 2020 2020 2020 6966 2063 7573            if cus
-0000e860: 746f 6d4d 6f64 656c 2061 6e64 206e 6f74  tomModel and not
-0000e870: 2063 7573 746f 6d4d 6f64 656c 2e73 7472   customModel.str
-0000e880: 6970 2829 2e6c 6f77 6572 2829 203d 3d20  ip().lower() == 
-0000e890: 636f 6e66 6967 2e65 7869 745f 656e 7472  config.exit_entr
-0000e8a0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000e8b0: 2020 2020 2020 2063 6f6e 6669 672e 656d         config.em
-0000e8c0: 6265 6464 696e 674d 6f64 656c 203d 2063  beddingModel = c
-0000e8d0: 7573 746f 6d4d 6f64 656c 200a 2020 2020  ustomModel .    
-0000e8e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000e900: 6e66 6967 2e65 6d62 6564 6469 6e67 4d6f  nfig.embeddingMo
-0000e910: 6465 6c20 3d20 6d6f 6465 6c0a 2020 2020  del = model.    
-0000e920: 2020 2020 2020 2020 7072 696e 7433 2866          print3(f
-0000e930: 2245 6d62 6564 6469 6e67 206d 6f64 656c  "Embedding model
-0000e940: 3a20 7b6d 6f64 656c 7d22 290a 2020 2020  : {model}").    
-0000e950: 2020 2020 6966 206e 6f74 206f 6c64 456d      if not oldEm
-0000e960: 6265 6464 696e 674d 6f64 656c 203d 3d20  beddingModel == 
-0000e970: 636f 6e66 6967 2e65 6d62 6564 6469 6e67  config.embedding
-0000e980: 4d6f 6465 6c3a 0a20 2020 2020 2020 2020  Model:.         
-0000e990: 2020 2070 7269 6e74 3128 6622 596f 7527     print1(f"You'
-0000e9a0: 7665 2063 6861 6e67 6520 7468 6520 656d  ve change the em
-0000e9b0: 6265 6464 696e 6720 6d6f 6465 6c20 6672  bedding model fr
-0000e9c0: 6f6d 2027 7b6f 6c64 456d 6265 6464 696e  om '{oldEmbeddin
-0000e9d0: 674d 6f64 656c 7d27 2074 6f20 277b 636f  gModel}' to '{co
-0000e9e0: 6e66 6967 2e65 6d62 6564 6469 6e67 4d6f  nfig.embeddingMo
-0000e9f0: 6465 6c7d 272e 2229 0a20 2020 2020 2020  del}'.").       
-0000ea00: 2020 2020 2070 7269 6e74 3128 2254 6f20       print1("To 
-0000ea10: 776f 726b 2077 6974 6820 7468 6520 6e65  work with the ne
-0000ea20: 776c 7920 7365 6c65 6374 6564 206d 6f64  wly selected mod
-0000ea30: 656c 2c20 7072 6576 696f 7573 206d 656d  el, previous mem
-0000ea40: 6f72 7920 7374 6f72 6520 616e 6420 7265  ory store and re
-0000ea50: 7472 6965 7665 6420 636f 6c6c 6563 7469  trieved collecti
-0000ea60: 6f6e 7320 6e65 6564 2074 6f20 6265 2064  ons need to be d
-0000ea70: 656c 6574 6564 2e22 290a 2020 2020 2020  eleted.").      
-0000ea80: 2020 2020 2020 7072 696e 7431 2822 446f        print1("Do
-0000ea90: 2079 6f75 2077 616e 7420 746f 2064 656c   you want to del
-0000eaa0: 6574 6520 7468 656d 206e 6f77 3f20 5b79  ete them now? [y
-0000eab0: 5d65 7320 2f20 5b4e 5d6f 2229 0a20 2020  ]es / [N]o").   
-0000eac0: 2020 2020 2020 2020 2063 6f6e 6669 726d           confirm
-0000ead0: 6174 696f 6e20 3d20 7365 6c66 2e70 726f  ation = self.pro
-0000eae0: 6d70 7473 2e73 696d 706c 6550 726f 6d70  mpts.simplePromp
-0000eaf0: 7428 7374 796c 653d 7365 6c66 2e70 726f  t(style=self.pro
-0000eb00: 6d70 7473 2e70 726f 6d70 7453 7479 6c65  mpts.promptStyle
-0000eb10: 322c 2064 6566 6175 6c74 3d22 7965 7322  2, default="yes"
-0000eb20: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000eb30: 2063 6f6e 6669 726d 6174 696f 6e2e 6c6f   confirmation.lo
-0000eb40: 7765 7228 2920 696e 2028 2279 222c 2022  wer() in ("y", "
-0000eb50: 7965 7322 293a 0a20 2020 2020 2020 2020  yes"):.         
-0000eb60: 2020 2020 2020 206d 656d 6f72 795f 7374         memory_st
-0000eb70: 6f72 6520 3d20 6f73 2e70 6174 682e 6a6f  ore = os.path.jo
-0000eb80: 696e 2863 6f6e 6669 672e 6c6f 6361 6c53  in(config.localS
-0000eb90: 746f 7261 6765 2c20 226d 656d 6f72 7922  torage, "memory"
-0000eba0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000ebb0: 2020 7265 7472 6965 7665 645f 636f 6c6c    retrieved_coll
-0000ebc0: 6563 7469 6f6e 7320 3d20 6f73 2e70 6174  ections = os.pat
-0000ebd0: 682e 6a6f 696e 2863 6f6e 6669 672e 6c6f  h.join(config.lo
-0000ebe0: 6361 6c53 746f 7261 6765 2c20 2261 7574  calStorage, "aut
-0000ebf0: 6f67 656e 222c 2022 7265 7472 6965 7665  ogen", "retrieve
-0000ec00: 7222 290a 2020 2020 2020 2020 2020 2020  r").            
-0000ec10: 2020 2020 666f 7220 666f 6c64 6572 2069      for folder i
-0000ec20: 6e20 286d 656d 6f72 795f 7374 6f72 652c  n (memory_store,
-0000ec30: 2072 6574 7269 6576 6564 5f63 6f6c 6c65   retrieved_colle
-0000ec40: 6374 696f 6e73 293a 0a20 2020 2020 2020  ctions):.       
-0000ec50: 2020 2020 2020 2020 2020 2020 2073 6875               shu
-0000ec60: 7469 6c2e 726d 7472 6565 2866 6f6c 6465  til.rmtree(folde
-0000ec70: 722c 2069 676e 6f72 655f 6572 726f 7273  r, ignore_errors
-0000ec80: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-0000ec90: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000eca0: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
-0000ecb0: 6622 446f 2079 6f75 2077 616e 7420 746f  f"Do you want to
-0000ecc0: 2063 6861 6e67 6520 6261 636b 2074 6865   change back the
-0000ecd0: 2065 6d62 6564 6469 6e67 206d 6f64 656c   embedding model
-0000ece0: 2066 726f 6d20 277b 636f 6e66 6967 2e65   from '{config.e
-0000ecf0: 6d62 6564 6469 6e67 4d6f 6465 6c7d 2720  mbeddingModel}' 
-0000ed00: 746f 2027 7b6f 6c64 456d 6265 6464 696e  to '{oldEmbeddin
-0000ed10: 674d 6f64 656c 7d27 3f20 5b79 5d65 7320  gModel}'? [y]es 
-0000ed20: 2f20 5b4e 5d6f 2229 0a20 2020 2020 2020  / [N]o").       
-0000ed30: 2020 2020 2020 2020 2063 6f6e 6669 726d           confirm
-0000ed40: 6174 696f 6e20 3d20 7365 6c66 2e70 726f  ation = self.pro
-0000ed50: 6d70 7473 2e73 696d 706c 6550 726f 6d70  mpts.simplePromp
-0000ed60: 7428 7374 796c 653d 7365 6c66 2e70 726f  t(style=self.pro
-0000ed70: 6d70 7473 2e70 726f 6d70 7453 7479 6c65  mpts.promptStyle
-0000ed80: 322c 2064 6566 6175 6c74 3d22 7965 7322  2, default="yes"
-0000ed90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000eda0: 2020 6966 206e 6f74 2063 6f6e 6669 726d    if not confirm
-0000edb0: 6174 696f 6e2e 6c6f 7765 7228 2920 696e  ation.lower() in
-0000edc0: 2028 2279 222c 2022 7965 7322 293a 0a20   ("y", "yes"):. 
-0000edd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ede0: 2020 2063 6f6e 6669 672e 656d 6265 6464     config.embedd
-0000edf0: 696e 674d 6f64 656c 203d 206f 6c64 456d  ingModel = oldEm
-0000ee00: 6265 6464 696e 674d 6f64 656c 0a20 2020  beddingModel.   
-0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee20: 2070 7269 6e74 3328 6622 456d 6265 6464   print3(f"Embedd
-0000ee30: 696e 6720 6d6f 6465 6c3a 207b 6f6c 6445  ing model: {oldE
-0000ee40: 6d62 6564 6469 6e67 4d6f 6465 6c7d 2229  mbeddingModel}")
-0000ee50: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000ee60: 6f6c 6445 6d62 6564 6469 6e67 4d6f 6465  oldEmbeddingMode
-0000ee70: 6c20 3d3d 2063 6f6e 6669 672e 656d 6265  l == config.embe
-0000ee80: 6464 696e 674d 6f64 656c 3a0a 2020 2020  ddingModel:.    
-0000ee90: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
-0000eea0: 6176 6543 6f6e 6669 6728 290a 0a20 2020  aveConfig()..   
-0000eeb0: 2064 6566 2073 6574 4175 746f 4765 6e42   def setAutoGenB
-0000eec0: 7569 6c64 6572 436f 6e66 6967 2873 656c  uilderConfig(sel
-0000eed0: 6629 3a0a 2020 2020 2020 2020 6966 206e  f):.        if n
-0000eee0: 6f74 2063 6f6e 6669 672e 6973 5465 726d  ot config.isTerm
-0000eef0: 7578 3a0a 2020 2020 2020 2020 2020 2020  ux:.            
-0000ef00: 4175 746f 4765 6e42 7569 6c64 6572 2829  AutoGenBuilder()
-0000ef10: 2e70 726f 6d70 7443 6f6e 6669 6728 290a  .promptConfig().
-0000ef20: 0a20 2020 2064 6566 2073 6574 4173 7369  .    def setAssi
-0000ef30: 7374 616e 744e 616d 6528 7365 6c66 293a  stantName(self):
-0000ef40: 0a20 2020 2020 2020 2070 7269 6e74 3128  .        print1(
-0000ef50: 2259 6f75 206d 6179 206d 6f64 6966 7920  "You may modify 
-0000ef60: 6d79 206e 616d 6520 6265 6c6f 773a 2229  my name below:")
-0000ef70: 0a20 2020 2020 2020 2066 7265 6547 656e  .        freeGen
-0000ef80: 6975 7341 494e 616d 6520 3d20 7365 6c66  iusAIName = self
-0000ef90: 2e70 726f 6d70 7473 2e73 696d 706c 6550  .prompts.simpleP
-0000efa0: 726f 6d70 7428 7374 796c 653d 7365 6c66  rompt(style=self
-0000efb0: 2e70 726f 6d70 7473 2e70 726f 6d70 7453  .prompts.promptS
-0000efc0: 7479 6c65 322c 2064 6566 6175 6c74 3d63  tyle2, default=c
-0000efd0: 6f6e 6669 672e 6672 6565 4765 6e69 7573  onfig.freeGenius
-0000efe0: 4149 4e61 6d65 290a 2020 2020 2020 2020  AIName).        
-0000eff0: 6966 2066 7265 6547 656e 6975 7341 494e  if freeGeniusAIN
-0000f000: 616d 6520 616e 6420 6e6f 7420 6672 6565  ame and not free
-0000f010: 4765 6e69 7573 4149 4e61 6d65 2e73 7472  GeniusAIName.str
-0000f020: 6970 2829 2e6c 6f77 6572 2829 203d 3d20  ip().lower() == 
-0000f030: 636f 6e66 6967 2e65 7869 745f 656e 7472  config.exit_entr
-0000f040: 793a 0a20 2020 2020 2020 2020 2020 2063  y:.            c
-0000f050: 6f6e 6669 672e 6672 6565 4765 6e69 7573  onfig.freeGenius
-0000f060: 4149 4e61 6d65 203d 2066 7265 6547 656e  AIName = freeGen
-0000f070: 6975 7341 494e 616d 650a 2020 2020 2020  iusAIName.      
-0000f080: 2020 2020 2020 636f 6e66 6967 2e6c 6f63        config.loc
-0000f090: 616c 5374 6f72 6167 6520 3d20 6765 744c  alStorage = getL
-0000f0a0: 6f63 616c 5374 6f72 6167 6528 290a 2020  ocalStorage().  
-0000f0b0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0000f0c0: 2e73 6176 6543 6f6e 6669 6728 290a 2020  .saveConfig().  
-0000f0d0: 2020 2020 2020 2020 2020 7072 696e 7433            print3
-0000f0e0: 2866 2259 6f75 2068 6176 6520 6368 616e  (f"You have chan
-0000f0f0: 6765 6420 6d79 206e 616d 6520 746f 3a20  ged my name to: 
-0000f100: 7b63 6f6e 6669 672e 6672 6565 4765 6e69  {config.freeGeni
-0000f110: 7573 4149 4e61 6d65 7d22 290a 0a20 2020  usAIName}")..   
-0000f120: 2064 6566 2073 6574 4375 7374 6f6d 5379   def setCustomSy
-0000f130: 7374 656d 4d65 7373 6167 6528 7365 6c66  stemMessage(self
-0000f140: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
-0000f150: 3128 2259 6f75 2063 616e 206d 6f64 6966  1("You can modif
-0000f160: 7920 7468 6520 7379 7374 656d 206d 6573  y the system mes
-0000f170: 7361 6765 2074 6f20 6675 726e 6973 6820  sage to furnish 
-0000f180: 6d65 2077 6974 6820 6465 7461 696c 7320  me with details 
-0000f190: 6162 6f75 7420 6d79 2063 6170 6162 696c  about my capabil
-0000f1a0: 6974 6965 732c 2063 6f6e 7374 7261 696e  ities, constrain
-0000f1b0: 7473 2c20 6f72 2061 6e79 2070 6572 7469  ts, or any perti
-0000f1c0: 6e65 6e74 2063 6f6e 7465 7874 2074 6861  nent context tha
-0000f1d0: 7420 6d61 7920 696e 666f 726d 206f 7572  t may inform our
-0000f1e0: 2069 6e74 6572 6163 7469 6f6e 732e 2054   interactions. T
-0000f1f0: 6869 7320 7769 6c6c 2067 7569 6465 206d  his will guide m
-0000f200: 6520 696e 206d 616e 6167 696e 6720 616e  e in managing an
-0000f210: 6420 7265 7370 6f6e 6469 6e67 2074 6f20  d responding to 
-0000f220: 796f 7572 2072 6571 7565 7374 7320 6170  your requests ap
-0000f230: 7072 6f70 7269 6174 656c 792e 2229 0a20  propriately."). 
-0000f240: 2020 2020 2020 2070 7269 6e74 3128 2250         print1("P
-0000f250: 6c65 6173 6520 6e6f 7465 2074 6861 7420  lease note that 
-0000f260: 616c 7465 7269 6e67 206d 7920 7379 7374  altering my syst
-0000f270: 656d 206d 6573 7361 6765 2064 6972 6563  em message direc
-0000f280: 746c 7920 6166 6665 6374 7320 6d79 2066  tly affects my f
-0000f290: 756e 6374 696f 6e61 6c69 7479 2e20 4861  unctionality. Ha
-0000f2a0: 6e64 6c65 2077 6974 6820 6361 7265 2e22  ndle with care."
-0000f2b0: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
-0000f2c0: 2822 456e 7465 7220 6375 7374 6f6d 2073  ("Enter custom s
-0000f2d0: 7973 7465 6d20 6d65 7373 6167 6520 6265  ystem message be
-0000f2e0: 6c6f 773a 2229 0a20 2020 2020 2020 2070  low:").        p
-0000f2f0: 7269 6e74 3128 6622 284b 6565 7020 6974  rint1(f"(Keep it
-0000f300: 2062 6c61 6e6b 2074 6f20 7573 6520 7b63   blank to use {c
-0000f310: 6f6e 6669 672e 6672 6565 4765 6e69 7573  onfig.freeGenius
-0000f320: 4149 4e61 6d65 7d20 6465 6661 756c 7420  AIName} default 
-0000f330: 7379 7374 656d 206d 6573 7361 6765 2e29  system message.)
-0000f340: 2229 0a20 2020 2020 2020 206d 6573 7361  ").        messa
-0000f350: 6765 203d 2073 656c 662e 7072 6f6d 7074  ge = self.prompt
-0000f360: 732e 7369 6d70 6c65 5072 6f6d 7074 2873  s.simplePrompt(s
-0000f370: 7479 6c65 3d73 656c 662e 7072 6f6d 7074  tyle=self.prompt
-0000f380: 732e 7072 6f6d 7074 5374 796c 6532 2c20  s.promptStyle2, 
-0000f390: 6465 6661 756c 743d 636f 6e66 6967 2e73  default=config.s
-0000f3a0: 7973 7465 6d4d 6573 7361 6765 5f6c 6574  ystemMessage_let
-0000f3b0: 6d65 646f 6974 290a 2020 2020 2020 2020  medoit).        
-0000f3c0: 6966 206d 6573 7361 6765 2061 6e64 206e  if message and n
-0000f3d0: 6f74 206d 6573 7361 6765 2e73 7472 6970  ot message.strip
-0000f3e0: 2829 2e6c 6f77 6572 2829 203d 3d20 636f  ().lower() == co
-0000f3f0: 6e66 6967 2e65 7869 745f 656e 7472 793a  nfig.exit_entry:
-0000f400: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-0000f410: 6669 672e 7379 7374 656d 4d65 7373 6167  fig.systemMessag
-0000f420: 655f 6c65 746d 6564 6f69 7420 3d20 6d65  e_letmedoit = me
-0000f430: 7373 6167 650a 2020 2020 2020 2020 2020  ssage.          
-0000f440: 2020 636f 6e66 6967 2e73 6176 6543 6f6e    config.saveCon
-0000f450: 6669 6728 290a 2020 2020 2020 2020 2020  fig().          
-0000f460: 2020 7072 696e 7433 2866 2243 7573 746f    print3(f"Custo
-0000f470: 6d20 7379 7374 656d 206d 6573 7361 6765  m system message
-0000f480: 3a20 7b63 6f6e 6669 672e 6672 6565 4765  : {config.freeGe
-0000f490: 6e69 7573 4149 4e61 6d65 7d22 290a 0a20  niusAIName}").. 
-0000f4a0: 2020 2064 6566 2073 6574 4375 7374 6f6d     def setCustom
-0000f4b0: 5465 7874 4564 6974 6f72 2873 656c 6629  TextEditor(self)
-0000f4c0: 3a0a 2020 2020 2020 2020 7072 696e 7431  :.        print1
-0000f4d0: 2822 506c 6561 7365 2073 7065 6369 6679  ("Please specify
-0000f4e0: 2063 7573 746f 6d20 7465 7874 2065 6469   custom text edi
-0000f4f0: 746f 7220 636f 6d6d 616e 6420 6265 6c6f  tor command belo
-0000f500: 773a 2229 0a20 2020 2020 2020 2070 7269  w:").        pri
-0000f510: 6e74 3128 2265 2e67 2e20 276d 6963 726f  nt1("e.g. 'micro
-0000f520: 202d 736f 6674 7772 6170 2074 7275 6520   -softwrap true 
-0000f530: 2d77 6f72 6477 7261 7020 7472 7565 2722  -wordwrap true'"
-0000f540: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
-0000f550: 2822 4c65 6176 6520 6974 2062 6c61 6e6b  ("Leave it blank
-0000f560: 2074 6f20 7573 6520 6f75 7220 6275 696c   to use our buil
-0000f570: 742d 696e 2074 6578 7420 6564 6974 6f72  t-in text editor
-0000f580: 2027 6554 6578 7445 6469 7427 2062 7920   'eTextEdit' by 
-0000f590: 6465 6661 756c 742e 2229 0a20 2020 2020  default.").     
-0000f5a0: 2020 2063 7573 746f 6d54 6578 7445 6469     customTextEdi
-0000f5b0: 746f 7220 3d20 7365 6c66 2e70 726f 6d70  tor = self.promp
-0000f5c0: 7473 2e73 696d 706c 6550 726f 6d70 7428  ts.simplePrompt(
-0000f5d0: 7374 796c 653d 7365 6c66 2e70 726f 6d70  style=self.promp
-0000f5e0: 7473 2e70 726f 6d70 7453 7479 6c65 322c  ts.promptStyle2,
-0000f5f0: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
-0000f600: 6375 7374 6f6d 5465 7874 4564 6974 6f72  customTextEditor
-0000f610: 290a 2020 2020 2020 2020 6966 2063 7573  ).        if cus
-0000f620: 746f 6d54 6578 7445 6469 746f 7220 616e  tomTextEditor an
-0000f630: 6420 6e6f 7420 6375 7374 6f6d 5465 7874  d not customText
-0000f640: 4564 6974 6f72 2e73 7472 6970 2829 2e6c  Editor.strip().l
-0000f650: 6f77 6572 2829 203d 3d20 636f 6e66 6967  ower() == config
-0000f660: 2e65 7869 745f 656e 7472 793a 0a20 2020  .exit_entry:.   
-0000f670: 2020 2020 2020 2020 2074 6578 7445 6469           textEdi
-0000f680: 746f 7220 3d20 7265 2e73 7562 2822 202e  tor = re.sub(" .
-0000f690: 2a3f 2422 2c20 2222 2c20 6375 7374 6f6d  *?$", "", custom
-0000f6a0: 5465 7874 4564 6974 6f72 290a 2020 2020  TextEditor).    
-0000f6b0: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
-0000f6c0: 6578 7445 6469 746f 7220 6f72 206e 6f74  extEditor or not
-0000f6d0: 2069 7343 6f6d 6d61 6e64 496e 7374 616c   isCommandInstal
-0000f6e0: 6c65 6428 7465 7874 4564 6974 6f72 293a  led(textEditor):
-0000f6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f700: 2070 7269 6e74 3228 2243 6f6d 6d61 6e64   print2("Command
-0000f710: 206e 6f74 2066 6f75 6e64 206f 6e20 796f   not found on yo
-0000f720: 7572 2064 6576 6963 6521 2229 0a20 2020  ur device!").   
-0000f730: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000f740: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000f750: 6f6e 6669 672e 6375 7374 6f6d 5465 7874  onfig.customText
-0000f760: 4564 6974 6f72 203d 2063 7573 746f 6d54  Editor = customT
-0000f770: 6578 7445 6469 746f 720a 2020 2020 2020  extEditor.      
-0000f780: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0000f790: 2e73 6176 6543 6f6e 6669 6728 290a 2020  .saveConfig().  
-0000f7a0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-0000f7b0: 696e 7433 2866 2243 7573 746f 6d20 7465  int3(f"Custom te
-0000f7c0: 7874 2065 6469 746f 723a 207b 636f 6e66  xt editor: {conf
-0000f7d0: 6967 2e63 7573 746f 6d54 6578 7445 6469  ig.customTextEdi
-0000f7e0: 746f 727d 2229 0a0a 2020 2020 6465 6620  tor}")..    def 
-0000f7f0: 7365 7443 6861 7452 6563 6f72 6443 6c6f  setChatRecordClo
-0000f800: 7365 7374 4d61 7463 6865 7328 7365 6c66  sestMatches(self
-0000f810: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
-0000f820: 3128 2250 6c65 6173 6520 7370 6563 6966  1("Please specif
-0000f830: 7920 7468 6520 6e75 6d62 6572 206f 6620  y the number of 
-0000f840: 636c 6f73 6573 7420 6d61 7463 6865 7320  closest matches 
-0000f850: 696e 2065 6163 6820 6d65 6d6f 7279 2072  in each memory r
-0000f860: 6574 7269 6576 616c 3a22 290a 2020 2020  etrieval:").    
-0000f870: 2020 2020 6368 6174 5265 636f 7264 436c      chatRecordCl
-0000f880: 6f73 6573 744d 6174 6368 6573 203d 2073  osestMatches = s
-0000f890: 656c 662e 7072 6f6d 7074 732e 7369 6d70  elf.prompts.simp
-0000f8a0: 6c65 5072 6f6d 7074 2873 7479 6c65 3d73  lePrompt(style=s
-0000f8b0: 656c 662e 7072 6f6d 7074 732e 7072 6f6d  elf.prompts.prom
-0000f8c0: 7074 5374 796c 6532 2c20 6e75 6d62 6572  ptStyle2, number
-0000f8d0: 4f6e 6c79 3d54 7275 652c 2064 6566 6175  Only=True, defau
-0000f8e0: 6c74 3d73 7472 2863 6f6e 6669 672e 6368  lt=str(config.ch
-0000f8f0: 6174 5265 636f 7264 436c 6f73 6573 744d  atRecordClosestM
-0000f900: 6174 6368 6573 2929 0a20 2020 2020 2020  atches)).       
-0000f910: 2069 6620 6368 6174 5265 636f 7264 436c   if chatRecordCl
-0000f920: 6f73 6573 744d 6174 6368 6573 2061 6e64  osestMatches and
-0000f930: 206e 6f74 2063 6861 7452 6563 6f72 6443   not chatRecordC
-0000f940: 6c6f 7365 7374 4d61 7463 6865 732e 7374  losestMatches.st
-0000f950: 7269 7028 292e 6c6f 7765 7228 2920 3d3d  rip().lower() ==
-0000f960: 2063 6f6e 6669 672e 6578 6974 5f65 6e74   config.exit_ent
-0000f970: 7279 2061 6e64 2069 6e74 2863 6861 7452  ry and int(chatR
-0000f980: 6563 6f72 6443 6c6f 7365 7374 4d61 7463  ecordClosestMatc
-0000f990: 6865 7329 203e 3d20 303a 0a20 2020 2020  hes) >= 0:.     
-0000f9a0: 2020 2020 2020 2063 6f6e 6669 672e 6368         config.ch
-0000f9b0: 6174 5265 636f 7264 436c 6f73 6573 744d  atRecordClosestM
-0000f9c0: 6174 6368 6573 203d 2069 6e74 2863 6861  atches = int(cha
-0000f9d0: 7452 6563 6f72 6443 6c6f 7365 7374 4d61  tRecordClosestMa
-0000f9e0: 7463 6865 7329 0a20 2020 2020 2020 2020  tches).         
-0000f9f0: 2020 2063 6f6e 6669 672e 7361 7665 436f     config.saveCo
-0000fa00: 6e66 6967 2829 0a20 2020 2020 2020 2020  nfig().         
-0000fa10: 2020 2070 7269 6e74 3328 6622 4e75 6d62     print3(f"Numb
-0000fa20: 6572 206f 6620 6d65 6d6f 7279 2063 6c6f  er of memory clo
-0000fa30: 7365 7374 206d 6174 6368 6573 3a20 7b63  sest matches: {c
-0000fa40: 6f6e 6669 672e 6368 6174 5265 636f 7264  onfig.chatRecord
-0000fa50: 436c 6f73 6573 744d 6174 6368 6573 7d22  ClosestMatches}"
-0000fa60: 290a 0a20 2020 2064 6566 2073 6574 4d65  )..    def setMe
-0000fa70: 6d6f 7279 436c 6f73 6573 744d 6174 6368  moryClosestMatch
-0000fa80: 6573 2873 656c 6629 3a0a 2020 2020 2020  es(self):.      
-0000fa90: 2020 7072 696e 7431 2822 506c 6561 7365    print1("Please
-0000faa0: 2073 7065 6369 6679 2074 6865 206e 756d   specify the num
-0000fab0: 6265 7220 6f66 2063 6c6f 7365 7374 206d  ber of closest m
-0000fac0: 6174 6368 6573 2069 6e20 6561 6368 206d  atches in each m
-0000fad0: 656d 6f72 7920 7265 7472 6965 7661 6c3a  emory retrieval:
-0000fae0: 2229 0a20 2020 2020 2020 206d 656d 6f72  ").        memor
-0000faf0: 7943 6c6f 7365 7374 4d61 7463 6865 7320  yClosestMatches 
-0000fb00: 3d20 7365 6c66 2e70 726f 6d70 7473 2e73  = self.prompts.s
-0000fb10: 696d 706c 6550 726f 6d70 7428 7374 796c  implePrompt(styl
-0000fb20: 653d 7365 6c66 2e70 726f 6d70 7473 2e70  e=self.prompts.p
-0000fb30: 726f 6d70 7453 7479 6c65 322c 206e 756d  romptStyle2, num
-0000fb40: 6265 724f 6e6c 793d 5472 7565 2c20 6465  berOnly=True, de
-0000fb50: 6661 756c 743d 7374 7228 636f 6e66 6967  fault=str(config
-0000fb60: 2e6d 656d 6f72 7943 6c6f 7365 7374 4d61  .memoryClosestMa
-0000fb70: 7463 6865 7329 290a 2020 2020 2020 2020  tches)).        
-0000fb80: 6966 206d 656d 6f72 7943 6c6f 7365 7374  if memoryClosest
-0000fb90: 4d61 7463 6865 7320 616e 6420 6e6f 7420  Matches and not 
-0000fba0: 6d65 6d6f 7279 436c 6f73 6573 744d 6174  memoryClosestMat
-0000fbb0: 6368 6573 2e73 7472 6970 2829 2e6c 6f77  ches.strip().low
-0000fbc0: 6572 2829 203d 3d20 636f 6e66 6967 2e65  er() == config.e
-0000fbd0: 7869 745f 656e 7472 7920 616e 6420 696e  xit_entry and in
-0000fbe0: 7428 6d65 6d6f 7279 436c 6f73 6573 744d  t(memoryClosestM
-0000fbf0: 6174 6368 6573 2920 3e3d 2030 3a0a 2020  atches) >= 0:.  
-0000fc00: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0000fc10: 2e6d 656d 6f72 7943 6c6f 7365 7374 4d61  .memoryClosestMa
-0000fc20: 7463 6865 7320 3d20 696e 7428 6d65 6d6f  tches = int(memo
-0000fc30: 7279 436c 6f73 6573 744d 6174 6368 6573  ryClosestMatches
-0000fc40: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
-0000fc50: 6e66 6967 2e73 6176 6543 6f6e 6669 6728  nfig.saveConfig(
-0000fc60: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-0000fc70: 696e 7433 2866 224e 756d 6265 7220 6f66  int3(f"Number of
-0000fc80: 206d 656d 6f72 7920 636c 6f73 6573 7420   memory closest 
-0000fc90: 6d61 7463 6865 733a 207b 636f 6e66 6967  matches: {config
-0000fca0: 2e6d 656d 6f72 7943 6c6f 7365 7374 4d61  .memoryClosestMa
-0000fcb0: 7463 6865 737d 2229 0a0a 2020 2020 6465  tches}")..    de
-0000fcc0: 6620 7365 744d 6178 4175 746f 436f 7272  f setMaxAutoCorr
-0000fcd0: 6563 7428 7365 6c66 293a 0a20 2020 2020  ect(self):.     
-0000fce0: 2020 2070 7269 6e74 3128 6622 5468 6520     print1(f"The 
-0000fcf0: 6175 746f 2d63 6f72 7265 6374 696f 6e20  auto-correction 
-0000fd00: 6665 6174 7572 6520 656e 6162 6c65 7320  feature enables 
-0000fd10: 7b63 6f6e 6669 672e 6672 6565 4765 6e69  {config.freeGeni
-0000fd20: 7573 4149 4e61 6d65 7d20 746f 2061 7574  usAIName} to aut
-0000fd30: 6f6d 6174 6963 616c 6c79 2066 6978 2062  omatically fix b
-0000fd40: 726f 6b65 6e20 5079 7468 6f6e 2063 6f64  roken Python cod
-0000fd50: 6520 6966 2069 7420 7761 7320 6e6f 7420  e if it was not 
-0000fd60: 6578 6563 7574 6564 2070 726f 7065 726c  executed properl
-0000fd70: 792e 2229 0a20 2020 2020 2020 2070 7269  y.").        pri
-0000fd80: 6e74 3128 2250 6c65 6173 6520 7370 6563  nt1("Please spec
-0000fd90: 6966 7920 6d61 7869 6d75 6d20 6e75 6d62  ify maximum numb
-0000fda0: 6572 206f 6620 6175 746f 2d63 6f72 7265  er of auto-corre
-0000fdb0: 6374 696f 6e20 6174 7465 6d70 7473 2062  ction attempts b
-0000fdc0: 656c 6f77 3a22 290a 2020 2020 2020 2020  elow:").        
-0000fdd0: 7072 696e 7431 2822 2852 656d 6172 6b73  print1("(Remarks
-0000fde0: 3a20 456e 7465 7220 2730 2720 6966 2079  : Enter '0' if y
-0000fdf0: 6f75 2077 616e 7420 746f 2064 6973 6162  ou want to disab
-0000fe00: 6c65 2061 7574 6f2d 636f 7272 6563 7469  le auto-correcti
-0000fe10: 6f6e 2066 6561 7475 7265 2922 290a 2020  on feature)").  
-0000fe20: 2020 2020 2020 6d61 7841 7574 6f43 6f72        maxAutoCor
-0000fe30: 7265 6374 203d 2073 656c 662e 7072 6f6d  rect = self.prom
-0000fe40: 7074 732e 7369 6d70 6c65 5072 6f6d 7074  pts.simplePrompt
-0000fe50: 2873 7479 6c65 3d73 656c 662e 7072 6f6d  (style=self.prom
-0000fe60: 7074 732e 7072 6f6d 7074 5374 796c 6532  pts.promptStyle2
-0000fe70: 2c20 6e75 6d62 6572 4f6e 6c79 3d54 7275  , numberOnly=Tru
-0000fe80: 652c 2064 6566 6175 6c74 3d73 7472 2863  e, default=str(c
-0000fe90: 6f6e 6669 672e 6d61 785f 636f 6e73 6563  onfig.max_consec
-0000fea0: 7574 6976 655f 6175 746f 5f63 6f72 7265  utive_auto_corre
-0000feb0: 6374 696f 6e29 290a 2020 2020 2020 2020  ction)).        
-0000fec0: 6966 206d 6178 4175 746f 436f 7272 6563  if maxAutoCorrec
-0000fed0: 7420 616e 6420 6e6f 7420 6d61 7841 7574  t and not maxAut
-0000fee0: 6f43 6f72 7265 6374 2e73 7472 6970 2829  oCorrect.strip()
-0000fef0: 2e6c 6f77 6572 2829 203d 3d20 636f 6e66  .lower() == conf
-0000ff00: 6967 2e65 7869 745f 656e 7472 7920 616e  ig.exit_entry an
-0000ff10: 6420 696e 7428 6d61 7841 7574 6f43 6f72  d int(maxAutoCor
-0000ff20: 7265 6374 2920 3e3d 2030 3a0a 2020 2020  rect) >= 0:.    
-0000ff30: 2020 2020 2020 2020 636f 6e66 6967 2e6d          config.m
-0000ff40: 6178 5f63 6f6e 7365 6375 7469 7665 5f61  ax_consecutive_a
-0000ff50: 7574 6f5f 636f 7272 6563 7469 6f6e 203d  uto_correction =
-0000ff60: 2069 6e74 286d 6178 4175 746f 436f 7272   int(maxAutoCorr
-0000ff70: 6563 7429 0a20 2020 2020 2020 2020 2020  ect).           
-0000ff80: 2063 6f6e 6669 672e 7361 7665 436f 6e66   config.saveConf
-0000ff90: 6967 2829 0a20 2020 2020 2020 2020 2020  ig().           
-0000ffa0: 2070 7269 6e74 3328 6622 4d61 7869 6d75   print3(f"Maximu
-0000ffb0: 6d20 636f 6e73 6563 7574 6976 6520 6175  m consecutive au
-0000ffc0: 746f 2d63 6f72 7265 6374 696f 6e3a 207b  to-correction: {
-0000ffd0: 636f 6e66 6967 2e6d 6178 5f63 6f6e 7365  config.max_conse
-0000ffe0: 6375 7469 7665 5f61 7574 6f5f 636f 7272  cutive_auto_corr
-0000fff0: 6563 7469 6f6e 7d22 290a 0a20 2020 2064  ection}")..    d
-00010000: 6566 2073 6574 4d69 6e54 6f6b 656e 7328  ef setMinTokens(
-00010010: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
-00010020: 7269 6e74 3128 2250 6c65 6173 6520 7370  rint1("Please sp
-00010030: 6563 6966 7920 6d69 6e69 6d75 6d20 6f75  ecify minimum ou
-00010040: 7470 7574 2074 6f6b 656e 7320 6265 6c6f  tput tokens belo
-00010050: 773a 2229 0a20 2020 2020 2020 2070 7269  w:").        pri
-00010060: 6e74 3128 2228 6170 706c 6963 6162 6c65  nt1("(applicable
-00010070: 2074 6f20 2763 6861 7467 7074 2720 616e   to 'chatgpt' an
-00010080: 6420 276c 6574 6d65 646f 6974 2720 696e  d 'letmedoit' in
-00010090: 7465 7266 6163 6573 206f 6e6c 7929 2229  terfaces only)")
-000100a0: 0a20 2020 2020 2020 206d 696e 746f 6b65  .        mintoke
-000100b0: 6e73 203d 2073 656c 662e 7072 6f6d 7074  ns = self.prompt
-000100c0: 732e 7369 6d70 6c65 5072 6f6d 7074 2873  s.simplePrompt(s
-000100d0: 7479 6c65 3d73 656c 662e 7072 6f6d 7074  tyle=self.prompt
-000100e0: 732e 7072 6f6d 7074 5374 796c 6532 2c20  s.promptStyle2, 
-000100f0: 6e75 6d62 6572 4f6e 6c79 3d54 7275 652c  numberOnly=True,
-00010100: 2064 6566 6175 6c74 3d73 7472 2863 6f6e   default=str(con
-00010110: 6669 672e 6368 6174 4750 5441 7069 4d69  fig.chatGPTApiMi
-00010120: 6e54 6f6b 656e 7329 290a 2020 2020 2020  nTokens)).      
-00010130: 2020 6966 206d 696e 746f 6b65 6e73 2061    if mintokens a
-00010140: 6e64 206e 6f74 206d 696e 746f 6b65 6e73  nd not mintokens
-00010150: 2e73 7472 6970 2829 2e6c 6f77 6572 2829  .strip().lower()
-00010160: 203d 3d20 636f 6e66 6967 2e65 7869 745f   == config.exit_
-00010170: 656e 7472 7920 616e 6420 696e 7428 6d69  entry and int(mi
-00010180: 6e74 6f6b 656e 7329 203e 2030 3a0a 2020  ntokens) > 0:.  
-00010190: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-000101a0: 2e63 6861 7447 5054 4170 694d 696e 546f  .chatGPTApiMinTo
-000101b0: 6b65 6e73 203d 2069 6e74 286d 696e 746f  kens = int(minto
-000101c0: 6b65 6e73 290a 2020 2020 2020 2020 2020  kens).          
-000101d0: 2020 6966 2063 6f6e 6669 672e 6368 6174    if config.chat
-000101e0: 4750 5441 7069 4d69 6e54 6f6b 656e 7320  GPTApiMinTokens 
-000101f0: 3e20 636f 6e66 6967 2e63 6861 7447 5054  > config.chatGPT
-00010200: 4170 694d 6178 546f 6b65 6e73 3a0a 2020  ApiMaxTokens:.  
-00010210: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00010220: 6e66 6967 2e63 6861 7447 5054 4170 694d  nfig.chatGPTApiM
-00010230: 696e 546f 6b65 6e73 203d 2063 6f6e 6669  inTokens = confi
-00010240: 672e 6368 6174 4750 5441 7069 4d61 7854  g.chatGPTApiMaxT
-00010250: 6f6b 656e 730a 2020 2020 2020 2020 2020  okens.          
-00010260: 2020 636f 6e66 6967 2e73 6176 6543 6f6e    config.saveCon
-00010270: 6669 6728 290a 2020 2020 2020 2020 2020  fig().          
-00010280: 2020 7072 696e 7433 2866 224d 696e 696d    print3(f"Minim
-00010290: 756d 206f 7574 7075 7420 746f 6b65 6e73  um output tokens
-000102a0: 3a20 7b63 6f6e 6669 672e 6368 6174 4750  : {config.chatGP
-000102b0: 5441 7069 4d69 6e54 6f6b 656e 737d 2229  TApiMinTokens}")
-000102c0: 0a0a 2020 2020 6465 6620 6765 744d 6178  ..    def getMax
-000102d0: 546f 6b65 6e73 2873 656c 6629 3a0a 2020  Tokens(self):.  
-000102e0: 2020 2020 2020 636f 6e74 6578 7457 696e        contextWin
-000102f0: 646f 774c 696d 6974 203d 2074 6f6b 656e  dowLimit = token
-00010300: 4c69 6d69 7473 5b63 6f6e 6669 672e 6368  Limits[config.ch
-00010310: 6174 4750 5441 7069 4d6f 6465 6c5d 0a20  atGPTApiModel]. 
-00010320: 2020 2020 2020 2066 756e 6374 696f 6e54         functionT
-00010330: 6f6b 656e 7320 3d20 636f 756e 745f 746f  okens = count_to
-00010340: 6b65 6e73 5f66 726f 6d5f 6675 6e63 7469  kens_from_functi
-00010350: 6f6e 7328 636f 6e66 6967 2e74 6f6f 6c46  ons(config.toolF
-00010360: 756e 6374 696f 6e53 6368 656d 6173 2e76  unctionSchemas.v
-00010370: 616c 7565 7328 2929 0a20 2020 2020 2020  alues()).       
-00010380: 206d 6178 546f 6b65 6e20 3d20 636f 6e74   maxToken = cont
-00010390: 6578 7457 696e 646f 774c 696d 6974 202d  extWindowLimit -
-000103a0: 2066 756e 6374 696f 6e54 6f6b 656e 7320   functionTokens 
-000103b0: 2d20 636f 6e66 6967 2e63 6861 7447 5054  - config.chatGPT
-000103c0: 4170 694d 696e 546f 6b65 6e73 0a20 2020  ApiMinTokens.   
-000103d0: 2020 2020 2069 6620 6d61 7854 6f6b 656e       if maxToken
-000103e0: 203e 2034 3039 3620 616e 6420 636f 6e66   > 4096 and conf
-000103f0: 6967 2e63 6861 7447 5054 4170 694d 6f64  ig.chatGPTApiMod
-00010400: 656c 2069 6e20 280a 2020 2020 2020 2020  el in (.        
-00010410: 2020 2020 2267 7074 2d34 2d74 7572 626f      "gpt-4-turbo
-00010420: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00010430: 6770 742d 342d 7475 7262 6f2d 7072 6576  gpt-4-turbo-prev
-00010440: 6965 7722 2c0a 2020 2020 2020 2020 2020  iew",.          
-00010450: 2020 2267 7074 2d34 2d30 3132 352d 7072    "gpt-4-0125-pr
-00010460: 6576 6965 7722 2c0a 2020 2020 2020 2020  eview",.        
-00010470: 2020 2020 2267 7074 2d34 2d31 3130 362d      "gpt-4-1106-
-00010480: 7072 6576 6965 7722 2c0a 2020 2020 2020  preview",.      
-00010490: 2020 2020 2020 2267 7074 2d33 2e35 2d74        "gpt-3.5-t
-000104a0: 7572 626f 222c 0a20 2020 2020 2020 2029  urbo",.        )
-000104b0: 3a0a 2020 2020 2020 2020 2020 2020 6d61  :.            ma
-000104c0: 7854 6f6b 656e 203d 2034 3039 360a 2020  xToken = 4096.  
-000104d0: 2020 2020 2020 7265 7475 726e 2063 6f6e        return con
-000104e0: 7465 7874 5769 6e64 6f77 4c69 6d69 742c  textWindowLimit,
-000104f0: 2066 756e 6374 696f 6e54 6f6b 656e 732c   functionTokens,
-00010500: 206d 6178 546f 6b65 6e0a 0a20 2020 2064   maxToken..    d
-00010510: 6566 2073 6574 4d61 7854 6f6b 656e 735f  ef setMaxTokens_
-00010520: 6e6f 6e5f 6368 6174 6770 7428 7365 6c66  non_chatgpt(self
-00010530: 293a 0a20 2020 2020 2020 2070 7269 6e74  ):.        print
-00010540: 3128 2250 6c65 6173 6520 7370 6563 6966  1("Please specif
-00010550: 7920 6d61 7869 6d75 6d20 6f75 7470 7574  y maximum output
-00010560: 2074 6f6b 656e 7320 6265 6c6f 773a 2229   tokens below:")
-00010570: 0a20 2020 2020 2020 2069 6620 636f 6e66  .        if conf
-00010580: 6967 2e6c 6c6d 496e 7465 7266 6163 6520  ig.llmInterface 
-00010590: 3d3d 2022 6765 6d69 6e69 223a 0a20 2020  == "gemini":.   
-000105a0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-000105b0: 203d 2063 6f6e 6669 672e 6765 6d69 6e69   = config.gemini
-000105c0: 7072 6f5f 6d61 785f 6f75 7470 7574 5f74  pro_max_output_t
-000105d0: 6f6b 656e 730a 2020 2020 2020 2020 656c  okens.        el
-000105e0: 6966 2063 6f6e 6669 672e 6c6c 6d49 6e74  if config.llmInt
-000105f0: 6572 6661 6365 203d 3d20 226c 6c61 6d61  erface == "llama
-00010600: 6370 7022 3a0a 2020 2020 2020 2020 2020  cpp":.          
-00010610: 2020 6465 6661 756c 7420 3d20 636f 6e66    default = conf
-00010620: 6967 2e6c 6c61 6d61 6370 704d 6169 6e4d  ig.llamacppMainM
-00010630: 6f64 656c 5f6d 6178 5f74 6f6b 656e 730a  odel_max_tokens.
-00010640: 2020 2020 2020 2020 656c 6966 2063 6f6e          elif con
-00010650: 6669 672e 6c6c 6d49 6e74 6572 6661 6365  fig.llmInterface
-00010660: 203d 3d20 226f 6c6c 616d 6122 3a0a 2020   == "ollama":.  
-00010670: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
-00010680: 7420 3d20 636f 6e66 6967 2e6f 6c6c 616d  t = config.ollam
-00010690: 614d 6169 6e4d 6f64 656c 5f6e 756d 5f70  aMainModel_num_p
-000106a0: 7265 6469 6374 0a20 2020 2020 2020 206d  redict.        m
-000106b0: 6178 746f 6b65 6e73 203d 2073 656c 662e  axtokens = self.
-000106c0: 7072 6f6d 7074 732e 7369 6d70 6c65 5072  prompts.simplePr
-000106d0: 6f6d 7074 2873 7479 6c65 3d73 656c 662e  ompt(style=self.
-000106e0: 7072 6f6d 7074 732e 7072 6f6d 7074 5374  prompts.promptSt
-000106f0: 796c 6532 2c20 6e75 6d62 6572 4f6e 6c79  yle2, numberOnly
-00010700: 3d54 7275 652c 2064 6566 6175 6c74 3d73  =True, default=s
-00010710: 7472 2864 6566 6175 6c74 2929 0a20 2020  tr(default)).   
-00010720: 2020 2020 2069 6620 6d61 7874 6f6b 656e       if maxtoken
-00010730: 7320 616e 6420 6e6f 7420 6d61 7874 6f6b  s and not maxtok
-00010740: 656e 732e 7374 7269 7028 292e 6c6f 7765  ens.strip().lowe
-00010750: 7228 2920 3d3d 2063 6f6e 6669 672e 6578  r() == config.ex
-00010760: 6974 5f65 6e74 7279 2061 6e64 2069 6e74  it_entry and int
-00010770: 286d 6178 746f 6b65 6e73 2920 3e20 303a  (maxtokens) > 0:
-00010780: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
-00010790: 746f 6b65 6e73 203d 2069 6e74 286d 6178  tokens = int(max
-000107a0: 746f 6b65 6e73 290a 2020 2020 2020 2020  tokens).        
-000107b0: 2020 2020 6966 2063 6f6e 6669 672e 6c6c      if config.ll
-000107c0: 6d49 6e74 6572 6661 6365 203d 3d20 2267  mInterface == "g
-000107d0: 656d 696e 6922 3a0a 2020 2020 2020 2020  emini":.        
-000107e0: 2020 2020 2020 2020 636f 6e66 6967 2e67          config.g
-000107f0: 656d 696e 6970 726f 5f6d 6178 5f6f 7574  eminipro_max_out
-00010800: 7075 745f 746f 6b65 6e73 203d 206d 6178  put_tokens = max
-00010810: 746f 6b65 6e73 0a20 2020 2020 2020 2020  tokens.         
-00010820: 2020 2065 6c69 6620 636f 6e66 6967 2e6c     elif config.l
-00010830: 6c6d 496e 7465 7266 6163 6520 3d3d 2022  lmInterface == "
-00010840: 6c6c 616d 6163 7070 223a 0a20 2020 2020  llamacpp":.     
-00010850: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00010860: 672e 6c6c 616d 6163 7070 4d61 696e 4d6f  g.llamacppMainMo
-00010870: 6465 6c5f 6d61 785f 746f 6b65 6e73 203d  del_max_tokens =
-00010880: 206d 6178 746f 6b65 6e73 0a20 2020 2020   maxtokens.     
-00010890: 2020 2020 2020 2065 6c69 6620 636f 6e66         elif conf
-000108a0: 6967 2e6c 6c6d 496e 7465 7266 6163 6520  ig.llmInterface 
-000108b0: 3d3d 2022 6f6c 6c61 6d61 223a 0a20 2020  == "ollama":.   
-000108c0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000108d0: 6669 672e 6f6c 6c61 6d61 4d61 696e 4d6f  fig.ollamaMainMo
-000108e0: 6465 6c5f 6e75 6d5f 7072 6564 6963 7420  del_num_predict 
-000108f0: 3d20 6d61 7874 6f6b 656e 730a 2020 2020  = maxtokens.    
-00010900: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
-00010910: 6176 6543 6f6e 6669 6728 290a 2020 2020  aveConfig().    
-00010920: 2020 2020 2020 2020 7072 696e 7433 2866          print3(f
-00010930: 224d 6178 696d 756d 206f 7574 7075 7420  "Maximum output 
-00010940: 746f 6b65 6e73 3a20 7b63 6f6e 6669 672e  tokens: {config.
-00010950: 6368 6174 4750 5441 7069 4d69 6e54 6f6b  chatGPTApiMinTok
-00010960: 656e 737d 2229 0a0a 2020 2020 6465 6620  ens}")..    def 
-00010970: 7365 744d 6178 546f 6b65 6e73 2873 656c  setMaxTokens(sel
-00010980: 6629 3a0a 2020 2020 2020 2020 2320 6e6f  f):.        # no
-00010990: 6e2d 6368 6174 6770 7420 7365 7474 696e  n-chatgpt settin
-000109a0: 6773 0a20 2020 2020 2020 2069 6620 6e6f  gs.        if no
-000109b0: 7420 636f 6e66 6967 2e6c 6c6d 496e 7465  t config.llmInte
-000109c0: 7266 6163 6520 696e 2028 2263 6861 7467  rface in ("chatg
-000109d0: 7074 222c 2022 6c65 746d 6564 6f69 7422  pt", "letmedoit"
-000109e0: 293a 0a20 2020 2020 2020 2020 2020 2073  ):.            s
-000109f0: 656c 662e 7365 744d 6178 546f 6b65 6e73  elf.setMaxTokens
-00010a00: 5f6e 6f6e 5f63 6861 7467 7074 2829 0a20  _non_chatgpt(). 
-00010a10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010a20: 6e20 4e6f 6e65 0a20 2020 2020 2020 2023  n None.        #
-00010a30: 2063 6861 7467 7074 2073 6574 7469 6e67   chatgpt setting
-00010a40: 730a 2020 2020 2020 2020 636f 6e74 6578  s.        contex
-00010a50: 7457 696e 646f 774c 696d 6974 2c20 6675  tWindowLimit, fu
-00010a60: 6e63 7469 6f6e 546f 6b65 6e73 2c20 746f  nctionTokens, to
-00010a70: 6b65 6e4c 696d 6974 203d 2073 656c 662e  kenLimit = self.
-00010a80: 6765 744d 6178 546f 6b65 6e73 2829 0a20  getMaxTokens(). 
-00010a90: 2020 2020 2020 2069 6620 746f 6b65 6e4c         if tokenL
-00010aa0: 696d 6974 203c 2063 6f6e 6669 672e 6368  imit < config.ch
-00010ab0: 6174 4750 5441 7069 4d69 6e54 6f6b 656e  atGPTApiMinToken
-00010ac0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
-00010ad0: 7269 6e74 3228 6622 4675 6e63 7469 6f6e  rint2(f"Function
-00010ae0: 2074 6f6b 656e 7320 5b7b 6675 6e63 7469   tokens [{functi
-00010af0: 6f6e 546f 6b65 6e73 7d5d 2065 7863 6565  onTokens}] excee
-00010b00: 6420 7b63 6f6e 6669 672e 6368 6174 4750  d {config.chatGP
-00010b10: 5441 7069 4d6f 6465 6c7d 206f 7574 7075  TApiModel} outpu
-00010b20: 7420 746f 6b65 6e20 6c69 6d69 742e 2229  t token limit.")
-00010b30: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00010b40: 6e74 3128 2245 6974 6865 7220 6368 616e  nt1("Either chan
-00010b50: 6765 2074 6f20 6120 6d6f 6465 6c20 7769  ge to a model wi
-00010b60: 7468 2068 6967 6865 7220 746f 6b65 6e20  th higher token 
-00010b70: 6c69 6d69 7420 6f72 2064 6973 6162 6c65  limit or disable
-00010b80: 2075 6e75 7365 6420 6675 6e63 7469 6f6e   unused function
-00010b90: 2d63 616c 6c20 706c 6775 696e 732e 2229  -call plguins.")
-00010ba0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00010bb0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00010bc0: 3128 7365 6c66 2e64 6976 6964 6572 290a  1(self.divider).
-00010bd0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00010be0: 7431 2822 4750 5420 616e 6420 656d 6265  t1("GPT and embe
-00010bf0: 6464 696e 6773 206d 6f64 656c 7320 7072  ddings models pr
-00010c00: 6f63 6573 7320 7465 7874 2069 6e20 6368  ocess text in ch
-00010c10: 756e 6b73 2063 616c 6c65 6420 746f 6b65  unks called toke
-00010c20: 6e73 2e20 4173 2061 2072 6f75 6768 2072  ns. As a rough r
-00010c30: 756c 6520 6f66 2074 6875 6d62 2c20 3120  ule of thumb, 1 
-00010c40: 746f 6b65 6e20 6973 2061 7070 726f 7869  token is approxi
-00010c50: 6d61 7465 6c79 2034 2063 6861 7261 6374  mately 4 charact
-00010c60: 6572 7320 6f72 2030 2e37 3520 776f 7264  ers or 0.75 word
-00010c70: 7320 666f 7220 456e 676c 6973 6820 7465  s for English te
-00010c80: 7874 2e20 4f6e 6520 6c69 6d69 7461 7469  xt. One limitati
-00010c90: 6f6e 2074 6f20 6b65 6570 2069 6e20 6d69  on to keep in mi
-00010ca0: 6e64 2069 7320 7468 6174 2066 6f72 2061  nd is that for a
-00010cb0: 2047 5054 206d 6f64 656c 2074 6865 2070   GPT model the p
-00010cc0: 726f 6d70 7420 616e 6420 7468 6520 6765  rompt and the ge
-00010cd0: 6e65 7261 7465 6420 6f75 7470 7574 2063  nerated output c
-00010ce0: 6f6d 6269 6e65 6420 6d75 7374 2062 6520  ombined must be 
-00010cf0: 6e6f 206d 6f72 6520 7468 616e 2074 6865  no more than the
-00010d00: 206d 6f64 656c 2773 206d 6178 696d 756d   model's maximum
-00010d10: 2063 6f6e 7465 7874 206c 656e 6774 682e   context length.
-00010d20: 2229 0a20 2020 2020 2020 2020 2020 2070  ").            p
-00010d30: 7269 6e74 3328 6622 4375 7272 656e 7420  rint3(f"Current 
-00010d40: 4750 5420 6d6f 6465 6c3a 207b 636f 6e66  GPT model: {conf
-00010d50: 6967 2e63 6861 7447 5054 4170 694d 6f64  ig.chatGPTApiMod
-00010d60: 656c 7d22 290a 2020 2020 2020 2020 2020  el}").          
-00010d70: 2020 7072 696e 7433 2866 224d 6178 696d    print3(f"Maxim
-00010d80: 756d 2063 6f6e 7465 7874 206c 656e 6774  um context lengt
-00010d90: 683a 207b 636f 6e74 6578 7457 696e 646f  h: {contextWindo
-00010da0: 774c 696d 6974 7d22 290a 2020 2020 2020  wLimit}").      
-00010db0: 2020 2020 2020 7072 696e 7433 2866 2243        print3(f"C
-00010dc0: 7572 7265 6e74 2066 756e 6374 696f 6e20  urrent function 
-00010dd0: 746f 6b65 6e73 3a20 7b66 756e 6374 696f  tokens: {functio
-00010de0: 6e54 6f6b 656e 737d 2229 0a20 2020 2020  nTokens}").     
-00010df0: 2020 2020 2020 2070 7269 6e74 3328 6622         print3(f"
-00010e00: 4d61 7869 6d75 6d20 6f75 7470 7574 2074  Maximum output t
-00010e10: 6f6b 656e 2061 6c6c 6f77 6564 2028 6578  oken allowed (ex
-00010e20: 636c 2e20 6675 6e63 7469 6f6e 7329 3a20  cl. functions): 
-00010e30: 7b74 6f6b 656e 4c69 6d69 747d 2229 0a20  {tokenLimit}"). 
-00010e40: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00010e50: 3128 7365 6c66 2e64 6976 6964 6572 290a  1(self.divider).
-00010e60: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00010e70: 7431 2822 506c 6561 7365 2073 7065 6369  t1("Please speci
-00010e80: 6679 206d 6178 696d 756d 206f 7574 7075  fy maximum outpu
-00010e90: 7420 746f 6b65 6e73 2062 656c 6f77 3a22  t tokens below:"
-00010ea0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
-00010eb0: 7874 6f6b 656e 7320 3d20 7365 6c66 2e70  xtokens = self.p
-00010ec0: 726f 6d70 7473 2e73 696d 706c 6550 726f  rompts.simplePro
-00010ed0: 6d70 7428 7374 796c 653d 7365 6c66 2e70  mpt(style=self.p
-00010ee0: 726f 6d70 7473 2e70 726f 6d70 7453 7479  rompts.promptSty
-00010ef0: 6c65 322c 206e 756d 6265 724f 6e6c 793d  le2, numberOnly=
-00010f00: 5472 7565 2c20 6465 6661 756c 743d 7374  True, default=st
-00010f10: 7228 636f 6e66 6967 2e63 6861 7447 5054  r(config.chatGPT
-00010f20: 4170 694d 6178 546f 6b65 6e73 2929 0a20  ApiMaxTokens)). 
-00010f30: 2020 2020 2020 2020 2020 2069 6620 6d61             if ma
-00010f40: 7874 6f6b 656e 7320 616e 6420 6e6f 7420  xtokens and not 
-00010f50: 6d61 7874 6f6b 656e 732e 7374 7269 7028  maxtokens.strip(
-00010f60: 292e 6c6f 7765 7228 2920 3d3d 2063 6f6e  ).lower() == con
-00010f70: 6669 672e 6578 6974 5f65 6e74 7279 2061  fig.exit_entry a
-00010f80: 6e64 2069 6e74 286d 6178 746f 6b65 6e73  nd int(maxtokens
-00010f90: 2920 3e20 303a 0a20 2020 2020 2020 2020  ) > 0:.         
-00010fa0: 2020 2020 2020 2063 6f6e 6669 672e 6368         config.ch
-00010fb0: 6174 4750 5441 7069 4d61 7854 6f6b 656e  atGPTApiMaxToken
-00010fc0: 7320 3d20 696e 7428 6d61 7874 6f6b 656e  s = int(maxtoken
-00010fd0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
-00010fe0: 2020 2069 6620 636f 6e66 6967 2e63 6861     if config.cha
-00010ff0: 7447 5054 4170 694d 6178 546f 6b65 6e73  tGPTApiMaxTokens
-00011000: 203e 2074 6f6b 656e 4c69 6d69 743a 0a20   > tokenLimit:. 
-00011010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011020: 2020 2063 6f6e 6669 672e 6368 6174 4750     config.chatGP
-00011030: 5441 7069 4d61 7854 6f6b 656e 7320 3d20  TApiMaxTokens = 
-00011040: 746f 6b65 6e4c 696d 6974 0a20 2020 2020  tokenLimit.     
-00011050: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00011060: 672e 7361 7665 436f 6e66 6967 2829 0a20  g.saveConfig(). 
-00011070: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00011080: 7269 6e74 3328 6622 4d61 7869 6d75 6d20  rint3(f"Maximum 
-00011090: 6f75 7470 7574 2074 6f6b 656e 733a 207b  output tokens: {
-000110a0: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
-000110b0: 694d 6178 546f 6b65 6e73 7d22 290a 0a20  iMaxTokens}").. 
-000110c0: 2020 2064 6566 2072 756e 5379 7374 656d     def runSystem
-000110d0: 436f 6d6d 616e 6428 7365 6c66 2c20 636f  Command(self, co
-000110e0: 6d6d 616e 6429 3a0a 2020 2020 2020 2020  mmand):.        
-000110f0: 636f 6d6d 616e 6420 3d20 636f 6d6d 616e  command = comman
-00011100: 642e 7374 7269 7028 295b 313a 5d0a 2020  d.strip()[1:].  
-00011110: 2020 2020 2020 6966 2022 5c6e 2220 696e        if "\n" in
-00011120: 2063 6f6d 6d61 6e64 3a0a 2020 2020 2020   command:.      
-00011130: 2020 2020 2020 636f 6d6d 616e 6420 3d20        command = 
-00011140: 223b 222e 6a6f 696e 2863 6f6d 6d61 6e64  ";".join(command
-00011150: 2e73 706c 6974 2822 5c6e 2229 290a 2020  .split("\n")).  
-00011160: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
-00011170: 7468 6973 506c 6174 666f 726d 203d 3d20  thisPlatform == 
-00011180: 2257 696e 646f 7773 223a 0a20 2020 2020  "Windows":.     
-00011190: 2020 2020 2020 206f 732e 7379 7374 656d         os.system
-000111a0: 2863 6f6d 6d61 6e64 290a 2020 2020 2020  (command).      
-000111b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000111c0: 2020 2020 6f73 2e73 7973 7465 6d28 6622      os.system(f"
-000111d0: 656e 7620 5154 5f51 5041 5f50 4c41 5446  env QT_QPA_PLATF
-000111e0: 4f52 4d5f 504c 5547 494e 5f50 4154 483d  ORM_PLUGIN_PATH=
-000111f0: 277b 636f 6e66 6967 2e65 6e76 5f51 545f  '{config.env_QT_
-00011200: 5150 415f 504c 4154 464f 524d 5f50 4c55  QPA_PLATFORM_PLU
-00011210: 4749 4e5f 5041 5448 7d27 207b 636f 6d6d  GIN_PATH}' {comm
-00011220: 616e 647d 2229 0a0a 2020 2020 6465 6620  and}")..    def 
-00011230: 746f 6767 6c65 4d75 6c74 696c 696e 6528  toggleMultiline(
-00011240: 7365 6c66 293a 0a20 2020 2020 2020 2063  self):.        c
-00011250: 6f6e 6669 672e 6d75 6c74 696c 696e 6549  onfig.multilineI
-00011260: 6e70 7574 203d 206e 6f74 2063 6f6e 6669  nput = not confi
-00011270: 672e 6d75 6c74 696c 696e 6549 6e70 7574  g.multilineInput
-00011280: 0a20 2020 2020 2020 2072 756e 5f69 6e5f  .        run_in_
-00011290: 7465 726d 696e 616c 286c 616d 6264 613a  terminal(lambda:
-000112a0: 2070 7269 6e74 3128 6622 4d75 6c74 692d   print1(f"Multi-
-000112b0: 6c69 6e65 2069 6e70 7574 207b 2765 6e61  line input {'ena
-000112c0: 626c 6564 2720 6966 2063 6f6e 6669 672e  bled' if config.
-000112d0: 6d75 6c74 696c 696e 6549 6e70 7574 2065  multilineInput e
-000112e0: 6c73 6520 2764 6973 6162 6c65 6427 7d21  lse 'disabled'}!
-000112f0: 2229 290a 2020 2020 2020 2020 6966 2063  ")).        if c
-00011300: 6f6e 6669 672e 6d75 6c74 696c 696e 6549  onfig.multilineI
-00011310: 6e70 7574 3a0a 2020 2020 2020 2020 2020  nput:.          
-00011320: 2020 7275 6e5f 696e 5f74 6572 6d69 6e61    run_in_termina
-00011330: 6c28 6c61 6d62 6461 3a20 7072 696e 7431  l(lambda: print1
-00011340: 2822 5573 6520 2765 7363 6170 6520 2b20  ("Use 'escape + 
-00011350: 656e 7465 7227 2074 6f20 636f 6d70 6c65  enter' to comple
-00011360: 7465 2079 6f75 7220 656e 7472 792e 2229  te your entry.")
-00011370: 290a 0a20 2020 2064 6566 2069 7354 7473  )..    def isTts
-00011380: 4176 6169 6c61 626c 6528 7365 6c66 293a  Available(self):
-00011390: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-000113a0: 636f 6e66 6967 2e69 7356 6c63 506c 6179  config.isVlcPlay
-000113b0: 6572 496e 7374 616c 6c65 6420 616e 6420  erInstalled and 
-000113c0: 6e6f 7420 636f 6e66 6967 2e69 7350 7967  not config.isPyg
-000113d0: 616d 6549 6e73 7461 6c6c 6564 2061 6e64  ameInstalled and
-000113e0: 206e 6f74 2063 6f6e 6669 672e 7474 7343   not config.ttsC
-000113f0: 6f6d 6d61 6e64 2061 6e64 206e 6f74 2063  ommand and not c
-00011400: 6f6e 6669 672e 656c 6576 656e 6c61 6273  onfig.elevenlabs
-00011410: 4170 693a 0a20 2020 2020 2020 2020 2020  Api:.           
-00011420: 2070 7269 6e74 3228 2254 6578 742d 746f   print2("Text-to
-00011430: 2d73 7065 6563 6820 6665 6174 7572 6520  -speech feature 
-00011440: 6973 206e 6f74 2065 6e61 626c 6564 2122  is not enabled!"
-00011450: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-00011460: 696e 7433 2822 5265 6164 3a20 6874 7470  int3("Read: http
-00011470: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00011480: 6c69 7261 6e77 6f6e 672f 6c65 746d 6564  liranwong/letmed
-00011490: 6f69 742f 7769 6b69 2f6c 6574 4d65 446f  oit/wiki/letMeDo
-000114a0: 4974 2d53 7065 616b 7322 290a 2020 2020  It-Speaks").    
-000114b0: 2020 2020 2020 2020 636f 6e66 6967 2e74          config.t
-000114c0: 7473 203d 2046 616c 7365 0a20 2020 2020  ts = False.     
-000114d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000114e0: 2020 2020 2063 6f6e 6669 672e 7474 7320       config.tts 
-000114f0: 3d20 5472 7565 0a20 2020 2020 2020 2072  = True.        r
-00011500: 6574 7572 6e20 636f 6e66 6967 2e74 7473  eturn config.tts
-00011510: 0a0a 2020 2020 6465 6620 746f 6767 6c65  ..    def toggle
-00011520: 696e 7075 7461 7564 696f 2873 656c 6629  inputaudio(self)
-00011530: 3a0a 2020 2020 2020 2020 6966 2073 656c  :.        if sel
-00011540: 662e 6973 5474 7341 7661 696c 6162 6c65  f.isTtsAvailable
-00011550: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00011560: 6e66 6967 2e74 7473 496e 7075 7420 3d20  nfig.ttsInput = 
-00011570: 6e6f 7420 636f 6e66 6967 2e74 7473 496e  not config.ttsIn
-00011580: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
-00011590: 636f 6e66 6967 2e73 6176 6543 6f6e 6669  config.saveConfi
-000115a0: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
-000115b0: 7072 696e 7433 2866 2249 6e70 7574 2041  print3(f"Input A
-000115c0: 7564 696f 3a20 277b 2765 6e61 626c 6564  udio: '{'enabled
-000115d0: 2720 6966 2063 6f6e 6669 672e 7474 7349  ' if config.ttsI
-000115e0: 6e70 7574 2065 6c73 6520 2764 6973 6162  nput else 'disab
-000115f0: 6c65 6427 7d27 2122 290a 0a20 2020 2064  led'}'!")..    d
-00011600: 6566 2074 6f67 676c 6572 6573 706f 6e73  ef togglerespons
-00011610: 6561 7564 696f 2873 656c 6629 3a0a 2020  eaudio(self):.  
-00011620: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
-00011630: 5474 7341 7661 696c 6162 6c65 3a0a 2020  TtsAvailable:.  
-00011640: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00011650: 2e74 7473 4f75 7470 7574 203d 206e 6f74  .ttsOutput = not
-00011660: 2063 6f6e 6669 672e 7474 734f 7574 7075   config.ttsOutpu
-00011670: 740a 2020 2020 2020 2020 2020 2020 636f  t.            co
-00011680: 6e66 6967 2e73 6176 6543 6f6e 6669 6728  nfig.saveConfig(
-00011690: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
-000116a0: 696e 7433 2866 2252 6573 706f 6e73 6520  int3(f"Response 
-000116b0: 4175 6469 6f3a 2027 7b27 656e 6162 6c65  Audio: '{'enable
-000116c0: 6427 2069 6620 636f 6e66 6967 2e74 7473  d' if config.tts
-000116d0: 4f75 7470 7574 2065 6c73 6520 2764 6973  Output else 'dis
-000116e0: 6162 6c65 6427 7d27 2122 290a 0a20 2020  abled'}'!")..   
-000116f0: 2064 6566 2064 6566 696e 6554 7473 436f   def defineTtsCo
-00011700: 6d6d 616e 6428 7365 6c66 293a 0a20 2020  mmand(self):.   
-00011710: 2020 2020 2070 7269 6e74 3128 2244 6566       print1("Def
-00011720: 696e 6520 6375 7374 6f6d 2074 6578 742d  ine custom text-
-00011730: 746f 2d73 7065 6563 6820 636f 6d6d 616e  to-speech comman
-00011740: 6420 6265 6c6f 773a 2229 0a20 2020 2020  d below:").     
-00011750: 2020 2070 7269 6e74 3128 2222 222a 206f     print1("""* o
-00011760: 6e20 6d61 634f 5320 5b27 7361 7920 2d76  n macOS ['say -v
-00011770: 2022 3f22 2720 746f 2063 6865 636b 2076   "?"' to check v
-00011780: 6f69 6365 735d 2c20 652e 672e 3a5c 6e27  oices], e.g.:\n'
-00011790: 7361 7927 206f 7220 2773 6179 202d 7220  say' or 'say -r 
-000117a0: 3230 3020 2d76 2044 616e 6965 6c27 2222  200 -v Daniel'""
-000117b0: 2229 0a20 2020 2020 2020 2070 7269 6e74  ").        print
-000117c0: 3128 222a 206f 6e20 5562 756e 7475 205b  1("* on Ubuntu [
-000117d0: 2765 7370 6561 6b20 2d2d 766f 6963 6573  'espeak --voices
-000117e0: 2720 746f 2063 6865 636b 2076 6f69 6365  ' to check voice
-000117f0: 735d 2c20 652e 672e 3a5c 6e27 6573 7065  s], e.g.:\n'espe
-00011800: 616b 2720 6f72 2027 6573 7065 616b 202d  ak' or 'espeak -
-00011810: 7320 3137 3520 2d76 2065 6e2d 6762 2722  s 175 -v en-gb'"
-00011820: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
-00011830: 2822 2a20 6f6e 2057 696e 646f 7773 2c20  ("* on Windows, 
-00011840: 7369 6d70 6c79 2065 6e74 6572 2027 7769  simply enter 'wi
-00011850: 6e64 6f77 7327 2068 6572 6520 746f 2075  ndows' here to u
-00011860: 7365 2057 696e 646f 7773 2062 7569 6c74  se Windows built
-00011870: 2d69 6e20 7370 6565 6368 2065 6e67 696e  -in speech engin
-00011880: 6522 2920 2320 6c65 746d 6564 6f69 742e  e") # letmedoit.
-00011890: 6169 2077 696c 6c20 6861 6e64 6c65 2074  ai will handle t
-000118a0: 6865 2063 6f6d 6d61 6e64 2066 6f72 2057  he command for W
-000118b0: 696e 646f 7773 2075 7365 7273 0a20 2020  indows users.   
-000118c0: 2020 2020 2070 7269 6e74 3128 2272 656d       print1("rem
-000118d0: 6172 6b73 3a20 616c 7761 7973 2070 6c61  arks: always pla
-000118e0: 6365 2074 6865 2076 6f69 6365 206f 7074  ce the voice opt
-000118f0: 696f 6e2c 2069 6620 616e 792c 2061 7420  ion, if any, at 
-00011900: 7468 6520 656e 6422 290a 2020 2020 2020  the end").      
-00011910: 2020 7474 7343 6f6d 6d61 6e64 203d 2073    ttsCommand = s
-00011920: 656c 662e 7072 6f6d 7074 732e 7369 6d70  elf.prompts.simp
-00011930: 6c65 5072 6f6d 7074 2873 7479 6c65 3d73  lePrompt(style=s
-00011940: 656c 662e 7072 6f6d 7074 732e 7072 6f6d  elf.prompts.prom
-00011950: 7074 5374 796c 6532 2c20 6465 6661 756c  ptStyle2, defaul
-00011960: 743d 636f 6e66 6967 2e74 7473 436f 6d6d  t=config.ttsComm
-00011970: 616e 6429 0a20 2020 2020 2020 2069 6620  and).        if 
-00011980: 7474 7343 6f6d 6d61 6e64 3a0a 2020 2020  ttsCommand:.    
-00011990: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
-000119a0: 5370 6563 6966 7920 636f 6d6d 616e 6420  Specify command 
-000119b0: 7375 6666 6978 2062 656c 6f77 2c20 6966  suffix below, if
-000119c0: 2061 6e79 205b 6c65 6176 6520 6974 2062   any [leave it b
-000119d0: 6c61 6e6b 2069 6620 4e2f 415d 3a22 290a  lank if N/A]:").
-000119e0: 2020 2020 2020 2020 2020 2020 7474 7343              ttsC
-000119f0: 6f6d 6d61 6e64 5375 6666 6978 203d 2073  ommandSuffix = s
-00011a00: 656c 662e 7072 6f6d 7074 732e 7369 6d70  elf.prompts.simp
-00011a10: 6c65 5072 6f6d 7074 2873 7479 6c65 3d73  lePrompt(style=s
-00011a20: 656c 662e 7072 6f6d 7074 732e 7072 6f6d  elf.prompts.prom
-00011a30: 7074 5374 796c 6532 2c20 6465 6661 756c  ptStyle2, defaul
-00011a40: 743d 636f 6e66 6967 2e74 7473 436f 6d6d  t=config.ttsComm
-00011a50: 616e 6453 7566 6669 7829 0a20 2020 2020  andSuffix).     
-00011a60: 2020 2020 2020 2069 6620 7474 7343 6f6d         if ttsCom
-00011a70: 6d61 6e64 2e6c 6f77 6572 2829 203d 3d20  mand.lower() == 
-00011a80: 2277 696e 646f 7773 223a 0a20 2020 2020  "windows":.     
-00011a90: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
-00011aa0: 6e64 203d 2066 2727 2750 6f77 6572 5368  nd = f'''PowerSh
-00011ab0: 656c 6c20 2d43 6f6d 6d61 6e64 2022 4164  ell -Command "Ad
-00011ac0: 642d 5479 7065 20e2 8093 4173 7365 6d62  d-Type ...Assemb
-00011ad0: 6c79 4e61 6d65 2053 7973 7465 6d2e 5370  lyName System.Sp
-00011ae0: 6565 6368 3b20 284e 6577 2d4f 626a 6563  eech; (New-Objec
-00011af0: 7420 5379 7374 656d 2e53 7065 6563 682e  t System.Speech.
-00011b00: 5379 6e74 6865 7369 732e 5370 6565 6368  Synthesis.Speech
-00011b10: 5379 6e74 6865 7369 7a65 7229 2e53 7065  Synthesizer).Spe
-00011b20: 616b 2827 7465 7374 696e 6727 293b 2227  ak('testing');"'
-00011b30: 2727 0a20 2020 2020 2020 2020 2020 2020  ''.             
-00011b40: 2020 2074 7473 436f 6d6d 616e 6453 7566     ttsCommandSuf
-00011b50: 6669 7820 3d20 2222 0a20 2020 2020 2020  fix = "".       
-00011b60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00011b70: 2020 2020 2020 2020 2020 2063 6f6d 6d61             comma
-00011b80: 6e64 203d 2066 2727 277b 7474 7343 6f6d  nd = f'''{ttsCom
-00011b90: 6d61 6e64 7d20 2274 6573 7469 6e67 227b  mand} "testing"{
-00011ba0: 7474 7343 6f6d 6d61 6e64 5375 6666 6978  ttsCommandSuffix
-00011bb0: 7d27 2727 0a20 2020 2020 2020 2020 2020  }'''.           
-00011bc0: 205f 2c20 7374 6445 7272 203d 2073 7562   _, stdErr = sub
-00011bd0: 7072 6f63 6573 732e 506f 7065 6e28 636f  process.Popen(co
-00011be0: 6d6d 616e 642c 2073 6865 6c6c 3d54 7275  mmand, shell=Tru
-00011bf0: 652c 2073 7464 6f75 743d 7375 6270 726f  e, stdout=subpro
-00011c00: 6365 7373 2e50 4950 452c 2073 7464 6572  cess.PIPE, stder
-00011c10: 723d 7375 6270 726f 6365 7373 2e50 4950  r=subprocess.PIP
-00011c20: 4529 2e63 6f6d 6d75 6e69 6361 7465 2829  E).communicate()
-00011c30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00011c40: 7374 6445 7272 3a0a 2020 2020 2020 2020  stdErr:.        
-00011c50: 2020 2020 2020 2020 7368 6f77 4572 726f          showErro
-00011c60: 7273 2829 2069 6620 636f 6e66 6967 2e64  rs() if config.d
-00011c70: 6576 656c 6f70 6572 2065 6c73 6520 7072  eveloper else pr
-00011c80: 696e 7431 2822 456e 7465 7265 6420 636f  int1("Entered co
-00011c90: 6d6d 616e 6420 696e 7661 6c69 6421 2229  mmand invalid!")
-00011ca0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00011cb0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00011cc0: 2020 2063 6f6e 6669 672e 7474 7343 6f6d     config.ttsCom
-00011cd0: 6d61 6e64 2c20 636f 6e66 6967 2e74 7473  mand, config.tts
-00011ce0: 436f 6d6d 616e 6453 7566 6669 7820 3d20  CommandSuffix = 
-00011cf0: 7474 7343 6f6d 6d61 6e64 2c20 7474 7343  ttsCommand, ttsC
-00011d00: 6f6d 6d61 6e64 5375 6666 6978 0a20 2020  ommandSuffix.   
-00011d10: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-00011d20: 6669 672e 7361 7665 436f 6e66 6967 2829  fig.saveConfig()
-00011d30: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00011d40: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00011d50: 672e 7474 7343 6f6d 6d61 6e64 2c20 636f  g.ttsCommand, co
-00011d60: 6e66 6967 2e74 7473 436f 6d6d 616e 6453  nfig.ttsCommandS
-00011d70: 7566 6669 7820 3d20 2222 2c20 2222 0a0a  uffix = "", ""..
-00011d80: 2020 2020 6465 6620 746f 6767 6c65 576f      def toggleWo
-00011d90: 7264 5772 6170 2873 656c 6629 3a0a 2020  rdWrap(self):.  
-00011da0: 2020 2020 2020 636f 6e66 6967 2e77 7261        config.wra
-00011db0: 7057 6f72 6473 203d 206e 6f74 2063 6f6e  pWords = not con
-00011dc0: 6669 672e 7772 6170 576f 7264 730a 2020  fig.wrapWords.  
-00011dd0: 2020 2020 2020 636f 6e66 6967 2e73 6176        config.sav
-00011de0: 6543 6f6e 6669 6728 290a 2020 2020 2020  eConfig().      
-00011df0: 2020 7072 696e 7433 2866 2257 6f72 6420    print3(f"Word 
-00011e00: 5772 6170 3a20 277b 2765 6e61 626c 6564  Wrap: '{'enabled
-00011e10: 2720 6966 2063 6f6e 6669 672e 7772 6170  ' if config.wrap
-00011e20: 576f 7264 7320 656c 7365 2027 6469 7361  Words else 'disa
-00011e30: 626c 6564 277d 2721 2229 0a0a 2020 2020  bled'}'!")..    
-00011e40: 6465 6620 746f 6767 6c65 4d6f 7573 6553  def toggleMouseS
-00011e50: 7570 706f 7274 2873 656c 6629 3a0a 2020  upport(self):.  
-00011e60: 2020 2020 2020 636f 6e66 6967 2e6d 6f75        config.mou
-00011e70: 7365 5375 7070 6f72 7420 3d20 6e6f 7420  seSupport = not 
-00011e80: 636f 6e66 6967 2e6d 6f75 7365 5375 7070  config.mouseSupp
-00011e90: 6f72 740a 2020 2020 2020 2020 636f 6e66  ort.        conf
-00011ea0: 6967 2e73 6176 6543 6f6e 6669 6728 290a  ig.saveConfig().
-00011eb0: 2020 2020 2020 2020 7072 696e 7433 2866          print3(f
-00011ec0: 2245 6e74 7279 204d 6f75 7365 2053 7570  "Entry Mouse Sup
-00011ed0: 706f 7274 3a20 277b 2765 6e61 626c 6564  port: '{'enabled
-00011ee0: 2720 6966 2063 6f6e 6669 672e 6d6f 7573  ' if config.mous
-00011ef0: 6553 7570 706f 7274 2065 6c73 6520 2764  eSupport else 'd
-00011f00: 6973 6162 6c65 6427 7d27 2122 290a 0a20  isabled'}'!").. 
-00011f10: 2020 2064 6566 2074 6f67 676c 6549 6d70     def toggleImp
-00011f20: 726f 7665 6457 7269 7469 6e67 2873 656c  rovedWriting(sel
-00011f30: 6629 3a0a 2020 2020 2020 2020 636f 6e66  f):.        conf
-00011f40: 6967 2e64 6973 706c 6179 496d 7072 6f76  ig.displayImprov
-00011f50: 6564 5772 6974 696e 6720 3d20 6e6f 7420  edWriting = not 
-00011f60: 636f 6e66 6967 2e64 6973 706c 6179 496d  config.displayIm
-00011f70: 7072 6f76 6564 5772 6974 696e 670a 2020  provedWriting.  
-00011f80: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
-00011f90: 6469 7370 6c61 7949 6d70 726f 7665 6457  displayImprovedW
-00011fa0: 7269 7469 6e67 3a0a 2020 2020 2020 2020  riting:.        
-00011fb0: 2020 2020 7072 696e 7431 2822 506c 6561      print1("Plea
-00011fc0: 7365 2073 7065 6369 6679 2074 6865 2077  se specify the w
-00011fd0: 7269 7469 6e67 2073 7479 6c65 2062 656c  riting style bel
-00011fe0: 6f77 3a22 290a 2020 2020 2020 2020 2020  ow:").          
-00011ff0: 2020 7374 796c 6520 3d20 7365 6c66 2e70    style = self.p
-00012000: 726f 6d70 7473 2e73 696d 706c 6550 726f  rompts.simplePro
-00012010: 6d70 7428 7374 796c 653d 7365 6c66 2e70  mpt(style=self.p
-00012020: 726f 6d70 7473 2e70 726f 6d70 7453 7479  rompts.promptSty
-00012030: 6c65 322c 2064 6566 6175 6c74 3d63 6f6e  le2, default=con
-00012040: 6669 672e 696d 7072 6f76 6564 5772 6974  fig.improvedWrit
-00012050: 696e 6753 7974 6c65 290a 2020 2020 2020  ingSytle).      
-00012060: 2020 2020 2020 6966 2073 7479 6c65 2061        if style a
-00012070: 6e64 206e 6f74 2073 7479 6c65 2069 6e20  nd not style in 
-00012080: 2863 6f6e 6669 672e 6578 6974 5f65 6e74  (config.exit_ent
-00012090: 7279 2c20 636f 6e66 6967 2e63 616e 6365  ry, config.cance
-000120a0: 6c5f 656e 7472 7929 3a0a 2020 2020 2020  l_entry):.      
-000120b0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-000120c0: 2e69 6d70 726f 7665 6457 7269 7469 6e67  .improvedWriting
-000120d0: 5379 746c 6520 3d20 7374 796c 650a 2020  Sytle = style.  
-000120e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000120f0: 6e66 6967 2e73 6176 6543 6f6e 6669 6728  nfig.saveConfig(
-00012100: 290a 2020 2020 2020 2020 7072 696e 7433  ).        print3
-00012110: 2866 2249 6d70 726f 7665 6420 5772 6974  (f"Improved Writ
-00012120: 696e 6720 4469 7370 6c61 793a 2027 7b27  ing Display: '{'
-00012130: 656e 6162 6c65 6427 2069 6620 636f 6e66  enabled' if conf
-00012140: 6967 2e64 6973 706c 6179 496d 7072 6f76  ig.displayImprov
-00012150: 6564 5772 6974 696e 6720 656c 7365 2027  edWriting else '
-00012160: 6469 7361 626c 6564 277d 2721 2229 0a0a  disabled'}'!")..
-00012170: 2020 2020 6465 6620 7365 7441 7564 696f      def setAudio
-00012180: 506c 6179 6261 636b 546f 6f6c 2873 656c  PlaybackTool(sel
-00012190: 6629 3a0a 2020 2020 2020 2020 706c 6179  f):.        play
-000121a0: 6261 636b 203d 2073 656c 662e 6469 616c  back = self.dial
-000121b0: 6f67 732e 6765 7456 616c 6964 4f70 7469  ogs.getValidOpti
-000121c0: 6f6e 7328 0a20 2020 2020 2020 2020 2020  ons(.           
-000121d0: 206f 7074 696f 6e73 3d28 2270 7967 616d   options=("pygam
-000121e0: 6522 2c20 2276 6c63 2229 2c0a 2020 2020  e", "vlc"),.    
-000121f0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00012200: 696f 6e73 3d28 2250 7947 616d 6522 2c20  ions=("PyGame", 
-00012210: 6622 564c 4320 506c 6179 6572 2028 772f  f"VLC Player (w/
-00012220: 2073 7065 6564 2063 6f6e 7472 6f6c 297b   speed control){
-00012230: 2720 5b69 6e73 7461 6c6c 6174 696f 6e20  ' [installation 
-00012240: 7265 7175 6972 6564 5d27 2069 6620 6e6f  required]' if no
-00012250: 7420 636f 6e66 6967 2e69 7356 6c63 506c  t config.isVlcPl
-00012260: 6179 6572 496e 7374 616c 6c65 6420 656c  ayerInstalled el
-00012270: 7365 2027 277d 2229 2c0a 2020 2020 2020  se ''}"),.      
-00012280: 2020 2020 2020 7469 746c 653d 2254 6578        title="Tex
-00012290: 742d 746f 2d53 7065 6563 6820 506c 6179  t-to-Speech Play
-000122a0: 6261 636b 222c 0a20 2020 2020 2020 2020  back",.         
-000122b0: 2020 2074 6578 743d 2253 656c 6563 7420     text="Select 
-000122c0: 6120 7465 7874 2d74 6f2d 7370 6565 6368  a text-to-speech
-000122d0: 2070 6c61 636b 6261 636b 2074 6f6f 6c3a   plackback tool:
-000122e0: 222c 0a20 2020 2020 2020 2020 2020 2064  ",.            d
-000122f0: 6566 6175 6c74 3d22 766c 6322 2069 6620  efault="vlc" if 
-00012300: 636f 6e66 6967 2e69 7356 6c63 506c 6179  config.isVlcPlay
-00012310: 6572 496e 7374 616c 6c65 6420 616e 6420  erInstalled and 
-00012320: 6e6f 7420 636f 6e66 6967 2e75 7365 5079  not config.usePy
-00012330: 6761 6d65 2065 6c73 6520 2270 7967 616d  game else "pygam
-00012340: 6522 2c0a 2020 2020 2020 2020 290a 2020  e",.        ).  
-00012350: 2020 2020 2020 6966 2070 6c61 7962 6163        if playbac
-00012360: 6b3a 0a20 2020 2020 2020 2020 2020 2069  k:.            i
-00012370: 6620 706c 6179 6261 636b 203d 3d20 2276  f playback == "v
-00012380: 6c63 223a 0a20 2020 2020 2020 2020 2020  lc":.           
-00012390: 2020 2020 2069 6620 6e6f 7420 636f 6e66       if not conf
-000123a0: 6967 2e69 7356 6c63 506c 6179 6572 496e  ig.isVlcPlayerIn
-000123b0: 7374 616c 6c65 643a 0a20 2020 2020 2020  stalled:.       
-000123c0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000123d0: 6e74 3128 2256 4c43 2070 6c61 7965 7220  nt1("VLC player 
-000123e0: 6e6f 7420 666f 756e 6421 2049 6e73 7461  not found! Insta
-000123f0: 6c6c 2069 7420 6669 7273 7421 2229 0a20  ll it first!"). 
-00012400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012410: 2020 2070 7269 6e74 3328 2254 6578 742d     print3("Text-
-00012420: 746f 2d53 7065 6563 6820 506c 6179 6261  to-Speech Playba
-00012430: 636b 2063 6861 6e67 6564 2074 6f3a 2050  ck changed to: P
-00012440: 7947 616d 6522 290a 2020 2020 2020 2020  yGame").        
-00012450: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00012460: 6967 2e75 7365 5079 6761 6d65 203d 2054  ig.usePygame = T
-00012470: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-00012480: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00012490: 2020 2020 2020 2020 2020 2020 2020 636f                co
-000124a0: 6e66 6967 2e75 7365 5079 6761 6d65 203d  nfig.usePygame =
-000124b0: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-000124c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000124d0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-000124e0: 7573 6550 7967 616d 6520 3d20 5472 7565  usePygame = True
-000124f0: 0a0a 2020 2020 6465 6620 7365 7454 6578  ..    def setTex
-00012500: 7454 6f53 7065 6563 6843 6f6e 6669 6728  tToSpeechConfig(
-00012510: 7365 6c66 293a 0a20 2020 2020 2020 2074  self):.        t
-00012520: 7473 506c 6174 666f 726d 203d 2073 656c  tsPlatform = sel
-00012530: 662e 6469 616c 6f67 732e 6765 7456 616c  f.dialogs.getVal
-00012540: 6964 4f70 7469 6f6e 7328 0a20 2020 2020  idOptions(.     
-00012550: 2020 2020 2020 206f 7074 696f 6e73 3d28         options=(
-00012560: 2267 6f6f 676c 6522 2c20 2267 6f6f 676c  "google", "googl
-00012570: 6563 6c6f 7564 222c 2022 656c 6576 656e  ecloud", "eleven
-00012580: 6c61 6273 222c 2022 6375 7374 6f6d 2229  labs", "custom")
-00012590: 2c0a 2020 2020 2020 2020 2020 2020 6465  ,.            de
-000125a0: 7363 7269 7074 696f 6e73 3d28 2247 6f6f  scriptions=("Goo
-000125b0: 676c 6520 5465 7874 2d74 6f2d 5370 6565  gle Text-to-Spee
-000125c0: 6368 2028 4765 6e65 7269 6329 222c 2022  ch (Generic)", "
-000125d0: 476f 6f67 6c65 2054 6578 742d 746f 2d53  Google Text-to-S
-000125e0: 7065 6563 6820 2841 5049 2922 2c20 2245  peech (API)", "E
-000125f0: 6c65 7665 6e4c 6162 7320 2841 5049 2922  levenLabs (API)"
-00012600: 2c20 2243 7573 746f 6d20 5465 7874 2d74  , "Custom Text-t
-00012610: 6f2d 5370 6565 6368 2043 6f6d 6d61 6e64  o-Speech Command
-00012620: 205b 6164 7661 6e63 6564 5d22 292c 0a20   [advanced]"),. 
-00012630: 2020 2020 2020 2020 2020 2074 6974 6c65             title
-00012640: 3d22 5465 7874 2d74 6f2d 5370 6565 6368  ="Text-to-Speech
-00012650: 2043 6f6e 6669 6775 7261 7469 6f6e 7322   Configurations"
-00012660: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
-00012670: 7874 3d22 5365 6c65 6374 2061 2074 6578  xt="Select a tex
-00012680: 742d 746f 2d73 7065 6563 6820 706c 6174  t-to-speech plat
-00012690: 666f 726d 3a22 2c0a 2020 2020 2020 2020  form:",.        
-000126a0: 2020 2020 6465 6661 756c 743d 636f 6e66      default=conf
-000126b0: 6967 2e74 7473 506c 6174 666f 726d 2c0a  ig.ttsPlatform,.
-000126c0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-000126d0: 2020 6966 2074 7473 506c 6174 666f 726d    if ttsPlatform
-000126e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-000126f0: 2074 7473 506c 6174 666f 726d 203d 3d20   ttsPlatform == 
-00012700: 2267 6f6f 676c 6563 6c6f 7564 2220 616e  "googlecloud" an
-00012710: 6420 6e6f 7420 286f 732e 656e 7669 726f  d not (os.enviro
-00012720: 6e5b 2247 4f4f 474c 455f 4150 504c 4943  n["GOOGLE_APPLIC
-00012730: 4154 494f 4e5f 4352 4544 454e 5449 414c  ATION_CREDENTIAL
-00012740: 5322 5d20 616e 6420 2254 6578 742d 746f  S"] and "Text-to
-00012750: 2d53 7065 6563 6822 2069 6e20 636f 6e66  -Speech" in conf
-00012760: 6967 2e65 6e61 626c 6564 476f 6f67 6c65  ig.enabledGoogle
-00012770: 4150 4973 293a 0a20 2020 2020 2020 2020  APIs):.         
-00012780: 2020 2020 2020 2070 7269 6e74 3228 2247         print2("G
-00012790: 6f6f 676c 6520 436c 6f75 6420 5465 7874  oogle Cloud Text
-000127a0: 2d74 6f2d 5370 6565 6368 2066 6561 7475  -to-Speech featu
-000127b0: 7265 2069 7320 6e6f 7420 656e 6162 6c65  re is not enable
-000127c0: 6421 2229 0a20 2020 2020 2020 2020 2020  d!").           
-000127d0: 2020 2020 2070 7269 6e74 3328 2252 6561       print3("Rea
-000127e0: 643a 2068 7474 7073 3a2f 2f67 6974 6875  d: https://githu
-000127f0: 622e 636f 6d2f 656c 6972 616e 776f 6e67  b.com/eliranwong
-00012800: 2f6c 6574 6d65 646f 6974 2f77 696b 692f  /letmedoit/wiki/
-00012810: 476f 6f67 6c65 2d41 5049 2d53 6574 7570  Google-API-Setup
-00012820: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00012830: 2020 2070 7269 6e74 3328 2254 6578 742d     print3("Text-
-00012840: 746f 2d53 7065 6563 6820 706c 6174 666f  to-Speech platfo
-00012850: 726d 2063 6861 6e67 6564 2074 6f3a 2047  rm changed to: G
-00012860: 6f6f 676c 6520 5465 7874 2d74 6f2d 5370  oogle Text-to-Sp
-00012870: 6565 6368 2028 4765 6e65 7269 6329 2229  eech (Generic)")
-00012880: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012890: 2063 6f6e 6669 672e 7474 7350 6c61 7466   config.ttsPlatf
-000128a0: 6f72 6d20 3d20 2267 6f6f 676c 6522 0a20  orm = "google". 
-000128b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000128c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000128d0: 2063 6f6e 6669 672e 7474 7350 6c61 7466   config.ttsPlatf
-000128e0: 6f72 6d20 3d20 7474 7350 6c61 7466 6f72  orm = ttsPlatfor
-000128f0: 6d0a 2020 2020 2020 2020 2320 6675 7274  m.        # furt
-00012900: 6865 7220 6f70 7469 6f6e 730a 2020 2020  her options.    
-00012910: 2020 2020 6966 2063 6f6e 6669 672e 7474      if config.tt
-00012920: 7350 6c61 7466 6f72 6d20 3d3d 2022 676f  sPlatform == "go
-00012930: 6f67 6c65 223a 0a20 2020 2020 2020 2020  ogle":.         
-00012940: 2020 2073 656c 662e 7365 7447 7474 734c     self.setGttsL
-00012950: 616e 6775 6167 6528 290a 2020 2020 2020  anguage().      
-00012960: 2020 2020 2020 7365 6c66 2e73 6574 4175        self.setAu
-00012970: 6469 6f50 6c61 7962 6163 6b54 6f6f 6c28  dioPlaybackTool(
-00012980: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00012990: 6c66 2e73 6574 566c 6353 7065 6564 2829  lf.setVlcSpeed()
-000129a0: 0a20 2020 2020 2020 2065 6c69 6620 636f  .        elif co
-000129b0: 6e66 6967 2e74 7473 506c 6174 666f 726d  nfig.ttsPlatform
-000129c0: 203d 3d20 2267 6f6f 676c 6563 6c6f 7564   == "googlecloud
-000129d0: 223a 0a20 2020 2020 2020 2020 2020 2073  ":.            s
-000129e0: 656c 662e 7365 7447 6374 7473 4c61 6e67  elf.setGcttsLang
-000129f0: 7561 6765 2829 0a20 2020 2020 2020 2020  uage().         
-00012a00: 2020 2073 656c 662e 7365 7447 6374 7473     self.setGctts
-00012a10: 5370 6565 6428 290a 2020 2020 2020 2020  Speed().        
-00012a20: 2020 2020 7365 6c66 2e73 6574 4175 6469      self.setAudi
-00012a30: 6f50 6c61 7962 6163 6b54 6f6f 6c28 290a  oPlaybackTool().
-00012a40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00012a50: 2e73 6574 566c 6353 7065 6564 2829 0a20  .setVlcSpeed(). 
-00012a60: 2020 2020 2020 2065 6c69 6620 636f 6e66         elif conf
-00012a70: 6967 2e74 7473 506c 6174 666f 726d 203d  ig.ttsPlatform =
-00012a80: 3d20 2265 6c65 7665 6e6c 6162 7322 3a0a  = "elevenlabs":.
-00012a90: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00012aa0: 6f74 2063 6f6e 6669 672e 656c 6576 656e  ot config.eleven
-00012ab0: 6c61 6273 4170 693a 0a20 2020 2020 2020  labsApi:.       
-00012ac0: 2020 2020 2020 2020 2073 656c 662e 6368           self.ch
-00012ad0: 616e 6765 456c 6576 656e 6c61 6273 4170  angeElevenlabsAp
-00012ae0: 6928 290a 2020 2020 2020 2020 2020 2020  i().            
-00012af0: 6966 206e 6f74 2063 6f6e 6669 672e 656c  if not config.el
-00012b00: 6576 656e 6c61 6273 4170 693a 0a20 2020  evenlabsApi:.   
-00012b10: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-00012b20: 6e74 3128 2245 6c65 7665 6e4c 6162 7320  nt1("ElevenLabs 
-00012b30: 4150 4920 6b65 7920 6e6f 7420 666f 756e  API key not foun
-00012b40: 6421 2229 0a20 2020 2020 2020 2020 2020  d!").           
-00012b50: 2020 2020 2070 7269 6e74 3328 2254 6578       print3("Tex
-00012b60: 742d 746f 2d53 7065 6563 6820 706c 6174  t-to-Speech plat
-00012b70: 666f 726d 2063 6861 6e67 6564 2074 6f3a  form changed to:
-00012b80: 2047 6f6f 676c 6520 5465 7874 2d74 6f2d   Google Text-to-
-00012b90: 5370 6565 6368 2028 4765 6e65 7269 6329  Speech (Generic)
-00012ba0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00012bb0: 2020 2063 6f6e 6669 672e 7474 7350 6c61     config.ttsPla
-00012bc0: 7466 6f72 6d20 3d20 2267 6f6f 676c 6522  tform = "google"
-00012bd0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00012be0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00012bf0: 2020 2073 656c 662e 7365 7445 6c65 7665     self.setEleve
-00012c00: 6e6c 6162 7356 6f69 6365 2829 0a20 2020  nlabsVoice().   
-00012c10: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
-00012c20: 2e74 7473 506c 6174 666f 726d 203d 3d20  .ttsPlatform == 
-00012c30: 2263 7573 746f 6d22 3a0a 2020 2020 2020  "custom":.      
-00012c40: 2020 2020 2020 7365 6c66 2e64 6566 696e        self.defin
-00012c50: 6554 7473 436f 6d6d 616e 6428 290a 2020  eTtsCommand().  
-00012c60: 2020 2020 2020 2320 7361 7665 2063 6f6e        # save con
-00012c70: 6669 6773 0a20 2020 2020 2020 2063 6f6e  figs.        con
-00012c80: 6669 672e 7361 7665 436f 6e66 6967 2829  fig.saveConfig()
-00012c90: 0a0a 2020 2020 6465 6620 7365 7456 6f69  ..    def setVoi
-00012ca0: 6365 5479 7069 6e67 436f 6e66 6967 2873  ceTypingConfig(s
-00012cb0: 656c 6629 3a0a 2020 2020 2020 2020 766f  elf):.        vo
-00012cc0: 6963 6554 7970 696e 6750 6c61 7466 6f72  iceTypingPlatfor
-00012cd0: 6d20 3d20 7365 6c66 2e64 6961 6c6f 6773  m = self.dialogs
-00012ce0: 2e67 6574 5661 6c69 644f 7074 696f 6e73  .getValidOptions
-00012cf0: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
-00012d00: 7469 6f6e 733d 2822 676f 6f67 6c65 222c  tions=("google",
-00012d10: 2022 676f 6f67 6c65 636c 6f75 6422 2c20   "googlecloud", 
-00012d20: 2277 6869 7370 6572 2229 2c0a 2020 2020  "whisper"),.    
-00012d30: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00012d40: 696f 6e73 3d28 2247 6f6f 676c 6520 5370  ions=("Google Sp
-00012d50: 6565 6368 2d74 6f2d 5465 7874 2028 4765  eech-to-Text (Ge
-00012d60: 6e65 7269 6329 205b 6f6e 6c69 6e65 5d22  neric) [online]"
-00012d70: 2c20 2247 6f6f 676c 6520 5370 6565 6368  , "Google Speech
-00012d80: 2d74 6f2d 5465 7874 2028 4150 4929 205b  -to-Text (API) [
-00012d90: 6f6e 6c69 6e65 5d22 2c20 224f 7065 6e41  online]", "OpenA
-00012da0: 4920 5768 6973 7065 7220 5b6f 6666 6c69  I Whisper [offli
-00012db0: 6e65 3b20 736c 6f77 6572 2077 6974 6820  ne; slower with 
-00012dc0: 6e6f 6e2d 456e 676c 6973 6820 766f 6963  non-English voic
-00012dd0: 6573 5d22 292c 0a20 2020 2020 2020 2020  es]"),.         
-00012de0: 2020 2074 6974 6c65 3d22 566f 6963 6520     title="Voice 
-00012df0: 5479 7069 6e67 2043 6f6e 6669 6775 7261  Typing Configura
-00012e00: 7469 6f6e 7322 2c0a 2020 2020 2020 2020  tions",.        
-00012e10: 2020 2020 7465 7874 3d22 5365 6c65 6374      text="Select
-00012e20: 2061 2076 6f69 6365 2074 7970 696e 6720   a voice typing 
-00012e30: 706c 6174 666f 726d 3a22 2c0a 2020 2020  platform:",.    
-00012e40: 2020 2020 2020 2020 6465 6661 756c 743d          default=
-00012e50: 636f 6e66 6967 2e76 6f69 6365 5479 7069  config.voiceTypi
-00012e60: 6e67 506c 6174 666f 726d 2c0a 2020 2020  ngPlatform,.    
-00012e70: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-00012e80: 2076 6f69 6365 5479 7069 6e67 506c 6174   voiceTypingPlat
-00012e90: 666f 726d 3a0a 2020 2020 2020 2020 2020  form:.          
-00012ea0: 2020 6966 2076 6f69 6365 5479 7069 6e67    if voiceTyping
-00012eb0: 506c 6174 666f 726d 203d 3d20 2267 6f6f  Platform == "goo
-00012ec0: 676c 6563 6c6f 7564 2220 616e 6420 6e6f  glecloud" and no
-00012ed0: 7420 286f 732e 656e 7669 726f 6e5b 2247  t (os.environ["G
-00012ee0: 4f4f 474c 455f 4150 504c 4943 4154 494f  OOGLE_APPLICATIO
-00012ef0: 4e5f 4352 4544 454e 5449 414c 5322 5d20  N_CREDENTIALS"] 
-00012f00: 616e 6420 2253 7065 6563 682d 746f 2d54  and "Speech-to-T
-00012f10: 6578 7422 2069 6e20 636f 6e66 6967 2e65  ext" in config.e
-00012f20: 6e61 626c 6564 476f 6f67 6c65 4150 4973  nabledGoogleAPIs
-00012f30: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00012f40: 2020 2070 7269 6e74 3228 2247 6f6f 676c     print2("Googl
-00012f50: 6520 436c 6f75 6420 5370 6565 6368 2d74  e Cloud Speech-t
-00012f60: 6f2d 5465 7874 2066 6561 7475 7265 2069  o-Text feature i
-00012f70: 7320 6e6f 7420 656e 6162 6c65 6421 2229  s not enabled!")
-00012f80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012f90: 2070 7269 6e74 3328 2252 6561 643a 2068   print3("Read: h
-00012fa0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00012fb0: 6d2f 656c 6972 616e 776f 6e67 2f6c 6574  m/eliranwong/let
-00012fc0: 6d65 646f 6974 2f77 696b 692f 476f 6f67  medoit/wiki/Goog
-00012fd0: 6c65 2d41 5049 2d53 6574 7570 2229 0a20  le-API-Setup"). 
-00012fe0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00012ff0: 7269 6e74 3328 2256 6f69 6365 2074 7970  rint3("Voice typ
-00013000: 696e 6720 706c 6174 666f 726d 2063 6861  ing platform cha
-00013010: 6e67 6564 2074 6f3a 2047 6f6f 676c 6520  nged to: Google 
-00013020: 5370 6565 6368 2d74 6f2d 5465 7874 2028  Speech-to-Text (
-00013030: 4765 6e65 7269 6329 2229 0a20 2020 2020  Generic)").     
-00013040: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00013050: 672e 766f 6963 6554 7970 696e 6750 6c61  g.voiceTypingPla
-00013060: 7466 6f72 6d20 3d20 2267 6f6f 676c 6522  tform = "google"
-00013070: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
-00013080: 6620 766f 6963 6554 7970 696e 6750 6c61  f voiceTypingPla
-00013090: 7466 6f72 6d20 3d3d 2022 7768 6973 7065  tform == "whispe
-000130a0: 7222 2061 6e64 206e 6f74 2069 7343 6f6d  r" and not isCom
-000130b0: 6d61 6e64 496e 7374 616c 6c65 6428 2266  mandInstalled("f
-000130c0: 666d 7065 6722 293a 0a20 2020 2020 2020  fmpeg"):.       
-000130d0: 2020 2020 2020 2020 2070 7269 6e74 3228           print2(
-000130e0: 2249 6e73 7461 6c6c 2027 6666 6d70 6567  "Install 'ffmpeg
-000130f0: 2720 6669 7273 7420 746f 2075 7365 206f  ' first to use o
-00013100: 6666 6c69 6e65 206f 7065 6e61 6920 7768  ffline openai wh
-00013110: 6973 7065 7220 6d6f 6465 6c21 2229 0a20  isper model!"). 
-00013120: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00013130: 7269 6e74 3328 2252 6561 643a 2068 7474  rint3("Read: htt
-00013140: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00013150: 6f70 656e 6169 2f77 6869 7370 6572 2373  openai/whisper#s
-00013160: 6574 7570 2229 0a20 2020 2020 2020 2020  etup").         
-00013170: 2020 2020 2020 2070 7269 6e74 3328 2256         print3("V
-00013180: 6f69 6365 2074 7970 696e 6720 706c 6174  oice typing plat
-00013190: 666f 726d 2063 6861 6e67 6564 2074 6f3a  form changed to:
-000131a0: 2047 6f6f 676c 6520 5370 6565 6368 2d74   Google Speech-t
-000131b0: 6f2d 5465 7874 2028 4765 6e65 7269 6329  o-Text (Generic)
-000131c0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-000131d0: 2020 2063 6f6e 6669 672e 766f 6963 6554     config.voiceT
-000131e0: 7970 696e 6750 6c61 7466 6f72 6d20 3d20  ypingPlatform = 
-000131f0: 2267 6f6f 676c 6522 0a20 2020 2020 2020  "google".       
-00013200: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00013210: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00013220: 672e 766f 6963 6554 7970 696e 6750 6c61  g.voiceTypingPla
-00013230: 7466 6f72 6d20 3d20 766f 6963 6554 7970  tform = voiceTyp
-00013240: 696e 6750 6c61 7466 6f72 6d0a 2020 2020  ingPlatform.    
-00013250: 2020 2020 2320 6c61 6e67 7561 6765 0a20      # language. 
-00013260: 2020 2020 2020 2073 656c 662e 7365 7453         self.setS
-00013270: 7065 6563 6854 6f54 6578 744c 616e 6775  peechToTextLangu
-00013280: 6167 6528 290a 2020 2020 2020 2020 2320  age().        # 
-00013290: 636f 6e66 6967 7572 6520 636f 6e66 6967  configure config
-000132a0: 2e76 6f69 6365 5479 7069 6e67 4164 6a75  .voiceTypingAdju
-000132b0: 7374 416d 6269 656e 744e 6f69 7365 0a20  stAmbientNoise. 
-000132c0: 2020 2020 2020 2076 6f69 6365 5479 7069         voiceTypi
-000132d0: 6e67 4164 6a75 7374 416d 6269 656e 744e  ngAdjustAmbientN
-000132e0: 6f69 7365 203d 2073 656c 662e 6469 616c  oise = self.dial
-000132f0: 6f67 732e 6765 7456 616c 6964 4f70 7469  ogs.getValidOpti
-00013300: 6f6e 7328 0a20 2020 2020 2020 2020 2020  ons(.           
-00013310: 206f 7074 696f 6e73 3d28 2259 6573 222c   options=("Yes",
-00013320: 2022 4e6f 2229 2c0a 2020 2020 2020 2020   "No"),.        
-00013330: 2020 2020 6465 7363 7269 7074 696f 6e73      descriptions
-00013340: 3d28 2259 6573 205b 736c 6f77 6572 5d22  =("Yes [slower]"
-00013350: 2c20 224e 6f22 292c 0a20 2020 2020 2020  , "No"),.       
-00013360: 2020 2020 2074 6974 6c65 3d22 4164 6a75       title="Adju
-00013370: 7374 2041 6d62 6965 6e74 204e 6f69 7365  st Ambient Noise
-00013380: 222c 0a20 2020 2020 2020 2020 2020 2074  ",.            t
-00013390: 6578 743d 2244 6f20 796f 7520 7761 6e74  ext="Do you want
-000133a0: 2074 6f20 6164 6a75 7374 2061 6d62 6965   to adjust ambie
-000133b0: 6e74 206e 6f69 7365 3f22 2c0a 2020 2020  nt noise?",.    
-000133c0: 2020 2020 2020 2020 6465 6661 756c 743d          default=
-000133d0: 2259 6573 2220 6966 2063 6f6e 6669 672e  "Yes" if config.
-000133e0: 766f 6963 6554 7970 696e 6741 646a 7573  voiceTypingAdjus
-000133f0: 7441 6d62 6965 6e74 4e6f 6973 6520 656c  tAmbientNoise el
-00013400: 7365 2022 4e6f 222c 0a20 2020 2020 2020  se "No",.       
-00013410: 2029 0a20 2020 2020 2020 2069 6620 766f   ).        if vo
-00013420: 6963 6554 7970 696e 6741 646a 7573 7441  iceTypingAdjustA
-00013430: 6d62 6965 6e74 4e6f 6973 653a 0a20 2020  mbientNoise:.   
-00013440: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-00013450: 766f 6963 6554 7970 696e 6741 646a 7573  voiceTypingAdjus
-00013460: 7441 6d62 6965 6e74 4e6f 6973 6520 3d20  tAmbientNoise = 
-00013470: 5472 7565 2069 6620 766f 6963 6554 7970  True if voiceTyp
-00013480: 696e 6741 646a 7573 7441 6d62 6965 6e74  ingAdjustAmbient
-00013490: 4e6f 6973 6520 3d3d 2022 5965 7322 2065  Noise == "Yes" e
-000134a0: 6c73 6520 4661 6c73 650a 2020 2020 2020  lse False.      
-000134b0: 2020 2320 6175 6469 6f20 6e6f 7469 6669    # audio notifi
-000134c0: 6361 7469 6f6e 0a20 2020 2020 2020 2076  cation.        v
-000134d0: 6f69 6365 5479 7069 6e67 4e6f 7469 6669  oiceTypingNotifi
-000134e0: 6361 7469 6f6e 203d 2073 656c 662e 6469  cation = self.di
-000134f0: 616c 6f67 732e 6765 7456 616c 6964 4f70  alogs.getValidOp
-00013500: 7469 6f6e 7328 0a20 2020 2020 2020 2020  tions(.         
-00013510: 2020 206f 7074 696f 6e73 3d28 2259 6573     options=("Yes
-00013520: 222c 2022 4e6f 2229 2c0a 2020 2020 2020  ", "No"),.      
-00013530: 2020 2020 2020 7469 746c 653d 2241 7564        title="Aud
-00013540: 696f 204e 6f74 6966 6963 6174 696f 6e22  io Notification"
-00013550: 2c0a 2020 2020 2020 2020 2020 2020 7465  ,.            te
-00013560: 7874 3d22 446f 2079 6f75 2077 616e 7420  xt="Do you want 
-00013570: 6175 6469 6f20 6e6f 7469 6669 6361 7469  audio notificati
-00013580: 6f6e 2077 6865 6e20 796f 7520 7573 6520  on when you use 
-00013590: 6d69 6372 6f70 686f 6e65 3f22 2c0a 2020  microphone?",.  
-000135a0: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
-000135b0: 743d 2259 6573 2220 6966 2063 6f6e 6669  t="Yes" if confi
-000135c0: 672e 766f 6963 6554 7970 696e 674e 6f74  g.voiceTypingNot
-000135d0: 6966 6963 6174 696f 6e20 656c 7365 2022  ification else "
-000135e0: 4e6f 222c 0a20 2020 2020 2020 2029 0a20  No",.        ). 
-000135f0: 2020 2020 2020 2069 6620 766f 6963 6554         if voiceT
-00013600: 7970 696e 674e 6f74 6966 6963 6174 696f  ypingNotificatio
-00013610: 6e3a 0a20 2020 2020 2020 2020 2020 2063  n:.            c
-00013620: 6f6e 6669 672e 766f 6963 6554 7970 696e  onfig.voiceTypin
-00013630: 674e 6f74 6966 6963 6174 696f 6e20 3d20  gNotification = 
-00013640: 5472 7565 2069 6620 766f 6963 6554 7970  True if voiceTyp
-00013650: 696e 674e 6f74 6966 6963 6174 696f 6e20  ingNotification 
-00013660: 3d3d 2022 5965 7322 2065 6c73 6520 4661  == "Yes" else Fa
-00013670: 6c73 650a 2020 2020 2020 2020 2320 6175  lse.        # au
-00013680: 746f 2063 6f6d 706c 6574 696f 6e3a 2076  to completion: v
-00013690: 6f69 6365 5479 7069 6e67 4175 746f 436f  oiceTypingAutoCo
-000136a0: 6d70 6c65 7465 0a20 2020 2020 2020 2076  mplete.        v
-000136b0: 6f69 6365 5479 7069 6e67 4175 746f 436f  oiceTypingAutoCo
-000136c0: 6d70 6c65 7465 203d 2073 656c 662e 6469  mplete = self.di
-000136d0: 616c 6f67 732e 6765 7456 616c 6964 4f70  alogs.getValidOp
-000136e0: 7469 6f6e 7328 0a20 2020 2020 2020 2020  tions(.         
-000136f0: 2020 206f 7074 696f 6e73 3d28 2259 6573     options=("Yes
-00013700: 222c 2022 4e6f 2229 2c0a 2020 2020 2020  ", "No"),.      
-00013710: 2020 2020 2020 7469 746c 653d 2241 7564        title="Aud
-00013720: 696f 2045 6e74 7279 2041 7574 6f20 436f  io Entry Auto Co
-00013730: 6d70 6c65 7469 6f6e 222c 0a20 2020 2020  mpletion",.     
-00013740: 2020 2020 2020 2074 6578 743d 2244 6f20         text="Do 
-00013750: 796f 7520 7761 6e74 2074 6f20 6175 746f  you want to auto
-00013760: 6d61 7469 6361 6c6c 7920 636f 6d70 6c65  matically comple
-00013770: 7465 2079 6f75 7220 656e 7472 7920 7768  te your entry wh
-00013780: 656e 206d 6963 726f 7068 6f6e 6520 7374  en microphone st
-00013790: 6f70 733f 222c 0a20 2020 2020 2020 2020  ops?",.         
-000137a0: 2020 2064 6566 6175 6c74 3d22 5965 7322     default="Yes"
-000137b0: 2069 6620 636f 6e66 6967 2e76 6f69 6365   if config.voice
-000137c0: 5479 7069 6e67 4175 746f 436f 6d70 6c65  TypingAutoComple
-000137d0: 7465 2065 6c73 6520 224e 6f22 2c0a 2020  te else "No",.  
-000137e0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000137f0: 6966 2076 6f69 6365 5479 7069 6e67 4175  if voiceTypingAu
-00013800: 746f 436f 6d70 6c65 7465 3a0a 2020 2020  toComplete:.    
-00013810: 2020 2020 2020 2020 636f 6e66 6967 2e76          config.v
-00013820: 6f69 6365 5479 7069 6e67 4175 746f 436f  oiceTypingAutoCo
-00013830: 6d70 6c65 7465 203d 2054 7275 6520 6966  mplete = True if
-00013840: 2076 6f69 6365 5479 7069 6e67 4175 746f   voiceTypingAuto
-00013850: 436f 6d70 6c65 7465 203d 3d20 2259 6573  Complete == "Yes
-00013860: 2220 656c 7365 2046 616c 7365 0a20 2020  " else False.   
-00013870: 2020 2020 2023 206e 6f74 6966 790a 2020       # notify.  
-00013880: 2020 2020 2020 7072 696e 7428 2222 290a        print("").
-00013890: 2020 2020 2020 2020 7072 696e 7433 2866          print3(f
-000138a0: 2256 6f69 6365 2054 7970 696e 6720 4d6f  "Voice Typing Mo
-000138b0: 6465 6c3a 207b 636f 6e66 6967 2e76 6f69  del: {config.voi
-000138c0: 6365 5479 7069 6e67 506c 6174 666f 726d  ceTypingPlatform
-000138d0: 7d22 290a 2020 2020 2020 2020 7072 696e  }").        prin
-000138e0: 7433 2866 2256 6f69 6365 2054 7970 696e  t3(f"Voice Typin
-000138f0: 6720 4c61 6e67 7561 6765 3a20 7b63 6f6e  g Language: {con
-00013900: 6669 672e 766f 6963 6554 7970 696e 674c  fig.voiceTypingL
-00013910: 616e 6775 6167 657d 2229 0a20 2020 2020  anguage}").     
-00013920: 2020 2070 7269 6e74 3328 6622 416d 6269     print3(f"Ambi
-00013930: 656e 7420 4e6f 6973 6520 4164 6a75 7374  ent Noise Adjust
-00013940: 6d65 6e74 3a20 7b63 6f6e 6669 672e 766f  ment: {config.vo
-00013950: 6963 6554 7970 696e 6741 646a 7573 7441  iceTypingAdjustA
-00013960: 6d62 6965 6e74 4e6f 6973 657d 2229 0a20  mbientNoise}"). 
-00013970: 2020 2020 2020 2070 7269 6e74 3328 6622         print3(f"
-00013980: 4175 6469 6f20 4e6f 7469 6669 6361 7469  Audio Notificati
-00013990: 6f6e 3a20 7b63 6f6e 6669 672e 766f 6963  on: {config.voic
-000139a0: 6554 7970 696e 674e 6f74 6966 6963 6174  eTypingNotificat
-000139b0: 696f 6e7d 2229 0a20 2020 2020 2020 2070  ion}").        p
-000139c0: 7269 6e74 3328 6622 4175 746f 2043 6f6d  rint3(f"Auto Com
-000139d0: 706c 6574 696f 6e3a 207b 636f 6e66 6967  pletion: {config
-000139e0: 2e76 6f69 6365 5479 7069 6e67 4175 746f  .voiceTypingAuto
-000139f0: 436f 6d70 6c65 7465 7d22 290a 2020 2020  Complete}").    
-00013a00: 2020 2020 2320 7361 7665 2063 6f6e 6669      # save confi
-00013a10: 6773 0a20 2020 2020 2020 2063 6f6e 6669  gs.        confi
-00013a20: 672e 7361 7665 436f 6e66 6967 2829 0a0a  g.saveConfig()..
-00013a30: 2020 2020 6465 6620 7361 7665 4368 6174      def saveChat
-00013a40: 2873 656c 662c 206d 6573 7361 6765 7329  (self, messages)
-00013a50: 3a0a 2020 2020 2020 2020 6d65 7373 6167  :.        messag
-00013a60: 6573 436f 7079 203d 2063 6f70 792e 6465  esCopy = copy.de
-00013a70: 6570 636f 7079 286d 6573 7361 6765 7329  epcopy(messages)
-00013a80: 0a0a 2020 2020 2020 2020 6966 2063 6f6e  ..        if con
-00013a90: 6669 672e 636f 6e76 6572 7361 7469 6f6e  fig.conversation
-00013aa0: 5374 6172 7465 643a 0a20 2020 2020 2020  Started:.       
-00013ab0: 2020 2020 2074 696d 6573 7461 6d70 203d       timestamp =
-00013ac0: 2067 6574 4375 7272 656e 7444 6174 6554   getCurrentDateT
-00013ad0: 696d 6528 290a 0a20 2020 2020 2020 2020  ime()..         
-00013ae0: 2020 2069 6620 6861 7361 7474 7228 636f     if hasattr(co
-00013af0: 6e66 6967 2c20 2273 6176 655f 6368 6174  nfig, "save_chat
-00013b00: 5f72 6563 6f72 6422 293a 0a20 2020 2020  _record"):.     
-00013b10: 2020 2020 2020 2020 2020 2023 2077 6865             # whe
-00013b20: 6e20 706c 7567 696e 2022 7361 7665 2063  n plugin "save c
-00013b30: 6861 7420 7265 636f 7264 7322 2069 7320  hat records" is 
-00013b40: 656e 6162 6c65 640a 2020 2020 2020 2020  enabled.        
-00013b50: 2020 2020 2020 2020 6d65 7373 6167 654c          messageL
-00013b60: 656e 6774 6820 3d20 6c65 6e28 6d65 7373  ength = len(mess
-00013b70: 6167 6573 436f 7079 290a 2020 2020 2020  agesCopy).      
-00013b80: 2020 2020 2020 2020 2020 666f 7220 6f72            for or
-00013b90: 6465 722c 2069 2069 6e20 656e 756d 6572  der, i in enumer
-00013ba0: 6174 6528 6d65 7373 6167 6573 436f 7079  ate(messagesCopy
-00013bb0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00013bc0: 2020 2020 2020 2069 734c 6173 7449 7465         isLastIte
-00013bd0: 6d20 3d20 286f 7264 6572 203d 3d20 286d  m = (order == (m
-00013be0: 6573 7361 6765 4c65 6e67 7468 202d 2031  essageLength - 1
-00013bf0: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
-00013c00: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-00013c10: 2e6c 6c6d 496e 7465 7266 6163 6520 696e  .llmInterface in
-00013c20: 2028 2263 6861 7467 7074 222c 2022 6c65   ("chatgpt", "le
-00013c30: 746d 6564 6f69 7422 2920 616e 6420 6e6f  tmedoit") and no
-00013c40: 7420 6973 4c61 7374 4974 656d 2061 6e64  t isLastItem and
-00013c50: 2069 2e67 6574 2822 726f 6c65 222c 2022   i.get("role", "
-00013c60: 2229 203d 3d20 2275 7365 7222 2061 6e64  ") == "user" and
-00013c70: 2022 6675 6e63 7469 6f6e 5f63 616c 6c22   "function_call"
-00013c80: 2069 6e20 6d65 7373 6167 6573 436f 7079   in messagesCopy
-00013c90: 5b6f 7264 6572 2b31 5d3a 0a20 2020 2020  [order+1]:.     
-00013ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013cb0: 2020 2069 5b22 746f 6f6c 225d 203d 206d     i["tool"] = m
-00013cc0: 6573 7361 6765 7343 6f70 795b 6f72 6465  essagesCopy[orde
-00013cd0: 722b 315d 5b22 6675 6e63 7469 6f6e 5f63  r+1]["function_c
-00013ce0: 616c 6c22 5d2e 6765 7428 226e 616d 6522  all"].get("name"
-00013cf0: 2c20 2222 290a 2020 2020 2020 2020 2020  , "").          
-00013d00: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-00013d10: 2e73 6176 655f 6368 6174 5f72 6563 6f72  .save_chat_recor
-00013d20: 6428 7469 6d65 7374 616d 702c 206f 7264  d(timestamp, ord
-00013d30: 6572 2c20 6929 0a0a 2020 2020 2020 2020  er, i)..        
-00013d40: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00013d50: 2020 2020 2020 2020 2066 6f6c 6465 7250           folderP
-00013d60: 6174 6820 3d20 6f73 2e70 6174 682e 6a6f  ath = os.path.jo
-00013d70: 696e 2863 6f6e 6669 672e 6c6f 6361 6c53  in(config.localS
-00013d80: 746f 7261 6765 2c20 2263 6861 7473 222c  torage, "chats",
-00013d90: 2072 652e 7375 6228 225e 285b 302d 395d   re.sub("^([0-9]
-00013da0: 2b3f 5c2d 5b30 2d39 5d2b 3f29 5c2d 2e2a  +?\-[0-9]+?)\-.*
-00013db0: 3f24 222c 2072 225c 3122 2c20 7469 6d65  ?$", r"\1", time
-00013dc0: 7374 616d 7029 290a 2020 2020 2020 2020  stamp)).        
-00013dd0: 2020 2020 2020 2020 5061 7468 2866 6f6c          Path(fol
-00013de0: 6465 7250 6174 6829 2e6d 6b64 6972 2870  derPath).mkdir(p
-00013df0: 6172 656e 7473 3d54 7275 652c 2065 7869  arents=True, exi
-00013e00: 7374 5f6f 6b3d 5472 7565 290a 2020 2020  st_ok=True).    
-00013e10: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00013e20: 732e 7061 7468 2e69 7364 6972 2866 6f6c  s.path.isdir(fol
-00013e30: 6465 7250 6174 6829 3a0a 2020 2020 2020  derPath):.      
-00013e40: 2020 2020 2020 2020 2020 2020 2020 6368                ch
-00013e50: 6174 4669 6c65 203d 206f 732e 7061 7468  atFile = os.path
-00013e60: 2e6a 6f69 6e28 666f 6c64 6572 5061 7468  .join(folderPath
-00013e70: 2c20 6622 7b74 696d 6573 7461 6d70 7d2e  , f"{timestamp}.
-00013e80: 7478 7422 290a 2020 2020 2020 2020 2020  txt").          
-00013e90: 2020 2020 2020 2020 2020 7769 7468 206f            with o
-00013ea0: 7065 6e28 6368 6174 4669 6c65 2c20 2277  pen(chatFile, "w
-00013eb0: 222c 2065 6e63 6f64 696e 673d 2275 7466  ", encoding="utf
-00013ec0: 2d38 2229 2061 7320 6669 6c65 4f62 6a3a  -8") as fileObj:
-00013ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ee0: 2020 2020 2020 2020 2066 696c 654f 626a           fileObj
-00013ef0: 2e77 7269 7465 2870 7072 696e 742e 7066  .write(pprint.pf
-00013f00: 6f72 6d61 7428 6d65 7373 6167 6573 436f  ormat(messagesCo
-00013f10: 7079 2929 0a20 2020 2020 2020 2020 2020  py)).           
-00013f20: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00013f30: 2020 2020 2020 2020 2070 7269 6e74 3228           print2(
-00013f40: 2246 6169 6c65 6420 746f 2073 6176 6520  "Failed to save 
-00013f50: 6368 6174 215c 6e22 290a 2020 2020 2020  chat!\n").      
-00013f60: 2020 2020 2020 2020 2020 7368 6f77 4572            showEr
-00013f70: 726f 7273 2829 0a0a 2020 2020 6465 6620  rors()..    def 
-00013f80: 6578 706f 7274 4368 6174 2873 656c 662c  exportChat(self,
-00013f90: 206d 6573 7361 6765 732c 206f 7065 6e46   messages, openF
-00013fa0: 696c 653d 5472 7565 293a 0a20 2020 2020  ile=True):.     
-00013fb0: 2020 2069 6620 636f 6e66 6967 2e63 6f6e     if config.con
-00013fc0: 7665 7273 6174 696f 6e53 7461 7274 6564  versationStarted
-00013fd0: 3a0a 2020 2020 2020 2020 2020 2020 706c  :.            pl
-00013fe0: 6169 6e54 6578 7420 3d20 2222 0a20 2020  ainText = "".   
-00013ff0: 2020 2020 2020 2020 2074 696d 6573 7461           timesta
-00014000: 6d70 203d 2067 6574 4375 7272 656e 7444  mp = getCurrentD
-00014010: 6174 6554 696d 6528 290a 0a20 2020 2020  ateTime()..     
-00014020: 2020 2020 2020 2066 6f72 2069 2069 6e20         for i in 
-00014030: 6d65 7373 6167 6573 3a0a 2020 2020 2020  messages:.      
-00014040: 2020 2020 2020 2020 2020 6966 2069 5b22            if i["
-00014050: 726f 6c65 225d 203d 3d20 2275 7365 7222  role"] == "user"
-00014060: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014070: 2020 2020 2020 636f 6e74 656e 7420 3d20        content = 
-00014080: 695b 2263 6f6e 7465 6e74 225d 0a20 2020  i["content"].   
-00014090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000140a0: 2070 6c61 696e 5465 7874 202b 3d20 6622   plainText += f"
-000140b0: 3e3e 3e20 7b63 6f6e 7465 6e74 7d22 0a20  >>> {content}". 
-000140c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000140d0: 6620 695b 2272 6f6c 6522 5d20 3d3d 2022  f i["role"] == "
-000140e0: 6675 6e63 7469 6f6e 223a 0a20 2020 2020  function":.     
-000140f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014100: 6620 706c 6169 6e54 6578 743a 0a20 2020  f plainText:.   
-00014110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014120: 2020 2020 2070 6c61 696e 5465 7874 202b       plainText +
-00014130: 3d20 225c 6e5c 6e22 0a20 2020 2020 2020  = "\n\n".       
-00014140: 2020 2020 2020 2020 2020 2020 206e 616d               nam
-00014150: 6520 3d20 695b 226e 616d 6522 5d0a 2020  e = i["name"].  
-00014160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014170: 2020 706c 6169 6e54 6578 7420 2b3d 2066    plainText += f
-00014180: 2260 6060 5c6e 7b6e 616d 657d 5c6e 6060  "```\n{name}\n``
-00014190: 6022 0a20 2020 2020 2020 2020 2020 2020  `".             
-000141a0: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-000141b0: 2069 5b22 636f 6e74 656e 7422 5d0a 2020   i["content"].  
-000141c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000141d0: 2020 706c 6169 6e54 6578 7420 2b3d 2066    plainText += f
-000141e0: 225c 6e5c 6e7b 636f 6e74 656e 747d 5c6e  "\n\n{content}\n
-000141f0: 5c6e 220a 2020 2020 2020 2020 2020 2020  \n".            
-00014200: 2020 2020 656c 6966 2069 5b22 726f 6c65      elif i["role
-00014210: 225d 203d 3d20 2261 7373 6973 7461 6e74  "] == "assistant
-00014220: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00014230: 2020 2020 2020 2063 6f6e 7465 6e74 203d         content =
-00014240: 2069 5b22 636f 6e74 656e 7422 5d0a 2020   i["content"].  
-00014250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014260: 2020 6966 2063 6f6e 7465 6e74 2069 7320    if content is 
-00014270: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014290: 2020 6966 2070 6c61 696e 5465 7874 3a0a    if plainText:.
-000142a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142b0: 2020 2020 2020 2020 2020 2020 706c 6169              plai
-000142c0: 6e54 6578 7420 2b3d 2022 5c6e 5c6e 220a  nText += "\n\n".
-000142d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142e0: 2020 2020 2020 2020 706c 6169 6e54 6578          plainTex
-000142f0: 7420 2b3d 2066 227b 636f 6e74 656e 747d  t += f"{content}
-00014300: 5c6e 5c6e 220a 2020 2020 2020 2020 2020  \n\n".          
-00014310: 2020 706c 6169 6e54 6578 7420 3d20 706c    plainText = pl
-00014320: 6169 6e54 6578 742e 7374 7269 7028 290a  ainText.strip().
-00014330: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00014340: 6f6e 6669 672e 7465 726d 696e 616c 456e  onfig.terminalEn
-00014350: 6162 6c65 5465 726d 7578 4150 493a 0a20  ableTermuxAPI:. 
-00014360: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00014370: 7964 6f63 2e70 6970 6570 6167 6572 2870  ydoc.pipepager(p
-00014380: 6c61 696e 5465 7874 2c20 636d 643d 2274  lainText, cmd="t
-00014390: 6572 6d75 782d 7368 6172 6520 2d61 2073  ermux-share -a s
-000143a0: 656e 6422 290a 2020 2020 2020 2020 2020  end").          
-000143b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-000143c0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
-000143d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143e0: 2066 6f6c 6465 7250 6174 6820 3d20 6f73   folderPath = os
-000143f0: 2e70 6174 682e 6a6f 696e 2863 6f6e 6669  .path.join(confi
-00014400: 672e 6c6f 6361 6c53 746f 7261 6765 2c20  g.localStorage, 
-00014410: 2263 6861 7473 222c 2022 6578 706f 7274  "chats", "export
-00014420: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00014430: 2020 2020 2020 2050 6174 6828 666f 6c64         Path(fold
-00014440: 6572 5061 7468 292e 6d6b 6469 7228 7061  erPath).mkdir(pa
-00014450: 7265 6e74 733d 5472 7565 2c20 6578 6973  rents=True, exis
-00014460: 745f 6f6b 3d54 7275 6529 0a20 2020 2020  t_ok=True).     
-00014470: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014480: 6620 6f73 2e70 6174 682e 6973 6469 7228  f os.path.isdir(
-00014490: 666f 6c64 6572 5061 7468 293a 0a20 2020  folderPath):.   
-000144a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000144b0: 2020 2020 2063 6861 7446 696c 6520 3d20       chatFile = 
-000144c0: 6f73 2e70 6174 682e 6a6f 696e 2866 6f6c  os.path.join(fol
-000144d0: 6465 7250 6174 682c 2066 227b 7469 6d65  derPath, f"{time
-000144e0: 7374 616d 707d 2e74 7874 2229 0a20 2020  stamp}.txt").   
+0000d3b0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000d3c0: 2822 4f6c 6c61 6d61 206e 6f74 2066 6f75  ("Ollama not fou
+0000d3d0: 6e64 2120 496e 7374 616c 6c20 4f6c 6c61  nd! Install Olla
+0000d3e0: 6d61 2066 6972 7374 2074 6f20 7573 6520  ma first to use 
+0000d3f0: 4f6c 6c61 6d61 206d 6f64 656c 206c 6962  Ollama model lib
+0000d400: 7261 7279 2122 290a 2020 2020 2020 2020  rary!").        
+0000d410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d420: 2020 2020 7072 696e 7428 2254 6f20 696e      print("To in
+0000d430: 7374 616c 6c20 4f6c 6c61 6d61 2c20 7669  stall Ollama, vi
+0000d440: 7369 7420 6874 7470 733a 2f2f 6f6c 6c61  sit https://olla
+0000d450: 6d61 2e63 6f6d 2229 0a20 2020 2020 2020  ma.com").       
+0000d460: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000d470: 6665 6174 7572 6520 3d3d 2022 6465 6661  feature == "defa
+0000d480: 756c 7422 3a0a 2020 2020 2020 2020 2020  ult":.          
+0000d490: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000d4a0: 6e66 6967 2e6c 6c61 6d61 6370 704d 6169  nfig.llamacppMai
+0000d4b0: 6e4d 6f64 656c 5f6f 6c6c 616d 615f 7461  nModel_ollama_ta
+0000d4c0: 6720 3d20 6d6f 6465 6c0a 2020 2020 2020  g = model.      
+0000d4d0: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000d4e0: 6966 2066 6561 7475 7265 203d 3d20 2263  if feature == "c
+0000d4f0: 6f64 6522 3a0a 2020 2020 2020 2020 2020  ode":.          
+0000d500: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000d510: 6e66 6967 2e6c 6c61 6d61 6370 7043 6861  nfig.llamacppCha
+0000d520: 744d 6f64 656c 5f6f 6c6c 616d 615f 7461  tModel_ollama_ta
+0000d530: 6720 3d20 6d6f 6465 6c0a 2020 2020 2020  g = model.      
+0000d540: 2020 2020 2020 656c 6966 206c 6962 7261        elif libra
+0000d550: 7279 203d 3d20 2248 7567 6769 6e67 6661  ry == "Huggingfa
+0000d560: 6365 2048 7562 223a 0a20 2020 2020 2020  ce Hub":.       
+0000d570: 2020 2020 2020 2020 2064 6f77 6e6c 6f61           downloa
+0000d580: 6465 6447 6775 664d 6f64 656c 7320 3d20  dedGgufModels = 
+0000d590: 6765 7444 6f77 6e6c 6f61 6465 6447 6775  getDownloadedGgu
+0000d5a0: 664d 6f64 656c 7328 290a 2020 2020 2020  fModels().      
+0000d5b0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000d5c0: 2064 6f77 6e6c 6f61 6465 6447 6775 664d   downloadedGgufM
+0000d5d0: 6f64 656c 733a 0a20 2020 2020 2020 2020  odels:.         
+0000d5e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0000d5f0: 7365 7443 7573 746f 6d48 7567 6769 6e67  setCustomHugging
+0000d600: 6661 6365 4d6f 6465 6c28 6665 6174 7572  faceModel(featur
+0000d610: 653d 6665 6174 7572 6529 0a20 2020 2020  e=feature).     
+0000d620: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000d630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d640: 2020 2020 206d 6f64 656c 203d 2073 656c       model = sel
+0000d650: 662e 6469 616c 6f67 732e 6765 7456 616c  f.dialogs.getVal
+0000d660: 6964 4f70 7469 6f6e 7328 0a20 2020 2020  idOptions(.     
+0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d680: 2020 206f 7074 696f 6e73 3d6c 6973 7428     options=list(
+0000d690: 646f 776e 6c6f 6164 6564 4767 7566 4d6f  downloadedGgufMo
+0000d6a0: 6465 6c73 2e6b 6579 7328 2929 202b 205b  dels.keys()) + [
+0000d6b0: 224f 7468 6572 7320 2e2e 2e22 5d2c 0a20  "Others ..."],. 
+0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d6d0: 2020 2020 2020 2074 6974 6c65 3d22 4875         title="Hu
+0000d6e0: 6767 696e 6766 6163 6520 4875 6220 4d6f  ggingface Hub Mo
+0000d6f0: 6465 6c22 2c0a 2020 2020 2020 2020 2020  del",.          
+0000d700: 2020 2020 2020 2020 2020 2020 2020 6465                de
+0000d710: 6661 756c 743d 2222 2069 6620 2e2e 2e20  fault="" if ... 
+0000d720: 656c 7365 2022 222c 0a20 2020 2020 2020  else "",.       
+0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d740: 2074 6578 743d 2253 656c 6563 7420 6120   text="Select a 
+0000d750: 6875 6767 696e 6766 6163 6520 6d6f 6465  huggingface mode
+0000d760: 6c3a 222c 0a20 2020 2020 2020 2020 2020  l:",.           
+0000d770: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000d780: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000d790: 6620 6d6f 6465 6c3a 0a20 2020 2020 2020  f model:.       
+0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7b0: 2069 6620 6d6f 6465 6c20 3d3d 2022 4f74   if model == "Ot
+0000d7c0: 6865 7273 202e 2e2e 223a 0a20 2020 2020  hers ...":.     
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 2020 2020 2020 2073 656c 662e 7365 7443         self.setC
+0000d7f0: 7573 746f 6d48 7567 6769 6e67 6661 6365  ustomHuggingface
+0000d800: 4d6f 6465 6c28 6665 6174 7572 653d 6665  Model(feature=fe
+0000d810: 6174 7572 6529 0a20 2020 2020 2020 2020  ature).         
+0000d820: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000d830: 6c69 6620 6665 6174 7572 6520 3d3d 2022  lif feature == "
+0000d840: 6465 6661 756c 7422 3a0a 2020 2020 2020  default":.      
+0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d860: 2020 2020 2020 636f 6e66 6967 2e6c 6c61        config.lla
+0000d870: 6d61 6370 704d 6169 6e4d 6f64 656c 5f6d  macppMainModel_m
+0000d880: 6f64 656c 5f70 6174 6820 3d20 646f 776e  odel_path = down
+0000d890: 6c6f 6164 6564 4767 7566 4d6f 6465 6c73  loadedGgufModels
+0000d8a0: 5b6d 6f64 656c 5d0a 2020 2020 2020 2020  [model].        
+0000d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8c0: 656c 6966 2066 6561 7475 7265 203d 3d20  elif feature == 
+0000d8d0: 2263 6f64 6522 3a0a 2020 2020 2020 2020  "code":.        
+0000d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8f0: 2020 2020 636f 6e66 6967 2e6c 6c61 6d61      config.llama
+0000d900: 6370 7043 6861 744d 6f64 656c 5f6d 6f64  cppChatModel_mod
+0000d910: 656c 5f70 6174 6820 3d20 646f 776e 6c6f  el_path = downlo
+0000d920: 6164 6564 4767 7566 4d6f 6465 6c73 5b6d  adedGgufModels[m
+0000d930: 6f64 656c 5d0a 2020 2020 2020 2020 2020  odel].          
+0000d940: 2020 656c 6966 206c 6962 7261 7279 203d    elif library =
+0000d950: 3d20 2243 7573 746f 6d20 4747 5546 223a  = "Custom GGUF":
+0000d960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d970: 2073 656c 662e 7365 7443 7573 746f 6d4d   self.setCustomM
+0000d980: 6f64 656c 5061 7468 2866 6561 7475 7265  odelPath(feature
+0000d990: 3d66 6561 7475 7265 290a 0a20 2020 2064  =feature)..    d
+0000d9a0: 6566 2073 6574 4375 7374 6f6d 4d6f 6465  ef setCustomMode
+0000d9b0: 6c50 6174 6828 7365 6c66 2c20 6665 6174  lPath(self, feat
+0000d9c0: 7572 653d 2264 6566 6175 6c74 2229 3a0a  ure="default"):.
+0000d9d0: 2020 2020 2020 2020 6d6f 6465 6c5f 7061          model_pa
+0000d9e0: 7468 203d 2073 656c 662e 6765 7450 6174  th = self.getPat
+0000d9f0: 682e 6765 7446 696c 6550 6174 6828 0a20  h.getFilePath(. 
+0000da00: 2020 2020 2020 2020 2020 2063 6865 636b             check
+0000da10: 5f69 7366 696c 653d 5472 7565 2c0a 2020  _isfile=True,.  
+0000da20: 2020 2020 2020 2020 2020 656d 7074 795f            empty_
+0000da30: 746f 5f63 616e 6365 6c3d 5472 7565 2c0a  to_cancel=True,.
+0000da40: 2020 2020 2020 2020 2020 2020 6c69 7374              list
+0000da50: 5f63 6f6e 7465 6e74 5f6f 6e5f 6469 7265  _content_on_dire
+0000da60: 6374 6f72 795f 6368 616e 6765 3d54 7275  ctory_change=Tru
+0000da70: 652c 0a20 2020 2020 2020 2020 2020 206b  e,.            k
+0000da80: 6565 705f 7374 6172 7475 705f 6469 7265  eep_startup_dire
+0000da90: 6374 6f72 793d 5472 7565 2c0a 2020 2020  ctory=True,.    
+0000daa0: 2020 2020 2020 2020 6d65 7373 6167 653d          message=
+0000dab0: 2245 6e74 6572 2061 2063 7573 746f 6d20  "Enter a custom 
+0000dac0: 6d6f 6465 6c20 7061 7468 3a22 2c0a 2020  model path:",.  
+0000dad0: 2020 2020 2020 2020 2020 6465 6661 756c            defaul
+0000dae0: 743d 636f 6e66 6967 2e6c 6c61 6d61 6370  t=config.llamacp
+0000daf0: 7043 6861 744d 6f64 656c 5f6d 6f64 656c  pChatModel_model
+0000db00: 5f70 6174 6820 6966 2066 6561 7475 7265  _path if feature
+0000db10: 203d 3d20 2263 6f64 6522 2065 6c73 6520   == "code" else 
+0000db20: 636f 6e66 6967 2e6c 6c61 6d61 6370 704d  config.llamacppM
+0000db30: 6169 6e4d 6f64 656c 5f6d 6f64 656c 5f70  ainModel_model_p
+0000db40: 6174 682c 0a20 2020 2020 2020 2029 0a20  ath,.        ). 
+0000db50: 2020 2020 2020 2069 6620 6d6f 6465 6c5f         if model_
+0000db60: 7061 7468 2061 6e64 206f 732e 7061 7468  path and os.path
+0000db70: 2e69 7366 696c 6528 6d6f 6465 6c5f 7061  .isfile(model_pa
+0000db80: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
+0000db90: 2069 6620 6665 6174 7572 6520 3d3d 2022   if feature == "
+0000dba0: 6465 6661 756c 7422 3a0a 2020 2020 2020  default":.      
+0000dbb0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0000dbc0: 2e6c 6c61 6d61 6370 704d 6169 6e4d 6f64  .llamacppMainMod
+0000dbd0: 656c 5f6d 6f64 656c 5f70 6174 6820 3d20  el_model_path = 
+0000dbe0: 6d6f 6465 6c5f 7061 7468 0a20 2020 2020  model_path.     
+0000dbf0: 2020 2020 2020 2065 6c69 6620 6665 6174         elif feat
+0000dc00: 7572 6520 3d3d 2022 636f 6465 223a 0a20  ure == "code":. 
+0000dc10: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000dc20: 6f6e 6669 672e 6c6c 616d 6163 7070 4368  onfig.llamacppCh
+0000dc30: 6174 4d6f 6465 6c5f 6d6f 6465 6c5f 7061  atModel_model_pa
+0000dc40: 7468 203d 206d 6f64 656c 5f70 6174 680a  th = model_path.
+0000dc50: 0a20 2020 2064 6566 2073 6574 4375 7374  .    def setCust
+0000dc60: 6f6d 4875 6767 696e 6766 6163 654d 6f64  omHuggingfaceMod
+0000dc70: 656c 2873 656c 662c 2066 6561 7475 7265  el(self, feature
+0000dc80: 3d22 6465 6661 756c 7422 293a 0a20 2020  ="default"):.   
+0000dc90: 2020 2020 2068 6973 746f 7279 466f 6c64       historyFold
+0000dca0: 6572 203d 206f 732e 7061 7468 2e6a 6f69  er = os.path.joi
+0000dcb0: 6e28 636f 6e66 6967 2e6c 6f63 616c 5374  n(config.localSt
+0000dcc0: 6f72 6167 652c 2022 6869 7374 6f72 7922  orage, "history"
+0000dcd0: 290a 2020 2020 2020 2020 5061 7468 2868  ).        Path(h
+0000dce0: 6973 746f 7279 466f 6c64 6572 292e 6d6b  istoryFolder).mk
+0000dcf0: 6469 7228 7061 7265 6e74 733d 5472 7565  dir(parents=True
+0000dd00: 2c20 6578 6973 745f 6f6b 3d54 7275 6529  , exist_ok=True)
+0000dd10: 0a20 2020 2020 2020 2072 6570 6f5f 6964  .        repo_id
+0000dd20: 5f68 6973 746f 7279 203d 206f 732e 7061  _history = os.pa
+0000dd30: 7468 2e6a 6f69 6e28 6869 7374 6f72 7946  th.join(historyF
+0000dd40: 6f6c 6465 722c 2022 6c6c 616d 6163 7070  older, "llamacpp
+0000dd50: 5f63 6f64 655f 7265 706f 5f69 6422 2069  _code_repo_id" i
+0000dd60: 6620 6665 6174 7572 6520 3d3d 2022 636f  f feature == "co
+0000dd70: 6465 2220 656c 7365 2022 6c6c 616d 6163  de" else "llamac
+0000dd80: 7070 5f64 6566 6175 6c74 5f72 6570 6f5f  pp_default_repo_
+0000dd90: 6964 2229 0a20 2020 2020 2020 2072 6570  id").        rep
+0000dda0: 6f5f 6964 5f73 6573 7369 6f6e 203d 2050  o_id_session = P
+0000ddb0: 726f 6d70 7453 6573 7369 6f6e 2868 6973  romptSession(his
+0000ddc0: 746f 7279 3d46 696c 6548 6973 746f 7279  tory=FileHistory
+0000ddd0: 2872 6570 6f5f 6964 5f68 6973 746f 7279  (repo_id_history
+0000dde0: 2929 0a20 2020 2020 2020 2066 696c 656e  )).        filen
+0000ddf0: 616d 655f 6869 7374 6f72 7920 3d20 6f73  ame_history = os
+0000de00: 2e70 6174 682e 6a6f 696e 2868 6973 746f  .path.join(histo
+0000de10: 7279 466f 6c64 6572 2c20 226c 6c61 6d61  ryFolder, "llama
+0000de20: 6370 705f 636f 6465 5f66 696c 656e 616d  cpp_code_filenam
+0000de30: 6522 2069 6620 6665 6174 7572 6520 3d3d  e" if feature ==
+0000de40: 2022 636f 6465 2220 656c 7365 2022 6c6c   "code" else "ll
+0000de50: 616d 6163 7070 5f64 6566 6175 6c74 5f66  amacpp_default_f
+0000de60: 696c 656e 616d 6522 290a 2020 2020 2020  ilename").      
+0000de70: 2020 6669 6c65 6e61 6d65 5f73 6573 7369    filename_sessi
+0000de80: 6f6e 203d 2050 726f 6d70 7453 6573 7369  on = PromptSessi
+0000de90: 6f6e 2868 6973 746f 7279 3d46 696c 6548  on(history=FileH
+0000dea0: 6973 746f 7279 2866 696c 656e 616d 655f  istory(filename_
+0000deb0: 6869 7374 6f72 7929 290a 2020 2020 2020  history)).      
+0000dec0: 2020 626f 7474 6f6d 5f74 6f6f 6c62 6172    bottom_toolbar
+0000ded0: 203d 2066 2222 2220 7b73 7472 2863 6f6e   = f""" {str(con
+0000dee0: 6669 672e 686f 746b 6579 5f65 7869 7429  fig.hotkey_exit)
+0000def0: 2e72 6570 6c61 6365 2822 2722 2c20 2222  .replace("'", ""
+0000df00: 297d 207b 636f 6e66 6967 2e65 7869 745f  )} {config.exit_
+0000df10: 656e 7472 797d 2222 220a 2020 2020 2020  entry}""".      
+0000df20: 2020 7072 696e 7431 2822 506c 6561 7365    print1("Please
+0000df30: 2073 7065 6369 6679 2074 6865 2068 7567   specify the hug
+0000df40: 6769 6e67 6661 6365 2072 6570 6f20 6964  gingface repo id
+0000df50: 206f 6620 6120 2a2e 6767 7566 206d 6f64   of a *.gguf mod
+0000df60: 656c 3a22 290a 2020 2020 2020 2020 7265  el:").        re
+0000df70: 706f 5f69 6420 3d20 7365 6c66 2e70 726f  po_id = self.pro
+0000df80: 6d70 7473 2e73 696d 706c 6550 726f 6d70  mpts.simplePromp
+0000df90: 7428 7374 796c 653d 7365 6c66 2e70 726f  t(style=self.pro
+0000dfa0: 6d70 7473 2e70 726f 6d70 7453 7479 6c65  mpts.promptStyle
+0000dfb0: 322c 2070 726f 6d70 7453 6573 7369 6f6e  2, promptSession
+0000dfc0: 3d72 6570 6f5f 6964 5f73 6573 7369 6f6e  =repo_id_session
+0000dfd0: 2c20 626f 7474 6f6d 5f74 6f6f 6c62 6172  , bottom_toolbar
+0000dfe0: 3d62 6f74 746f 6d5f 746f 6f6c 6261 722c  =bottom_toolbar,
+0000dff0: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
+0000e000: 6c6c 616d 6163 7070 4368 6174 4d6f 6465  llamacppChatMode
+0000e010: 6c5f 7265 706f 5f69 6420 6966 2066 6561  l_repo_id if fea
+0000e020: 7475 7265 203d 3d20 2263 6f64 6522 2065  ture == "code" e
+0000e030: 6c73 6520 636f 6e66 6967 2e6c 6c61 6d61  lse config.llama
+0000e040: 6370 704d 6169 6e4d 6f64 656c 5f72 6570  cppMainModel_rep
+0000e050: 6f5f 6964 290a 2020 2020 2020 2020 7072  o_id).        pr
+0000e060: 696e 7432 2822 506c 6561 7365 2073 7065  int2("Please spe
+0000e070: 6369 6679 2061 2066 696c 656e 616d 6520  cify a filename 
+0000e080: 6f72 2067 6c6f 6220 7061 7474 6572 6e20  or glob pattern 
+0000e090: 746f 206d 6174 6368 2074 6865 206d 6f64  to match the mod
+0000e0a0: 656c 2066 696c 6520 696e 2074 6865 2072  el file in the r
+0000e0b0: 6570 6f3a 2229 0a20 2020 2020 2020 2066  epo:").        f
+0000e0c0: 696c 656e 616d 6520 3d20 7365 6c66 2e70  ilename = self.p
+0000e0d0: 726f 6d70 7473 2e73 696d 706c 6550 726f  rompts.simplePro
+0000e0e0: 6d70 7428 7374 796c 653d 7365 6c66 2e70  mpt(style=self.p
+0000e0f0: 726f 6d70 7473 2e70 726f 6d70 7453 7479  rompts.promptSty
+0000e100: 6c65 322c 2070 726f 6d70 7453 6573 7369  le2, promptSessi
+0000e110: 6f6e 3d66 696c 656e 616d 655f 7365 7373  on=filename_sess
+0000e120: 696f 6e2c 2062 6f74 746f 6d5f 746f 6f6c  ion, bottom_tool
+0000e130: 6261 723d 626f 7474 6f6d 5f74 6f6f 6c62  bar=bottom_toolb
+0000e140: 6172 2c20 6465 6661 756c 743d 636f 6e66  ar, default=conf
+0000e150: 6967 2e6c 6c61 6d61 6370 7043 6861 744d  ig.llamacppChatM
+0000e160: 6f64 656c 5f66 696c 656e 616d 6520 6966  odel_filename if
+0000e170: 2066 6561 7475 7265 203d 3d20 2263 6f64   feature == "cod
+0000e180: 6522 2065 6c73 6520 636f 6e66 6967 2e6c  e" else config.l
+0000e190: 6c61 6d61 6370 704d 6169 6e4d 6f64 656c  lamacppMainModel
+0000e1a0: 5f66 696c 656e 616d 6529 0a20 2020 2020  _filename).     
+0000e1b0: 2020 2069 6620 2872 6570 6f5f 6964 2061     if (repo_id a
+0000e1c0: 6e64 206e 6f74 2072 6570 6f5f 6964 2e6c  nd not repo_id.l
+0000e1d0: 6f77 6572 2829 203d 3d20 636f 6e66 6967  ower() == config
+0000e1e0: 2e65 7869 745f 656e 7472 7929 2061 6e64  .exit_entry) and
+0000e1f0: 2028 6669 6c65 6e61 6d65 2061 6e64 206e   (filename and n
+0000e200: 6f74 2066 696c 656e 616d 652e 6c6f 7765  ot filename.lowe
+0000e210: 7228 2920 3d3d 2063 6f6e 6669 672e 6578  r() == config.ex
+0000e220: 6974 5f65 6e74 7279 293a 0a20 2020 2020  it_entry):.     
+0000e230: 2020 2020 2020 2069 6620 6665 6174 7572         if featur
+0000e240: 6520 3d3d 2022 6465 6661 756c 7422 3a0a  e == "default":.
+0000e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e260: 636f 6e66 6967 2e6c 6c61 6d61 6370 704d  config.llamacppM
+0000e270: 6169 6e4d 6f64 656c 5f72 6570 6f5f 6964  ainModel_repo_id
+0000e280: 203d 2072 6570 6f5f 6964 0a20 2020 2020   = repo_id.     
+0000e290: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+0000e2a0: 672e 6c6c 616d 6163 7070 4d61 696e 4d6f  g.llamacppMainMo
+0000e2b0: 6465 6c5f 6669 6c65 6e61 6d65 203d 2066  del_filename = f
+0000e2c0: 696c 656e 616d 650a 2020 2020 2020 2020  ilename.        
+0000e2d0: 2020 2020 2020 2020 636f 6e66 6967 2e6c          config.l
+0000e2e0: 6c61 6d61 6370 704d 6169 6e4d 6f64 656c  lamacppMainModel
+0000e2f0: 5f6d 6f64 656c 5f70 6174 6820 3d20 2222  _model_path = ""
+0000e300: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000e310: 6620 6665 6174 7572 6520 3d3d 2022 636f  f feature == "co
+0000e320: 6465 223a 0a20 2020 2020 2020 2020 2020  de":.           
+0000e330: 2020 2020 2063 6f6e 6669 672e 6c6c 616d       config.llam
+0000e340: 6163 7070 4368 6174 4d6f 6465 6c5f 7265  acppChatModel_re
+0000e350: 706f 5f69 6420 3d20 7265 706f 5f69 640a  po_id = repo_id.
+0000e360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e370: 636f 6e66 6967 2e6c 6c61 6d61 6370 7043  config.llamacppC
+0000e380: 6861 744d 6f64 656c 5f66 696c 656e 616d  hatModel_filenam
+0000e390: 6520 3d20 6669 6c65 6e61 6d65 0a20 2020  e = filename.   
+0000e3a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000e3b0: 6669 672e 6c6c 616d 6163 7070 4368 6174  fig.llamacppChat
+0000e3c0: 4d6f 6465 6c5f 6d6f 6465 6c5f 7061 7468  Model_model_path
+0000e3d0: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
+0000e3e0: 2020 4361 6c6c 4c4c 4d2e 6368 6563 6b43    CallLLM.checkC
+0000e3f0: 6f6d 706c 6574 696f 6e28 290a 2020 2020  ompletion().    
+0000e400: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000e410: 2020 2020 2020 7072 696e 7432 2822 4163        print2("Ac
+0000e420: 7469 6f6e 2063 616e 6365 6c6c 6564 2064  tion cancelled d
+0000e430: 7565 2074 6f20 696e 7375 6666 6963 6965  ue to insufficie
+0000e440: 6e74 2069 6e66 6f72 6d61 7469 6f6e 2122  nt information!"
+0000e450: 290a 0a20 2020 2064 6566 2073 6574 4c6c  )..    def setLl
+0000e460: 6d4d 6f64 656c 5f63 6861 7467 7074 2873  mModel_chatgpt(s
+0000e470: 656c 6629 3a0a 2020 2020 2020 2020 6d6f  elf):.        mo
+0000e480: 6465 6c20 3d20 7365 6c66 2e64 6961 6c6f  del = self.dialo
+0000e490: 6773 2e67 6574 5661 6c69 644f 7074 696f  gs.getValidOptio
+0000e4a0: 6e73 280a 2020 2020 2020 2020 2020 2020  ns(.            
+0000e4b0: 6f70 7469 6f6e 733d 7365 6c66 2e6d 6f64  options=self.mod
+0000e4c0: 656c 732c 0a20 2020 2020 2020 2020 2020  els,.           
+0000e4d0: 2074 6974 6c65 3d22 4675 6e63 7469 6f6e   title="Function
+0000e4e0: 2043 616c 6c69 6e67 204d 6f64 656c 222c   Calling Model",
+0000e4f0: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+0000e500: 6175 6c74 3d63 6f6e 6669 672e 6368 6174  ault=config.chat
+0000e510: 4750 5441 7069 4d6f 6465 6c20 6966 2063  GPTApiModel if c
+0000e520: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
+0000e530: 4d6f 6465 6c20 696e 2073 656c 662e 6d6f  Model in self.mo
+0000e540: 6465 6c73 2065 6c73 6520 7365 6c66 2e6d  dels else self.m
+0000e550: 6f64 656c 735b 305d 2c0a 2020 2020 2020  odels[0],.      
+0000e560: 2020 2020 2020 7465 7874 3d22 5365 6c65        text="Sele
+0000e570: 6374 2061 2066 756e 6374 696f 6e20 6361  ct a function ca
+0000e580: 6c6c 206d 6f64 656c 3a5c 6e28 666f 7220  ll model:\n(for 
+0000e590: 626f 7468 2063 6861 7420 616e 6420 7461  both chat and ta
+0000e5a0: 736b 2065 7865 6375 7469 6f6e 2922 2c0a  sk execution)",.
+0000e5b0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e5c0: 2020 6966 206d 6f64 656c 3a0a 2020 2020    if model:.    
+0000e5d0: 2020 2020 2020 2020 636f 6e66 6967 2e63          config.c
+0000e5e0: 6861 7447 5054 4170 694d 6f64 656c 203d  hatGPTApiModel =
+0000e5f0: 206d 6f64 656c 0a20 2020 2020 2020 2020   model.         
+0000e600: 2020 2070 7269 6e74 3328 6622 4368 6174     print3(f"Chat
+0000e610: 4750 5420 6d6f 6465 6c3a 207b 6d6f 6465  GPT model: {mode
+0000e620: 6c7d 2229 0a20 2020 2020 2020 2020 2020  l}").           
+0000e630: 2023 2073 6574 206d 6178 2074 6f6b 656e   # set max token
+0000e640: 730a 2020 2020 2020 2020 2020 2020 636f  s.            co
+0000e650: 6e66 6967 2e63 6861 7447 5054 4170 694d  nfig.chatGPTApiM
+0000e660: 6178 546f 6b65 6e73 203d 2073 656c 662e  axTokens = self.
+0000e670: 6765 744d 6178 546f 6b65 6e73 2829 5b2d  getMaxTokens()[-
+0000e680: 315d 0a20 2020 2020 2020 2020 2020 2070  1].            p
+0000e690: 7269 6e74 3328 6622 4d61 7869 6d75 6d20  rint3(f"Maximum 
+0000e6a0: 6f75 7470 7574 2074 6f6b 656e 733a 207b  output tokens: {
+0000e6b0: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
+0000e6c0: 694d 6178 546f 6b65 6e73 7d22 290a 0a20  iMaxTokens}").. 
+0000e6d0: 2020 2064 6566 2073 6574 4368 6174 626f     def setChatbo
+0000e6e0: 7428 7365 6c66 293a 0a20 2020 2020 2020  t(self):.       
+0000e6f0: 206d 6f64 656c 203d 2073 656c 662e 6469   model = self.di
+0000e700: 616c 6f67 732e 6765 7456 616c 6964 4f70  alogs.getValidOp
+0000e710: 7469 6f6e 7328 0a20 2020 2020 2020 2020  tions(.         
+0000e720: 2020 206f 7074 696f 6e73 3d28 2263 6861     options=("cha
+0000e730: 7467 7074 222c 2022 6765 6d69 6e69 7072  tgpt", "geminipr
+0000e740: 6f22 2c20 2270 616c 6d32 222c 2022 636f  o", "palm2", "co
+0000e750: 6465 7922 292c 0a20 2020 2020 2020 2020  dey"),.         
+0000e760: 2020 2074 6974 6c65 3d22 4368 6174 2d6f     title="Chat-o
+0000e770: 6e6c 7920 6d6f 6465 6c22 2c0a 2020 2020  nly model",.    
+0000e780: 2020 2020 2020 2020 6465 6661 756c 743d          default=
+0000e790: 636f 6e66 6967 2e63 6861 7462 6f74 2c0a  config.chatbot,.
+0000e7a0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+0000e7b0: 3d22 5365 6c65 6374 2064 6566 6175 6c74  ="Select default
+0000e7c0: 2063 6861 742d 6f6e 6c79 206d 6f64 656c   chat-only model
+0000e7d0: 3a5c 6e28 4465 6661 756c 7420 6d6f 6465  :\n(Default mode
+0000e7e0: 6c20 6973 206c 6f61 6465 6420 7768 656e  l is loaded when
+0000e7f0: 2079 6f75 2069 6e63 6c75 6465 2027 5b43   you include '[C
+0000e800: 4841 545d 2720 696e 2079 6f75 7220 696e  HAT]' in your in
+0000e810: 7075 7429 222c 0a20 2020 2020 2020 2029  put)",.        )
+0000e820: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+0000e830: 6c3a 0a20 2020 2020 2020 2020 2020 2063  l:.            c
+0000e840: 6f6e 6669 672e 6368 6174 626f 7420 3d20  onfig.chatbot = 
+0000e850: 6d6f 6465 6c0a 2020 2020 2020 2020 2020  model.          
+0000e860: 2020 7072 696e 7433 2866 2243 6861 742d    print3(f"Chat-
+0000e870: 6f6e 6c79 206d 6f64 656c 3a20 7b6d 6f64  only model: {mod
+0000e880: 656c 7d22 290a 0a20 2020 2064 6566 2073  el}")..    def s
+0000e890: 6574 456d 6265 6464 696e 674d 6f64 656c  etEmbeddingModel
+0000e8a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000e8b0: 6f6c 6445 6d62 6564 6469 6e67 4d6f 6465  oldEmbeddingMode
+0000e8c0: 6c20 3d20 636f 6e66 6967 2e65 6d62 6564  l = config.embed
+0000e8d0: 6469 6e67 4d6f 6465 6c0a 2020 2020 2020  dingModel.      
+0000e8e0: 2020 6d6f 6465 6c20 3d20 7365 6c66 2e64    model = self.d
+0000e8f0: 6961 6c6f 6773 2e67 6574 5661 6c69 644f  ialogs.getValidO
+0000e900: 7074 696f 6e73 280a 2020 2020 2020 2020  ptions(.        
+0000e910: 2020 2020 6f70 7469 6f6e 733d 2822 7465      options=("te
+0000e920: 7874 2d65 6d62 6564 6469 6e67 2d33 2d6c  xt-embedding-3-l
+0000e930: 6172 6765 222c 2022 7465 7874 2d65 6d62  arge", "text-emb
+0000e940: 6564 6469 6e67 2d33 2d73 6d61 6c6c 222c  edding-3-small",
+0000e950: 2022 7465 7874 2d65 6d62 6564 6469 6e67   "text-embedding
+0000e960: 2d61 6461 2d30 3032 222c 2022 7061 7261  -ada-002", "para
+0000e970: 7068 7261 7365 2d6d 756c 7469 6c69 6e67  phrase-multiling
+0000e980: 7561 6c2d 6d70 6e65 742d 6261 7365 2d76  ual-mpnet-base-v
+0000e990: 3222 2c20 2261 6c6c 2d6d 706e 6574 2d62  2", "all-mpnet-b
+0000e9a0: 6173 652d 7632 222c 2022 616c 6c2d 4d69  ase-v2", "all-Mi
+0000e9b0: 6e69 4c4d 2d4c 362d 7632 222c 2022 6375  niLM-L6-v2", "cu
+0000e9c0: 7374 6f6d 2229 2c0a 2020 2020 2020 2020  stom"),.        
+0000e9d0: 2020 2020 7469 746c 653d 2245 6d62 6564      title="Embed
+0000e9e0: 6469 6e67 206d 6f64 656c 222c 0a20 2020  ding model",.   
+0000e9f0: 2020 2020 2020 2020 2064 6566 6175 6c74           default
+0000ea00: 3d63 6f6e 6669 672e 656d 6265 6464 696e  =config.embeddin
+0000ea10: 674d 6f64 656c 2c0a 2020 2020 2020 2020  gModel,.        
+0000ea20: 2020 2020 7465 7874 3d22 5365 6c65 6374      text="Select
+0000ea30: 2061 6e20 656d 6265 6464 696e 6720 6d6f   an embedding mo
+0000ea40: 6465 6c3a 222c 0a20 2020 2020 2020 2029  del:",.        )
+0000ea50: 0a20 2020 2020 2020 2069 6620 6d6f 6465  .        if mode
+0000ea60: 6c3a 0a20 2020 2020 2020 2020 2020 2069  l:.            i
+0000ea70: 6620 6d6f 6465 6c20 3d3d 2022 6375 7374  f model == "cust
+0000ea80: 6f6d 223a 0a20 2020 2020 2020 2020 2020  om":.           
+0000ea90: 2020 2020 2070 7269 6e74 3128 2245 6e74       print1("Ent
+0000eaa0: 6572 204f 7065 6e41 4920 6f72 2053 656e  er OpenAI or Sen
+0000eab0: 7465 6e63 6520 5472 616e 7366 6f72 6d65  tence Transforme
+0000eac0: 7220 456d 6265 6464 696e 6720 6d6f 6465  r Embedding mode
+0000ead0: 6c3a 2229 0a20 2020 2020 2020 2020 2020  l:").           
+0000eae0: 2020 2020 2070 7269 6e74 3128 2252 6561       print1("Rea
+0000eaf0: 6420 6d6f 7265 2061 743a 2068 7474 7073  d more at: https
+0000eb00: 3a2f 2f77 7777 2e73 6265 7274 2e6e 6574  ://www.sbert.net
+0000eb10: 2f64 6f63 732f 7072 6574 7261 696e 6564  /docs/pretrained
+0000eb20: 5f6d 6f64 656c 732e 6874 6d6c 2229 0a20  _models.html"). 
+0000eb30: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000eb40: 7573 746f 6d4d 6f64 656c 203d 2073 656c  ustomModel = sel
+0000eb50: 662e 7072 6f6d 7074 732e 7369 6d70 6c65  f.prompts.simple
+0000eb60: 5072 6f6d 7074 2873 7479 6c65 3d73 656c  Prompt(style=sel
+0000eb70: 662e 7072 6f6d 7074 732e 7072 6f6d 7074  f.prompts.prompt
+0000eb80: 5374 796c 6532 2c20 6465 6661 756c 743d  Style2, default=
+0000eb90: 636f 6e66 6967 2e65 6d62 6564 6469 6e67  config.embedding
+0000eba0: 4d6f 6465 6c29 0a20 2020 2020 2020 2020  Model).         
+0000ebb0: 2020 2020 2020 2069 6620 6375 7374 6f6d         if custom
+0000ebc0: 4d6f 6465 6c20 616e 6420 6e6f 7420 6375  Model and not cu
+0000ebd0: 7374 6f6d 4d6f 6465 6c2e 7374 7269 7028  stomModel.strip(
+0000ebe0: 292e 6c6f 7765 7228 2920 3d3d 2063 6f6e  ).lower() == con
+0000ebf0: 6669 672e 6578 6974 5f65 6e74 7279 3a0a  fig.exit_entry:.
+0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec10: 2020 2020 636f 6e66 6967 2e65 6d62 6564      config.embed
+0000ec20: 6469 6e67 4d6f 6465 6c20 3d20 6375 7374  dingModel = cust
+0000ec30: 6f6d 4d6f 6465 6c20 0a20 2020 2020 2020  omModel .       
+0000ec40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000ec50: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+0000ec60: 672e 656d 6265 6464 696e 674d 6f64 656c  g.embeddingModel
+0000ec70: 203d 206d 6f64 656c 0a20 2020 2020 2020   = model.       
+0000ec80: 2020 2020 2070 7269 6e74 3328 6622 456d       print3(f"Em
+0000ec90: 6265 6464 696e 6720 6d6f 6465 6c3a 207b  bedding model: {
+0000eca0: 6d6f 6465 6c7d 2229 0a20 2020 2020 2020  model}").       
+0000ecb0: 2069 6620 6e6f 7420 6f6c 6445 6d62 6564   if not oldEmbed
+0000ecc0: 6469 6e67 4d6f 6465 6c20 3d3d 2063 6f6e  dingModel == con
+0000ecd0: 6669 672e 656d 6265 6464 696e 674d 6f64  fig.embeddingMod
+0000ece0: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+0000ecf0: 7072 696e 7431 2866 2259 6f75 2776 6520  print1(f"You've 
+0000ed00: 6368 616e 6765 2074 6865 2065 6d62 6564  change the embed
+0000ed10: 6469 6e67 206d 6f64 656c 2066 726f 6d20  ding model from 
+0000ed20: 277b 6f6c 6445 6d62 6564 6469 6e67 4d6f  '{oldEmbeddingMo
+0000ed30: 6465 6c7d 2720 746f 2027 7b63 6f6e 6669  del}' to '{confi
+0000ed40: 672e 656d 6265 6464 696e 674d 6f64 656c  g.embeddingModel
+0000ed50: 7d27 2e22 290a 2020 2020 2020 2020 2020  }'.").          
+0000ed60: 2020 7072 696e 7431 2822 546f 2077 6f72    print1("To wor
+0000ed70: 6b20 7769 7468 2074 6865 206e 6577 6c79  k with the newly
+0000ed80: 2073 656c 6563 7465 6420 6d6f 6465 6c2c   selected model,
+0000ed90: 2070 7265 7669 6f75 7320 6d65 6d6f 7279   previous memory
+0000eda0: 2073 746f 7265 2061 6e64 2072 6574 7269   store and retri
+0000edb0: 6576 6564 2063 6f6c 6c65 6374 696f 6e73  eved collections
+0000edc0: 206e 6565 6420 746f 2062 6520 6465 6c65   need to be dele
+0000edd0: 7465 642e 2229 0a20 2020 2020 2020 2020  ted.").         
+0000ede0: 2020 2070 7269 6e74 3128 2244 6f20 796f     print1("Do yo
+0000edf0: 7520 7761 6e74 2074 6f20 6465 6c65 7465  u want to delete
+0000ee00: 2074 6865 6d20 6e6f 773f 205b 795d 6573   them now? [y]es
+0000ee10: 202f 205b 4e5d 6f22 290a 2020 2020 2020   / [N]o").      
+0000ee20: 2020 2020 2020 636f 6e66 6972 6d61 7469        confirmati
+0000ee30: 6f6e 203d 2073 656c 662e 7072 6f6d 7074  on = self.prompt
+0000ee40: 732e 7369 6d70 6c65 5072 6f6d 7074 2873  s.simplePrompt(s
+0000ee50: 7479 6c65 3d73 656c 662e 7072 6f6d 7074  tyle=self.prompt
+0000ee60: 732e 7072 6f6d 7074 5374 796c 6532 2c20  s.promptStyle2, 
+0000ee70: 6465 6661 756c 743d 2279 6573 2229 0a20  default="yes"). 
+0000ee80: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+0000ee90: 6e66 6972 6d61 7469 6f6e 2e6c 6f77 6572  nfirmation.lower
+0000eea0: 2829 2069 6e20 2822 7922 2c20 2279 6573  () in ("y", "yes
+0000eeb0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+0000eec0: 2020 2020 6d65 6d6f 7279 5f73 746f 7265      memory_store
+0000eed0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+0000eee0: 636f 6e66 6967 2e6c 6f63 616c 5374 6f72  config.localStor
+0000eef0: 6167 652c 2022 6d65 6d6f 7279 2229 0a20  age, "memory"). 
+0000ef00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000ef10: 6574 7269 6576 6564 5f63 6f6c 6c65 6374  etrieved_collect
+0000ef20: 696f 6e73 203d 206f 732e 7061 7468 2e6a  ions = os.path.j
+0000ef30: 6f69 6e28 636f 6e66 6967 2e6c 6f63 616c  oin(config.local
+0000ef40: 5374 6f72 6167 652c 2022 6175 746f 6765  Storage, "autoge
+0000ef50: 6e22 2c20 2272 6574 7269 6576 6572 2229  n", "retriever")
+0000ef60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ef70: 2066 6f72 2066 6f6c 6465 7220 696e 2028   for folder in (
+0000ef80: 6d65 6d6f 7279 5f73 746f 7265 2c20 7265  memory_store, re
+0000ef90: 7472 6965 7665 645f 636f 6c6c 6563 7469  trieved_collecti
+0000efa0: 6f6e 7329 3a0a 2020 2020 2020 2020 2020  ons):.          
+0000efb0: 2020 2020 2020 2020 2020 7368 7574 696c            shutil
+0000efc0: 2e72 6d74 7265 6528 666f 6c64 6572 2c20  .rmtree(folder, 
+0000efd0: 6967 6e6f 7265 5f65 7272 6f72 733d 5472  ignore_errors=Tr
+0000efe0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+0000eff0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000f000: 2020 2020 2020 7072 696e 7431 2866 2244        print1(f"D
+0000f010: 6f20 796f 7520 7761 6e74 2074 6f20 6368  o you want to ch
+0000f020: 616e 6765 2062 6163 6b20 7468 6520 656d  ange back the em
+0000f030: 6265 6464 696e 6720 6d6f 6465 6c20 6672  bedding model fr
+0000f040: 6f6d 2027 7b63 6f6e 6669 672e 656d 6265  om '{config.embe
+0000f050: 6464 696e 674d 6f64 656c 7d27 2074 6f20  ddingModel}' to 
+0000f060: 277b 6f6c 6445 6d62 6564 6469 6e67 4d6f  '{oldEmbeddingMo
+0000f070: 6465 6c7d 273f 205b 795d 6573 202f 205b  del}'? [y]es / [
+0000f080: 4e5d 6f22 290a 2020 2020 2020 2020 2020  N]o").          
+0000f090: 2020 2020 2020 636f 6e66 6972 6d61 7469        confirmati
+0000f0a0: 6f6e 203d 2073 656c 662e 7072 6f6d 7074  on = self.prompt
+0000f0b0: 732e 7369 6d70 6c65 5072 6f6d 7074 2873  s.simplePrompt(s
+0000f0c0: 7479 6c65 3d73 656c 662e 7072 6f6d 7074  tyle=self.prompt
+0000f0d0: 732e 7072 6f6d 7074 5374 796c 6532 2c20  s.promptStyle2, 
+0000f0e0: 6465 6661 756c 743d 2279 6573 2229 0a20  default="yes"). 
+0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f100: 6620 6e6f 7420 636f 6e66 6972 6d61 7469  f not confirmati
+0000f110: 6f6e 2e6c 6f77 6572 2829 2069 6e20 2822  on.lower() in ("
+0000f120: 7922 2c20 2279 6573 2229 3a0a 2020 2020  y", "yes"):.    
+0000f130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f140: 636f 6e66 6967 2e65 6d62 6564 6469 6e67  config.embedding
+0000f150: 4d6f 6465 6c20 3d20 6f6c 6445 6d62 6564  Model = oldEmbed
+0000f160: 6469 6e67 4d6f 6465 6c0a 2020 2020 2020  dingModel.      
+0000f170: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000f180: 696e 7433 2866 2245 6d62 6564 6469 6e67  int3(f"Embedding
+0000f190: 206d 6f64 656c 3a20 7b6f 6c64 456d 6265   model: {oldEmbe
+0000f1a0: 6464 696e 674d 6f64 656c 7d22 290a 2020  ddingModel}").  
+0000f1b0: 2020 2020 2020 6966 206e 6f74 206f 6c64        if not old
+0000f1c0: 456d 6265 6464 696e 674d 6f64 656c 203d  EmbeddingModel =
+0000f1d0: 3d20 636f 6e66 6967 2e65 6d62 6564 6469  = config.embeddi
+0000f1e0: 6e67 4d6f 6465 6c3a 0a20 2020 2020 2020  ngModel:.       
+0000f1f0: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
+0000f200: 436f 6e66 6967 2829 0a0a 2020 2020 6465  Config()..    de
+0000f210: 6620 7365 7441 7574 6f47 656e 4275 696c  f setAutoGenBuil
+0000f220: 6465 7243 6f6e 6669 6728 7365 6c66 293a  derConfig(self):
+0000f230: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000f240: 636f 6e66 6967 2e69 7354 6572 6d75 783a  config.isTermux:
+0000f250: 0a20 2020 2020 2020 2020 2020 2041 7574  .            Aut
+0000f260: 6f47 656e 4275 696c 6465 7228 292e 7072  oGenBuilder().pr
+0000f270: 6f6d 7074 436f 6e66 6967 2829 0a0a 2020  omptConfig()..  
+0000f280: 2020 6465 6620 7365 7441 7373 6973 7461    def setAssista
+0000f290: 6e74 4e61 6d65 2873 656c 6629 3a0a 2020  ntName(self):.  
+0000f2a0: 2020 2020 2020 7072 696e 7431 2822 596f        print1("Yo
+0000f2b0: 7520 6d61 7920 6d6f 6469 6679 206d 7920  u may modify my 
+0000f2c0: 6e61 6d65 2062 656c 6f77 3a22 290a 2020  name below:").  
+0000f2d0: 2020 2020 2020 6672 6565 4765 6e69 7573        freeGenius
+0000f2e0: 4149 4e61 6d65 203d 2073 656c 662e 7072  AIName = self.pr
+0000f2f0: 6f6d 7074 732e 7369 6d70 6c65 5072 6f6d  ompts.simpleProm
+0000f300: 7074 2873 7479 6c65 3d73 656c 662e 7072  pt(style=self.pr
+0000f310: 6f6d 7074 732e 7072 6f6d 7074 5374 796c  ompts.promptStyl
+0000f320: 6532 2c20 6465 6661 756c 743d 636f 6e66  e2, default=conf
+0000f330: 6967 2e66 7265 6547 656e 6975 7341 494e  ig.freeGeniusAIN
+0000f340: 616d 6529 0a20 2020 2020 2020 2069 6620  ame).        if 
+0000f350: 6672 6565 4765 6e69 7573 4149 4e61 6d65  freeGeniusAIName
+0000f360: 2061 6e64 206e 6f74 2066 7265 6547 656e   and not freeGen
+0000f370: 6975 7341 494e 616d 652e 7374 7269 7028  iusAIName.strip(
+0000f380: 292e 6c6f 7765 7228 2920 3d3d 2063 6f6e  ).lower() == con
+0000f390: 6669 672e 6578 6974 5f65 6e74 7279 3a0a  fig.exit_entry:.
+0000f3a0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+0000f3b0: 6967 2e66 7265 6547 656e 6975 7341 494e  ig.freeGeniusAIN
+0000f3c0: 616d 6520 3d20 6672 6565 4765 6e69 7573  ame = freeGenius
+0000f3d0: 4149 4e61 6d65 0a20 2020 2020 2020 2020  AIName.         
+0000f3e0: 2020 2063 6f6e 6669 672e 6c6f 6361 6c53     config.localS
+0000f3f0: 746f 7261 6765 203d 2067 6574 4c6f 6361  torage = getLoca
+0000f400: 6c53 746f 7261 6765 2829 0a20 2020 2020  lStorage().     
+0000f410: 2020 2020 2020 2063 6f6e 6669 672e 7361         config.sa
+0000f420: 7665 436f 6e66 6967 2829 0a20 2020 2020  veConfig().     
+0000f430: 2020 2020 2020 2070 7269 6e74 3328 6622         print3(f"
+0000f440: 596f 7520 6861 7665 2063 6861 6e67 6564  You have changed
+0000f450: 206d 7920 6e61 6d65 2074 6f3a 207b 636f   my name to: {co
+0000f460: 6e66 6967 2e66 7265 6547 656e 6975 7341  nfig.freeGeniusA
+0000f470: 494e 616d 657d 2229 0a0a 2020 2020 6465  IName}")..    de
+0000f480: 6620 7365 7443 7573 746f 6d53 7973 7465  f setCustomSyste
+0000f490: 6d4d 6573 7361 6765 2873 656c 6629 3a0a  mMessage(self):.
+0000f4a0: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+0000f4b0: 596f 7520 6361 6e20 6d6f 6469 6679 2074  You can modify t
+0000f4c0: 6865 2073 7973 7465 6d20 6d65 7373 6167  he system messag
+0000f4d0: 6520 746f 2066 7572 6e69 7368 206d 6520  e to furnish me 
+0000f4e0: 7769 7468 2064 6574 6169 6c73 2061 626f  with details abo
+0000f4f0: 7574 206d 7920 6361 7061 6269 6c69 7469  ut my capabiliti
+0000f500: 6573 2c20 636f 6e73 7472 6169 6e74 732c  es, constraints,
+0000f510: 206f 7220 616e 7920 7065 7274 696e 656e   or any pertinen
+0000f520: 7420 636f 6e74 6578 7420 7468 6174 206d  t context that m
+0000f530: 6179 2069 6e66 6f72 6d20 6f75 7220 696e  ay inform our in
+0000f540: 7465 7261 6374 696f 6e73 2e20 5468 6973  teractions. This
+0000f550: 2077 696c 6c20 6775 6964 6520 6d65 2069   will guide me i
+0000f560: 6e20 6d61 6e61 6769 6e67 2061 6e64 2072  n managing and r
+0000f570: 6573 706f 6e64 696e 6720 746f 2079 6f75  esponding to you
+0000f580: 7220 7265 7175 6573 7473 2061 7070 726f  r requests appro
+0000f590: 7072 6961 7465 6c79 2e22 290a 2020 2020  priately.").    
+0000f5a0: 2020 2020 7072 696e 7431 2822 506c 6561      print1("Plea
+0000f5b0: 7365 206e 6f74 6520 7468 6174 2061 6c74  se note that alt
+0000f5c0: 6572 696e 6720 6d79 2073 7973 7465 6d20  ering my system 
+0000f5d0: 6d65 7373 6167 6520 6469 7265 6374 6c79  message directly
+0000f5e0: 2061 6666 6563 7473 206d 7920 6675 6e63   affects my func
+0000f5f0: 7469 6f6e 616c 6974 792e 2048 616e 646c  tionality. Handl
+0000f600: 6520 7769 7468 2063 6172 652e 2229 0a20  e with care."). 
+0000f610: 2020 2020 2020 2070 7269 6e74 3128 2245         print1("E
+0000f620: 6e74 6572 2063 7573 746f 6d20 7379 7374  nter custom syst
+0000f630: 656d 206d 6573 7361 6765 2062 656c 6f77  em message below
+0000f640: 3a22 290a 2020 2020 2020 2020 7072 696e  :").        prin
+0000f650: 7431 2866 2228 4b65 6570 2069 7420 626c  t1(f"(Keep it bl
+0000f660: 616e 6b20 746f 2075 7365 207b 636f 6e66  ank to use {conf
+0000f670: 6967 2e66 7265 6547 656e 6975 7341 494e  ig.freeGeniusAIN
+0000f680: 616d 657d 2064 6566 6175 6c74 2073 7973  ame} default sys
+0000f690: 7465 6d20 6d65 7373 6167 652e 2922 290a  tem message.)").
+0000f6a0: 2020 2020 2020 2020 6d65 7373 6167 6520          message 
+0000f6b0: 3d20 7365 6c66 2e70 726f 6d70 7473 2e73  = self.prompts.s
+0000f6c0: 696d 706c 6550 726f 6d70 7428 7374 796c  implePrompt(styl
+0000f6d0: 653d 7365 6c66 2e70 726f 6d70 7473 2e70  e=self.prompts.p
+0000f6e0: 726f 6d70 7453 7479 6c65 322c 2064 6566  romptStyle2, def
+0000f6f0: 6175 6c74 3d63 6f6e 6669 672e 7379 7374  ault=config.syst
+0000f700: 656d 4d65 7373 6167 655f 6c65 746d 6564  emMessage_letmed
+0000f710: 6f69 7429 0a20 2020 2020 2020 2069 6620  oit).        if 
+0000f720: 6d65 7373 6167 6520 616e 6420 6e6f 7420  message and not 
+0000f730: 6d65 7373 6167 652e 7374 7269 7028 292e  message.strip().
+0000f740: 6c6f 7765 7228 2920 3d3d 2063 6f6e 6669  lower() == confi
+0000f750: 672e 6578 6974 5f65 6e74 7279 3a0a 2020  g.exit_entry:.  
+0000f760: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0000f770: 2e73 7973 7465 6d4d 6573 7361 6765 5f6c  .systemMessage_l
+0000f780: 6574 6d65 646f 6974 203d 206d 6573 7361  etmedoit = messa
+0000f790: 6765 0a20 2020 2020 2020 2020 2020 2063  ge.            c
+0000f7a0: 6f6e 6669 672e 7361 7665 436f 6e66 6967  onfig.saveConfig
+0000f7b0: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+0000f7c0: 7269 6e74 3328 6622 4375 7374 6f6d 2073  rint3(f"Custom s
+0000f7d0: 7973 7465 6d20 6d65 7373 6167 653a 207b  ystem message: {
+0000f7e0: 636f 6e66 6967 2e66 7265 6547 656e 6975  config.freeGeniu
+0000f7f0: 7341 494e 616d 657d 2229 0a0a 2020 2020  sAIName}")..    
+0000f800: 6465 6620 7365 7443 7573 746f 6d54 6578  def setCustomTex
+0000f810: 7445 6469 746f 7228 7365 6c66 293a 0a20  tEditor(self):. 
+0000f820: 2020 2020 2020 2070 7269 6e74 3128 2250         print1("P
+0000f830: 6c65 6173 6520 7370 6563 6966 7920 6375  lease specify cu
+0000f840: 7374 6f6d 2074 6578 7420 6564 6974 6f72  stom text editor
+0000f850: 2063 6f6d 6d61 6e64 2062 656c 6f77 3a22   command below:"
+0000f860: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
+0000f870: 2822 652e 672e 2027 6d69 6372 6f20 2d73  ("e.g. 'micro -s
+0000f880: 6f66 7477 7261 7020 7472 7565 202d 776f  oftwrap true -wo
+0000f890: 7264 7772 6170 2074 7275 6527 2229 0a20  rdwrap true'"). 
+0000f8a0: 2020 2020 2020 2070 7269 6e74 3128 224c         print1("L
+0000f8b0: 6561 7665 2069 7420 626c 616e 6b20 746f  eave it blank to
+0000f8c0: 2075 7365 206f 7572 2062 7569 6c74 2d69   use our built-i
+0000f8d0: 6e20 7465 7874 2065 6469 746f 7220 2765  n text editor 'e
+0000f8e0: 5465 7874 4564 6974 2720 6279 2064 6566  TextEdit' by def
+0000f8f0: 6175 6c74 2e22 290a 2020 2020 2020 2020  ault.").        
+0000f900: 6375 7374 6f6d 5465 7874 4564 6974 6f72  customTextEditor
+0000f910: 203d 2073 656c 662e 7072 6f6d 7074 732e   = self.prompts.
+0000f920: 7369 6d70 6c65 5072 6f6d 7074 2873 7479  simplePrompt(sty
+0000f930: 6c65 3d73 656c 662e 7072 6f6d 7074 732e  le=self.prompts.
+0000f940: 7072 6f6d 7074 5374 796c 6532 2c20 6465  promptStyle2, de
+0000f950: 6661 756c 743d 636f 6e66 6967 2e63 7573  fault=config.cus
+0000f960: 746f 6d54 6578 7445 6469 746f 7229 0a20  tomTextEditor). 
+0000f970: 2020 2020 2020 2069 6620 6375 7374 6f6d         if custom
+0000f980: 5465 7874 4564 6974 6f72 2061 6e64 206e  TextEditor and n
+0000f990: 6f74 2063 7573 746f 6d54 6578 7445 6469  ot customTextEdi
+0000f9a0: 746f 722e 7374 7269 7028 292e 6c6f 7765  tor.strip().lowe
+0000f9b0: 7228 2920 3d3d 2063 6f6e 6669 672e 6578  r() == config.ex
+0000f9c0: 6974 5f65 6e74 7279 3a0a 2020 2020 2020  it_entry:.      
+0000f9d0: 2020 2020 2020 7465 7874 4564 6974 6f72        textEditor
+0000f9e0: 203d 2072 652e 7375 6228 2220 2e2a 3f24   = re.sub(" .*?$
+0000f9f0: 222c 2022 222c 2063 7573 746f 6d54 6578  ", "", customTex
+0000fa00: 7445 6469 746f 7229 0a20 2020 2020 2020  tEditor).       
+0000fa10: 2020 2020 2069 6620 6e6f 7420 7465 7874       if not text
+0000fa20: 4564 6974 6f72 206f 7220 6e6f 7420 6973  Editor or not is
+0000fa30: 436f 6d6d 616e 6449 6e73 7461 6c6c 6564  CommandInstalled
+0000fa40: 2874 6578 7445 6469 746f 7229 3a0a 2020  (textEditor):.  
+0000fa50: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+0000fa60: 696e 7432 2822 436f 6d6d 616e 6420 6e6f  int2("Command no
+0000fa70: 7420 666f 756e 6420 6f6e 2079 6f75 7220  t found on your 
+0000fa80: 6465 7669 6365 2122 290a 2020 2020 2020  device!").      
+0000fa90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000faa0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+0000fab0: 6967 2e63 7573 746f 6d54 6578 7445 6469  ig.customTextEdi
+0000fac0: 746f 7220 3d20 6375 7374 6f6d 5465 7874  tor = customText
+0000fad0: 4564 6974 6f72 0a20 2020 2020 2020 2020  Editor.         
+0000fae0: 2020 2020 2020 2063 6f6e 6669 672e 7361         config.sa
+0000faf0: 7665 436f 6e66 6967 2829 0a20 2020 2020  veConfig().     
+0000fb00: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000fb10: 3328 6622 4375 7374 6f6d 2074 6578 7420  3(f"Custom text 
+0000fb20: 6564 6974 6f72 3a20 7b63 6f6e 6669 672e  editor: {config.
+0000fb30: 6375 7374 6f6d 5465 7874 4564 6974 6f72  customTextEditor
+0000fb40: 7d22 290a 0a20 2020 2064 6566 2073 6574  }")..    def set
+0000fb50: 4368 6174 5265 636f 7264 436c 6f73 6573  ChatRecordCloses
+0000fb60: 744d 6174 6368 6573 2873 656c 6629 3a0a  tMatches(self):.
+0000fb70: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+0000fb80: 506c 6561 7365 2073 7065 6369 6679 2074  Please specify t
+0000fb90: 6865 206e 756d 6265 7220 6f66 2063 6c6f  he number of clo
+0000fba0: 7365 7374 206d 6174 6368 6573 2069 6e20  sest matches in 
+0000fbb0: 6561 6368 206d 656d 6f72 7920 7265 7472  each memory retr
+0000fbc0: 6965 7661 6c3a 2229 0a20 2020 2020 2020  ieval:").       
+0000fbd0: 2063 6861 7452 6563 6f72 6443 6c6f 7365   chatRecordClose
+0000fbe0: 7374 4d61 7463 6865 7320 3d20 7365 6c66  stMatches = self
+0000fbf0: 2e70 726f 6d70 7473 2e73 696d 706c 6550  .prompts.simpleP
+0000fc00: 726f 6d70 7428 7374 796c 653d 7365 6c66  rompt(style=self
+0000fc10: 2e70 726f 6d70 7473 2e70 726f 6d70 7453  .prompts.promptS
+0000fc20: 7479 6c65 322c 206e 756d 6265 724f 6e6c  tyle2, numberOnl
+0000fc30: 793d 5472 7565 2c20 6465 6661 756c 743d  y=True, default=
+0000fc40: 7374 7228 636f 6e66 6967 2e63 6861 7452  str(config.chatR
+0000fc50: 6563 6f72 6443 6c6f 7365 7374 4d61 7463  ecordClosestMatc
+0000fc60: 6865 7329 290a 2020 2020 2020 2020 6966  hes)).        if
+0000fc70: 2063 6861 7452 6563 6f72 6443 6c6f 7365   chatRecordClose
+0000fc80: 7374 4d61 7463 6865 7320 616e 6420 6e6f  stMatches and no
+0000fc90: 7420 6368 6174 5265 636f 7264 436c 6f73  t chatRecordClos
+0000fca0: 6573 744d 6174 6368 6573 2e73 7472 6970  estMatches.strip
+0000fcb0: 2829 2e6c 6f77 6572 2829 203d 3d20 636f  ().lower() == co
+0000fcc0: 6e66 6967 2e65 7869 745f 656e 7472 7920  nfig.exit_entry 
+0000fcd0: 616e 6420 696e 7428 6368 6174 5265 636f  and int(chatReco
+0000fce0: 7264 436c 6f73 6573 744d 6174 6368 6573  rdClosestMatches
+0000fcf0: 2920 3e3d 2030 3a0a 2020 2020 2020 2020  ) >= 0:.        
+0000fd00: 2020 2020 636f 6e66 6967 2e63 6861 7452      config.chatR
+0000fd10: 6563 6f72 6443 6c6f 7365 7374 4d61 7463  ecordClosestMatc
+0000fd20: 6865 7320 3d20 696e 7428 6368 6174 5265  hes = int(chatRe
+0000fd30: 636f 7264 436c 6f73 6573 744d 6174 6368  cordClosestMatch
+0000fd40: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+0000fd50: 636f 6e66 6967 2e73 6176 6543 6f6e 6669  config.saveConfi
+0000fd60: 6728 290a 2020 2020 2020 2020 2020 2020  g().            
+0000fd70: 7072 696e 7433 2866 224e 756d 6265 7220  print3(f"Number 
+0000fd80: 6f66 206d 656d 6f72 7920 636c 6f73 6573  of memory closes
+0000fd90: 7420 6d61 7463 6865 733a 207b 636f 6e66  t matches: {conf
+0000fda0: 6967 2e63 6861 7452 6563 6f72 6443 6c6f  ig.chatRecordClo
+0000fdb0: 7365 7374 4d61 7463 6865 737d 2229 0a0a  sestMatches}")..
+0000fdc0: 2020 2020 6465 6620 7365 744d 656d 6f72      def setMemor
+0000fdd0: 7943 6c6f 7365 7374 4d61 7463 6865 7328  yClosestMatches(
+0000fde0: 7365 6c66 293a 0a20 2020 2020 2020 2070  self):.        p
+0000fdf0: 7269 6e74 3128 2250 6c65 6173 6520 7370  rint1("Please sp
+0000fe00: 6563 6966 7920 7468 6520 6e75 6d62 6572  ecify the number
+0000fe10: 206f 6620 636c 6f73 6573 7420 6d61 7463   of closest matc
+0000fe20: 6865 7320 696e 2065 6163 6820 6d65 6d6f  hes in each memo
+0000fe30: 7279 2072 6574 7269 6576 616c 3a22 290a  ry retrieval:").
+0000fe40: 2020 2020 2020 2020 6d65 6d6f 7279 436c          memoryCl
+0000fe50: 6f73 6573 744d 6174 6368 6573 203d 2073  osestMatches = s
+0000fe60: 656c 662e 7072 6f6d 7074 732e 7369 6d70  elf.prompts.simp
+0000fe70: 6c65 5072 6f6d 7074 2873 7479 6c65 3d73  lePrompt(style=s
+0000fe80: 656c 662e 7072 6f6d 7074 732e 7072 6f6d  elf.prompts.prom
+0000fe90: 7074 5374 796c 6532 2c20 6e75 6d62 6572  ptStyle2, number
+0000fea0: 4f6e 6c79 3d54 7275 652c 2064 6566 6175  Only=True, defau
+0000feb0: 6c74 3d73 7472 2863 6f6e 6669 672e 6d65  lt=str(config.me
+0000fec0: 6d6f 7279 436c 6f73 6573 744d 6174 6368  moryClosestMatch
+0000fed0: 6573 2929 0a20 2020 2020 2020 2069 6620  es)).        if 
+0000fee0: 6d65 6d6f 7279 436c 6f73 6573 744d 6174  memoryClosestMat
+0000fef0: 6368 6573 2061 6e64 206e 6f74 206d 656d  ches and not mem
+0000ff00: 6f72 7943 6c6f 7365 7374 4d61 7463 6865  oryClosestMatche
+0000ff10: 732e 7374 7269 7028 292e 6c6f 7765 7228  s.strip().lower(
+0000ff20: 2920 3d3d 2063 6f6e 6669 672e 6578 6974  ) == config.exit
+0000ff30: 5f65 6e74 7279 2061 6e64 2069 6e74 286d  _entry and int(m
+0000ff40: 656d 6f72 7943 6c6f 7365 7374 4d61 7463  emoryClosestMatc
+0000ff50: 6865 7329 203e 3d20 303a 0a20 2020 2020  hes) >= 0:.     
+0000ff60: 2020 2020 2020 2063 6f6e 6669 672e 6d65         config.me
+0000ff70: 6d6f 7279 436c 6f73 6573 744d 6174 6368  moryClosestMatch
+0000ff80: 6573 203d 2069 6e74 286d 656d 6f72 7943  es = int(memoryC
+0000ff90: 6c6f 7365 7374 4d61 7463 6865 7329 0a20  losestMatches). 
+0000ffa0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+0000ffb0: 672e 7361 7665 436f 6e66 6967 2829 0a20  g.saveConfig(). 
+0000ffc0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+0000ffd0: 3328 6622 4e75 6d62 6572 206f 6620 6d65  3(f"Number of me
+0000ffe0: 6d6f 7279 2063 6c6f 7365 7374 206d 6174  mory closest mat
+0000fff0: 6368 6573 3a20 7b63 6f6e 6669 672e 6d65  ches: {config.me
+00010000: 6d6f 7279 436c 6f73 6573 744d 6174 6368  moryClosestMatch
+00010010: 6573 7d22 290a 0a20 2020 2064 6566 2073  es}")..    def s
+00010020: 6574 4d61 7841 7574 6f43 6f72 7265 6374  etMaxAutoCorrect
+00010030: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+00010040: 7072 696e 7431 2866 2254 6865 2061 7574  print1(f"The aut
+00010050: 6f2d 636f 7272 6563 7469 6f6e 2066 6561  o-correction fea
+00010060: 7475 7265 2065 6e61 626c 6573 207b 636f  ture enables {co
+00010070: 6e66 6967 2e66 7265 6547 656e 6975 7341  nfig.freeGeniusA
+00010080: 494e 616d 657d 2074 6f20 6175 746f 6d61  IName} to automa
+00010090: 7469 6361 6c6c 7920 6669 7820 6272 6f6b  tically fix brok
+000100a0: 656e 2050 7974 686f 6e20 636f 6465 2069  en Python code i
+000100b0: 6620 6974 2077 6173 206e 6f74 2065 7865  f it was not exe
+000100c0: 6375 7465 6420 7072 6f70 6572 6c79 2e22  cuted properly."
+000100d0: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
+000100e0: 2822 506c 6561 7365 2073 7065 6369 6679  ("Please specify
+000100f0: 206d 6178 696d 756d 206e 756d 6265 7220   maximum number 
+00010100: 6f66 2061 7574 6f2d 636f 7272 6563 7469  of auto-correcti
+00010110: 6f6e 2061 7474 656d 7074 7320 6265 6c6f  on attempts belo
+00010120: 773a 2229 0a20 2020 2020 2020 2070 7269  w:").        pri
+00010130: 6e74 3128 2228 5265 6d61 726b 733a 2045  nt1("(Remarks: E
+00010140: 6e74 6572 2027 3027 2069 6620 796f 7520  nter '0' if you 
+00010150: 7761 6e74 2074 6f20 6469 7361 626c 6520  want to disable 
+00010160: 6175 746f 2d63 6f72 7265 6374 696f 6e20  auto-correction 
+00010170: 6665 6174 7572 6529 2229 0a20 2020 2020  feature)").     
+00010180: 2020 206d 6178 4175 746f 436f 7272 6563     maxAutoCorrec
+00010190: 7420 3d20 7365 6c66 2e70 726f 6d70 7473  t = self.prompts
+000101a0: 2e73 696d 706c 6550 726f 6d70 7428 7374  .simplePrompt(st
+000101b0: 796c 653d 7365 6c66 2e70 726f 6d70 7473  yle=self.prompts
+000101c0: 2e70 726f 6d70 7453 7479 6c65 322c 206e  .promptStyle2, n
+000101d0: 756d 6265 724f 6e6c 793d 5472 7565 2c20  umberOnly=True, 
+000101e0: 6465 6661 756c 743d 7374 7228 636f 6e66  default=str(conf
+000101f0: 6967 2e6d 6178 5f63 6f6e 7365 6375 7469  ig.max_consecuti
+00010200: 7665 5f61 7574 6f5f 636f 7272 6563 7469  ve_auto_correcti
+00010210: 6f6e 2929 0a20 2020 2020 2020 2069 6620  on)).        if 
+00010220: 6d61 7841 7574 6f43 6f72 7265 6374 2061  maxAutoCorrect a
+00010230: 6e64 206e 6f74 206d 6178 4175 746f 436f  nd not maxAutoCo
+00010240: 7272 6563 742e 7374 7269 7028 292e 6c6f  rrect.strip().lo
+00010250: 7765 7228 2920 3d3d 2063 6f6e 6669 672e  wer() == config.
+00010260: 6578 6974 5f65 6e74 7279 2061 6e64 2069  exit_entry and i
+00010270: 6e74 286d 6178 4175 746f 436f 7272 6563  nt(maxAutoCorrec
+00010280: 7429 203e 3d20 303a 0a20 2020 2020 2020  t) >= 0:.       
+00010290: 2020 2020 2063 6f6e 6669 672e 6d61 785f       config.max_
+000102a0: 636f 6e73 6563 7574 6976 655f 6175 746f  consecutive_auto
+000102b0: 5f63 6f72 7265 6374 696f 6e20 3d20 696e  _correction = in
+000102c0: 7428 6d61 7841 7574 6f43 6f72 7265 6374  t(maxAutoCorrect
+000102d0: 290a 2020 2020 2020 2020 2020 2020 636f  ).            co
+000102e0: 6e66 6967 2e73 6176 6543 6f6e 6669 6728  nfig.saveConfig(
+000102f0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+00010300: 696e 7433 2866 224d 6178 696d 756d 2063  int3(f"Maximum c
+00010310: 6f6e 7365 6375 7469 7665 2061 7574 6f2d  onsecutive auto-
+00010320: 636f 7272 6563 7469 6f6e 3a20 7b63 6f6e  correction: {con
+00010330: 6669 672e 6d61 785f 636f 6e73 6563 7574  fig.max_consecut
+00010340: 6976 655f 6175 746f 5f63 6f72 7265 6374  ive_auto_correct
+00010350: 696f 6e7d 2229 0a0a 2020 2020 6465 6620  ion}")..    def 
+00010360: 7365 744d 696e 546f 6b65 6e73 2873 656c  setMinTokens(sel
+00010370: 6629 3a0a 2020 2020 2020 2020 7072 696e  f):.        prin
+00010380: 7431 2822 506c 6561 7365 2073 7065 6369  t1("Please speci
+00010390: 6679 206d 696e 696d 756d 206f 7574 7075  fy minimum outpu
+000103a0: 7420 746f 6b65 6e73 2062 656c 6f77 3a22  t tokens below:"
+000103b0: 290a 2020 2020 2020 2020 7072 696e 7431  ).        print1
+000103c0: 2822 2861 7070 6c69 6361 626c 6520 746f  ("(applicable to
+000103d0: 2027 6368 6174 6770 7427 2061 6e64 2027   'chatgpt' and '
+000103e0: 6c65 746d 6564 6f69 7427 2069 6e74 6572  letmedoit' inter
+000103f0: 6661 6365 7320 6f6e 6c79 2922 290a 2020  faces only)").  
+00010400: 2020 2020 2020 6d69 6e74 6f6b 656e 7320        mintokens 
+00010410: 3d20 7365 6c66 2e70 726f 6d70 7473 2e73  = self.prompts.s
+00010420: 696d 706c 6550 726f 6d70 7428 7374 796c  implePrompt(styl
+00010430: 653d 7365 6c66 2e70 726f 6d70 7473 2e70  e=self.prompts.p
+00010440: 726f 6d70 7453 7479 6c65 322c 206e 756d  romptStyle2, num
+00010450: 6265 724f 6e6c 793d 5472 7565 2c20 6465  berOnly=True, de
+00010460: 6661 756c 743d 7374 7228 636f 6e66 6967  fault=str(config
+00010470: 2e63 6861 7447 5054 4170 694d 696e 546f  .chatGPTApiMinTo
+00010480: 6b65 6e73 2929 0a20 2020 2020 2020 2069  kens)).        i
+00010490: 6620 6d69 6e74 6f6b 656e 7320 616e 6420  f mintokens and 
+000104a0: 6e6f 7420 6d69 6e74 6f6b 656e 732e 7374  not mintokens.st
+000104b0: 7269 7028 292e 6c6f 7765 7228 2920 3d3d  rip().lower() ==
+000104c0: 2063 6f6e 6669 672e 6578 6974 5f65 6e74   config.exit_ent
+000104d0: 7279 2061 6e64 2069 6e74 286d 696e 746f  ry and int(minto
+000104e0: 6b65 6e73 2920 3e20 303a 0a20 2020 2020  kens) > 0:.     
+000104f0: 2020 2020 2020 2063 6f6e 6669 672e 6368         config.ch
+00010500: 6174 4750 5441 7069 4d69 6e54 6f6b 656e  atGPTApiMinToken
+00010510: 7320 3d20 696e 7428 6d69 6e74 6f6b 656e  s = int(mintoken
+00010520: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
+00010530: 6620 636f 6e66 6967 2e63 6861 7447 5054  f config.chatGPT
+00010540: 4170 694d 696e 546f 6b65 6e73 203e 2063  ApiMinTokens > c
+00010550: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
+00010560: 4d61 7854 6f6b 656e 733a 0a20 2020 2020  MaxTokens:.     
+00010570: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00010580: 672e 6368 6174 4750 5441 7069 4d69 6e54  g.chatGPTApiMinT
+00010590: 6f6b 656e 7320 3d20 636f 6e66 6967 2e63  okens = config.c
+000105a0: 6861 7447 5054 4170 694d 6178 546f 6b65  hatGPTApiMaxToke
+000105b0: 6e73 0a20 2020 2020 2020 2020 2020 2063  ns.            c
+000105c0: 6f6e 6669 672e 7361 7665 436f 6e66 6967  onfig.saveConfig
+000105d0: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+000105e0: 7269 6e74 3328 6622 4d69 6e69 6d75 6d20  rint3(f"Minimum 
+000105f0: 6f75 7470 7574 2074 6f6b 656e 733a 207b  output tokens: {
+00010600: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
+00010610: 694d 696e 546f 6b65 6e73 7d22 290a 0a20  iMinTokens}").. 
+00010620: 2020 2064 6566 2067 6574 4d61 7854 6f6b     def getMaxTok
+00010630: 656e 7328 7365 6c66 293a 0a20 2020 2020  ens(self):.     
+00010640: 2020 2063 6f6e 7465 7874 5769 6e64 6f77     contextWindow
+00010650: 4c69 6d69 7420 3d20 746f 6b65 6e4c 696d  Limit = tokenLim
+00010660: 6974 735b 636f 6e66 6967 2e63 6861 7447  its[config.chatG
+00010670: 5054 4170 694d 6f64 656c 5d0a 2020 2020  PTApiModel].    
+00010680: 2020 2020 6675 6e63 7469 6f6e 546f 6b65      functionToke
+00010690: 6e73 203d 2063 6f75 6e74 5f74 6f6b 656e  ns = count_token
+000106a0: 735f 6672 6f6d 5f66 756e 6374 696f 6e73  s_from_functions
+000106b0: 2863 6f6e 6669 672e 746f 6f6c 4675 6e63  (config.toolFunc
+000106c0: 7469 6f6e 5363 6865 6d61 732e 7661 6c75  tionSchemas.valu
+000106d0: 6573 2829 290a 2020 2020 2020 2020 6d61  es()).        ma
+000106e0: 7854 6f6b 656e 203d 2063 6f6e 7465 7874  xToken = context
+000106f0: 5769 6e64 6f77 4c69 6d69 7420 2d20 6675  WindowLimit - fu
+00010700: 6e63 7469 6f6e 546f 6b65 6e73 202d 2063  nctionTokens - c
+00010710: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
+00010720: 4d69 6e54 6f6b 656e 730a 2020 2020 2020  MinTokens.      
+00010730: 2020 6966 206d 6178 546f 6b65 6e20 3e20    if maxToken > 
+00010740: 3430 3936 2061 6e64 2063 6f6e 6669 672e  4096 and config.
+00010750: 6368 6174 4750 5441 7069 4d6f 6465 6c20  chatGPTApiModel 
+00010760: 696e 2028 0a20 2020 2020 2020 2020 2020  in (.           
+00010770: 2022 6770 742d 342d 7475 7262 6f22 2c0a   "gpt-4-turbo",.
+00010780: 2020 2020 2020 2020 2020 2020 2267 7074              "gpt
+00010790: 2d34 2d74 7572 626f 2d70 7265 7669 6577  -4-turbo-preview
+000107a0: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
+000107b0: 6770 742d 342d 3031 3235 2d70 7265 7669  gpt-4-0125-previ
+000107c0: 6577 222c 0a20 2020 2020 2020 2020 2020  ew",.           
+000107d0: 2022 6770 742d 342d 3131 3036 2d70 7265   "gpt-4-1106-pre
+000107e0: 7669 6577 222c 0a20 2020 2020 2020 2020  view",.         
+000107f0: 2020 2022 6770 742d 332e 352d 7475 7262     "gpt-3.5-turb
+00010800: 6f22 2c0a 2020 2020 2020 2020 293a 0a20  o",.        ):. 
+00010810: 2020 2020 2020 2020 2020 206d 6178 546f             maxTo
+00010820: 6b65 6e20 3d20 3430 3936 0a20 2020 2020  ken = 4096.     
+00010830: 2020 2072 6574 7572 6e20 636f 6e74 6578     return contex
+00010840: 7457 696e 646f 774c 696d 6974 2c20 6675  tWindowLimit, fu
+00010850: 6e63 7469 6f6e 546f 6b65 6e73 2c20 6d61  nctionTokens, ma
+00010860: 7854 6f6b 656e 0a0a 2020 2020 6465 6620  xToken..    def 
+00010870: 7365 744d 6178 546f 6b65 6e73 5f6e 6f6e  setMaxTokens_non
+00010880: 5f63 6861 7467 7074 2873 656c 6629 3a0a  _chatgpt(self):.
+00010890: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+000108a0: 506c 6561 7365 2073 7065 6369 6679 206d  Please specify m
+000108b0: 6178 696d 756d 206f 7574 7075 7420 746f  aximum output to
+000108c0: 6b65 6e73 2062 656c 6f77 3a22 290a 2020  kens below:").  
+000108d0: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
+000108e0: 6c6c 6d49 6e74 6572 6661 6365 203d 3d20  llmInterface == 
+000108f0: 2267 656d 696e 6922 3a0a 2020 2020 2020  "gemini":.      
+00010900: 2020 2020 2020 6465 6661 756c 7420 3d20        default = 
+00010910: 636f 6e66 6967 2e67 656d 696e 6970 726f  config.geminipro
+00010920: 5f6d 6178 5f6f 7574 7075 745f 746f 6b65  _max_output_toke
+00010930: 6e73 0a20 2020 2020 2020 2065 6c69 6620  ns.        elif 
+00010940: 636f 6e66 6967 2e6c 6c6d 496e 7465 7266  config.llmInterf
+00010950: 6163 6520 3d3d 2022 6c6c 616d 6163 7070  ace == "llamacpp
+00010960: 223a 0a20 2020 2020 2020 2020 2020 2064  ":.            d
+00010970: 6566 6175 6c74 203d 2063 6f6e 6669 672e  efault = config.
+00010980: 6c6c 616d 6163 7070 4d61 696e 4d6f 6465  llamacppMainMode
+00010990: 6c5f 6d61 785f 746f 6b65 6e73 0a20 2020  l_max_tokens.   
+000109a0: 2020 2020 2065 6c69 6620 636f 6e66 6967       elif config
+000109b0: 2e6c 6c6d 496e 7465 7266 6163 6520 3d3d  .llmInterface ==
+000109c0: 2022 6f6c 6c61 6d61 223a 0a20 2020 2020   "ollama":.     
+000109d0: 2020 2020 2020 2064 6566 6175 6c74 203d         default =
+000109e0: 2063 6f6e 6669 672e 6f6c 6c61 6d61 4d61   config.ollamaMa
+000109f0: 696e 4d6f 6465 6c5f 6e75 6d5f 7072 6564  inModel_num_pred
+00010a00: 6963 740a 2020 2020 2020 2020 6d61 7874  ict.        maxt
+00010a10: 6f6b 656e 7320 3d20 7365 6c66 2e70 726f  okens = self.pro
+00010a20: 6d70 7473 2e73 696d 706c 6550 726f 6d70  mpts.simplePromp
+00010a30: 7428 7374 796c 653d 7365 6c66 2e70 726f  t(style=self.pro
+00010a40: 6d70 7473 2e70 726f 6d70 7453 7479 6c65  mpts.promptStyle
+00010a50: 322c 206e 756d 6265 724f 6e6c 793d 5472  2, numberOnly=Tr
+00010a60: 7565 2c20 6465 6661 756c 743d 7374 7228  ue, default=str(
+00010a70: 6465 6661 756c 7429 290a 2020 2020 2020  default)).      
+00010a80: 2020 6966 206d 6178 746f 6b65 6e73 2061    if maxtokens a
+00010a90: 6e64 206e 6f74 206d 6178 746f 6b65 6e73  nd not maxtokens
+00010aa0: 2e73 7472 6970 2829 2e6c 6f77 6572 2829  .strip().lower()
+00010ab0: 203d 3d20 636f 6e66 6967 2e65 7869 745f   == config.exit_
+00010ac0: 656e 7472 7920 616e 6420 696e 7428 6d61  entry and int(ma
+00010ad0: 7874 6f6b 656e 7329 203e 2030 3a0a 2020  xtokens) > 0:.  
+00010ae0: 2020 2020 2020 2020 2020 6d61 7874 6f6b            maxtok
+00010af0: 656e 7320 3d20 696e 7428 6d61 7874 6f6b  ens = int(maxtok
+00010b00: 656e 7329 0a20 2020 2020 2020 2020 2020  ens).           
+00010b10: 2069 6620 636f 6e66 6967 2e6c 6c6d 496e   if config.llmIn
+00010b20: 7465 7266 6163 6520 3d3d 2022 6765 6d69  terface == "gemi
+00010b30: 6e69 223a 0a20 2020 2020 2020 2020 2020  ni":.           
+00010b40: 2020 2020 2063 6f6e 6669 672e 6765 6d69       config.gemi
+00010b50: 6e69 7072 6f5f 6d61 785f 6f75 7470 7574  nipro_max_output
+00010b60: 5f74 6f6b 656e 7320 3d20 6d61 7874 6f6b  _tokens = maxtok
+00010b70: 656e 730a 2020 2020 2020 2020 2020 2020  ens.            
+00010b80: 656c 6966 2063 6f6e 6669 672e 6c6c 6d49  elif config.llmI
+00010b90: 6e74 6572 6661 6365 203d 3d20 226c 6c61  nterface == "lla
+00010ba0: 6d61 6370 7022 3a0a 2020 2020 2020 2020  macpp":.        
+00010bb0: 2020 2020 2020 2020 636f 6e66 6967 2e6c          config.l
+00010bc0: 6c61 6d61 6370 704d 6169 6e4d 6f64 656c  lamacppMainModel
+00010bd0: 5f6d 6178 5f74 6f6b 656e 7320 3d20 6d61  _max_tokens = ma
+00010be0: 7874 6f6b 656e 730a 2020 2020 2020 2020  xtokens.        
+00010bf0: 2020 2020 656c 6966 2063 6f6e 6669 672e      elif config.
+00010c00: 6c6c 6d49 6e74 6572 6661 6365 203d 3d20  llmInterface == 
+00010c10: 226f 6c6c 616d 6122 3a0a 2020 2020 2020  "ollama":.      
+00010c20: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00010c30: 2e6f 6c6c 616d 614d 6169 6e4d 6f64 656c  .ollamaMainModel
+00010c40: 5f6e 756d 5f70 7265 6469 6374 203d 206d  _num_predict = m
+00010c50: 6178 746f 6b65 6e73 0a20 2020 2020 2020  axtokens.       
+00010c60: 2020 2020 2063 6f6e 6669 672e 7361 7665       config.save
+00010c70: 436f 6e66 6967 2829 0a20 2020 2020 2020  Config().       
+00010c80: 2020 2020 2070 7269 6e74 3328 6622 4d61       print3(f"Ma
+00010c90: 7869 6d75 6d20 6f75 7470 7574 2074 6f6b  ximum output tok
+00010ca0: 656e 733a 207b 636f 6e66 6967 2e63 6861  ens: {config.cha
+00010cb0: 7447 5054 4170 694d 696e 546f 6b65 6e73  tGPTApiMinTokens
+00010cc0: 7d22 290a 0a20 2020 2064 6566 2073 6574  }")..    def set
+00010cd0: 4d61 7854 6f6b 656e 7328 7365 6c66 293a  MaxTokens(self):
+00010ce0: 0a20 2020 2020 2020 2023 206e 6f6e 2d63  .        # non-c
+00010cf0: 6861 7467 7074 2073 6574 7469 6e67 730a  hatgpt settings.
+00010d00: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
+00010d10: 6f6e 6669 672e 6c6c 6d49 6e74 6572 6661  onfig.llmInterfa
+00010d20: 6365 2069 6e20 2822 6368 6174 6770 7422  ce in ("chatgpt"
+00010d30: 2c20 226c 6574 6d65 646f 6974 2229 3a0a  , "letmedoit"):.
+00010d40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00010d50: 2e73 6574 4d61 7854 6f6b 656e 735f 6e6f  .setMaxTokens_no
+00010d60: 6e5f 6368 6174 6770 7428 290a 2020 2020  n_chatgpt().    
+00010d70: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00010d80: 6f6e 650a 2020 2020 2020 2020 2320 6368  one.        # ch
+00010d90: 6174 6770 7420 7365 7474 696e 6773 0a20  atgpt settings. 
+00010da0: 2020 2020 2020 2063 6f6e 7465 7874 5769         contextWi
+00010db0: 6e64 6f77 4c69 6d69 742c 2066 756e 6374  ndowLimit, funct
+00010dc0: 696f 6e54 6f6b 656e 732c 2074 6f6b 656e  ionTokens, token
+00010dd0: 4c69 6d69 7420 3d20 7365 6c66 2e67 6574  Limit = self.get
+00010de0: 4d61 7854 6f6b 656e 7328 290a 2020 2020  MaxTokens().    
+00010df0: 2020 2020 6966 2074 6f6b 656e 4c69 6d69      if tokenLimi
+00010e00: 7420 3c20 636f 6e66 6967 2e63 6861 7447  t < config.chatG
+00010e10: 5054 4170 694d 696e 546f 6b65 6e73 3a0a  PTApiMinTokens:.
+00010e20: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00010e30: 7432 2866 2246 756e 6374 696f 6e20 746f  t2(f"Function to
+00010e40: 6b65 6e73 205b 7b66 756e 6374 696f 6e54  kens [{functionT
+00010e50: 6f6b 656e 737d 5d20 6578 6365 6564 207b  okens}] exceed {
+00010e60: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
+00010e70: 694d 6f64 656c 7d20 6f75 7470 7574 2074  iModel} output t
+00010e80: 6f6b 656e 206c 696d 6974 2e22 290a 2020  oken limit.").  
+00010e90: 2020 2020 2020 2020 2020 7072 696e 7431            print1
+00010ea0: 2822 4569 7468 6572 2063 6861 6e67 6520  ("Either change 
+00010eb0: 746f 2061 206d 6f64 656c 2077 6974 6820  to a model with 
+00010ec0: 6869 6768 6572 2074 6f6b 656e 206c 696d  higher token lim
+00010ed0: 6974 206f 7220 6469 7361 626c 6520 756e  it or disable un
+00010ee0: 7573 6564 2066 756e 6374 696f 6e2d 6361  used function-ca
+00010ef0: 6c6c 2070 6c67 7569 6e73 2e22 290a 2020  ll plguins.").  
+00010f00: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00010f10: 2020 2020 2020 2020 7072 696e 7431 2873          print1(s
+00010f20: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
+00010f30: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
+00010f40: 2247 5054 2061 6e64 2065 6d62 6564 6469  "GPT and embeddi
+00010f50: 6e67 7320 6d6f 6465 6c73 2070 726f 6365  ngs models proce
+00010f60: 7373 2074 6578 7420 696e 2063 6875 6e6b  ss text in chunk
+00010f70: 7320 6361 6c6c 6564 2074 6f6b 656e 732e  s called tokens.
+00010f80: 2041 7320 6120 726f 7567 6820 7275 6c65   As a rough rule
+00010f90: 206f 6620 7468 756d 622c 2031 2074 6f6b   of thumb, 1 tok
+00010fa0: 656e 2069 7320 6170 7072 6f78 696d 6174  en is approximat
+00010fb0: 656c 7920 3420 6368 6172 6163 7465 7273  ely 4 characters
+00010fc0: 206f 7220 302e 3735 2077 6f72 6473 2066   or 0.75 words f
+00010fd0: 6f72 2045 6e67 6c69 7368 2074 6578 742e  or English text.
+00010fe0: 204f 6e65 206c 696d 6974 6174 696f 6e20   One limitation 
+00010ff0: 746f 206b 6565 7020 696e 206d 696e 6420  to keep in mind 
+00011000: 6973 2074 6861 7420 666f 7220 6120 4750  is that for a GP
+00011010: 5420 6d6f 6465 6c20 7468 6520 7072 6f6d  T model the prom
+00011020: 7074 2061 6e64 2074 6865 2067 656e 6572  pt and the gener
+00011030: 6174 6564 206f 7574 7075 7420 636f 6d62  ated output comb
+00011040: 696e 6564 206d 7573 7420 6265 206e 6f20  ined must be no 
+00011050: 6d6f 7265 2074 6861 6e20 7468 6520 6d6f  more than the mo
+00011060: 6465 6c27 7320 6d61 7869 6d75 6d20 636f  del's maximum co
+00011070: 6e74 6578 7420 6c65 6e67 7468 2e22 290a  ntext length.").
+00011080: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00011090: 7433 2866 2243 7572 7265 6e74 2047 5054  t3(f"Current GPT
+000110a0: 206d 6f64 656c 3a20 7b63 6f6e 6669 672e   model: {config.
+000110b0: 6368 6174 4750 5441 7069 4d6f 6465 6c7d  chatGPTApiModel}
+000110c0: 2229 0a20 2020 2020 2020 2020 2020 2070  ").            p
+000110d0: 7269 6e74 3328 6622 4d61 7869 6d75 6d20  rint3(f"Maximum 
+000110e0: 636f 6e74 6578 7420 6c65 6e67 7468 3a20  context length: 
+000110f0: 7b63 6f6e 7465 7874 5769 6e64 6f77 4c69  {contextWindowLi
+00011100: 6d69 747d 2229 0a20 2020 2020 2020 2020  mit}").         
+00011110: 2020 2070 7269 6e74 3328 6622 4375 7272     print3(f"Curr
+00011120: 656e 7420 6675 6e63 7469 6f6e 2074 6f6b  ent function tok
+00011130: 656e 733a 207b 6675 6e63 7469 6f6e 546f  ens: {functionTo
+00011140: 6b65 6e73 7d22 290a 2020 2020 2020 2020  kens}").        
+00011150: 2020 2020 7072 696e 7433 2866 224d 6178      print3(f"Max
+00011160: 696d 756d 206f 7574 7075 7420 746f 6b65  imum output toke
+00011170: 6e20 616c 6c6f 7765 6420 2865 7863 6c2e  n allowed (excl.
+00011180: 2066 756e 6374 696f 6e73 293a 207b 746f   functions): {to
+00011190: 6b65 6e4c 696d 6974 7d22 290a 2020 2020  kenLimit}").    
+000111a0: 2020 2020 2020 2020 7072 696e 7431 2873          print1(s
+000111b0: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
+000111c0: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
+000111d0: 2250 6c65 6173 6520 7370 6563 6966 7920  "Please specify 
+000111e0: 6d61 7869 6d75 6d20 6f75 7470 7574 2074  maximum output t
+000111f0: 6f6b 656e 7320 6265 6c6f 773a 2229 0a20  okens below:"). 
+00011200: 2020 2020 2020 2020 2020 206d 6178 746f             maxto
+00011210: 6b65 6e73 203d 2073 656c 662e 7072 6f6d  kens = self.prom
+00011220: 7074 732e 7369 6d70 6c65 5072 6f6d 7074  pts.simplePrompt
+00011230: 2873 7479 6c65 3d73 656c 662e 7072 6f6d  (style=self.prom
+00011240: 7074 732e 7072 6f6d 7074 5374 796c 6532  pts.promptStyle2
+00011250: 2c20 6e75 6d62 6572 4f6e 6c79 3d54 7275  , numberOnly=Tru
+00011260: 652c 2064 6566 6175 6c74 3d73 7472 2863  e, default=str(c
+00011270: 6f6e 6669 672e 6368 6174 4750 5441 7069  onfig.chatGPTApi
+00011280: 4d61 7854 6f6b 656e 7329 290a 2020 2020  MaxTokens)).    
+00011290: 2020 2020 2020 2020 6966 206d 6178 746f          if maxto
+000112a0: 6b65 6e73 2061 6e64 206e 6f74 206d 6178  kens and not max
+000112b0: 746f 6b65 6e73 2e73 7472 6970 2829 2e6c  tokens.strip().l
+000112c0: 6f77 6572 2829 203d 3d20 636f 6e66 6967  ower() == config
+000112d0: 2e65 7869 745f 656e 7472 7920 616e 6420  .exit_entry and 
+000112e0: 696e 7428 6d61 7874 6f6b 656e 7329 203e  int(maxtokens) >
+000112f0: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00011300: 2020 2020 636f 6e66 6967 2e63 6861 7447      config.chatG
+00011310: 5054 4170 694d 6178 546f 6b65 6e73 203d  PTApiMaxTokens =
+00011320: 2069 6e74 286d 6178 746f 6b65 6e73 290a   int(maxtokens).
+00011330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011340: 6966 2063 6f6e 6669 672e 6368 6174 4750  if config.chatGP
+00011350: 5441 7069 4d61 7854 6f6b 656e 7320 3e20  TApiMaxTokens > 
+00011360: 746f 6b65 6e4c 696d 6974 3a0a 2020 2020  tokenLimit:.    
+00011370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011380: 636f 6e66 6967 2e63 6861 7447 5054 4170  config.chatGPTAp
+00011390: 694d 6178 546f 6b65 6e73 203d 2074 6f6b  iMaxTokens = tok
+000113a0: 656e 4c69 6d69 740a 2020 2020 2020 2020  enLimit.        
+000113b0: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
+000113c0: 6176 6543 6f6e 6669 6728 290a 2020 2020  aveConfig().    
+000113d0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+000113e0: 7433 2866 224d 6178 696d 756d 206f 7574  t3(f"Maximum out
+000113f0: 7075 7420 746f 6b65 6e73 3a20 7b63 6f6e  put tokens: {con
+00011400: 6669 672e 6368 6174 4750 5441 7069 4d61  fig.chatGPTApiMa
+00011410: 7854 6f6b 656e 737d 2229 0a0a 2020 2020  xTokens}")..    
+00011420: 6465 6620 7275 6e53 7973 7465 6d43 6f6d  def runSystemCom
+00011430: 6d61 6e64 2873 656c 662c 2063 6f6d 6d61  mand(self, comma
+00011440: 6e64 293a 0a20 2020 2020 2020 2063 6f6d  nd):.        com
+00011450: 6d61 6e64 203d 2063 6f6d 6d61 6e64 2e73  mand = command.s
+00011460: 7472 6970 2829 5b31 3a5d 0a20 2020 2020  trip()[1:].     
+00011470: 2020 2069 6620 225c 6e22 2069 6e20 636f     if "\n" in co
+00011480: 6d6d 616e 643a 0a20 2020 2020 2020 2020  mmand:.         
+00011490: 2020 2063 6f6d 6d61 6e64 203d 2022 3b22     command = ";"
+000114a0: 2e6a 6f69 6e28 636f 6d6d 616e 642e 7370  .join(command.sp
+000114b0: 6c69 7428 225c 6e22 2929 0a20 2020 2020  lit("\n")).     
+000114c0: 2020 2069 6620 636f 6e66 6967 2e74 6869     if config.thi
+000114d0: 7350 6c61 7466 6f72 6d20 3d3d 2022 5769  sPlatform == "Wi
+000114e0: 6e64 6f77 7322 3a0a 2020 2020 2020 2020  ndows":.        
+000114f0: 2020 2020 6f73 2e73 7973 7465 6d28 636f      os.system(co
+00011500: 6d6d 616e 6429 0a20 2020 2020 2020 2065  mmand).        e
+00011510: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00011520: 206f 732e 7379 7374 656d 2866 2265 6e76   os.system(f"env
+00011530: 2051 545f 5150 415f 504c 4154 464f 524d   QT_QPA_PLATFORM
+00011540: 5f50 4c55 4749 4e5f 5041 5448 3d27 7b63  _PLUGIN_PATH='{c
+00011550: 6f6e 6669 672e 656e 765f 5154 5f51 5041  onfig.env_QT_QPA
+00011560: 5f50 4c41 5446 4f52 4d5f 504c 5547 494e  _PLATFORM_PLUGIN
+00011570: 5f50 4154 487d 2720 7b63 6f6d 6d61 6e64  _PATH}' {command
+00011580: 7d22 290a 0a20 2020 2064 6566 2074 6f67  }")..    def tog
+00011590: 676c 654d 756c 7469 6c69 6e65 2873 656c  gleMultiline(sel
+000115a0: 6629 3a0a 2020 2020 2020 2020 636f 6e66  f):.        conf
+000115b0: 6967 2e6d 756c 7469 6c69 6e65 496e 7075  ig.multilineInpu
+000115c0: 7420 3d20 6e6f 7420 636f 6e66 6967 2e6d  t = not config.m
+000115d0: 756c 7469 6c69 6e65 496e 7075 740a 2020  ultilineInput.  
+000115e0: 2020 2020 2020 7275 6e5f 696e 5f74 6572        run_in_ter
+000115f0: 6d69 6e61 6c28 6c61 6d62 6461 3a20 7072  minal(lambda: pr
+00011600: 696e 7431 2866 224d 756c 7469 2d6c 696e  int1(f"Multi-lin
+00011610: 6520 696e 7075 7420 7b27 656e 6162 6c65  e input {'enable
+00011620: 6427 2069 6620 636f 6e66 6967 2e6d 756c  d' if config.mul
+00011630: 7469 6c69 6e65 496e 7075 7420 656c 7365  tilineInput else
+00011640: 2027 6469 7361 626c 6564 277d 2122 2929   'disabled'}!"))
+00011650: 0a20 2020 2020 2020 2069 6620 636f 6e66  .        if conf
+00011660: 6967 2e6d 756c 7469 6c69 6e65 496e 7075  ig.multilineInpu
+00011670: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
+00011680: 756e 5f69 6e5f 7465 726d 696e 616c 286c  un_in_terminal(l
+00011690: 616d 6264 613a 2070 7269 6e74 3128 2255  ambda: print1("U
+000116a0: 7365 2027 6573 6361 7065 202b 2065 6e74  se 'escape + ent
+000116b0: 6572 2720 746f 2063 6f6d 706c 6574 6520  er' to complete 
+000116c0: 796f 7572 2065 6e74 7279 2e22 2929 0a0a  your entry."))..
+000116d0: 2020 2020 6465 6620 6973 5474 7341 7661      def isTtsAva
+000116e0: 696c 6162 6c65 2873 656c 6629 3a0a 2020  ilable(self):.  
+000116f0: 2020 2020 2020 6966 206e 6f74 2063 6f6e        if not con
+00011700: 6669 672e 6973 566c 6350 6c61 7965 7249  fig.isVlcPlayerI
+00011710: 6e73 7461 6c6c 6564 2061 6e64 206e 6f74  nstalled and not
+00011720: 2063 6f6e 6669 672e 6973 5079 6761 6d65   config.isPygame
+00011730: 496e 7374 616c 6c65 6420 616e 6420 6e6f  Installed and no
+00011740: 7420 636f 6e66 6967 2e74 7473 436f 6d6d  t config.ttsComm
+00011750: 616e 6420 616e 6420 6e6f 7420 636f 6e66  and and not conf
+00011760: 6967 2e65 6c65 7665 6e6c 6162 7341 7069  ig.elevenlabsApi
+00011770: 3a0a 2020 2020 2020 2020 2020 2020 7072  :.            pr
+00011780: 696e 7432 2822 5465 7874 2d74 6f2d 7370  int2("Text-to-sp
+00011790: 6565 6368 2066 6561 7475 7265 2069 7320  eech feature is 
+000117a0: 6e6f 7420 656e 6162 6c65 6421 2229 0a20  not enabled!"). 
+000117b0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+000117c0: 3328 2252 6561 643a 2068 7474 7073 3a2f  3("Read: https:/
+000117d0: 2f67 6974 6875 622e 636f 6d2f 656c 6972  /github.com/elir
+000117e0: 616e 776f 6e67 2f6c 6574 6d65 646f 6974  anwong/letmedoit
+000117f0: 2f77 696b 692f 6c65 744d 6544 6f49 742d  /wiki/letMeDoIt-
+00011800: 5370 6561 6b73 2229 0a20 2020 2020 2020  Speaks").       
+00011810: 2020 2020 2063 6f6e 6669 672e 7474 7320       config.tts 
+00011820: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00011830: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00011840: 2020 636f 6e66 6967 2e74 7473 203d 2054    config.tts = T
+00011850: 7275 650a 2020 2020 2020 2020 7265 7475  rue.        retu
+00011860: 726e 2063 6f6e 6669 672e 7474 730a 0a20  rn config.tts.. 
+00011870: 2020 2064 6566 2074 6f67 676c 6569 6e70     def toggleinp
+00011880: 7574 6175 6469 6f28 7365 6c66 293a 0a20  utaudio(self):. 
+00011890: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
+000118a0: 7354 7473 4176 6169 6c61 626c 653a 0a20  sTtsAvailable:. 
+000118b0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+000118c0: 672e 7474 7349 6e70 7574 203d 206e 6f74  g.ttsInput = not
+000118d0: 2063 6f6e 6669 672e 7474 7349 6e70 7574   config.ttsInput
+000118e0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+000118f0: 6669 672e 7361 7665 436f 6e66 6967 2829  fig.saveConfig()
+00011900: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00011910: 6e74 3328 6622 496e 7075 7420 4175 6469  nt3(f"Input Audi
+00011920: 6f3a 2027 7b27 656e 6162 6c65 6427 2069  o: '{'enabled' i
+00011930: 6620 636f 6e66 6967 2e74 7473 496e 7075  f config.ttsInpu
+00011940: 7420 656c 7365 2027 6469 7361 626c 6564  t else 'disabled
+00011950: 277d 2721 2229 0a0a 2020 2020 6465 6620  '}'!")..    def 
+00011960: 746f 6767 6c65 7265 7370 6f6e 7365 6175  toggleresponseau
+00011970: 6469 6f28 7365 6c66 293a 0a20 2020 2020  dio(self):.     
+00011980: 2020 2069 6620 7365 6c66 2e69 7354 7473     if self.isTts
+00011990: 4176 6169 6c61 626c 653a 0a20 2020 2020  Available:.     
+000119a0: 2020 2020 2020 2063 6f6e 6669 672e 7474         config.tt
+000119b0: 734f 7574 7075 7420 3d20 6e6f 7420 636f  sOutput = not co
+000119c0: 6e66 6967 2e74 7473 4f75 7470 7574 0a20  nfig.ttsOutput. 
+000119d0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+000119e0: 672e 7361 7665 436f 6e66 6967 2829 0a20  g.saveConfig(). 
+000119f0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00011a00: 3328 6622 5265 7370 6f6e 7365 2041 7564  3(f"Response Aud
+00011a10: 696f 3a20 277b 2765 6e61 626c 6564 2720  io: '{'enabled' 
+00011a20: 6966 2063 6f6e 6669 672e 7474 734f 7574  if config.ttsOut
+00011a30: 7075 7420 656c 7365 2027 6469 7361 626c  put else 'disabl
+00011a40: 6564 277d 2721 2229 0a0a 2020 2020 6465  ed'}'!")..    de
+00011a50: 6620 6465 6669 6e65 5474 7343 6f6d 6d61  f defineTtsComma
+00011a60: 6e64 2873 656c 6629 3a0a 2020 2020 2020  nd(self):.      
+00011a70: 2020 7072 696e 7431 2822 4465 6669 6e65    print1("Define
+00011a80: 2063 7573 746f 6d20 7465 7874 2d74 6f2d   custom text-to-
+00011a90: 7370 6565 6368 2063 6f6d 6d61 6e64 2062  speech command b
+00011aa0: 656c 6f77 3a22 290a 2020 2020 2020 2020  elow:").        
+00011ab0: 7072 696e 7431 2822 2222 2a20 6f6e 206d  print1("""* on m
+00011ac0: 6163 4f53 205b 2773 6179 202d 7620 223f  acOS ['say -v "?
+00011ad0: 2227 2074 6f20 6368 6563 6b20 766f 6963  "' to check voic
+00011ae0: 6573 5d2c 2065 2e67 2e3a 5c6e 2773 6179  es], e.g.:\n'say
+00011af0: 2720 6f72 2027 7361 7920 2d72 2032 3030  ' or 'say -r 200
+00011b00: 202d 7620 4461 6e69 656c 2722 2222 290a   -v Daniel'""").
+00011b10: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+00011b20: 2a20 6f6e 2055 6275 6e74 7520 5b27 6573  * on Ubuntu ['es
+00011b30: 7065 616b 202d 2d76 6f69 6365 7327 2074  peak --voices' t
+00011b40: 6f20 6368 6563 6b20 766f 6963 6573 5d2c  o check voices],
+00011b50: 2065 2e67 2e3a 5c6e 2765 7370 6561 6b27   e.g.:\n'espeak'
+00011b60: 206f 7220 2765 7370 6561 6b20 2d73 2031   or 'espeak -s 1
+00011b70: 3735 202d 7620 656e 2d67 6227 2229 0a20  75 -v en-gb'"). 
+00011b80: 2020 2020 2020 2070 7269 6e74 3128 222a         print1("*
+00011b90: 206f 6e20 5769 6e64 6f77 732c 2073 696d   on Windows, sim
+00011ba0: 706c 7920 656e 7465 7220 2777 696e 646f  ply enter 'windo
+00011bb0: 7773 2720 6865 7265 2074 6f20 7573 6520  ws' here to use 
+00011bc0: 5769 6e64 6f77 7320 6275 696c 742d 696e  Windows built-in
+00011bd0: 2073 7065 6563 6820 656e 6769 6e65 2229   speech engine")
+00011be0: 2023 206c 6574 6d65 646f 6974 2e61 6920   # letmedoit.ai 
+00011bf0: 7769 6c6c 2068 616e 646c 6520 7468 6520  will handle the 
+00011c00: 636f 6d6d 616e 6420 666f 7220 5769 6e64  command for Wind
+00011c10: 6f77 7320 7573 6572 730a 2020 2020 2020  ows users.      
+00011c20: 2020 7072 696e 7431 2822 7265 6d61 726b    print1("remark
+00011c30: 733a 2061 6c77 6179 7320 706c 6163 6520  s: always place 
+00011c40: 7468 6520 766f 6963 6520 6f70 7469 6f6e  the voice option
+00011c50: 2c20 6966 2061 6e79 2c20 6174 2074 6865  , if any, at the
+00011c60: 2065 6e64 2229 0a20 2020 2020 2020 2074   end").        t
+00011c70: 7473 436f 6d6d 616e 6420 3d20 7365 6c66  tsCommand = self
+00011c80: 2e70 726f 6d70 7473 2e73 696d 706c 6550  .prompts.simpleP
+00011c90: 726f 6d70 7428 7374 796c 653d 7365 6c66  rompt(style=self
+00011ca0: 2e70 726f 6d70 7473 2e70 726f 6d70 7453  .prompts.promptS
+00011cb0: 7479 6c65 322c 2064 6566 6175 6c74 3d63  tyle2, default=c
+00011cc0: 6f6e 6669 672e 7474 7343 6f6d 6d61 6e64  onfig.ttsCommand
+00011cd0: 290a 2020 2020 2020 2020 6966 2074 7473  ).        if tts
+00011ce0: 436f 6d6d 616e 643a 0a20 2020 2020 2020  Command:.       
+00011cf0: 2020 2020 2070 7269 6e74 3128 2253 7065       print1("Spe
+00011d00: 6369 6679 2063 6f6d 6d61 6e64 2073 7566  cify command suf
+00011d10: 6669 7820 6265 6c6f 772c 2069 6620 616e  fix below, if an
+00011d20: 7920 5b6c 6561 7665 2069 7420 626c 616e  y [leave it blan
+00011d30: 6b20 6966 204e 2f41 5d3a 2229 0a20 2020  k if N/A]:").   
+00011d40: 2020 2020 2020 2020 2074 7473 436f 6d6d           ttsComm
+00011d50: 616e 6453 7566 6669 7820 3d20 7365 6c66  andSuffix = self
+00011d60: 2e70 726f 6d70 7473 2e73 696d 706c 6550  .prompts.simpleP
+00011d70: 726f 6d70 7428 7374 796c 653d 7365 6c66  rompt(style=self
+00011d80: 2e70 726f 6d70 7473 2e70 726f 6d70 7453  .prompts.promptS
+00011d90: 7479 6c65 322c 2064 6566 6175 6c74 3d63  tyle2, default=c
+00011da0: 6f6e 6669 672e 7474 7343 6f6d 6d61 6e64  onfig.ttsCommand
+00011db0: 5375 6666 6978 290a 2020 2020 2020 2020  Suffix).        
+00011dc0: 2020 2020 6966 2074 7473 436f 6d6d 616e      if ttsComman
+00011dd0: 642e 6c6f 7765 7228 2920 3d3d 2022 7769  d.lower() == "wi
+00011de0: 6e64 6f77 7322 3a0a 2020 2020 2020 2020  ndows":.        
+00011df0: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+00011e00: 3d20 6627 2727 506f 7765 7253 6865 6c6c  = f'''PowerShell
+00011e10: 202d 436f 6d6d 616e 6420 2241 6464 2d54   -Command "Add-T
+00011e20: 7970 6520 e280 9341 7373 656d 626c 794e  ype ...AssemblyN
+00011e30: 616d 6520 5379 7374 656d 2e53 7065 6563  ame System.Speec
+00011e40: 683b 2028 4e65 772d 4f62 6a65 6374 2053  h; (New-Object S
+00011e50: 7973 7465 6d2e 5370 6565 6368 2e53 796e  ystem.Speech.Syn
+00011e60: 7468 6573 6973 2e53 7065 6563 6853 796e  thesis.SpeechSyn
+00011e70: 7468 6573 697a 6572 292e 5370 6561 6b28  thesizer).Speak(
+00011e80: 2774 6573 7469 6e67 2729 3b22 2727 270a  'testing');"'''.
+00011e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011ea0: 7474 7343 6f6d 6d61 6e64 5375 6666 6978  ttsCommandSuffix
+00011eb0: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
+00011ec0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00011ed0: 2020 2020 2020 2020 636f 6d6d 616e 6420          command 
+00011ee0: 3d20 6627 2727 7b74 7473 436f 6d6d 616e  = f'''{ttsComman
+00011ef0: 647d 2022 7465 7374 696e 6722 7b74 7473  d} "testing"{tts
+00011f00: 436f 6d6d 616e 6453 7566 6669 787d 2727  CommandSuffix}''
+00011f10: 270a 2020 2020 2020 2020 2020 2020 5f2c  '.            _,
+00011f20: 2073 7464 4572 7220 3d20 7375 6270 726f   stdErr = subpro
+00011f30: 6365 7373 2e50 6f70 656e 2863 6f6d 6d61  cess.Popen(comma
+00011f40: 6e64 2c20 7368 656c 6c3d 5472 7565 2c20  nd, shell=True, 
+00011f50: 7374 646f 7574 3d73 7562 7072 6f63 6573  stdout=subproces
+00011f60: 732e 5049 5045 2c20 7374 6465 7272 3d73  s.PIPE, stderr=s
+00011f70: 7562 7072 6f63 6573 732e 5049 5045 292e  ubprocess.PIPE).
+00011f80: 636f 6d6d 756e 6963 6174 6528 290a 2020  communicate().  
+00011f90: 2020 2020 2020 2020 2020 6966 2073 7464            if std
+00011fa0: 4572 723a 0a20 2020 2020 2020 2020 2020  Err:.           
+00011fb0: 2020 2020 2073 686f 7745 7272 6f72 7328       showErrors(
+00011fc0: 2920 6966 2063 6f6e 6669 672e 6465 7665  ) if config.deve
+00011fd0: 6c6f 7065 7220 656c 7365 2070 7269 6e74  loper else print
+00011fe0: 3128 2245 6e74 6572 6564 2063 6f6d 6d61  1("Entered comma
+00011ff0: 6e64 2069 6e76 616c 6964 2122 290a 2020  nd invalid!").  
+00012000: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00012010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012020: 636f 6e66 6967 2e74 7473 436f 6d6d 616e  config.ttsComman
+00012030: 642c 2063 6f6e 6669 672e 7474 7343 6f6d  d, config.ttsCom
+00012040: 6d61 6e64 5375 6666 6978 203d 2074 7473  mandSuffix = tts
+00012050: 436f 6d6d 616e 642c 2074 7473 436f 6d6d  Command, ttsComm
+00012060: 616e 6453 7566 6669 780a 2020 2020 2020  andSuffix.      
+00012070: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00012080: 2e73 6176 6543 6f6e 6669 6728 290a 2020  .saveConfig().  
+00012090: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+000120a0: 2020 2020 2020 2020 636f 6e66 6967 2e74          config.t
+000120b0: 7473 436f 6d6d 616e 642c 2063 6f6e 6669  tsCommand, confi
+000120c0: 672e 7474 7343 6f6d 6d61 6e64 5375 6666  g.ttsCommandSuff
+000120d0: 6978 203d 2022 222c 2022 220a 0a20 2020  ix = "", ""..   
+000120e0: 2064 6566 2074 6f67 676c 6557 6f72 6457   def toggleWordW
+000120f0: 7261 7028 7365 6c66 293a 0a20 2020 2020  rap(self):.     
+00012100: 2020 2063 6f6e 6669 672e 7772 6170 576f     config.wrapWo
+00012110: 7264 7320 3d20 6e6f 7420 636f 6e66 6967  rds = not config
+00012120: 2e77 7261 7057 6f72 6473 0a20 2020 2020  .wrapWords.     
+00012130: 2020 2063 6f6e 6669 672e 7361 7665 436f     config.saveCo
+00012140: 6e66 6967 2829 0a20 2020 2020 2020 2070  nfig().        p
+00012150: 7269 6e74 3328 6622 576f 7264 2057 7261  rint3(f"Word Wra
+00012160: 703a 2027 7b27 656e 6162 6c65 6427 2069  p: '{'enabled' i
+00012170: 6620 636f 6e66 6967 2e77 7261 7057 6f72  f config.wrapWor
+00012180: 6473 2065 6c73 6520 2764 6973 6162 6c65  ds else 'disable
+00012190: 6427 7d27 2122 290a 0a20 2020 2064 6566  d'}'!")..    def
+000121a0: 2074 6f67 676c 654d 6f75 7365 5375 7070   toggleMouseSupp
+000121b0: 6f72 7428 7365 6c66 293a 0a20 2020 2020  ort(self):.     
+000121c0: 2020 2063 6f6e 6669 672e 6d6f 7573 6553     config.mouseS
+000121d0: 7570 706f 7274 203d 206e 6f74 2063 6f6e  upport = not con
+000121e0: 6669 672e 6d6f 7573 6553 7570 706f 7274  fig.mouseSupport
+000121f0: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
+00012200: 7361 7665 436f 6e66 6967 2829 0a20 2020  saveConfig().   
+00012210: 2020 2020 2070 7269 6e74 3328 6622 456e       print3(f"En
+00012220: 7472 7920 4d6f 7573 6520 5375 7070 6f72  try Mouse Suppor
+00012230: 743a 2027 7b27 656e 6162 6c65 6427 2069  t: '{'enabled' i
+00012240: 6620 636f 6e66 6967 2e6d 6f75 7365 5375  f config.mouseSu
+00012250: 7070 6f72 7420 656c 7365 2027 6469 7361  pport else 'disa
+00012260: 626c 6564 277d 2721 2229 0a0a 2020 2020  bled'}'!")..    
+00012270: 6465 6620 746f 6767 6c65 496d 7072 6f76  def toggleImprov
+00012280: 6564 5772 6974 696e 6728 7365 6c66 293a  edWriting(self):
+00012290: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
+000122a0: 6469 7370 6c61 7949 6d70 726f 7665 6457  displayImprovedW
+000122b0: 7269 7469 6e67 203d 206e 6f74 2063 6f6e  riting = not con
+000122c0: 6669 672e 6469 7370 6c61 7949 6d70 726f  fig.displayImpro
+000122d0: 7665 6457 7269 7469 6e67 0a20 2020 2020  vedWriting.     
+000122e0: 2020 2069 6620 636f 6e66 6967 2e64 6973     if config.dis
+000122f0: 706c 6179 496d 7072 6f76 6564 5772 6974  playImprovedWrit
+00012300: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+00012310: 2070 7269 6e74 3128 2250 6c65 6173 6520   print1("Please 
+00012320: 7370 6563 6966 7920 7468 6520 7772 6974  specify the writ
+00012330: 696e 6720 7374 796c 6520 6265 6c6f 773a  ing style below:
+00012340: 2229 0a20 2020 2020 2020 2020 2020 2073  ").            s
+00012350: 7479 6c65 203d 2073 656c 662e 7072 6f6d  tyle = self.prom
+00012360: 7074 732e 7369 6d70 6c65 5072 6f6d 7074  pts.simplePrompt
+00012370: 2873 7479 6c65 3d73 656c 662e 7072 6f6d  (style=self.prom
+00012380: 7074 732e 7072 6f6d 7074 5374 796c 6532  pts.promptStyle2
+00012390: 2c20 6465 6661 756c 743d 636f 6e66 6967  , default=config
+000123a0: 2e69 6d70 726f 7665 6457 7269 7469 6e67  .improvedWriting
+000123b0: 5379 746c 6529 0a20 2020 2020 2020 2020  Sytle).         
+000123c0: 2020 2069 6620 7374 796c 6520 616e 6420     if style and 
+000123d0: 6e6f 7420 7374 796c 6520 696e 2028 636f  not style in (co
+000123e0: 6e66 6967 2e65 7869 745f 656e 7472 792c  nfig.exit_entry,
+000123f0: 2063 6f6e 6669 672e 6361 6e63 656c 5f65   config.cancel_e
+00012400: 6e74 7279 293a 0a20 2020 2020 2020 2020  ntry):.         
+00012410: 2020 2020 2020 2063 6f6e 6669 672e 696d         config.im
+00012420: 7072 6f76 6564 5772 6974 696e 6753 7974  provedWritingSyt
+00012430: 6c65 203d 2073 7479 6c65 0a20 2020 2020  le = style.     
+00012440: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00012450: 672e 7361 7665 436f 6e66 6967 2829 0a20  g.saveConfig(). 
+00012460: 2020 2020 2020 2070 7269 6e74 3328 6622         print3(f"
+00012470: 496d 7072 6f76 6564 2057 7269 7469 6e67  Improved Writing
+00012480: 2044 6973 706c 6179 3a20 277b 2765 6e61   Display: '{'ena
+00012490: 626c 6564 2720 6966 2063 6f6e 6669 672e  bled' if config.
+000124a0: 6469 7370 6c61 7949 6d70 726f 7665 6457  displayImprovedW
+000124b0: 7269 7469 6e67 2065 6c73 6520 2764 6973  riting else 'dis
+000124c0: 6162 6c65 6427 7d27 2122 290a 0a20 2020  abled'}'!")..   
+000124d0: 2064 6566 2073 6574 4175 6469 6f50 6c61   def setAudioPla
+000124e0: 7962 6163 6b54 6f6f 6c28 7365 6c66 293a  ybackTool(self):
+000124f0: 0a20 2020 2020 2020 2070 6c61 7962 6163  .        playbac
+00012500: 6b20 3d20 7365 6c66 2e64 6961 6c6f 6773  k = self.dialogs
+00012510: 2e67 6574 5661 6c69 644f 7074 696f 6e73  .getValidOptions
+00012520: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
+00012530: 7469 6f6e 733d 2822 7079 6761 6d65 222c  tions=("pygame",
+00012540: 2022 766c 6322 292c 0a20 2020 2020 2020   "vlc"),.       
+00012550: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00012560: 733d 2822 5079 4761 6d65 222c 2066 2256  s=("PyGame", f"V
+00012570: 4c43 2050 6c61 7965 7220 2877 2f20 7370  LC Player (w/ sp
+00012580: 6565 6420 636f 6e74 726f 6c29 7b27 205b  eed control){' [
+00012590: 696e 7374 616c 6c61 7469 6f6e 2072 6571  installation req
+000125a0: 7569 7265 645d 2720 6966 206e 6f74 2063  uired]' if not c
+000125b0: 6f6e 6669 672e 6973 566c 6350 6c61 7965  onfig.isVlcPlaye
+000125c0: 7249 6e73 7461 6c6c 6564 2065 6c73 6520  rInstalled else 
+000125d0: 2727 7d22 292c 0a20 2020 2020 2020 2020  ''}"),.         
+000125e0: 2020 2074 6974 6c65 3d22 5465 7874 2d74     title="Text-t
+000125f0: 6f2d 5370 6565 6368 2050 6c61 7962 6163  o-Speech Playbac
+00012600: 6b22 2c0a 2020 2020 2020 2020 2020 2020  k",.            
+00012610: 7465 7874 3d22 5365 6c65 6374 2061 2074  text="Select a t
+00012620: 6578 742d 746f 2d73 7065 6563 6820 706c  ext-to-speech pl
+00012630: 6163 6b62 6163 6b20 746f 6f6c 3a22 2c0a  ackback tool:",.
+00012640: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+00012650: 756c 743d 2276 6c63 2220 6966 2063 6f6e  ult="vlc" if con
+00012660: 6669 672e 6973 566c 6350 6c61 7965 7249  fig.isVlcPlayerI
+00012670: 6e73 7461 6c6c 6564 2061 6e64 206e 6f74  nstalled and not
+00012680: 2063 6f6e 6669 672e 7573 6550 7967 616d   config.usePygam
+00012690: 6520 656c 7365 2022 7079 6761 6d65 222c  e else "pygame",
+000126a0: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+000126b0: 2020 2069 6620 706c 6179 6261 636b 3a0a     if playback:.
+000126c0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+000126d0: 6c61 7962 6163 6b20 3d3d 2022 766c 6322  layback == "vlc"
+000126e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000126f0: 2020 6966 206e 6f74 2063 6f6e 6669 672e    if not config.
+00012700: 6973 566c 6350 6c61 7965 7249 6e73 7461  isVlcPlayerInsta
+00012710: 6c6c 6564 3a0a 2020 2020 2020 2020 2020  lled:.          
+00012720: 2020 2020 2020 2020 2020 7072 696e 7431            print1
+00012730: 2822 564c 4320 706c 6179 6572 206e 6f74  ("VLC player not
+00012740: 2066 6f75 6e64 2120 496e 7374 616c 6c20   found! Install 
+00012750: 6974 2066 6972 7374 2122 290a 2020 2020  it first!").    
+00012760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012770: 7072 696e 7433 2822 5465 7874 2d74 6f2d  print3("Text-to-
+00012780: 5370 6565 6368 2050 6c61 7962 6163 6b20  Speech Playback 
+00012790: 6368 616e 6765 6420 746f 3a20 5079 4761  changed to: PyGa
+000127a0: 6d65 2229 0a20 2020 2020 2020 2020 2020  me").           
+000127b0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+000127c0: 7573 6550 7967 616d 6520 3d20 5472 7565  usePygame = True
+000127d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000127e0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000127f0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00012800: 672e 7573 6550 7967 616d 6520 3d20 4661  g.usePygame = Fa
+00012810: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00012820: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00012830: 2020 2020 2020 636f 6e66 6967 2e75 7365        config.use
+00012840: 5079 6761 6d65 203d 2054 7275 650a 0a20  Pygame = True.. 
+00012850: 2020 2064 6566 2073 6574 5465 7874 546f     def setTextTo
+00012860: 5370 6565 6368 436f 6e66 6967 2873 656c  SpeechConfig(sel
+00012870: 6629 3a0a 2020 2020 2020 2020 7474 7350  f):.        ttsP
+00012880: 6c61 7466 6f72 6d20 3d20 7365 6c66 2e64  latform = self.d
+00012890: 6961 6c6f 6773 2e67 6574 5661 6c69 644f  ialogs.getValidO
+000128a0: 7074 696f 6e73 280a 2020 2020 2020 2020  ptions(.        
+000128b0: 2020 2020 6f70 7469 6f6e 733d 2822 676f      options=("go
+000128c0: 6f67 6c65 222c 2022 676f 6f67 6c65 636c  ogle", "googlecl
+000128d0: 6f75 6422 2c20 2265 6c65 7665 6e6c 6162  oud", "elevenlab
+000128e0: 7322 2c20 2263 7573 746f 6d22 292c 0a20  s", "custom"),. 
+000128f0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00012900: 6970 7469 6f6e 733d 2822 476f 6f67 6c65  iptions=("Google
+00012910: 2054 6578 742d 746f 2d53 7065 6563 6820   Text-to-Speech 
+00012920: 2847 656e 6572 6963 2922 2c20 2247 6f6f  (Generic)", "Goo
+00012930: 676c 6520 5465 7874 2d74 6f2d 5370 6565  gle Text-to-Spee
+00012940: 6368 2028 4150 4929 222c 2022 456c 6576  ch (API)", "Elev
+00012950: 656e 4c61 6273 2028 4150 4929 222c 2022  enLabs (API)", "
+00012960: 4375 7374 6f6d 2054 6578 742d 746f 2d53  Custom Text-to-S
+00012970: 7065 6563 6820 436f 6d6d 616e 6420 5b61  peech Command [a
+00012980: 6476 616e 6365 645d 2229 2c0a 2020 2020  dvanced]"),.    
+00012990: 2020 2020 2020 2020 7469 746c 653d 2254          title="T
+000129a0: 6578 742d 746f 2d53 7065 6563 6820 436f  ext-to-Speech Co
+000129b0: 6e66 6967 7572 6174 696f 6e73 222c 0a20  nfigurations",. 
+000129c0: 2020 2020 2020 2020 2020 2074 6578 743d             text=
+000129d0: 2253 656c 6563 7420 6120 7465 7874 2d74  "Select a text-t
+000129e0: 6f2d 7370 6565 6368 2070 6c61 7466 6f72  o-speech platfor
+000129f0: 6d3a 222c 0a20 2020 2020 2020 2020 2020  m:",.           
+00012a00: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
+00012a10: 7474 7350 6c61 7466 6f72 6d2c 0a20 2020  ttsPlatform,.   
+00012a20: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+00012a30: 6620 7474 7350 6c61 7466 6f72 6d3a 0a20  f ttsPlatform:. 
+00012a40: 2020 2020 2020 2020 2020 2069 6620 7474             if tt
+00012a50: 7350 6c61 7466 6f72 6d20 3d3d 2022 676f  sPlatform == "go
+00012a60: 6f67 6c65 636c 6f75 6422 2061 6e64 206e  oglecloud" and n
+00012a70: 6f74 2028 6f73 2e65 6e76 6972 6f6e 5b22  ot (os.environ["
+00012a80: 474f 4f47 4c45 5f41 5050 4c49 4341 5449  GOOGLE_APPLICATI
+00012a90: 4f4e 5f43 5245 4445 4e54 4941 4c53 225d  ON_CREDENTIALS"]
+00012aa0: 2061 6e64 2022 5465 7874 2d74 6f2d 5370   and "Text-to-Sp
+00012ab0: 6565 6368 2220 696e 2063 6f6e 6669 672e  eech" in config.
+00012ac0: 656e 6162 6c65 6447 6f6f 676c 6541 5049  enabledGoogleAPI
+00012ad0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
+00012ae0: 2020 2020 7072 696e 7432 2822 476f 6f67      print2("Goog
+00012af0: 6c65 2043 6c6f 7564 2054 6578 742d 746f  le Cloud Text-to
+00012b00: 2d53 7065 6563 6820 6665 6174 7572 6520  -Speech feature 
+00012b10: 6973 206e 6f74 2065 6e61 626c 6564 2122  is not enabled!"
+00012b20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012b30: 2020 7072 696e 7433 2822 5265 6164 3a20    print3("Read: 
+00012b40: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00012b50: 6f6d 2f65 6c69 7261 6e77 6f6e 672f 6c65  om/eliranwong/le
+00012b60: 746d 6564 6f69 742f 7769 6b69 2f47 6f6f  tmedoit/wiki/Goo
+00012b70: 676c 652d 4150 492d 5365 7475 7022 290a  gle-API-Setup").
+00012b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b90: 7072 696e 7433 2822 5465 7874 2d74 6f2d  print3("Text-to-
+00012ba0: 5370 6565 6368 2070 6c61 7466 6f72 6d20  Speech platform 
+00012bb0: 6368 616e 6765 6420 746f 3a20 476f 6f67  changed to: Goog
+00012bc0: 6c65 2054 6578 742d 746f 2d53 7065 6563  le Text-to-Speec
+00012bd0: 6820 2847 656e 6572 6963 2922 290a 2020  h (Generic)").  
+00012be0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00012bf0: 6e66 6967 2e74 7473 506c 6174 666f 726d  nfig.ttsPlatform
+00012c00: 203d 2022 676f 6f67 6c65 220a 2020 2020   = "google".    
+00012c10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00012c20: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00012c30: 6e66 6967 2e74 7473 506c 6174 666f 726d  nfig.ttsPlatform
+00012c40: 203d 2074 7473 506c 6174 666f 726d 0a20   = ttsPlatform. 
+00012c50: 2020 2020 2020 2023 2066 7572 7468 6572         # further
+00012c60: 206f 7074 696f 6e73 0a20 2020 2020 2020   options.       
+00012c70: 2069 6620 636f 6e66 6967 2e74 7473 506c   if config.ttsPl
+00012c80: 6174 666f 726d 203d 3d20 2267 6f6f 676c  atform == "googl
+00012c90: 6522 3a0a 2020 2020 2020 2020 2020 2020  e":.            
+00012ca0: 7365 6c66 2e73 6574 4774 7473 4c61 6e67  self.setGttsLang
+00012cb0: 7561 6765 2829 0a20 2020 2020 2020 2020  uage().         
+00012cc0: 2020 2073 656c 662e 7365 7441 7564 696f     self.setAudio
+00012cd0: 506c 6179 6261 636b 546f 6f6c 2829 0a20  PlaybackTool(). 
+00012ce0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012cf0: 7365 7456 6c63 5370 6565 6428 290a 2020  setVlcSpeed().  
+00012d00: 2020 2020 2020 656c 6966 2063 6f6e 6669        elif confi
+00012d10: 672e 7474 7350 6c61 7466 6f72 6d20 3d3d  g.ttsPlatform ==
+00012d20: 2022 676f 6f67 6c65 636c 6f75 6422 3a0a   "googlecloud":.
+00012d30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00012d40: 2e73 6574 4763 7474 734c 616e 6775 6167  .setGcttsLanguag
+00012d50: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+00012d60: 7365 6c66 2e73 6574 4763 7474 7353 7065  self.setGcttsSpe
+00012d70: 6564 2829 0a20 2020 2020 2020 2020 2020  ed().           
+00012d80: 2073 656c 662e 7365 7441 7564 696f 506c   self.setAudioPl
+00012d90: 6179 6261 636b 546f 6f6c 2829 0a20 2020  aybackTool().   
+00012da0: 2020 2020 2020 2020 2073 656c 662e 7365           self.se
+00012db0: 7456 6c63 5370 6565 6428 290a 2020 2020  tVlcSpeed().    
+00012dc0: 2020 2020 656c 6966 2063 6f6e 6669 672e      elif config.
+00012dd0: 7474 7350 6c61 7466 6f72 6d20 3d3d 2022  ttsPlatform == "
+00012de0: 656c 6576 656e 6c61 6273 223a 0a20 2020  elevenlabs":.   
+00012df0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00012e00: 636f 6e66 6967 2e65 6c65 7665 6e6c 6162  config.elevenlab
+00012e10: 7341 7069 3a0a 2020 2020 2020 2020 2020  sApi:.          
+00012e20: 2020 2020 2020 7365 6c66 2e63 6861 6e67        self.chang
+00012e30: 6545 6c65 7665 6e6c 6162 7341 7069 2829  eElevenlabsApi()
+00012e40: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00012e50: 6e6f 7420 636f 6e66 6967 2e65 6c65 7665  not config.eleve
+00012e60: 6e6c 6162 7341 7069 3a0a 2020 2020 2020  nlabsApi:.      
+00012e70: 2020 2020 2020 2020 2020 7072 696e 7431            print1
+00012e80: 2822 456c 6576 656e 4c61 6273 2041 5049  ("ElevenLabs API
+00012e90: 206b 6579 206e 6f74 2066 6f75 6e64 2122   key not found!"
+00012ea0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012eb0: 2020 7072 696e 7433 2822 5465 7874 2d74    print3("Text-t
+00012ec0: 6f2d 5370 6565 6368 2070 6c61 7466 6f72  o-Speech platfor
+00012ed0: 6d20 6368 616e 6765 6420 746f 3a20 476f  m changed to: Go
+00012ee0: 6f67 6c65 2054 6578 742d 746f 2d53 7065  ogle Text-to-Spe
+00012ef0: 6563 6820 2847 656e 6572 6963 2922 290a  ech (Generic)").
+00012f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f10: 636f 6e66 6967 2e74 7473 506c 6174 666f  config.ttsPlatfo
+00012f20: 726d 203d 2022 676f 6f67 6c65 220a 2020  rm = "google".  
+00012f30: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00012f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012f50: 7365 6c66 2e73 6574 456c 6576 656e 6c61  self.setElevenla
+00012f60: 6273 566f 6963 6528 290a 2020 2020 2020  bsVoice().      
+00012f70: 2020 656c 6966 2063 6f6e 6669 672e 7474    elif config.tt
+00012f80: 7350 6c61 7466 6f72 6d20 3d3d 2022 6375  sPlatform == "cu
+00012f90: 7374 6f6d 223a 0a20 2020 2020 2020 2020  stom":.         
+00012fa0: 2020 2073 656c 662e 6465 6669 6e65 5474     self.defineTt
+00012fb0: 7343 6f6d 6d61 6e64 2829 0a20 2020 2020  sCommand().     
+00012fc0: 2020 2023 2073 6176 6520 636f 6e66 6967     # save config
+00012fd0: 730a 2020 2020 2020 2020 636f 6e66 6967  s.        config
+00012fe0: 2e73 6176 6543 6f6e 6669 6728 290a 0a20  .saveConfig().. 
+00012ff0: 2020 2064 6566 2073 6574 566f 6963 6554     def setVoiceT
+00013000: 7970 696e 6743 6f6e 6669 6728 7365 6c66  ypingConfig(self
+00013010: 293a 0a20 2020 2020 2020 2076 6f69 6365  ):.        voice
+00013020: 5479 7069 6e67 506c 6174 666f 726d 203d  TypingPlatform =
+00013030: 2073 656c 662e 6469 616c 6f67 732e 6765   self.dialogs.ge
+00013040: 7456 616c 6964 4f70 7469 6f6e 7328 0a20  tValidOptions(. 
+00013050: 2020 2020 2020 2020 2020 206f 7074 696f             optio
+00013060: 6e73 3d28 2267 6f6f 676c 6522 2c20 2267  ns=("google", "g
+00013070: 6f6f 676c 6563 6c6f 7564 222c 2022 7768  ooglecloud", "wh
+00013080: 6973 7065 7222 292c 0a20 2020 2020 2020  isper"),.       
+00013090: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+000130a0: 733d 2822 476f 6f67 6c65 2053 7065 6563  s=("Google Speec
+000130b0: 682d 746f 2d54 6578 7420 2847 656e 6572  h-to-Text (Gener
+000130c0: 6963 2920 5b6f 6e6c 696e 655d 222c 2022  ic) [online]", "
+000130d0: 476f 6f67 6c65 2053 7065 6563 682d 746f  Google Speech-to
+000130e0: 2d54 6578 7420 2841 5049 2920 5b6f 6e6c  -Text (API) [onl
+000130f0: 696e 655d 222c 2022 4f70 656e 4149 2057  ine]", "OpenAI W
+00013100: 6869 7370 6572 205b 6f66 666c 696e 653b  hisper [offline;
+00013110: 2073 6c6f 7765 7220 7769 7468 206e 6f6e   slower with non
+00013120: 2d45 6e67 6c69 7368 2076 6f69 6365 735d  -English voices]
+00013130: 2229 2c0a 2020 2020 2020 2020 2020 2020  "),.            
+00013140: 7469 746c 653d 2256 6f69 6365 2054 7970  title="Voice Typ
+00013150: 696e 6720 436f 6e66 6967 7572 6174 696f  ing Configuratio
+00013160: 6e73 222c 0a20 2020 2020 2020 2020 2020  ns",.           
+00013170: 2074 6578 743d 2253 656c 6563 7420 6120   text="Select a 
+00013180: 766f 6963 6520 7479 7069 6e67 2070 6c61  voice typing pla
+00013190: 7466 6f72 6d3a 222c 0a20 2020 2020 2020  tform:",.       
+000131a0: 2020 2020 2064 6566 6175 6c74 3d63 6f6e       default=con
+000131b0: 6669 672e 766f 6963 6554 7970 696e 6750  fig.voiceTypingP
+000131c0: 6c61 7466 6f72 6d2c 0a20 2020 2020 2020  latform,.       
+000131d0: 2029 0a20 2020 2020 2020 2069 6620 766f   ).        if vo
+000131e0: 6963 6554 7970 696e 6750 6c61 7466 6f72  iceTypingPlatfor
+000131f0: 6d3a 0a20 2020 2020 2020 2020 2020 2069  m:.            i
+00013200: 6620 766f 6963 6554 7970 696e 6750 6c61  f voiceTypingPla
+00013210: 7466 6f72 6d20 3d3d 2022 676f 6f67 6c65  tform == "google
+00013220: 636c 6f75 6422 2061 6e64 206e 6f74 2028  cloud" and not (
+00013230: 6f73 2e65 6e76 6972 6f6e 5b22 474f 4f47  os.environ["GOOG
+00013240: 4c45 5f41 5050 4c49 4341 5449 4f4e 5f43  LE_APPLICATION_C
+00013250: 5245 4445 4e54 4941 4c53 225d 2061 6e64  REDENTIALS"] and
+00013260: 2022 5370 6565 6368 2d74 6f2d 5465 7874   "Speech-to-Text
+00013270: 2220 696e 2063 6f6e 6669 672e 656e 6162  " in config.enab
+00013280: 6c65 6447 6f6f 676c 6541 5049 7329 3a0a  ledGoogleAPIs):.
+00013290: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132a0: 7072 696e 7432 2822 476f 6f67 6c65 2043  print2("Google C
+000132b0: 6c6f 7564 2053 7065 6563 682d 746f 2d54  loud Speech-to-T
+000132c0: 6578 7420 6665 6174 7572 6520 6973 206e  ext feature is n
+000132d0: 6f74 2065 6e61 626c 6564 2122 290a 2020  ot enabled!").  
+000132e0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+000132f0: 696e 7433 2822 5265 6164 3a20 6874 7470  int3("Read: http
+00013300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00013310: 6c69 7261 6e77 6f6e 672f 6c65 746d 6564  liranwong/letmed
+00013320: 6f69 742f 7769 6b69 2f47 6f6f 676c 652d  oit/wiki/Google-
+00013330: 4150 492d 5365 7475 7022 290a 2020 2020  API-Setup").    
+00013340: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00013350: 7433 2822 566f 6963 6520 7479 7069 6e67  t3("Voice typing
+00013360: 2070 6c61 7466 6f72 6d20 6368 616e 6765   platform change
+00013370: 6420 746f 3a20 476f 6f67 6c65 2053 7065  d to: Google Spe
+00013380: 6563 682d 746f 2d54 6578 7420 2847 656e  ech-to-Text (Gen
+00013390: 6572 6963 2922 290a 2020 2020 2020 2020  eric)").        
+000133a0: 2020 2020 2020 2020 636f 6e66 6967 2e76          config.v
+000133b0: 6f69 6365 5479 7069 6e67 506c 6174 666f  oiceTypingPlatfo
+000133c0: 726d 203d 2022 676f 6f67 6c65 220a 2020  rm = "google".  
+000133d0: 2020 2020 2020 2020 2020 656c 6966 2076            elif v
+000133e0: 6f69 6365 5479 7069 6e67 506c 6174 666f  oiceTypingPlatfo
+000133f0: 726d 203d 3d20 2277 6869 7370 6572 2220  rm == "whisper" 
+00013400: 616e 6420 6e6f 7420 6973 436f 6d6d 616e  and not isComman
+00013410: 6449 6e73 7461 6c6c 6564 2822 6666 6d70  dInstalled("ffmp
+00013420: 6567 2229 3a0a 2020 2020 2020 2020 2020  eg"):.          
+00013430: 2020 2020 2020 7072 696e 7432 2822 496e        print2("In
+00013440: 7374 616c 6c20 2766 666d 7065 6727 2066  stall 'ffmpeg' f
+00013450: 6972 7374 2074 6f20 7573 6520 6f66 666c  irst to use offl
+00013460: 696e 6520 6f70 656e 6169 2077 6869 7370  ine openai whisp
+00013470: 6572 206d 6f64 656c 2122 290a 2020 2020  er model!").    
+00013480: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00013490: 7433 2822 5265 6164 3a20 6874 7470 733a  t3("Read: https:
+000134a0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7065  //github.com/ope
+000134b0: 6e61 692f 7768 6973 7065 7223 7365 7475  nai/whisper#setu
+000134c0: 7022 290a 2020 2020 2020 2020 2020 2020  p").            
+000134d0: 2020 2020 7072 696e 7433 2822 566f 6963      print3("Voic
+000134e0: 6520 7479 7069 6e67 2070 6c61 7466 6f72  e typing platfor
+000134f0: 6d20 6368 616e 6765 6420 746f 3a20 476f  m changed to: Go
+00013500: 6f67 6c65 2053 7065 6563 682d 746f 2d54  ogle Speech-to-T
+00013510: 6578 7420 2847 656e 6572 6963 2922 290a  ext (Generic)").
+00013520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013530: 636f 6e66 6967 2e76 6f69 6365 5479 7069  config.voiceTypi
+00013540: 6e67 506c 6174 666f 726d 203d 2022 676f  ngPlatform = "go
+00013550: 6f67 6c65 220a 2020 2020 2020 2020 2020  ogle".          
+00013560: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00013570: 2020 2020 2020 2020 636f 6e66 6967 2e76          config.v
+00013580: 6f69 6365 5479 7069 6e67 506c 6174 666f  oiceTypingPlatfo
+00013590: 726d 203d 2076 6f69 6365 5479 7069 6e67  rm = voiceTyping
+000135a0: 506c 6174 666f 726d 0a20 2020 2020 2020  Platform.       
+000135b0: 2023 206c 616e 6775 6167 650a 2020 2020   # language.    
+000135c0: 2020 2020 7365 6c66 2e73 6574 5370 6565      self.setSpee
+000135d0: 6368 546f 5465 7874 4c61 6e67 7561 6765  chToTextLanguage
+000135e0: 2829 0a20 2020 2020 2020 2023 2063 6f6e  ().        # con
+000135f0: 6669 6775 7265 2063 6f6e 6669 672e 766f  figure config.vo
+00013600: 6963 6554 7970 696e 6741 646a 7573 7441  iceTypingAdjustA
+00013610: 6d62 6965 6e74 4e6f 6973 650a 2020 2020  mbientNoise.    
+00013620: 2020 2020 766f 6963 6554 7970 696e 6741      voiceTypingA
+00013630: 646a 7573 7441 6d62 6965 6e74 4e6f 6973  djustAmbientNois
+00013640: 6520 3d20 7365 6c66 2e64 6961 6c6f 6773  e = self.dialogs
+00013650: 2e67 6574 5661 6c69 644f 7074 696f 6e73  .getValidOptions
+00013660: 280a 2020 2020 2020 2020 2020 2020 6f70  (.            op
+00013670: 7469 6f6e 733d 2822 5965 7322 2c20 224e  tions=("Yes", "N
+00013680: 6f22 292c 0a20 2020 2020 2020 2020 2020  o"),.           
+00013690: 2064 6573 6372 6970 7469 6f6e 733d 2822   descriptions=("
+000136a0: 5965 7320 5b73 6c6f 7765 725d 222c 2022  Yes [slower]", "
+000136b0: 4e6f 2229 2c0a 2020 2020 2020 2020 2020  No"),.          
+000136c0: 2020 7469 746c 653d 2241 646a 7573 7420    title="Adjust 
+000136d0: 416d 6269 656e 7420 4e6f 6973 6522 2c0a  Ambient Noise",.
+000136e0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+000136f0: 3d22 446f 2079 6f75 2077 616e 7420 746f  ="Do you want to
+00013700: 2061 646a 7573 7420 616d 6269 656e 7420   adjust ambient 
+00013710: 6e6f 6973 653f 222c 0a20 2020 2020 2020  noise?",.       
+00013720: 2020 2020 2064 6566 6175 6c74 3d22 5965       default="Ye
+00013730: 7322 2069 6620 636f 6e66 6967 2e76 6f69  s" if config.voi
+00013740: 6365 5479 7069 6e67 4164 6a75 7374 416d  ceTypingAdjustAm
+00013750: 6269 656e 744e 6f69 7365 2065 6c73 6520  bientNoise else 
+00013760: 224e 6f22 2c0a 2020 2020 2020 2020 290a  "No",.        ).
+00013770: 2020 2020 2020 2020 6966 2076 6f69 6365          if voice
+00013780: 5479 7069 6e67 4164 6a75 7374 416d 6269  TypingAdjustAmbi
+00013790: 656e 744e 6f69 7365 3a0a 2020 2020 2020  entNoise:.      
+000137a0: 2020 2020 2020 636f 6e66 6967 2e76 6f69        config.voi
+000137b0: 6365 5479 7069 6e67 4164 6a75 7374 416d  ceTypingAdjustAm
+000137c0: 6269 656e 744e 6f69 7365 203d 2054 7275  bientNoise = Tru
+000137d0: 6520 6966 2076 6f69 6365 5479 7069 6e67  e if voiceTyping
+000137e0: 4164 6a75 7374 416d 6269 656e 744e 6f69  AdjustAmbientNoi
+000137f0: 7365 203d 3d20 2259 6573 2220 656c 7365  se == "Yes" else
+00013800: 2046 616c 7365 0a20 2020 2020 2020 2023   False.        #
+00013810: 2061 7564 696f 206e 6f74 6966 6963 6174   audio notificat
+00013820: 696f 6e0a 2020 2020 2020 2020 766f 6963  ion.        voic
+00013830: 6554 7970 696e 674e 6f74 6966 6963 6174  eTypingNotificat
+00013840: 696f 6e20 3d20 7365 6c66 2e64 6961 6c6f  ion = self.dialo
+00013850: 6773 2e67 6574 5661 6c69 644f 7074 696f  gs.getValidOptio
+00013860: 6e73 280a 2020 2020 2020 2020 2020 2020  ns(.            
+00013870: 6f70 7469 6f6e 733d 2822 5965 7322 2c20  options=("Yes", 
+00013880: 224e 6f22 292c 0a20 2020 2020 2020 2020  "No"),.         
+00013890: 2020 2074 6974 6c65 3d22 4175 6469 6f20     title="Audio 
+000138a0: 4e6f 7469 6669 6361 7469 6f6e 222c 0a20  Notification",. 
+000138b0: 2020 2020 2020 2020 2020 2074 6578 743d             text=
+000138c0: 2244 6f20 796f 7520 7761 6e74 2061 7564  "Do you want aud
+000138d0: 696f 206e 6f74 6966 6963 6174 696f 6e20  io notification 
+000138e0: 7768 656e 2079 6f75 2075 7365 206d 6963  when you use mic
+000138f0: 726f 7068 6f6e 653f 222c 0a20 2020 2020  rophone?",.     
+00013900: 2020 2020 2020 2064 6566 6175 6c74 3d22         default="
+00013910: 5965 7322 2069 6620 636f 6e66 6967 2e76  Yes" if config.v
+00013920: 6f69 6365 5479 7069 6e67 4e6f 7469 6669  oiceTypingNotifi
+00013930: 6361 7469 6f6e 2065 6c73 6520 224e 6f22  cation else "No"
+00013940: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00013950: 2020 2020 6966 2076 6f69 6365 5479 7069      if voiceTypi
+00013960: 6e67 4e6f 7469 6669 6361 7469 6f6e 3a0a  ngNotification:.
+00013970: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00013980: 6967 2e76 6f69 6365 5479 7069 6e67 4e6f  ig.voiceTypingNo
+00013990: 7469 6669 6361 7469 6f6e 203d 2054 7275  tification = Tru
+000139a0: 6520 6966 2076 6f69 6365 5479 7069 6e67  e if voiceTyping
+000139b0: 4e6f 7469 6669 6361 7469 6f6e 203d 3d20  Notification == 
+000139c0: 2259 6573 2220 656c 7365 2046 616c 7365  "Yes" else False
+000139d0: 0a20 2020 2020 2020 2023 2061 7574 6f20  .        # auto 
+000139e0: 636f 6d70 6c65 7469 6f6e 3a20 766f 6963  completion: voic
+000139f0: 6554 7970 696e 6741 7574 6f43 6f6d 706c  eTypingAutoCompl
+00013a00: 6574 650a 2020 2020 2020 2020 766f 6963  ete.        voic
+00013a10: 6554 7970 696e 6741 7574 6f43 6f6d 706c  eTypingAutoCompl
+00013a20: 6574 6520 3d20 7365 6c66 2e64 6961 6c6f  ete = self.dialo
+00013a30: 6773 2e67 6574 5661 6c69 644f 7074 696f  gs.getValidOptio
+00013a40: 6e73 280a 2020 2020 2020 2020 2020 2020  ns(.            
+00013a50: 6f70 7469 6f6e 733d 2822 5965 7322 2c20  options=("Yes", 
+00013a60: 224e 6f22 292c 0a20 2020 2020 2020 2020  "No"),.         
+00013a70: 2020 2074 6974 6c65 3d22 4175 6469 6f20     title="Audio 
+00013a80: 456e 7472 7920 4175 746f 2043 6f6d 706c  Entry Auto Compl
+00013a90: 6574 696f 6e22 2c0a 2020 2020 2020 2020  etion",.        
+00013aa0: 2020 2020 7465 7874 3d22 446f 2079 6f75      text="Do you
+00013ab0: 2077 616e 7420 746f 2061 7574 6f6d 6174   want to automat
+00013ac0: 6963 616c 6c79 2063 6f6d 706c 6574 6520  ically complete 
+00013ad0: 796f 7572 2065 6e74 7279 2077 6865 6e20  your entry when 
+00013ae0: 6d69 6372 6f70 686f 6e65 2073 746f 7073  microphone stops
+00013af0: 3f22 2c0a 2020 2020 2020 2020 2020 2020  ?",.            
+00013b00: 6465 6661 756c 743d 2259 6573 2220 6966  default="Yes" if
+00013b10: 2063 6f6e 6669 672e 766f 6963 6554 7970   config.voiceTyp
+00013b20: 696e 6741 7574 6f43 6f6d 706c 6574 6520  ingAutoComplete 
+00013b30: 656c 7365 2022 4e6f 222c 0a20 2020 2020  else "No",.     
+00013b40: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00013b50: 766f 6963 6554 7970 696e 6741 7574 6f43  voiceTypingAutoC
+00013b60: 6f6d 706c 6574 653a 0a20 2020 2020 2020  omplete:.       
+00013b70: 2020 2020 2063 6f6e 6669 672e 766f 6963       config.voic
+00013b80: 6554 7970 696e 6741 7574 6f43 6f6d 706c  eTypingAutoCompl
+00013b90: 6574 6520 3d20 5472 7565 2069 6620 766f  ete = True if vo
+00013ba0: 6963 6554 7970 696e 6741 7574 6f43 6f6d  iceTypingAutoCom
+00013bb0: 706c 6574 6520 3d3d 2022 5965 7322 2065  plete == "Yes" e
+00013bc0: 6c73 6520 4661 6c73 650a 2020 2020 2020  lse False.      
+00013bd0: 2020 2320 6e6f 7469 6679 0a20 2020 2020    # notify.     
+00013be0: 2020 2070 7269 6e74 2822 2229 0a20 2020     print("").   
+00013bf0: 2020 2020 2070 7269 6e74 3328 6622 566f       print3(f"Vo
+00013c00: 6963 6520 5479 7069 6e67 204d 6f64 656c  ice Typing Model
+00013c10: 3a20 7b63 6f6e 6669 672e 766f 6963 6554  : {config.voiceT
+00013c20: 7970 696e 6750 6c61 7466 6f72 6d7d 2229  ypingPlatform}")
+00013c30: 0a20 2020 2020 2020 2070 7269 6e74 3328  .        print3(
+00013c40: 6622 566f 6963 6520 5479 7069 6e67 204c  f"Voice Typing L
+00013c50: 616e 6775 6167 653a 207b 636f 6e66 6967  anguage: {config
+00013c60: 2e76 6f69 6365 5479 7069 6e67 4c61 6e67  .voiceTypingLang
+00013c70: 7561 6765 7d22 290a 2020 2020 2020 2020  uage}").        
+00013c80: 7072 696e 7433 2866 2241 6d62 6965 6e74  print3(f"Ambient
+00013c90: 204e 6f69 7365 2041 646a 7573 746d 656e   Noise Adjustmen
+00013ca0: 743a 207b 636f 6e66 6967 2e76 6f69 6365  t: {config.voice
+00013cb0: 5479 7069 6e67 4164 6a75 7374 416d 6269  TypingAdjustAmbi
+00013cc0: 656e 744e 6f69 7365 7d22 290a 2020 2020  entNoise}").    
+00013cd0: 2020 2020 7072 696e 7433 2866 2241 7564      print3(f"Aud
+00013ce0: 696f 204e 6f74 6966 6963 6174 696f 6e3a  io Notification:
+00013cf0: 207b 636f 6e66 6967 2e76 6f69 6365 5479   {config.voiceTy
+00013d00: 7069 6e67 4e6f 7469 6669 6361 7469 6f6e  pingNotification
+00013d10: 7d22 290a 2020 2020 2020 2020 7072 696e  }").        prin
+00013d20: 7433 2866 2241 7574 6f20 436f 6d70 6c65  t3(f"Auto Comple
+00013d30: 7469 6f6e 3a20 7b63 6f6e 6669 672e 766f  tion: {config.vo
+00013d40: 6963 6554 7970 696e 6741 7574 6f43 6f6d  iceTypingAutoCom
+00013d50: 706c 6574 657d 2229 0a20 2020 2020 2020  plete}").       
+00013d60: 2023 2073 6176 6520 636f 6e66 6967 730a   # save configs.
+00013d70: 2020 2020 2020 2020 636f 6e66 6967 2e73          config.s
+00013d80: 6176 6543 6f6e 6669 6728 290a 0a20 2020  aveConfig()..   
+00013d90: 2064 6566 2073 6176 6543 6861 7428 7365   def saveChat(se
+00013da0: 6c66 2c20 6d65 7373 6167 6573 293a 0a20  lf, messages):. 
+00013db0: 2020 2020 2020 206d 6573 7361 6765 7343         messagesC
+00013dc0: 6f70 7920 3d20 636f 7079 2e64 6565 7063  opy = copy.deepc
+00013dd0: 6f70 7928 6d65 7373 6167 6573 290a 0a20  opy(messages).. 
+00013de0: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
+00013df0: 2e63 6f6e 7665 7273 6174 696f 6e53 7461  .conversationSta
+00013e00: 7274 6564 3a0a 2020 2020 2020 2020 2020  rted:.          
+00013e10: 2020 7469 6d65 7374 616d 7020 3d20 6765    timestamp = ge
+00013e20: 7443 7572 7265 6e74 4461 7465 5469 6d65  tCurrentDateTime
+00013e30: 2829 0a0a 2020 2020 2020 2020 2020 2020  ()..            
+00013e40: 6966 2068 6173 6174 7472 2863 6f6e 6669  if hasattr(confi
+00013e50: 672c 2022 7361 7665 5f63 6861 745f 7265  g, "save_chat_re
+00013e60: 636f 7264 2229 3a0a 2020 2020 2020 2020  cord"):.        
+00013e70: 2020 2020 2020 2020 2320 7768 656e 2070          # when p
+00013e80: 6c75 6769 6e20 2273 6176 6520 6368 6174  lugin "save chat
+00013e90: 2072 6563 6f72 6473 2220 6973 2065 6e61   records" is ena
+00013ea0: 626c 6564 0a20 2020 2020 2020 2020 2020  bled.           
+00013eb0: 2020 2020 206d 6573 7361 6765 4c65 6e67       messageLeng
+00013ec0: 7468 203d 206c 656e 286d 6573 7361 6765  th = len(message
+00013ed0: 7343 6f70 7929 0a20 2020 2020 2020 2020  sCopy).         
+00013ee0: 2020 2020 2020 2066 6f72 206f 7264 6572         for order
+00013ef0: 2c20 6920 696e 2065 6e75 6d65 7261 7465  , i in enumerate
+00013f00: 286d 6573 7361 6765 7343 6f70 7929 3a0a  (messagesCopy):.
+00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f20: 2020 2020 6973 4c61 7374 4974 656d 203d      isLastItem =
+00013f30: 2028 6f72 6465 7220 3d3d 2028 6d65 7373   (order == (mess
+00013f40: 6167 654c 656e 6774 6820 2d20 3129 290a  ageLength - 1)).
+00013f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f60: 2020 2020 6966 2063 6f6e 6669 672e 6c6c      if config.ll
+00013f70: 6d49 6e74 6572 6661 6365 2069 6e20 2822  mInterface in ("
+00013f80: 6368 6174 6770 7422 2c20 226c 6574 6d65  chatgpt", "letme
+00013f90: 646f 6974 2229 2061 6e64 206e 6f74 2069  doit") and not i
+00013fa0: 734c 6173 7449 7465 6d20 616e 6420 692e  sLastItem and i.
+00013fb0: 6765 7428 2272 6f6c 6522 2c20 2222 2920  get("role", "") 
+00013fc0: 3d3d 2022 7573 6572 2220 616e 6420 2266  == "user" and "f
+00013fd0: 756e 6374 696f 6e5f 6361 6c6c 2220 696e  unction_call" in
+00013fe0: 206d 6573 7361 6765 7343 6f70 795b 6f72   messagesCopy[or
+00013ff0: 6465 722b 315d 3a0a 2020 2020 2020 2020  der+1]:.        
+00014000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014010: 695b 2274 6f6f 6c22 5d20 3d20 6d65 7373  i["tool"] = mess
+00014020: 6167 6573 436f 7079 5b6f 7264 6572 2b31  agesCopy[order+1
+00014030: 5d5b 2266 756e 6374 696f 6e5f 6361 6c6c  ]["function_call
+00014040: 225d 2e67 6574 2822 6e61 6d65 222c 2022  "].get("name", "
+00014050: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00014060: 2020 2020 2020 2063 6f6e 6669 672e 7361         config.sa
+00014070: 7665 5f63 6861 745f 7265 636f 7264 2874  ve_chat_record(t
+00014080: 696d 6573 7461 6d70 2c20 6f72 6465 722c  imestamp, order,
+00014090: 2069 290a 0a20 2020 2020 2020 2020 2020   i)..           
+000140a0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+000140b0: 2020 2020 2020 666f 6c64 6572 5061 7468        folderPath
+000140c0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+000140d0: 636f 6e66 6967 2e6c 6f63 616c 5374 6f72  config.localStor
+000140e0: 6167 652c 2022 6368 6174 7322 2c20 7265  age, "chats", re
+000140f0: 2e73 7562 2822 5e28 5b30 2d39 5d2b 3f5c  .sub("^([0-9]+?\
+00014100: 2d5b 302d 395d 2b3f 295c 2d2e 2a3f 2422  -[0-9]+?)\-.*?$"
+00014110: 2c20 7222 5c31 222c 2074 696d 6573 7461  , r"\1", timesta
+00014120: 6d70 2929 0a20 2020 2020 2020 2020 2020  mp)).           
+00014130: 2020 2020 2050 6174 6828 666f 6c64 6572       Path(folder
+00014140: 5061 7468 292e 6d6b 6469 7228 7061 7265  Path).mkdir(pare
+00014150: 6e74 733d 5472 7565 2c20 6578 6973 745f  nts=True, exist_
+00014160: 6f6b 3d54 7275 6529 0a20 2020 2020 2020  ok=True).       
+00014170: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
+00014180: 6174 682e 6973 6469 7228 666f 6c64 6572  ath.isdir(folder
+00014190: 5061 7468 293a 0a20 2020 2020 2020 2020  Path):.         
+000141a0: 2020 2020 2020 2020 2020 2063 6861 7446             chatF
+000141b0: 696c 6520 3d20 6f73 2e70 6174 682e 6a6f  ile = os.path.jo
+000141c0: 696e 2866 6f6c 6465 7250 6174 682c 2066  in(folderPath, f
+000141d0: 227b 7469 6d65 7374 616d 707d 2e74 7874  "{timestamp}.txt
+000141e0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+000141f0: 2020 2020 2020 2077 6974 6820 6f70 656e         with open
+00014200: 2863 6861 7446 696c 652c 2022 7722 2c20  (chatFile, "w", 
+00014210: 656e 636f 6469 6e67 3d22 7574 662d 3822  encoding="utf-8"
+00014220: 2920 6173 2066 696c 654f 626a 3a0a 2020  ) as fileObj:.  
+00014230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014240: 2020 2020 2020 6669 6c65 4f62 6a2e 7772        fileObj.wr
+00014250: 6974 6528 7070 7269 6e74 2e70 666f 726d  ite(pprint.pform
+00014260: 6174 286d 6573 7361 6765 7343 6f70 7929  at(messagesCopy)
+00014270: 290a 2020 2020 2020 2020 2020 2020 6578  ).            ex
+00014280: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+00014290: 2020 2020 2020 7072 696e 7432 2822 4661        print2("Fa
+000142a0: 696c 6564 2074 6f20 7361 7665 2063 6861  iled to save cha
+000142b0: 7421 5c6e 2229 0a20 2020 2020 2020 2020  t!\n").         
+000142c0: 2020 2020 2020 2073 686f 7745 7272 6f72         showError
+000142d0: 7328 290a 0a20 2020 2064 6566 2065 7870  s()..    def exp
+000142e0: 6f72 7443 6861 7428 7365 6c66 2c20 6d65  ortChat(self, me
+000142f0: 7373 6167 6573 2c20 6f70 656e 4669 6c65  ssages, openFile
+00014300: 3d54 7275 6529 3a0a 2020 2020 2020 2020  =True):.        
+00014310: 6966 2063 6f6e 6669 672e 636f 6e76 6572  if config.conver
+00014320: 7361 7469 6f6e 5374 6172 7465 643a 0a20  sationStarted:. 
+00014330: 2020 2020 2020 2020 2020 2070 6c61 696e             plain
+00014340: 5465 7874 203d 2022 220a 2020 2020 2020  Text = "".      
+00014350: 2020 2020 2020 7469 6d65 7374 616d 7020        timestamp 
+00014360: 3d20 6765 7443 7572 7265 6e74 4461 7465  = getCurrentDate
+00014370: 5469 6d65 2829 0a0a 2020 2020 2020 2020  Time()..        
+00014380: 2020 2020 666f 7220 6920 696e 206d 6573      for i in mes
+00014390: 7361 6765 733a 0a20 2020 2020 2020 2020  sages:.         
+000143a0: 2020 2020 2020 2069 6620 695b 2272 6f6c         if i["rol
+000143b0: 6522 5d20 3d3d 2022 7573 6572 223a 0a20  e"] == "user":. 
+000143c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143d0: 2020 2063 6f6e 7465 6e74 203d 2069 5b22     content = i["
+000143e0: 636f 6e74 656e 7422 5d0a 2020 2020 2020  content"].      
+000143f0: 2020 2020 2020 2020 2020 2020 2020 706c                pl
+00014400: 6169 6e54 6578 7420 2b3d 2066 223e 3e3e  ainText += f">>>
+00014410: 207b 636f 6e74 656e 747d 220a 2020 2020   {content}".    
+00014420: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+00014430: 5b22 726f 6c65 225d 203d 3d20 2266 756e  ["role"] == "fun
+00014440: 6374 696f 6e22 3a0a 2020 2020 2020 2020  ction":.        
+00014450: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00014460: 6c61 696e 5465 7874 3a0a 2020 2020 2020  lainText:.      
+00014470: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014480: 2020 706c 6169 6e54 6578 7420 2b3d 2022    plainText += "
+00014490: 5c6e 5c6e 220a 2020 2020 2020 2020 2020  \n\n".          
+000144a0: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
+000144b0: 2069 5b22 6e61 6d65 225d 0a20 2020 2020   i["name"].     
+000144c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000144d0: 6c61 696e 5465 7874 202b 3d20 6622 6060  lainText += f"``
+000144e0: 605c 6e7b 6e61 6d65 7d5c 6e60 6060 220a  `\n{name}\n```".
 000144f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014500: 2020 2020 2077 6974 6820 6f70 656e 2863       with open(c
-00014510: 6861 7446 696c 652c 2022 7722 2c20 656e  hatFile, "w", en
-00014520: 636f 6469 6e67 3d22 7574 662d 3822 2920  coding="utf-8") 
-00014530: 6173 2066 696c 654f 626a 3a0a 2020 2020  as fileObj:.    
-00014540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014550: 2020 2020 2020 2020 6669 6c65 4f62 6a2e          fileObj.
-00014560: 7772 6974 6528 706c 6169 6e54 6578 7429  write(plainText)
-00014570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014580: 2020 2020 2020 2020 2069 6620 6f70 656e           if open
-00014590: 4669 6c65 2061 6e64 206f 732e 7061 7468  File and os.path
-000145a0: 2e69 7366 696c 6528 6368 6174 4669 6c65  .isfile(chatFile
-000145b0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000145c0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000145d0: 732e 7379 7374 656d 2866 2727 277b 636f  s.system(f'''{co
-000145e0: 6e66 6967 2e6f 7065 6e7d 2022 7b63 6861  nfig.open} "{cha
-000145f0: 7446 696c 657d 2227 2727 290a 2020 2020  tFile}"''').    
-00014600: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-00014610: 7074 3a0a 2020 2020 2020 2020 2020 2020  pt:.            
-00014620: 2020 2020 2020 2020 7072 696e 7432 2822          print2("
-00014630: 4661 696c 6564 2074 6f20 7361 7665 2063  Failed to save c
-00014640: 6861 7421 5c6e 2229 0a20 2020 2020 2020  hat!\n").       
-00014650: 2020 2020 2020 2020 2020 2020 2073 686f               sho
-00014660: 7745 7272 6f72 7328 290a 0a20 2020 2064  wErrors()..    d
-00014670: 6566 2072 756e 496e 7374 7275 6374 696f  ef runInstructio
-00014680: 6e28 7365 6c66 293a 0a20 2020 2020 2020  n(self):.       
-00014690: 2069 6e73 7472 7563 7469 6f6e 7320 3d20   instructions = 
-000146a0: 6c69 7374 2863 6f6e 6669 672e 7072 6564  list(config.pred
-000146b0: 6566 696e 6564 496e 7374 7275 6374 696f  efinedInstructio
-000146c0: 6e73 2e6b 6579 7328 2929 0a20 2020 2020  ns.keys()).     
-000146d0: 2020 2069 6e73 7472 7563 7469 6f6e 203d     instruction =
-000146e0: 2073 656c 662e 6469 616c 6f67 732e 6765   self.dialogs.ge
-000146f0: 7456 616c 6964 4f70 7469 6f6e 7328 0a20  tValidOptions(. 
-00014700: 2020 2020 2020 2020 2020 206f 7074 696f             optio
-00014710: 6e73 3d69 6e73 7472 7563 7469 6f6e 732c  ns=instructions,
-00014720: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
-00014730: 6c65 3d22 5072 6564 6566 696e 6564 2049  le="Predefined I
-00014740: 6e73 7472 7563 7469 6f6e 7322 2c0a 2020  nstructions",.  
-00014750: 2020 2020 2020 2020 2020 7465 7874 3d22            text="
-00014760: 5365 6c65 6374 2061 6e20 696e 7374 7275  Select an instru
-00014770: 6374 696f 6e3a 222c 0a20 2020 2020 2020  ction:",.       
-00014780: 2029 0a20 2020 2020 2020 2069 6620 696e   ).        if in
-00014790: 7374 7275 6374 696f 6e3a 0a20 2020 2020  struction:.     
-000147a0: 2020 2020 2020 2063 6f6e 6669 672e 6465         config.de
-000147b0: 6661 756c 7445 6e74 7279 203d 2063 6f6e  faultEntry = con
-000147c0: 6669 672e 7072 6564 6566 696e 6564 496e  fig.predefinedIn
-000147d0: 7374 7275 6374 696f 6e73 5b69 6e73 7472  structions[instr
-000147e0: 7563 7469 6f6e 5d0a 2020 2020 2020 2020  uction].        
-000147f0: 2020 2020 636f 6e66 6967 2e61 6363 6570      config.accep
-00014800: 745f 6465 6661 756c 7420 3d20 5472 7565  t_default = True
-00014810: 0a0a 2020 2020 6465 6620 6368 616e 6765  ..    def change
-00014820: 436f 6e74 6578 7428 7365 6c66 293a 0a20  Context(self):. 
-00014830: 2020 2020 2020 2063 6f6e 7465 7874 7320         contexts 
-00014840: 3d20 6c69 7374 2863 6f6e 6669 672e 7072  = list(config.pr
-00014850: 6564 6566 696e 6564 436f 6e74 6578 7473  edefinedContexts
-00014860: 2e6b 6579 7328 2929 0a20 2020 2020 2020  .keys()).       
-00014870: 2070 7265 6465 6669 6e65 6443 6f6e 7465   predefinedConte
-00014880: 7874 203d 2073 656c 662e 6469 616c 6f67  xt = self.dialog
-00014890: 732e 6765 7456 616c 6964 4f70 7469 6f6e  s.getValidOption
-000148a0: 7328 0a20 2020 2020 2020 2020 2020 206f  s(.            o
-000148b0: 7074 696f 6e73 3d63 6f6e 7465 7874 732c  ptions=contexts,
-000148c0: 0a20 2020 2020 2020 2020 2020 2074 6974  .            tit
-000148d0: 6c65 3d22 5072 6564 6566 696e 6564 2043  le="Predefined C
-000148e0: 6f6e 7465 7874 7322 2c0a 2020 2020 2020  ontexts",.      
-000148f0: 2020 2020 2020 6465 6661 756c 743d 636f        default=co
-00014900: 6e66 6967 2e70 7265 6465 6669 6e65 6443  nfig.predefinedC
-00014910: 6f6e 7465 7874 2c0a 2020 2020 2020 2020  ontext,.        
-00014920: 2020 2020 7465 7874 3d22 5365 6c65 6374      text="Select
-00014930: 2061 2063 6f6e 7465 7874 3a22 2c0a 2020   a context:",.  
-00014940: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00014950: 6966 2070 7265 6465 6669 6e65 6443 6f6e  if predefinedCon
-00014960: 7465 7874 3a0a 2020 2020 2020 2020 2020  text:.          
-00014970: 2020 636f 6e66 6967 2e70 7265 6465 6669    config.predefi
-00014980: 6e65 6443 6f6e 7465 7874 203d 2070 7265  nedContext = pre
-00014990: 6465 6669 6e65 6443 6f6e 7465 7874 0a20  definedContext. 
-000149a0: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-000149b0: 6e66 6967 2e70 7265 6465 6669 6e65 6443  nfig.predefinedC
-000149c0: 6f6e 7465 7874 203d 3d20 225b 6375 7374  ontext == "[cust
-000149d0: 6f6d 5d22 3a0a 2020 2020 2020 2020 2020  om]":.          
-000149e0: 2020 2020 2020 7072 696e 7431 2822 4564        print1("Ed
-000149f0: 6974 2063 7573 746f 6d20 636f 6e74 6578  it custom contex
-00014a00: 7420 6265 6c6f 773a 2229 0a20 2020 2020  t below:").     
-00014a10: 2020 2020 2020 2020 2020 2063 7573 746f             custo
-00014a20: 6d43 6f6e 7465 7874 203d 2073 656c 662e  mContext = self.
-00014a30: 7072 6f6d 7074 732e 7369 6d70 6c65 5072  prompts.simplePr
-00014a40: 6f6d 7074 2873 7479 6c65 3d73 656c 662e  ompt(style=self.
-00014a50: 7072 6f6d 7074 732e 7072 6f6d 7074 5374  prompts.promptSt
-00014a60: 796c 6532 2c20 6465 6661 756c 743d 636f  yle2, default=co
-00014a70: 6e66 6967 2e63 7573 746f 6d50 7265 6465  nfig.customPrede
-00014a80: 6669 6e65 6443 6f6e 7465 7874 290a 2020  finedContext).  
-00014a90: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014aa0: 2063 7573 746f 6d43 6f6e 7465 7874 2061   customContext a
-00014ab0: 6e64 206e 6f74 2063 7573 746f 6d43 6f6e  nd not customCon
-00014ac0: 7465 7874 2e73 7472 6970 2829 2e6c 6f77  text.strip().low
-00014ad0: 6572 2829 203d 3d20 636f 6e66 6967 2e65  er() == config.e
-00014ae0: 7869 745f 656e 7472 793a 0a20 2020 2020  xit_entry:.     
-00014af0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00014b00: 6f6e 6669 672e 6375 7374 6f6d 5072 6564  onfig.customPred
-00014b10: 6566 696e 6564 436f 6e74 6578 7420 3d20  efinedContext = 
-00014b20: 6375 7374 6f6d 436f 6e74 6578 742e 7374  customContext.st
-00014b30: 7269 7028 290a 2020 2020 2020 2020 656c  rip().        el
-00014b40: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00014b50: 2320 6120 7761 7920 746f 2071 7569 636b  # a way to quick
-00014b60: 6c79 2063 6c65 616e 2075 7020 636f 6e74  ly clean up cont
-00014b70: 6578 740a 2020 2020 2020 2020 2020 2020  ext.            
-00014b80: 636f 6e66 6967 2e70 7265 6465 6669 6e65  config.predefine
-00014b90: 6443 6f6e 7465 7874 203d 2022 5b6e 6f6e  dContext = "[non
-00014ba0: 655d 220a 2020 2020 2020 2020 636f 6e66  e]".        conf
-00014bb0: 6967 2e73 6176 6543 6f6e 6669 6728 290a  ig.saveConfig().
-00014bc0: 2020 2020 2020 2020 7365 6c66 2e73 686f          self.sho
-00014bd0: 7743 7572 7265 6e74 436f 6e74 6578 7428  wCurrentContext(
-00014be0: 290a 0a20 2020 2064 6566 2067 6574 4469  )..    def getDi
-00014bf0: 7265 6374 6f72 794c 6973 7428 7365 6c66  rectoryList(self
-00014c00: 293a 0a20 2020 2020 2020 2064 6972 6563  ):.        direc
-00014c10: 746f 7279 4c69 7374 203d 205b 5d0a 2020  toryList = [].  
-00014c20: 2020 2020 2020 666f 7220 6620 696e 206f        for f in o
-00014c30: 732e 6c69 7374 6469 7228 272e 2729 3a0a  s.listdir('.'):.
-00014c40: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-00014c50: 732e 7061 7468 2e69 7364 6972 2866 293a  s.path.isdir(f):
-00014c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c70: 2073 6570 6172 6174 6f72 203d 2022 5c5c   separator = "\\
-00014c80: 2220 6966 2063 6f6e 6669 672e 7468 6973  " if config.this
-00014c90: 506c 6174 666f 726d 203d 3d20 2257 696e  Platform == "Win
-00014ca0: 646f 7773 2220 656c 7365 2022 2f22 0a20  dows" else "/". 
-00014cb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00014cc0: 6972 6563 746f 7279 4c69 7374 2e61 7070  irectoryList.app
-00014cd0: 656e 6428 6622 7b66 7d7b 7365 7061 7261  end(f"{f}{separa
-00014ce0: 746f 727d 2229 0a20 2020 2020 2020 2020  tor}").         
-00014cf0: 2020 2065 6c69 6620 6f73 2e70 6174 682e     elif os.path.
-00014d00: 6973 6669 6c65 2866 293a 0a20 2020 2020  isfile(f):.     
-00014d10: 2020 2020 2020 2020 2020 2064 6972 6563             direc
-00014d20: 746f 7279 4c69 7374 2e61 7070 656e 6428  toryList.append(
-00014d30: 6629 0a20 2020 2020 2020 2072 6574 7572  f).        retur
-00014d40: 6e20 6469 7265 6374 6f72 794c 6973 740a  n directoryList.
-00014d50: 0a20 2020 2064 6566 2073 686f 774c 6f67  .    def showLog
-00014d60: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
-00014d70: 2061 7070 4e61 6d65 203d 2063 6f6e 6669   appName = confi
-00014d80: 672e 6672 6565 4765 6e69 7573 4149 4e61  g.freeGeniusAINa
-00014d90: 6d65 2e73 706c 6974 2829 5b30 5d2e 7570  me.split()[0].up
-00014da0: 7065 7228 290a 2020 2020 2020 2020 7465  per().        te
-00014db0: 726d 696e 616c 5f77 6964 7468 203d 2073  rminal_width = s
-00014dc0: 6875 7469 6c2e 6765 745f 7465 726d 696e  hutil.get_termin
-00014dd0: 616c 5f73 697a 6528 292e 636f 6c75 6d6e  al_size().column
-00014de0: 730a 2020 2020 2020 2020 7472 793a 0a20  s.        try:. 
-00014df0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-00014e00: 6172 7420 696d 706f 7274 2074 6578 7432  art import text2
-00014e10: 6172 740a 2020 2020 2020 2020 2020 2020  art.            
-00014e20: 6966 2074 6572 6d69 6e61 6c5f 7769 6474  if terminal_widt
-00014e30: 6820 3e3d 2033 323a 0a20 2020 2020 2020  h >= 32:.       
-00014e40: 2020 2020 2020 2020 206c 6f67 6f20 3d20           logo = 
-00014e50: 7465 7874 3261 7274 2861 7070 4e61 6d65  text2art(appName
-00014e60: 2c20 666f 6e74 3d22 6379 6265 726d 6564  , font="cybermed
-00014e70: 756d 2229 0a20 2020 2020 2020 2020 2020  um").           
-00014e80: 2065 6c69 6620 7465 726d 696e 616c 5f77   elif terminal_w
-00014e90: 6964 7468 203e 3d20 3230 3a0a 2020 2020  idth >= 20:.    
-00014ea0: 2020 2020 2020 2020 2020 2020 6c6f 676f              logo
-00014eb0: 203d 2074 6578 7432 6172 7428 2220 222e   = text2art(" ".
-00014ec0: 6a6f 696e 2861 7070 4e61 6d65 2920 2b20  join(appName) + 
-00014ed0: 2220 222c 2066 6f6e 743d 2277 6869 7465  " ", font="white
-00014ee0: 5f62 7562 626c 6522 290a 2020 2020 2020  _bubble").      
-00014ef0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00014f00: 2020 2020 2020 2020 2020 2020 6c6f 676f              logo
-00014f10: 203d 2063 6f6e 6669 672e 6672 6565 4765   = config.freeGe
-00014f20: 6e69 7573 4149 4e61 6d65 0a20 2020 2020  niusAIName.     
-00014f30: 2020 2020 2020 206c 6f67 6f20 3d20 6c6f         logo = lo
-00014f40: 676f 5b3a 2d31 5d20 2320 7265 6d6f 7665  go[:-1] # remove
-00014f50: 2074 6865 206c 696e 6562 7265 616b 2061   the linebreak a
-00014f60: 7420 7468 6520 656e 640a 2020 2020 2020  t the end.      
-00014f70: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
-00014f80: 2020 2020 2020 6c6f 676f 203d 2063 6f6e        logo = con
-00014f90: 6669 672e 6672 6565 4765 6e69 7573 4149  fig.freeGeniusAI
-00014fa0: 4e61 6d65 0a20 2020 2020 2020 2070 7269  Name.        pri
-00014fb0: 6e74 5f66 6f72 6d61 7474 6564 5f74 6578  nt_formatted_tex
-00014fc0: 7428 4854 4d4c 2866 223c 7b63 6f6e 6669  t(HTML(f"<{confi
-00014fd0: 672e 7465 726d 696e 616c 436f 6d6d 616e  g.terminalComman
-00014fe0: 6445 6e74 7279 436f 6c6f 7232 7d3e 7b6c  dEntryColor2}>{l
-00014ff0: 6f67 6f7d 3c2f 7b63 6f6e 6669 672e 7465  ogo}</{config.te
-00015000: 726d 696e 616c 436f 6d6d 616e 6445 6e74  rminalCommandEnt
-00015010: 7279 436f 6c6f 7232 7d3e 2229 290a 0a20  ryColor2}>")).. 
-00015020: 2020 2064 6566 2072 756e 5079 7468 6f6e     def runPython
-00015030: 5363 7269 7074 2873 656c 662c 2073 6372  Script(self, scr
-00015040: 6970 7429 3a0a 2020 2020 2020 2020 7363  ipt):.        sc
-00015050: 7269 7074 203d 2073 6372 6970 742e 7374  ript = script.st
-00015060: 7269 7028 295b 333a 2d33 5d0a 2020 2020  rip()[3:-3].    
-00015070: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00015080: 2020 2020 2065 7865 6328 7363 7269 7074       exec(script
-00015090: 2c20 676c 6f62 616c 7328 2929 0a20 2020  , globals()).   
-000150a0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-000150b0: 2020 2020 2020 2020 2074 7261 6365 203d           trace =
-000150c0: 2074 7261 6365 6261 636b 2e66 6f72 6d61   traceback.forma
-000150d0: 745f 6578 6328 290a 2020 2020 2020 2020  t_exc().        
-000150e0: 2020 2020 7072 696e 7428 7472 6163 6520      print(trace 
-000150f0: 6966 2063 6f6e 6669 672e 6465 7665 6c6f  if config.develo
-00015100: 7065 7220 656c 7365 2022 4572 726f 7220  per else "Error 
-00015110: 656e 636f 756e 7465 7265 6421 2229 0a20  encountered!"). 
-00015120: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00015130: 3128 636f 6e66 6967 2e64 6976 6964 6572  1(config.divider
-00015140: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-00015150: 2063 6f6e 6669 672e 6d61 785f 636f 6e73   config.max_cons
-00015160: 6563 7574 6976 655f 6175 746f 5f63 6f72  ecutive_auto_cor
-00015170: 7265 6374 696f 6e20 3e20 303a 0a20 2020  rection > 0:.   
-00015180: 2020 2020 2020 2020 2020 2020 2043 616c               Cal
-00015190: 6c4c 4c4d 2e61 7574 6f43 6f72 7265 6374  lLLM.autoCorrect
-000151a0: 5079 7468 6f6e 436f 6465 2873 6372 6970  PythonCode(scrip
-000151b0: 742c 2074 7261 6365 290a 0a20 2020 2064  t, trace)..    d
-000151c0: 6566 2073 7461 7274 4368 6174 7328 7365  ef startChats(se
-000151d0: 6c66 293a 0a20 2020 2020 2020 2074 6f6b  lf):.        tok
-000151e0: 656e 5661 6c69 6461 746f 7220 3d20 546f  enValidator = To
-000151f0: 6b65 6e56 616c 6964 6174 6f72 2829 0a20  kenValidator(). 
-00015200: 2020 2020 2020 2064 6566 2067 6574 4479         def getDy
-00015210: 6e61 6d69 6354 6f6f 6c42 6172 2829 3a0a  namicToolBar():.
-00015220: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015230: 726e 2063 6f6e 6669 672e 6479 6e61 6d69  rn config.dynami
-00015240: 6354 6f6f 6c42 6172 5465 7874 0a20 2020  cToolBarText.   
-00015250: 2020 2020 2064 6566 2073 7461 7274 4368       def startCh
-00015260: 6174 2829 3a0a 2020 2020 2020 2020 2020  at():.          
-00015270: 2020 636c 6561 7228 290a 2020 2020 2020    clear().      
-00015280: 2020 2020 2020 7072 696e 7431 2873 656c        print1(sel
-00015290: 662e 6469 7669 6465 7229 0a20 2020 2020  f.divider).     
-000152a0: 2020 2020 2020 2073 656c 662e 7368 6f77         self.show
-000152b0: 4c6f 676f 2829 0a20 2020 2020 2020 2020  Logo().         
-000152c0: 2020 2073 656c 662e 7368 6f77 4375 7272     self.showCurr
-000152d0: 656e 7443 6f6e 7465 7874 2829 0a20 2020  entContext().   
-000152e0: 2020 2020 2020 2020 2023 2067 6f20 746f           # go to
-000152f0: 2073 7461 7274 7570 2064 6972 6563 746f   startup directo
-00015300: 7279 0a20 2020 2020 2020 2020 2020 2073  ry.            s
-00015310: 746f 7261 6765 6469 7265 6374 6f72 7920  toragedirectory 
-00015320: 3d20 636f 6e66 6967 2e6c 6f63 616c 5374  = config.localSt
-00015330: 6f72 6167 650a 2020 2020 2020 2020 2020  orage.          
-00015340: 2020 6f73 2e63 6864 6972 2873 746f 7261    os.chdir(stora
-00015350: 6765 6469 7265 6374 6f72 7929 0a20 2020  gedirectory).   
-00015360: 2020 2020 2020 2020 206d 6573 7361 6765           message
-00015370: 7320 3d20 4361 6c6c 4c4c 4d2e 7265 7365  s = CallLLM.rese
-00015380: 744d 6573 7361 6765 7328 290a 2020 2020  tMessages().    
-00015390: 2020 2020 2020 2020 2370 7269 6e74 3128          #print1(
-000153a0: 6622 7374 6172 7475 7020 6469 7265 6374  f"startup direct
-000153b0: 6f72 793a 5c6e 7b73 746f 7261 6765 6469  ory:\n{storagedi
-000153c0: 7265 6374 6f72 797d 2229 0a20 2020 2020  rectory}").     
-000153d0: 2020 2020 2020 2070 7269 6e74 5f66 6f72         print_for
-000153e0: 6d61 7474 6564 5f74 6578 7428 4854 4d4c  matted_text(HTML
-000153f0: 2866 223c 7b63 6f6e 6669 672e 7465 726d  (f"<{config.term
-00015400: 696e 616c 5072 6f6d 7074 496e 6469 6361  inalPromptIndica
-00015410: 746f 7243 6f6c 6f72 327d 3e44 6972 6563  torColor2}>Direc
-00015420: 746f 7279 3a3c 2f7b 636f 6e66 6967 2e74  tory:</{config.t
-00015430: 6572 6d69 6e61 6c50 726f 6d70 7449 6e64  erminalPromptInd
-00015440: 6963 6174 6f72 436f 6c6f 7232 7d3e 207b  icatorColor2}> {
-00015450: 7374 6f72 6167 6564 6972 6563 746f 7279  storagedirectory
-00015460: 7d22 2929 0a20 2020 2020 2020 2020 2020  }")).           
-00015470: 2070 7269 6e74 3128 7365 6c66 2e64 6976   print1(self.div
-00015480: 6964 6572 290a 0a20 2020 2020 2020 2020  ider)..         
-00015490: 2020 2063 6f6e 6669 672e 636f 6e76 6572     config.conver
-000154a0: 7361 7469 6f6e 5374 6172 7465 6420 3d20  sationStarted = 
-000154b0: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-000154c0: 2020 7265 7475 726e 2028 7374 6f72 6167    return (storag
-000154d0: 6564 6972 6563 746f 7279 2c20 6d65 7373  edirectory, mess
-000154e0: 6167 6573 290a 2020 2020 2020 2020 7374  ages).        st
-000154f0: 6f72 6167 6564 6972 6563 746f 7279 2c20  oragedirectory, 
-00015500: 636f 6e66 6967 2e63 7572 7265 6e74 4d65  config.currentMe
-00015510: 7373 6167 6573 203d 2073 7461 7274 4368  ssages = startCh
-00015520: 6174 2829 0a20 2020 2020 2020 2063 6f6e  at().        con
-00015530: 6669 672e 6d75 6c74 696c 696e 6549 6e70  fig.multilineInp
-00015540: 7574 203d 2046 616c 7365 0a20 2020 2020  ut = False.     
-00015550: 2020 2066 6561 7475 7265 734c 6f77 6572     featuresLower
-00015560: 203d 206c 6973 7428 7365 6c66 2e61 6374   = list(self.act
-00015570: 696f 6e73 2e6b 6579 7328 2929 202b 205b  ions.keys()) + [
-00015580: 222e 2e2e 225d 0a20 2020 2020 2020 2023  "..."].        #
-00015590: 2069 6e70 7574 2073 7567 6765 7374 696f   input suggestio
-000155a0: 6e73 0a20 2020 2020 2020 2063 6f6e 6669  ns.        confi
-000155b0: 672e 696e 7075 7453 7567 6765 7374 696f  g.inputSuggestio
-000155c0: 6e73 202b 3d20 6665 6174 7572 6573 4c6f  ns += featuresLo
-000155d0: 7765 720a 2020 2020 2020 2020 636f 6d70  wer.        comp
-000155e0: 6c65 7465 7220 3d20 4675 7a7a 7943 6f6d  leter = FuzzyCom
-000155f0: 706c 6574 6572 2857 6f72 6443 6f6d 706c  pleter(WordCompl
-00015600: 6574 6572 2863 6f6e 6669 672e 696e 7075  eter(config.inpu
-00015610: 7453 7567 6765 7374 696f 6e73 2c20 6967  tSuggestions, ig
-00015620: 6e6f 7265 5f63 6173 653d 5472 7565 2929  nore_case=True))
-00015630: 2069 6620 636f 6e66 6967 2e69 6e70 7574   if config.input
-00015640: 5375 6767 6573 7469 6f6e 7320 656c 7365  Suggestions else
-00015650: 204e 6f6e 650a 2020 2020 2020 2020 636f   None.        co
-00015660: 6d70 6c65 7465 725f 6465 7665 6c6f 7065  mpleter_develope
-00015670: 7220 3d20 4675 7a7a 7943 6f6d 706c 6574  r = FuzzyComplet
-00015680: 6572 2857 6f72 6443 6f6d 706c 6574 6572  er(WordCompleter
-00015690: 2863 6f6e 6669 672e 696e 7075 7453 7567  (config.inputSug
-000156a0: 6765 7374 696f 6e73 5b3a 5d20 2b20 5b66  gestions[:] + [f
-000156b0: 2263 6f6e 6669 672e 7b69 7d22 2066 6f72  "config.{i}" for
-000156c0: 2069 2069 6e20 6469 7228 636f 6e66 6967   i in dir(config
-000156d0: 2920 6966 206e 6f74 2069 2e73 7461 7274  ) if not i.start
-000156e0: 7377 6974 6828 225f 5f22 295d 202b 2073  swith("__")] + s
-000156f0: 656c 662e 6765 7444 6972 6563 746f 7279  elf.getDirectory
-00015700: 4c69 7374 2829 2c20 6967 6e6f 7265 5f63  List(), ignore_c
-00015710: 6173 653d 5472 7565 2929 0a20 2020 2020  ase=True)).     
-00015720: 2020 2077 6869 6c65 2054 7275 653a 0a20     while True:. 
-00015730: 2020 2020 2020 2020 2020 2023 2064 6566             # def
-00015740: 6175 6c74 2074 6f6f 6c62 6172 2074 6578  ault toolbar tex
-00015750: 740a 2020 2020 2020 2020 2020 2020 636f  t.            co
-00015760: 6e66 6967 2e64 796e 616d 6963 546f 6f6c  nfig.dynamicTool
-00015770: 4261 7254 6578 7420 3d20 6622 2222 207b  BarText = f""" {
-00015780: 7374 7228 636f 6e66 6967 2e68 6f74 6b65  str(config.hotke
-00015790: 795f 6578 6974 292e 7265 706c 6163 6528  y_exit).replace(
-000157a0: 2227 222c 2022 2229 7d20 6578 6974 207b  "'", "")} exit {
-000157b0: 7374 7228 636f 6e66 6967 2e68 6f74 6b65  str(config.hotke
-000157c0: 795f 6469 7370 6c61 795f 6b65 795f 636f  y_display_key_co
-000157d0: 6d62 6f29 2e72 6570 6c61 6365 2822 2722  mbo).replace("'"
-000157e0: 2c20 2222 297d 2073 686f 7274 6375 7473  , "")} shortcuts
-000157f0: 2022 2222 0a20 2020 2020 2020 2020 2020   """.           
-00015800: 2023 2064 6973 706c 6179 2063 7572 7265   # display curre
-00015810: 6e74 2064 6972 6563 746f 7279 2069 6620  nt directory if 
-00015820: 6368 616e 6765 640a 2020 2020 2020 2020  changed.        
-00015830: 2020 2020 6375 7272 656e 7444 6972 6563      currentDirec
-00015840: 746f 7279 203d 206f 732e 6765 7463 7764  tory = os.getcwd
-00015850: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
-00015860: 6620 6e6f 7420 6375 7272 656e 7444 6972  f not currentDir
-00015870: 6563 746f 7279 203d 3d20 7374 6f72 6167  ectory == storag
-00015880: 6564 6972 6563 746f 7279 3a0a 2020 2020  edirectory:.    
-00015890: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
-000158a0: 6e74 3128 7365 6c66 2e64 6976 6964 6572  nt1(self.divider
-000158b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000158c0: 2020 7072 696e 7433 2866 2243 7572 7265    print3(f"Curre
-000158d0: 6e74 2064 6972 6563 746f 7279 3a20 7b63  nt directory: {c
-000158e0: 7572 7265 6e74 4469 7265 6374 6f72 797d  urrentDirectory}
-000158f0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00015900: 2020 2070 7269 6e74 3128 7365 6c66 2e64     print1(self.d
-00015910: 6976 6964 6572 290a 2020 2020 2020 2020  ivider).        
-00015920: 2020 2020 2020 2020 7374 6f72 6167 6564          storaged
-00015930: 6972 6563 746f 7279 203d 2063 7572 7265  irectory = curre
-00015940: 6e74 4469 7265 6374 6f72 790a 2020 2020  ntDirectory.    
-00015950: 2020 2020 2020 2020 2320 6465 6661 756c          # defaul
-00015960: 7420 696e 7075 7420 656e 7472 790a 2020  t input entry.  
-00015970: 2020 2020 2020 2020 2020 6163 6365 7074            accept
-00015980: 5f64 6566 6175 6c74 203d 2063 6f6e 6669  _default = confi
-00015990: 672e 6163 6365 7074 5f64 6566 6175 6c74  g.accept_default
-000159a0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
-000159b0: 6669 672e 6163 6365 7074 5f64 6566 6175  fig.accept_defau
-000159c0: 6c74 203d 2046 616c 7365 0a20 2020 2020  lt = False.     
-000159d0: 2020 2020 2020 2064 6566 6175 6c74 456e         defaultEn
-000159e0: 7472 7920 3d20 636f 6e66 6967 2e64 6566  try = config.def
-000159f0: 6175 6c74 456e 7472 790a 2020 2020 2020  aultEntry.      
-00015a00: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-00015a10: 2e69 7366 696c 6528 6465 6661 756c 7445  .isfile(defaultE
-00015a20: 6e74 7279 293a 0a20 2020 2020 2020 2020  ntry):.         
-00015a30: 2020 2020 2020 2064 6566 6175 6c74 456e         defaultEn
-00015a40: 7472 7920 3d20 6627 4669 6c65 3a20 227b  try = f'File: "{
-00015a50: 6465 6661 756c 7445 6e74 7279 7d22 5c6e  defaultEntry}"\n
-00015a60: 270a 2020 2020 2020 2020 2020 2020 656c  '.            el
-00015a70: 6966 206f 732e 7061 7468 2e69 7364 6972  if os.path.isdir
-00015a80: 2864 6566 6175 6c74 456e 7472 7929 3a0a  (defaultEntry):.
-00015a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015aa0: 6465 6661 756c 7445 6e74 7279 203d 2066  defaultEntry = f
-00015ab0: 2746 6f6c 6465 723a 2022 7b64 6566 6175  'Folder: "{defau
-00015ac0: 6c74 456e 7472 797d 225c 6e27 0a20 2020  ltEntry}"\n'.   
-00015ad0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-00015ae0: 6465 6661 756c 7445 6e74 7279 203d 2022  defaultEntry = "
-00015af0: 220a 0a20 2020 2020 2020 2020 2020 2023  "..            #
-00015b00: 2075 7365 7220 696e 7075 740a 2020 2020   user input.    
-00015b10: 2020 2020 2020 2020 7573 6572 496e 7075          userInpu
-00015b20: 7420 3d20 7365 6c66 2e70 726f 6d70 7473  t = self.prompts
-00015b30: 2e73 696d 706c 6550 726f 6d70 7428 7072  .simplePrompt(pr
-00015b40: 6f6d 7074 5365 7373 696f 6e3d 7365 6c66  omptSession=self
-00015b50: 2e74 6572 6d69 6e61 6c5f 6368 6174 5f73  .terminal_chat_s
-00015b60: 6573 7369 6f6e 2c20 636f 6d70 6c65 7465  ession, complete
-00015b70: 723d 636f 6d70 6c65 7465 725f 6465 7665  r=completer_deve
-00015b80: 6c6f 7065 7220 6966 2063 6f6e 6669 672e  loper if config.
-00015b90: 6465 7665 6c6f 7065 7220 656c 7365 2063  developer else c
-00015ba0: 6f6d 706c 6574 6572 2c20 6465 6661 756c  ompleter, defaul
-00015bb0: 743d 6465 6661 756c 7445 6e74 7279 2c20  t=defaultEntry, 
-00015bc0: 6163 6365 7074 5f64 6566 6175 6c74 3d61  accept_default=a
-00015bd0: 6363 6570 745f 6465 6661 756c 742c 2076  ccept_default, v
-00015be0: 616c 6964 6174 6f72 3d74 6f6b 656e 5661  alidator=tokenVa
-00015bf0: 6c69 6461 746f 722c 2062 6f74 746f 6d5f  lidator, bottom_
-00015c00: 746f 6f6c 6261 723d 6765 7444 796e 616d  toolbar=getDynam
-00015c10: 6963 546f 6f6c 4261 7229 0a20 2020 2020  icToolBar).     
-00015c20: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00015c30: 2020 2020 2320 7570 6461 7465 2073 7973      # update sys
-00015c40: 7465 6d20 6d65 7373 6167 6520 7768 656e  tem message when
-00015c50: 2075 7365 7220 656e 7465 7220 6120 6e65   user enter a ne
-00015c60: 7720 696e 7075 740a 2020 2020 2020 2020  w input.        
-00015c70: 2020 2020 636f 6e66 6967 2e63 7572 7265      config.curre
-00015c80: 6e74 4d65 7373 6167 6573 203d 2073 656c  ntMessages = sel
-00015c90: 662e 7570 6461 7465 5379 7374 656d 4d65  f.updateSystemMe
-00015ca0: 7373 6167 6528 636f 6e66 6967 2e63 7572  ssage(config.cur
-00015cb0: 7265 6e74 4d65 7373 6167 6573 290a 2020  rentMessages).  
-00015cc0: 2020 2020 2020 2020 2020 0a20 2020 2020            .     
-00015cd0: 2020 2020 2020 2023 2064 6973 706c 6179         # display
-00015ce0: 206f 7074 696f 6e73 2077 6865 6e20 656d   options when em
-00015cf0: 7074 7920 7374 7269 6e67 2069 7320 656e  pty string is en
-00015d00: 7465 7265 640a 2020 2020 2020 2020 2020  tered.          
-00015d10: 2020 7573 6572 496e 7075 744c 6f77 6572    userInputLower
-00015d20: 203d 2075 7365 7249 6e70 7574 2e6c 6f77   = userInput.low
-00015d30: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
-00015d40: 2069 6620 636f 6e66 6967 2e61 6464 5061   if config.addPa
-00015d50: 7468 4174 2069 7320 6e6f 7420 4e6f 6e65  thAt is not None
-00015d60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00015d70: 2020 7072 6566 6978 203d 2075 7365 7249    prefix = userI
-00015d80: 6e70 7574 5b3a 636f 6e66 6967 2e61 6464  nput[:config.add
-00015d90: 5061 7468 4174 5d0a 2020 2020 2020 2020  PathAt].        
-00015da0: 2020 2020 2020 2020 7072 6566 6978 5370          prefixSp
-00015db0: 6c69 7420 3d20 7072 6566 6978 2e72 7370  lit = prefix.rsp
-00015dc0: 6c69 7428 2220 222c 2031 290a 2020 2020  lit(" ", 1).    
-00015dd0: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-00015de0: 656e 2870 7265 6669 7853 706c 6974 2920  en(prefixSplit) 
-00015df0: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
-00015e00: 2020 2020 2020 2020 2064 6566 6175 6c74           default
-00015e10: 203d 2070 7265 6669 7853 706c 6974 5b2d   = prefixSplit[-
-00015e20: 315d 0a20 2020 2020 2020 2020 2020 2020  1].             
-00015e30: 2020 2020 2020 2070 7265 6669 7820 3d20         prefix = 
-00015e40: 6622 7b70 7265 6669 7853 706c 6974 5b30  f"{prefixSplit[0
-00015e50: 5d7d 2022 0a20 2020 2020 2020 2020 2020  ]} ".           
-00015e60: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00015e70: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00015e80: 6566 6175 6c74 203d 2070 7265 6669 780a  efault = prefix.
-00015e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ea0: 2020 2020 7072 6566 6978 203d 2022 220a      prefix = "".
-00015eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015ec0: 7375 6666 6978 203d 2075 7365 7249 6e70  suffix = userInp
-00015ed0: 7574 5b63 6f6e 6669 672e 6164 6450 6174  ut[config.addPat
-00015ee0: 6841 743a 5d0a 2020 2020 2020 2020 2020  hAt:].          
-00015ef0: 2020 2020 2020 636f 6e66 6967 2e61 6464        config.add
-00015f00: 5061 7468 4174 203d 204e 6f6e 650a 2020  PathAt = None.  
-00015f10: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00015f20: 206e 6f74 2064 6566 6175 6c74 3a0a 2020   not default:.  
-00015f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f40: 2020 6465 6661 756c 7420 3d20 6f73 2e67    default = os.g
-00015f50: 6574 6377 6428 290a 2020 2020 2020 2020  etcwd().        
-00015f60: 2020 2020 2020 2020 7573 6572 5061 7468          userPath
-00015f70: 203d 2073 656c 662e 6765 7450 6174 682e   = self.getPath.
-00015f80: 6765 7450 6174 6828 6d65 7373 6167 653d  getPath(message=
-00015f90: 6622 7b70 7265 6669 787d 3c7b 636f 6e66  f"{prefix}<{conf
-00015fa0: 6967 2e74 6572 6d69 6e61 6c43 6f6d 6d61  ig.terminalComma
-00015fb0: 6e64 456e 7472 7943 6f6c 6f72 327d 3e5b  ndEntryColor2}>[
-00015fc0: 6164 6420 6120 7061 7468 2068 6572 655d  add a path here]
-00015fd0: 3c2f 7b63 6f6e 6669 672e 7465 726d 696e  </{config.termin
-00015fe0: 616c 436f 6d6d 616e 6445 6e74 7279 436f  alCommandEntryCo
-00015ff0: 6c6f 7232 7d3e 7b73 7566 6669 787d 222c  lor2}>{suffix}",
-00016000: 2070 726f 6d70 7449 6e64 6963 6174 6f72   promptIndicator
-00016010: 3d22 3e3e 3e20 222c 2065 6d70 7479 5f74  =">>> ", empty_t
-00016020: 6f5f 6361 6e63 656c 3d54 7275 652c 2064  o_cancel=True, d
-00016030: 6566 6175 6c74 3d64 6566 6175 6c74 290a  efault=default).
-00016040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016050: 636f 6e66 6967 2e64 6566 6175 6c74 456e  config.defaultEn
-00016060: 7472 7920 3d20 6622 7b70 7265 6669 787d  try = f"{prefix}
-00016070: 7b75 7365 7250 6174 687d 7b73 7566 6669  {userPath}{suffi
-00016080: 787d 220a 2020 2020 2020 2020 2020 2020  x}".            
-00016090: 2020 2020 7573 6572 496e 7075 7420 3d20      userInput = 
-000160a0: 2222 0a20 2020 2020 2020 2020 2020 2065  "".            e
-000160b0: 6c69 6620 6e6f 7420 7573 6572 496e 7075  lif not userInpu
-000160c0: 744c 6f77 6572 3a0a 2020 2020 2020 2020  tLower:.        
-000160d0: 2020 2020 2020 2020 7573 6572 496e 7075          userInpu
-000160e0: 7420 3d20 636f 6e66 6967 2e62 6c61 6e6b  t = config.blank
-000160f0: 456e 7472 7941 6374 696f 6e0a 2020 2020  EntryAction.    
-00016100: 2020 2020 2020 2020 6966 2075 7365 7249          if userI
-00016110: 6e70 7574 203d 3d20 222e 2e2e 223a 0a20  nput == "...":. 
-00016120: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00016130: 7365 7249 6e70 7574 203d 2075 7365 7249  serInput = userI
-00016140: 6e70 7574 4c6f 7765 7220 3d20 7365 6c66  nputLower = self
-00016150: 2e72 756e 4163 7469 6f6e 7328 7573 6572  .runActions(user
-00016160: 496e 7075 7429 0a20 2020 2020 2020 2020  Input).         
-00016170: 2020 2023 656c 6966 2075 7365 7249 6e70     #elif userInp
-00016180: 7574 4c6f 7765 7220 696e 2074 7570 6c65  utLower in tuple
-00016190: 2873 656c 662e 6163 7469 6f6e 732e 6b65  (self.actions.ke
-000161a0: 7973 2829 293a 0a20 2020 2020 2020 2020  ys()):.         
-000161b0: 2020 2065 6c69 6620 7573 6572 496e 7075     elif userInpu
-000161c0: 744c 6f77 6572 2e73 7461 7274 7377 6974  tLower.startswit
-000161d0: 6828 222e 2229 2061 6e64 206e 6f74 2075  h(".") and not u
-000161e0: 7365 7249 6e70 7574 4c6f 7765 7220 696e  serInputLower in
-000161f0: 2028 636f 6e66 6967 2e65 7869 745f 656e   (config.exit_en
-00016200: 7472 792c 2063 6f6e 6669 672e 6361 6e63  try, config.canc
-00016210: 656c 5f65 6e74 7279 2c20 222e 6e65 7722  el_entry, ".new"
-00016220: 2c20 222e 636f 6e74 6578 7422 293a 0a20  , ".context"):. 
-00016230: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00016240: 7365 7249 6e70 7574 203d 2075 7365 7249  serInput = userI
-00016250: 6e70 7574 4c6f 7765 7220 3d20 7365 6c66  nputLower = self
-00016260: 2e72 756e 4163 7469 6f6e 7328 222e 2e2e  .runActions("...
-00016270: 222c 2075 7365 7249 6e70 7574 290a 0a20  ", userInput).. 
-00016280: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-00016290: 7454 6f6f 6c44 6570 656e 6465 6e63 6528  tToolDependence(
-000162a0: 7573 6572 496e 7075 7429 3a0a 2020 2020  userInput):.    
-000162b0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-000162c0: 696e 7565 0a0a 2020 2020 2020 2020 2020  inue..          
-000162d0: 2020 2320 7265 706c 6163 6520 616c 6961    # replace alia
-000162e0: 732c 2069 6620 616e 792c 2077 6974 6820  s, if any, with 
-000162f0: 6675 6c6c 2065 6e74 7279 0a20 2020 2020  full entry.     
-00016300: 2020 2020 2020 2066 6f72 2061 6c69 6173         for alias
-00016310: 2c20 6675 6c6c 456e 7472 7920 696e 2063  , fullEntry in c
-00016320: 6f6e 6669 672e 616c 6961 7365 732e 6974  onfig.aliases.it
-00016330: 656d 7328 293a 0a20 2020 2020 2020 2020  ems():.         
-00016340: 2020 2020 2020 2023 7573 6572 496e 7075         #userInpu
-00016350: 7420 3d20 7265 2e73 7562 2861 6c69 6173  t = re.sub(alias
-00016360: 2c20 6675 6c6c 456e 7472 792c 2075 7365  , fullEntry, use
-00016370: 7249 6e70 7574 2920 2320 6572 726f 7220  rInput) # error 
-00016380: 6f6e 2057 696e 646f 7773 2063 6f7a 206f  on Windows coz o
-00016390: 6620 5769 6e64 6f77 7320 7061 7468 0a20  f Windows path. 
-000163a0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-000163b0: 7365 7249 6e70 7574 203d 2075 7365 7249  serInput = userI
-000163c0: 6e70 7574 2e72 6570 6c61 6365 2861 6c69  nput.replace(ali
-000163d0: 6173 2c20 6675 6c6c 456e 7472 7929 0a0a  as, fullEntry)..
-000163e0: 2020 2020 2020 2020 2020 2020 2320 6f70              # op
-000163f0: 656e 2066 696c 6520 2f20 6469 7265 6374  en file / direct
-00016400: 6f72 7920 6469 7265 6374 6c79 0a20 2020  ory directly.   
-00016410: 2020 2020 2020 2020 2064 6f63 735f 7061           docs_pa
-00016420: 7468 203d 2069 7345 7869 7374 696e 6750  th = isExistingP
-00016430: 6174 6828 7573 6572 496e 7075 7429 0a20  ath(userInput). 
-00016440: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
-00016450: 2e70 6174 682e 6973 6669 6c65 2864 6f63  .path.isfile(doc
-00016460: 735f 7061 7468 293a 0a20 2020 2020 2020  s_path):.       
-00016470: 2020 2020 2020 2020 206f 732e 7379 7374           os.syst
-00016480: 656d 2866 227b 636f 6e66 6967 2e6f 7065  em(f"{config.ope
-00016490: 6e7d 207b 646f 6373 5f70 6174 687d 2229  n} {docs_path}")
-000164a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000164b0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-000164c0: 2020 2020 2020 656c 6966 206f 732e 7061        elif os.pa
-000164d0: 7468 2e69 7364 6972 2864 6f63 735f 7061  th.isdir(docs_pa
-000164e0: 7468 293a 0a20 2020 2020 2020 2020 2020  th):.           
-000164f0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00016500: 2020 2020 2020 2020 2020 2020 2020 6f73                os
-00016510: 2e63 6864 6972 2864 6f63 735f 7061 7468  .chdir(docs_path
-00016520: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016530: 2020 2020 2020 7072 696e 7433 2866 2244        print3(f"D
-00016540: 6972 6563 746f 7279 2063 6861 6e67 6564  irectory changed
-00016550: 2074 6f3a 207b 646f 6373 5f70 6174 687d   to: {docs_path}
-00016560: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-00016570: 2020 2020 2020 2073 656c 662e 6765 7450         self.getP
-00016580: 6174 682e 6469 7370 6c61 7944 6972 6563  ath.displayDirec
-00016590: 746f 7279 436f 6e74 656e 7428 290a 2020  toryContent().  
-000165a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000165b0: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
-000165c0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-000165d0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000165e0: 2020 2020 2020 2070 6173 730a 0a20 2020         pass..   
-000165f0: 2020 2020 2020 2020 2023 2074 7279 2065           # try e
-00016600: 7661 6c0a 2020 2020 2020 2020 2020 2020  val.            
-00016610: 6966 2063 6f6e 6669 672e 6465 7665 6c6f  if config.develo
-00016620: 7065 7220 616e 6420 6e6f 7420 7573 6572  per and not user
-00016630: 496e 7075 7420 3d3d 2022 2e2e 2e22 3a0a  Input == "...":.
-00016640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016650: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00016660: 2020 2020 2020 2020 2076 616c 7565 203d           value =
-00016670: 2065 7661 6c28 7573 6572 496e 7075 7429   eval(userInput)
-00016680: 2023 2069 7420 736f 6c76 6520 7369 6d70   # it solve simp
-00016690: 6c65 206d 6174 682c 2065 2e67 2e20 312b  le math, e.g. 1+
-000166a0: 312c 206f 7220 7265 6164 2076 6172 6961  1, or read varia
-000166b0: 626c 6573 2c20 652e 672e 2064 6972 2863  bles, e.g. dir(c
-000166c0: 6f6e 6669 6729 0a20 2020 2020 2020 2020  onfig).         
-000166d0: 2020 2020 2020 2020 2020 2069 6620 7661             if va
-000166e0: 6c75 6520 6973 206e 6f74 204e 6f6e 653a  lue is not None:
-000166f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016700: 2020 2020 2020 2020 2023 7072 696e 7428           #print(
-00016710: 7661 6c75 6529 0a20 2020 2020 2020 2020  value).         
-00016720: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00016730: 7072 696e 742e 7070 7269 6e74 2876 616c  print.pprint(val
-00016740: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-00016750: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00016760: 7428 2222 290a 2020 2020 2020 2020 2020  t("").          
-00016770: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00016780: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-00016790: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-000167a0: 7265 2e73 6561 7263 6828 225e 7072 696e  re.search("^prin
-000167b0: 745c 285b 5e5c 295c 295d 2b3f 5c29 2422  t\([^\)\)]+?\)$"
-000167c0: 2c20 7573 6572 496e 7075 7429 3a0a 2020  , userInput):.  
-000167d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000167e0: 2020 2020 2020 7072 696e 7428 2222 290a        print("").
-000167f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016800: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
-00016810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016820: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
-00016830: 2020 2020 2020 2020 2020 2020 2070 6173               pas
-00016840: 730a 2020 2020 2020 2020 2020 2020 2320  s.            # 
-00016850: 7472 7920 746f 2072 756e 2061 7320 6120  try to run as a 
-00016860: 7079 7468 6f6e 2073 6372 6970 7420 6669  python script fi
-00016870: 7273 740a 2020 2020 2020 2020 2020 2020  rst.            
-00016880: 6966 2063 6f6e 6669 672e 6465 7665 6c6f  if config.develo
-00016890: 7065 723a 0a20 2020 2020 2020 2020 2020  per:.           
-000168a0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-000168b0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
-000168c0: 6563 2875 7365 7249 6e70 7574 2c20 676c  ec(userInput, gl
-000168d0: 6f62 616c 7328 2929 0a20 2020 2020 2020  obals()).       
-000168e0: 2020 2020 2020 2020 2020 2020 2070 7269               pri
-000168f0: 6e74 2822 2229 0a20 2020 2020 2020 2020  nt("").         
-00016900: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
-00016910: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
-00016920: 2020 2020 6578 6365 7074 3a0a 2020 2020      except:.    
+00014500: 2020 2020 636f 6e74 656e 7420 3d20 695b      content = i[
+00014510: 2263 6f6e 7465 6e74 225d 0a20 2020 2020  "content"].     
+00014520: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00014530: 6c61 696e 5465 7874 202b 3d20 6622 5c6e  lainText += f"\n
+00014540: 5c6e 7b63 6f6e 7465 6e74 7d5c 6e5c 6e22  \n{content}\n\n"
+00014550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014560: 2065 6c69 6620 695b 2272 6f6c 6522 5d20   elif i["role"] 
+00014570: 3d3d 2022 6173 7369 7374 616e 7422 3a0a  == "assistant":.
+00014580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014590: 2020 2020 636f 6e74 656e 7420 3d20 695b      content = i[
+000145a0: 2263 6f6e 7465 6e74 225d 0a20 2020 2020  "content"].     
+000145b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000145c0: 6620 636f 6e74 656e 7420 6973 206e 6f74  f content is not
+000145d0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000145e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000145f0: 6620 706c 6169 6e54 6578 743a 0a20 2020  f plainText:.   
+00014600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014610: 2020 2020 2020 2020 2070 6c61 696e 5465           plainTe
+00014620: 7874 202b 3d20 225c 6e5c 6e22 0a20 2020  xt += "\n\n".   
+00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014640: 2020 2020 2070 6c61 696e 5465 7874 202b       plainText +
+00014650: 3d20 6622 7b63 6f6e 7465 6e74 7d5c 6e5c  = f"{content}\n\
+00014660: 6e22 0a20 2020 2020 2020 2020 2020 2070  n".            p
+00014670: 6c61 696e 5465 7874 203d 2070 6c61 696e  lainText = plain
+00014680: 5465 7874 2e73 7472 6970 2829 0a20 2020  Text.strip().   
+00014690: 2020 2020 2020 2020 2069 6620 636f 6e66           if conf
+000146a0: 6967 2e74 6572 6d69 6e61 6c45 6e61 626c  ig.terminalEnabl
+000146b0: 6554 6572 6d75 7841 5049 3a0a 2020 2020  eTermuxAPI:.    
+000146c0: 2020 2020 2020 2020 2020 2020 7079 646f              pydo
+000146d0: 632e 7069 7065 7061 6765 7228 706c 6169  c.pipepager(plai
+000146e0: 6e54 6578 742c 2063 6d64 3d22 7465 726d  nText, cmd="term
+000146f0: 7578 2d73 6861 7265 202d 6120 7365 6e64  ux-share -a send
+00014700: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+00014710: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014720: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00014730: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+00014740: 6c64 6572 5061 7468 203d 206f 732e 7061  lderPath = os.pa
+00014750: 7468 2e6a 6f69 6e28 636f 6e66 6967 2e6c  th.join(config.l
+00014760: 6f63 616c 5374 6f72 6167 652c 2022 6368  ocalStorage, "ch
+00014770: 6174 7322 2c20 2265 7870 6f72 7422 290a  ats", "export").
+00014780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014790: 2020 2020 5061 7468 2866 6f6c 6465 7250      Path(folderP
+000147a0: 6174 6829 2e6d 6b64 6972 2870 6172 656e  ath).mkdir(paren
+000147b0: 7473 3d54 7275 652c 2065 7869 7374 5f6f  ts=True, exist_o
+000147c0: 6b3d 5472 7565 290a 2020 2020 2020 2020  k=True).        
+000147d0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+000147e0: 732e 7061 7468 2e69 7364 6972 2866 6f6c  s.path.isdir(fol
+000147f0: 6465 7250 6174 6829 3a0a 2020 2020 2020  derPath):.      
+00014800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014810: 2020 6368 6174 4669 6c65 203d 206f 732e    chatFile = os.
+00014820: 7061 7468 2e6a 6f69 6e28 666f 6c64 6572  path.join(folder
+00014830: 5061 7468 2c20 6622 7b74 696d 6573 7461  Path, f"{timesta
+00014840: 6d70 7d2e 7478 7422 290a 2020 2020 2020  mp}.txt").      
+00014850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014860: 2020 7769 7468 206f 7065 6e28 6368 6174    with open(chat
+00014870: 4669 6c65 2c20 2277 222c 2065 6e63 6f64  File, "w", encod
+00014880: 696e 673d 2275 7466 2d38 2229 2061 7320  ing="utf-8") as 
+00014890: 6669 6c65 4f62 6a3a 0a20 2020 2020 2020  fileObj:.       
+000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148b0: 2020 2020 2066 696c 654f 626a 2e77 7269       fileObj.wri
+000148c0: 7465 2870 6c61 696e 5465 7874 290a 2020  te(plainText).  
+000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148e0: 2020 2020 2020 6966 206f 7065 6e46 696c        if openFil
+000148f0: 6520 616e 6420 6f73 2e70 6174 682e 6973  e and os.path.is
+00014900: 6669 6c65 2863 6861 7446 696c 6529 3a0a  file(chatFile):.
+00014910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014920: 2020 2020 2020 2020 2020 2020 6f73 2e73              os.s
+00014930: 7973 7465 6d28 6627 2727 7b63 6f6e 6669  ystem(f'''{confi
+00014940: 672e 6f70 656e 7d20 227b 6368 6174 4669  g.open} "{chatFi
+00014950: 6c65 7d22 2727 2729 0a20 2020 2020 2020  le}"''').       
+00014960: 2020 2020 2020 2020 2065 7863 6570 743a           except:
+00014970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014980: 2020 2020 2070 7269 6e74 3228 2246 6169       print2("Fai
+00014990: 6c65 6420 746f 2073 6176 6520 6368 6174  led to save chat
+000149a0: 215c 6e22 290a 2020 2020 2020 2020 2020  !\n").          
+000149b0: 2020 2020 2020 2020 2020 7368 6f77 4572            showEr
+000149c0: 726f 7273 2829 0a0a 2020 2020 6465 6620  rors()..    def 
+000149d0: 7275 6e49 6e73 7472 7563 7469 6f6e 2873  runInstruction(s
+000149e0: 656c 6629 3a0a 2020 2020 2020 2020 696e  elf):.        in
+000149f0: 7374 7275 6374 696f 6e73 203d 206c 6973  structions = lis
+00014a00: 7428 636f 6e66 6967 2e70 7265 6465 6669  t(config.predefi
+00014a10: 6e65 6449 6e73 7472 7563 7469 6f6e 732e  nedInstructions.
+00014a20: 6b65 7973 2829 290a 2020 2020 2020 2020  keys()).        
+00014a30: 696e 7374 7275 6374 696f 6e20 3d20 7365  instruction = se
+00014a40: 6c66 2e64 6961 6c6f 6773 2e67 6574 5661  lf.dialogs.getVa
+00014a50: 6c69 644f 7074 696f 6e73 280a 2020 2020  lidOptions(.    
+00014a60: 2020 2020 2020 2020 6f70 7469 6f6e 733d          options=
+00014a70: 696e 7374 7275 6374 696f 6e73 2c0a 2020  instructions,.  
+00014a80: 2020 2020 2020 2020 2020 7469 746c 653d            title=
+00014a90: 2250 7265 6465 6669 6e65 6420 496e 7374  "Predefined Inst
+00014aa0: 7275 6374 696f 6e73 222c 0a20 2020 2020  ructions",.     
+00014ab0: 2020 2020 2020 2074 6578 743d 2253 656c         text="Sel
+00014ac0: 6563 7420 616e 2069 6e73 7472 7563 7469  ect an instructi
+00014ad0: 6f6e 3a22 2c0a 2020 2020 2020 2020 290a  on:",.        ).
+00014ae0: 2020 2020 2020 2020 6966 2069 6e73 7472          if instr
+00014af0: 7563 7469 6f6e 3a0a 2020 2020 2020 2020  uction:.        
+00014b00: 2020 2020 636f 6e66 6967 2e64 6566 6175      config.defau
+00014b10: 6c74 456e 7472 7920 3d20 636f 6e66 6967  ltEntry = config
+00014b20: 2e70 7265 6465 6669 6e65 6449 6e73 7472  .predefinedInstr
+00014b30: 7563 7469 6f6e 735b 696e 7374 7275 6374  uctions[instruct
+00014b40: 696f 6e5d 0a20 2020 2020 2020 2020 2020  ion].           
+00014b50: 2063 6f6e 6669 672e 6163 6365 7074 5f64   config.accept_d
+00014b60: 6566 6175 6c74 203d 2054 7275 650a 0a20  efault = True.. 
+00014b70: 2020 2064 6566 2063 6861 6e67 6543 6f6e     def changeCon
+00014b80: 7465 7874 2873 656c 6629 3a0a 2020 2020  text(self):.    
+00014b90: 2020 2020 636f 6e74 6578 7473 203d 206c      contexts = l
+00014ba0: 6973 7428 636f 6e66 6967 2e70 7265 6465  ist(config.prede
+00014bb0: 6669 6e65 6443 6f6e 7465 7874 732e 6b65  finedContexts.ke
+00014bc0: 7973 2829 290a 2020 2020 2020 2020 7072  ys()).        pr
+00014bd0: 6564 6566 696e 6564 436f 6e74 6578 7420  edefinedContext 
+00014be0: 3d20 7365 6c66 2e64 6961 6c6f 6773 2e67  = self.dialogs.g
+00014bf0: 6574 5661 6c69 644f 7074 696f 6e73 280a  etValidOptions(.
+00014c00: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+00014c10: 6f6e 733d 636f 6e74 6578 7473 2c0a 2020  ons=contexts,.  
+00014c20: 2020 2020 2020 2020 2020 7469 746c 653d            title=
+00014c30: 2250 7265 6465 6669 6e65 6420 436f 6e74  "Predefined Cont
+00014c40: 6578 7473 222c 0a20 2020 2020 2020 2020  exts",.         
+00014c50: 2020 2064 6566 6175 6c74 3d63 6f6e 6669     default=confi
+00014c60: 672e 7072 6564 6566 696e 6564 436f 6e74  g.predefinedCont
+00014c70: 6578 742c 0a20 2020 2020 2020 2020 2020  ext,.           
+00014c80: 2074 6578 743d 2253 656c 6563 7420 6120   text="Select a 
+00014c90: 636f 6e74 6578 743a 222c 0a20 2020 2020  context:",.     
+00014ca0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+00014cb0: 7072 6564 6566 696e 6564 436f 6e74 6578  predefinedContex
+00014cc0: 743a 0a20 2020 2020 2020 2020 2020 2063  t:.            c
+00014cd0: 6f6e 6669 672e 7072 6564 6566 696e 6564  onfig.predefined
+00014ce0: 436f 6e74 6578 7420 3d20 7072 6564 6566  Context = predef
+00014cf0: 696e 6564 436f 6e74 6578 740a 2020 2020  inedContext.    
+00014d00: 2020 2020 2020 2020 6966 2063 6f6e 6669          if confi
+00014d10: 672e 7072 6564 6566 696e 6564 436f 6e74  g.predefinedCont
+00014d20: 6578 7420 3d3d 2022 5b63 7573 746f 6d5d  ext == "[custom]
+00014d30: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00014d40: 2020 2070 7269 6e74 3128 2245 6469 7420     print1("Edit 
+00014d50: 6375 7374 6f6d 2063 6f6e 7465 7874 2062  custom context b
+00014d60: 656c 6f77 3a22 290a 2020 2020 2020 2020  elow:").        
+00014d70: 2020 2020 2020 2020 6375 7374 6f6d 436f          customCo
+00014d80: 6e74 6578 7420 3d20 7365 6c66 2e70 726f  ntext = self.pro
+00014d90: 6d70 7473 2e73 696d 706c 6550 726f 6d70  mpts.simplePromp
+00014da0: 7428 7374 796c 653d 7365 6c66 2e70 726f  t(style=self.pro
+00014db0: 6d70 7473 2e70 726f 6d70 7453 7479 6c65  mpts.promptStyle
+00014dc0: 322c 2064 6566 6175 6c74 3d63 6f6e 6669  2, default=confi
+00014dd0: 672e 6375 7374 6f6d 5072 6564 6566 696e  g.customPredefin
+00014de0: 6564 436f 6e74 6578 7429 0a20 2020 2020  edContext).     
+00014df0: 2020 2020 2020 2020 2020 2069 6620 6375             if cu
+00014e00: 7374 6f6d 436f 6e74 6578 7420 616e 6420  stomContext and 
+00014e10: 6e6f 7420 6375 7374 6f6d 436f 6e74 6578  not customContex
+00014e20: 742e 7374 7269 7028 292e 6c6f 7765 7228  t.strip().lower(
+00014e30: 2920 3d3d 2063 6f6e 6669 672e 6578 6974  ) == config.exit
+00014e40: 5f65 6e74 7279 3a0a 2020 2020 2020 2020  _entry:.        
+00014e50: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
+00014e60: 6967 2e63 7573 746f 6d50 7265 6465 6669  ig.customPredefi
+00014e70: 6e65 6443 6f6e 7465 7874 203d 2063 7573  nedContext = cus
+00014e80: 746f 6d43 6f6e 7465 7874 2e73 7472 6970  tomContext.strip
+00014e90: 2829 0a20 2020 2020 2020 2065 6c73 653a  ().        else:
+00014ea0: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
+00014eb0: 2077 6179 2074 6f20 7175 6963 6b6c 7920   way to quickly 
+00014ec0: 636c 6561 6e20 7570 2063 6f6e 7465 7874  clean up context
+00014ed0: 0a20 2020 2020 2020 2020 2020 2063 6f6e  .            con
+00014ee0: 6669 672e 7072 6564 6566 696e 6564 436f  fig.predefinedCo
+00014ef0: 6e74 6578 7420 3d20 225b 6e6f 6e65 5d22  ntext = "[none]"
+00014f00: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
+00014f10: 7361 7665 436f 6e66 6967 2829 0a20 2020  saveConfig().   
+00014f20: 2020 2020 2073 656c 662e 7368 6f77 4375       self.showCu
+00014f30: 7272 656e 7443 6f6e 7465 7874 2829 0a0a  rrentContext()..
+00014f40: 2020 2020 6465 6620 6765 7444 6972 6563      def getDirec
+00014f50: 746f 7279 4c69 7374 2873 656c 6629 3a0a  toryList(self):.
+00014f60: 2020 2020 2020 2020 6469 7265 6374 6f72          director
+00014f70: 794c 6973 7420 3d20 5b5d 0a20 2020 2020  yList = [].     
+00014f80: 2020 2066 6f72 2066 2069 6e20 6f73 2e6c     for f in os.l
+00014f90: 6973 7464 6972 2827 2e27 293a 0a20 2020  istdir('.'):.   
+00014fa0: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
+00014fb0: 6174 682e 6973 6469 7228 6629 3a0a 2020  ath.isdir(f):.  
+00014fc0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00014fd0: 7061 7261 746f 7220 3d20 225c 5c22 2069  parator = "\\" i
+00014fe0: 6620 636f 6e66 6967 2e74 6869 7350 6c61  f config.thisPla
+00014ff0: 7466 6f72 6d20 3d3d 2022 5769 6e64 6f77  tform == "Window
+00015000: 7322 2065 6c73 6520 222f 220a 2020 2020  s" else "/".    
+00015010: 2020 2020 2020 2020 2020 2020 6469 7265              dire
+00015020: 6374 6f72 794c 6973 742e 6170 7065 6e64  ctoryList.append
+00015030: 2866 227b 667d 7b73 6570 6172 6174 6f72  (f"{f}{separator
+00015040: 7d22 290a 2020 2020 2020 2020 2020 2020  }").            
+00015050: 656c 6966 206f 732e 7061 7468 2e69 7366  elif os.path.isf
+00015060: 696c 6528 6629 3a0a 2020 2020 2020 2020  ile(f):.        
+00015070: 2020 2020 2020 2020 6469 7265 6374 6f72          director
+00015080: 794c 6973 742e 6170 7065 6e64 2866 290a  yList.append(f).
+00015090: 2020 2020 2020 2020 7265 7475 726e 2064          return d
+000150a0: 6972 6563 746f 7279 4c69 7374 0a0a 2020  irectoryList..  
+000150b0: 2020 6465 6620 7368 6f77 4c6f 676f 2873    def showLogo(s
+000150c0: 656c 6629 3a0a 2020 2020 2020 2020 6170  elf):.        ap
+000150d0: 704e 616d 6520 3d20 636f 6e66 6967 2e66  pName = config.f
+000150e0: 7265 6547 656e 6975 7341 494e 616d 652e  reeGeniusAIName.
+000150f0: 7370 6c69 7428 295b 305d 2e75 7070 6572  split()[0].upper
+00015100: 2829 0a20 2020 2020 2020 2074 6572 6d69  ().        termi
+00015110: 6e61 6c5f 7769 6474 6820 3d20 7368 7574  nal_width = shut
+00015120: 696c 2e67 6574 5f74 6572 6d69 6e61 6c5f  il.get_terminal_
+00015130: 7369 7a65 2829 2e63 6f6c 756d 6e73 0a20  size().columns. 
+00015140: 2020 2020 2020 2074 7279 3a0a 2020 2020         try:.    
+00015150: 2020 2020 2020 2020 6672 6f6d 2061 7274          from art
+00015160: 2069 6d70 6f72 7420 7465 7874 3261 7274   import text2art
+00015170: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00015180: 7465 726d 696e 616c 5f77 6964 7468 203e  terminal_width >
+00015190: 3d20 3332 3a0a 2020 2020 2020 2020 2020  = 32:.          
+000151a0: 2020 2020 2020 6c6f 676f 203d 2074 6578        logo = tex
+000151b0: 7432 6172 7428 6170 704e 616d 652c 2066  t2art(appName, f
+000151c0: 6f6e 743d 2263 7962 6572 6d65 6475 6d22  ont="cybermedum"
+000151d0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+000151e0: 6966 2074 6572 6d69 6e61 6c5f 7769 6474  if terminal_widt
+000151f0: 6820 3e3d 2032 303a 0a20 2020 2020 2020  h >= 20:.       
+00015200: 2020 2020 2020 2020 206c 6f67 6f20 3d20           logo = 
+00015210: 7465 7874 3261 7274 2822 2022 2e6a 6f69  text2art(" ".joi
+00015220: 6e28 6170 704e 616d 6529 202b 2022 2022  n(appName) + " "
+00015230: 2c20 666f 6e74 3d22 7768 6974 655f 6275  , font="white_bu
+00015240: 6262 6c65 2229 0a20 2020 2020 2020 2020  bble").         
+00015250: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00015260: 2020 2020 2020 2020 206c 6f67 6f20 3d20           logo = 
+00015270: 636f 6e66 6967 2e66 7265 6547 656e 6975  config.freeGeniu
+00015280: 7341 494e 616d 650a 2020 2020 2020 2020  sAIName.        
+00015290: 2020 2020 6c6f 676f 203d 206c 6f67 6f5b      logo = logo[
+000152a0: 3a2d 315d 2023 2072 656d 6f76 6520 7468  :-1] # remove th
+000152b0: 6520 6c69 6e65 6272 6561 6b20 6174 2074  e linebreak at t
+000152c0: 6865 2065 6e64 0a20 2020 2020 2020 2065  he end.        e
+000152d0: 7863 6570 743a 0a20 2020 2020 2020 2020  xcept:.         
+000152e0: 2020 206c 6f67 6f20 3d20 636f 6e66 6967     logo = config
+000152f0: 2e66 7265 6547 656e 6975 7341 494e 616d  .freeGeniusAINam
+00015300: 650a 2020 2020 2020 2020 7072 696e 745f  e.        print_
+00015310: 666f 726d 6174 7465 645f 7465 7874 2848  formatted_text(H
+00015320: 544d 4c28 6622 3c7b 636f 6e66 6967 2e74  TML(f"<{config.t
+00015330: 6572 6d69 6e61 6c43 6f6d 6d61 6e64 456e  erminalCommandEn
+00015340: 7472 7943 6f6c 6f72 327d 3e7b 6c6f 676f  tryColor2}>{logo
+00015350: 7d3c 2f7b 636f 6e66 6967 2e74 6572 6d69  }</{config.termi
+00015360: 6e61 6c43 6f6d 6d61 6e64 456e 7472 7943  nalCommandEntryC
+00015370: 6f6c 6f72 327d 3e22 2929 0a0a 2020 2020  olor2}>"))..    
+00015380: 6465 6620 7275 6e50 7974 686f 6e53 6372  def runPythonScr
+00015390: 6970 7428 7365 6c66 2c20 7363 7269 7074  ipt(self, script
+000153a0: 293a 0a20 2020 2020 2020 2073 6372 6970  ):.        scrip
+000153b0: 7420 3d20 7363 7269 7074 2e73 7472 6970  t = script.strip
+000153c0: 2829 5b33 3a2d 335d 0a20 2020 2020 2020  ()[3:-3].       
+000153d0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+000153e0: 2020 6578 6563 2873 6372 6970 742c 2067    exec(script, g
+000153f0: 6c6f 6261 6c73 2829 290a 2020 2020 2020  lobals()).      
+00015400: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+00015410: 2020 2020 2020 7472 6163 6520 3d20 7472        trace = tr
+00015420: 6163 6562 6163 6b2e 666f 726d 6174 5f65  aceback.format_e
+00015430: 7863 2829 0a20 2020 2020 2020 2020 2020  xc().           
+00015440: 2070 7269 6e74 2874 7261 6365 2069 6620   print(trace if 
+00015450: 636f 6e66 6967 2e64 6576 656c 6f70 6572  config.developer
+00015460: 2065 6c73 6520 2245 7272 6f72 2065 6e63   else "Error enc
+00015470: 6f75 6e74 6572 6564 2122 290a 2020 2020  ountered!").    
+00015480: 2020 2020 2020 2020 7072 696e 7431 2863          print1(c
+00015490: 6f6e 6669 672e 6469 7669 6465 7229 0a20  onfig.divider). 
+000154a0: 2020 2020 2020 2020 2020 2069 6620 636f             if co
+000154b0: 6e66 6967 2e6d 6178 5f63 6f6e 7365 6375  nfig.max_consecu
+000154c0: 7469 7665 5f61 7574 6f5f 636f 7272 6563  tive_auto_correc
+000154d0: 7469 6f6e 203e 2030 3a0a 2020 2020 2020  tion > 0:.      
+000154e0: 2020 2020 2020 2020 2020 4361 6c6c 4c4c            CallLL
+000154f0: 4d2e 6175 746f 436f 7272 6563 7450 7974  M.autoCorrectPyt
+00015500: 686f 6e43 6f64 6528 7363 7269 7074 2c20  honCode(script, 
+00015510: 7472 6163 6529 0a0a 2020 2020 6465 6620  trace)..    def 
+00015520: 7374 6172 7443 6861 7473 2873 656c 6629  startChats(self)
+00015530: 3a0a 2020 2020 2020 2020 746f 6b65 6e56  :.        tokenV
+00015540: 616c 6964 6174 6f72 203d 2054 6f6b 656e  alidator = Token
+00015550: 5661 6c69 6461 746f 7228 290a 2020 2020  Validator().    
+00015560: 2020 2020 6465 6620 6765 7444 796e 616d      def getDynam
+00015570: 6963 546f 6f6c 4261 7228 293a 0a20 2020  icToolBar():.   
+00015580: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00015590: 636f 6e66 6967 2e64 796e 616d 6963 546f  config.dynamicTo
+000155a0: 6f6c 4261 7254 6578 740a 2020 2020 2020  olBarText.      
+000155b0: 2020 6465 6620 7374 6172 7443 6861 7428    def startChat(
+000155c0: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
+000155d0: 6c65 6172 2829 0a20 2020 2020 2020 2020  lear().         
+000155e0: 2020 2070 7269 6e74 3128 7365 6c66 2e64     print1(self.d
+000155f0: 6976 6964 6572 290a 2020 2020 2020 2020  ivider).        
+00015600: 2020 2020 7365 6c66 2e73 686f 774c 6f67      self.showLog
+00015610: 6f28 290a 2020 2020 2020 2020 2020 2020  o().            
+00015620: 7365 6c66 2e73 686f 7743 7572 7265 6e74  self.showCurrent
+00015630: 436f 6e74 6578 7428 290a 2020 2020 2020  Context().      
+00015640: 2020 2020 2020 2320 676f 2074 6f20 7374        # go to st
+00015650: 6172 7475 7020 6469 7265 6374 6f72 790a  artup directory.
+00015660: 2020 2020 2020 2020 2020 2020 7374 6f72              stor
+00015670: 6167 6564 6972 6563 746f 7279 203d 2063  agedirectory = c
+00015680: 6f6e 6669 672e 6c6f 6361 6c53 746f 7261  onfig.localStora
+00015690: 6765 0a20 2020 2020 2020 2020 2020 206f  ge.            o
+000156a0: 732e 6368 6469 7228 7374 6f72 6167 6564  s.chdir(storaged
+000156b0: 6972 6563 746f 7279 290a 2020 2020 2020  irectory).      
+000156c0: 2020 2020 2020 6d65 7373 6167 6573 203d        messages =
+000156d0: 2043 616c 6c4c 4c4d 2e72 6573 6574 4d65   CallLLM.resetMe
+000156e0: 7373 6167 6573 2829 0a20 2020 2020 2020  ssages().       
+000156f0: 2020 2020 2023 7072 696e 7431 2866 2273       #print1(f"s
+00015700: 7461 7274 7570 2064 6972 6563 746f 7279  tartup directory
+00015710: 3a5c 6e7b 7374 6f72 6167 6564 6972 6563  :\n{storagedirec
+00015720: 746f 7279 7d22 290a 2020 2020 2020 2020  tory}").        
+00015730: 2020 2020 7072 696e 745f 666f 726d 6174      print_format
+00015740: 7465 645f 7465 7874 2848 544d 4c28 6622  ted_text(HTML(f"
+00015750: 3c7b 636f 6e66 6967 2e74 6572 6d69 6e61  <{config.termina
+00015760: 6c50 726f 6d70 7449 6e64 6963 6174 6f72  lPromptIndicator
+00015770: 436f 6c6f 7232 7d3e 4469 7265 6374 6f72  Color2}>Director
+00015780: 793a 3c2f 7b63 6f6e 6669 672e 7465 726d  y:</{config.term
+00015790: 696e 616c 5072 6f6d 7074 496e 6469 6361  inalPromptIndica
+000157a0: 746f 7243 6f6c 6f72 327d 3e20 7b73 746f  torColor2}> {sto
+000157b0: 7261 6765 6469 7265 6374 6f72 797d 2229  ragedirectory}")
+000157c0: 290a 2020 2020 2020 2020 2020 2020 7072  ).            pr
+000157d0: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
+000157e0: 7229 0a0a 2020 2020 2020 2020 2020 2020  r)..            
+000157f0: 636f 6e66 6967 2e63 6f6e 7665 7273 6174  config.conversat
+00015800: 696f 6e53 7461 7274 6564 203d 2046 616c  ionStarted = Fal
+00015810: 7365 0a20 2020 2020 2020 2020 2020 2072  se.            r
+00015820: 6574 7572 6e20 2873 746f 7261 6765 6469  eturn (storagedi
+00015830: 7265 6374 6f72 792c 206d 6573 7361 6765  rectory, message
+00015840: 7329 0a20 2020 2020 2020 2073 746f 7261  s).        stora
+00015850: 6765 6469 7265 6374 6f72 792c 2063 6f6e  gedirectory, con
+00015860: 6669 672e 6375 7272 656e 744d 6573 7361  fig.currentMessa
+00015870: 6765 7320 3d20 7374 6172 7443 6861 7428  ges = startChat(
+00015880: 290a 2020 2020 2020 2020 636f 6e66 6967  ).        config
+00015890: 2e6d 756c 7469 6c69 6e65 496e 7075 7420  .multilineInput 
+000158a0: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+000158b0: 6665 6174 7572 6573 4c6f 7765 7220 3d20  featuresLower = 
+000158c0: 6c69 7374 2873 656c 662e 6163 7469 6f6e  list(self.action
+000158d0: 732e 6b65 7973 2829 2920 2b20 5b22 2e2e  s.keys()) + ["..
+000158e0: 2e22 5d0a 2020 2020 2020 2020 2320 696e  ."].        # in
+000158f0: 7075 7420 7375 6767 6573 7469 6f6e 730a  put suggestions.
+00015900: 2020 2020 2020 2020 636f 6e66 6967 2e69          config.i
+00015910: 6e70 7574 5375 6767 6573 7469 6f6e 7320  nputSuggestions 
+00015920: 2b3d 2066 6561 7475 7265 734c 6f77 6572  += featuresLower
+00015930: 0a20 2020 2020 2020 2063 6f6d 706c 6574  .        complet
+00015940: 6572 203d 2046 757a 7a79 436f 6d70 6c65  er = FuzzyComple
+00015950: 7465 7228 576f 7264 436f 6d70 6c65 7465  ter(WordComplete
+00015960: 7228 636f 6e66 6967 2e69 6e70 7574 5375  r(config.inputSu
+00015970: 6767 6573 7469 6f6e 732c 2069 676e 6f72  ggestions, ignor
+00015980: 655f 6361 7365 3d54 7275 6529 2920 6966  e_case=True)) if
+00015990: 2063 6f6e 6669 672e 696e 7075 7453 7567   config.inputSug
+000159a0: 6765 7374 696f 6e73 2065 6c73 6520 4e6f  gestions else No
+000159b0: 6e65 0a20 2020 2020 2020 2063 6f6d 706c  ne.        compl
+000159c0: 6574 6572 5f64 6576 656c 6f70 6572 203d  eter_developer =
+000159d0: 2046 757a 7a79 436f 6d70 6c65 7465 7228   FuzzyCompleter(
+000159e0: 576f 7264 436f 6d70 6c65 7465 7228 636f  WordCompleter(co
+000159f0: 6e66 6967 2e69 6e70 7574 5375 6767 6573  nfig.inputSugges
+00015a00: 7469 6f6e 735b 3a5d 202b 205b 6622 636f  tions[:] + [f"co
+00015a10: 6e66 6967 2e7b 697d 2220 666f 7220 6920  nfig.{i}" for i 
+00015a20: 696e 2064 6972 2863 6f6e 6669 6729 2069  in dir(config) i
+00015a30: 6620 6e6f 7420 692e 7374 6172 7473 7769  f not i.startswi
+00015a40: 7468 2822 5f5f 2229 5d20 2b20 7365 6c66  th("__")] + self
+00015a50: 2e67 6574 4469 7265 6374 6f72 794c 6973  .getDirectoryLis
+00015a60: 7428 292c 2069 676e 6f72 655f 6361 7365  t(), ignore_case
+00015a70: 3d54 7275 6529 290a 2020 2020 2020 2020  =True)).        
+00015a80: 7768 696c 6520 5472 7565 3a0a 2020 2020  while True:.    
+00015a90: 2020 2020 2020 2020 2320 6465 6661 756c          # defaul
+00015aa0: 7420 746f 6f6c 6261 7220 7465 7874 0a20  t toolbar text. 
+00015ab0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+00015ac0: 672e 6479 6e61 6d69 6354 6f6f 6c42 6172  g.dynamicToolBar
+00015ad0: 5465 7874 203d 2066 2222 2220 7b73 7472  Text = f""" {str
+00015ae0: 2863 6f6e 6669 672e 686f 746b 6579 5f65  (config.hotkey_e
+00015af0: 7869 7429 2e72 6570 6c61 6365 2822 2722  xit).replace("'"
+00015b00: 2c20 2222 297d 2065 7869 7420 7b73 7472  , "")} exit {str
+00015b10: 2863 6f6e 6669 672e 686f 746b 6579 5f64  (config.hotkey_d
+00015b20: 6973 706c 6179 5f6b 6579 5f63 6f6d 626f  isplay_key_combo
+00015b30: 292e 7265 706c 6163 6528 2227 222c 2022  ).replace("'", "
+00015b40: 2229 7d20 7368 6f72 7463 7574 7320 2222  ")} shortcuts ""
+00015b50: 220a 2020 2020 2020 2020 2020 2020 2320  ".            # 
+00015b60: 6469 7370 6c61 7920 6375 7272 656e 7420  display current 
+00015b70: 6469 7265 6374 6f72 7920 6966 2063 6861  directory if cha
+00015b80: 6e67 6564 0a20 2020 2020 2020 2020 2020  nged.           
+00015b90: 2063 7572 7265 6e74 4469 7265 6374 6f72   currentDirector
+00015ba0: 7920 3d20 6f73 2e67 6574 6377 6428 290a  y = os.getcwd().
+00015bb0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00015bc0: 6f74 2063 7572 7265 6e74 4469 7265 6374  ot currentDirect
+00015bd0: 6f72 7920 3d3d 2073 746f 7261 6765 6469  ory == storagedi
+00015be0: 7265 6374 6f72 793a 0a20 2020 2020 2020  rectory:.       
+00015bf0: 2020 2020 2020 2020 2023 7072 696e 7431           #print1
+00015c00: 2873 656c 662e 6469 7669 6465 7229 0a20  (self.divider). 
+00015c10: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00015c20: 7269 6e74 3328 6622 4375 7272 656e 7420  rint3(f"Current 
+00015c30: 6469 7265 6374 6f72 793a 207b 6375 7272  directory: {curr
+00015c40: 656e 7444 6972 6563 746f 7279 7d22 290a  entDirectory}").
+00015c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c60: 7072 696e 7431 2873 656c 662e 6469 7669  print1(self.divi
+00015c70: 6465 7229 0a20 2020 2020 2020 2020 2020  der).           
+00015c80: 2020 2020 2073 746f 7261 6765 6469 7265       storagedire
+00015c90: 6374 6f72 7920 3d20 6375 7272 656e 7444  ctory = currentD
+00015ca0: 6972 6563 746f 7279 0a20 2020 2020 2020  irectory.       
+00015cb0: 2020 2020 2023 2064 6566 6175 6c74 2069       # default i
+00015cc0: 6e70 7574 2065 6e74 7279 0a20 2020 2020  nput entry.     
+00015cd0: 2020 2020 2020 2061 6363 6570 745f 6465         accept_de
+00015ce0: 6661 756c 7420 3d20 636f 6e66 6967 2e61  fault = config.a
+00015cf0: 6363 6570 745f 6465 6661 756c 740a 2020  ccept_default.  
+00015d00: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00015d10: 2e61 6363 6570 745f 6465 6661 756c 7420  .accept_default 
+00015d20: 3d20 4661 6c73 650a 2020 2020 2020 2020  = False.        
+00015d30: 2020 2020 6465 6661 756c 7445 6e74 7279      defaultEntry
+00015d40: 203d 2063 6f6e 6669 672e 6465 6661 756c   = config.defaul
+00015d50: 7445 6e74 7279 0a20 2020 2020 2020 2020  tEntry.         
+00015d60: 2020 2069 6620 6f73 2e70 6174 682e 6973     if os.path.is
+00015d70: 6669 6c65 2864 6566 6175 6c74 456e 7472  file(defaultEntr
+00015d80: 7929 3a0a 2020 2020 2020 2020 2020 2020  y):.            
+00015d90: 2020 2020 6465 6661 756c 7445 6e74 7279      defaultEntry
+00015da0: 203d 2066 2746 696c 653a 2022 7b64 6566   = f'File: "{def
+00015db0: 6175 6c74 456e 7472 797d 225c 6e27 0a20  aultEntry}"\n'. 
+00015dc0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00015dd0: 6f73 2e70 6174 682e 6973 6469 7228 6465  os.path.isdir(de
+00015de0: 6661 756c 7445 6e74 7279 293a 0a20 2020  faultEntry):.   
+00015df0: 2020 2020 2020 2020 2020 2020 2064 6566               def
+00015e00: 6175 6c74 456e 7472 7920 3d20 6627 466f  aultEntry = f'Fo
+00015e10: 6c64 6572 3a20 227b 6465 6661 756c 7445  lder: "{defaultE
+00015e20: 6e74 7279 7d22 5c6e 270a 2020 2020 2020  ntry}"\n'.      
+00015e30: 2020 2020 2020 636f 6e66 6967 2e64 6566        config.def
+00015e40: 6175 6c74 456e 7472 7920 3d20 2222 0a0a  aultEntry = ""..
+00015e50: 2020 2020 2020 2020 2020 2020 2320 7573              # us
+00015e60: 6572 2069 6e70 7574 0a20 2020 2020 2020  er input.       
+00015e70: 2020 2020 2075 7365 7249 6e70 7574 203d       userInput =
+00015e80: 2073 656c 662e 7072 6f6d 7074 732e 7369   self.prompts.si
+00015e90: 6d70 6c65 5072 6f6d 7074 2870 726f 6d70  mplePrompt(promp
+00015ea0: 7453 6573 7369 6f6e 3d73 656c 662e 7465  tSession=self.te
+00015eb0: 726d 696e 616c 5f63 6861 745f 7365 7373  rminal_chat_sess
+00015ec0: 696f 6e2c 2063 6f6d 706c 6574 6572 3d63  ion, completer=c
+00015ed0: 6f6d 706c 6574 6572 5f64 6576 656c 6f70  ompleter_develop
+00015ee0: 6572 2069 6620 636f 6e66 6967 2e64 6576  er if config.dev
+00015ef0: 656c 6f70 6572 2065 6c73 6520 636f 6d70  eloper else comp
+00015f00: 6c65 7465 722c 2064 6566 6175 6c74 3d64  leter, default=d
+00015f10: 6566 6175 6c74 456e 7472 792c 2061 6363  efaultEntry, acc
+00015f20: 6570 745f 6465 6661 756c 743d 6163 6365  ept_default=acce
+00015f30: 7074 5f64 6566 6175 6c74 2c20 7661 6c69  pt_default, vali
+00015f40: 6461 746f 723d 746f 6b65 6e56 616c 6964  dator=tokenValid
+00015f50: 6174 6f72 2c20 626f 7474 6f6d 5f74 6f6f  ator, bottom_too
+00015f60: 6c62 6172 3d67 6574 4479 6e61 6d69 6354  lbar=getDynamicT
+00015f70: 6f6f 6c42 6172 290a 2020 2020 2020 2020  oolBar).        
+00015f80: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00015f90: 2023 2075 7064 6174 6520 7379 7374 656d   # update system
+00015fa0: 206d 6573 7361 6765 2077 6865 6e20 7573   message when us
+00015fb0: 6572 2065 6e74 6572 2061 206e 6577 2069  er enter a new i
+00015fc0: 6e70 7574 0a20 2020 2020 2020 2020 2020  nput.           
+00015fd0: 2063 6f6e 6669 672e 6375 7272 656e 744d   config.currentM
+00015fe0: 6573 7361 6765 7320 3d20 7365 6c66 2e75  essages = self.u
+00015ff0: 7064 6174 6553 7973 7465 6d4d 6573 7361  pdateSystemMessa
+00016000: 6765 2863 6f6e 6669 672e 6375 7272 656e  ge(config.curren
+00016010: 744d 6573 7361 6765 7329 0a20 2020 2020  tMessages).     
+00016020: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00016030: 2020 2020 2320 6469 7370 6c61 7920 6f70      # display op
+00016040: 7469 6f6e 7320 7768 656e 2065 6d70 7479  tions when empty
+00016050: 2073 7472 696e 6720 6973 2065 6e74 6572   string is enter
+00016060: 6564 0a20 2020 2020 2020 2020 2020 2075  ed.            u
+00016070: 7365 7249 6e70 7574 4c6f 7765 7220 3d20  serInputLower = 
+00016080: 7573 6572 496e 7075 742e 6c6f 7765 7228  userInput.lower(
+00016090: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+000160a0: 2063 6f6e 6669 672e 6164 6450 6174 6841   config.addPathA
+000160b0: 7420 6973 206e 6f74 204e 6f6e 653a 0a20  t is not None:. 
+000160c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000160d0: 7265 6669 7820 3d20 7573 6572 496e 7075  refix = userInpu
+000160e0: 745b 3a63 6f6e 6669 672e 6164 6450 6174  t[:config.addPat
+000160f0: 6841 745d 0a20 2020 2020 2020 2020 2020  hAt].           
+00016100: 2020 2020 2070 7265 6669 7853 706c 6974       prefixSplit
+00016110: 203d 2070 7265 6669 782e 7273 706c 6974   = prefix.rsplit
+00016120: 2822 2022 2c20 3129 0a20 2020 2020 2020  (" ", 1).       
+00016130: 2020 2020 2020 2020 2069 6620 6c65 6e28           if len(
+00016140: 7072 6566 6978 5370 6c69 7429 203e 2031  prefixSplit) > 1
+00016150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016160: 2020 2020 2020 6465 6661 756c 7420 3d20        default = 
+00016170: 7072 6566 6978 5370 6c69 745b 2d31 5d0a  prefixSplit[-1].
+00016180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016190: 2020 2020 7072 6566 6978 203d 2066 227b      prefix = f"{
+000161a0: 7072 6566 6978 5370 6c69 745b 305d 7d20  prefixSplit[0]} 
+000161b0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000161c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000161d0: 2020 2020 2020 2020 2020 2020 6465 6661              defa
+000161e0: 756c 7420 3d20 7072 6566 6978 0a20 2020  ult = prefix.   
+000161f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016200: 2070 7265 6669 7820 3d20 2222 0a20 2020   prefix = "".   
+00016210: 2020 2020 2020 2020 2020 2020 2073 7566               suf
+00016220: 6669 7820 3d20 7573 6572 496e 7075 745b  fix = userInput[
+00016230: 636f 6e66 6967 2e61 6464 5061 7468 4174  config.addPathAt
+00016240: 3a5d 0a20 2020 2020 2020 2020 2020 2020  :].             
+00016250: 2020 2063 6f6e 6669 672e 6164 6450 6174     config.addPat
+00016260: 6841 7420 3d20 4e6f 6e65 0a20 2020 2020  hAt = None.     
+00016270: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+00016280: 7420 6465 6661 756c 743a 0a20 2020 2020  t default:.     
+00016290: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+000162a0: 6566 6175 6c74 203d 206f 732e 6765 7463  efault = os.getc
+000162b0: 7764 2829 0a20 2020 2020 2020 2020 2020  wd().           
+000162c0: 2020 2020 2075 7365 7250 6174 6820 3d20       userPath = 
+000162d0: 7365 6c66 2e67 6574 5061 7468 2e67 6574  self.getPath.get
+000162e0: 5061 7468 286d 6573 7361 6765 3d66 227b  Path(message=f"{
+000162f0: 7072 6566 6978 7d3c 7b63 6f6e 6669 672e  prefix}<{config.
+00016300: 7465 726d 696e 616c 436f 6d6d 616e 6445  terminalCommandE
+00016310: 6e74 7279 436f 6c6f 7232 7d3e 5b61 6464  ntryColor2}>[add
+00016320: 2061 2070 6174 6820 6865 7265 5d3c 2f7b   a path here]</{
+00016330: 636f 6e66 6967 2e74 6572 6d69 6e61 6c43  config.terminalC
+00016340: 6f6d 6d61 6e64 456e 7472 7943 6f6c 6f72  ommandEntryColor
+00016350: 327d 3e7b 7375 6666 6978 7d22 2c20 7072  2}>{suffix}", pr
+00016360: 6f6d 7074 496e 6469 6361 746f 723d 223e  omptIndicator=">
+00016370: 3e3e 2022 2c20 656d 7074 795f 746f 5f63  >> ", empty_to_c
+00016380: 616e 6365 6c3d 5472 7565 2c20 6465 6661  ancel=True, defa
+00016390: 756c 743d 6465 6661 756c 7429 0a20 2020  ult=default).   
+000163a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+000163b0: 6669 672e 6465 6661 756c 7445 6e74 7279  fig.defaultEntry
+000163c0: 203d 2066 227b 7072 6566 6978 7d7b 7573   = f"{prefix}{us
+000163d0: 6572 5061 7468 7d7b 7375 6666 6978 7d22  erPath}{suffix}"
+000163e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000163f0: 2075 7365 7249 6e70 7574 203d 2022 220a   userInput = "".
+00016400: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00016410: 206e 6f74 2075 7365 7249 6e70 7574 4c6f   not userInputLo
+00016420: 7765 723a 0a20 2020 2020 2020 2020 2020  wer:.           
+00016430: 2020 2020 2075 7365 7249 6e70 7574 203d       userInput =
+00016440: 2063 6f6e 6669 672e 626c 616e 6b45 6e74   config.blankEnt
+00016450: 7279 4163 7469 6f6e 0a20 2020 2020 2020  ryAction.       
+00016460: 2020 2020 2069 6620 7573 6572 496e 7075       if userInpu
+00016470: 7420 3d3d 2022 2e2e 2e22 3a0a 2020 2020  t == "...":.    
+00016480: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00016490: 496e 7075 7420 3d20 7573 6572 496e 7075  Input = userInpu
+000164a0: 744c 6f77 6572 203d 2073 656c 662e 7275  tLower = self.ru
+000164b0: 6e41 6374 696f 6e73 2875 7365 7249 6e70  nActions(userInp
+000164c0: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
+000164d0: 2365 6c69 6620 7573 6572 496e 7075 744c  #elif userInputL
+000164e0: 6f77 6572 2069 6e20 7475 706c 6528 7365  ower in tuple(se
+000164f0: 6c66 2e61 6374 696f 6e73 2e6b 6579 7328  lf.actions.keys(
+00016500: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00016510: 656c 6966 2075 7365 7249 6e70 7574 4c6f  elif userInputLo
+00016520: 7765 722e 7374 6172 7473 7769 7468 2822  wer.startswith("
+00016530: 2e22 2920 616e 6420 6e6f 7420 7573 6572  .") and not user
+00016540: 496e 7075 744c 6f77 6572 2069 6e20 2863  InputLower in (c
+00016550: 6f6e 6669 672e 6578 6974 5f65 6e74 7279  onfig.exit_entry
+00016560: 2c20 636f 6e66 6967 2e63 616e 6365 6c5f  , config.cancel_
+00016570: 656e 7472 792c 2022 2e6e 6577 222c 2022  entry, ".new", "
+00016580: 2e63 6f6e 7465 7874 2229 3a0a 2020 2020  .context"):.    
+00016590: 2020 2020 2020 2020 2020 2020 7573 6572              user
+000165a0: 496e 7075 7420 3d20 7573 6572 496e 7075  Input = userInpu
+000165b0: 744c 6f77 6572 203d 2073 656c 662e 7275  tLower = self.ru
+000165c0: 6e41 6374 696f 6e73 2822 2e2e 2e22 2c20  nActions("...", 
+000165d0: 7573 6572 496e 7075 7429 0a0a 2020 2020  userInput)..    
+000165e0: 2020 2020 2020 2020 6966 2073 6574 546f          if setTo
+000165f0: 6f6c 4465 7065 6e64 656e 6365 2875 7365  olDependence(use
+00016600: 7249 6e70 7574 293a 0a20 2020 2020 2020  rInput):.       
+00016610: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+00016620: 650a 0a20 2020 2020 2020 2020 2020 2023  e..            #
+00016630: 2072 6570 6c61 6365 2061 6c69 6173 2c20   replace alias, 
+00016640: 6966 2061 6e79 2c20 7769 7468 2066 756c  if any, with ful
+00016650: 6c20 656e 7472 790a 2020 2020 2020 2020  l entry.        
+00016660: 2020 2020 666f 7220 616c 6961 732c 2066      for alias, f
+00016670: 756c 6c45 6e74 7279 2069 6e20 636f 6e66  ullEntry in conf
+00016680: 6967 2e61 6c69 6173 6573 2e69 7465 6d73  ig.aliases.items
+00016690: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+000166a0: 2020 2020 2375 7365 7249 6e70 7574 203d      #userInput =
+000166b0: 2072 652e 7375 6228 616c 6961 732c 2066   re.sub(alias, f
+000166c0: 756c 6c45 6e74 7279 2c20 7573 6572 496e  ullEntry, userIn
+000166d0: 7075 7429 2023 2065 7272 6f72 206f 6e20  put) # error on 
+000166e0: 5769 6e64 6f77 7320 636f 7a20 6f66 2057  Windows coz of W
+000166f0: 696e 646f 7773 2070 6174 680a 2020 2020  indows path.    
+00016700: 2020 2020 2020 2020 2020 2020 7573 6572              user
+00016710: 496e 7075 7420 3d20 7573 6572 496e 7075  Input = userInpu
+00016720: 742e 7265 706c 6163 6528 616c 6961 732c  t.replace(alias,
+00016730: 2066 756c 6c45 6e74 7279 290a 0a20 2020   fullEntry)..   
+00016740: 2020 2020 2020 2020 2023 206f 7065 6e20           # open 
+00016750: 6669 6c65 202f 2064 6972 6563 746f 7279  file / directory
+00016760: 2064 6972 6563 746c 790a 2020 2020 2020   directly.      
+00016770: 2020 2020 2020 646f 6373 5f70 6174 6820        docs_path 
+00016780: 3d20 6973 4578 6973 7469 6e67 5061 7468  = isExistingPath
+00016790: 2875 7365 7249 6e70 7574 290a 2020 2020  (userInput).    
+000167a0: 2020 2020 2020 2020 6966 206f 732e 7061          if os.pa
+000167b0: 7468 2e69 7366 696c 6528 646f 6373 5f70  th.isfile(docs_p
+000167c0: 6174 6829 3a0a 2020 2020 2020 2020 2020  ath):.          
+000167d0: 2020 2020 2020 6f73 2e73 7973 7465 6d28        os.system(
+000167e0: 6622 7b63 6f6e 6669 672e 6f70 656e 7d20  f"{config.open} 
+000167f0: 7b64 6f63 735f 7061 7468 7d22 290a 2020  {docs_path}").  
+00016800: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00016810: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
+00016820: 2020 2065 6c69 6620 6f73 2e70 6174 682e     elif os.path.
+00016830: 6973 6469 7228 646f 6373 5f70 6174 6829  isdir(docs_path)
+00016840: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016850: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00016860: 2020 2020 2020 2020 2020 206f 732e 6368             os.ch
+00016870: 6469 7228 646f 6373 5f70 6174 6829 0a20  dir(docs_path). 
+00016880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016890: 2020 2070 7269 6e74 3328 6622 4469 7265     print3(f"Dire
+000168a0: 6374 6f72 7920 6368 616e 6765 6420 746f  ctory changed to
+000168b0: 3a20 7b64 6f63 735f 7061 7468 7d22 290a  : {docs_path}").
+000168c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168d0: 2020 2020 7365 6c66 2e67 6574 5061 7468      self.getPath
+000168e0: 2e64 6973 706c 6179 4469 7265 6374 6f72  .displayDirector
+000168f0: 7943 6f6e 7465 6e74 2829 0a20 2020 2020  yContent().     
+00016900: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00016910: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+00016920: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
 00016930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016940: 7061 7373 0a0a 2020 2020 2020 2020 2020  pass..          
-00016950: 2020 6966 2075 7365 7249 6e70 7574 2e73    if userInput.s
-00016960: 7461 7274 7377 6974 6828 2221 2229 3a0a  tartswith("!"):.
-00016970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016980: 7365 6c66 2e72 756e 5379 7374 656d 436f  self.runSystemCo
-00016990: 6d6d 616e 6428 7573 6572 496e 7075 7429  mmand(userInput)
-000169a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000169b0: 2070 7269 6e74 2822 2229 0a20 2020 2020   print("").     
-000169c0: 2020 2020 2020 2065 6c69 6620 636f 6e66         elif conf
-000169d0: 6967 2e64 6576 656c 6f70 6572 2061 6e64  ig.developer and
-000169e0: 2075 7365 7249 6e70 7574 2e73 7461 7274   userInput.start
-000169f0: 7377 6974 6828 2260 6060 2229 2061 6e64  swith("```") and
-00016a00: 2075 7365 7249 6e70 7574 2e65 6e64 7377   userInput.endsw
-00016a10: 6974 6828 2260 6060 2229 2061 6e64 206e  ith("```") and n
-00016a20: 6f74 2075 7365 7249 6e70 7574 203d 3d20  ot userInput == 
-00016a30: 2260 6060 6060 6022 3a0a 2020 2020 2020  "``````":.      
-00016a40: 2020 2020 2020 2020 2020 7573 6572 496e            userIn
-00016a50: 7075 7420 3d20 7265 2e73 7562 2822 6060  put = re.sub("``
-00016a60: 6070 7974 686f 6e22 2c20 2260 6060 222c  `python", "```",
-00016a70: 2075 7365 7249 6e70 7574 290a 2020 2020   userInput).    
-00016a80: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016a90: 2e72 756e 5079 7468 6f6e 5363 7269 7074  .runPythonScript
-00016aa0: 2875 7365 7249 6e70 7574 290a 2020 2020  (userInput).    
-00016ab0: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-00016ac0: 7428 2222 290a 2020 2020 2020 2020 2020  t("").          
-00016ad0: 2020 656c 6966 2075 7365 7249 6e70 7574    elif userInput
-00016ae0: 4c6f 7765 7220 3d3d 2063 6f6e 6669 672e  Lower == config.
-00016af0: 6578 6974 5f65 6e74 7279 3a0a 2020 2020  exit_entry:.    
-00016b00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00016b10: 2e73 6176 6543 6861 7428 636f 6e66 6967  .saveChat(config
-00016b20: 2e63 7572 7265 6e74 4d65 7373 6167 6573  .currentMessages
-00016b30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00016b40: 2020 7265 7475 726e 2073 656c 662e 6578    return self.ex
-00016b50: 6974 4163 7469 6f6e 2829 0a20 2020 2020  itAction().     
-00016b60: 2020 2020 2020 2065 6c69 6620 7573 6572         elif user
-00016b70: 496e 7075 744c 6f77 6572 203d 3d20 636f  InputLower == co
-00016b80: 6e66 6967 2e63 616e 6365 6c5f 656e 7472  nfig.cancel_entr
-00016b90: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-00016ba0: 2020 2070 6173 730a 2020 2020 2020 2020     pass.        
-00016bb0: 2020 2020 656c 6966 2075 7365 7249 6e70      elif userInp
-00016bc0: 7574 4c6f 7765 7220 3d3d 2022 2e63 6f6e  utLower == ".con
-00016bd0: 7465 7874 223a 0a20 2020 2020 2020 2020  text":.         
-00016be0: 2020 2020 2020 2073 656c 662e 6368 616e         self.chan
-00016bf0: 6765 436f 6e74 6578 7428 290a 2020 2020  geContext().    
-00016c00: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00016c10: 6f74 2063 6f6e 6669 672e 6170 706c 7950  ot config.applyP
-00016c20: 7265 6465 6669 6e65 6443 6f6e 7465 7874  redefinedContext
-00016c30: 416c 7761 7973 3a0a 2020 2020 2020 2020  Always:.        
-00016c40: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-00016c50: 6f6e 6669 672e 636f 6e76 6572 7361 7469  onfig.conversati
-00016c60: 6f6e 5374 6172 7465 643a 0a20 2020 2020  onStarted:.     
-00016c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016c80: 2020 2073 656c 662e 7361 7665 4368 6174     self.saveChat
-00016c90: 2863 6f6e 6669 672e 6375 7272 656e 744d  (config.currentM
-00016ca0: 6573 7361 6765 7329 0a20 2020 2020 2020  essages).       
-00016cb0: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-00016cc0: 7261 6765 6469 7265 6374 6f72 792c 2063  ragedirectory, c
-00016cd0: 6f6e 6669 672e 6375 7272 656e 744d 6573  onfig.currentMes
-00016ce0: 7361 6765 7320 3d20 7374 6172 7443 6861  sages = startCha
-00016cf0: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00016d00: 656c 6966 2075 7365 7249 6e70 7574 4c6f  elif userInputLo
-00016d10: 7765 7220 3d3d 2022 2e6e 6577 223a 0a20  wer == ".new":. 
-00016d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016d30: 656c 662e 7361 7665 4368 6174 2863 6f6e  elf.saveChat(con
-00016d40: 6669 672e 6375 7272 656e 744d 6573 7361  fig.currentMessa
-00016d50: 6765 7329 0a20 2020 2020 2020 2020 2020  ges).           
-00016d60: 2020 2020 2073 746f 7261 6765 6469 7265       storagedire
-00016d70: 6374 6f72 792c 2063 6f6e 6669 672e 6375  ctory, config.cu
-00016d80: 7272 656e 744d 6573 7361 6765 7320 3d20  rrentMessages = 
-00016d90: 7374 6172 7443 6861 7428 290a 2020 2020  startChat().    
-00016da0: 2020 2020 2020 2020 656c 6966 2075 7365          elif use
-00016db0: 7249 6e70 7574 2061 6e64 206e 6f74 2075  rInput and not u
-00016dc0: 7365 7249 6e70 7574 4c6f 7765 7220 696e  serInputLower in
-00016dd0: 2066 6561 7475 7265 734c 6f77 6572 3a0a   featuresLower:.
-00016de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016df0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-00016e00: 2020 2020 2020 2020 2069 6620 7573 6572           if user
-00016e10: 496e 7075 7420 616e 6420 636f 6e66 6967  Input and config
-00016e20: 2e74 7473 496e 7075 743a 0a20 2020 2020  .ttsInput:.     
-00016e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016e40: 2020 2054 5453 5574 696c 2e70 6c61 7928     TTSUtil.play(
-00016e50: 7573 6572 496e 7075 7429 0a20 2020 2020  userInput).     
-00016e60: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00016e70: 2046 6561 7475 7265 3a20 696d 7072 6f76   Feature: improv
-00016e80: 6520 7772 6974 696e 673a 0a20 2020 2020  e writing:.     
-00016e90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00016ea0: 7065 6369 616c 456e 7472 7950 6174 7465  pecialEntryPatte
-00016eb0: 726e 203d 2022 5c5b 544f 4f4c 5f5b 5e5c  rn = "\[TOOL_[^\
-00016ec0: 5b5c 5d5d 2a3f 5c5d 7c5c 5b4e 4f5f 544f  [\]]*?\]|\[NO_TO
-00016ed0: 4f4c 5c5d 7c5c 5b4e 4f5f 5343 5245 454e  OL\]|\[NO_SCREEN
-00016ee0: 494e 475c 5d22 0a20 2020 2020 2020 2020  ING\]".         
-00016ef0: 2020 2020 2020 2020 2020 2073 7065 6369             speci
-00016f00: 616c 456e 7472 7920 3d20 7265 2e73 6561  alEntry = re.sea
-00016f10: 7263 6828 7370 6563 6961 6c45 6e74 7279  rch(specialEntry
-00016f20: 5061 7474 6572 6e2c 2075 7365 7249 6e70  Pattern, userInp
-00016f30: 7574 290a 2020 2020 2020 2020 2020 2020  ut).            
-00016f40: 2020 2020 2020 2020 7370 6563 6961 6c45          specialE
-00016f50: 6e74 7279 203d 2073 7065 6369 616c 456e  ntry = specialEn
-00016f60: 7472 792e 6772 6f75 7028 3029 2069 6620  try.group(0) if 
-00016f70: 7370 6563 6961 6c45 6e74 7279 2065 6c73  specialEntry els
-00016f80: 6520 2222 0a20 2020 2020 2020 2020 2020  e "".           
-00016f90: 2020 2020 2020 2020 2075 7365 7249 6e70           userInp
-00016fa0: 7574 203d 2072 652e 7375 6228 7370 6563  ut = re.sub(spec
-00016fb0: 6961 6c45 6e74 7279 5061 7474 6572 6e2c  ialEntryPattern,
-00016fc0: 2022 222c 2075 7365 7249 6e70 7574 2920   "", userInput) 
-00016fd0: 2320 7265 6d6f 7665 2073 7065 6369 616c  # remove special
-00016fe0: 2065 6e74 7279 2074 656d 706f 7261 7269   entry temporari
-00016ff0: 6c79 0a20 2020 2020 2020 2020 2020 2020  ly.             
-00017000: 2020 2020 2020 2069 6620 7573 6572 496e         if userIn
-00017010: 7075 7420 616e 6420 636f 6e66 6967 2e64  put and config.d
-00017020: 6973 706c 6179 496d 7072 6f76 6564 5772  isplayImprovedWr
-00017030: 6974 696e 673a 0a20 2020 2020 2020 2020  iting:.         
-00017040: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-00017050: 7365 7249 6e70 7574 203d 2072 652e 7375  serInput = re.su
-00017060: 6228 225c 6e5c 5b43 7572 7265 6e74 2074  b("\n\[Current t
-00017070: 696d 653a 205b 5e5c 6e5d 2a3f 2422 2c20  ime: [^\n]*?$", 
-00017080: 2222 2c20 7573 6572 496e 7075 7429 0a20  "", userInput). 
-00017090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170a0: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
-000170b0: 2e69 7354 6572 6d75 783a 0a20 2020 2020  .isTermux:.     
-000170c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000170d0: 2020 2020 2020 2064 6179 5f6f 665f 7765         day_of_we
-000170e0: 656b 203d 2022 220a 2020 2020 2020 2020  ek = "".        
-000170f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017100: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00017110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017120: 2020 6461 795f 6f66 5f77 6565 6b20 3d20    day_of_week = 
-00017130: 6622 746f 6461 7920 6973 207b 6765 7444  f"today is {getD
-00017140: 6179 4f66 5765 656b 2829 7d20 616e 6420  ayOfWeek()} and 
-00017150: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00017160: 2020 2020 2020 2020 2020 696d 7072 6f76            improv
-00017170: 6564 5665 7273 696f 6e20 3d20 4361 6c6c  edVersion = Call
-00017180: 4c4c 4d2e 6765 7453 696e 676c 6543 6861  LLM.getSingleCha
-00017190: 7452 6573 706f 6e73 6528 6622 2222 496d  tResponse(f"""Im
-000171a0: 7072 6f76 6520 7468 6520 666f 6c6c 6f77  prove the follow
-000171b0: 696e 6720 7772 6974 696e 672c 2061 6363  ing writing, acc
-000171c0: 6f72 6469 6e67 2074 6f20 7b63 6f6e 6669  ording to {confi
-000171d0: 672e 696d 7072 6f76 6564 5772 6974 696e  g.improvedWritin
-000171e0: 6753 7974 6c65 7d0a 496e 2061 6464 6974  gSytle}.In addit
-000171f0: 696f 6e2c 2049 2077 6f75 6c64 206c 696b  ion, I would lik
-00017200: 6520 796f 7520 746f 2068 656c 7020 6d65  e you to help me
-00017210: 2077 6974 6820 636f 6e76 6572 7469 6e67   with converting
-00017220: 2072 656c 6174 6976 6520 6461 7465 7320   relative dates 
-00017230: 616e 6420 7469 6d65 732c 2069 6620 616e  and times, if an
-00017240: 792c 2069 6e74 6f20 6578 6163 7420 6461  y, into exact da
-00017250: 7465 7320 616e 6420 7469 6d65 7320 6261  tes and times ba
-00017260: 7365 6420 6f6e 2074 6865 2072 6566 6572  sed on the refer
-00017270: 656e 6365 2074 6861 7420 7b64 6179 5f6f  ence that {day_o
-00017280: 665f 7765 656b 7d63 7572 7265 6e74 2064  f_week}current d
-00017290: 6174 6574 696d 6520 6973 207b 7374 7228  atetime is {str(
-000172a0: 6461 7465 7469 6d65 2e64 6174 6574 696d  datetime.datetim
-000172b0: 652e 6e6f 7728 2929 7d2e 0a52 656d 656d  e.now())}..Remem
-000172c0: 6265 722c 2070 726f 7669 6465 206d 6520  ber, provide me 
-000172d0: 7769 7468 2074 6865 2069 6d70 726f 7665  with the improve
-000172e0: 6420 7772 6974 696e 6720 6f6e 6c79 2c20  d writing only, 
-000172f0: 656e 636c 6f73 6564 2069 6e20 7472 6970  enclosed in trip
-00017300: 6c65 2071 756f 7465 7320 6060 6020 616e  le quotes ``` an
-00017310: 6420 7769 7468 6f75 7420 616e 7920 6164  d without any ad
-00017320: 6469 7469 6f6e 616c 2069 6e66 6f72 6d61  ditional informa
-00017330: 7469 6f6e 206f 7220 636f 6d6d 656e 7473  tion or comments
-00017340: 2e0a 4d79 2077 7269 7469 6e67 3a0a 7b75  ..My writing:.{u
-00017350: 7365 7249 6e70 7574 7d22 2222 290a 2020  serInput}""").  
-00017360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017370: 2020 2020 2020 6966 2069 6d70 726f 7665        if improve
-00017380: 6456 6572 7369 6f6e 2061 6e64 2069 6d70  dVersion and imp
-00017390: 726f 7665 6456 6572 7369 6f6e 2e73 7461  rovedVersion.sta
-000173a0: 7274 7377 6974 6828 2260 6060 2229 2061  rtswith("```") a
-000173b0: 6e64 2069 6d70 726f 7665 6456 6572 7369  nd improvedVersi
-000173c0: 6f6e 2e65 6e64 7377 6974 6828 2260 6060  on.endswith("```
-000173d0: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000173e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000173f0: 7072 696e 7431 2869 6d70 726f 7665 6456  print1(improvedV
-00017400: 6572 7369 6f6e 290a 2020 2020 2020 2020  ersion).        
-00017410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017420: 2020 2020 7573 6572 496e 7075 7420 3d20      userInput = 
-00017430: 696d 7072 6f76 6564 5665 7273 696f 6e5b  improvedVersion[
-00017440: 333a 2d33 5d0a 2020 2020 2020 2020 2020  3:-3].          
-00017450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017460: 2020 6966 2063 6f6e 6669 672e 7474 734f    if config.ttsO
-00017470: 7574 7075 743a 0a20 2020 2020 2020 2020  utput:.         
-00017480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017490: 2020 2020 2020 2054 5453 5574 696c 2e70         TTSUtil.p
-000174a0: 6c61 7928 7573 6572 496e 7075 7429 0a20  lay(userInput). 
+00016940: 2020 2020 7061 7373 0a0a 2020 2020 2020      pass..      
+00016950: 2020 2020 2020 2320 7472 7920 6576 616c        # try eval
+00016960: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016970: 636f 6e66 6967 2e64 6576 656c 6f70 6572  config.developer
+00016980: 2061 6e64 206e 6f74 2075 7365 7249 6e70   and not userInp
+00016990: 7574 203d 3d20 222e 2e2e 223a 0a20 2020  ut == "...":.   
+000169a0: 2020 2020 2020 2020 2020 2020 2074 7279               try
+000169b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000169c0: 2020 2020 2020 7661 6c75 6520 3d20 6576        value = ev
+000169d0: 616c 2875 7365 7249 6e70 7574 2920 2320  al(userInput) # 
+000169e0: 6974 2073 6f6c 7665 2073 696d 706c 6520  it solve simple 
+000169f0: 6d61 7468 2c20 652e 672e 2031 2b31 2c20  math, e.g. 1+1, 
+00016a00: 6f72 2072 6561 6420 7661 7269 6162 6c65  or read variable
+00016a10: 732c 2065 2e67 2e20 6469 7228 636f 6e66  s, e.g. dir(conf
+00016a20: 6967 290a 2020 2020 2020 2020 2020 2020  ig).            
+00016a30: 2020 2020 2020 2020 6966 2076 616c 7565          if value
+00016a40: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00016a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016a60: 2020 2020 2020 2370 7269 6e74 2876 616c        #print(val
+00016a70: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
+00016a80: 2020 2020 2020 2020 2020 2020 7070 7269              ppri
+00016a90: 6e74 2e70 7072 696e 7428 7661 6c75 6529  nt.pprint(value)
+00016aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016ab0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00016ac0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00016ad0: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+00016ae0: 6e75 650a 2020 2020 2020 2020 2020 2020  nue.            
+00016af0: 2020 2020 2020 2020 656c 6966 2072 652e          elif re.
+00016b00: 7365 6172 6368 2822 5e70 7269 6e74 5c28  search("^print\(
+00016b10: 5b5e 5c29 5c29 5d2b 3f5c 2924 222c 2075  [^\)\)]+?\)$", u
+00016b20: 7365 7249 6e70 7574 293a 0a20 2020 2020  serInput):.     
+00016b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b40: 2020 2070 7269 6e74 2822 2229 0a20 2020     print("").   
+00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016b60: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+00016b70: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00016b80: 6365 7074 3a0a 2020 2020 2020 2020 2020  cept:.          
+00016b90: 2020 2020 2020 2020 2020 7061 7373 0a20            pass. 
+00016ba0: 2020 2020 2020 2020 2020 2023 2074 7279             # try
+00016bb0: 2074 6f20 7275 6e20 6173 2061 2070 7974   to run as a pyt
+00016bc0: 686f 6e20 7363 7269 7074 2066 6972 7374  hon script first
+00016bd0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00016be0: 636f 6e66 6967 2e64 6576 656c 6f70 6572  config.developer
+00016bf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00016c00: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00016c10: 2020 2020 2020 2020 2020 2065 7865 6328             exec(
+00016c20: 7573 6572 496e 7075 742c 2067 6c6f 6261  userInput, globa
+00016c30: 6c73 2829 290a 2020 2020 2020 2020 2020  ls()).          
+00016c40: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00016c50: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
+00016c60: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+00016c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c80: 2065 7863 6570 743a 0a20 2020 2020 2020   except:.       
+00016c90: 2020 2020 2020 2020 2020 2020 2070 6173               pas
+00016ca0: 730a 0a20 2020 2020 2020 2020 2020 2069  s..            i
+00016cb0: 6620 7573 6572 496e 7075 742e 7374 6172  f userInput.star
+00016cc0: 7473 7769 7468 2822 2122 293a 0a20 2020  tswith("!"):.   
+00016cd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00016ce0: 662e 7275 6e53 7973 7465 6d43 6f6d 6d61  f.runSystemComma
+00016cf0: 6e64 2875 7365 7249 6e70 7574 290a 2020  nd(userInput).  
+00016d00: 2020 2020 2020 2020 2020 2020 2020 7072                pr
+00016d10: 696e 7428 2222 290a 2020 2020 2020 2020  int("").        
+00016d20: 2020 2020 656c 6966 2063 6f6e 6669 672e      elif config.
+00016d30: 6465 7665 6c6f 7065 7220 616e 6420 7573  developer and us
+00016d40: 6572 496e 7075 742e 7374 6172 7473 7769  erInput.startswi
+00016d50: 7468 2822 6060 6022 2920 616e 6420 7573  th("```") and us
+00016d60: 6572 496e 7075 742e 656e 6473 7769 7468  erInput.endswith
+00016d70: 2822 6060 6022 2920 616e 6420 6e6f 7420  ("```") and not 
+00016d80: 7573 6572 496e 7075 7420 3d3d 2022 6060  userInput == "``
+00016d90: 6060 6060 223a 0a20 2020 2020 2020 2020  ````":.         
+00016da0: 2020 2020 2020 2075 7365 7249 6e70 7574         userInput
+00016db0: 203d 2072 652e 7375 6228 2260 6060 7079   = re.sub("```py
+00016dc0: 7468 6f6e 222c 2022 6060 6022 2c20 7573  thon", "```", us
+00016dd0: 6572 496e 7075 7429 0a20 2020 2020 2020  erInput).       
+00016de0: 2020 2020 2020 2020 2073 656c 662e 7275           self.ru
+00016df0: 6e50 7974 686f 6e53 6372 6970 7428 7573  nPythonScript(us
+00016e00: 6572 496e 7075 7429 0a20 2020 2020 2020  erInput).       
+00016e10: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+00016e20: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+00016e30: 6c69 6620 7573 6572 496e 7075 744c 6f77  lif userInputLow
+00016e40: 6572 203d 3d20 636f 6e66 6967 2e65 7869  er == config.exi
+00016e50: 745f 656e 7472 793a 0a20 2020 2020 2020  t_entry:.       
+00016e60: 2020 2020 2020 2020 2073 656c 662e 7361           self.sa
+00016e70: 7665 4368 6174 2863 6f6e 6669 672e 6375  veChat(config.cu
+00016e80: 7272 656e 744d 6573 7361 6765 7329 0a20  rrentMessages). 
+00016e90: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00016ea0: 6574 7572 6e20 7365 6c66 2e65 7869 7441  eturn self.exitA
+00016eb0: 6374 696f 6e28 290a 2020 2020 2020 2020  ction().        
+00016ec0: 2020 2020 656c 6966 2075 7365 7249 6e70      elif userInp
+00016ed0: 7574 4c6f 7765 7220 3d3d 2063 6f6e 6669  utLower == confi
+00016ee0: 672e 6361 6e63 656c 5f65 6e74 7279 3a0a  g.cancel_entry:.
+00016ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016f00: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+00016f10: 2065 6c69 6620 7573 6572 496e 7075 744c   elif userInputL
+00016f20: 6f77 6572 203d 3d20 222e 636f 6e74 6578  ower == ".contex
+00016f30: 7422 3a0a 2020 2020 2020 2020 2020 2020  t":.            
+00016f40: 2020 2020 7365 6c66 2e63 6861 6e67 6543      self.changeC
+00016f50: 6f6e 7465 7874 2829 0a20 2020 2020 2020  ontext().       
+00016f60: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00016f70: 636f 6e66 6967 2e61 7070 6c79 5072 6564  config.applyPred
+00016f80: 6566 696e 6564 436f 6e74 6578 7441 6c77  efinedContextAlw
+00016f90: 6179 733a 0a20 2020 2020 2020 2020 2020  ays:.           
+00016fa0: 2020 2020 2020 2020 2069 6620 636f 6e66           if conf
+00016fb0: 6967 2e63 6f6e 7665 7273 6174 696f 6e53  ig.conversationS
+00016fc0: 7461 7274 6564 3a0a 2020 2020 2020 2020  tarted:.        
+00016fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016fe0: 7365 6c66 2e73 6176 6543 6861 7428 636f  self.saveChat(co
+00016ff0: 6e66 6967 2e63 7572 7265 6e74 4d65 7373  nfig.currentMess
+00017000: 6167 6573 290a 2020 2020 2020 2020 2020  ages).          
+00017010: 2020 2020 2020 2020 2020 7374 6f72 6167            storag
+00017020: 6564 6972 6563 746f 7279 2c20 636f 6e66  edirectory, conf
+00017030: 6967 2e63 7572 7265 6e74 4d65 7373 6167  ig.currentMessag
+00017040: 6573 203d 2073 7461 7274 4368 6174 2829  es = startChat()
+00017050: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+00017060: 6620 7573 6572 496e 7075 744c 6f77 6572  f userInputLower
+00017070: 203d 3d20 222e 6e65 7722 3a0a 2020 2020   == ".new":.    
+00017080: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017090: 2e73 6176 6543 6861 7428 636f 6e66 6967  .saveChat(config
+000170a0: 2e63 7572 7265 6e74 4d65 7373 6167 6573  .currentMessages
+000170b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000170c0: 2020 7374 6f72 6167 6564 6972 6563 746f    storagedirecto
+000170d0: 7279 2c20 636f 6e66 6967 2e63 7572 7265  ry, config.curre
+000170e0: 6e74 4d65 7373 6167 6573 203d 2073 7461  ntMessages = sta
+000170f0: 7274 4368 6174 2829 0a20 2020 2020 2020  rtChat().       
+00017100: 2020 2020 2065 6c69 6620 7573 6572 496e       elif userIn
+00017110: 7075 7420 616e 6420 6e6f 7420 7573 6572  put and not user
+00017120: 496e 7075 744c 6f77 6572 2069 6e20 6665  InputLower in fe
+00017130: 6174 7572 6573 4c6f 7765 723a 0a20 2020  aturesLower:.   
+00017140: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00017150: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00017160: 2020 2020 2020 6966 2075 7365 7249 6e70        if userInp
+00017170: 7574 2061 6e64 2063 6f6e 6669 672e 7474  ut and config.tt
+00017180: 7349 6e70 7574 3a0a 2020 2020 2020 2020  sInput:.        
+00017190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000171a0: 5454 5355 7469 6c2e 706c 6179 2875 7365  TTSUtil.play(use
+000171b0: 7249 6e70 7574 290a 2020 2020 2020 2020  rInput).        
+000171c0: 2020 2020 2020 2020 2020 2020 2320 4665              # Fe
+000171d0: 6174 7572 653a 2069 6d70 726f 7665 2077  ature: improve w
+000171e0: 7269 7469 6e67 3a0a 2020 2020 2020 2020  riting:.        
+000171f0: 2020 2020 2020 2020 2020 2020 7370 6563              spec
+00017200: 6961 6c45 6e74 7279 5061 7474 6572 6e20  ialEntryPattern 
+00017210: 3d20 225c 5b54 4f4f 4c5f 5b5e 5c5b 5c5d  = "\[TOOL_[^\[\]
+00017220: 5d2a 3f5c 5d7c 5c5b 4e4f 5f54 4f4f 4c5c  ]*?\]|\[NO_TOOL\
+00017230: 5d7c 5c5b 4e4f 5f53 4352 4545 4e49 4e47  ]|\[NO_SCREENING
+00017240: 5c5d 220a 2020 2020 2020 2020 2020 2020  \]".            
+00017250: 2020 2020 2020 2020 7370 6563 6961 6c45          specialE
+00017260: 6e74 7279 203d 2072 652e 7365 6172 6368  ntry = re.search
+00017270: 2873 7065 6369 616c 456e 7472 7950 6174  (specialEntryPat
+00017280: 7465 726e 2c20 7573 6572 496e 7075 7429  tern, userInput)
+00017290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000172a0: 2020 2020 2073 7065 6369 616c 456e 7472       specialEntr
+000172b0: 7920 3d20 7370 6563 6961 6c45 6e74 7279  y = specialEntry
+000172c0: 2e67 726f 7570 2830 2920 6966 2073 7065  .group(0) if spe
+000172d0: 6369 616c 456e 7472 7920 656c 7365 2022  cialEntry else "
+000172e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+000172f0: 2020 2020 2020 7573 6572 496e 7075 7420        userInput 
+00017300: 3d20 7265 2e73 7562 2873 7065 6369 616c  = re.sub(special
+00017310: 456e 7472 7950 6174 7465 726e 2c20 2222  EntryPattern, ""
+00017320: 2c20 7573 6572 496e 7075 7429 2023 2072  , userInput) # r
+00017330: 656d 6f76 6520 7370 6563 6961 6c20 656e  emove special en
+00017340: 7472 7920 7465 6d70 6f72 6172 696c 790a  try temporarily.
+00017350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017360: 2020 2020 6966 2075 7365 7249 6e70 7574      if userInput
+00017370: 2061 6e64 2063 6f6e 6669 672e 6469 7370   and config.disp
+00017380: 6c61 7949 6d70 726f 7665 6457 7269 7469  layImprovedWriti
+00017390: 6e67 3a0a 2020 2020 2020 2020 2020 2020  ng:.            
+000173a0: 2020 2020 2020 2020 2020 2020 7573 6572              user
+000173b0: 496e 7075 7420 3d20 7265 2e73 7562 2822  Input = re.sub("
+000173c0: 5c6e 5c5b 4375 7272 656e 7420 7469 6d65  \n\[Current time
+000173d0: 3a20 5b5e 5c6e 5d2a 3f24 222c 2022 222c  : [^\n]*?$", "",
+000173e0: 2075 7365 7249 6e70 7574 290a 2020 2020   userInput).    
+000173f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017400: 2020 2020 6966 2063 6f6e 6669 672e 6973      if config.is
+00017410: 5465 726d 7578 3a0a 2020 2020 2020 2020  Termux:.        
+00017420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017430: 2020 2020 6461 795f 6f66 5f77 6565 6b20      day_of_week 
+00017440: 3d20 2222 0a20 2020 2020 2020 2020 2020  = "".           
+00017450: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+00017460: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00017470: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00017480: 6179 5f6f 665f 7765 656b 203d 2066 2274  ay_of_week = f"t
+00017490: 6f64 6179 2069 7320 7b67 6574 4461 794f  oday is {getDayO
+000174a0: 6657 6565 6b28 297d 2061 6e64 2022 0a20  fWeek()} and ". 
 000174b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000174c0: 2020 2069 6620 7370 6563 6961 6c45 6e74     if specialEnt
-000174d0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-000174e0: 2020 2020 2020 2020 2020 2020 7573 6572              user
-000174f0: 496e 7075 7420 3d20 6622 7b75 7365 7249  Input = f"{userI
-00017500: 6e70 7574 7d7b 7370 6563 6961 6c45 6e74  nput}{specialEnt
-00017510: 7279 7d22 0a20 2020 2020 2020 2020 2020  ry}".           
-00017520: 2020 2020 2020 2020 2023 2072 6566 696e           # refin
-00017530: 6520 6d65 7373 6167 6573 2062 6566 6f72  e messages befor
-00017540: 6520 7275 6e6e 696e 6720 636f 6d70 6c65  e running comple
-00017550: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00017560: 2020 2020 2020 2020 2066 696e 6554 756e           fineTun
-00017570: 6564 5573 6572 496e 7075 7420 3d20 7365  edUserInput = se
-00017580: 6c66 2e66 696e 6554 756e 6555 7365 7249  lf.fineTuneUserI
-00017590: 6e70 7574 2875 7365 7249 6e70 7574 290a  nput(userInput).
-000175a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175b0: 2020 2020 2320 696e 2063 6173 6520 6f66      # in case of
-000175c0: 2074 7261 6e73 6c61 7469 6f6e 0a20 2020   translation.   
-000175d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000175e0: 2069 6620 636f 6e66 6967 2e70 7265 6465   if config.prede
-000175f0: 6669 6e65 6443 6f6e 7465 7874 203d 3d20  finedContext == 
-00017600: 224c 6574 206d 6520 5472 616e 736c 6174  "Let me Translat
-00017610: 6522 2061 6e64 2066 696e 6554 756e 6564  e" and fineTuned
-00017620: 5573 6572 496e 7075 742e 7374 6172 7473  UserInput.starts
-00017630: 7769 7468 2822 4173 7369 7374 206d 6520  with("Assist me 
-00017640: 6279 2061 6374 696e 6720 6173 2061 2074  by acting as a t
-00017650: 7261 6e73 6c61 746f 722e 5c6e 506c 6561  ranslator.\nPlea
-00017660: 7365 2074 7261 6e73 6c61 7465 2229 3a0a  se translate"):.
-00017670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017680: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
-00017690: 506c 6561 7365 2073 7065 6369 6679 2062  Please specify b
-000176a0: 656c 6f77 2074 6865 206c 616e 6775 6167  elow the languag
-000176b0: 6520 796f 7520 776f 756c 6420 6c69 6b65  e you would like
-000176c0: 2074 6865 2063 6f6e 7465 6e74 2074 6f20   the content to 
-000176d0: 6265 2074 7261 6e73 6c61 7465 6420 696e  be translated in
-000176e0: 746f 3a22 290a 2020 2020 2020 2020 2020  to:").          
-000176f0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00017700: 6e67 7561 6765 203d 2073 656c 662e 7072  nguage = self.pr
-00017710: 6f6d 7074 732e 7369 6d70 6c65 5072 6f6d  ompts.simpleProm
-00017720: 7074 2873 7479 6c65 3d73 656c 662e 7072  pt(style=self.pr
-00017730: 6f6d 7074 732e 7072 6f6d 7074 5374 796c  ompts.promptStyl
-00017740: 6532 2c20 6465 6661 756c 743d 636f 6e66  e2, default=conf
-00017750: 6967 2e74 7261 6e73 6c61 7465 546f 4c61  ig.translateToLa
-00017760: 6e67 7561 6765 290a 2020 2020 2020 2020  nguage).        
+000174c0: 2020 2020 2020 2069 6d70 726f 7665 6456         improvedV
+000174d0: 6572 7369 6f6e 203d 2043 616c 6c4c 4c4d  ersion = CallLLM
+000174e0: 2e67 6574 5369 6e67 6c65 4368 6174 5265  .getSingleChatRe
+000174f0: 7370 6f6e 7365 2866 2222 2249 6d70 726f  sponse(f"""Impro
+00017500: 7665 2074 6865 2066 6f6c 6c6f 7769 6e67  ve the following
+00017510: 2077 7269 7469 6e67 2c20 6163 636f 7264   writing, accord
+00017520: 696e 6720 746f 207b 636f 6e66 6967 2e69  ing to {config.i
+00017530: 6d70 726f 7665 6457 7269 7469 6e67 5379  mprovedWritingSy
+00017540: 746c 657d 0a49 6e20 6164 6469 7469 6f6e  tle}.In addition
+00017550: 2c20 4920 776f 756c 6420 6c69 6b65 2079  , I would like y
+00017560: 6f75 2074 6f20 6865 6c70 206d 6520 7769  ou to help me wi
+00017570: 7468 2063 6f6e 7665 7274 696e 6720 7265  th converting re
+00017580: 6c61 7469 7665 2064 6174 6573 2061 6e64  lative dates and
+00017590: 2074 696d 6573 2c20 6966 2061 6e79 2c20   times, if any, 
+000175a0: 696e 746f 2065 7861 6374 2064 6174 6573  into exact dates
+000175b0: 2061 6e64 2074 696d 6573 2062 6173 6564   and times based
+000175c0: 206f 6e20 7468 6520 7265 6665 7265 6e63   on the referenc
+000175d0: 6520 7468 6174 207b 6461 795f 6f66 5f77  e that {day_of_w
+000175e0: 6565 6b7d 6375 7272 656e 7420 6461 7465  eek}current date
+000175f0: 7469 6d65 2069 7320 7b73 7472 2864 6174  time is {str(dat
+00017600: 6574 696d 652e 6461 7465 7469 6d65 2e6e  etime.datetime.n
+00017610: 6f77 2829 297d 2e0a 5265 6d65 6d62 6572  ow())}..Remember
+00017620: 2c20 7072 6f76 6964 6520 6d65 2077 6974  , provide me wit
+00017630: 6820 7468 6520 696d 7072 6f76 6564 2077  h the improved w
+00017640: 7269 7469 6e67 206f 6e6c 792c 2065 6e63  riting only, enc
+00017650: 6c6f 7365 6420 696e 2074 7269 706c 6520  losed in triple 
+00017660: 7175 6f74 6573 2060 6060 2061 6e64 2077  quotes ``` and w
+00017670: 6974 686f 7574 2061 6e79 2061 6464 6974  ithout any addit
+00017680: 696f 6e61 6c20 696e 666f 726d 6174 696f  ional informatio
+00017690: 6e20 6f72 2063 6f6d 6d65 6e74 732e 0a4d  n or comments..M
+000176a0: 7920 7772 6974 696e 673a 0a7b 7573 6572  y writing:.{user
+000176b0: 496e 7075 747d 2222 2229 0a20 2020 2020  Input}""").     
+000176c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000176d0: 2020 2069 6620 696d 7072 6f76 6564 5665     if improvedVe
+000176e0: 7273 696f 6e20 616e 6420 696d 7072 6f76  rsion and improv
+000176f0: 6564 5665 7273 696f 6e2e 7374 6172 7473  edVersion.starts
+00017700: 7769 7468 2822 6060 6022 2920 616e 6420  with("```") and 
+00017710: 696d 7072 6f76 6564 5665 7273 696f 6e2e  improvedVersion.
+00017720: 656e 6473 7769 7468 2822 6060 6022 293a  endswith("```"):
+00017730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017740: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+00017750: 6e74 3128 696d 7072 6f76 6564 5665 7273  nt1(improvedVers
+00017760: 696f 6e29 0a20 2020 2020 2020 2020 2020  ion).           
 00017770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017780: 6966 206c 616e 6775 6167 6520 616e 6420  if language and 
-00017790: 6e6f 7420 6c61 6e67 7561 6765 2e73 7472  not language.str
-000177a0: 6970 2829 2e6c 6f77 6572 2829 2069 6e20  ip().lower() in 
-000177b0: 2863 6f6e 6669 672e 6361 6e63 656c 5f65  (config.cancel_e
-000177c0: 6e74 7279 2c20 636f 6e66 6967 2e65 7869  ntry, config.exi
-000177d0: 745f 656e 7472 7929 3a0a 2020 2020 2020  t_entry):.      
+00017780: 2075 7365 7249 6e70 7574 203d 2069 6d70   userInput = imp
+00017790: 726f 7665 6456 6572 7369 6f6e 5b33 3a2d  rovedVersion[3:-
+000177a0: 335d 0a20 2020 2020 2020 2020 2020 2020  3].             
+000177b0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000177c0: 6620 636f 6e66 6967 2e74 7473 4f75 7470  f config.ttsOutp
+000177d0: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
 000177e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000177f0: 2020 2020 2020 6669 6e65 5475 6e65 6455        fineTunedU
-00017800: 7365 7249 6e70 7574 203d 2066 227b 6669  serInput = f"{fi
-00017810: 6e65 5475 6e65 6455 7365 7249 6e70 7574  neTunedUserInput
-00017820: 7d5c 6e5c 6e50 6c65 6173 6520 7472 616e  }\n\nPlease tran
-00017830: 736c 6174 6520 7468 6520 636f 6e74 656e  slate the conten
-00017840: 7420 696e 746f 203c 6c61 6e67 7561 6765  t into <language
-00017850: 3e7b 6c61 6e67 7561 6765 7d3c 2f6c 616e  >{language}</lan
-00017860: 6775 6167 653e 2e22 0a20 2020 2020 2020  guage>.".       
-00017870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017880: 2020 2020 2063 6f6e 6669 672e 7472 616e       config.tran
-00017890: 736c 6174 6554 6f4c 616e 6775 6167 6520  slateToLanguage 
-000178a0: 3d20 6c61 6e67 7561 6765 0a20 2020 2020  = language.     
-000178b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178c0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000178d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178e0: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
-000178f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017900: 2020 2320 636c 6561 7220 636f 6e66 6967    # clear config
-00017910: 2e70 7265 6465 6669 6e65 6443 6f6e 7465  .predefinedConte
-00017920: 7874 5465 6d70 2069 6620 616e 790a 2020  xtTemp if any.  
-00017930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017940: 2020 6966 2063 6f6e 6669 672e 7072 6564    if config.pred
-00017950: 6566 696e 6564 436f 6e74 6578 7454 656d  efinedContextTem
-00017960: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
-00017970: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00017980: 672e 7072 6564 6566 696e 6564 436f 6e74  g.predefinedCont
-00017990: 6578 7420 3d20 636f 6e66 6967 2e70 7265  ext = config.pre
-000179a0: 6465 6669 6e65 6443 6f6e 7465 7874 5465  definedContextTe
-000179b0: 6d70 0a20 2020 2020 2020 2020 2020 2020  mp.             
-000179c0: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-000179d0: 672e 7072 6564 6566 696e 6564 436f 6e74  g.predefinedCont
-000179e0: 6578 7454 656d 7020 3d20 2222 0a20 2020  extTemp = "".   
-000179f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a00: 2023 2065 6d70 7479 2063 6f6e 6669 672e   # empty config.
-00017a10: 7061 6765 7243 6f6e 7465 6e74 0a20 2020  pagerContent.   
-00017a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017a30: 2063 6f6e 6669 672e 7061 6765 7243 6f6e   config.pagerCon
-00017a40: 7465 6e74 203d 2022 220a 0a20 2020 2020  tent = ""..     
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00017a60: 2063 6865 636b 2073 7065 6369 616c 2065   check special e
-00017a70: 6e74 7269 6573 0a20 2020 2020 2020 2020  ntries.         
-00017a80: 2020 2020 2020 2020 2020 2023 2069 6620             # if 
-00017a90: 7573 6572 2063 616c 6c20 6120 6368 6174  user call a chat
-00017aa0: 626f 7420 7769 7468 6f75 7420 6675 6e63  bot without func
-00017ab0: 7469 6f6e 2063 616c 6c69 6e67 0a20 2020  tion calling.   
-00017ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ad0: 2069 6620 225b 4348 4154 5d22 2069 6e20   if "[CHAT]" in 
-00017ae0: 6669 6e65 5475 6e65 6455 7365 7249 6e70  fineTunedUserInp
-00017af0: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
-00017b00: 2020 2020 2020 2020 2020 2020 6368 6174              chat
-00017b10: 626f 7420 3d20 636f 6e66 6967 2e6c 6c6d  bot = config.llm
-00017b20: 496e 7465 7266 6163 650a 2020 2020 2020  Interface.      
-00017b30: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00017b40: 6966 2063 616c 6c43 6861 7442 6f74 203a  if callChatBot :
-00017b50: 3d20 7265 2e73 6561 7263 6828 225c 5b43  = re.search("\[C
-00017b60: 4841 545f 285b 5e5c 5b5c 5d5d 2b3f 295c  HAT_([^\[\]]+?)\
-00017b70: 5d22 2c20 6669 6e65 5475 6e65 6455 7365  ]", fineTunedUse
-00017b80: 7249 6e70 7574 293a 0a20 2020 2020 2020  rInput):.       
-00017b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ba0: 2063 6861 7462 6f74 203d 2063 616c 6c43   chatbot = callC
-00017bb0: 6861 7442 6f74 2e67 726f 7570 2831 292e  hatBot.group(1).
-00017bc0: 6c6f 7765 7228 2920 6966 2063 616c 6c43  lower() if callC
-00017bd0: 6861 7442 6f74 2061 6e64 2063 616c 6c43  hatBot and callC
-00017be0: 6861 7442 6f74 2e67 726f 7570 2831 292e  hatBot.group(1).
-00017bf0: 6c6f 7765 7228 2920 696e 2028 2263 6861  lower() in ("cha
-00017c00: 7467 7074 222c 2022 6765 6d69 6e69 7072  tgpt", "geminipr
-00017c10: 6f22 2c20 2270 616c 6d32 222c 2022 636f  o", "palm2", "co
-00017c20: 6465 7922 2920 656c 7365 2022 220a 2020  dey") else "".  
+000177f0: 2020 2020 5454 5355 7469 6c2e 706c 6179      TTSUtil.play
+00017800: 2875 7365 7249 6e70 7574 290a 2020 2020  (userInput).    
+00017810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017820: 6966 2073 7065 6369 616c 456e 7472 793a  if specialEntry:
+00017830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017840: 2020 2020 2020 2020 2075 7365 7249 6e70           userInp
+00017850: 7574 203d 2066 227b 7573 6572 496e 7075  ut = f"{userInpu
+00017860: 747d 7b73 7065 6369 616c 456e 7472 797d  t}{specialEntry}
+00017870: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+00017880: 2020 2020 2020 2320 7265 6669 6e65 206d        # refine m
+00017890: 6573 7361 6765 7320 6265 666f 7265 2072  essages before r
+000178a0: 756e 6e69 6e67 2063 6f6d 706c 6574 696f  unning completio
+000178b0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
+000178c0: 2020 2020 2020 6669 6e65 5475 6e65 6455        fineTunedU
+000178d0: 7365 7249 6e70 7574 203d 2073 656c 662e  serInput = self.
+000178e0: 6669 6e65 5475 6e65 5573 6572 496e 7075  fineTuneUserInpu
+000178f0: 7428 7573 6572 496e 7075 7429 0a20 2020  t(userInput).   
+00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017910: 2023 2069 6e20 6361 7365 206f 6620 7472   # in case of tr
+00017920: 616e 736c 6174 696f 6e0a 2020 2020 2020  anslation.      
+00017930: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017940: 2063 6f6e 6669 672e 7072 6564 6566 696e   config.predefin
+00017950: 6564 436f 6e74 6578 7420 3d3d 2022 4c65  edContext == "Le
+00017960: 7420 6d65 2054 7261 6e73 6c61 7465 2220  t me Translate" 
+00017970: 616e 6420 6669 6e65 5475 6e65 6455 7365  and fineTunedUse
+00017980: 7249 6e70 7574 2e73 7461 7274 7377 6974  rInput.startswit
+00017990: 6828 2241 7373 6973 7420 6d65 2062 7920  h("Assist me by 
+000179a0: 6163 7469 6e67 2061 7320 6120 7472 616e  acting as a tran
+000179b0: 736c 6174 6f72 2e5c 6e50 6c65 6173 6520  slator.\nPlease 
+000179c0: 7472 616e 736c 6174 6522 293a 0a20 2020  translate"):.   
+000179d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000179e0: 2020 2020 2070 7269 6e74 3128 2250 6c65       print1("Ple
+000179f0: 6173 6520 7370 6563 6966 7920 6265 6c6f  ase specify belo
+00017a00: 7720 7468 6520 6c61 6e67 7561 6765 2079  w the language y
+00017a10: 6f75 2077 6f75 6c64 206c 696b 6520 7468  ou would like th
+00017a20: 6520 636f 6e74 656e 7420 746f 2062 6520  e content to be 
+00017a30: 7472 616e 736c 6174 6564 2069 6e74 6f3a  translated into:
+00017a40: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00017a50: 2020 2020 2020 2020 2020 206c 616e 6775             langu
+00017a60: 6167 6520 3d20 7365 6c66 2e70 726f 6d70  age = self.promp
+00017a70: 7473 2e73 696d 706c 6550 726f 6d70 7428  ts.simplePrompt(
+00017a80: 7374 796c 653d 7365 6c66 2e70 726f 6d70  style=self.promp
+00017a90: 7473 2e70 726f 6d70 7453 7479 6c65 322c  ts.promptStyle2,
+00017aa0: 2064 6566 6175 6c74 3d63 6f6e 6669 672e   default=config.
+00017ab0: 7472 616e 736c 6174 6554 6f4c 616e 6775  translateToLangu
+00017ac0: 6167 6529 0a20 2020 2020 2020 2020 2020  age).           
+00017ad0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00017ae0: 6c61 6e67 7561 6765 2061 6e64 206e 6f74  language and not
+00017af0: 206c 616e 6775 6167 652e 7374 7269 7028   language.strip(
+00017b00: 292e 6c6f 7765 7228 2920 696e 2028 636f  ).lower() in (co
+00017b10: 6e66 6967 2e63 616e 6365 6c5f 656e 7472  nfig.cancel_entr
+00017b20: 792c 2063 6f6e 6669 672e 6578 6974 5f65  y, config.exit_e
+00017b30: 6e74 7279 293a 0a20 2020 2020 2020 2020  ntry):.         
+00017b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b50: 2020 2066 696e 6554 756e 6564 5573 6572     fineTunedUser
+00017b60: 496e 7075 7420 3d20 6622 7b66 696e 6554  Input = f"{fineT
+00017b70: 756e 6564 5573 6572 496e 7075 747d 5c6e  unedUserInput}\n
+00017b80: 5c6e 506c 6561 7365 2074 7261 6e73 6c61  \nPlease transla
+00017b90: 7465 2074 6865 2063 6f6e 7465 6e74 2069  te the content i
+00017ba0: 6e74 6f20 3c6c 616e 6775 6167 653e 7b6c  nto <language>{l
+00017bb0: 616e 6775 6167 657d 3c2f 6c61 6e67 7561  anguage}</langua
+00017bc0: 6765 3e2e 220a 2020 2020 2020 2020 2020  ge>.".          
+00017bd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017be0: 2020 636f 6e66 6967 2e74 7261 6e73 6c61    config.transla
+00017bf0: 7465 546f 4c61 6e67 7561 6765 203d 206c  teToLanguage = l
+00017c00: 616e 6775 6167 650a 2020 2020 2020 2020  anguage.        
+00017c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017c20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
 00017c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00017c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c60: 6368 6174 626f 7420 3d20 2222 0a20 2020  chatbot = "".   
-00017c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017c80: 2069 6620 6368 6174 626f 743a 0a20 2020   if chatbot:.   
-00017c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ca0: 2020 2020 2023 2063 616c 6c20 7468 6520       # call the 
-00017cb0: 7370 6369 6669 6564 2063 6861 7462 6f74  spcified chatbot
-00017cc0: 2074 6f20 636f 6e74 696e 7565 2074 6865   to continue the
-00017cd0: 2063 6f6e 7665 7273 6174 696f 6e0a 2020   conversation.  
-00017ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017cf0: 2020 2020 2020 6669 6e65 5475 6e65 6455        fineTunedU
-00017d00: 7365 7249 6e70 7574 203d 2072 652e 7375  serInput = re.su
-00017d10: 6228 225c 5b43 4841 545c 5d7c 5c5b 4348  b("\[CHAT\]|\[CH
-00017d20: 4154 5f5b 5e5c 5b5c 5d5d 2b3f 5c5d 222c  AT_[^\[\]]+?\]",
-00017d30: 2022 222c 2066 696e 6554 756e 6564 5573   "", fineTunedUs
-00017d40: 6572 496e 7075 7429 0a20 2020 2020 2020  erInput).       
-00017d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017d60: 2073 656c 662e 6c61 756e 6368 4368 6174   self.launchChat
-00017d70: 626f 7428 6368 6174 626f 742c 2066 696e  bot(chatbot, fin
-00017d80: 6554 756e 6564 5573 6572 496e 7075 7429  eTunedUserInput)
-00017d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017da0: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-00017db0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00017dc0: 2020 2020 2020 2320 7768 656e 2075 7365        # when use
-00017dd0: 7220 646f 6e27 7420 7761 6e74 2061 2066  r don't want a f
-00017de0: 756e 6374 696f 6e20 6361 6c6c 0a20 2020  unction call.   
-00017df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017e00: 206e 6f46 756e 6374 696f 6e43 616c 6c20   noFunctionCall 
-00017e10: 3d20 2822 5b4e 4f5f 544f 4f4c 5d22 2069  = ("[NO_TOOL]" i
-00017e20: 6e20 6669 6e65 5475 6e65 6455 7365 7249  n fineTunedUserI
-00017e30: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
-00017e40: 2020 2020 2020 2020 2020 2320 7768 656e            # when
-00017e50: 2075 7365 7220 7761 6e74 2074 6f20 6361   user want to ca
-00017e60: 6c6c 2061 2070 6172 7469 6375 6c61 7220  ll a particular 
-00017e70: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
-00017e80: 2020 2020 2020 2020 2020 2020 2063 6865               che
-00017e90: 636b 4361 6c6c 5370 6563 6966 6963 4675  ckCallSpecificFu
-00017ea0: 6e63 7469 6f6e 203d 2072 652e 7365 6172  nction = re.sear
-00017eb0: 6368 2822 5c5b 544f 4f4c 5f28 5b5e 5c5b  ch("\[TOOL_([^\[
-00017ec0: 5c5d 5d2b 3f29 5c5d 222c 2066 696e 6554  \]]+?)\]", fineT
-00017ed0: 756e 6564 5573 6572 496e 7075 7429 0a20  unedUserInput). 
-00017ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017ef0: 2020 2063 6f6e 6669 672e 7365 6c65 6374     config.select
-00017f00: 6564 546f 6f6c 203d 2063 6865 636b 4361  edTool = checkCa
-00017f10: 6c6c 5370 6563 6966 6963 4675 6e63 7469  llSpecificFuncti
-00017f20: 6f6e 2e67 726f 7570 2831 2920 6966 2063  on.group(1) if c
-00017f30: 6865 636b 4361 6c6c 5370 6563 6966 6963  heckCallSpecific
-00017f40: 4675 6e63 7469 6f6e 2061 6e64 2063 6865  Function and che
-00017f50: 636b 4361 6c6c 5370 6563 6966 6963 4675  ckCallSpecificFu
-00017f60: 6e63 7469 6f6e 2e67 726f 7570 2831 2920  nction.group(1) 
-00017f70: 696e 2063 6f6e 6669 672e 746f 6f6c 4675  in config.toolFu
-00017f80: 6e63 7469 6f6e 4d65 7468 6f64 7320 656c  nctionMethods el
-00017f90: 7365 2022 220a 2020 2020 2020 2020 2020  se "".          
-00017fa0: 2020 2020 2020 2020 2020 6966 2063 6f6e            if con
-00017fb0: 6669 672e 6465 7665 6c6f 7065 7220 616e  fig.developer an
-00017fc0: 6420 636f 6e66 6967 2e73 656c 6563 7465  d config.selecte
-00017fd0: 6454 6f6f 6c3a 0a20 2020 2020 2020 2020  dTool:.         
-00017fe0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00017ff0: 7072 696e 7431 2866 2263 616c 6c69 6e67  print1(f"calling
-00018000: 2066 756e 6374 696f 6e20 277b 636f 6e66   function '{conf
-00018010: 6967 2e73 656c 6563 7465 6454 6f6f 6c7d  ig.selectedTool}
-00018020: 2720 2e2e 2e22 290a 2020 2020 2020 2020  ' ...").        
-00018030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018040: 7072 696e 745f 666f 726d 6174 7465 645f  print_formatted_
-00018050: 7465 7874 2848 544d 4c28 6622 3c7b 636f  text(HTML(f"<{co
-00018060: 6e66 6967 2e74 6572 6d69 6e61 6c50 726f  nfig.terminalPro
-00018070: 6d70 7449 6e64 6963 6174 6f72 436f 6c6f  mptIndicatorColo
-00018080: 7232 7d3e 4361 6c6c 696e 6720 6675 6e63  r2}>Calling func
-00018090: 7469 6f6e 3c2f 7b63 6f6e 6669 672e 7465  tion</{config.te
-000180a0: 726d 696e 616c 5072 6f6d 7074 496e 6469  rminalPromptIndi
-000180b0: 6361 746f 7243 6f6c 6f72 327d 3e20 3c7b  catorColor2}> <{
-000180c0: 636f 6e66 6967 2e74 6572 6d69 6e61 6c43  config.terminalC
-000180d0: 6f6d 6d61 6e64 456e 7472 7943 6f6c 6f72  ommandEntryColor
-000180e0: 327d 3e27 7b63 6f6e 6669 672e 7365 6c65  2}>'{config.sele
-000180f0: 6374 6564 546f 6f6c 7d27 3c2f 7b63 6f6e  ctedTool}'</{con
-00018100: 6669 672e 7465 726d 696e 616c 436f 6d6d  fig.terminalComm
-00018110: 616e 6445 6e74 7279 436f 6c6f 7232 7d3e  andEntryColor2}>
-00018120: 203c 7b63 6f6e 6669 672e 7465 726d 696e   <{config.termin
-00018130: 616c 5072 6f6d 7074 496e 6469 6361 746f  alPromptIndicato
-00018140: 7243 6f6c 6f72 327d 3e2e 2e2e 3c2f 7b63  rColor2}>...</{c
-00018150: 6f6e 6669 672e 7465 726d 696e 616c 5072  onfig.terminalPr
-00018160: 6f6d 7074 496e 6469 6361 746f 7243 6f6c  omptIndicatorCol
-00018170: 6f72 327d 3e22 2929 0a20 2020 2020 2020  or2}>")).       
-00018180: 2020 2020 2020 2020 2020 2020 2066 696e               fin
-00018190: 6554 756e 6564 5573 6572 496e 7075 7420  eTunedUserInput 
-000181a0: 3d20 7265 2e73 7562 2873 7065 6369 616c  = re.sub(special
-000181b0: 456e 7472 7950 6174 7465 726e 2c20 2222  EntryPattern, ""
-000181c0: 2c20 6669 6e65 5475 6e65 6455 7365 7249  , fineTunedUserI
-000181d0: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
-000181e0: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-000181f0: 2e63 7572 7265 6e74 4d65 7373 6167 6573  .currentMessages
-00018200: 2e61 7070 656e 6428 7b22 726f 6c65 223a  .append({"role":
-00018210: 2022 7573 6572 222c 2022 636f 6e74 656e   "user", "conten
-00018220: 7422 3a20 6669 6e65 5475 6e65 6455 7365  t": fineTunedUse
-00018230: 7249 6e70 7574 7d29 0a0a 2020 2020 2020  rInput})..      
-00018240: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00018250: 7374 6172 7420 7370 696e 6e69 6e67 0a20  start spinning. 
-00018260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018270: 2020 2063 6f6e 6669 672e 7374 6f70 5f65     config.stop_e
-00018280: 7665 6e74 203d 2074 6872 6561 6469 6e67  vent = threading
-00018290: 2e45 7665 6e74 2829 0a20 2020 2020 2020  .Event().       
-000182a0: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-000182b0: 6669 672e 7370 696e 6e65 725f 7468 7265  fig.spinner_thre
-000182c0: 6164 203d 2074 6872 6561 6469 6e67 2e54  ad = threading.T
-000182d0: 6872 6561 6428 7461 7267 6574 3d73 7069  hread(target=spi
-000182e0: 6e6e 696e 675f 616e 696d 6174 696f 6e2c  nning_animation,
-000182f0: 2061 7267 733d 2863 6f6e 6669 672e 7374   args=(config.st
-00018300: 6f70 5f65 7665 6e74 2c29 290a 2020 2020  op_event,)).    
-00018310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018320: 636f 6e66 6967 2e73 7069 6e6e 6572 5f74  config.spinner_t
-00018330: 6872 6561 642e 7374 6172 7428 290a 0a20  hread.start().. 
-00018340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018350: 2020 2023 2066 6f72 6365 206c 6f61 6469     # force loadi
-00018360: 6e67 2069 6e74 6572 6e65 7420 7365 6172  ng internet sear
-00018370: 6368 6573 0a20 2020 2020 2020 2020 2020  ches.           
-00018380: 2020 2020 2020 2020 2069 6620 636f 6e66           if conf
-00018390: 6967 2e6c 6f61 6469 6e67 496e 7465 726e  ig.loadingIntern
-000183a0: 6574 5365 6172 6368 6573 203d 3d20 2261  etSearches == "a
-000183b0: 6c77 6179 7322 3a0a 2020 2020 2020 2020  lways":.        
-000183c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183d0: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
-000183e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000183f0: 2063 6f6e 6669 672e 6375 7272 656e 744d   config.currentM
-00018400: 6573 7361 6765 7320 3d20 4361 6c6c 4c4c  essages = CallLL
-00018410: 4d2e 7275 6e53 696e 676c 6546 756e 6374  M.runSingleFunct
-00018420: 696f 6e43 616c 6c28 636f 6e66 6967 2e63  ionCall(config.c
-00018430: 7572 7265 6e74 4d65 7373 6167 6573 2c20  urrentMessages, 
-00018440: 2269 6e74 6567 7261 7465 5f67 6f6f 676c  "integrate_googl
-00018450: 655f 7365 6172 6368 6573 2229 0a20 2020  e_searches").   
-00018460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018470: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-00018480: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018490: 2020 2020 2020 2020 2070 7269 6e74 3128           print1(
-000184a0: 2255 6e61 626c 6520 746f 206c 6f61 6420  "Unable to load 
-000184b0: 696e 7465 726e 6574 2072 6573 6f75 7263  internet resourc
-000184c0: 6573 2e22 290a 2020 2020 2020 2020 2020  es.").          
-000184d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000184e0: 2020 7368 6f77 4572 726f 7273 2829 0a0a    showErrors()..
-000184f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018500: 2020 2020 636f 6d70 6c65 7469 6f6e 203d      completion =
-00018510: 2043 616c 6c4c 4c4d 2e72 756e 4765 6e69   CallLLM.runGeni
-00018520: 7573 4361 6c6c 2863 6f6e 6669 672e 6375  usCall(config.cu
-00018530: 7272 656e 744d 6573 7361 6765 732c 206e  rrentMessages, n
-00018540: 6f46 756e 6374 696f 6e43 616c 6c29 0a20  oFunctionCall). 
-00018550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018560: 2020 200a 2020 2020 2020 2020 2020 2020     .            
-00018570: 2020 2020 2020 2020 2320 7374 6f70 2073          # stop s
-00018580: 7069 6e6e 696e 670a 2020 2020 2020 2020  pinning.        
-00018590: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-000185a0: 6967 2e72 756e 5079 7468 6f6e 203d 2054  ig.runPython = T
-000185b0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-000185c0: 2020 2020 2020 2020 7374 6f70 5370 696e          stopSpin
-000185d0: 6e69 6e67 2829 0a0a 2020 2020 2020 2020  ning()..        
-000185e0: 2020 2020 2020 2020 2020 2020 6966 2063              if c
-000185f0: 6f6d 706c 6574 696f 6e20 6973 206e 6f74  ompletion is not
-00018600: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00018610: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00018620: 2043 7265 6174 6520 6120 6e65 7720 7468   Create a new th
-00018630: 7265 6164 2066 6f72 2074 6865 2073 7472  read for the str
-00018640: 6561 6d69 6e67 2074 6173 6b0a 2020 2020  eaming task.    
-00018650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018660: 2020 2020 7374 7265 616d 696e 6757 6f72      streamingWor
-00018670: 6457 7261 7070 6572 203d 2053 7472 6561  dWrapper = Strea
-00018680: 6d69 6e67 576f 7264 5772 6170 7065 7228  mingWordWrapper(
-00018690: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000186a0: 2020 2020 2020 2020 2020 7374 7265 616d            stream
-000186b0: 696e 675f 6576 656e 7420 3d20 7468 7265  ing_event = thre
-000186c0: 6164 696e 672e 4576 656e 7428 290a 2020  ading.Event().  
-000186d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000186e0: 2020 2020 2020 7365 6c66 2e73 7472 6561        self.strea
-000186f0: 6d69 6e67 5f74 6872 6561 6420 3d20 7468  ming_thread = th
-00018700: 7265 6164 696e 672e 5468 7265 6164 2874  reading.Thread(t
-00018710: 6172 6765 743d 7374 7265 616d 696e 6757  arget=streamingW
-00018720: 6f72 6457 7261 7070 6572 2e73 7472 6561  ordWrapper.strea
-00018730: 6d4f 7574 7075 7473 2c20 6172 6773 3d28  mOutputs, args=(
-00018740: 7374 7265 616d 696e 675f 6576 656e 742c  streaming_event,
-00018750: 2063 6f6d 706c 6574 696f 6e2c 2054 7275   completion, Tru
-00018760: 6520 6966 2063 6f6e 6669 672e 6c6c 6d49  e if config.llmI
-00018770: 6e74 6572 6661 6365 2069 6e20 2822 6368  nterface in ("ch
-00018780: 6174 6770 7422 2c20 226c 6574 6d65 646f  atgpt", "letmedo
-00018790: 6974 2229 2065 6c73 6520 4661 6c73 6529  it") else False)
-000187a0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-000187b0: 2020 2020 2020 2020 2020 2320 5374 6172            # Star
-000187c0: 7420 7468 6520 7374 7265 616d 696e 6720  t the streaming 
-000187d0: 7468 7265 6164 0a20 2020 2020 2020 2020  thread.         
-000187e0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000187f0: 656c 662e 7374 7265 616d 696e 675f 7468  elf.streaming_th
-00018800: 7265 6164 2e73 7461 7274 2829 0a0a 2020  read.start()..  
-00018810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018820: 2020 2020 2020 2320 7761 6974 2077 6869        # wait whi
-00018830: 6c65 2074 6578 7420 6f75 7470 7574 2069  le text output i
-00018840: 7320 7374 6561 6d69 6e67 3b20 6361 7074  s steaming; capt
-00018850: 7572 6520 6b65 7920 636f 6d62 6f20 2763  ure key combo 'c
-00018860: 7472 6c2b 7127 206f 7220 2763 7472 6c2b  trl+q' or 'ctrl+
-00018870: 7a27 2074 6f20 7374 6f70 2074 6865 2073  z' to stop the s
-00018880: 7472 6561 6d69 6e67 0a20 2020 2020 2020  treaming.       
-00018890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188a0: 2073 7472 6561 6d69 6e67 576f 7264 5772   streamingWordWr
-000188b0: 6170 7065 722e 6b65 7954 6f53 746f 7053  apper.keyToStopS
-000188c0: 7472 6561 6d69 6e67 2873 7472 6561 6d69  treaming(streami
-000188d0: 6e67 5f65 7665 6e74 290a 0a20 2020 2020  ng_event)..     
-000188e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000188f0: 2020 2023 2077 6865 6e20 7374 7265 616d     # when stream
-00018900: 696e 6720 6973 2064 6f6e 6520 6f72 2077  ing is done or w
-00018910: 6865 6e20 7573 6572 2070 7265 7373 2022  hen user press "
-00018920: 6374 726c 2b71 220a 2020 2020 2020 2020  ctrl+q".        
-00018930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018940: 7365 6c66 2e73 7472 6561 6d69 6e67 5f74  self.streaming_t
-00018950: 6872 6561 642e 6a6f 696e 2829 0a0a 2020  hread.join()..  
-00018960: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00018970: 6572 726f 7220 636f 6465 733a 2068 7474  error codes: htt
-00018980: 7073 3a2f 2f70 6c61 7466 6f72 6d2e 6f70  ps://platform.op
-00018990: 656e 6169 2e63 6f6d 2f64 6f63 732f 6775  enai.com/docs/gu
-000189a0: 6964 6573 2f65 7272 6f72 2d63 6f64 6573  ides/error-codes
-000189b0: 2f70 7974 686f 6e2d 6c69 6272 6172 792d  /python-library-
-000189c0: 6572 726f 722d 7479 7065 730a 2020 2020  error-types.    
-000189d0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
-000189e0: 7074 206f 7065 6e61 692e 4150 4945 7272  pt openai.APIErr
-000189f0: 6f72 2061 7320 653a 0a20 2020 2020 2020  or as e:.       
-00018a00: 2020 2020 2020 2020 2020 2020 2073 746f               sto
-00018a10: 7053 7069 6e6e 696e 6728 290a 2020 2020  pSpinning().    
-00018a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018a30: 2348 616e 646c 6520 4150 4920 6572 726f  #Handle API erro
-00018a40: 7220 6865 7265 2c20 652e 672e 2072 6574  r here, e.g. ret
-00018a50: 7279 206f 7220 6c6f 670a 2020 2020 2020  ry or log.      
-00018a60: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00018a70: 696e 7431 2866 224f 7065 6e41 4920 4150  int1(f"OpenAI AP
-00018a80: 4920 7265 7475 726e 6564 2061 6e20 4150  I returned an AP
-00018a90: 4920 4572 726f 723a 207b 657d 2229 0a20  I Error: {e}"). 
-00018aa0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00018ab0: 7863 6570 7420 6f70 656e 6169 2e41 5049  xcept openai.API
-00018ac0: 436f 6e6e 6563 7469 6f6e 4572 726f 7220  ConnectionError 
-00018ad0: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-00018ae0: 2020 2020 2020 2020 2020 7374 6f70 5370            stopSp
-00018af0: 696e 6e69 6e67 2829 0a20 2020 2020 2020  inning().       
-00018b00: 2020 2020 2020 2020 2020 2020 2023 4861               #Ha
-00018b10: 6e64 6c65 2063 6f6e 6e65 6374 696f 6e20  ndle connection 
-00018b20: 6572 726f 7220 6865 7265 0a20 2020 2020  error here.     
-00018b30: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00018b40: 7269 6e74 3128 6622 4661 696c 6564 2074  rint1(f"Failed t
-00018b50: 6f20 636f 6e6e 6563 7420 746f 204f 7065  o connect to Ope
-00018b60: 6e41 4920 4150 493a 207b 657d 2229 0a20  nAI API: {e}"). 
-00018b70: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-00018b80: 7863 6570 7420 6f70 656e 6169 2e52 6174  xcept openai.Rat
-00018b90: 654c 696d 6974 4572 726f 7220 6173 2065  eLimitError as e
-00018ba0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00018bb0: 2020 2020 2020 7374 6f70 5370 696e 6e69        stopSpinni
-00018bc0: 6e67 2829 0a20 2020 2020 2020 2020 2020  ng().           
-00018bd0: 2020 2020 2020 2020 2023 4861 6e64 6c65           #Handle
-00018be0: 2072 6174 6520 6c69 6d69 7420 6572 726f   rate limit erro
-00018bf0: 7220 2877 6520 7265 636f 6d6d 656e 6420  r (we recommend 
-00018c00: 7573 696e 6720 6578 706f 6e65 6e74 6961  using exponentia
-00018c10: 6c20 6261 636b 6f66 6629 0a20 2020 2020  l backoff).     
-00018c20: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00018c30: 7269 6e74 3128 6622 4f70 656e 4149 2041  rint1(f"OpenAI A
-00018c40: 5049 2072 6571 7565 7374 2065 7863 6565  PI request excee
-00018c50: 6465 6420 7261 7465 206c 696d 6974 3a20  ded rate limit: 
-00018c60: 7b65 7d22 290a 2020 2020 2020 2020 2020  {e}").          
-00018c70: 2020 2020 2020 6578 6365 7074 3a0a 2020        except:.  
-00018c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018c90: 2020 7374 6f70 5370 696e 6e69 6e67 2829    stopSpinning()
-00018ca0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00018cb0: 2020 2020 2074 7261 6365 203d 2074 7261       trace = tra
-00018cc0: 6365 6261 636b 2e66 6f72 6d61 745f 6578  ceback.format_ex
-00018cd0: 6328 290a 2020 2020 2020 2020 2020 2020  c().            
-00018ce0: 2020 2020 2020 2020 6966 2022 506c 6561          if "Plea
-00018cf0: 7365 2072 6564 7563 6520 7468 6520 6c65  se reduce the le
-00018d00: 6e67 7468 206f 6620 7468 6520 6d65 7373  ngth of the mess
-00018d10: 6167 6573 206f 7220 636f 6d70 6c65 7469  ages or completi
-00018d20: 6f6e 2220 696e 2074 7261 6365 3a0a 2020  on" in trace:.  
-00018d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018d40: 2020 2020 2020 7072 696e 7431 2822 4d61        print1("Ma
-00018d50: 7869 6d75 6d20 746f 6b65 6e73 2072 6561  ximum tokens rea
-00018d60: 6368 6564 2122 290a 2020 2020 2020 2020  ched!").        
-00018d70: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-00018d80: 2063 6f6e 6669 672e 6465 7665 6c6f 7065   config.develope
-00018d90: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
-00018da0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00018db0: 3128 7365 6c66 2e64 6976 6964 6572 290a  1(self.divider).
-00018dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018dd0: 2020 2020 2020 2020 7072 696e 7431 2874          print1(t
-00018de0: 7261 6365 290a 2020 2020 2020 2020 2020  race).          
-00018df0: 2020 2020 2020 2020 2020 2020 2020 7072                pr
-00018e00: 696e 7431 2873 656c 662e 6469 7669 6465  int1(self.divide
-00018e10: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
-00018e20: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00018e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018e40: 2020 2020 2070 7269 6e74 3128 2245 7272       print1("Err
-00018e50: 6f72 2065 6e63 6f75 6e74 6572 6564 2122  or encountered!"
-00018e60: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-00018e70: 2020 2020 2020 2063 6f6e 6669 672e 6465         config.de
-00018e80: 6661 756c 7445 6e74 7279 203d 2075 7365  faultEntry = use
-00018e90: 7249 6e70 7574 0a20 2020 2020 2020 2020  rInput.         
-00018ea0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-00018eb0: 3128 2273 7461 7274 696e 6720 6120 6e65  1("starting a ne
-00018ec0: 7720 6368 6174 2122 290a 2020 2020 2020  w chat!").      
-00018ed0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00018ee0: 6c66 2e73 6176 6543 6861 7428 636f 6e66  lf.saveChat(conf
-00018ef0: 6967 2e63 7572 7265 6e74 4d65 7373 6167  ig.currentMessag
-00018f00: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
-00018f10: 2020 2020 2020 2020 7374 6f72 6167 6564          storaged
-00018f20: 6972 6563 746f 7279 2c20 636f 6e66 6967  irectory, config
-00018f30: 2e63 7572 7265 6e74 4d65 7373 6167 6573  .currentMessages
-00018f40: 203d 2073 7461 7274 4368 6174 2829 0a0a   = startChat()..
-00018f50: 2020 2020 6465 6620 6c61 756e 6368 4368      def launchCh
-00018f60: 6174 626f 7428 7365 6c66 2c20 6368 6174  atbot(self, chat
-00018f70: 626f 742c 2066 696e 6554 756e 6564 5573  bot, fineTunedUs
-00018f80: 6572 496e 7075 7429 3a0a 2020 2020 2020  erInput):.      
-00018f90: 2020 6966 206e 6f74 2063 6861 7462 6f74    if not chatbot
-00018fa0: 3a0a 2020 2020 2020 2020 2020 2020 6368  :.            ch
-00018fb0: 6174 626f 7420 3d20 636f 6e66 6967 2e6c  atbot = config.l
-00018fc0: 6c6d 496e 7465 7266 6163 650a 2020 2020  lmInterface.    
-00018fd0: 2020 2020 6966 2063 6f6e 6669 672e 6973      if config.is
-00018fe0: 5465 726d 7578 3a0a 2020 2020 2020 2020  Termux:.        
-00018ff0: 2020 2020 2363 6861 7462 6f74 203d 2022      #chatbot = "
-00019000: 6368 6174 6770 7422 0a20 2020 2020 2020  chatgpt".       
-00019010: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00019020: 2063 6861 7462 6f74 7320 3d20 7b0a 2020   chatbots = {.  
-00019030: 2020 2020 2020 2020 2020 226c 6c61 6d61            "llama
-00019040: 6370 7022 3a20 6c61 6d62 6461 3a20 4c6c  cpp": lambda: Ll
-00019050: 616d 6163 7070 4368 6174 286d 6f64 656c  amacppChat(model
-00019060: 3d4e 6f6e 6520 6966 2063 6f6e 6669 672e  =None if config.
-00019070: 7573 6541 6464 6974 696f 6e61 6c43 6861  useAdditionalCha
-00019080: 744d 6f64 656c 2065 6c73 6520 636f 6e66  tModel else conf
-00019090: 6967 2e6c 6c61 6d61 6370 704d 6169 6e4d  ig.llamacppMainM
-000190a0: 6f64 656c 292e 7275 6e28 6669 6e65 5475  odel).run(fineTu
-000190b0: 6e65 6455 7365 7249 6e70 7574 292c 0a20  nedUserInput),. 
-000190c0: 2020 2020 2020 2020 2020 2022 6f6c 6c61             "olla
-000190d0: 6d61 223a 206c 616d 6264 613a 204f 6c6c  ma": lambda: Oll
-000190e0: 616d 6143 6861 7428 292e 7275 6e28 6669  amaChat().run(fi
-000190f0: 6e65 5475 6e65 6455 7365 7249 6e70 7574  neTunedUserInput
-00019100: 2c20 6d6f 6465 6c3d 636f 6e66 6967 2e6f  , model=config.o
-00019110: 6c6c 616d 6143 6861 744d 6f64 656c 2069  llamaChatModel i
-00019120: 6620 636f 6e66 6967 2e75 7365 4164 6469  f config.useAddi
-00019130: 7469 6f6e 616c 4368 6174 4d6f 6465 6c20  tionalChatModel 
-00019140: 656c 7365 2063 6f6e 6669 672e 6f6c 6c61  else config.olla
-00019150: 6d61 4d61 696e 4d6f 6465 6c29 2c0a 2020  maMainModel),.  
-00019160: 2020 2020 2020 2020 2020 2263 6861 7467            "chatg
-00019170: 7074 223a 206c 616d 6264 613a 2043 6861  pt": lambda: Cha
-00019180: 7447 5054 2829 2e72 756e 2866 696e 6554  tGPT().run(fineT
-00019190: 756e 6564 5573 6572 496e 7075 7429 2c0a  unedUserInput),.
-000191a0: 2020 2020 2020 2020 2020 2020 226c 6574              "let
-000191b0: 6d65 646f 6974 223a 206c 616d 6264 613a  medoit": lambda:
-000191c0: 2043 6861 7447 5054 2829 2e72 756e 2866   ChatGPT().run(f
-000191d0: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
-000191e0: 7429 2c0a 2020 2020 2020 2020 2020 2020  t),.            
-000191f0: 2267 656d 696e 6922 3a20 6c61 6d62 6461  "gemini": lambda
-00019200: 3a20 4765 6d69 6e69 5072 6f28 7465 6d70  : GeminiPro(temp
-00019210: 6572 6174 7572 653d 636f 6e66 6967 2e6c  erature=config.l
-00019220: 6c6d 5465 6d70 6572 6174 7572 6529 2e72  lmTemperature).r
-00019230: 756e 2866 696e 6554 756e 6564 5573 6572  un(fineTunedUser
-00019240: 496e 7075 7429 2c0a 2020 2020 2020 2020  Input),.        
-00019250: 2020 2020 2267 656d 696e 6970 726f 223a      "geminipro":
-00019260: 206c 616d 6264 613a 2047 656d 696e 6950   lambda: GeminiP
-00019270: 726f 2874 656d 7065 7261 7475 7265 3d63  ro(temperature=c
-00019280: 6f6e 6669 672e 6c6c 6d54 656d 7065 7261  onfig.llmTempera
-00019290: 7475 7265 292e 7275 6e28 6669 6e65 5475  ture).run(fineTu
-000192a0: 6e65 6455 7365 7249 6e70 7574 292c 0a20  nedUserInput),. 
-000192b0: 2020 2020 2020 2020 2020 2022 7061 6c6d             "palm
-000192c0: 3222 3a20 6c61 6d62 6461 3a20 5061 6c6d  2": lambda: Palm
-000192d0: 3228 292e 7275 6e28 6669 6e65 5475 6e65  2().run(fineTune
-000192e0: 6455 7365 7249 6e70 7574 2c20 7465 6d70  dUserInput, temp
-000192f0: 6572 6174 7572 653d 636f 6e66 6967 2e6c  erature=config.l
-00019300: 6c6d 5465 6d70 6572 6174 7572 6529 2c0a  lmTemperature),.
-00019310: 2020 2020 2020 2020 2020 2020 2263 6f64              "cod
-00019320: 6579 223a 206c 616d 6264 613a 2043 6f64  ey": lambda: Cod
-00019330: 6579 2829 2e72 756e 2866 696e 6554 756e  ey().run(fineTun
-00019340: 6564 5573 6572 496e 7075 742c 2074 656d  edUserInput, tem
-00019350: 7065 7261 7475 7265 3d63 6f6e 6669 672e  perature=config.
-00019360: 6c6c 6d54 656d 7065 7261 7475 7265 292c  llmTemperature),
-00019370: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00019380: 2020 2069 6620 6368 6174 626f 7420 696e     if chatbot in
-00019390: 2063 6861 7462 6f74 733a 0a20 2020 2020   chatbots:.     
-000193a0: 2020 2020 2020 2063 6861 7462 6f74 735b         chatbots[
-000193b0: 6368 6174 626f 745d 2829 0a0a 2020 2020  chatbot]()..    
-000193c0: 6465 6620 6164 6450 6167 6572 5465 7874  def addPagerText
-000193d0: 2873 656c 662c 2074 6578 742c 2077 7261  (self, text, wra
-000193e0: 7057 6f72 6473 3d46 616c 7365 293a 0a20  pWords=False):. 
-000193f0: 2020 2020 2020 2069 6620 7772 6170 576f         if wrapWo
-00019400: 7264 733a 0a20 2020 2020 2020 2020 2020  rds:.           
-00019410: 2074 6578 7420 3d20 7365 6c66 2e67 6574   text = self.get
-00019420: 5772 6170 7065 6448 544d 4c54 6578 7428  WrappedHTMLText(
-00019430: 7465 7874 290a 2020 2020 2020 2020 636f  text).        co
-00019440: 6e66 6967 2e70 6167 6572 436f 6e74 656e  nfig.pagerConten
-00019450: 7420 2b3d 2066 227b 7465 7874 7d5c 6e22  t += f"{text}\n"
-00019460: 0a0a 2020 2020 6465 6620 6c61 756e 6368  ..    def launch
-00019470: 5061 6765 7228 7365 6c66 2c20 7061 6765  Pager(self, page
-00019480: 7243 6f6e 7465 6e74 3d4e 6f6e 6529 3a0a  rContent=None):.
-00019490: 2020 2020 2020 2020 6966 2070 6167 6572          if pager
-000194a0: 436f 6e74 656e 7420 6973 204e 6f6e 653a  Content is None:
-000194b0: 0a20 2020 2020 2020 2020 2020 2070 6167  .            pag
-000194c0: 6572 436f 6e74 656e 7420 3d20 636f 6e66  erContent = conf
-000194d0: 6967 2e70 6167 6572 436f 6e74 656e 740a  ig.pagerContent.
-000194e0: 2020 2020 2020 2020 6966 2070 6167 6572          if pager
-000194f0: 436f 6e74 656e 743a 0a20 2020 2020 2020  Content:.       
-00019500: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00019510: 2020 2020 2020 2020 2020 6966 2073 6875            if shu
-00019520: 7469 6c2e 7768 6963 6828 2262 6174 2229  til.which("bat")
-00019530: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019540: 2020 2020 2020 2320 5769 6e64 6f77 7320        # Windows 
-00019550: 7573 6572 7320 6361 6e20 696e 7374 616c  users can instal
-00019560: 6c20 6261 7420 636f 6d6d 616e 6420 7769  l bat command wi
-00019570: 7468 2073 636f 6f70 0a20 2020 2020 2020  th scoop.       
-00019580: 2020 2020 2020 2020 2020 2020 2023 2072               # r
-00019590: 6561 643a 2068 7474 7073 3a2f 2f67 6974  ead: https://git
-000195a0: 6875 622e 636f 6d2f 5363 6f6f 7049 6e73  hub.com/ScoopIns
-000195b0: 7461 6c6c 6572 2f53 636f 6f70 0a20 2020  taller/Scoop.   
-000195c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000195d0: 2023 203e 2069 7772 202d 7573 6562 2067   # > iwr -useb g
-000195e0: 6574 2e73 636f 6f70 2e73 6820 7c20 6965  et.scoop.sh | ie
-000195f0: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
-00019600: 2020 2020 2020 2320 3e20 7363 6f6f 7020        # > scoop 
-00019610: 696e 7374 616c 6c20 6172 6961 3220 6261  install aria2 ba
-00019620: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00019630: 2020 2020 2020 6966 2072 652e 7365 6172        if re.sear
-00019640: 6368 2822 3c5b 5e3c 3e5d 2b3f 3e22 2c20  ch("<[^<>]+?>", 
-00019650: 7061 6765 7243 6f6e 7465 6e74 293a 0a20  pagerContent):. 
-00019660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019670: 2020 2020 2020 2070 6167 6572 436f 6e74         pagerCont
-00019680: 656e 7420 3d20 5465 7874 5574 696c 2e63  ent = TextUtil.c
-00019690: 6f6e 7665 7274 4874 6d6c 5461 6754 6f43  onvertHtmlTagToC
-000196a0: 6f6c 6f72 616d 6128 7061 6765 7243 6f6e  olorama(pagerCon
-000196b0: 7465 6e74 290a 2020 2020 2020 2020 2020  tent).          
-000196c0: 2020 2020 2020 2020 2020 6c61 6e67 7561            langua
-000196d0: 6765 203d 2022 5079 7468 6f6e 2220 6966  ge = "Python" if
-000196e0: 2022 6060 6070 7974 686f 6e22 2069 6e20   "```python" in 
-000196f0: 7061 6765 7243 6f6e 7465 6e74 2065 6c73  pagerContent els
-00019700: 6520 224d 6172 6b64 6f77 6e22 0a20 2020  e "Markdown".   
-00019710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019720: 2070 7964 6f63 2e70 6970 6570 6167 6572   pydoc.pipepager
-00019730: 2870 6167 6572 436f 6e74 656e 742c 2063  (pagerContent, c
-00019740: 6d64 3d66 2262 6174 202d 6c20 7b6c 616e  md=f"bat -l {lan
-00019750: 6775 6167 657d 202d 2d70 6167 696e 6720  guage} --paging 
-00019760: 616c 7761 7973 2229 0a20 2020 2020 2020  always").       
-00019770: 2020 2020 2020 2020 2065 6c69 6620 7368           elif sh
-00019780: 7574 696c 2e77 6869 6368 2822 6c65 7373  util.which("less
-00019790: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000197a0: 2020 2020 2020 2020 2320 5769 6e64 6f77          # Window
-000197b0: 7320 7573 6572 7320 6361 6e20 696e 7374  s users can inst
-000197c0: 616c 6c20 6c65 7373 2063 6f6d 6d61 6e64  all less command
-000197d0: 2077 6974 6820 7363 6f6f 700a 2020 2020   with scoop.    
-000197e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000197f0: 2320 7265 6164 3a20 6874 7470 733a 2f2f  # read: https://
-00019800: 6769 7468 7562 2e63 6f6d 2f53 636f 6f70  github.com/Scoop
-00019810: 496e 7374 616c 6c65 722f 5363 6f6f 700a  Installer/Scoop.
-00019820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019830: 2020 2020 2320 3e20 6977 7220 2d75 7365      # > iwr -use
-00019840: 6220 6765 742e 7363 6f6f 702e 7368 207c  b get.scoop.sh |
-00019850: 2069 6578 0a20 2020 2020 2020 2020 2020   iex.           
-00019860: 2020 2020 2020 2020 2023 203e 2073 636f           # > sco
-00019870: 6f70 2069 6e73 7461 6c6c 2061 7269 6132  op install aria2
-00019880: 206c 6573 730a 2020 2020 2020 2020 2020   less.          
-00019890: 2020 2020 2020 2020 2020 6966 2072 652e            if re.
-000198a0: 7365 6172 6368 2822 3c5b 5e3c 3e5d 2b3f  search("<[^<>]+?
-000198b0: 3e22 2c20 7061 6765 7243 6f6e 7465 6e74  >", pagerContent
-000198c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-000198d0: 2020 2020 2020 2020 2020 2070 6167 6572             pager
-000198e0: 436f 6e74 656e 7420 3d20 5465 7874 5574  Content = TextUt
-000198f0: 696c 2e63 6f6e 7665 7274 4874 6d6c 5461  il.convertHtmlTa
-00019900: 6754 6f43 6f6c 6f72 616d 6128 7061 6765  gToColorama(page
-00019910: 7243 6f6e 7465 6e74 290a 2020 2020 2020  rContent).      
-00019920: 2020 2020 2020 2020 2020 2020 2020 7079                py
-00019930: 646f 632e 7069 7065 7061 6765 7228 7061  doc.pipepager(pa
-00019940: 6765 7243 6f6e 7465 6e74 2c20 636d 643d  gerContent, cmd=
-00019950: 276c 6573 7320 2d52 2729 0a20 2020 2020  'less -R').     
-00019960: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-00019970: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019980: 2020 2020 2070 7964 6f63 2e70 6167 6572       pydoc.pager
-00019990: 2870 6167 6572 436f 6e74 656e 7429 0a20  (pagerContent). 
-000199a0: 2020 2020 2020 2020 2020 2065 7863 6570             excep
-000199b0: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-000199c0: 2020 2063 6f6e 6669 672e 7061 6765 7256     config.pagerV
-000199d0: 6965 7720 3d20 4661 6c73 650a 2020 2020  iew = False.    
-000199e0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
-000199f0: 4572 726f 7273 2829 0a0a 2020 2020 2320  Errors()..    # 
-00019a00: 7772 6170 2068 746d 6c20 7465 7874 2061  wrap html text a
-00019a10: 7420 7370 6163 6573 0a20 2020 2064 6566  t spaces.    def
-00019a20: 2067 6574 5772 6170 7065 6448 544d 4c54   getWrappedHTMLT
-00019a30: 6578 7428 7365 6c66 2c20 7465 7874 2c20  ext(self, text, 
-00019a40: 7465 726d 696e 616c 5f77 6964 7468 3d4e  terminal_width=N
-00019a50: 6f6e 6529 3a0a 2020 2020 2020 2020 6966  one):.        if
-00019a60: 206e 6f74 2022 2022 2069 6e20 7465 7874   not " " in text
-00019a70: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00019a80: 7475 726e 2074 6578 740a 2020 2020 2020  turn text.      
-00019a90: 2020 6966 2074 6572 6d69 6e61 6c5f 7769    if terminal_wi
-00019aa0: 6474 6820 6973 204e 6f6e 653a 0a20 2020  dth is None:.   
-00019ab0: 2020 2020 2020 2020 2074 6572 6d69 6e61           termina
-00019ac0: 6c5f 7769 6474 6820 3d20 7368 7574 696c  l_width = shutil
-00019ad0: 2e67 6574 5f74 6572 6d69 6e61 6c5f 7369  .get_terminal_si
-00019ae0: 7a65 2829 2e63 6f6c 756d 6e73 0a20 2020  ze().columns.   
-00019af0: 2020 2020 2073 656c 662e 7772 6170 7065       self.wrappe
-00019b00: 6454 6578 7420 3d20 2222 0a20 2020 2020  dText = "".     
-00019b10: 2020 2073 656c 662e 6c69 6e65 5769 6474     self.lineWidt
-00019b20: 6820 3d20 300a 0a20 2020 2020 2020 2064  h = 0..        d
-00019b30: 6566 2061 6464 576f 7264 7328 776f 7264  ef addWords(word
-00019b40: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00019b50: 776f 7264 7320 3d20 776f 7264 732e 7370  words = words.sp
-00019b60: 6c69 7428 2220 2229 0a20 2020 2020 2020  lit(" ").       
-00019b70: 2020 2020 2066 6f72 2069 6e64 6578 2c20       for index, 
-00019b80: 6974 656d 2069 6e20 656e 756d 6572 6174  item in enumerat
-00019b90: 6528 776f 7264 7329 3a0a 2020 2020 2020  e(words):.      
-00019ba0: 2020 2020 2020 2020 2020 6973 4c61 7374            isLast
-00019bb0: 4974 656d 203d 2028 6c65 6e28 776f 7264  Item = (len(word
-00019bc0: 7329 202d 2069 6e64 6578 203d 3d20 3129  s) - index == 1)
-00019bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019be0: 2069 6620 6973 5f43 4a4b 2869 7465 6d29   if is_CJK(item)
-00019bf0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019c00: 2020 2020 2020 666f 7220 6949 6e64 6578        for iIndex
-00019c10: 2c20 6920 696e 2065 6e75 6d65 7261 7465  , i in enumerate
-00019c20: 2869 7465 6d29 3a0a 2020 2020 2020 2020  (item):.        
-00019c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c40: 6973 5370 6163 6549 7465 6d20 3d20 286e  isSpaceItem = (n
-00019c50: 6f74 2069 734c 6173 7449 7465 6d20 616e  ot isLastItem an
-00019c60: 6420 286c 656e 2869 7465 6d29 202d 2069  d (len(item) - i
-00019c70: 496e 6465 7820 3d3d 2031 2929 0a20 2020  Index == 1)).   
-00019c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019c90: 2020 2020 2069 5769 6474 6820 3d20 6765       iWidth = ge
-00019ca0: 7453 7472 696e 6757 6964 7468 2869 290a  tStringWidth(i).
-00019cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019cc0: 2020 2020 2020 2020 6966 2069 7353 7061          if isSpa
-00019cd0: 6365 4974 656d 3a0a 2020 2020 2020 2020  ceItem:.        
-00019ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019cf0: 2020 2020 6e65 774c 696e 6557 6964 7468      newLineWidth
-00019d00: 203d 2073 656c 662e 6c69 6e65 5769 6474   = self.lineWidt
-00019d10: 6820 2b20 6957 6964 7468 202b 2031 0a20  h + iWidth + 1. 
-00019d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d30: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00019d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d50: 2020 2020 2020 2020 206e 6577 4c69 6e65           newLine
-00019d60: 5769 6474 6820 3d20 7365 6c66 2e6c 696e  Width = self.lin
-00019d70: 6557 6964 7468 202b 2069 5769 6474 680a  eWidth + iWidth.
-00019d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019d90: 2020 2020 2020 2020 6966 206e 6577 4c69          if newLi
-00019da0: 6e65 5769 6474 6820 3e20 7465 726d 696e  neWidth > termin
-00019db0: 616c 5f77 6964 7468 3a0a 2020 2020 2020  al_width:.      
-00019dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019dd0: 2020 2020 2020 7365 6c66 2e77 7261 7070        self.wrapp
-00019de0: 6564 5465 7874 202b 3d20 6622 5c6e 7b69  edText += f"\n{i
-00019df0: 7d20 2220 6966 2069 7353 7061 6365 4974  } " if isSpaceIt
-00019e00: 656d 2065 6c73 6520 6622 5c6e 7b69 7d22  em else f"\n{i}"
-00019e10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019e20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019e30: 662e 6c69 6e65 5769 6474 6820 3d20 6957  f.lineWidth = iW
-00019e40: 6964 7468 202b 2031 2069 6620 6973 5370  idth + 1 if isSp
-00019e50: 6163 6549 7465 6d20 656c 7365 2069 5769  aceItem else iWi
-00019e60: 6474 680a 2020 2020 2020 2020 2020 2020  dth.            
-00019e70: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00019e80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019e90: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00019ea0: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
-00019eb0: 3d20 6622 7b69 7d20 2220 6966 2069 7353  = f"{i} " if isS
-00019ec0: 7061 6365 4974 656d 2065 6c73 6520 690a  paceItem else i.
-00019ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019ee0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00019ef0: 2e6c 696e 6557 6964 7468 202b 3d20 6957  .lineWidth += iW
-00019f00: 6964 7468 202b 2031 2069 6620 6973 5370  idth + 1 if isSp
-00019f10: 6163 6549 7465 6d20 656c 7365 2069 5769  aceItem else iWi
-00019f20: 6474 680a 2020 2020 2020 2020 2020 2020  dth.            
-00019f30: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00019f40: 2020 2020 2020 2020 2020 2020 2020 6974                it
-00019f50: 656d 5769 6474 6820 3d20 6765 7453 7472  emWidth = getStr
-00019f60: 696e 6757 6964 7468 2869 7465 6d29 0a20  ingWidth(item). 
-00019f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019f80: 2020 2069 6620 6973 4c61 7374 4974 656d     if isLastItem
-00019f90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019fa0: 2020 2020 2020 2020 2020 6e65 774c 696e            newLin
-00019fb0: 6557 6964 7468 203d 2073 656c 662e 6c69  eWidth = self.li
-00019fc0: 6e65 5769 6474 6820 2b20 6974 656d 5769  neWidth + itemWi
-00019fd0: 6474 680a 2020 2020 2020 2020 2020 2020  dth.            
-00019fe0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00019ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a000: 2020 2020 2020 6e65 774c 696e 6557 6964        newLineWid
-0001a010: 7468 203d 2073 656c 662e 6c69 6e65 5769  th = self.lineWi
-0001a020: 6474 6820 2b20 6974 656d 5769 6474 6820  dth + itemWidth 
-0001a030: 2b20 310a 2020 2020 2020 2020 2020 2020  + 1.            
-0001a040: 2020 2020 2020 2020 6966 206e 6577 4c69          if newLi
-0001a050: 6e65 5769 6474 6820 3e20 7465 726d 696e  neWidth > termin
-0001a060: 616c 5f77 6964 7468 3a0a 2020 2020 2020  al_width:.      
-0001a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a080: 2020 7365 6c66 2e77 7261 7070 6564 5465    self.wrappedTe
-0001a090: 7874 202b 3d20 6622 5c6e 7b69 7465 6d7d  xt += f"\n{item}
-0001a0a0: 2220 6966 2069 734c 6173 7449 7465 6d20  " if isLastItem 
-0001a0b0: 656c 7365 2066 225c 6e7b 6974 656d 7d20  else f"\n{item} 
-0001a0c0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0001a0d0: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-0001a0e0: 696e 6557 6964 7468 203d 2069 7465 6d57  ineWidth = itemW
-0001a0f0: 6964 7468 2069 6620 6973 4c61 7374 4974  idth if isLastIt
-0001a100: 656d 2065 6c73 6520 6974 656d 5769 6474  em else itemWidt
-0001a110: 6820 2b20 310a 2020 2020 2020 2020 2020  h + 1.          
-0001a120: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0001a130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a140: 2020 2020 2020 2020 7365 6c66 2e77 7261          self.wra
-0001a150: 7070 6564 5465 7874 202b 3d20 6974 656d  ppedText += item
-0001a160: 2069 6620 6973 4c61 7374 4974 656d 2065   if isLastItem e
-0001a170: 6c73 6520 6622 7b69 7465 6d7d 2022 0a20  lse f"{item} ". 
-0001a180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a190: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
-0001a1a0: 5769 6474 6820 2b3d 2069 7465 6d57 6964  Width += itemWid
-0001a1b0: 7468 2069 6620 6973 4c61 7374 4974 656d  th if isLastItem
-0001a1c0: 2065 6c73 6520 6974 656d 5769 6474 6820   else itemWidth 
-0001a1d0: 2b20 310a 0a20 2020 2020 2020 2064 6566  + 1..        def
-0001a1e0: 2070 726f 6365 7373 4c69 6e65 286c 696e   processLine(lin
-0001a1f0: 6554 6578 7429 3a0a 2020 2020 2020 2020  eText):.        
-0001a200: 2020 2020 6966 2072 652e 7365 6172 6368      if re.search
-0001a210: 2822 3c5b 5e3c 3e5d 2b3f 3e22 2c20 6c69  ("<[^<>]+?>", li
-0001a220: 6e65 5465 7874 293a 0a20 2020 2020 2020  neText):.       
-0001a230: 2020 2020 2020 2020 2023 2068 616e 646c           # handl
-0001a240: 6520 6874 6d6c 2f78 6d6c 2074 6167 730a  e html/xml tags.
-0001a250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a260: 6368 756e 6b73 203d 206c 696e 6554 6578  chunks = lineTex
-0001a270: 742e 7370 6c69 7428 223e 2229 0a20 2020  t.split(">").   
-0001a280: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-0001a290: 616c 4368 756e 6b73 203d 206c 656e 2863  alChunks = len(c
-0001a2a0: 6875 6e6b 7329 0a20 2020 2020 2020 2020  hunks).         
-0001a2b0: 2020 2020 2020 2066 6f72 2069 6e64 6578         for index
-0001a2c0: 2c20 6368 756e 6b20 696e 2065 6e75 6d65  , chunk in enume
-0001a2d0: 7261 7465 2863 6875 6e6b 7329 3a0a 2020  rate(chunks):.  
-0001a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a2f0: 2020 6973 4c61 7374 4368 756e 6b20 3d20    isLastChunk = 
-0001a300: 2874 6f74 616c 4368 756e 6b73 202d 2069  (totalChunks - i
-0001a310: 6e64 6578 203d 3d20 3129 0a20 2020 2020  ndex == 1).     
-0001a320: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001a330: 6620 6973 4c61 7374 4368 756e 6b3a 0a20  f isLastChunk:. 
-0001a340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a350: 2020 2020 2020 2061 6464 576f 7264 7328         addWords(
-0001a360: 6368 756e 6b29 0a20 2020 2020 2020 2020  chunk).         
-0001a370: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0001a380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a390: 2020 2020 2020 2020 2074 6167 203d 2054           tag = T
-0001a3a0: 7275 6520 6966 2022 3c22 2069 6e20 6368  rue if "<" in ch
-0001a3b0: 756e 6b20 656c 7365 2046 616c 7365 0a20  unk else False. 
-0001a3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3d0: 2020 2020 2020 2069 6620 7461 673a 0a20         if tag:. 
-0001a3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a3f0: 2020 2020 2020 2020 2020 206e 6f6e 5461             nonTa
-0001a400: 672c 2074 6167 436f 6e74 656e 7420 3d20  g, tagContent = 
-0001a410: 6368 756e 6b2e 7273 706c 6974 2822 3c22  chunk.rsplit("<"
-0001a420: 2c20 3129 0a20 2020 2020 2020 2020 2020  , 1).           
-0001a430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a440: 2061 6464 576f 7264 7328 6e6f 6e54 6167   addWords(nonTag
-0001a450: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0001a460: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0001a470: 6c66 2e77 7261 7070 6564 5465 7874 202b  lf.wrappedText +
-0001a480: 3d20 6622 3c7b 7461 6743 6f6e 7465 6e74  = f"<{tagContent
-0001a490: 7d3e 220a 2020 2020 2020 2020 2020 2020  }>".            
-0001a4a0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0001a4b0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0001a4c0: 2020 2020 2020 2020 2020 2020 2020 6164                ad
-0001a4d0: 6457 6f72 6473 2866 227b 6368 756e 6b7d  dWords(f"{chunk}
-0001a4e0: 3e22 290a 2020 2020 2020 2020 2020 2020  >").            
-0001a4f0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0001a500: 2020 2020 2020 6164 6457 6f72 6473 286c        addWords(l
-0001a510: 696e 6554 6578 7429 0a0a 2020 2020 2020  ineText)..      
-0001a520: 2020 6c69 6e65 7320 3d20 7465 7874 2e73    lines = text.s
-0001a530: 706c 6974 2822 5c6e 2229 0a20 2020 2020  plit("\n").     
-0001a540: 2020 2074 6f74 616c 4c69 6e65 7320 3d20     totalLines = 
-0001a550: 6c65 6e28 6c69 6e65 7329 0a20 2020 2020  len(lines).     
-0001a560: 2020 2066 6f72 2069 6e64 6578 2c20 6c69     for index, li
-0001a570: 6e65 2069 6e20 656e 756d 6572 6174 6528  ne in enumerate(
-0001a580: 6c69 6e65 7329 3a0a 2020 2020 2020 2020  lines):.        
-0001a590: 2020 2020 6973 4c61 7374 4c69 6e65 203d      isLastLine =
-0001a5a0: 2028 746f 7461 6c4c 696e 6573 202d 2069   (totalLines - i
-0001a5b0: 6e64 6578 203d 3d20 3129 0a20 2020 2020  ndex == 1).     
-0001a5c0: 2020 2020 2020 2070 726f 6365 7373 4c69         processLi
-0001a5d0: 6e65 286c 696e 6529 0a20 2020 2020 2020  ne(line).       
-0001a5e0: 2020 2020 2069 6620 6e6f 7420 6973 4c61       if not isLa
-0001a5f0: 7374 4c69 6e65 3a0a 2020 2020 2020 2020  stLine:.        
-0001a600: 2020 2020 2020 2020 7365 6c66 2e77 7261          self.wra
-0001a610: 7070 6564 5465 7874 202b 3d20 225c 6e22  ppedText += "\n"
-0001a620: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a630: 2073 656c 662e 6c69 6e65 5769 6474 6820   self.lineWidth 
-0001a640: 3d20 300a 0a20 2020 2020 2020 2072 6574  = 0..        ret
-0001a650: 7572 6e20 7365 6c66 2e77 7261 7070 6564  urn self.wrapped
-0001a660: 5465 7874 0a                             Text.
+00017c40: 2020 636f 6e74 696e 7565 0a20 2020 2020    continue.     
+00017c50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00017c60: 2063 6c65 6172 2063 6f6e 6669 672e 7072   clear config.pr
+00017c70: 6564 6566 696e 6564 436f 6e74 6578 7454  edefinedContextT
+00017c80: 656d 7020 6966 2061 6e79 0a20 2020 2020  emp if any.     
+00017c90: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00017ca0: 6620 636f 6e66 6967 2e70 7265 6465 6669  f config.predefi
+00017cb0: 6e65 6443 6f6e 7465 7874 5465 6d70 3a0a  nedContextTemp:.
+00017cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017cd0: 2020 2020 2020 2020 636f 6e66 6967 2e70          config.p
+00017ce0: 7265 6465 6669 6e65 6443 6f6e 7465 7874  redefinedContext
+00017cf0: 203d 2063 6f6e 6669 672e 7072 6564 6566   = config.predef
+00017d00: 696e 6564 436f 6e74 6578 7454 656d 700a  inedContextTemp.
+00017d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017d20: 2020 2020 2020 2020 636f 6e66 6967 2e70          config.p
+00017d30: 7265 6465 6669 6e65 6443 6f6e 7465 7874  redefinedContext
+00017d40: 5465 6d70 203d 2022 220a 2020 2020 2020  Temp = "".      
+00017d50: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00017d60: 656d 7074 7920 636f 6e66 6967 2e70 6167  empty config.pag
+00017d70: 6572 436f 6e74 656e 740a 2020 2020 2020  erContent.      
+00017d80: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00017d90: 6e66 6967 2e70 6167 6572 436f 6e74 656e  nfig.pagerConten
+00017da0: 7420 3d20 2222 0a0a 2020 2020 2020 2020  t = ""..        
+00017db0: 2020 2020 2020 2020 2020 2020 2320 6368              # ch
+00017dc0: 6563 6b20 7370 6563 6961 6c20 656e 7472  eck special entr
+00017dd0: 6965 730a 2020 2020 2020 2020 2020 2020  ies.            
+00017de0: 2020 2020 2020 2020 2320 6966 2075 7365          # if use
+00017df0: 7220 6361 6c6c 2061 2063 6861 7462 6f74  r call a chatbot
+00017e00: 2077 6974 686f 7574 2066 756e 6374 696f   without functio
+00017e10: 6e20 6361 6c6c 696e 670a 2020 2020 2020  n calling.      
+00017e20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017e30: 2022 5b43 4841 545d 2220 696e 2066 696e   "[CHAT]" in fin
+00017e40: 6554 756e 6564 5573 6572 496e 7075 743a  eTunedUserInput:
+00017e50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017e60: 2020 2020 2020 2020 2063 6861 7462 6f74           chatbot
+00017e70: 203d 2063 6f6e 6669 672e 6c6c 6d49 6e74   = config.llmInt
+00017e80: 6572 6661 6365 0a20 2020 2020 2020 2020  erface.         
+00017e90: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+00017ea0: 6361 6c6c 4368 6174 426f 7420 3a3d 2072  callChatBot := r
+00017eb0: 652e 7365 6172 6368 2822 5c5b 4348 4154  e.search("\[CHAT
+00017ec0: 5f28 5b5e 5c5b 5c5d 5d2b 3f29 5c5d 222c  _([^\[\]]+?)\]",
+00017ed0: 2066 696e 6554 756e 6564 5573 6572 496e   fineTunedUserIn
+00017ee0: 7075 7429 3a0a 2020 2020 2020 2020 2020  put):.          
+00017ef0: 2020 2020 2020 2020 2020 2020 2020 6368                ch
+00017f00: 6174 626f 7420 3d20 6361 6c6c 4368 6174  atbot = callChat
+00017f10: 426f 742e 6772 6f75 7028 3129 2e6c 6f77  Bot.group(1).low
+00017f20: 6572 2829 2069 6620 6361 6c6c 4368 6174  er() if callChat
+00017f30: 426f 7420 616e 6420 6361 6c6c 4368 6174  Bot and callChat
+00017f40: 426f 742e 6772 6f75 7028 3129 2e6c 6f77  Bot.group(1).low
+00017f50: 6572 2829 2069 6e20 2822 6368 6174 6770  er() in ("chatgp
+00017f60: 7422 2c20 2267 656d 696e 6970 726f 222c  t", "geminipro",
+00017f70: 2022 7061 6c6d 3222 2c20 2263 6f64 6579   "palm2", "codey
+00017f80: 2229 2065 6c73 6520 2222 0a20 2020 2020  ") else "".     
+00017f90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00017fa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00017fb0: 2020 2020 2020 2020 2020 2020 2063 6861               cha
+00017fc0: 7462 6f74 203d 2022 220a 2020 2020 2020  tbot = "".      
+00017fd0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00017fe0: 2063 6861 7462 6f74 3a0a 2020 2020 2020   chatbot:.      
+00017ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018000: 2020 2320 6361 6c6c 2074 6865 2073 7063    # call the spc
+00018010: 6966 6965 6420 6368 6174 626f 7420 746f  ified chatbot to
+00018020: 2063 6f6e 7469 6e75 6520 7468 6520 636f   continue the co
+00018030: 6e76 6572 7361 7469 6f6e 0a20 2020 2020  nversation.     
+00018040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018050: 2020 2066 696e 6554 756e 6564 5573 6572     fineTunedUser
+00018060: 496e 7075 7420 3d20 7265 2e73 7562 2822  Input = re.sub("
+00018070: 5c5b 4348 4154 5c5d 7c5c 5b43 4841 545f  \[CHAT\]|\[CHAT_
+00018080: 5b5e 5c5b 5c5d 5d2b 3f5c 5d22 2c20 2222  [^\[\]]+?\]", ""
+00018090: 2c20 6669 6e65 5475 6e65 6455 7365 7249  , fineTunedUserI
+000180a0: 6e70 7574 290a 2020 2020 2020 2020 2020  nput).          
+000180b0: 2020 2020 2020 2020 2020 2020 2020 7365                se
+000180c0: 6c66 2e6c 6175 6e63 6843 6861 7462 6f74  lf.launchChatbot
+000180d0: 2863 6861 7462 6f74 2c20 6669 6e65 5475  (chatbot, fineTu
+000180e0: 6e65 6455 7365 7249 6e70 7574 290a 2020  nedUserInput).  
+000180f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018100: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+00018110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018120: 2020 2023 2077 6865 6e20 7573 6572 2064     # when user d
+00018130: 6f6e 2774 2077 616e 7420 6120 6675 6e63  on't want a func
+00018140: 7469 6f6e 2063 616c 6c0a 2020 2020 2020  tion call.      
+00018150: 2020 2020 2020 2020 2020 2020 2020 6e6f                no
+00018160: 4675 6e63 7469 6f6e 4361 6c6c 203d 2028  FunctionCall = (
+00018170: 225b 4e4f 5f54 4f4f 4c5d 2220 696e 2066  "[NO_TOOL]" in f
+00018180: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
+00018190: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+000181a0: 2020 2020 2020 2023 2077 6865 6e20 7573         # when us
+000181b0: 6572 2077 616e 7420 746f 2063 616c 6c20  er want to call 
+000181c0: 6120 7061 7274 6963 756c 6172 2066 756e  a particular fun
+000181d0: 6374 696f 6e0a 2020 2020 2020 2020 2020  ction.          
+000181e0: 2020 2020 2020 2020 2020 6368 6563 6b43            checkC
+000181f0: 616c 6c53 7065 6369 6669 6346 756e 6374  allSpecificFunct
+00018200: 696f 6e20 3d20 7265 2e73 6561 7263 6828  ion = re.search(
+00018210: 225c 5b54 4f4f 4c5f 285b 5e5c 5b5c 5d5d  "\[TOOL_([^\[\]]
+00018220: 2b3f 295c 5d22 2c20 6669 6e65 5475 6e65  +?)\]", fineTune
+00018230: 6455 7365 7249 6e70 7574 290a 2020 2020  dUserInput).    
+00018240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018250: 636f 6e66 6967 2e73 656c 6563 7465 6454  config.selectedT
+00018260: 6f6f 6c20 3d20 6368 6563 6b43 616c 6c53  ool = checkCallS
+00018270: 7065 6369 6669 6346 756e 6374 696f 6e2e  pecificFunction.
+00018280: 6772 6f75 7028 3129 2069 6620 6368 6563  group(1) if chec
+00018290: 6b43 616c 6c53 7065 6369 6669 6346 756e  kCallSpecificFun
+000182a0: 6374 696f 6e20 616e 6420 6368 6563 6b43  ction and checkC
+000182b0: 616c 6c53 7065 6369 6669 6346 756e 6374  allSpecificFunct
+000182c0: 696f 6e2e 6772 6f75 7028 3129 2069 6e20  ion.group(1) in 
+000182d0: 636f 6e66 6967 2e74 6f6f 6c46 756e 6374  config.toolFunct
+000182e0: 696f 6e4d 6574 686f 6473 2065 6c73 6520  ionMethods else 
+000182f0: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+00018300: 2020 2020 2020 2069 6620 636f 6e66 6967         if config
+00018310: 2e64 6576 656c 6f70 6572 2061 6e64 2063  .developer and c
+00018320: 6f6e 6669 672e 7365 6c65 6374 6564 546f  onfig.selectedTo
+00018330: 6f6c 3a0a 2020 2020 2020 2020 2020 2020  ol:.            
+00018340: 2020 2020 2020 2020 2020 2020 2370 7269              #pri
+00018350: 6e74 3128 6622 6361 6c6c 696e 6720 6675  nt1(f"calling fu
+00018360: 6e63 7469 6f6e 2027 7b63 6f6e 6669 672e  nction '{config.
+00018370: 7365 6c65 6374 6564 546f 6f6c 7d27 202e  selectedTool}' .
+00018380: 2e2e 2229 0a20 2020 2020 2020 2020 2020  ..").           
+00018390: 2020 2020 2020 2020 2020 2020 2070 7269               pri
+000183a0: 6e74 5f66 6f72 6d61 7474 6564 5f74 6578  nt_formatted_tex
+000183b0: 7428 4854 4d4c 2866 223c 7b63 6f6e 6669  t(HTML(f"<{confi
+000183c0: 672e 7465 726d 696e 616c 5072 6f6d 7074  g.terminalPrompt
+000183d0: 496e 6469 6361 746f 7243 6f6c 6f72 327d  IndicatorColor2}
+000183e0: 3e43 616c 6c69 6e67 2066 756e 6374 696f  >Calling functio
+000183f0: 6e3c 2f7b 636f 6e66 6967 2e74 6572 6d69  n</{config.termi
+00018400: 6e61 6c50 726f 6d70 7449 6e64 6963 6174  nalPromptIndicat
+00018410: 6f72 436f 6c6f 7232 7d3e 203c 7b63 6f6e  orColor2}> <{con
+00018420: 6669 672e 7465 726d 696e 616c 436f 6d6d  fig.terminalComm
+00018430: 616e 6445 6e74 7279 436f 6c6f 7232 7d3e  andEntryColor2}>
+00018440: 277b 636f 6e66 6967 2e73 656c 6563 7465  '{config.selecte
+00018450: 6454 6f6f 6c7d 273c 2f7b 636f 6e66 6967  dTool}'</{config
+00018460: 2e74 6572 6d69 6e61 6c43 6f6d 6d61 6e64  .terminalCommand
+00018470: 456e 7472 7943 6f6c 6f72 327d 3e20 3c7b  EntryColor2}> <{
+00018480: 636f 6e66 6967 2e74 6572 6d69 6e61 6c50  config.terminalP
+00018490: 726f 6d70 7449 6e64 6963 6174 6f72 436f  romptIndicatorCo
+000184a0: 6c6f 7232 7d3e 2e2e 2e3c 2f7b 636f 6e66  lor2}>...</{conf
+000184b0: 6967 2e74 6572 6d69 6e61 6c50 726f 6d70  ig.terminalPromp
+000184c0: 7449 6e64 6963 6174 6f72 436f 6c6f 7232  tIndicatorColor2
+000184d0: 7d3e 2229 290a 2020 2020 2020 2020 2020  }>")).          
+000184e0: 2020 2020 2020 2020 2020 6669 6e65 5475            fineTu
+000184f0: 6e65 6455 7365 7249 6e70 7574 203d 2072  nedUserInput = r
+00018500: 652e 7375 6228 7370 6563 6961 6c45 6e74  e.sub(specialEnt
+00018510: 7279 5061 7474 6572 6e2c 2022 222c 2066  ryPattern, "", f
+00018520: 696e 6554 756e 6564 5573 6572 496e 7075  ineTunedUserInpu
+00018530: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00018540: 2020 2020 2020 2063 6f6e 6669 672e 6375         config.cu
+00018550: 7272 656e 744d 6573 7361 6765 732e 6170  rrentMessages.ap
+00018560: 7065 6e64 287b 2272 6f6c 6522 3a20 2275  pend({"role": "u
+00018570: 7365 7222 2c20 2263 6f6e 7465 6e74 223a  ser", "content":
+00018580: 2066 696e 6554 756e 6564 5573 6572 496e   fineTunedUserIn
+00018590: 7075 747d 290a 0a20 2020 2020 2020 2020  put})..         
+000185a0: 2020 2020 2020 2020 2020 2023 2073 7461             # sta
+000185b0: 7274 2073 7069 6e6e 696e 670a 2020 2020  rt spinning.    
+000185c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000185d0: 636f 6e66 6967 2e73 746f 705f 6576 656e  config.stop_even
+000185e0: 7420 3d20 7468 7265 6164 696e 672e 4576  t = threading.Ev
+000185f0: 656e 7428 290a 2020 2020 2020 2020 2020  ent().          
+00018600: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00018610: 2e73 7069 6e6e 6572 5f74 6872 6561 6420  .spinner_thread 
+00018620: 3d20 7468 7265 6164 696e 672e 5468 7265  = threading.Thre
+00018630: 6164 2874 6172 6765 743d 7370 696e 6e69  ad(target=spinni
+00018640: 6e67 5f61 6e69 6d61 7469 6f6e 2c20 6172  ng_animation, ar
+00018650: 6773 3d28 636f 6e66 6967 2e73 746f 705f  gs=(config.stop_
+00018660: 6576 656e 742c 2929 0a20 2020 2020 2020  event,)).       
+00018670: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+00018680: 6669 672e 7370 696e 6e65 725f 7468 7265  fig.spinner_thre
+00018690: 6164 2e73 7461 7274 2829 0a0a 2020 2020  ad.start()..    
+000186a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000186b0: 2320 666f 7263 6520 6c6f 6164 696e 6720  # force loading 
+000186c0: 696e 7465 726e 6574 2073 6561 7263 6865  internet searche
+000186d0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+000186e0: 2020 2020 2020 6966 2063 6f6e 6669 672e        if config.
+000186f0: 6c6f 6164 696e 6749 6e74 6572 6e65 7453  loadingInternetS
+00018700: 6561 7263 6865 7320 3d3d 2022 616c 7761  earches == "alwa
+00018710: 7973 223a 0a20 2020 2020 2020 2020 2020  ys":.           
+00018720: 2020 2020 2020 2020 2020 2020 2074 7279               try
+00018730: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00018740: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00018750: 6e66 6967 2e63 7572 7265 6e74 4d65 7373  nfig.currentMess
+00018760: 6167 6573 203d 2043 616c 6c4c 4c4d 2e72  ages = CallLLM.r
+00018770: 756e 5369 6e67 6c65 4675 6e63 7469 6f6e  unSingleFunction
+00018780: 4361 6c6c 2863 6f6e 6669 672e 6375 7272  Call(config.curr
+00018790: 656e 744d 6573 7361 6765 732c 2022 696e  entMessages, "in
+000187a0: 7465 6772 6174 655f 676f 6f67 6c65 5f73  tegrate_google_s
+000187b0: 6561 7263 6865 7322 290a 2020 2020 2020  earches").      
+000187c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187d0: 2020 6578 6365 7074 3a0a 2020 2020 2020    except:.      
+000187e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000187f0: 2020 2020 2020 7072 696e 7431 2822 556e        print1("Un
+00018800: 6162 6c65 2074 6f20 6c6f 6164 2069 6e74  able to load int
+00018810: 6572 6e65 7420 7265 736f 7572 6365 732e  ernet resources.
+00018820: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00018830: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018840: 686f 7745 7272 6f72 7328 290a 0a20 2020  howErrors()..   
+00018850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018860: 2063 6f6d 706c 6574 696f 6e20 3d20 4361   completion = Ca
+00018870: 6c6c 4c4c 4d2e 7275 6e47 656e 6975 7343  llLLM.runGeniusC
+00018880: 616c 6c28 636f 6e66 6967 2e63 7572 7265  all(config.curre
+00018890: 6e74 4d65 7373 6167 6573 2c20 6e6f 4675  ntMessages, noFu
+000188a0: 6e63 7469 6f6e 4361 6c6c 290a 2020 2020  nctionCall).    
+000188b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000188c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000188d0: 2020 2020 2023 2073 746f 7020 7370 696e       # stop spin
+000188e0: 6e69 6e67 0a20 2020 2020 2020 2020 2020  ning.           
+000188f0: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+00018900: 7275 6e50 7974 686f 6e20 3d20 5472 7565  runPython = True
+00018910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018920: 2020 2020 2073 746f 7053 7069 6e6e 696e       stopSpinnin
+00018930: 6728 290a 0a20 2020 2020 2020 2020 2020  g()..           
+00018940: 2020 2020 2020 2020 2069 6620 636f 6d70           if comp
+00018950: 6c65 7469 6f6e 2069 7320 6e6f 7420 4e6f  letion is not No
+00018960: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00018970: 2020 2020 2020 2020 2020 2020 2320 4372              # Cr
+00018980: 6561 7465 2061 206e 6577 2074 6872 6561  eate a new threa
+00018990: 6420 666f 7220 7468 6520 7374 7265 616d  d for the stream
+000189a0: 696e 6720 7461 736b 0a20 2020 2020 2020  ing task.       
+000189b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000189c0: 2073 7472 6561 6d69 6e67 576f 7264 5772   streamingWordWr
+000189d0: 6170 7065 7220 3d20 5374 7265 616d 696e  apper = Streamin
+000189e0: 6757 6f72 6457 7261 7070 6572 2829 0a20  gWordWrapper(). 
+000189f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a00: 2020 2020 2020 2073 7472 6561 6d69 6e67         streaming
+00018a10: 5f65 7665 6e74 203d 2074 6872 6561 6469  _event = threadi
+00018a20: 6e67 2e45 7665 6e74 2829 0a20 2020 2020  ng.Event().     
+00018a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018a40: 2020 2073 656c 662e 7374 7265 616d 696e     self.streamin
+00018a50: 675f 7468 7265 6164 203d 2074 6872 6561  g_thread = threa
+00018a60: 6469 6e67 2e54 6872 6561 6428 7461 7267  ding.Thread(targ
+00018a70: 6574 3d73 7472 6561 6d69 6e67 576f 7264  et=streamingWord
+00018a80: 5772 6170 7065 722e 7374 7265 616d 4f75  Wrapper.streamOu
+00018a90: 7470 7574 732c 2061 7267 733d 2873 7472  tputs, args=(str
+00018aa0: 6561 6d69 6e67 5f65 7665 6e74 2c20 636f  eaming_event, co
+00018ab0: 6d70 6c65 7469 6f6e 2c20 5472 7565 2069  mpletion, True i
+00018ac0: 6620 636f 6e66 6967 2e6c 6c6d 496e 7465  f config.llmInte
+00018ad0: 7266 6163 6520 696e 2028 2263 6861 7467  rface in ("chatg
+00018ae0: 7074 222c 2022 6c65 746d 6564 6f69 7422  pt", "letmedoit"
+00018af0: 2920 656c 7365 2046 616c 7365 2929 0a20  ) else False)). 
+00018b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b10: 2020 2020 2020 2023 2053 7461 7274 2074         # Start t
+00018b20: 6865 2073 7472 6561 6d69 6e67 2074 6872  he streaming thr
+00018b30: 6561 640a 2020 2020 2020 2020 2020 2020  ead.            
+00018b40: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00018b50: 2e73 7472 6561 6d69 6e67 5f74 6872 6561  .streaming_threa
+00018b60: 642e 7374 6172 7428 290a 0a20 2020 2020  d.start()..     
+00018b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018b80: 2020 2023 2077 6169 7420 7768 696c 6520     # wait while 
+00018b90: 7465 7874 206f 7574 7075 7420 6973 2073  text output is s
+00018ba0: 7465 616d 696e 673b 2063 6170 7475 7265  teaming; capture
+00018bb0: 206b 6579 2063 6f6d 626f 2027 6374 726c   key combo 'ctrl
+00018bc0: 2b71 2720 6f72 2027 6374 726c 2b7a 2720  +q' or 'ctrl+z' 
+00018bd0: 746f 2073 746f 7020 7468 6520 7374 7265  to stop the stre
+00018be0: 616d 696e 670a 2020 2020 2020 2020 2020  aming.          
+00018bf0: 2020 2020 2020 2020 2020 2020 2020 7374                st
+00018c00: 7265 616d 696e 6757 6f72 6457 7261 7070  reamingWordWrapp
+00018c10: 6572 2e6b 6579 546f 5374 6f70 5374 7265  er.keyToStopStre
+00018c20: 616d 696e 6728 7374 7265 616d 696e 675f  aming(streaming_
+00018c30: 6576 656e 7429 0a0a 2020 2020 2020 2020  event)..        
+00018c40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018c50: 2320 7768 656e 2073 7472 6561 6d69 6e67  # when streaming
+00018c60: 2069 7320 646f 6e65 206f 7220 7768 656e   is done or when
+00018c70: 2075 7365 7220 7072 6573 7320 2263 7472   user press "ctr
+00018c80: 6c2b 7122 0a20 2020 2020 2020 2020 2020  l+q".           
+00018c90: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00018ca0: 662e 7374 7265 616d 696e 675f 7468 7265  f.streaming_thre
+00018cb0: 6164 2e6a 6f69 6e28 290a 0a20 2020 2020  ad.join()..     
+00018cc0: 2020 2020 2020 2020 2020 2023 2065 7272             # err
+00018cd0: 6f72 2063 6f64 6573 3a20 6874 7470 733a  or codes: https:
+00018ce0: 2f2f 706c 6174 666f 726d 2e6f 7065 6e61  //platform.opena
+00018cf0: 692e 636f 6d2f 646f 6373 2f67 7569 6465  i.com/docs/guide
+00018d00: 732f 6572 726f 722d 636f 6465 732f 7079  s/error-codes/py
+00018d10: 7468 6f6e 2d6c 6962 7261 7279 2d65 7272  thon-library-err
+00018d20: 6f72 2d74 7970 6573 0a20 2020 2020 2020  or-types.       
+00018d30: 2020 2020 2020 2020 2065 7863 6570 7420           except 
+00018d40: 6f70 656e 6169 2e41 5049 4572 726f 7220  openai.APIError 
+00018d50: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
+00018d60: 2020 2020 2020 2020 2020 7374 6f70 5370            stopSp
+00018d70: 696e 6e69 6e67 2829 0a20 2020 2020 2020  inning().       
+00018d80: 2020 2020 2020 2020 2020 2020 2023 4861               #Ha
+00018d90: 6e64 6c65 2041 5049 2065 7272 6f72 2068  ndle API error h
+00018da0: 6572 652c 2065 2e67 2e20 7265 7472 7920  ere, e.g. retry 
+00018db0: 6f72 206c 6f67 0a20 2020 2020 2020 2020  or log.         
+00018dc0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00018dd0: 3128 6622 4f70 656e 4149 2041 5049 2072  1(f"OpenAI API r
+00018de0: 6574 7572 6e65 6420 616e 2041 5049 2045  eturned an API E
+00018df0: 7272 6f72 3a20 7b65 7d22 290a 2020 2020  rror: {e}").    
+00018e00: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00018e10: 7074 206f 7065 6e61 692e 4150 4943 6f6e  pt openai.APICon
+00018e20: 6e65 6374 696f 6e45 7272 6f72 2061 7320  nectionError as 
+00018e30: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00018e40: 2020 2020 2020 2073 746f 7053 7069 6e6e         stopSpinn
+00018e50: 696e 6728 290a 2020 2020 2020 2020 2020  ing().          
+00018e60: 2020 2020 2020 2020 2020 2348 616e 646c            #Handl
+00018e70: 6520 636f 6e6e 6563 7469 6f6e 2065 7272  e connection err
+00018e80: 6f72 2068 6572 650a 2020 2020 2020 2020  or here.        
+00018e90: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00018ea0: 7431 2866 2246 6169 6c65 6420 746f 2063  t1(f"Failed to c
+00018eb0: 6f6e 6e65 6374 2074 6f20 4f70 656e 4149  onnect to OpenAI
+00018ec0: 2041 5049 3a20 7b65 7d22 290a 2020 2020   API: {e}").    
+00018ed0: 2020 2020 2020 2020 2020 2020 6578 6365              exce
+00018ee0: 7074 206f 7065 6e61 692e 5261 7465 4c69  pt openai.RateLi
+00018ef0: 6d69 7445 7272 6f72 2061 7320 653a 0a20  mitError as e:. 
+00018f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00018f10: 2020 2073 746f 7053 7069 6e6e 696e 6728     stopSpinning(
+00018f20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00018f30: 2020 2020 2020 2348 616e 646c 6520 7261        #Handle ra
+00018f40: 7465 206c 696d 6974 2065 7272 6f72 2028  te limit error (
+00018f50: 7765 2072 6563 6f6d 6d65 6e64 2075 7369  we recommend usi
+00018f60: 6e67 2065 7870 6f6e 656e 7469 616c 2062  ng exponential b
+00018f70: 6163 6b6f 6666 290a 2020 2020 2020 2020  ackoff).        
+00018f80: 2020 2020 2020 2020 2020 2020 7072 696e              prin
+00018f90: 7431 2866 224f 7065 6e41 4920 4150 4920  t1(f"OpenAI API 
+00018fa0: 7265 7175 6573 7420 6578 6365 6564 6564  request exceeded
+00018fb0: 2072 6174 6520 6c69 6d69 743a 207b 657d   rate limit: {e}
+00018fc0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+00018fd0: 2020 2065 7863 6570 743a 0a20 2020 2020     except:.     
+00018fe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00018ff0: 746f 7053 7069 6e6e 696e 6728 290a 2020  topSpinning().  
+00019000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019010: 2020 7472 6163 6520 3d20 7472 6163 6562    trace = traceb
+00019020: 6163 6b2e 666f 726d 6174 5f65 7863 2829  ack.format_exc()
+00019030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019040: 2020 2020 2069 6620 2250 6c65 6173 6520       if "Please 
+00019050: 7265 6475 6365 2074 6865 206c 656e 6774  reduce the lengt
+00019060: 6820 6f66 2074 6865 206d 6573 7361 6765  h of the message
+00019070: 7320 6f72 2063 6f6d 706c 6574 696f 6e22  s or completion"
+00019080: 2069 6e20 7472 6163 653a 0a20 2020 2020   in trace:.     
+00019090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000190a0: 2020 2070 7269 6e74 3128 224d 6178 696d     print1("Maxim
+000190b0: 756d 2074 6f6b 656e 7320 7265 6163 6865  um tokens reache
+000190c0: 6421 2229 0a20 2020 2020 2020 2020 2020  d!").           
+000190d0: 2020 2020 2020 2020 2065 6c69 6620 636f           elif co
+000190e0: 6e66 6967 2e64 6576 656c 6f70 6572 3a0a  nfig.developer:.
+000190f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019100: 2020 2020 2020 2020 7072 696e 7431 2873          print1(s
+00019110: 656c 662e 6469 7669 6465 7229 0a20 2020  elf.divider).   
+00019120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019130: 2020 2020 2070 7269 6e74 3128 7472 6163       print1(trac
+00019140: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+00019150: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00019160: 3128 7365 6c66 2e64 6976 6964 6572 290a  1(self.divider).
+00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019180: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00019190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191a0: 2020 7072 696e 7431 2822 4572 726f 7220    print1("Error 
+000191b0: 656e 636f 756e 7465 7265 6421 2229 0a0a  encountered!")..
+000191c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000191d0: 2020 2020 636f 6e66 6967 2e64 6566 6175      config.defau
+000191e0: 6c74 456e 7472 7920 3d20 7573 6572 496e  ltEntry = userIn
+000191f0: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
+00019200: 2020 2020 2020 2020 7072 696e 7431 2822          print1("
+00019210: 7374 6172 7469 6e67 2061 206e 6577 2063  starting a new c
+00019220: 6861 7421 2229 0a20 2020 2020 2020 2020  hat!").         
+00019230: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019240: 7361 7665 4368 6174 2863 6f6e 6669 672e  saveChat(config.
+00019250: 6375 7272 656e 744d 6573 7361 6765 7329  currentMessages)
+00019260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019270: 2020 2020 2073 746f 7261 6765 6469 7265       storagedire
+00019280: 6374 6f72 792c 2063 6f6e 6669 672e 6375  ctory, config.cu
+00019290: 7272 656e 744d 6573 7361 6765 7320 3d20  rrentMessages = 
+000192a0: 7374 6172 7443 6861 7428 290a 0a20 2020  startChat()..   
+000192b0: 2064 6566 206c 6175 6e63 6843 6861 7462   def launchChatb
+000192c0: 6f74 2873 656c 662c 2063 6861 7462 6f74  ot(self, chatbot
+000192d0: 2c20 6669 6e65 5475 6e65 6455 7365 7249  , fineTunedUserI
+000192e0: 6e70 7574 293a 0a20 2020 2020 2020 2069  nput):.        i
+000192f0: 6620 6e6f 7420 6368 6174 626f 743a 0a20  f not chatbot:. 
+00019300: 2020 2020 2020 2020 2020 2063 6861 7462             chatb
+00019310: 6f74 203d 2063 6f6e 6669 672e 6c6c 6d49  ot = config.llmI
+00019320: 6e74 6572 6661 6365 0a20 2020 2020 2020  nterface.       
+00019330: 2069 6620 636f 6e66 6967 2e69 7354 6572   if config.isTer
+00019340: 6d75 783a 0a20 2020 2020 2020 2020 2020  mux:.           
+00019350: 2023 6368 6174 626f 7420 3d20 2263 6861   #chatbot = "cha
+00019360: 7467 7074 220a 2020 2020 2020 2020 2020  tgpt".          
+00019370: 2020 2e2e 2e0a 2020 2020 2020 2020 6368    ....        ch
+00019380: 6174 626f 7473 203d 207b 0a20 2020 2020  atbots = {.     
+00019390: 2020 2020 2020 2022 6c6c 616d 6163 7070         "llamacpp
+000193a0: 223a 206c 616d 6264 613a 204c 6c61 6d61  ": lambda: Llama
+000193b0: 6370 7043 6861 7428 6d6f 6465 6c3d 4e6f  cppChat(model=No
+000193c0: 6e65 2069 6620 636f 6e66 6967 2e75 7365  ne if config.use
+000193d0: 4164 6469 7469 6f6e 616c 4368 6174 4d6f  AdditionalChatMo
+000193e0: 6465 6c20 656c 7365 2063 6f6e 6669 672e  del else config.
+000193f0: 6c6c 616d 6163 7070 4d61 696e 4d6f 6465  llamacppMainMode
+00019400: 6c29 2e72 756e 2866 696e 6554 756e 6564  l).run(fineTuned
+00019410: 5573 6572 496e 7075 7429 2c0a 2020 2020  UserInput),.    
+00019420: 2020 2020 2020 2020 226f 6c6c 616d 6122          "ollama"
+00019430: 3a20 6c61 6d62 6461 3a20 4f6c 6c61 6d61  : lambda: Ollama
+00019440: 4368 6174 2829 2e72 756e 2866 696e 6554  Chat().run(fineT
+00019450: 756e 6564 5573 6572 496e 7075 742c 206d  unedUserInput, m
+00019460: 6f64 656c 3d63 6f6e 6669 672e 6f6c 6c61  odel=config.olla
+00019470: 6d61 4368 6174 4d6f 6465 6c20 6966 2063  maChatModel if c
+00019480: 6f6e 6669 672e 7573 6541 6464 6974 696f  onfig.useAdditio
+00019490: 6e61 6c43 6861 744d 6f64 656c 2065 6c73  nalChatModel els
+000194a0: 6520 636f 6e66 6967 2e6f 6c6c 616d 614d  e config.ollamaM
+000194b0: 6169 6e4d 6f64 656c 292c 0a20 2020 2020  ainModel),.     
+000194c0: 2020 2020 2020 2022 6368 6174 6770 7422         "chatgpt"
+000194d0: 3a20 6c61 6d62 6461 3a20 4368 6174 4750  : lambda: ChatGP
+000194e0: 5428 292e 7275 6e28 6669 6e65 5475 6e65  T().run(fineTune
+000194f0: 6455 7365 7249 6e70 7574 292c 0a20 2020  dUserInput),.   
+00019500: 2020 2020 2020 2020 2022 6c65 746d 6564           "letmed
+00019510: 6f69 7422 3a20 6c61 6d62 6461 3a20 4368  oit": lambda: Ch
+00019520: 6174 4750 5428 292e 7275 6e28 6669 6e65  atGPT().run(fine
+00019530: 5475 6e65 6455 7365 7249 6e70 7574 292c  TunedUserInput),
+00019540: 0a20 2020 2020 2020 2020 2020 2022 6765  .            "ge
+00019550: 6d69 6e69 223a 206c 616d 6264 613a 2047  mini": lambda: G
+00019560: 656d 696e 6950 726f 2874 656d 7065 7261  eminiPro(tempera
+00019570: 7475 7265 3d63 6f6e 6669 672e 6c6c 6d54  ture=config.llmT
+00019580: 656d 7065 7261 7475 7265 292e 7275 6e28  emperature).run(
+00019590: 6669 6e65 5475 6e65 6455 7365 7249 6e70  fineTunedUserInp
+000195a0: 7574 292c 0a20 2020 2020 2020 2020 2020  ut),.           
+000195b0: 2022 6765 6d69 6e69 7072 6f22 3a20 6c61   "geminipro": la
+000195c0: 6d62 6461 3a20 4765 6d69 6e69 5072 6f28  mbda: GeminiPro(
+000195d0: 7465 6d70 6572 6174 7572 653d 636f 6e66  temperature=conf
+000195e0: 6967 2e6c 6c6d 5465 6d70 6572 6174 7572  ig.llmTemperatur
+000195f0: 6529 2e72 756e 2866 696e 6554 756e 6564  e).run(fineTuned
+00019600: 5573 6572 496e 7075 7429 2c0a 2020 2020  UserInput),.    
+00019610: 2020 2020 2020 2020 2270 616c 6d32 223a          "palm2":
+00019620: 206c 616d 6264 613a 2050 616c 6d32 2829   lambda: Palm2()
+00019630: 2e72 756e 2866 696e 6554 756e 6564 5573  .run(fineTunedUs
+00019640: 6572 496e 7075 742c 2074 656d 7065 7261  erInput, tempera
+00019650: 7475 7265 3d63 6f6e 6669 672e 6c6c 6d54  ture=config.llmT
+00019660: 656d 7065 7261 7475 7265 292c 0a20 2020  emperature),.   
+00019670: 2020 2020 2020 2020 2022 636f 6465 7922           "codey"
+00019680: 3a20 6c61 6d62 6461 3a20 436f 6465 7928  : lambda: Codey(
+00019690: 292e 7275 6e28 6669 6e65 5475 6e65 6455  ).run(fineTunedU
+000196a0: 7365 7249 6e70 7574 2c20 7465 6d70 6572  serInput, temper
+000196b0: 6174 7572 653d 636f 6e66 6967 2e6c 6c6d  ature=config.llm
+000196c0: 5465 6d70 6572 6174 7572 6529 2c0a 2020  Temperature),.  
+000196d0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000196e0: 6966 2063 6861 7462 6f74 2069 6e20 6368  if chatbot in ch
+000196f0: 6174 626f 7473 3a0a 2020 2020 2020 2020  atbots:.        
+00019700: 2020 2020 6368 6174 626f 7473 5b63 6861      chatbots[cha
+00019710: 7462 6f74 5d28 290a 0a20 2020 2064 6566  tbot]()..    def
+00019720: 2061 6464 5061 6765 7254 6578 7428 7365   addPagerText(se
+00019730: 6c66 2c20 7465 7874 2c20 7772 6170 576f  lf, text, wrapWo
+00019740: 7264 733d 4661 6c73 6529 3a0a 2020 2020  rds=False):.    
+00019750: 2020 2020 6966 2077 7261 7057 6f72 6473      if wrapWords
+00019760: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
+00019770: 7874 203d 2073 656c 662e 6765 7457 7261  xt = self.getWra
+00019780: 7070 6564 4854 4d4c 5465 7874 2874 6578  ppedHTMLText(tex
+00019790: 7429 0a20 2020 2020 2020 2063 6f6e 6669  t).        confi
+000197a0: 672e 7061 6765 7243 6f6e 7465 6e74 202b  g.pagerContent +
+000197b0: 3d20 6622 7b74 6578 747d 5c6e 220a 0a20  = f"{text}\n".. 
+000197c0: 2020 2064 6566 206c 6175 6e63 6850 6167     def launchPag
+000197d0: 6572 2873 656c 662c 2070 6167 6572 436f  er(self, pagerCo
+000197e0: 6e74 656e 743d 4e6f 6e65 293a 0a20 2020  ntent=None):.   
+000197f0: 2020 2020 2069 6620 7061 6765 7243 6f6e       if pagerCon
+00019800: 7465 6e74 2069 7320 4e6f 6e65 3a0a 2020  tent is None:.  
+00019810: 2020 2020 2020 2020 2020 7061 6765 7243            pagerC
+00019820: 6f6e 7465 6e74 203d 2063 6f6e 6669 672e  ontent = config.
+00019830: 7061 6765 7243 6f6e 7465 6e74 0a20 2020  pagerContent.   
+00019840: 2020 2020 2069 6620 7061 6765 7243 6f6e       if pagerCon
+00019850: 7465 6e74 3a0a 2020 2020 2020 2020 2020  tent:.          
+00019860: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00019870: 2020 2020 2020 2069 6620 7368 7574 696c         if shutil
+00019880: 2e77 6869 6368 2822 6261 7422 293a 0a20  .which("bat"):. 
+00019890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000198a0: 2020 2023 2057 696e 646f 7773 2075 7365     # Windows use
+000198b0: 7273 2063 616e 2069 6e73 7461 6c6c 2062  rs can install b
+000198c0: 6174 2063 6f6d 6d61 6e64 2077 6974 6820  at command with 
+000198d0: 7363 6f6f 700a 2020 2020 2020 2020 2020  scoop.          
+000198e0: 2020 2020 2020 2020 2020 2320 7265 6164            # read
+000198f0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00019900: 2e63 6f6d 2f53 636f 6f70 496e 7374 616c  .com/ScoopInstal
+00019910: 6c65 722f 5363 6f6f 700a 2020 2020 2020  ler/Scoop.      
+00019920: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00019930: 3e20 6977 7220 2d75 7365 6220 6765 742e  > iwr -useb get.
+00019940: 7363 6f6f 702e 7368 207c 2069 6578 0a20  scoop.sh | iex. 
+00019950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019960: 2020 2023 203e 2073 636f 6f70 2069 6e73     # > scoop ins
+00019970: 7461 6c6c 2061 7269 6132 2062 6174 0a20  tall aria2 bat. 
+00019980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019990: 2020 2069 6620 7265 2e73 6561 7263 6828     if re.search(
+000199a0: 223c 5b5e 3c3e 5d2b 3f3e 222c 2070 6167  "<[^<>]+?>", pag
+000199b0: 6572 436f 6e74 656e 7429 3a0a 2020 2020  erContent):.    
+000199c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199d0: 2020 2020 7061 6765 7243 6f6e 7465 6e74      pagerContent
+000199e0: 203d 2054 6578 7455 7469 6c2e 636f 6e76   = TextUtil.conv
+000199f0: 6572 7448 746d 6c54 6167 546f 436f 6c6f  ertHtmlTagToColo
+00019a00: 7261 6d61 2870 6167 6572 436f 6e74 656e  rama(pagerConten
+00019a10: 7429 0a20 2020 2020 2020 2020 2020 2020  t).             
+00019a20: 2020 2020 2020 206c 616e 6775 6167 6520         language 
+00019a30: 3d20 2250 7974 686f 6e22 2069 6620 2260  = "Python" if "`
+00019a40: 6060 7079 7468 6f6e 2220 696e 2070 6167  ``python" in pag
+00019a50: 6572 436f 6e74 656e 7420 656c 7365 2022  erContent else "
+00019a60: 4d61 726b 646f 776e 220a 2020 2020 2020  Markdown".      
+00019a70: 2020 2020 2020 2020 2020 2020 2020 7079                py
+00019a80: 646f 632e 7069 7065 7061 6765 7228 7061  doc.pipepager(pa
+00019a90: 6765 7243 6f6e 7465 6e74 2c20 636d 643d  gerContent, cmd=
+00019aa0: 6622 6261 7420 2d6c 207b 6c61 6e67 7561  f"bat -l {langua
+00019ab0: 6765 7d20 2d2d 7061 6769 6e67 2061 6c77  ge} --paging alw
+00019ac0: 6179 7322 290a 2020 2020 2020 2020 2020  ays").          
+00019ad0: 2020 2020 2020 656c 6966 2073 6875 7469        elif shuti
+00019ae0: 6c2e 7768 6963 6828 226c 6573 7322 293a  l.which("less"):
+00019af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019b00: 2020 2020 2023 2057 696e 646f 7773 2075       # Windows u
+00019b10: 7365 7273 2063 616e 2069 6e73 7461 6c6c  sers can install
+00019b20: 206c 6573 7320 636f 6d6d 616e 6420 7769   less command wi
+00019b30: 7468 2073 636f 6f70 0a20 2020 2020 2020  th scoop.       
+00019b40: 2020 2020 2020 2020 2020 2020 2023 2072               # r
+00019b50: 6561 643a 2068 7474 7073 3a2f 2f67 6974  ead: https://git
+00019b60: 6875 622e 636f 6d2f 5363 6f6f 7049 6e73  hub.com/ScoopIns
+00019b70: 7461 6c6c 6572 2f53 636f 6f70 0a20 2020  taller/Scoop.   
+00019b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019b90: 2023 203e 2069 7772 202d 7573 6562 2067   # > iwr -useb g
+00019ba0: 6574 2e73 636f 6f70 2e73 6820 7c20 6965  et.scoop.sh | ie
+00019bb0: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+00019bc0: 2020 2020 2020 2320 3e20 7363 6f6f 7020        # > scoop 
+00019bd0: 696e 7374 616c 6c20 6172 6961 3220 6c65  install aria2 le
+00019be0: 7373 0a20 2020 2020 2020 2020 2020 2020  ss.             
+00019bf0: 2020 2020 2020 2069 6620 7265 2e73 6561         if re.sea
+00019c00: 7263 6828 223c 5b5e 3c3e 5d2b 3f3e 222c  rch("<[^<>]+?>",
+00019c10: 2070 6167 6572 436f 6e74 656e 7429 3a0a   pagerContent):.
+00019c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c30: 2020 2020 2020 2020 7061 6765 7243 6f6e          pagerCon
+00019c40: 7465 6e74 203d 2054 6578 7455 7469 6c2e  tent = TextUtil.
+00019c50: 636f 6e76 6572 7448 746d 6c54 6167 546f  convertHtmlTagTo
+00019c60: 436f 6c6f 7261 6d61 2870 6167 6572 436f  Colorama(pagerCo
+00019c70: 6e74 656e 7429 0a20 2020 2020 2020 2020  ntent).         
+00019c80: 2020 2020 2020 2020 2020 2070 7964 6f63             pydoc
+00019c90: 2e70 6970 6570 6167 6572 2870 6167 6572  .pipepager(pager
+00019ca0: 436f 6e74 656e 742c 2063 6d64 3d27 6c65  Content, cmd='le
+00019cb0: 7373 202d 5227 290a 2020 2020 2020 2020  ss -R').        
+00019cc0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00019cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ce0: 2020 7079 646f 632e 7061 6765 7228 7061    pydoc.pager(pa
+00019cf0: 6765 7243 6f6e 7465 6e74 290a 2020 2020  gerContent).    
+00019d00: 2020 2020 2020 2020 6578 6365 7074 3a0a          except:.
+00019d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d20: 636f 6e66 6967 2e70 6167 6572 5669 6577  config.pagerView
+00019d30: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
+00019d40: 2020 2020 2020 2020 2073 686f 7745 7272           showErr
+00019d50: 6f72 7328 290a 0a20 2020 2023 2077 7261  ors()..    # wra
+00019d60: 7020 6874 6d6c 2074 6578 7420 6174 2073  p html text at s
+00019d70: 7061 6365 730a 2020 2020 6465 6620 6765  paces.    def ge
+00019d80: 7457 7261 7070 6564 4854 4d4c 5465 7874  tWrappedHTMLText
+00019d90: 2873 656c 662c 2074 6578 742c 2074 6572  (self, text, ter
+00019da0: 6d69 6e61 6c5f 7769 6474 683d 4e6f 6e65  minal_width=None
+00019db0: 293a 0a20 2020 2020 2020 2069 6620 6e6f  ):.        if no
+00019dc0: 7420 2220 2220 696e 2074 6578 743a 0a20  t " " in text:. 
+00019dd0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00019de0: 6e20 7465 7874 0a20 2020 2020 2020 2069  n text.        i
+00019df0: 6620 7465 726d 696e 616c 5f77 6964 7468  f terminal_width
+00019e00: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00019e10: 2020 2020 2020 7465 726d 696e 616c 5f77        terminal_w
+00019e20: 6964 7468 203d 2073 6875 7469 6c2e 6765  idth = shutil.ge
+00019e30: 745f 7465 726d 696e 616c 5f73 697a 6528  t_terminal_size(
+00019e40: 292e 636f 6c75 6d6e 730a 2020 2020 2020  ).columns.      
+00019e50: 2020 7365 6c66 2e77 7261 7070 6564 5465    self.wrappedTe
+00019e60: 7874 203d 2022 220a 2020 2020 2020 2020  xt = "".        
+00019e70: 7365 6c66 2e6c 696e 6557 6964 7468 203d  self.lineWidth =
+00019e80: 2030 0a0a 2020 2020 2020 2020 6465 6620   0..        def 
+00019e90: 6164 6457 6f72 6473 2877 6f72 6473 293a  addWords(words):
+00019ea0: 0a20 2020 2020 2020 2020 2020 2077 6f72  .            wor
+00019eb0: 6473 203d 2077 6f72 6473 2e73 706c 6974  ds = words.split
+00019ec0: 2822 2022 290a 2020 2020 2020 2020 2020  (" ").          
+00019ed0: 2020 666f 7220 696e 6465 782c 2069 7465    for index, ite
+00019ee0: 6d20 696e 2065 6e75 6d65 7261 7465 2877  m in enumerate(w
+00019ef0: 6f72 6473 293a 0a20 2020 2020 2020 2020  ords):.         
+00019f00: 2020 2020 2020 2069 734c 6173 7449 7465         isLastIte
+00019f10: 6d20 3d20 286c 656e 2877 6f72 6473 2920  m = (len(words) 
+00019f20: 2d20 696e 6465 7820 3d3d 2031 290a 2020  - index == 1).  
+00019f30: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00019f40: 2069 735f 434a 4b28 6974 656d 293a 0a20   is_CJK(item):. 
+00019f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019f60: 2020 2066 6f72 2069 496e 6465 782c 2069     for iIndex, i
+00019f70: 2069 6e20 656e 756d 6572 6174 6528 6974   in enumerate(it
+00019f80: 656d 293a 0a20 2020 2020 2020 2020 2020  em):.           
+00019f90: 2020 2020 2020 2020 2020 2020 2069 7353               isS
+00019fa0: 7061 6365 4974 656d 203d 2028 6e6f 7420  paceItem = (not 
+00019fb0: 6973 4c61 7374 4974 656d 2061 6e64 2028  isLastItem and (
+00019fc0: 6c65 6e28 6974 656d 2920 2d20 6949 6e64  len(item) - iInd
+00019fd0: 6578 203d 3d20 3129 290a 2020 2020 2020  ex == 1)).      
+00019fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019ff0: 2020 6957 6964 7468 203d 2067 6574 5374    iWidth = getSt
+0001a000: 7269 6e67 5769 6474 6828 6929 0a20 2020  ringWidth(i).   
+0001a010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a020: 2020 2020 2069 6620 6973 5370 6163 6549       if isSpaceI
+0001a030: 7465 6d3a 0a20 2020 2020 2020 2020 2020  tem:.           
+0001a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a050: 206e 6577 4c69 6e65 5769 6474 6820 3d20   newLineWidth = 
+0001a060: 7365 6c66 2e6c 696e 6557 6964 7468 202b  self.lineWidth +
+0001a070: 2069 5769 6474 6820 2b20 310a 2020 2020   iWidth + 1.    
+0001a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a090: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0001a0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0b0: 2020 2020 2020 6e65 774c 696e 6557 6964        newLineWid
+0001a0c0: 7468 203d 2073 656c 662e 6c69 6e65 5769  th = self.lineWi
+0001a0d0: 6474 6820 2b20 6957 6964 7468 0a20 2020  dth + iWidth.   
+0001a0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a0f0: 2020 2020 2069 6620 6e65 774c 696e 6557       if newLineW
+0001a100: 6964 7468 203e 2074 6572 6d69 6e61 6c5f  idth > terminal_
+0001a110: 7769 6474 683a 0a20 2020 2020 2020 2020  width:.         
+0001a120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a130: 2020 2073 656c 662e 7772 6170 7065 6454     self.wrappedT
+0001a140: 6578 7420 2b3d 2066 225c 6e7b 697d 2022  ext += f"\n{i} "
+0001a150: 2069 6620 6973 5370 6163 6549 7465 6d20   if isSpaceItem 
+0001a160: 656c 7365 2066 225c 6e7b 697d 220a 2020  else f"\n{i}".  
+0001a170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a180: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0001a190: 696e 6557 6964 7468 203d 2069 5769 6474  ineWidth = iWidt
+0001a1a0: 6820 2b20 3120 6966 2069 7353 7061 6365  h + 1 if isSpace
+0001a1b0: 4974 656d 2065 6c73 6520 6957 6964 7468  Item else iWidth
+0001a1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a1d0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001a1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a1f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a200: 7772 6170 7065 6454 6578 7420 2b3d 2066  wrappedText += f
+0001a210: 227b 697d 2022 2069 6620 6973 5370 6163  "{i} " if isSpac
+0001a220: 6549 7465 6d20 656c 7365 2069 0a20 2020  eItem else i.   
+0001a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a240: 2020 2020 2020 2020 2073 656c 662e 6c69           self.li
+0001a250: 6e65 5769 6474 6820 2b3d 2069 5769 6474  neWidth += iWidt
+0001a260: 6820 2b20 3120 6966 2069 7353 7061 6365  h + 1 if isSpace
+0001a270: 4974 656d 2065 6c73 6520 6957 6964 7468  Item else iWidth
+0001a280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a290: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0001a2a0: 2020 2020 2020 2020 2020 2069 7465 6d57             itemW
+0001a2b0: 6964 7468 203d 2067 6574 5374 7269 6e67  idth = getString
+0001a2c0: 5769 6474 6828 6974 656d 290a 2020 2020  Width(item).    
+0001a2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a2e0: 6966 2069 734c 6173 7449 7465 6d3a 0a20  if isLastItem:. 
+0001a2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a300: 2020 2020 2020 206e 6577 4c69 6e65 5769         newLineWi
+0001a310: 6474 6820 3d20 7365 6c66 2e6c 696e 6557  dth = self.lineW
+0001a320: 6964 7468 202b 2069 7465 6d57 6964 7468  idth + itemWidth
+0001a330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a340: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0001a350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a360: 2020 206e 6577 4c69 6e65 5769 6474 6820     newLineWidth 
+0001a370: 3d20 7365 6c66 2e6c 696e 6557 6964 7468  = self.lineWidth
+0001a380: 202b 2069 7465 6d57 6964 7468 202b 2031   + itemWidth + 1
+0001a390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a3a0: 2020 2020 2069 6620 6e65 774c 696e 6557       if newLineW
+0001a3b0: 6964 7468 203e 2074 6572 6d69 6e61 6c5f  idth > terminal_
+0001a3c0: 7769 6474 683a 0a20 2020 2020 2020 2020  width:.         
+0001a3d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a3e0: 656c 662e 7772 6170 7065 6454 6578 7420  elf.wrappedText 
+0001a3f0: 2b3d 2066 225c 6e7b 6974 656d 7d22 2069  += f"\n{item}" i
+0001a400: 6620 6973 4c61 7374 4974 656d 2065 6c73  f isLastItem els
+0001a410: 6520 6622 5c6e 7b69 7465 6d7d 2022 0a20  e f"\n{item} ". 
+0001a420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a430: 2020 2020 2020 2073 656c 662e 6c69 6e65         self.line
+0001a440: 5769 6474 6820 3d20 6974 656d 5769 6474  Width = itemWidt
+0001a450: 6820 6966 2069 734c 6173 7449 7465 6d20  h if isLastItem 
+0001a460: 656c 7365 2069 7465 6d57 6964 7468 202b  else itemWidth +
+0001a470: 2031 0a20 2020 2020 2020 2020 2020 2020   1.             
+0001a480: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0001a490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4a0: 2020 2020 2073 656c 662e 7772 6170 7065       self.wrappe
+0001a4b0: 6454 6578 7420 2b3d 2069 7465 6d20 6966  dText += item if
+0001a4c0: 2069 734c 6173 7449 7465 6d20 656c 7365   isLastItem else
+0001a4d0: 2066 227b 6974 656d 7d20 220a 2020 2020   f"{item} ".    
+0001a4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a4f0: 2020 2020 7365 6c66 2e6c 696e 6557 6964      self.lineWid
+0001a500: 7468 202b 3d20 6974 656d 5769 6474 6820  th += itemWidth 
+0001a510: 6966 2069 734c 6173 7449 7465 6d20 656c  if isLastItem el
+0001a520: 7365 2069 7465 6d57 6964 7468 202b 2031  se itemWidth + 1
+0001a530: 0a0a 2020 2020 2020 2020 6465 6620 7072  ..        def pr
+0001a540: 6f63 6573 734c 696e 6528 6c69 6e65 5465  ocessLine(lineTe
+0001a550: 7874 293a 0a20 2020 2020 2020 2020 2020  xt):.           
+0001a560: 2069 6620 7265 2e73 6561 7263 6828 223c   if re.search("<
+0001a570: 5b5e 3c3e 5d2b 3f3e 222c 206c 696e 6554  [^<>]+?>", lineT
+0001a580: 6578 7429 3a0a 2020 2020 2020 2020 2020  ext):.          
+0001a590: 2020 2020 2020 2320 6861 6e64 6c65 2068        # handle h
+0001a5a0: 746d 6c2f 786d 6c20 7461 6773 0a20 2020  tml/xml tags.   
+0001a5b0: 2020 2020 2020 2020 2020 2020 2063 6875               chu
+0001a5c0: 6e6b 7320 3d20 6c69 6e65 5465 7874 2e73  nks = lineText.s
+0001a5d0: 706c 6974 2822 3e22 290a 2020 2020 2020  plit(">").      
+0001a5e0: 2020 2020 2020 2020 2020 746f 7461 6c43            totalC
+0001a5f0: 6875 6e6b 7320 3d20 6c65 6e28 6368 756e  hunks = len(chun
+0001a600: 6b73 290a 2020 2020 2020 2020 2020 2020  ks).            
+0001a610: 2020 2020 666f 7220 696e 6465 782c 2063      for index, c
+0001a620: 6875 6e6b 2069 6e20 656e 756d 6572 6174  hunk in enumerat
+0001a630: 6528 6368 756e 6b73 293a 0a20 2020 2020  e(chunks):.     
+0001a640: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0001a650: 734c 6173 7443 6875 6e6b 203d 2028 746f  sLastChunk = (to
+0001a660: 7461 6c43 6875 6e6b 7320 2d20 696e 6465  talChunks - inde
+0001a670: 7820 3d3d 2031 290a 2020 2020 2020 2020  x == 1).        
+0001a680: 2020 2020 2020 2020 2020 2020 6966 2069              if i
+0001a690: 734c 6173 7443 6875 6e6b 3a0a 2020 2020  sLastChunk:.    
+0001a6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6b0: 2020 2020 6164 6457 6f72 6473 2863 6875      addWords(chu
+0001a6c0: 6e6b 290a 2020 2020 2020 2020 2020 2020  nk).            
+0001a6d0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0001a6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a6f0: 2020 2020 2020 7461 6720 3d20 5472 7565        tag = True
+0001a700: 2069 6620 223c 2220 696e 2063 6875 6e6b   if "<" in chunk
+0001a710: 2065 6c73 6520 4661 6c73 650a 2020 2020   else False.    
+0001a720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a730: 2020 2020 6966 2074 6167 3a0a 2020 2020      if tag:.    
+0001a740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a750: 2020 2020 2020 2020 6e6f 6e54 6167 2c20          nonTag, 
+0001a760: 7461 6743 6f6e 7465 6e74 203d 2063 6875  tagContent = chu
+0001a770: 6e6b 2e72 7370 6c69 7428 223c 222c 2031  nk.rsplit("<", 1
+0001a780: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0001a790: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+0001a7a0: 6457 6f72 6473 286e 6f6e 5461 6729 0a20  dWords(nonTag). 
+0001a7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a7c0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a7d0: 7772 6170 7065 6454 6578 7420 2b3d 2066  wrappedText += f
+0001a7e0: 223c 7b74 6167 436f 6e74 656e 747d 3e22  "<{tagContent}>"
+0001a7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a800: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0001a810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a820: 2020 2020 2020 2020 2020 2061 6464 576f             addWo
+0001a830: 7264 7328 6622 7b63 6875 6e6b 7d3e 2229  rds(f"{chunk}>")
+0001a840: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0001a850: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0001a860: 2020 2061 6464 576f 7264 7328 6c69 6e65     addWords(line
+0001a870: 5465 7874 290a 0a20 2020 2020 2020 206c  Text)..        l
+0001a880: 696e 6573 203d 2074 6578 742e 7370 6c69  ines = text.spli
+0001a890: 7428 225c 6e22 290a 2020 2020 2020 2020  t("\n").        
+0001a8a0: 746f 7461 6c4c 696e 6573 203d 206c 656e  totalLines = len
+0001a8b0: 286c 696e 6573 290a 2020 2020 2020 2020  (lines).        
+0001a8c0: 666f 7220 696e 6465 782c 206c 696e 6520  for index, line 
+0001a8d0: 696e 2065 6e75 6d65 7261 7465 286c 696e  in enumerate(lin
+0001a8e0: 6573 293a 0a20 2020 2020 2020 2020 2020  es):.           
+0001a8f0: 2069 734c 6173 744c 696e 6520 3d20 2874   isLastLine = (t
+0001a900: 6f74 616c 4c69 6e65 7320 2d20 696e 6465  otalLines - inde
+0001a910: 7820 3d3d 2031 290a 2020 2020 2020 2020  x == 1).        
+0001a920: 2020 2020 7072 6f63 6573 734c 696e 6528      processLine(
+0001a930: 6c69 6e65 290a 2020 2020 2020 2020 2020  line).          
+0001a940: 2020 6966 206e 6f74 2069 734c 6173 744c    if not isLastL
+0001a950: 696e 653a 0a20 2020 2020 2020 2020 2020  ine:.           
+0001a960: 2020 2020 2073 656c 662e 7772 6170 7065       self.wrappe
+0001a970: 6454 6578 7420 2b3d 2022 5c6e 220a 2020  dText += "\n".  
+0001a980: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001a990: 6c66 2e6c 696e 6557 6964 7468 203d 2030  lf.lineWidth = 0
+0001a9a0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0001a9b0: 2073 656c 662e 7772 6170 7065 6454 6578   self.wrappedTex
+0001a9c0: 740a                                     t.
```

### Comparing `freegenius-0.0.95/freegenius/utils/call_chatgpt.py` & `freegenius-0.0.97/freegenius/utils/call_chatgpt.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,15 +359,15 @@
     # Auto Function Call equivalence
 
     @staticmethod
     def runGeniusCall(messages: dict, noFunctionCall: bool = False):
         user_request = messages[-1]["content"]
         if config.intent_screening:
             # 1. Intent Screening
-            noFunctionCall = True if noFunctionCall else CallChatGPT.screen_user_request(messages=messages)
+            noFunctionCall = True if noFunctionCall else CallChatGPT.isChatOnly(messages=messages)
         if noFunctionCall or config.tool_dependence <= 0.0:
             return CallChatGPT.regularCall(messages)
         else:
             # 2. Tool Selection
             if config.selectedTool and config.selectedTool in config.toolFunctionSchemas:
                 tool_name = config.selectedTool
                 tool_schema = config.toolFunctionSchemas[tool_name]
@@ -456,15 +456,16 @@
                     # tool function executed without chat extension
                     config.currentMessages.append({"role": "assistant", "content": config.tempContent if config.tempContent else "Done!"})
                     config.tempContent = ""
                     config.conversationStarted = True
                     return None
 
     @staticmethod
-    def screen_user_request(messages: dict) -> bool:
+    def isChatOnly(messages: dict) -> bool:
+        print2("```screening")
         properties = {
             "answer": {
                 "type": "string",
                 "description": """Evaluate my request to determine if you are able to resolve my request as a text-based AI:
 - Answer 'no' if you are asked to execute a computing task or an online search.
 - Answer 'no' if you are asked for updates / news / real-time information.
 - Answer 'yes' if the request is a greeting or translation.
@@ -478,15 +479,18 @@
             "parameters": {
                 "type": "object",
                 "properties": properties,
                 "required": ["code"],
             },
         }
         output = CallChatGPT.getResponseDict(messages, schema=schema)
-        return True if "yes" in str(output).lower() else False
+        chatOnly = True if "yes" in str(output).lower() else False
+        print3(f"""Tool may {"not " if chatOnly else ""}be required.""")
+        print2("```")
+        return chatOnly
 
     @staticmethod
     def extractToolParameters(schema: dict, ongoingMessages: list = [], **kwargs) -> dict:
         """
         Extract action parameters
         """
         parameters = CallChatGPT.getResponseDict(messages=ongoingMessages, schema=schema, **kwargs)
```

### Comparing `freegenius-0.0.95/freegenius/utils/call_gemini.py` & `freegenius-0.0.97/freegenius/utils/call_gemini.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,15 +202,15 @@
     # Auto Function Call equivalence
 
     @staticmethod
     def runGeniusCall(messages: dict, noFunctionCall: bool = False):
         user_request = messages[-1]["content"]
         if config.intent_screening:
             # 1. Intent Screening
-            noFunctionCall = True if noFunctionCall else CallGemini.screen_user_request(messages=messages, user_request=user_request)
+            noFunctionCall = True if noFunctionCall else CallGemini.isChatOnly(messages=messages, user_request=user_request)
         if noFunctionCall or config.tool_dependence <= 0.0:
             return CallGemini.regularCall(messages)
         else:
             # 2. Tool Selection
             if config.selectedTool and config.selectedTool in config.toolFunctionSchemas:
                 tool_name = config.selectedTool
                 tool_schema = config.toolFunctionSchemas[tool_name]
@@ -288,16 +288,16 @@
                     # tool function executed without chat extension
                     config.currentMessages.append({"role": "assistant", "content": config.tempContent if config.tempContent else "Done!"})
                     config.tempContent = ""
                     config.conversationStarted = True
                     return None
 
     @staticmethod
-    def screen_user_request(messages: dict, user_request: str) -> bool:
-        
+    def isChatOnly(messages: dict, user_request: str) -> bool:
+        print2("```screening")
         deviceInfo = f"""\n\nMy device information:\n{getDeviceInfo()}""" if config.includeDeviceInfoInContext else ""
         properties = {
             "answer": {
                 "type": "string",
                 "description": """Evaluate my request to determine if you are able to resolve my request as a text-based AI:
 - Answer 'no' if you are asked to execute a computing task or an online search.
 - Answer 'no' if you are asked for updates / news / real-time information.
@@ -320,15 +320,18 @@
 <request>
 {user_request}{deviceInfo}
 </request>"""
 
         history, *_ = toGeminiMessages(messages=messages)
 
         output = CallGemini.getResponseDict(history, schema=schema, userMessage=userMessage)
-        return True if "yes" in str(output).lower() else False
+        chatOnly = True if "yes" in str(output).lower() else False
+        print3(f"""Tool may {"not " if chatOnly else ""}be required.""")
+        print2("```")
+        return chatOnly
 
     @staticmethod
     def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], **kwargs) -> dict:
         """
         Extract action parameters
         """
```

### Comparing `freegenius-0.0.95/freegenius/utils/call_llamacpp.py` & `freegenius-0.0.97/freegenius/utils/call_llamacpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from freegenius import config, showErrors, get_or_create_collection, query_vectors, getDeviceInfo, isValidPythodCode, executeToolFunction, toParameterSchema
-from freegenius import print1, print2, print3, selectTool, getPythonFunctionResponse, extractPythonCode, downloadStableDiffusionFiles, screening
+from freegenius import print1, print2, print3, selectTool, getPythonFunctionResponse, extractPythonCode, downloadStableDiffusionFiles, screening, isToolRequired
 from typing import Optional
 from llama_cpp import Llama
 from prompt_toolkit import prompt
 from pathlib import Path
 from huggingface_hub import hf_hub_download
 import traceback, json, re, os, pprint, copy, datetime
-from guidance import models
 
 
 class CallLlamaCpp:
 
     @staticmethod
     def checkCompletion():
 
@@ -258,15 +257,15 @@
     # Auto Function call equivalence
 
     @staticmethod
     def runGeniusCall(messages: dict, noFunctionCall: bool = False):
         user_request = messages[-1]["content"]
         if config.intent_screening:
             # 1. Intent Screening
-            noFunctionCall = True if noFunctionCall else CallLlamaCpp.screen_user_request(messages=messages, user_request=user_request)
+            noFunctionCall = True if noFunctionCall else (not isToolRequired(user_request))
         if noFunctionCall or config.tool_dependence <= 0.0:
             return CallLlamaCpp.regularCall(messages)
         else:
             # 2. Tool Selection
             if config.selectedTool and config.selectedTool in config.toolFunctionSchemas:
                 tool_name = config.selectedTool
                 tool_schema = config.toolFunctionSchemas[tool_name]["parameters"]
@@ -347,35 +346,15 @@
                     # tool function executed without chat extension
                     config.currentMessages.append({"role": "assistant", "content": config.tempContent if config.tempContent else "Done!"})
                     config.tempContent = ""
                     config.conversationStarted = True
                     return None
 
     @staticmethod
-    def screen_user_request(messages: dict, user_request: str) -> bool:
-        lm = models.LlamaCpp(
-            config.llamacppMainModel_model_path,
-            echo = False,
-            chat_format="chatml",
-            n_ctx=config.llamacppMainModel_n_ctx,
-            n_batch=config.llamacppMainModel_n_batch,
-            verbose=config.llamacppMainModel_verbose,
-            n_gpu_layers=config.llamacppMainModel_n_gpu_layers,
-            **config.llamacppMainModel_additional_model_options,
-        )
-        try:
-            tool = screening(lm, user_request)
-        except:
-            tool = True
-        lm.reset()
-        del lm
-        return not tool
-
-    @staticmethod
-    def screen_user_request_old(messages: dict, user_request: str) -> bool:
+    def isChatOnly(messages: dict, user_request: str) -> bool:
         
         deviceInfo = f"""\n\nMy device information:\n{getDeviceInfo()}""" if config.includeDeviceInfoInContext else ""
         answer = {
             "answer": {
                 "type": "string",
                 "description": """Either 'yes' or 'no':
 - Answer 'no' if you are asked to execute a computing task.
@@ -427,14 +406,43 @@
         try:
             output = output["answer"]
         except:
             return False
         return True if (not output) or str(output).lower() == "yes" else False
 
     @staticmethod
+    def extractToolParameters_testing(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, max_tokens: Optional[int]=None, **kwargs) -> dict:
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
+            response = outputStructuredData(
+                lm=lm,
+                schema=schema,
+                json_output=False,
+                messages=ongoingMessages,
+                use_system_message=False,
+                request=userInput,
+                temperature=temperature,
+                max_tokens=max_tokens,
+            )
+        except:
+            response = {}
+        lm.reset()
+        del lm
+        return response
+
+    @staticmethod
     def extractToolParameters(schema: dict, userInput: str, ongoingMessages: list = [], temperature: Optional[float]=None, max_tokens: Optional[int]=None, **kwargs) -> dict:
         """
         Extract action parameters
         """
         schema = toParameterSchema(schema)
         schemaCopy = copy.deepcopy(schema)
```

### Comparing `freegenius-0.0.95/freegenius/utils/call_llm.py` & `freegenius-0.0.97/freegenius/utils/call_llm.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/call_ollama.py` & `freegenius-0.0.97/freegenius/utils/call_ollama.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from freegenius import showErrors, get_or_create_collection, query_vectors, getDeviceInfo, isValidPythodCode, executeToolFunction, toParameterSchema
-from freegenius import print1, print2, print3, selectTool, getPythonFunctionResponse, extractPythonCode, isValidPythodCode, downloadStableDiffusionFiles
+from freegenius import print1, print2, print3, selectTool, getPythonFunctionResponse, extractPythonCode, isValidPythodCode, downloadStableDiffusionFiles, isToolRequired
 from freegenius import config
 import shutil, re, traceback, json, ollama, pprint, copy, datetime
 from typing import Optional
 from freegenius.utils.download import Downloader
 from ollama import Options
 from prompt_toolkit import prompt
 
@@ -217,15 +217,15 @@
     @staticmethod
     def runGeniusCall(messages: dict, noFunctionCall: bool = False):
         user_request = messages[-1]["content"]
         if config.intent_screening:
             # 1. Intent Screening
             if config.developer:
                 print1("screening ...")
-            noFunctionCall = True if noFunctionCall else CallOllama.screen_user_request(messages=messages, user_request=user_request)
+            noFunctionCall = True if noFunctionCall else (not isToolRequired(user_request))
         if noFunctionCall or config.tool_dependence <= 0.0:
             return CallOllama.regularCall(messages)
         else:
             # 2. Tool Selection
             if config.selectedTool and config.selectedTool in config.toolFunctionSchemas:
                 tool_name = config.selectedTool
                 tool_schema = config.toolFunctionSchemas[tool_name]["parameters"]
@@ -302,15 +302,15 @@
                     # tool function executed without chat extension
                     config.currentMessages.append({"role": "assistant", "content": config.tempContent if config.tempContent else "Done!"})
                     config.tempContent = ""
                     config.conversationStarted = True
                     return None
 
     @staticmethod
-    def screen_user_request(messages: dict, user_request: str) -> bool:
+    def isChatOnly(messages: dict, user_request: str) -> bool:
         
         deviceInfo = f"""\n\nMy device information:\n{getDeviceInfo()}""" if config.includeDeviceInfoInContext else ""
         schema = {
             "answer": {
                 "type": "string",
                 "description": """Evaluate my request to determine if it is within your capabilities as a text-based AI:
 - Answer 'no' if you are asked to execute a computing task or an online search.
```

### Comparing `freegenius-0.0.95/freegenius/utils/config_essential.py` & `freegenius-0.0.97/freegenius/utils/config_essential.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,14 +30,22 @@
     ('intent_screening', False), # set True to increase both reliability and waiting time
     ('tool_dependence', 0.8), # range: 0.0 - 1.0; 0.0 means model's its own capabilities; 1.0; use at least one function call plugin among available tools
     ('tool_auto_selection_threshold', 0.5), # range: 0.0 - 1.0; tool auto selection is implemented when the closest tool match has a semantic distance lower than its value; manual selection from top matched tools is implemented when the closest distance fall between its value and tool_dependence
     ('tool_selection_max_choices', 4), # when tool search distance is higher than tool_auto_selection_threshold but lower than or equal to tool_dependence, manual selection implemented among the top matched tools.  This value specifies the maximum number of choices for manual tool selection in such cases.
     ('tokenizers_parallelism', 'true'), # 'true' / 'false'
     ('includeDeviceInfoInContext', False),
     ('includeIpInDeviceInfo', False),
+    ('zero_shot_classification_model', 'facebook/bart-large-mnli'),
+    ('labels_kind', ("greeting", "translation", "math", "question", "description", "command", "statement", "insturction")),
+    ('labels_information', ("common knowledge", "published content", "trained knowledge", "archived records", "historical records", "programming", "technical knowledge", "religious knowledge", "literature", "evolving data", "recent updates", "latest information", "current information", "up-to-date news", "device information", "real-time data")),
+    ('labels_action', ("calculation", "writing a text-response", "carrying out a task on your device")),
+    ('labels_kind_chat_only_options', ("greeting", "translation", "math")),
+    ('labels_kind_information_options', ("question", "description")),
+    ('labels_information_chat_only_options', ("common knowledge", "published content", "trained knowledge", "archived records", "historical records", "programming", "technical knowledge", "religious knowledge", "literature")),
+    ('labels_action_chat_only_options', ("calculation", "writing a text-response")),
     ('useAdditionalChatModel', False),
     ('stableDiffusion_verbose', False),
     ('stableDiffusion_model_path', ""),
     ('stableDiffusion_output_width', 512),
     ('stableDiffusion_output_height', 512),
     ('autogenstudio_server_port', 8081),
     ('ollamaVisionModel', 'llava'), # ollama model used for vision
```

### Comparing `freegenius-0.0.95/freegenius/utils/config_tools.py` & `freegenius-0.0.97/freegenius/utils/config_tools.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/download.py` & `freegenius-0.0.97/freegenius/utils/download.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/get_path_prompt.py` & `freegenius-0.0.97/freegenius/utils/get_path_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/ollama_models.py` & `freegenius-0.0.97/freegenius/utils/ollama_models.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/promptValidator.py` & `freegenius-0.0.97/freegenius/utils/promptValidator.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/prompt_multiline_shared_key_bindings.py` & `freegenius-0.0.97/freegenius/utils/prompt_multiline_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/prompt_shared_key_bindings.py` & `freegenius-0.0.97/freegenius/utils/prompt_shared_key_bindings.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/prompts.py` & `freegenius-0.0.97/freegenius/utils/prompts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/python_utils.py` & `freegenius-0.0.97/freegenius/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/shared_utils.py` & `freegenius-0.0.97/freegenius/utils/shared_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from freegenius import config
 from freegenius.utils.terminal_mode_dialogs import TerminalModeDialogs
 import sys, os, geocoder, platform, socket, geocoder, datetime, requests, netifaces, getpass, pendulum, pkg_resources, webbrowser, unicodedata
-import traceback, uuid, re, textwrap, signal, wcwidth, shutil, threading, time, tiktoken, subprocess, json, base64, html2text, pydoc
+import traceback, uuid, re, textwrap, signal, wcwidth, shutil, threading, time, tiktoken, subprocess, json, base64, html2text, pydoc, codecs
 from packaging import version
 from chromadb.utils import embedding_functions
 from pygments.styles import get_style_by_name
 from prompt_toolkit.styles.pygments import style_from_pygments_cls
 from prompt_toolkit import print_formatted_text, HTML
 from prompt_toolkit import prompt
 from typing import Optional, Any
@@ -14,22 +14,58 @@
 from PIL import Image
 from openai import OpenAI
 from huggingface_hub import hf_hub_download
 from bs4 import BeautifulSoup
 from urllib.parse import quote
 from guidance import select, gen
 from typing import Union
+from transformers import pipeline
+
 
 # non-Android only
 if not config.isTermux:
     from autogen.retrieve_utils import TEXT_FORMATS
 
 # a dummy import line to resolve ALSA error display on Linux
 import sounddevice
 
+# transformers
+
+def classify(user_input, candidate_labels):
+    classifier = pipeline(task="zero-shot-classification", model=config.zero_shot_classification_model)
+    response = classifier(
+        user_input,
+        candidate_labels=candidate_labels,
+    )
+    labels = response["labels"]
+    return labels[0]
+
+def isToolRequired(user_input) -> bool:
+    tool = True
+    print2("```screening")
+    # check the kind of input
+    kind = classify(user_input, config.labels_kind)
+    print3(f"Kind: {kind}")
+    if kind in config.labels_kind_chat_only_options:
+        tool = False
+    elif kind in config.labels_kind_information_options:
+        # check the nature of the requested information
+        information = classify(user_input, config.labels_information)
+        print3(f"Information: {information}")
+        if information in config.labels_information_chat_only_options:
+            tool = False
+    else:
+        # check the nature of the requested response
+        action = classify(user_input, config.labels_action)
+        print3(f"Action: {action}")
+        if action in config.labels_action_chat_only_options:
+            tool = False
+    print3(f"""Comment: Tool may {"" if tool else "not "}be required.""")
+    print2("```")
+    return tool
 
 # guidance
 
 def screening(lm, user_input) -> bool:
     tool = False
 
     print2("```screening")
@@ -81,18 +117,18 @@
     print3(f"""Comment: Tool may {"" if tool else "not "}be required.""")
     print2("```")
 
     return tool
 
 def outputStructuredData(lm, schema: dict, json_output: bool=False, messages: list = [], use_system_message: bool=True, request: str="", temperature: Optional[float]=None, max_tokens: Optional[int]=None, **kwargs) -> Union[dict, str]:
     properties = toParameterSchema(schema)["properties"]
+    request = f", particularly related to the following request:\n{request}" if request else "."
     lm += toChatml(messages, use_system_message=use_system_message).rstrip()
     lm += f"""<|im_start|>assistant.
-I am answering your questions based on the content in our conversation given above, particularly related to the following request:
-{request}
+I am answering your questions based on the content in our conversation given above{request}
 <|im_end|>
 """
     for key, value in properties.items():
         description = value["description"].replace("\n", " ")
         if "enum" in value:
             options = value["enum"]
             options_str = "', '".join(value["enum"])
@@ -103,15 +139,15 @@
 <|im_start|>assistant
 Answer: {select(options, name=key) if "enum" in value else gen(name=key, stop="<")}
 <|im_end|>
 '''
 
     response = {}
     for i in properties:
-        response[i] = lm.get(i, "").rstrip()
+        response[i] = codecs.decode(lm.get(i, "").rstrip(), "unicode_escape")
     return json.dumps(response) if json_output else response
 
 def select_tool(lm, user_input):
     tool_names = list(config.toolFunctionSchemas.keys())
     tools = {i:config.toolFunctionSchemas[i]["description"] for i in config.toolFunctionSchemas}
 
     lm += f"""<|im_start|>user
```

### Comparing `freegenius-0.0.95/freegenius/utils/shortcuts.py` & `freegenius-0.0.97/freegenius/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/single_prompt.py` & `freegenius-0.0.97/freegenius/utils/single_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/streaming_word_wrapper.py` & `freegenius-0.0.97/freegenius/utils/streaming_word_wrapper.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/sttLanguages.py` & `freegenius-0.0.97/freegenius/utils/sttLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/terminal_mode_dialogs.py` & `freegenius-0.0.97/freegenius/utils/terminal_mode_dialogs.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/terminal_system_command_prompt.py` & `freegenius-0.0.97/freegenius/utils/terminal_system_command_prompt.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/text_utils.py` & `freegenius-0.0.97/freegenius/utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/tool_plugins.py` & `freegenius-0.0.97/freegenius/utils/tool_plugins.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/ttsLanguages.py` & `freegenius-0.0.97/freegenius/utils/ttsLanguages.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/tts_utils.py` & `freegenius-0.0.97/freegenius/utils/tts_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius/utils/vlc_utils.py` & `freegenius-0.0.97/freegenius/utils/vlc_utils.py`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius.egg-info/PKG-INFO` & `freegenius-0.0.97/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freegenius
-Version: 0.0.95
+Version: 0.0.97
 Summary: FreeGenius AI, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.
 Home-page: https://letmedoit.ai
 Author: Eliran Wong
 Author-email: support@letmedoit.ai
 License: GNU General Public License (GPL)
 Project-URL: Source, https://github.com/eliranwong/letmedoit
 Project-URL: Tracker, https://github.com/eliranwong/letmedoit/issues
@@ -18,21 +18,84 @@
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <3.12
+Requires-Dist: openai==1.19.0
+Requires-Dist: requests
+Requires-Dist: argparse
+Requires-Dist: pendulum
+Requires-Dist: folium
+Requires-Dist: seaborn[stats]
+Requires-Dist: sympy
+Requires-Dist: numpy
+Requires-Dist: prompt_toolkit
+Requires-Dist: Pygments
+Requires-Dist: datetime
+Requires-Dist: netifaces
+Requires-Dist: geocoder
+Requires-Dist: googlesearch-python
+Requires-Dist: art
+Requires-Dist: apsw
+Requires-Dist: gTTS
+Requires-Dist: google-cloud-speech
+Requires-Dist: google-cloud-texttospeech
+Requires-Dist: google-cloud-aiplatform==1.47.0
+Requires-Dist: pywhatkit
+Requires-Dist: yt-dlp
+Requires-Dist: rembg
+Requires-Dist: qrcode
+Requires-Dist: pyperclip
+Requires-Dist: colorama
+Requires-Dist: pillow
+Requires-Dist: docker
+Requires-Dist: einops
+Requires-Dist: transformers==4.40.1
+Requires-Dist: torch==2.2.2
+Requires-Dist: torchvision==0.17.2
+Requires-Dist: sentence-transformers
+Requires-Dist: chromadb==0.4.24
+Requires-Dist: unstructured[all-docs]
+Requires-Dist: pyautogen[autobuild,retrievechat]==0.2.24
+Requires-Dist: autogenstudio==0.0.56
+Requires-Dist: tiktoken
+Requires-Dist: pygame
+Requires-Dist: PySide6
+Requires-Dist: feedparser
+Requires-Dist: html2text
+Requires-Dist: pypdf
+Requires-Dist: PyMuPDF
+Requires-Dist: yfinance
+Requires-Dist: setuptools-rust
+Requires-Dist: SpeechRecognition
+Requires-Dist: openai-whisper
+Requires-Dist: soundfile==0.12.1
+Requires-Dist: sounddevice==0.4.6
+Requires-Dist: elevenlabs==1.0.3
+Requires-Dist: ollama==0.1.8
+Requires-Dist: llama-cpp-python[server]==0.2.61
+Requires-Dist: huggingface-hub
+Requires-Dist: langchain==0.1.13
+Requires-Dist: langchain_openai==0.1.3
+Requires-Dist: pydub
+Requires-Dist: stable-diffusion-cpp-python
+Requires-Dist: pytz
+Requires-Dist: geopy
+Requires-Dist: guidance==0.1.13
 
 # FreeGenius AI
 
 FreeGenius AI is an ambitious project sparked by the pioneering work of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). It's designed with the primary objective of offering a comprehensive suite of AI solutions that mirror the capabilities of [LetMeDoIt AI](https://github.com/eliranwong/letmedoit). However, FreeGenius AI is remarkably different in that all core features are completely free, and it doesn't require the use of an OpenAI key.
 
 As with [LetMeDoIt AI](https://github.com/eliranwong/letmedoit), FreeGenius AI is designed to be capable of engaging in intuitive conversations, executing codes, providing up-to-date information, and performing a wide range of tasks. It's designed to learn, adapt, and grow with the user, offering personalized experiences and interactions.
 
+![freegenius_ai_screenshot](https://github.com/eliranwong/freegenius/assets/25262722/1e9dd18e-aa4b-4e2c-8d76-386af7ba00ea)
+
 # Beyond LetMeDoIt AI
 
 https://github.com/eliranwong/freegenius/wiki/Beyond-LetMeDoIt-AI
 
 # Goals
 
 The author aims to equip FreeGenius AI, as an AI suite that is able to:
@@ -96,14 +159,18 @@
 ## Speech-to-Text Options
 
 1. Google Text-to-Speech (Generic)
 2. Google Text-to-Speech (API)
 3. Elevenlabs (API)
 4. Custom system commands
 
+# Highly Customizable
+
+![plugins](https://github.com/eliranwong/freegenius/assets/25262722/6bb4b2f6-5684-42c1-95e3-7b12c3a38db6)
+
 # Installation
 
 Install FreeGenius AI, by running:
 
 To set up virtual environment (recommended):
 
 > mkdir -p ~/apps/freegenius
```

### Comparing `freegenius-0.0.95/freegenius.egg-info/SOURCES.txt` & `freegenius-0.0.97/freegenius.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius.egg-info/entry_points.txt` & `freegenius-0.0.97/freegenius.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `freegenius-0.0.95/freegenius.egg-info/requires.txt` & `freegenius-0.0.97/freegenius.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 rembg
 qrcode
 pyperclip
 colorama
 pillow
 docker
 einops
-transformers
+transformers==4.40.1
 torch==2.2.2
 torchvision==0.17.2
 sentence-transformers
 chromadb==0.4.24
 unstructured[all-docs]
 pyautogen[autobuild,retrievechat]==0.2.24
 autogenstudio==0.0.56
@@ -49,12 +49,13 @@
 soundfile==0.12.1
 sounddevice==0.4.6
 elevenlabs==1.0.3
 ollama==0.1.8
 llama-cpp-python[server]==0.2.61
 huggingface-hub
 langchain==0.1.13
+langchain_openai==0.1.3
 pydub
 stable-diffusion-cpp-python
 pytz
 geopy
 guidance==0.1.13
```

### Comparing `freegenius-0.0.95/setup.py` & `freegenius-0.0.97/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 # make sure config.py is empty
 open(os.path.join(package, "config.py"), "w").close()
 
 # https://packaging.python.org/en/latest/guides/distributing-packages-using-setuptools/
 setup(
     name=package,
-    version="0.0.95",
+    version="0.0.97",
     python_requires=">=3.8, <3.12",
     description=f"{appFullName}, an advanced AI assistant that can talk and take multi-step actions. Supports numerous open-source LLMs via Llama.cpp or Ollama, with optional integration with AutoGen agents, OpenAI API, Google Gemini Pro and unlimited plugins.",
     long_description=long_description,
     author="Eliran Wong",
     author_email="support@letmedoit.ai",
     cmdclass={
         'install': PreInstallCommand,
```

