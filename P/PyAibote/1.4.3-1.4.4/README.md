# Comparing `tmp/PyAibote-1.4.3.tar.gz` & `tmp/PyAibote-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyAibote-1.4.3.tar", last modified: Mon Apr 22 14:11:38 2024, max compression
+gzip compressed data, was "PyAibote-1.4.4.tar", last modified: Thu Apr 25 13:24:19 2024, max compression
```

## Comparing `PyAibote-1.4.3.tar` & `PyAibote-1.4.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 14:11:38.153920 PyAibote-1.4.3/
--rw-rw-rw-   0        0        0     1089 2024-04-22 14:11:38.075918 PyAibote-1.4.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-22 14:11:37.417934 PyAibote-1.4.3/PyAibote/
--rw-rw-rw-   0        0        0     2788 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/AndroidBot.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:11:37.628938 PyAibote-1.4.3/PyAibote/AndroidBotModel/
--rw-rw-rw-   0        0        0     7584 2024-04-22 14:02:06.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
--rw-rw-rw-   0        0        0     2381 2024-04-22 13:58:45.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/AndroidLoadWait.py
--rw-rw-rw-   0        0        0     2924 2024-04-22 14:05:12.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/ColorFindingOperation.py
--rw-rw-rw-   0        0        0     6152 2024-04-22 14:05:18.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/Control.py
--rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/CoordinateOperation.py
--rw-rw-rw-   0        0        0    12733 2024-04-22 14:05:28.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0    17545 2024-04-22 14:05:53.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/EquipmentOperation.py
--rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/FileTransfer.py
--rw-rw-rw-   0        0        0     8092 2024-04-22 14:06:01.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/MapFindingOperation.py
--rw-rw-rw-   0        0        0     9064 2024-04-22 14:06:06.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/OcrCorrelation.py
--rw-rw-rw-   0        0        0      949 2024-04-22 14:06:12.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
--rw-rw-rw-   0        0        0     9217 2024-04-22 14:06:16.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/ScreenshotOperation.py
--rw-rw-rw-   0        0        0     1926 2024-04-22 14:06:20.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/UrlRequest.py
--rw-rw-rw-   0        0        0     4218 2024-04-22 14:06:28.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     1781 2024-04-22 14:06:33.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/YoloService.py
--rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.4.3/PyAibote/AndroidBotModel/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:11:37.632937 PyAibote-1.4.3/PyAibote/CommonUse/
--rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.4.3/PyAibote/CommonUse/ChatGenerative.py
--rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.4.3/PyAibote/CommonUse/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:11:37.723920 PyAibote-1.4.3/PyAibote/Tool/
--rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/Tool/DatabaseFunc.py
--rw-rw-rw-   0        0        0     2188 2024-03-19 01:39:35.000000 PyAibote-1.4.3/PyAibote/Tool/DebugStartDriver.py
--rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/Tool/Logger.py
--rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/Tool/LoggerFunc.py
--rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/Tool/SendTcpData.py
--rw-rw-rw-   0        0        0      532 2024-01-13 09:10:40.000000 PyAibote-1.4.3/PyAibote/Tool/SocketServer.py
--rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/Tool/Sqlite3DataBase.py
--rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.4.3/PyAibote/Tool/UniversalFunction.py
--rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/Tool/WriteReadFileFunc.py
--rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/Tool/__init__.py
--rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/WebBot.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:11:37.857918 PyAibote-1.4.3/PyAibote/WebBotModel/
--rw-rw-rw-   0        0        0     3465 2024-04-22 14:07:39.000000 PyAibote-1.4.3/PyAibote/WebBotModel/CookiesOperation.py
--rw-rw-rw-   0        0        0      892 2024-04-22 14:07:49.000000 PyAibote-1.4.3/PyAibote/WebBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    11034 2024-04-22 14:07:57.000000 PyAibote-1.4.3/PyAibote/WebBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.4.3/PyAibote/WebBotModel/IframeOperation.py
--rw-rw-rw-   0        0        0      804 2024-04-22 14:08:02.000000 PyAibote-1.4.3/PyAibote/WebBotModel/JSinjection.py
--rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.4.3/PyAibote/WebBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     3649 2024-04-22 14:08:09.000000 PyAibote-1.4.3/PyAibote/WebBotModel/PagesAndNavigation.py
--rw-rw-rw-   0        0        0     1005 2024-04-22 14:02:29.000000 PyAibote-1.4.3/PyAibote/WebBotModel/PopUpWindow.py
--rw-rw-rw-   0        0        0     3421 2024-04-22 07:22:21.000000 PyAibote-1.4.3/PyAibote/WebBotModel/WebLoadWait.py
--rw-rw-rw-   0        0        0     5518 2024-04-22 14:08:16.000000 PyAibote-1.4.3/PyAibote/WebBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.4.3/PyAibote/WebBotModel/__init__.py
--rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.4.3/PyAibote/WindowsBot.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:11:38.074918 PyAibote-1.4.3/PyAibote/WindowsBotModel/
--rw-rw-rw-   0        0        0    19762 2024-04-22 14:08:25.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/ColorOperation.py
--rw-rw-rw-   0        0        0    21461 2024-03-28 05:02:42.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/DigitalHumanOperation.py
--rw-rw-rw-   0        0        0     1756 2024-04-22 14:02:44.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/DrivingOperation.py
--rw-rw-rw-   0        0        0    13246 2024-04-22 14:08:33.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/ElementOperation.py
--rw-rw-rw-   0        0        0     4863 2024-04-22 14:03:06.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/ExcelOperation.py
--rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/KeymouseOperation.py
--rw-rw-rw-   0        0        0     8223 2024-04-22 14:03:16.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/OcrOperation.py
--rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/OtherOperations.py
--rw-rw-rw-   0        0        0     2293 2024-04-22 14:03:22.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/SystemOperation.py
--rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/VerificationCodeOperation.py
--rw-rw-rw-   0        0        0     6058 2024-04-22 14:03:35.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/VoiceService.py
--rw-rw-rw-   0        0        0     7427 2024-04-22 14:03:52.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/WinHidCorrelation.py
--rw-rw-rw-   0        0        0     2412 2024-04-22 07:22:40.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/WinLoadWait.py
--rw-rw-rw-   0        0        0     8331 2024-04-22 14:08:39.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/WindowOperation.py
--rw-rw-rw-   0        0        0     2764 2024-04-22 14:03:57.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/YoloOperation.py
--rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.4.3/PyAibote/WindowsBotModel/__init__.py
--rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.4.3/PyAibote/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 14:11:37.442937 PyAibote-1.4.3/PyAibote.egg-info/
--rw-rw-rw-   0        0        0     1089 2024-04-22 14:11:37.000000 PyAibote-1.4.3/PyAibote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2493 2024-04-22 14:11:37.000000 PyAibote-1.4.3/PyAibote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 14:11:37.000000 PyAibote-1.4.3/PyAibote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2024-04-22 14:11:37.000000 PyAibote-1.4.3/PyAibote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-04-22 14:11:37.000000 PyAibote-1.4.3/PyAibote.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     9118 2024-04-11 10:04:43.000000 PyAibote-1.4.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 14:11:38.153920 PyAibote-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1425 2024-04-22 14:11:06.000000 PyAibote-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:24:19.401428 PyAibote-1.4.4/
+-rw-rw-rw-   0        0        0     1089 2024-04-25 13:24:19.400431 PyAibote-1.4.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-25 13:24:19.006739 PyAibote-1.4.4/PyAibote/
+-rw-rw-rw-   0        0        0     2679 2024-04-25 13:20:13.000000 PyAibote-1.4.4/PyAibote/AndroidBot.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:24:19.109734 PyAibote-1.4.4/PyAibote/AndroidBotModel/
+-rw-rw-rw-   0        0        0     7584 2024-04-22 14:02:06.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/AndroidHidCorrelation.py
+-rw-rw-rw-   0        0        0     2381 2024-04-22 13:58:45.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/AndroidLoadWait.py
+-rw-rw-rw-   0        0        0     2924 2024-04-22 14:05:12.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/ColorFindingOperation.py
+-rw-rw-rw-   0        0        0     6152 2024-04-22 14:05:18.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/Control.py
+-rw-rw-rw-   0        0        0     5580 2024-03-19 01:39:35.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/CoordinateOperation.py
+-rw-rw-rw-   0        0        0    12733 2024-04-22 14:05:28.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0    17545 2024-04-22 14:05:53.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/EquipmentOperation.py
+-rw-rw-rw-   0        0        0     3094 2024-01-17 08:25:14.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/FileTransfer.py
+-rw-rw-rw-   0        0        0     8092 2024-04-22 14:06:01.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/MapFindingOperation.py
+-rw-rw-rw-   0        0        0     9064 2024-04-22 14:06:06.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/OcrCorrelation.py
+-rw-rw-rw-   0        0        0      949 2024-04-22 14:06:12.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/ScreenProjectionOperation.py
+-rw-rw-rw-   0        0        0     9217 2024-04-22 14:06:16.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/ScreenshotOperation.py
+-rw-rw-rw-   0        0        0     1926 2024-04-22 14:06:20.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/UrlRequest.py
+-rw-rw-rw-   0        0        0     4218 2024-04-22 14:06:28.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     1781 2024-04-22 14:06:33.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/YoloService.py
+-rw-rw-rw-   0        0        0     1088 2024-02-27 23:24:38.000000 PyAibote-1.4.4/PyAibote/AndroidBotModel/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:24:19.142376 PyAibote-1.4.4/PyAibote/CommonUse/
+-rw-rw-rw-   0        0        0     2101 2024-02-15 23:31:42.000000 PyAibote-1.4.4/PyAibote/CommonUse/ChatGenerative.py
+-rw-rw-rw-   0        0        0        0 2024-02-27 23:33:36.000000 PyAibote-1.4.4/PyAibote/CommonUse/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:24:19.237430 PyAibote-1.4.4/PyAibote/Tool/
+-rw-rw-rw-   0        0        0     5457 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/Tool/DatabaseFunc.py
+-rw-rw-rw-   0        0        0     2188 2024-03-19 01:39:35.000000 PyAibote-1.4.4/PyAibote/Tool/DebugStartDriver.py
+-rw-rw-rw-   0        0        0     2223 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/Tool/Logger.py
+-rw-rw-rw-   0        0        0     1749 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/Tool/LoggerFunc.py
+-rw-rw-rw-   0        0        0      912 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/Tool/SendTcpData.py
+-rw-rw-rw-   0        0        0      992 2024-04-25 13:18:13.000000 PyAibote-1.4.4/PyAibote/Tool/SocketServer.py
+-rw-rw-rw-   0        0        0     3342 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/Tool/Sqlite3DataBase.py
+-rw-rw-rw-   0        0        0      660 2024-01-18 08:34:16.000000 PyAibote-1.4.4/PyAibote/Tool/UniversalFunction.py
+-rw-rw-rw-   0        0        0     4364 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/Tool/WriteReadFileFunc.py
+-rw-rw-rw-   0        0        0      550 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/Tool/__init__.py
+-rw-rw-rw-   0        0        0     1998 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/WebBot.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:24:19.305431 PyAibote-1.4.4/PyAibote/WebBotModel/
+-rw-rw-rw-   0        0        0     3465 2024-04-22 14:07:39.000000 PyAibote-1.4.4/PyAibote/WebBotModel/CookiesOperation.py
+-rw-rw-rw-   0        0        0      892 2024-04-22 14:07:49.000000 PyAibote-1.4.4/PyAibote/WebBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    11034 2024-04-22 14:07:57.000000 PyAibote-1.4.4/PyAibote/WebBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0      697 2024-01-12 10:05:13.000000 PyAibote-1.4.4/PyAibote/WebBotModel/IframeOperation.py
+-rw-rw-rw-   0        0        0      804 2024-04-22 14:08:02.000000 PyAibote-1.4.4/PyAibote/WebBotModel/JSinjection.py
+-rw-rw-rw-   0        0        0     3592 2024-01-26 00:38:04.000000 PyAibote-1.4.4/PyAibote/WebBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     3649 2024-04-22 14:08:09.000000 PyAibote-1.4.4/PyAibote/WebBotModel/PagesAndNavigation.py
+-rw-rw-rw-   0        0        0     1005 2024-04-22 14:02:29.000000 PyAibote-1.4.4/PyAibote/WebBotModel/PopUpWindow.py
+-rw-rw-rw-   0        0        0     3421 2024-04-22 07:22:21.000000 PyAibote-1.4.4/PyAibote/WebBotModel/WebLoadWait.py
+-rw-rw-rw-   0        0        0     5548 2024-04-24 07:42:11.000000 PyAibote-1.4.4/PyAibote/WebBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0      654 2024-02-15 23:42:13.000000 PyAibote-1.4.4/PyAibote/WebBotModel/__init__.py
+-rw-rw-rw-   0        0        0     4186 2024-03-19 01:40:59.000000 PyAibote-1.4.4/PyAibote/WindowsBot.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:24:19.398437 PyAibote-1.4.4/PyAibote/WindowsBotModel/
+-rw-rw-rw-   0        0        0    19762 2024-04-22 14:08:25.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/ColorOperation.py
+-rw-rw-rw-   0        0        0    21461 2024-03-28 05:02:42.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/DigitalHumanOperation.py
+-rw-rw-rw-   0        0        0     1756 2024-04-22 14:02:44.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/DrivingOperation.py
+-rw-rw-rw-   0        0        0    13246 2024-04-22 14:08:33.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/ElementOperation.py
+-rw-rw-rw-   0        0        0     4863 2024-04-22 14:03:06.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/ExcelOperation.py
+-rw-rw-rw-   0        0        0     6629 2024-01-13 17:47:39.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/KeymouseOperation.py
+-rw-rw-rw-   0        0        0     8223 2024-04-22 14:03:16.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/OcrOperation.py
+-rw-rw-rw-   0        0        0      703 2024-01-15 07:27:07.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/OtherOperations.py
+-rw-rw-rw-   0        0        0     2293 2024-04-22 14:03:22.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/SystemOperation.py
+-rw-rw-rw-   0        0        0     5962 2024-01-22 23:03:02.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/VerificationCodeOperation.py
+-rw-rw-rw-   0        0        0     6058 2024-04-22 14:03:35.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/VoiceService.py
+-rw-rw-rw-   0        0        0     7427 2024-04-22 14:03:52.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/WinHidCorrelation.py
+-rw-rw-rw-   0        0        0     2412 2024-04-22 07:22:40.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/WinLoadWait.py
+-rw-rw-rw-   0        0        0     8331 2024-04-22 14:08:39.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/WindowOperation.py
+-rw-rw-rw-   0        0        0     2764 2024-04-22 14:03:57.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/YoloOperation.py
+-rw-rw-rw-   0        0        0     1115 2024-02-15 23:42:02.000000 PyAibote-1.4.4/PyAibote/WindowsBotModel/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-02-27 10:41:36.000000 PyAibote-1.4.4/PyAibote/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 13:24:19.033736 PyAibote-1.4.4/PyAibote.egg-info/
+-rw-rw-rw-   0        0        0     1089 2024-04-25 13:24:18.000000 PyAibote-1.4.4/PyAibote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2493 2024-04-25 13:24:18.000000 PyAibote-1.4.4/PyAibote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 13:24:18.000000 PyAibote-1.4.4/PyAibote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2024-04-25 13:24:18.000000 PyAibote-1.4.4/PyAibote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-25 13:24:18.000000 PyAibote-1.4.4/PyAibote.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9118 2024-04-11 10:04:43.000000 PyAibote-1.4.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-25 13:24:19.401428 PyAibote-1.4.4/setup.cfg
+-rw-rw-rw-   0        0        0     1425 2024-04-25 13:24:08.000000 PyAibote-1.4.4/setup.py
```

### Comparing `PyAibote-1.4.3/PKG-INFO` & `PyAibote-1.4.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.4.3
+Version: 1.4.4
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBot.py` & `PyAibote-1.4.4/PyAibote/AndroidBot.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,15 @@
     def handle(self):
         self.info(f"<-<- Client connection at {self.client_address[0]}: {self.client_address[1]}")
         self.debug(f"<-<- Client connection at {self.client_address[0]}: {self.client_address[1]}")
         self.script_main()
 
 
     @classmethod
-    def execute(self, IP: str, Port: int):
-        if Port < 0 or Port > 65535:
-            raise OSError("`listen_port` must be in 0-65535.")
-
+    def execute(self, IP: str, Port):
         ThreadingTCPServer.StartThreadingTCPServer(self, IP, Port)
```

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/AndroidHidCorrelation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/AndroidHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/AndroidLoadWait.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/AndroidLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/ColorFindingOperation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/ColorFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/Control.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/Control.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/CoordinateOperation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/CoordinateOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/ElementOperation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/EquipmentOperation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/EquipmentOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/FileTransfer.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/FileTransfer.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/MapFindingOperation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/MapFindingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/OcrCorrelation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/OcrCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/ScreenProjectionOperation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/ScreenProjectionOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/ScreenshotOperation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/ScreenshotOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/UrlRequest.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/UrlRequest.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/VerificationCodeOperation.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/YoloService.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/YoloService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/AndroidBotModel/__init__.py` & `PyAibote-1.4.4/PyAibote/AndroidBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/CommonUse/ChatGenerative.py` & `PyAibote-1.4.4/PyAibote/CommonUse/ChatGenerative.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/DatabaseFunc.py` & `PyAibote-1.4.4/PyAibote/Tool/DatabaseFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/DebugStartDriver.py` & `PyAibote-1.4.4/PyAibote/Tool/DebugStartDriver.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/Logger.py` & `PyAibote-1.4.4/PyAibote/Tool/Logger.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/LoggerFunc.py` & `PyAibote-1.4.4/PyAibote/Tool/LoggerFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/SendTcpData.py` & `PyAibote-1.4.4/PyAibote/Tool/SendTcpData.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/Sqlite3DataBase.py` & `PyAibote-1.4.4/PyAibote/Tool/Sqlite3DataBase.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/UniversalFunction.py` & `PyAibote-1.4.4/PyAibote/Tool/UniversalFunction.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/WriteReadFileFunc.py` & `PyAibote-1.4.4/PyAibote/Tool/WriteReadFileFunc.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/Tool/__init__.py` & `PyAibote-1.4.4/PyAibote/Tool/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBot.py` & `PyAibote-1.4.4/PyAibote/WebBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/CookiesOperation.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/CookiesOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/DrivingOperation.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/ElementOperation.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/IframeOperation.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/IframeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/JSinjection.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/JSinjection.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/KeymouseOperation.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/PagesAndNavigation.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/PagesAndNavigation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/PopUpWindow.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/PopUpWindow.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/WebLoadWait.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/WebLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/WindowOperation.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/WindowOperation.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,24 +20,25 @@
         response = response.replace("\n","").replace("\t","")
 
         if response == "null":
             return None
         response = json.loads(response)
         return response
 
-    def set_window_pos(self, status, left: float = 0, top: float = 0, width: float = 0, height: float = 0) -> bool:
+    def set_window_pos(self, status: str = "normal", left: float = 0, top: float = 0, width: float = 0, height: float = 0) -> bool:
         """
             设置窗口位置和窗口大小窗口状态
             Set window position and window size window state
 
+            status: 正常:"normal"  最小化:"minimized"  最大化:"maximized"  全屏:"fullscreen"
             left:   浏览器相对于与Windows窗口左上角X坐标点     可选参数，浏览器窗口位置，此参数仅 status 值为 "normal" 时有效
             top:    浏览器相对于与Windows窗口左上角Y坐标点     可选参数，浏览器窗口位置，此参数仅 status 值为 "normal" 时有效
             width:  浏览器本身宽度                           可选参数，浏览器窗口位置，此参数仅 status 值为 "normal" 时有效
             height: 浏览器本身高度                           可选参数，浏览器窗口位置，此参数仅 windowState 值为 "normal" 时有效
-            status: 正常:"normal"  最小化:"minimized"  最大化:"maximized"  全屏:"fullscreen"
+            
             return: 布尔值
 
             left: an optional parameter, browser window position, relative to the X coordinate point in the upper left corner of the Windows window. This parameter is only valid when the status value is "normal"
             top: the optional parameter of the browser relative to the Y coordinate point in the upper left corner of the Windows window, and the browser window position. This parameter is only valid when the status value is "normal"
             width: optional parameter of browser width and browser window position. This parameter is only valid when the status value is "normal"
             height: optional parameter of browser height and browser window position. This parameter is only valid when the value of windowState is "normal"
             status: normal: "normal" minimize: "minimized" maximize: "maximized" fullscreen: "full screen"
```

### Comparing `PyAibote-1.4.3/PyAibote/WebBotModel/__init__.py` & `PyAibote-1.4.4/PyAibote/WebBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBot.py` & `PyAibote-1.4.4/PyAibote/WindowsBot.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/ColorOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/ColorOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/DigitalHumanOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/DigitalHumanOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/DrivingOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/DrivingOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/ElementOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/ElementOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/ExcelOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/ExcelOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/KeymouseOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/KeymouseOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/OcrOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/OcrOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/OtherOperations.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/OtherOperations.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/SystemOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/SystemOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/VerificationCodeOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/VerificationCodeOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/VoiceService.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/VoiceService.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/WinHidCorrelation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/WinHidCorrelation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/WinLoadWait.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/WinLoadWait.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/WindowOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/WindowOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/YoloOperation.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/YoloOperation.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote/WindowsBotModel/__init__.py` & `PyAibote-1.4.4/PyAibote/WindowsBotModel/__init__.py`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/PyAibote.egg-info/PKG-INFO` & `PyAibote-1.4.4/PyAibote.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyAibote
-Version: 1.4.3
+Version: 1.4.4
 Summary: A pure code RPA office automation framework, which supports Android, Browser and Windows
 Home-page: https://www.pyaibote.com
 Author: Riven
 Author-email: pyaibote@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.7,<4.0
```

### Comparing `PyAibote-1.4.3/PyAibote.egg-info/SOURCES.txt` & `PyAibote-1.4.4/PyAibote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/README.md` & `PyAibote-1.4.4/README.md`

 * *Files identical despite different names*

### Comparing `PyAibote-1.4.3/setup.py` & `PyAibote-1.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "Pillow",
     "requests",
     "pymysql"
 ]
 
 setup(
     name="PyAibote", 
-    version="1.4.3", 
+    version="1.4.4", 
     author="Riven", 
     author_email="pyaibote@163.com", 
     description="A pure code RPA office automation framework, which supports Android, Browser and Windows", 
     long_description="Support Android native APP and H5 interface elements and color positioning. The speed of element location is 10 times that of Appium framework, and the color location of 2340*1080 image only takes 50 milliseconds, It supports the positioning of window interface elements and colors developed by Windows applications,. NET, WinForm, WPF, QT, Java (GUI libraries such JAVA(Swing and AWT) and Electron. The exclusive xpath algorithm is concise and rapid, and the positioning speed of elements/colors is 3 times and 20 times that of visual RPA, respectively, All browsers and applications that support the chromium kernel. A web automation framework developed by C/C++ language based on browser kernel protocol. Ten times faster than Selenium", # 加载read_me的内容
     long_description_content_type="text/markdown", 
     url="https://www.pyaibote.com",  
     packages=packages,
```

