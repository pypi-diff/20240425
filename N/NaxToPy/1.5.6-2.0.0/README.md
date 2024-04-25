# Comparing `tmp/NaxToPy-1.5.6.tar.gz` & `tmp/naxtopy-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NaxToPy-1.5.6.tar", last modified: Wed Mar 13 14:42:58 2024, max compression
+gzip compressed data, was "naxtopy-2.0.0.tar", last modified: Fri Apr 19 07:28:20 2024, max compression
```

## Comparing `NaxToPy-1.5.6.tar` & `naxtopy-2.0.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.963428 NaxToPy-1.5.6/
--rw-rw-rw-   0        0        0     5368 2023-10-30 12:44:44.000000 NaxToPy-1.5.6/LICENSE
--rw-rw-rw-   0        0        0    20934 2024-03-13 14:42:57.968821 NaxToPy-1.5.6/PKG-INFO
--rw-rw-rw-   0        0        0    13792 2024-03-13 14:40:16.000000 NaxToPy-1.5.6/README.md
--rw-rw-rw-   0        0        0     1143 2024-03-13 14:41:27.000000 NaxToPy-1.5.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-13 14:42:57.980062 NaxToPy-1.5.6/setup.cfg
--rw-rw-rw-   0        0        0      462 2024-01-18 10:36:31.000000 NaxToPy-1.5.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.446428 NaxToPy-1.5.6/src/
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.451428 NaxToPy-1.5.6/src/NaxToPy/
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.462428 NaxToPy-1.5.6/src/NaxToPy/Core/
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.454428 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/
--rw-rw-rw-   0        0        0      765 2024-02-13 12:32:13.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/AllClasses.py
--rw-rw-rw-   0        0        0    24827 2024-02-13 12:32:13.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PComponent.py
--rw-rw-rw-   0        0        0     4555 2023-12-18 10:36:26.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PConnector.py
--rw-rw-rw-   0        0        0     2006 2023-12-18 10:36:26.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PCoord.py
--rw-rw-rw-   0        0        0     6775 2023-12-18 10:36:26.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PElement.py
--rw-rw-rw-   0        0        0     6100 2023-12-18 10:36:26.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PFreeBody.py
--rw-rw-rw-   0        0        0     3543 2023-12-18 10:36:26.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PIncrement.py
--rw-rw-rw-   0        0        0    12594 2024-02-20 15:26:51.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PLoadCase.py
--rw-rw-rw-   0        0        0    16923 2023-12-18 10:36:26.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PMaterial.py
--rw-rw-rw-   0        0        0   354507 2024-03-04 08:20:42.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PModelInputData.py
--rw-rw-rw-   0        0        0     7338 2023-12-18 10:36:26.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PNode.py
--rw-rw-rw-   0        0        0    12012 2023-11-29 11:18:13.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PProperty.py
--rw-rw-rw-   0        0        0     6121 2024-02-13 12:32:13.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PReport.py
--rw-rw-rw-   0        0        0    11302 2024-03-04 10:02:52.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PResult.py
--rw-rw-rw-   0        0        0     2044 2023-12-18 10:36:26.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PSection.py
--rw-rw-rw-   0        0        0     2777 2023-09-21 06:53:42.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PSet.py
--rw-rw-rw-   0        0        0      708 2023-06-14 08:40:16.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/ProgresBar.py
--rw-rw-rw-   0        0        0        2 2023-01-27 14:45:07.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Classes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.456428 NaxToPy-1.5.6/src/NaxToPy/Core/Constants/
--rw-rw-rw-   0        0        0     1515 2024-03-13 14:42:02.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Constants/Constants.py
--rw-rw-rw-   0        0        0        2 2023-01-23 07:52:14.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Constants/__init__.py
--rw-rw-rw-   0        0        0    16398 2023-05-30 07:39:47.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Constants/librerias.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.459428 NaxToPy-1.5.6/src/NaxToPy/Core/Errors/
--rw-rw-rw-   0        0        0     1420 2023-05-25 07:57:17.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Errors/N2PColors.py
--rw-rw-rw-   0        0        0     2205 2023-10-19 09:23:23.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Errors/N2PFileHandler.py
--rw-rw-rw-   0        0        0    50384 2024-03-04 08:20:42.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Errors/N2PLog.py
--rw-rw-rw-   0        0        0        2 2023-01-23 07:52:14.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Errors/__init__.py
--rw-rw-rw-   0        0        0    74165 2024-03-13 14:32:12.000000 NaxToPy-1.5.6/src/NaxToPy/Core/N2PModelContent.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.462428 NaxToPy-1.5.6/src/NaxToPy/Core/Reference_Finder/
--rw-rw-rw-   0        0        0     8474 2024-02-19 10:31:24.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Reference_Finder/__Reference_Finder.py
--rw-rw-rw-   0        0        0        2 2023-01-20 07:41:18.000000 NaxToPy-1.5.6/src/NaxToPy/Core/Reference_Finder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.465428 NaxToPy-1.5.6/src/NaxToPy/Core/_AuxFunc/
--rw-rw-rw-   0        0        0     3627 2024-01-04 10:24:30.000000 NaxToPy-1.5.6/src/NaxToPy/Core/_AuxFunc/_NetToPython.py
--rw-rw-rw-   0        0        0        2 2022-11-22 11:07:36.000000 NaxToPy-1.5.6/src/NaxToPy/Core/_AuxFunc/__init__.py
--rw-rw-rw-   0        0        0      183 2024-01-18 10:12:28.000000 NaxToPy-1.5.6/src/NaxToPy/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.474428 NaxToPy-1.5.6/src/NaxToPy/Modules/
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.471428 NaxToPy-1.5.6/src/NaxToPy/Modules/Fasteners/
--rw-rw-rw-   0        0        0    39747 2024-03-04 08:31:59.000000 NaxToPy-1.5.6/src/NaxToPy/Modules/Fasteners/N2PUpdateFastener.py
--rw-rw-rw-   0        0        0       50 2024-03-04 09:43:21.000000 NaxToPy-1.5.6/src/NaxToPy/Modules/Fasteners/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.474428 NaxToPy-1.5.6/src/NaxToPy/Modules/N2PEnvelope/
--rw-rw-rw-   0        0        0     4226 2024-01-03 07:54:23.000000 NaxToPy-1.5.6/src/NaxToPy/Modules/N2PEnvelope/N2PEnvelope.py
--rw-rw-rw-   0        0        0        0 2023-07-11 07:33:21.000000 NaxToPy-1.5.6/src/NaxToPy/Modules/N2PEnvelope/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.477428 NaxToPy-1.5.6/src/NaxToPy/Modules/N2PtoEXE/
--rw-rw-rw-   0        0        0     7696 2024-02-19 09:54:11.000000 NaxToPy-1.5.6/src/NaxToPy/Modules/N2PtoEXE/N2PtoEXE.py
--rw-rw-rw-   0        0        0        2 2023-03-30 09:33:43.000000 NaxToPy-1.5.6/src/NaxToPy/Modules/N2PtoEXE/__init__.py
--rw-rw-rw-   0        0        0       50 2024-03-04 09:52:33.000000 NaxToPy-1.5.6/src/NaxToPy/Modules/__init__.py
--rw-rw-rw-   0        0        0   198996 2023-04-14 09:43:58.000000 NaxToPy-1.5.6/src/NaxToPy/NaxToPy.ico
--rw-rw-rw-   0        0        0      487 2024-03-04 09:42:19.000000 NaxToPy-1.5.6/src/NaxToPy/__init__.py
--rw-rw-rw-   0        0        0     7882 2024-01-02 09:26:08.000000 NaxToPy-1.5.6/src/NaxToPy/user_functions.txt
-drwxrwxrwx   0        0        0        0 2024-03-13 14:42:57.448428 NaxToPy-1.5.6/src/NaxToPy.egg-info/
--rw-rw-rw-   0        0        0    20934 2024-03-13 14:42:57.000000 NaxToPy-1.5.6/src/NaxToPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1813 2024-03-13 14:42:57.000000 NaxToPy-1.5.6/src/NaxToPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-13 14:42:57.000000 NaxToPy-1.5.6/src/NaxToPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-03-13 14:42:57.000000 NaxToPy-1.5.6/src/NaxToPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-03-13 14:42:57.000000 NaxToPy-1.5.6/src/NaxToPy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.808955 naxtopy-2.0.0/
+-rw-rw-rw-   0        0        0     5368 2024-04-08 09:50:46.000000 naxtopy-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0    21374 2024-04-19 07:28:20.814478 naxtopy-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14232 2024-03-21 12:25:22.000000 naxtopy-2.0.0/README.md
+-rw-rw-rw-   0        0        0     1143 2024-03-04 15:18:14.000000 naxtopy-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-19 07:28:20.826789 naxtopy-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      462 2024-01-18 10:36:31.000000 naxtopy-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.176955 naxtopy-2.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.182955 naxtopy-2.0.0/src/NaxToPy/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.193955 naxtopy-2.0.0/src/NaxToPy/Core/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.185955 naxtopy-2.0.0/src/NaxToPy/Core/Classes/
+-rw-rw-rw-   0        0        0      765 2024-02-13 12:32:13.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/AllClasses.py
+-rw-rw-rw-   0        0        0    24803 2024-03-12 11:50:17.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PComponent.py
+-rw-rw-rw-   0        0        0     4555 2023-12-18 10:36:26.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PConnector.py
+-rw-rw-rw-   0        0        0     2006 2023-12-18 10:36:26.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PCoord.py
+-rw-rw-rw-   0        0        0     6772 2024-03-04 14:59:02.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PElement.py
+-rw-rw-rw-   0        0        0     6094 2024-03-04 14:59:02.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PFreeBody.py
+-rw-rw-rw-   0        0        0     3351 2024-03-12 11:33:59.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PIncrement.py
+-rw-rw-rw-   0        0        0    12323 2024-04-19 07:02:20.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PLoadCase.py
+-rw-rw-rw-   0        0        0    16923 2023-12-18 10:36:26.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PMaterial.py
+-rw-rw-rw-   0        0        0   355653 2024-04-09 15:09:23.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PModelInputData.py
+-rw-rw-rw-   0        0        0     7335 2024-03-04 14:59:02.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PNode.py
+-rw-rw-rw-   0        0        0    12012 2023-11-29 11:18:13.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PProperty.py
+-rw-rw-rw-   0        0        0     6118 2024-04-12 06:30:49.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PReport.py
+-rw-rw-rw-   0        0        0    12237 2024-04-15 08:18:55.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PResult.py
+-rw-rw-rw-   0        0        0     2044 2023-12-18 10:36:26.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PSection.py
+-rw-rw-rw-   0        0        0     2777 2023-09-21 06:53:42.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PSet.py
+-rw-rw-rw-   0        0        0      708 2023-06-14 08:40:16.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/ProgresBar.py
+-rw-rw-rw-   0        0        0        2 2023-01-27 14:45:07.000000 naxtopy-2.0.0/src/NaxToPy/Core/Classes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.188955 naxtopy-2.0.0/src/NaxToPy/Core/Constants/
+-rw-rw-rw-   0        0        0     1583 2024-04-19 07:27:53.000000 naxtopy-2.0.0/src/NaxToPy/Core/Constants/Constants.py
+-rw-rw-rw-   0        0        0        2 2023-01-23 07:52:14.000000 naxtopy-2.0.0/src/NaxToPy/Core/Constants/__init__.py
+-rw-rw-rw-   0        0        0    16398 2023-05-30 07:39:47.000000 naxtopy-2.0.0/src/NaxToPy/Core/Constants/librerias.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.191955 naxtopy-2.0.0/src/NaxToPy/Core/Errors/
+-rw-rw-rw-   0        0        0     1420 2023-05-25 07:57:17.000000 naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PColors.py
+-rw-rw-rw-   0        0        0     2205 2023-10-19 09:23:23.000000 naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PFileHandler.py
+-rw-rw-rw-   0        0        0    52152 2024-04-19 07:02:20.000000 naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PLog.py
+-rw-rw-rw-   0        0        0        2 2023-01-23 07:52:14.000000 naxtopy-2.0.0/src/NaxToPy/Core/Errors/__init__.py
+-rw-rw-rw-   0        0        0    74013 2024-04-19 07:02:20.000000 naxtopy-2.0.0/src/NaxToPy/Core/N2PModelContent.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.193955 naxtopy-2.0.0/src/NaxToPy/Core/Reference_Finder/
+-rw-rw-rw-   0        0        0    10217 2024-04-03 13:12:21.000000 naxtopy-2.0.0/src/NaxToPy/Core/Reference_Finder/__Reference_Finder.py
+-rw-rw-rw-   0        0        0        2 2023-01-20 07:41:18.000000 naxtopy-2.0.0/src/NaxToPy/Core/Reference_Finder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.196955 naxtopy-2.0.0/src/NaxToPy/Core/_AuxFunc/
+-rw-rw-rw-   0        0        0     3627 2024-01-04 10:24:30.000000 naxtopy-2.0.0/src/NaxToPy/Core/_AuxFunc/_NetToPython.py
+-rw-rw-rw-   0        0        0        2 2022-11-22 11:07:36.000000 naxtopy-2.0.0/src/NaxToPy/Core/_AuxFunc/__init__.py
+-rw-rw-rw-   0        0        0      183 2024-01-18 10:12:28.000000 naxtopy-2.0.0/src/NaxToPy/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.205955 naxtopy-2.0.0/src/NaxToPy/Modules/
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.202955 naxtopy-2.0.0/src/NaxToPy/Modules/Fasteners/
+-rw-rw-rw-   0        0        0    41254 2024-03-05 10:31:16.000000 naxtopy-2.0.0/src/NaxToPy/Modules/Fasteners/N2PUpdateFastener.py
+-rw-rw-rw-   0        0        0       50 2024-03-04 09:43:21.000000 naxtopy-2.0.0/src/NaxToPy/Modules/Fasteners/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.205955 naxtopy-2.0.0/src/NaxToPy/Modules/N2PEnvelope/
+-rw-rw-rw-   0        0        0     4216 2024-03-04 14:59:02.000000 naxtopy-2.0.0/src/NaxToPy/Modules/N2PEnvelope/N2PEnvelope.py
+-rw-rw-rw-   0        0        0        0 2023-07-11 07:33:21.000000 naxtopy-2.0.0/src/NaxToPy/Modules/N2PEnvelope/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.208955 naxtopy-2.0.0/src/NaxToPy/Modules/N2PtoEXE/
+-rw-rw-rw-   0        0        0     7791 2024-04-03 09:13:01.000000 naxtopy-2.0.0/src/NaxToPy/Modules/N2PtoEXE/N2PtoEXE.py
+-rw-rw-rw-   0        0        0        2 2023-03-30 09:33:43.000000 naxtopy-2.0.0/src/NaxToPy/Modules/N2PtoEXE/__init__.py
+-rw-rw-rw-   0        0        0       50 2024-03-04 09:52:33.000000 naxtopy-2.0.0/src/NaxToPy/Modules/__init__.py
+-rw-rw-rw-   0        0        0   198996 2023-04-14 09:43:58.000000 naxtopy-2.0.0/src/NaxToPy/NaxToPy.ico
+-rw-rw-rw-   0        0        0      487 2024-02-13 12:32:13.000000 naxtopy-2.0.0/src/NaxToPy/__init__.py
+-rw-rw-rw-   0        0        0     7882 2024-01-02 09:26:08.000000 naxtopy-2.0.0/src/NaxToPy/user_functions.txt
+drwxrwxrwx   0        0        0        0 2024-04-19 07:28:20.179955 naxtopy-2.0.0/src/NaxToPy.egg-info/
+-rw-rw-rw-   0        0        0    21374 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1813 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-19 07:28:20.000000 naxtopy-2.0.0/src/NaxToPy.egg-info/top_level.txt
```

### Comparing `NaxToPy-1.5.6/LICENSE` & `naxtopy-2.0.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2023 Idaero Solutions
+Copyright (c) 2024 Idaero Solutions
 
 This freeware license agreement (“agreement”) is a legally binding contract
 between the individual who downloads the software (“you”) and the licensor,
 that should be read in its entirety. This is an agreement governing your use
 this software own by Idaero Solutions, further defined herein as “software”,
 and the licensor of the software is willing to provide you with access to the
 software only on the condition that you accept all of the terms and conditions
```

### Comparing `NaxToPy-1.5.6/PKG-INFO` & `naxtopy-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: NaxToPy
-Version: 1.5.6
+Version: 2.0.0
 Summary: Package for postprocessing FEM results in Python
 Home-page: https://www.idaerosolutions.com/Home/NaxToPy
 Download-URL: https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US
 Author-email: Idaero Solutions <manuel.sanchez@idaerosolutions.com>
-License: Copyright (c) 2023 Idaero Solutions
+License: Copyright (c) 2024 Idaero Solutions
         
         This freeware license agreement (“agreement”) is a legally binding contract
         between the individual who downloads the software (“you”) and the licensor,
         that should be read in its entirety. This is an agreement governing your use
         this software own by Idaero Solutions, further defined herein as “software”,
         and the licensor of the software is willing to provide you with access to the
         software only on the condition that you accept all of the terms and conditions
@@ -142,16 +142,17 @@
 It could be easily combined with other Python packages as Matplotlib or Pandas. This provides access
 to the full coding power of Python to interpret and process the results, without the need to install
 any additional software other than having NaxTo already installed (see the _Download_ and _Homepage_
 links on the left).
 
 **NaxToPy** is a powerful tool for FEM analysis post-processing!
 
-**CAUTION:** This version is only compatible with **NaxTo 2024.0.5**.
-Check in _Programs and Features_ the NaxTo version that is installed.
+**CAUTION:** To use NaxToPy, [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US) must be installed.
+This version is compatible with **NaxTo 2024.1**. It may be compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
+Check in _Programs and Features_ the NaxTo version that is installed. 
 
 ## Installation
 
 
 If python is callable from the command line:
 
 `py -m pip install NaxToPy`
@@ -250,14 +251,19 @@
 ### v.1.5.5
 1. Bug Fix: Now is possible to call the module N2PUpdateFastener
 
 ### v.1.5.6
 1. The method new_envelope_loadcase() now has the option to choose the envelope group. Which means the user can ask for
 the LoadCases that are critical or the Increment that is critical instead of the value.
 
+### v.2.0.0
+1. Changes made to align the library with updates in lower-level dependencies.
+2. New internal methods to look for the compatibility with low-level dependencies.
+3. The name of the .log is now NaxToPy_Year-Month-Day.log.
+
 # Documentation
 
 **NaxToPy** is a package developed by Idaero Solutions© as a part of the **NaxTo** software.
 
 NaxToPy only use three dependeces:
 - NumPy: https://numpy.org/
 - PythonNET: https://pythonnet.github.io/
```

### Comparing `NaxToPy-1.5.6/README.md` & `naxtopy-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,17 @@
 It could be easily combined with other Python packages as Matplotlib or Pandas. This provides access
 to the full coding power of Python to interpret and process the results, without the need to install
 any additional software other than having NaxTo already installed (see the _Download_ and _Homepage_
 links on the left).
 
 **NaxToPy** is a powerful tool for FEM analysis post-processing!
 
-**CAUTION:** This version is only compatible with **NaxTo 2024.0.5**.
-Check in _Programs and Features_ the NaxTo version that is installed.
+**CAUTION:** To use NaxToPy, [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US) must be installed.
+This version is compatible with **NaxTo 2024.1**. It may be compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
+Check in _Programs and Features_ the NaxTo version that is installed. 
 
 ## Installation
 
 
 If python is callable from the command line:
 
 `py -m pip install NaxToPy`
@@ -126,14 +127,19 @@
 ### v.1.5.5
 1. Bug Fix: Now is possible to call the module N2PUpdateFastener
 
 ### v.1.5.6
 1. The method new_envelope_loadcase() now has the option to choose the envelope group. Which means the user can ask for
 the LoadCases that are critical or the Increment that is critical instead of the value.
 
+### v.2.0.0
+1. Changes made to align the library with updates in lower-level dependencies.
+2. New internal methods to look for the compatibility with low-level dependencies.
+3. The name of the .log is now NaxToPy_Year-Month-Day.log.
+
 # Documentation
 
 **NaxToPy** is a package developed by Idaero Solutions© as a part of the **NaxTo** software.
 
 NaxToPy only use three dependeces:
 - NumPy: https://numpy.org/
 - PythonNET: https://pythonnet.github.io/
```

### Comparing `NaxToPy-1.5.6/pyproject.toml` & `naxtopy-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 733e 3d36 372e 382e 3022  uptools>=67.8.0"
 00000030: 5d0d 0a62 7569 6c64 2d62 6163 6b65 6e64  ]..build-backend
 00000040: 203d 2022 7365 7475 7074 6f6f 6c73 2e62   = "setuptools.b
 00000050: 7569 6c64 5f6d 6574 6122 0d0a 0d0a 5b70  uild_meta"....[p
 00000060: 726f 6a65 6374 5d0d 0a6e 616d 6520 3d20  roject]..name = 
 00000070: 224e 6178 546f 5079 220d 0a76 6572 7369  "NaxToPy"..versi
-00000080: 6f6e 203d 2022 312e 352e 3622 0d0a 6c69  on = "1.5.6"..li
+00000080: 6f6e 203d 2022 322e 302e 3022 0d0a 6c69  on = "2.0.0"..li
 00000090: 6365 6e73 6520 3d20 7b66 696c 6520 3d20  cense = {file = 
 000000a0: 224c 4943 454e 5345 227d 0d0a 6175 7468  "LICENSE"}..auth
 000000b0: 6f72 7320 3d20 5b20 7b20 6e61 6d65 203d  ors = [ { name =
 000000c0: 2022 4964 6165 726f 2053 6f6c 7574 696f   "Idaero Solutio
 000000d0: 6e73 222c 2065 6d61 696c 203d 2022 6d61  ns", email = "ma
 000000e0: 6e75 656c 2e73 616e 6368 657a 4069 6461  nuel.sanchez@ida
 000000f0: 6572 6f73 6f6c 7574 696f 6e73 2e63 6f6d  erosolutions.com
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/AllClasses.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/AllClasses.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PComponent.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PComponent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from NaxToPy.Core.Classes.N2PSection import N2PSection
 from NaxToPy.Core.Errors.N2PLog import N2PLog
-from VizzerClasses import N2ParamInputResults
-from VizzerClasses import N2TensorTransformation
+from NaxToModel import N2ParamInputResults
+from NaxToModel import N2TensorTransformation
 from array import array
 import numpy as np
 from NaxToPy.Core._AuxFunc._NetToPython import _numpytonet
 from typing import Union
 
 
 # Clase Component de Python
@@ -27,15 +27,15 @@
             Args:
                 name: str -> name of the component
                 sections: list[N2Sections] -> list with instances of N2Sections
                 result_father: N2PResult
         """
         self.__name__ = name
         self.__sections__ = [N2PSection(sections[i].Name,
-                                        sections[i].number) for i in range(0, len(sections))]
+                                        sections[i].Number) for i in range(0, len(sections))]
         self.__result_father__ = result_father
     # ---------------------------------------------------------------------------------------------
 
     # Metodo para Obtener el Nombre de la Componente
     # ----------------------------------------------
     @property
     def Name(self) -> str:
@@ -58,25 +58,25 @@
         # aun no se han construido. Por eso el metodo de la propiedad es la que busca los argumentos y llama
         # al metodo dentro de Vizzer classes.
         solver = self.__result_father__.__loadCase_father__.__solver__
         result = self.__result_father__.Name
         component = self.Name
         return bool(N2TensorTransformation.IsResultSupported(solver, result, component))
 
-    # Metodo para llamar a la funcion de VizzerClasses que devueleve el array de resultados-----------------------------
+    # Metodo para llamar a la funcion de NaxToModel que devueleve el array de resultados-----------------------------
     def get_result_array(self, sections=None, aveSections=-1, cornerData=False, aveNodes=-1, variation=100,
                          realPolar=0, coordsys: int = -1000,
                          v1: tuple = (1, 0, 0), v2: tuple = (0, 1, 0)) -> tuple[list, str]:
         """Deprecated method. Please, use get_result_list instead for asking the results as a list. If a numpy array is
         preferred, use get_result_ndarray"""
         return self.get_result_list(sections, aveSections, cornerData, aveNodes, variation,
                                     realPolar, coordsys, v1, v2)
     # ------------------------------------------------------------------------------------------------------------------
 
-    # Metodo para llamar a la funcion de VizzerClasses que devueleve el array de resultados como lista------------------
+    # Metodo para llamar a la funcion de NaxToModel que devueleve el array de resultados como lista------------------
     def get_result_list(self, sections=None, aveSections=-1, cornerData=False, aveNodes=-1, variation=100,
                          realPolar=0, coordsys: int = -1000,
                          v1: Union[tuple, np.ndarray] = (1,0,0), v2: Union[tuple, np.ndarray] = (0,1,0)) -> tuple[list, str]:
         """ Returns a tuple with the list of floats with the result array asked and a str with the position of the
         results
 
         Args:
@@ -132,15 +132,15 @@
                 z=v1^v2,
                 y=z^x.
 
         Returns: 
             results: tuple(list[float], str)
 
         """
-        # Aquí se prepara la llamada a la funcion de VizzerClasses.N2PModelContent.getArraytoPlot(). Esta usa como
+        # Aquí se prepara la llamada a la funcion de NaxToModel.N2PModelContent.getArraytoPlot(). Esta usa como
         # argumento un objeto de la clase N2ParamImputResults. Por se instancia y se modifican sus propiedades antes
         # de hacer la llamada a la funcion.
 
         # Aqui se mete el sistema de coordenadas en el que queremos que nos saque la informacion.
         # Para ello primero comprobamos que es viable hacer la tansformacion (puede que aun no este implementada o que
         # la componente simplemente no la admita al ser un escalar a secas)
 
@@ -160,15 +160,15 @@
         elif results[1] == 3:
             return(list(results[0]), 'ELEMENT NODAL')
         else:
             N2PLog.Error.E206(self.Name)
             return(-1, 'NO RESULTS')
     # ------------------------------------------------------------------------------------------------------------------
 
-    # Metodo para llamar a la funcion de VizzerClasses que devuelve el array de resultados como array de numpy----------
+    # Metodo para llamar a la funcion de NaxToModel que devuelve el array de resultados como array de numpy----------
     def get_result_ndarray(self, sections=None, aveSections=-1, cornerData=False, aveNodes=-1, variation=100,
                          realPolar=0, coordsys: int = -1000,
                          v1: Union[tuple, np.ndarray ] = (1,0,0), v2: Union[tuple, np.ndarray ] = (0,1,0)) -> tuple[np.array, str]:
         """ Returns a tuple with the numpy array of floats with the result array asked and a str with the position of
         the results
 
         Args:
@@ -241,15 +241,15 @@
         elif results[1] == 3:
             return(np.array(results[0], np.float64), 'ELEMENT NODAL')
         else:
             N2PLog.Error.E206(self.Name)
             return(-1, 'NO RESULTS')
     # ------------------------------------------------------------------------------------------------------------------
 
-    # # Metodo que devulve un dataframe con los resulados tras llamar a la funcion de VizzerClasses--
+    # # Metodo que devulve un dataframe con los resulados tras llamar a la funcion de NaxToModel--
     # def get_result_dataframe(self, sections=None, aveSections=-1, cornerData=False, aveNodes=-1,
     #                          variation=100, realPolar=0, coordsys: int = -1000,
     #                          v1: tuple = (1,0,0), v2: tuple = (0,1,0)) -> DataFrame:
     #     """Returns a DataFrame of pandas with the results array of a component as data for the active increment.
     #
     #     Args:
     #
@@ -388,15 +388,15 @@
         py_dict = {(int(key.split(":")[0].replace("DoF_LCD", "-").replace("DoF_LC", "")),
                     int(key.split(":")[1][2:])): np.array(value, np.float64)
                    for key, value in dict(cs_dict[0]).items()}
 
         return py_dict
     # ------------------------------------------------------------------------------------------------------------------
 
-    # Metodo que crea la formula que necesita la funcion de VizzerClasses ----------------------------------------------
+    # Metodo que crea la formula que necesita la funcion de NaxToModel ----------------------------------------------
     def _create_formula(self, list_lc_incr: list[tuple["N2PLoadCase", "N2PIncrement"],...]) -> str:
 
         if isinstance(list_lc_incr, tuple):
             list_lc_incr = [list_lc_incr]
 
         N2PLoadCase = type(self.__result_father__.__loadCase_father__)
         N2PIncrement = type(self.__result_father__.__loadCase_father__.Increments[0])
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PConnector.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PConnector.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PCoord.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PCoord.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PElement.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PElement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import array
 
 from NaxToPy.Core.Classes.N2PNode import N2PNode
-from VizzerClasses import N2ElementsCoordinateSystems
+from NaxToModel import N2ElementsCoordinateSystems
 
 # Clase Element de Python
 class N2PElement:
     """Class with the information of an element.
 
     Attributes:
         ID: int.
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PFreeBody.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PFreeBody.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """ Module with all the FreeBody related classes.
 """
-from VizzerClasses import N2FBDSection, N2FBD, N2FBDResult
+from NaxToModel import N2FBDSection, N2FBD, N2FBDResult
 from NaxToPy.Core.Classes.N2PNode import N2PNode
 from NaxToPy.Core.Classes.N2PElement import N2PElement
 from NaxToPy.Core.Classes.N2PCoord import N2PCoord
 from NaxToPy.Core.Classes.N2PIncrement import N2PIncrement
 from NaxToPy.Core.Classes.N2PLoadCase import N2PLoadCase
 from array import array
 
@@ -57,15 +57,15 @@
 
 
         if outpoint is not None:
             self.__centroid = False
         else:
             self.__centroid = True
 
-        # Llamada al constructor de VizzerClasses
+        # Llamada al constructor de NaxToModel
         n2fbdsection = N2FBDSection(self.__name)
 
         # Se incluye la parte:
         n2fbdsection.NodesPartID = self.__model._N2PModelContent__StrPartToID.get(self.__nodelist[0].PartID, 0)
 
         # Si se define un sistema de coordenadas se evalua la propiedad, si no, no se evalua y se usara el global
         if coordsys is not None:
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PIncrement.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PIncrement.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,56 @@
 # Clase Increment de Python --------------------------------------------------------------------------------------------
 class N2PIncrement:
-    '''Class which contains the information associated to an increment/frame of a N2PLoadCase instance.
-
-    Attributes:
-        Name: str.
-        ImaginaryEigenvalue: float.
-        RealEigenvalue: float.
-        ID: int.
-        Time: double.
-    '''
+    """Class which contains the information associated to an increment/frame of a N2PLoadCase instance."""
 
     # Constructor de N2PIncrement --------------------------------------------------------------------------------------
-    def __init__(self, name, eigi, eigr, number, time):
-        '''Python Increment Constructor
-            Input:
-                name: str -> name of the increment
-                eigi: double -> value of the imaginary eigenvalue
-                eigr: double -> value of the real eigenvalue
-                number: int -> number of the increment within the sequence of increments in the load case
-                time: double -> value of the increment
-            ----------
-            Returns:
-                N2PIncrement: object
-        '''
-        self.__name__ = name
-        self.__eigi__ = eigi
-        self.__eigr__ = eigr
-        self.__number__ = number
-        self.__time__ = time
+    def __init__(self, info):
+        self.__info__ = info
     # ------------------------------------------------------------------------------------------------------------------
 
     # Metodo para obtener el nombre del incremento ---------------------------------------------------------------------
     @property
     def Name(self) -> str:
-        return(str(self.__name__))
+        """Name of the Increment"""
+        return(str(self.__info__.Name))
     # ------------------------------------------------------------------------------------------------------------------
 
     # Metodo para obtener el valor del autovalor real ------------------------------------------------------------------
     @property
     def RealEigenvalue(self) -> float:
-        return(float(self.__eigr__))
+        """Real Eigenvalue of the increment"""
+        return(float(self.__info__.EigReal))
     # ------------------------------------------------------------------------------------------------------------------
 
     # Metodo para obtener el valor del autovalor imaginario ------------------------------------------------------------
     @property
     def ImaginaryEigenvalue(self) -> float:
-        return(float(self.__eigi__))
+        """Imaginary Eigenvalue of the increment"""
+        return(float(self.__info__.EigImg))
     # ------------------------------------------------------------------------------------------------------------------
 
     # Metodo para obtener el ID del incremento en el caso de carga -----------------------------------------------------
     @property
     def ID(self) -> int:
-        return(int(self.__number__))
+        """Solver ID of the Increment"""
+        return(int(self.__info__.ID))
     # ------------------------------------------------------------------------------------------------------------------
 
     # Metodo para obtener el valor del incremento ----------------------------------------------------------------------
     @property
     def Time(self) -> float:
         ''' Returns the value of the increment/frame'''
-        return(float(self.__time__))
+        return(float(self.__info__.Time))
+    # ------------------------------------------------------------------------------------------------------------------
+
+    # Metodo para obtener el tipo de Solucion --- ----------------------------------------------------------------------
+    @property
+    def Solution(self) -> str:
+        """Returns the value of the Solution name of the Increment"""
+        return(str(self.__info__.Solution))
     # ------------------------------------------------------------------------------------------------------------------
 
     # Special Method for Object Representation -------------------------------------------------------------------------
     def __repr__(self):
         return f"N2PIncrement({self.ID}: \"{self.Name}\")"
     # ------------------------------------------------------------------------------------------------------------------
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PLoadCase.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PLoadCase.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,35 +42,31 @@
         ----------
         Returns:
             N2PLoadCase: object
         '''
         self.__id__ = id
         self.__idoriginal__ = id_original
 
-        self.__increments__ = [N2PIncrement(increments[i].Name,
-                                            increments[i].eigi,
-                                            increments[i].eigr,
-                                            increments[i].number,
-                                            increments[i].time) for i in range(0, len(increments))]
+        self.__increments__ = [N2PIncrement(increments[i]) for i in range(0, len(increments))]
 
         self.__incrementsnumberlist__ = increments_number_list
         self.__iscomplex__ = is_complex
         self.__lctype__ = lc_type
         self.__namelc__ = name
-        self.__results__ = {results[i].name: N2PResult(results[i].Components,
+        self.__results__ = {results[i].Name: N2PResult(results[i].Components,
                                                        results[i].Position,
                                                        results[i].derivedComps,
-                                                       results[i].description,
+                                                       results[i].Description,
                                                        results[i].elemTypes,
                                                        results[i].fcode,
-                                                       results[i].name,
+                                                       results[i].Name,
                                                        self) for i in range(0, len(results))}
 
         self.__solutiontype__ = solution_type
-        self.__activeIncrement__ = list(increments)[-1].number
+        self.__activeIncrement__ = list(increments)[-1].ID
         self.__solver__ = solver
         self.__modelFather__ = model_father
         self.__n2loadcase = n2loadcase
     # ------------------------------------------------------------------------------------------------------------------
 
     # Metodo para obtener el numero de identificacion interno del caso de carga ----------------------------------------
     @property
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PMaterial.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PMaterial.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PModelInputData.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PModelInputData.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,17 +43,17 @@
     def DataType(self) -> str:
         return self.__inputdata.DataType.ToString()
 
     @property
     def Lines(self) -> list[str, ...]:
         return list(self.__inputdata.Lines)
 
-    # @property
-    # def FilePathId(self) -> str:
-    #     return self.__inputdata.FilePathId
+    @property
+    def FilePathId(self) -> int:
+        return self.__inputdata.FilePathId
 
     # @property
     # def Children(self) -> list["N2PInputData"]:
     #     return list(self.__inputdata.Children)
 
 
 class N2PCard(N2PInputData):
@@ -123,28 +123,54 @@
         DictionaryIDsFiles: dict.
         TypeOfFile: str.
     """
 
     def __init__(self, listbulkdatacards, inputfiledata):
         self.__listbulkdatacards = listbulkdatacards
         self.__inputfiledata = inputfiledata
+        self.__listinstructions = []
+        self.__listcomments = []
+        self.__dictionary_files_ids = {value: key for key, value in self.DictionaryIDsFiles.items()}
 
     @property
     def ListBulkDataCards(self) -> list[N2PCard, ...]:
         """List with the N2PCard objects of the input FEM file. It has all bulk data cards of the model"""
         return self.__listbulkdatacards
 
     @property
     def DictionaryIDsFiles(self) -> dict:
         return dict(self.__inputfiledata.DictionaryIDsFiles)
 
     @property
+    def DictionaryFilesIDs(self) -> dict:
+        return dict(self.__dictionary_files_ids)
+
+    @property
     def TypeOfFile(self) -> str:
         return self.__inputfiledata.TypeOfFile.ToString()
 
+    @property
+    def ListInstructions(self) -> list[N2PInputData]:
+        """List with the instructions of the model. They are the commands above the BEGIN BULK: Executive Control
+        Statements and Control Case Commands"""
+        if self.__listinstructions:
+            return self.__listinstructions
+        else:
+            self.__listinstructions = [N2PInputData(i) for i in self.__inputfiledata.StructuredInfo.ModelInstructions]
+            return self.__listinstructions
+
+    @property
+    def ListComments(self) -> list[N2PInputData]:
+        """List with all the comments in the FEM Input File"""
+        if self.__listcomments:
+            return self.__listcomments
+        else:
+            self.__listcomments = [N2PInputData(i) for i in self.__inputfiledata.StructuredInfo.ModelComments]
+            return self.__listcomments
+
     def get_cards_by_field(self, fields: list[str, ], row: int = 0, col: int = 0) -> list[N2PCard, ]:
         """Method that returns a list with the N2PCard objects of the input FEM file that meet the condition.
         In other words, that field is equal to the string in the position defined. If no row or column is defined, the
         string will compare with the position (0,0) of the card, that is the name of the card.
 
         Args:
             fields: str | list[str]
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PNode.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PNode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import array
 import time
-from VizzerClasses.Classes import N2AdjacencyFunctions
+from NaxToModel.Classes import N2AdjacencyFunctions
 
 
 class N2PNode:
     """Class with the information of a node/grid.
 
     Attributes:
         ID: int.
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PProperty.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PProperty.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PReport.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PReport.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from NaxToPy.Core.Classes.N2PNode import N2PNode
 from NaxToPy.Core.Classes.N2PElement import N2PElement
 from NaxToPy.Core.Errors.N2PLog import N2PLog
 from NaxToPy.Core.Classes.N2PComponent import _get_axis
 from NaxToPy.Core._AuxFunc._NetToPython import _numpytonet
 import numpy as np
 from typing import Union
-from VizzerClasses import N2Report, N2ParamInputResults, N2Enums
+from NaxToModel import N2Report, N2ParamInputResults, N2Enums
 from System import Object, Array
 
 
 class N2PReport:
     """Class that contains the data of a report. It includes the input data: load cases, the selection (that could be a
     list of N2PNode or N2PElement), if envelope,... and the output data: results array asked"""
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PResult.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PResult.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from NaxToPy.Core.Classes.N2PComponent import N2PComponent
 from NaxToPy.Core.Errors.N2PLog import N2PLog
-from VizzerClasses import N2Component
+from NaxToModel import N2Component
 from System.Collections.Generic import List
 
 
 # Clase Result de Python --------------------------------------------------------------------------
 class N2PResult:
     """Class which contains the information associated to a result of a N2PLoadCase"""
 
@@ -80,15 +80,39 @@
     @property
     def Name(self) -> str:
         return(str(self.__name__))
     # ---------------------------------------------------------------------------------------------
 
     # Metodo para obtener las componentes disponibles en el resultado -----------------------------
     def get_component(self, name: str) -> N2PComponent:
-        """Returns a N2Component as component with name specified
+        """Returns a N2Component as component with name specified. It can be a Raw Component or a derived component
+
+        Args:
+            name: str
+
+        Returns:
+            component: N2PComponent
+        """
+
+        if isinstance(name, str):
+            component = self.Components.get(name, None)
+            if not component:
+                component = self.DerivedComponents.get(name, None)
+            if component is None:
+                N2PLog.Error.E215(name)
+            return component
+
+        # Devolver todos los resultados
+        else:
+            N2PLog.Error.E216()
+    # ---------------------------------------------------------------------------------------------
+
+    # Metodo para obtener las componentes originales disponibles en el resultado -----------------------------
+    def get_raw_component(self, name: str) -> N2PComponent:
+        """Returns a N2Component as component with name specified. It checks only in the original list of components
 
         Args:
             name: str
 
         Returns:
             component: N2PComponent
         """
@@ -150,18 +174,18 @@
         Returns:
             N2PComponent: Derived load case.
         """
 
         # Recuperamos la instancia N2ModelModelContent
         mc = self.__loadCase_father__.__modelFather__._N2PModelContent__vzmodel
 
-        # Llamada al constructor de N2Component de VizzerClasses
+        # Llamada al constructor de N2Component de NaxToModel
         new_d_comp = N2Component(mc, name, formula)
 
-        # Se incluye en la lista de compornentes derivadas de vizzerclasses. Para ello tengo que comprobar que existe
+        # Se incluye en la lista de compornentes derivadas de NaxToModel. Para ello tengo que comprobar que existe
         # dicha lista. Si no existe la tengo que crear como lista de C#
         if not mc.DerivedComponents:
             mc.DerivedComponents = List[N2Component]()
 
         # Now I add the new derived component to the list
         mc.DerivedComponents.Add(new_d_comp)
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PSection.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PSection.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/N2PSet.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/N2PSet.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Classes/ProgresBar.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Classes/ProgresBar.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Constants/librerias.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Constants/librerias.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Errors/N2PColors.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PColors.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Errors/N2PFileHandler.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PFileHandler.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Errors/N2PLog.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Errors/N2PLog.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         __clevel = logging.INFO
 
     __directory = os.path.dirname(os.path.abspath(sys.argv[0]))
 
     if __directory == "C:\\Users":
         __directory = os.path.expanduser("~") + "\\Documents\\"
 
-    __filename = time.strftime("NaxToPy_%d-%m-%Y.log", time.localtime())
+    __filename = time.strftime("NaxToPy_%Y-%m-%d.log", time.localtime())
     __path = os.path.join(__directory, __filename)
 
     __logger = logging.getLogger('Logger')
     __logger.setLevel("DEBUG")
 
     # Formato en el que se presenta los datos del registro en el archivo .log
     __formatter = logging.Formatter("%(asctime)s %(levelname)-8s %(message)-5s", "%H:%M:%S")
@@ -132,16 +132,16 @@
             """Method for timing the instructions during debug
             """
             message = f"Time (s) {instruction}: {timee}"
             N2PLog._N2PLog__logger.debug(message)
 
         @staticmethod
         def D101(path) -> None:
-            """Method that shows the location of the VizzerClasses library found"""
-            message = f"VizzerClasses found at: {path}"
+            """Method that shows the location of the NaxToModel library found"""
+            message = f"NaxToModel found at: {path}"
             N2PLog._N2PLog__logger.debug(message)
 
         @staticmethod
         def D102() -> None:
             """Method that shows if the property Program_Call of N2ModelContent was changed"""
             message = f"Program_Call of N2ModelContent has been set"
             N2PLog._N2PLog__logger.debug(message)
@@ -203,26 +203,31 @@
             """
             N2PLog._N2PLog__logger.info(message)
 
         @staticmethod
         def I100() -> None:
             """ Information that show that the NaxToPy Runing Code.
             """
-            from IdaeroLicense import LicenseManager
+            from NaxToLicense import LicenseManager
             from System import DateTime
+            from datetime import datetime
+
+            current_date = datetime.now()
+
+            time_date = DateTime(current_date.year, current_date.month, current_date.day, current_date.hour,
+                                 current_date.minute, current_date.second)
 
-            time_date = DateTime.Now
             licen = LicenseManager()
 
-            if licen.HasLicense():
+            if not licen.HasLicense():
                 err = LicenseManager.GenerateCommunityLicense()
                 licen.HasLicense()
 
             code = licen.GetRunCode(time_date)
-            message = f"I100: The NaxToPy Running with the code: {code}"
+            message = f"I100: NaxToPy Running with the code: {code}"
             N2PLog._set_format2(time_date.ToString().split(" ")[1])
             N2PLog._N2PLog__logger.info(message)
             N2PLog._set_format1()
 
         @staticmethod
         def I101(vizzer_libs) -> None:
             """ Information that show that the NaxTo libraries were correctly found at vizzer_libs.
@@ -264,24 +269,24 @@
             """ Information given when the program is called from a .exe file.
             """
             message = "I107: Working with the executable version of NaxToPy."
             N2PLog._N2PLog__logger.info(message)
 
         @staticmethod
         def I108() -> None:
-            """ Information given when the program use the develover version of VizzerClasses.
+            """ Information given when the program use the develover version of NaxToModel.
             """
-            message = "I108: Working with developer version of VizzerClasses."
+            message = "I108: Working with developer version of NaxToModel."
             N2PLog._N2PLog__logger.info(message)
 
         @staticmethod
         def I109() -> None:
-            """ Information given when the VizzerClasses library is load correctly.
+            """ Information given when the NaxToModel library is load correctly.
             """
-            message = f"I109: The library VizzerClasses.dll was load successfully."
+            message = f"I109: The library NaxToModel.dll was load successfully."
             N2PLog._N2PLog__logger.info(message)
 
         @staticmethod
         def I110(path) -> None:
             """ Information given when the file .N2P is saved correctly.
             """
             message = f"I110: The file {path} has been successfully saved."
@@ -375,14 +380,30 @@
         def W103() -> None:
             """ Warning raised when the Windows Register is modified by NaxToPy: The Path value is deleted
             """
             message = f"W103: The Path Value in Windows Register has been deleted."
             N2PLog._N2PLog__logger.warning(message)
 
         @staticmethod
+        def W104(naxver) -> None:
+            """ Warning raised when the version NaxTo that this NaxToPy version is prepared for is not found
+            """
+            message = f"W104: This NaxToPy should work with {naxver}, that is NOT found. Checking compatibility with" \
+                      f"other versions installed"
+            N2PLog._N2PLog__logger.warning(message)
+
+        @staticmethod
+        def W105() -> None:
+            """ Warning raised when the assemblies founded are not saved as compatible
+            """
+            message = f"W105: No library was found to be compatible with this NaxToPy version. The package may" \
+                      f"work but is recommended to find a compatible NaxTo or NaxToPy version."
+            N2PLog._N2PLog__logger.warning(message)
+
+        @staticmethod
         def W200() -> None:
             """ Warning raised when the executable file is build without the icon
             """
             message = "W200: The .exe file will not have the NaxToPy icon. There should have been an error while loading it"
             N2PLog._N2PLog__logger.warning(message)
 
         @staticmethod
@@ -831,18 +852,19 @@
         def E311() -> None:
             ''' Error raised when the sortby parameter of the N2PReport is not one of the possible ones.
             '''
             message = f"E311: THE SORTBY PARAMETER FOR A N2PREPORT MUST BE 'LC' OR 'IDS' "
             N2PLog._N2PLog__logger.error(message)
 
         @staticmethod
-        def E312() -> None:
-            ''' Error raised when the components asked for the N2PReport are not found in the model
+        def E312(lc, result) -> None:
+            ''' Error raised when the components asked for the N2PReport are not found in the result of the loadcase
             '''
-            message = f"E312: THE COMPONENTS ASKED FOR THE N2PREPORT ARE NOT IN THE MODEL"
+            message = f"E312: THE COMPONENTS ASKED FOR THE N2PREPORT ARE NOT IN THE RESULT {result} OF THE " \
+                      f"LOAD CASE {lc}"
             N2PLog._N2PLog__logger.error(message)
 
         @staticmethod
         def E313() -> None:
             ''' Error raised when there is an error in the arguments, probably in the formulas.
             '''
             message = f"E313: THERE IS AN ERROR IN THE ARGUMENTS OF THE METHOD new_report()"
@@ -919,15 +941,15 @@
             message = f"C102: THE CURRENT PYTHON VERSION ({py_version}) IS NOT SUPPORTED."
             N2PLog._N2PLog__logger.critical(message)
 
         @staticmethod
         def C103() -> None:
             """ Critical Error raised when VizzerClasses.dll is not properly load.
             """
-            message = f"C103: THE LIBRARY 'VizzerClasses.dll' COULDN'T BE LOADED CORRECTLY"
+            message = f"C103: THE LIBRARY 'NaxToModel.dll' COULDN'T BE LOADED CORRECTLY"
             N2PLog._N2PLog__logger.critical(message)
 
         @staticmethod
         def C104() -> None:
             """ Critical Error raised when the console argument in n2ptoexe is not a bool type.
             """
             message = f"C104: THE ARGUMENT CONSOLE MUST BE A BOOLEAN: True | False"
@@ -959,24 +981,26 @@
             """ Error raised when the file couldn't be found.
             """
             message = f"C108: THE FILE {path} DOESN'T EXIST"
             N2PLog._N2PLog__logger.critical(message)
 
         @staticmethod
         def C109(ver, comp_ver) -> None:
-            """ Error raised when NaxTo is not installed.
+            """ Error raised when NaxTo is not compatible with NaxToPy.
             """
-            message = f"C109: THIS VERSION OF NAXTOPY ({ver}) IS ONLY COMPATIBLE WITH THIS ASSEMBLY VERSION: {comp_ver}"
+            message = f"C109: THIS VERSION OF NAXTOPY ({ver}) IS NOT COMPATIBLE WITH THIS ASSEMBLY VERSION: {comp_ver}"
             N2PLog._N2PLog__logger.critical(message)
 
         @staticmethod
-        def C110(ver, comp_ver) -> None:
+        def C110(ver, naxver) -> None:
             """ Error raised when there aren't installed a compatible version of  with minor changes.
             """
-            message = f"C110: THIS VERSION OF NAXTOPY({ver}) IS NOT COMPATIBLE WITH THIS NAXTO VERSION: {comp_ver}"
+            message = f"C110: THIS VERSION OF NAXTOPY({ver}) IS NOT COMPATIBLE WITH THE NAXTO VERSIONS THAT ARE " \
+                      f"INSTALLED. UPDATE TO A COMPATIBLE NAXTO VERSION ({naxver}) OR DOWNLOAD FROM " \
+                      f"https://pypi.org/project/NaxToPy/ A COMPATIBLE NAXTOPY VERSION"
             N2PLog._N2PLog__logger.critical(message)
 
         @staticmethod
         def C111(ver) -> None:
             """ Error raised when there version of NaxTo is not found.
             """
             message = f"C111: NAXTO VERSION WAS NOT FOUND. PLEASE, CHECK IF NAXTO{ver} IS INSTALLED"
@@ -990,14 +1014,22 @@
             """
             message = f"C112: ERROR RAISED WHEN THERE IS AN ERROR IN THE SA OF ELEMENTS. THIS MAY BE CAUSED BY A MEMORY" \
                       f"LEAK IN THE LOW LEVEL LIBRERIES. A SOLUTION MAY BE CHANGE THE \"initilaize\" method to parallel:" \
                       f"model = NaxToPy.load_model(path, parallelprocessing=True)"
             N2PLog._N2PLog__logger.critical(message)
 
         @staticmethod
+        def C113(lib, ver, listver) -> None:
+            """ Error raised when the NaxToPy versions the dll is compatible with is not this one
+            """
+            message = f"C113: THE LIBRARY {lib} IS NOT COMPATIBLE WITH NAXTOPY {ver}. INSTALL ANY OF THESE VERSION OF" \
+                      f"NAXTOPY {listver} OR UPDATE NAXTO"
+            N2PLog._N2PLog__logger.critical(message)
+
+        @staticmethod
         def C200() -> None:
             """ Critical error raised when numpy couldn't be installed.
             """
             message = "C200: NUMPY PACKAGE COULDN\'T BE INSTALLED. PLEASE, INSATALL IT MANUALY."
             N2PLog._N2PLog__logger.critical(message)
 
     # ------------------------------------------------------------------------------------------------------------------
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/N2PModelContent.py` & `naxtopy-2.0.0/src/NaxToPy/Core/N2PModelContent.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from VizzerClasses import N2ModelContent
-from VizzerClasses import N2LoadCase
-from VizzerClasses.Classes import N2AdjacencyFunctions
-from VizzerClasses.Classes import N2FreeEdges
-from VizzerClasses import EnvelopGroup
-from VizzerClasses import EnvelopCriteria
+from NaxToModel import N2ModelContent
+from NaxToModel import N2LoadCase
+from NaxToModel.Classes import N2AdjacencyFunctions
+from NaxToModel.Classes import N2FreeEdges
+from NaxToModel import EnvelopGroup
+from NaxToModel import EnvelopCriteria
 from NaxToPy.Core.Classes.N2PLoadCase import N2PLoadCase
 from NaxToPy.Core.Classes.N2PIncrement import N2PIncrement
 from NaxToPy.Core.Classes.N2PElement import N2PElement
 from NaxToPy.Core.Classes.N2PConnector import N2PConnector
 from NaxToPy.Core.Classes.N2PNode import N2PNode
 from NaxToPy.Core.Classes.N2PCoord import N2PCoord
 from NaxToPy.Core.Classes.N2PConnector import N2PConnector
@@ -15,22 +15,25 @@
 from NaxToPy.Core.Errors.N2PLog import N2PLog
 from NaxToPy.Core.Classes.N2PMaterial import N2PMaterial, N2PMatE, N2PMatMisc, N2PMatI
 from NaxToPy.Core.Classes.N2PProperty import N2PProperty, N2PComp, N2PShell, N2PSolid
 from NaxToPy.Core.Classes.N2PSet import N2PSet
 from NaxToPy.Core.Classes.N2PModelInputData import *
 from NaxToPy.Core.Constants.Constants import BINARY_EXTENSIONS
 from NaxToPy.Core.Classes.N2PReport import N2PReport
+
+
 import time
 import sys
 import numpy as np
 import os
 import array
 import System
 from collections import OrderedDict
 from typing import Union, overload
+from itertools import chain
 
 
 # Clase Model Content de Python ----------------------------------------------------------------------------------------
 class N2PModelContent:
     '''Main Class of the NaxToPy package. Keeps almost all the information contained in the output result.
 
     Attributes:
@@ -265,23 +268,23 @@
         N2PLog.Debug.D100("N2PConnector Dictionary", t2-t1)
         # --------------------------------------------------------------------------------------------------------------
 
         ################################################################################################################
         ########################################    N2PModelInputData     ##############################################
         ################################################################################################################
         t1 = time.time()
-        if self.__vzmodel.InfoInputFileData is not None:
-            n2pmodelimpudata = self.__vzmodel.InfoInputFileData.ListBulkDataCards
+        if self.__vzmodel.NastranInfoInputFileData is not None:
+            n2pmodelimpudata = self.__vzmodel.NastranInfoInputFileData.ListBulkDataCards
 
             #lista_cards = zeros(len(n2pmodelimpudata), object)
             #diccionario
             #llamar por separado a las tarjetas (props, elems, mat, ...)
             #lista_cards = [construct_dict[card.CardType.ToString()](card) for card in n2pmodelimpudata]
             lista_cards = list(CONSTRUCTDICT[card.CardType.ToString()](card) for card in n2pmodelimpudata)
-            self.__modelinputdata = N2PModelInputData(lista_cards, self.__vzmodel.InfoInputFileData)
+            self.__modelinputdata = N2PModelInputData(lista_cards, self.__vzmodel.NastranInfoInputFileData)
 
         else:
             self.__modelinputdata = None
         t2 = time.time()-t1
         N2PLog.Debug.D100("N2PModelInputData", t2)
         # --------------------------------------------------------------------------------------------------------------
     # ------------------------------------------------------------------------------------------------------------------
@@ -381,19 +384,19 @@
 
             dictmateriales = dict(self.__vzmodel.N2MatDict)
 
             for key, value in dictmateriales.items():
                 if self.Solver == "Nastran" or self.Solver == "Optistruct" or self.Solver == "InputFileNastran":
                     key = int(key)
 
-                if value.GetType().ToString() == 'VizzerClasses.N2MatE':
+                if value.GetType().ToString() == 'NaxToModel.N2MatE':
                     self.__material_dict[key] = N2PMatE(value, self)
-                elif value.GetType().ToString() == 'VizzerClasses.N2MatI':
+                elif value.GetType().ToString() == 'NaxToModel.N2MatI':
                     self.__material_dict[key] = N2PMatI(value, self)
-                elif value.GetType().ToString() == 'VizzerClasses.N2MatMisc':
+                elif value.GetType().ToString() == 'NaxToModel.N2MatMisc':
                     self.__material_dict[key] = N2PMatMisc(value, self)
 
         t2 = time.time()
         N2PLog.Debug.D100("N2PMaterial Dictionary", t2-t1)
         return self.__material_dict
     # ------------------------------------------------------------------------------------------------------------------
 
@@ -419,21 +422,21 @@
             for key, value in dictprop.items():
 
                 if self.Solver == "Nastran" or self.Solver == "Optistruct" or self.Solver == "InputFileNastran":
                     key = int(key)
                     if key < 0:
                         N2PLog.Error.E227(key)
 
-                if value.GetType().ToString() == 'VizzerClasses.N2Shell':
+                if value.GetType().ToString() == 'NaxToModel.N2Shell':
                     self.__property_dict[key] = N2PShell(value, self)
 
-                elif value.GetType().ToString() == 'VizzerClasses.N2Comp':
+                elif value.GetType().ToString() == 'NaxToModel.N2Comp':
                     self.__property_dict[key] = N2PComp(value, self)
 
-                elif value.GetType().ToString() == 'VizzerClasses.N2Solid':
+                elif value.GetType().ToString() == 'NaxToModel.N2Solid':
                     self.__property_dict[key] = N2PSolid(value, self)
 
         t2 = time.time()
         N2PLog.Debug.D100("N2PProperty Dictionary", t2 - t1)
         return self.__property_dict
     # ------------------------------------------------------------------------------------------------------------------
 
@@ -1088,21 +1091,21 @@
 
         if i > 0:
             N2PLog.Warning.W301(name)
 
         # Argumentos para N2LoadCase
         envelopgroup = N2LoadCase
 
-        # Genera una instancia de un N2LoadCase the VizzerClasses
+        # Genera una instancia de un N2LoadCase de NaxToModel
         cs_lc = N2LoadCase(self.__vzmodel, name, formula)
 
         # Método de N2LoadCase que pone todoo en su sitio
         cs_lc.RecalculateLCInfo2Formule()
 
-        # Se transforma el caso de carga de VizzerClasses en un N2PLoadCase de python
+        # Se transforma el caso de carga de NaxToModel en un N2PLoadCase de python
         py_lc = N2PLoadCase(cs_lc.ID, cs_lc.IDOriginal, cs_lc.Increments, cs_lc.IncrementsNumberList, cs_lc.IsComplex,
                             cs_lc.TypeLoadCase, cs_lc.Name, cs_lc.Results, cs_lc.SolutionType, cs_lc.Solver, self, cs_lc)
 
         # Se añade el caso de carga de csharp a N2ModelContent de Vizzer
         self.__vzmodel.LoadCases.Add(cs_lc)
 
         # Se añade el case de carga de python a N2PModelContent
@@ -1110,15 +1113,16 @@
 
         # Se añade al diccionario si este ya existe
         if self.__LCs_by_ID__:
             self.__LCs_by_ID__[py_lc.ID] = py_lc
 
         return py_lc
 
-    def new_envelope_loadcase(self, name: str, formula: str, criteria: str="ExtremeMax") -> N2PLoadCase:
+    def new_envelope_loadcase(self, name: str, formula: str, criteria: str = "ExtremeMax",
+                              envelgroup: str = "ByContour") -> N2PLoadCase:
         """Method of N2PModelContent that generate a new N2PLoadCase that is the envelope of the load cases and increments
         selected.
 
         The id is automatically generated. It will be negative, starting at -1. If the new load case use a derivated or
         envelope load case use LCD1 in the formula instead of LC-1:
 
         Args:
@@ -1169,21 +1173,21 @@
         envelgroup_maping = {
             'ByContour': EnvelopGroup.ByContour,
             'ByLoadCaseID': EnvelopGroup.ByLoadCaseID,
             'ByIncrement': EnvelopGroup.ByIncrement
         }
         envelopgroup = envelgroup_maping.get(envelgroup, EnvelopGroup.ByContour)
 
-        # Genera una instancia de un N2LoadCase the VizzerClasses
+        # Genera una instancia de un N2LoadCase de NaxToModel
         cs_lc = N2LoadCase(self.__vzmodel, name, formula, True, envelopgroup, False, envelopcriteria)
 
         # Método de N2LoadCase que pone todoo en su sitio
         cs_lc.RecalculateLCInfo2Formule()
 
-        # Se transforma el caso de carga de VizzerClasses en un N2PLoadCase de python
+        # Se transforma el caso de carga de NaxToModel en un N2PLoadCase de python
         py_lc = N2PLoadCase(cs_lc.ID, cs_lc.IDOriginal, cs_lc.Increments, cs_lc.IncrementsNumberList, cs_lc.IsComplex,
                             cs_lc.TypeLoadCase, cs_lc.Name, cs_lc.Results, cs_lc.SolutionType, cs_lc.Solver, self, cs_lc)
 
         # Se añade el caso de carga de csharp a N2ModelContent de Vizzer
         self.__vzmodel.LoadCases.Add(cs_lc)
 
         # Se añade el case de carga de python a N2PModelContent
@@ -1223,15 +1227,15 @@
             allincr: bool -> Parameter for asking all increments for the load cases asked.
 
             result: str -> Name of the result to ask.
 
             componentssections: str -> Formula with the components and the section desired. Each component can have
                 several sections, and the structure must be: <ComopnentName:X#Y#Z#> where X, Y, Z are the names of the
                 section. After each name of section there must be an #, even if there is only one. Example:
-                "<VONMISES:Z1#Z2#>,<MAX_SHEAR:Z1#Z2#>"
+                "<VONMISES:Z1#Z2#>,<MAX_SHEAR:Z1#Z2#>". If there is no section, use NONE#: "<FX:NONE#>,<FY:NONE#>"
 
             ifenvelope: bool -> Parameter to ask only for the results of the envelope of the load cases
 
             selection: list -> List of N2PElement or N2PNode where the results are desired. The user must take care that
                 with displacements the list must be nodes and for stresses must be elements.
 
             sortby: str -> This parameter have two options: "LC" and "IDS". Specify if the results should be sorted by
@@ -1285,17 +1289,18 @@
             False, list_n2pelements, "IDS", aveSections=-4, coordsys=-1)
         """
         # Here it is checkd if the components, the loadcases and the result exist and the formula is right
         try:
             lcs = [int(lc.split(":")[0][3:]) for lc in lc_incr.split(",")]
             components = [c.split(":")[0][1:] for c in componentssections.split(",")]
             for lc in lcs:
-                A = self.get_load_case(lc).get_result(result).Components.keys()
-                if not all(c in self.get_load_case(lc).get_result(result).Components.keys() for c in components):
-                    N2PLog.Error.E312()
+                all_comps = chain(self.get_load_case(lc).get_result(result).Components.keys(),
+                                  self.get_load_case(lc).get_result(result).DerivedComponents.keys())
+                if not all(c in all_comps for c in components):
+                    N2PLog.Error.E312(lc, result)
                     return "ERROR"
         except:
             N2PLog.Error.E313()
             return "ERROR"
 
         return N2PReport(self.__vzmodel, lc_incr, allincr, result, componentssections, ifenvelope, selection, sortby,
                          aveSections, cornerData, aveNodes, variation, realPolar, coordsys, v1, v2)
@@ -1377,26 +1382,28 @@
             aux_lc = list_lc_incr[0][0]
         elif isinstance(list_lc_incr[0][0], int):
             aux_lc = self.get_load_case(list_lc_incr[0][0])
         else:
             N2PLog.Error.E310()
             return None
 
+        n2pcomp = aux_lc.get_result(result).get_component(component)
+
         # Aqui se llama la funcion de verdad que es un metodo de N2PComponent. Se llama a ella porque hace uso de otras
         # funciones ya definidas (n2paraminputresult) en la clase y es mejor no repetir codigo.
-        return aux_lc.get_result(result).get_component(component)._get_result_by_LCs_Incr(list_lc_incr,
-                                                                                          sections,
-                                                                                          aveSections,
-                                                                                          cornerData,
-                                                                                          aveNodes,
-                                                                                          variation,
-                                                                                          realPolar,
-                                                                                          coordsys,
-                                                                                          v1,
-                                                                                          v2)
+        return n2pcomp._get_result_by_LCs_Incr(list_lc_incr,
+                                               sections,
+                                               aveSections,
+                                               cornerData,
+                                               aveNodes,
+                                               variation,
+                                               realPolar,
+                                               coordsys,
+                                               v1,
+                                               v2)
 
     # ------------------------------------------------------------------------------------------------------------------
 
     ####################################################################################################################
     #######################################     ElementsCoordSys      ##################################################
     ####################################################################################################################
     def _elements_coord_sys(self):
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/Reference_Finder/__Reference_Finder.py` & `naxtopy-2.0.0/src/NaxToPy/Core/Reference_Finder/__Reference_Finder.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     else:
         N2PLog.Critical.C102(py_version)
         # sys.exit(f"C102: THE CURRENT PYTHON VERSION IS NOT SUPPORTED.")
 
 
 # Funcion que devuelve la ruta donde se encuentran las librerias de NaxTo----------------------
 def vizzer_libs() -> list[str, ...]:
-    """Funcion que devuelve las rutas donde se encuentran las librerias de VizzerClasses. Si hay varias versiones
+    """Funcion que devuelve las rutas donde se encuentran las librerias de NaxToModel. Si hay varias versiones
     puede haber varias rutas.
 
     ----------
     Returns: 
         vizzer_libs: str
             Ruta a las librerias de NaxTo
     """
     vizzer_libs = []
 
-    # Miro en LOCAL MACHINE, donde está instalado el NAXTOVIEW. Ahí se busca la libreria de VizzerClasses.
+    # Miro en LOCAL MACHINE, donde está instalado el NAXTOVIEW. Ahí se busca la libreria de NaxToModel.
     key_id = winreg.HKEY_LOCAL_MACHINE
 
     try:
         sub_key_id = winreg.OpenKeyEx(key_id, os.path.join("SOFTWARE", "IDAERO"))
         naxto_ver = winreg.QueryInfoKey(sub_key_id)
         naxto_ver2 = list()
 
@@ -150,74 +150,116 @@
             N2PLog.Warning.W103()
     except FileNotFoundError:
         pass
 # ----------------------------------------------------------------------------------------------------------------------
 
 
 # ----------------------------------------------------------------------------------------------------------------------
-def compatible_vizzer(vizzer_libs: list) -> str:
-    """Returns the path of the VizzerClasses this NaxToPy version is compatible with"""
+def compatible_vizzer(vizzer_libs: list) -> tuple[str, bool]:
+    """Returns the path of the NaxToModel this NaxToPy version is compatible with"""
 
+    # Se busca si alguna de las rutas contiene la version para la que esta preparado esta version
+    for lib in vizzer_libs:
+        if NAXTO_VERSION in lib:
+            lib_path = lib + "\\" + VIZZER_CLASSES_DLL
+
+            # Si alguna es de esta version hay que ver si el assembly, que cambia con cada step es compatible.
+            # Previamente se verifica que el archivo existe:
+            if os.path.exists(lib_path):
+                versionInfo = FileVersionInfo.GetVersionInfo(lib_path)
+                assemblyVersion = versionInfo.FileVersion
+
+                # Si la version es compatible se devuelve la ruta y un boleano indicando si es compatible
+                if assemblyVersion in VIZZER_COMPATIBILITY:
+                    return lib_path, True
+
+    N2PLog.Warning.W104(NAXTO_VERSION)
+    # Aunque la version este bien, el assembly no. Puede que de un step a otro no haya compatibilidad.
+    backup = ""
+
+    # Comprobamos si hay alguna version que contenga una dll compatible
     for lib in vizzer_libs:
         lib_path = lib + "\\" + VIZZER_CLASSES_DLL
+        if not os.path.exists(lib_path):
+            continue
         versionInfo = FileVersionInfo.GetVersionInfo(lib_path)
         assemblyVersion = versionInfo.FileVersion
 
-        if assemblyVersion == VIZZER_ASSEMBLY:
-            return lib_path
+        if not backup:
+            backup = lib_path
+
+        if assemblyVersion in VIZZER_COMPATIBILITY:
+            return lib_path, True
+
+    N2PLog.Warning.W105()
+
+    # Si ninguna libreria es compatible se prueba con una de ellas, la primera que exista. Pero se indica que no es
+    # compatible. Mas adelante se comprubea si dentro de la libreria se indica que esta version de NaxToPy es compatible
+    # con ella
+    if backup:
+        return backup, False
+    else:
+        N2PLog.Critical.C110(VERSION, NAXTO_VERSION)
 
-    N2PLog.Critical.C109(VERSION, VIZZER_ASSEMBLY)
     # sys.exit()
 # ---------------------------------------------------------------------------------------------
 
 
 def _naxto_gen(vizzer: str) -> str:
     dir_viz = os.path.dirname(vizzer)
     if "GIT_REPOSITORIES" in dir_viz:
-        return os.path.join(r"C:\GIT_REPOSITORIES\NAXTO\NAXTOLibsDebug\NAXLicense\v.3.0", "IdaeroLicense.dll")
-    return os.path.join(dir_viz, "IdaeroLicense.dll")
+        return os.path.join(r"C:\GIT_REPOSITORIES\NAXTO\NAXTOLibsDebug\NAXLicense\v.4.0", "NaxToLicense.dll")
+    return os.path.join(dir_viz, "NaxToLicense.dll")
 
 
-# Inicializador para encontrar la libreria de VizzerClasses
+# Inicializador para encontrar la libreria de NaxToModel
 def __reference_finder():
     # La ruta cambia si se tiene el repositorio de NaxToView
     developer_vizzer = DEVELOPER_VIZZER + "\\" + VIZZER_CLASSES_DLL
+    compatible = True
 
     # Si se crea un .exe queremos que encuentre unas nuevas librerias distribuibles, que estarán en la carpeta temporal que se
     # crea cuando se ejecuta el .exe. Tampoco se ejecutan los modulos del reference finder
     if getattr(sys, 'frozen', False):
         destroy_register()
         create_register()
         exe_dir = sys._MEIPASS
-        vizzer_path = exe_dir + "\\bin\\VizzerClasses.dll"
+        vizzer_path = exe_dir + "\\bin\\NaxToModel.dll"
         N2PLog.Info.I107()
 
     elif os.path.isfile(developer_vizzer):
         if VERSION.split(".")[-1][0:3] == "dev":
             destroy_register()
             create_register()
 
         vizzer_path = developer_vizzer
         N2PLog.Info.I108()
 
     else:
         destroy_register()
         # Compruebo que la version de python es compatible
         py_ver_comp()
-        # Busco todas las vizzerclasses
+        # Busco todas las NaxToModel
         list_libs = vizzer_libs()
-        # Devuelvo el path de la vizzerclasses que es compatible con NaxToPy
-        vizzer_path = compatible_vizzer(list_libs)
+
+        vizzer_path, compatible = compatible_vizzer(list_libs)
 
     # Llamada a las librerias
     try:
         clr.AddReference(vizzer_path)
+        if not compatible:
+            from NaxToModel import Global
+            if VERSION in list(Global.NAXTOPY_COMPATIBILITY):
+                pass
+            else:
+                N2PLog.Critical.C113(vizzer_path, VERSION, list(Global.NAXTOPY_COMPATIBILITY))
+                sys.exit()
         N2PLog.Info.I109()
         N2PLog.Debug.D101(vizzer_path)
         naxto_c = _naxto_gen(vizzer_path)
         clr.AddReference(naxto_c)
     except:
         N2PLog.Critical.C103()
-        # sys.exit("C103: THE LIBRARY 'VizzerClasses.dll' COULDN'T BE LOADED CORRECTLY")
+        # sys.exit("C103: THE LIBRARY 'NaxToModel.dll' COULDN'T BE LOADED CORRECTLY")
 
     N2PLog.Info.I100()
 # ---------------------------------------------------------------------------------------------
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Core/_AuxFunc/_NetToPython.py` & `naxtopy-2.0.0/src/NaxToPy/Core/_AuxFunc/_NetToPython.py`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Modules/Fasteners/N2PUpdateFastener.py` & `naxtopy-2.0.0/src/NaxToPy/Modules/Fasteners/N2PUpdateFastener.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,62 @@
 from NaxToPy.Core.N2PModelContent import N2PModelContent, N2PProperty, N2PModelInputData, N2PNode
 from NaxToPy.Core.N2PModelContent import N2PElement
 
 
 class N2PUpdateFastener:
     """
     This class stores information about fasteners and provides methods to update their stiffness and generate a new
-    bdf file with the updated data.
+    FEM Input File (.bdf, .fem, .dat, etc.) file with the updated data.
 
     Fastener information can be input either as a dictionary (for a single type of fastener) or as a list of dictionaries
     (for multiple types). Each dictionary must include at least the keys for diameter ["D"] and elastic modulus ["E"].
     Optional keys include head height ["h_head"], nut height ["h_nut"], Poisson ratio ["nu"], shear modulus ["G"],
     connection type ("bolt" or "rivet") ["connection_type"], shear type ("simple" or "double") ["shear_type"], and the
     beta value for Nelson method ["beta"].
 
     IDs of fasteners to be updated can be provided as either a single list (for a single type of fastener) or as a list
     of lists (for multiple types). If no list of IDs is provided, all fasteners in the model will be updated.
 
     When multiple types of fasteners are used, the order of the list of dictionaries must match the order of the list
     of ID lists to ensure proper mapping of variables.
 
     Supported methods for stiffness calculation include HUTH, TATE_ROSENFELD, SWIFT, BOEING, GRUMMAN, and NELSON.
+
+    Example:
+        Example 1:
+
+        >>> import NaxToPy as n2p
+        >>> model = n2p.load_model("model.dat")
+        >>> info1 = {"D": 4.8,
+        ...         "E": 110000}
+        >>> info2 = {"D": 7.2,
+        ...         "E": 70000,
+        ...         "connection_type": "rivet",
+        ...         "shear_type": "double"}
+        >>> ele1 = [1000, 1001, 1002]
+        >>> ele2 = [2000, 2001, 2002]
+        >>> update1 = N2PUpdateFastener(model, [info1, info2], [ele1, ele2], "BOEING")
+        >>> update1.calculate() # This will update the model in memory with the information of the object.
+        >>> model.ModelInputData.rebuild_file() # With the model updated, the model is rewritten
+
+        Example 2:
+
+        >>> model = n2p.load_model("model.dat")
+        >>> update2 = N2PUpdateFastener(model, {}) # Create the object without information
+        >>> update2.IDList = [3000, 3001, 3002] # Add the information using it properties
+        >>> update2.StiffnessMethod = "GRUMMAN"
+        >>> update2.FastenerInformation = {3000: {"D": 4.8, "E": 70000, "connection_type": "rivet"},
+        ...                                3001: {"D": 6.8, "E": 70000, "connection_type": "bolt"},
+        ...                                3002: {"D": 7.2, "E": 70000, "shear_type": "double"}}
+        >>> update2.calculate() # This will update the model in memory with the information of the object.
+        >>> model.ModelInputData.rebuild_file() # With the model updated, the model is rewritten
+
     """
 
-    def __init__(self,model: N2PModelContent, information: Union[dict, list], id_list: list = None,
+    def __init__(self, model: N2PModelContent, information: Union[dict, list], id_list: list = None,
                  stiffness_method: str = "HUTH"):
         self.__model = model
         self.__stiffness_method = stiffness_method
 
         # Extract information from the model
         tinit = time.time()
         self.__c_rivet, self.__p_rivet, self.__nodes_crivet = self.__info_extraction()
@@ -90,21 +120,16 @@
                 info_fasteners['beta'] = 0.5
 
 
         # Map each fastener with its properties
         self.__mapping_fastener_properties()
 
     def __mapping_fastener_properties(self):
-
-        properties_map = {}
-        for prop, ID in zip(self.__info_list, self.__id_list):
-            for fastener in ID:
-                properties_map[fastener] = prop
-
-        self.__fastener_properties = properties_map
+        self.__fastener_properties = {fastener: prop for prop, IDs in zip(self.__info_list, self.__id_list) for fastener
+                                      in IDs}
 
     def __read_bolts(self, path: str) -> dict:
         """
         Reads a csv containing the information about fasteners to be updated
         Args:
             path (str): path to BDF file
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Modules/N2PEnvelope/N2PEnvelope.py` & `naxtopy-2.0.0/src/NaxToPy/Modules/N2PEnvelope/N2PEnvelope.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Module that generates the envelope of points cloud.
 """
 import sys, os
 import numpy as np
-from VizzerClasses import N2Envelope
+from NaxToModel import N2Envelope
 import System
 from NaxToPy.Core._AuxFunc._NetToPython import _nettonumpy, _numpytonet
 from NaxToPy.Core.Errors.N2PLog import N2PLog
 from typing import Union
 
 # Una envolvente es el conjunto de objetos de una dimensión menor que la de los puntos facilitados, y que es tangente
 # a estos y que los encierra. Es decir, representa la frontera de estos puntos.
@@ -93,22 +93,22 @@
     N2PLog.Info.I203()
 
     # Compruebo que efectivamente el usuario ha introducido un array de Numpy
     if isinstance(array2D, np.ndarray):
 
         # _numpytonet(array2D) es una funcion que transforma un array de numpy en un array de .NET, en este caso en un
         # System.Double[,]
-        # Se llama a la funcion de envelope the vizzerclasses
+        # Se llama a la funcion de envelope de NaxToModel
         aux = N2Envelope.Calculate(_numpytonet(array2D), "all")
 
         # Se crea un array de numpy vacio de objetos. Tiene que ser de objetos porque se mezclan variables, ya que en la
         # columna 0 habra enteros mientras que en las demas habra columnas
         envel = np.zeros((aux.GetLength(0), aux.GetLength(1)), dtype=object)
 
-        # Relleno el array de numpy con los valores obtenidos del array de vizzerclasses
+        # Relleno el array de numpy con los valores obtenidos del array de NaxToModel
         for i in range(aux.GetLength(0)):
             for j in range(aux.GetLength(1)):
                 # qhull devulve los indices empezando por 1. Necesitamos que lo devuelva por 0.
                 if j == 0:
                     envel[i, j] = aux[i, j] - 1
                 else:
                     envel[i, j] = aux[i, j]
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/Modules/N2PtoEXE/N2PtoEXE.py` & `naxtopy-2.0.0/src/NaxToPy/Modules/N2PtoEXE/N2PtoEXE.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pkgutil
 import os
 from pkg_resources import resource_filename
 import sys
 
 import NaxToPy.Core.Reference_Finder.__Reference_Finder as RF
 from NaxToPy.Core.Errors.N2PLog import N2PLog
+from NaxToPy.Core.Constants.Constants import VIZZER_CLASSES_DLL
 
 
 # Funcion que busca el path del icono de NaxToPy -----------------------------------------------------------------------
 def __ico_path() -> str:
     """ Funcion oculta que busca el icono de NaxToPy
 
         Returns: 
@@ -165,15 +166,15 @@
         N2PLog.Critical.C104()
         # sys.exit("C104: THE ARGUMENT CONSOLE MUST BE A BOOLEAN: True | False")
 
 
     if __busca_n2p(path):
 
         libs_paths = RF.vizzer_libs()
-        libs_path = RF.compatible_vizzer(libs_paths)[:-18]
+        libs_path = RF.compatible_vizzer(libs_paths)[0][:-(len(VIZZER_CLASSES_DLL) + 1)]
         dll_list = __list_ext_libs(libs_path, solver, abaqusversion)
         
 
         # Aqui se cargan las propiedades de la llamada a PyInstaler
         pyinstaller_cmd = [path] + [consl]
         pyinstaller_cmd += dll_list
         if icon == -1:
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy/NaxToPy.ico` & `naxtopy-2.0.0/src/NaxToPy/NaxToPy.ico`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy/user_functions.txt` & `naxtopy-2.0.0/src/NaxToPy/user_functions.txt`

 * *Files identical despite different names*

### Comparing `NaxToPy-1.5.6/src/NaxToPy.egg-info/PKG-INFO` & `naxtopy-2.0.0/src/NaxToPy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: NaxToPy
-Version: 1.5.6
+Version: 2.0.0
 Summary: Package for postprocessing FEM results in Python
 Home-page: https://www.idaerosolutions.com/Home/NaxToPy
 Download-URL: https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US
 Author-email: Idaero Solutions <manuel.sanchez@idaerosolutions.com>
-License: Copyright (c) 2023 Idaero Solutions
+License: Copyright (c) 2024 Idaero Solutions
         
         This freeware license agreement (“agreement”) is a legally binding contract
         between the individual who downloads the software (“you”) and the licensor,
         that should be read in its entirety. This is an agreement governing your use
         this software own by Idaero Solutions, further defined herein as “software”,
         and the licensor of the software is willing to provide you with access to the
         software only on the condition that you accept all of the terms and conditions
@@ -142,16 +142,17 @@
 It could be easily combined with other Python packages as Matplotlib or Pandas. This provides access
 to the full coding power of Python to interpret and process the results, without the need to install
 any additional software other than having NaxTo already installed (see the _Download_ and _Homepage_
 links on the left).
 
 **NaxToPy** is a powerful tool for FEM analysis post-processing!
 
-**CAUTION:** This version is only compatible with **NaxTo 2024.0.5**.
-Check in _Programs and Features_ the NaxTo version that is installed.
+**CAUTION:** To use NaxToPy, [**NaxTo**](https://apps.microsoft.com/detail/XP9MMH0KDKGRJN?hl=en-US&gl=US) must be installed.
+This version is compatible with **NaxTo 2024.1**. It may be compatible with all the steps of this version (2024.1.0, 2024.1.1, 2024.1.2, etc.).
+Check in _Programs and Features_ the NaxTo version that is installed. 
 
 ## Installation
 
 
 If python is callable from the command line:
 
 `py -m pip install NaxToPy`
@@ -250,14 +251,19 @@
 ### v.1.5.5
 1. Bug Fix: Now is possible to call the module N2PUpdateFastener
 
 ### v.1.5.6
 1. The method new_envelope_loadcase() now has the option to choose the envelope group. Which means the user can ask for
 the LoadCases that are critical or the Increment that is critical instead of the value.
 
+### v.2.0.0
+1. Changes made to align the library with updates in lower-level dependencies.
+2. New internal methods to look for the compatibility with low-level dependencies.
+3. The name of the .log is now NaxToPy_Year-Month-Day.log.
+
 # Documentation
 
 **NaxToPy** is a package developed by Idaero Solutions© as a part of the **NaxTo** software.
 
 NaxToPy only use three dependeces:
 - NumPy: https://numpy.org/
 - PythonNET: https://pythonnet.github.io/
```

### Comparing `NaxToPy-1.5.6/src/NaxToPy.egg-info/SOURCES.txt` & `naxtopy-2.0.0/src/NaxToPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

