# Comparing `tmp/DLMS_SPODES_client-0.8.7.tar.gz` & `tmp/DLMS_SPODES_client-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.8.7.tar", last modified: Tue Apr 23 11:04:07 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.8.8.tar", last modified: Thu Apr 25 07:27:55 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.8.7.tar` & `DLMS_SPODES_client-0.8.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.090102 DLMS_SPODES_client-0.8.7/
--rw-rw-rw-   0        0        0      526 2024-04-23 11:04:07.090102 DLMS_SPODES_client-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.7/README.md
--rw-rw-rw-   0        0        0      836 2024-04-23 11:03:54.000000 DLMS_SPODES_client-0.8.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-23 11:04:07.091101 DLMS_SPODES_client-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.919098 DLMS_SPODES_client-0.8.7/src/
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.937106 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   115215 2024-04-22 05:45:45.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.908098 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.958101 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.011101 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.073104 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.076102 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     4992 2024-04-22 07:11:32.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0     3749 2024-04-22 08:32:27.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/services.py
--rw-rw-rw-   0        0        0    46225 2024-04-23 09:34:24.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.952123 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3251 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.087101 DLMS_SPODES_client-0.8.7/test/
--rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.7/test/name2.csv
--rw-rw-rw-   0        0        0    10534 2024-04-23 10:56:23.000000 DLMS_SPODES_client-0.8.7/test/test_Client.py
--rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.7/test/test_logger.py
--rw-rw-rw-   0        0        0      360 2024-04-22 08:34:06.000000 DLMS_SPODES_client-0.8.7/test/test_services.py
--rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.7/test/конфигурация GSM.csv
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.593679 DLMS_SPODES_client-0.8.8/
+-rw-rw-rw-   0        0        0      526 2024-04-25 07:27:55.592678 DLMS_SPODES_client-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.8/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-25 07:27:35.000000 DLMS_SPODES_client-0.8.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-25 07:27:55.593679 DLMS_SPODES_client-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.425678 DLMS_SPODES_client-0.8.8/src/
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.441678 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   114782 2024-04-24 12:45:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.414677 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.459677 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.511681 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.576678 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.578679 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     4992 2024-04-22 07:11:32.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0     3749 2024-04-22 08:32:27.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/services.py
+-rw-rw-rw-   0        0        0    45295 2024-04-24 14:11:55.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.455678 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-25 07:27:55.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3251 2024-04-25 07:27:55.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-25 07:27:55.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-25 07:27:55.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-25 07:27:55.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-25 07:27:55.000000 DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-25 07:27:55.590678 DLMS_SPODES_client-0.8.8/test/
+-rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.8/test/name2.csv
+-rw-rw-rw-   0        0        0    10533 2024-04-25 06:53:18.000000 DLMS_SPODES_client-0.8.8/test/test_Client.py
+-rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.8/test/test_logger.py
+-rw-rw-rw-   0        0        0      360 2024-04-22 08:34:06.000000 DLMS_SPODES_client-0.8.8/test/test_services.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.8/test/конфигурация GSM.csv
```

### Comparing `DLMS_SPODES_client-0.8.7/PKG-INFO` & `DLMS_SPODES_client-0.8.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.8.7
+Version: 0.8.8
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.8.7/pyproject.toml` & `DLMS_SPODES_client-0.8.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.8.7"
+version = "0.8.8"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
-    "DLMS-SPODES == 0.69.6",
+    "DLMS-SPODES == 0.70.0",
     "DLMS-SPODES-communications >= 1.2.4",
     "pycryptodomex>=3.15"
 ]
 description="dlms-spodes"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords=['dlms', 'spodes', 'client']
```

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1101,18 +1101,14 @@
         return await self.read_data_block()
 
     def matching_LDN(self, value: octet_string.LDN):
         if value == self.objects.LDN.value:
             """secret matching"""
         elif self.objects.LDN.value is None:
             self.objects.LDN.set_attr(2, value)
-        elif bytes(value)[3:] == bytes(self.objects.LDN.value) and self.objects.manufacturer in (b'101', b'102', b'103', b'104'):
-            # todo: add read version for update
-            self.log(logL.WARN, F"temporary solution(for update 101, 102, 103, 104 to KPZ): changed LDN from {self.objects.LDN.value.to_str()} to {value.to_str()} after update, please save configures!")
-            self.objects.LDN.set_attr(2, value)
         else:
             raise exc.IDError('Несоответствие серийного номера')
 
     @cached_property
     def n_phases(self) -> int:
         """cached phases amount"""
         return self.objects.get_n_phases()
```

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/servers.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/servers.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/services.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/services.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,47 +240,50 @@
                 res = await t.exchange(c)
             except exc.ResultError as e:
                 res = e
             ret.append(res)
         return ret
 
 
-class InitType(ExTask):
-    """nothing params"""
-    # async def exchange(self, c: Client, is_public: bool = False):
-    #     await c.close()  # close hdlc before init
-    #     return await super(InitType, self).exchange(c, is_public=True)
+class FindServerVersion(ExTask):
+    """try find COSEM server version, return: instance(B group), CDT"""
 
-    async def exchange(self, c: Client):
-        # read LDN
-        data = await c.read_attr(collection.AttrDesc.LDN_VALUE)
-        ldn = octet_string.LDN(data)
-        # find device_id(type for Russia)
-        type_value, _ = cdt.get_instance_and_pdu_from_value(await c.read_attr(ut.CosemAttributeDescriptor((1, "0.0.96.1.1.255", 2))))
-        # find version data
+    async def exchange(self, c: Client) -> tuple[int, cdt.CommonDataType]:
         for desc in (ut.CosemAttributeDescriptor((1, "0.0.0.2.1.255", 2)), ut.CosemAttributeDescriptor((1, "0.0.96.1.2.255", 2))):
             try:
-                ver_value, _ = cdt.get_instance_and_pdu_from_value(await c.read_attr(desc))
-                break
+                return desc.instance_id.contents[1], cdt.get_instance_and_pdu_from_value(await c.read_attr(desc))[0]
             except exc.ResultError as e:
                 if e.result == pdu.DataAccessResult.OBJECT_UNDEFINED:
                     """try search in old object and set to new"""
                     continue
                 else:
                     raise e
-            except exc.NeedUpdate as e:
-                c.log(logL.WARN, F"{e}. I do it...")
-                break
         else:
             raise exc.NoObject(F"not find version object in server")
+
+
+class InitType(ExTask):
+    """nothing params"""
+    # async def exchange(self, c: Client, is_public: bool = False):
+    #     await c.close()  # close hdlc before init
+    #     return await super(InitType, self).exchange(c, is_public=True)
+
+    async def exchange(self, c: Client) -> bool:
+        # read LDN
+        data = await c.read_attr(collection.AttrDesc.LDN_VALUE)
+        ldn = octet_string.LDN(data)
+        # find device_id(type for Russia)
+        type_value, _ = cdt.get_instance_and_pdu_from_value(await c.read_attr(ut.CosemAttributeDescriptor((1, "0.0.96.1.1.255", 2))))
+        ver_inst, ser_ver = await FindServerVersion().exchange(c)
         try:
             c.objects = collection.get_collection(
                 manufacturer=ldn.manufacturer(),
                 server_type=type_value,
-                server_ver=AppVersion.from_str(ver_value.to_str()))
+                server_ver=AppVersion.from_str(ser_ver.to_str()),
+                ver_instance=ver_inst)
             c.objects.LDN.set_attr(2, ldn)
         except exc.NoConfig as e:
             c.log(logL.WARN, F"false init type procedure: {e}, start create objects from device")
             new_collection = collection.Collection(ldn=ldn)
             # read association
             object_list: cdt.Array = cdt.Array(await c.read_attr(collection.AttrDesc.OBJECT_LIST), type_=structs.ObjectListElement)
             for c_id, ver, ln, _ in object_list:
@@ -300,14 +303,15 @@
                 keys=(media_id.DEVICE_ID_OBJECTS,
                       media_id.OTHER_ABSTRACT_GENERAL_PURPOSE_OBIS_CODES)):
                 await c.read_attribute(d_id, 2)
 
             # TODO: handle 6.2.42 DLMS UA 1000-1 Ed. 14 - Device ID objects, 6.2.4 Other abstract general purpose OBIS codes(Program entries for version)
             # TODO: keep in Types
         c.log(logL.INFO, F"added {len(c.objects)} DLMS objects")
+        return True
 
 
 @dataclass
 class ReadAttribute(ExTask):
     ln: collection.LNContaining
     index: int
 
@@ -476,32 +480,14 @@
 
 
 @dataclass
 class UpdateFirmware(ExTask):
     """only for KPZ now"""
 
     async def exchange(self, c: Client) -> bool:
-        # check available action todo: not work in 0.0.38
-        # if c.current_association.object_list is None:
-        #     await ReadAttribute(
-        #         ln=c.current_association.logical_name,
-        #         index=2
-        #     ).exchange(c)
-        # image_objects: collection.ImageTransfer = collection.get_filtered(objects=c.current_association.objects, keys=(overview.ClassID.IMAGE_TRANSFER, ))
-        # if len(image_objects) == 0:
-        #     c.set_error(Application.MISSING_OBJ, "not find image_transfer in current association")
-        #     return False
-        # for obj in image_objects:
-        #     if not c.current_association.is_accessible(
-        #                                         ln=obj.logical_name,
-        #                                         index=4,    # image_activate
-        #                                         m_id=c.m_id):
-        #         c.set_error(Transmit.NO_ACCESS, "not has access for activate image in current association")
-        #         return False
-        # read properties for update
         read_seq = Sequence()
         match c.objects.collection_ver:
             case AppVersion(0, 0, patch) if 25 <= patch < 26:
                 read_seq.append(ReadAttribute(
                     ln=c.objects.firmwares_description.logical_name,
                     index=2))
                 read_seq.append(ReadAttribute(
@@ -542,20 +528,15 @@
                     index=2))
                 read_seq.append(ReadAttributes(
                     ln=c.objects.firmware_image_transfer.logical_name,
                     indexes=(2, 6)))
                 read_seq.append(ReadAttribute(
                     ln=c.objects.boot_image_transfer.logical_name,
                     index=2))
-            case AppVersion(-1):
-                read_seq.append(ReadAttribute(
-                    ln=c.objects.firmware_version.logical_name,
-                    index=2))
-                c.set_error(Application.VERSION_ERROR, 'Need reread')
-            case AppVersion(0, 0, 0):
+            case AppVersion(0, 0, 0) | AppVersion(-1):
                 c.set_error(Application.VERSION_ERROR, 'Unknown metrology Version')
                 return False
             case AppVersion():
                 c.set_error(Application.VERSION_ERROR, F'Version {c.objects.server_ver} don\'t read update properties')
                 return False
             case _:
                 c.set_error(Transmit.READ_ERROR, 'Wrong AppVersion')
@@ -639,38 +620,46 @@
         # update
         match c.objects.server_ver[0]:
             case AppVersion(0, 0, 53 | 54) | AppVersion(1, 1 | 2 | 3 | 4 | 5 | 6):
                 if await self.__is_updated_image_3(c=c, obj=c.objects.boot_image_transfer):
                     await ReadAttribute(
                         ln=c.objects.firmwares_description.logical_name,
                         index=2).exchange(c)
-                    return await self.__is_updated_image_3(c=c, obj=c.objects.firmware_image_transfer)
+                    res = await self.__is_updated_image_3(c=c, obj=c.objects.firmware_image_transfer)
+                else:
+                    return False
             case AppVersion(0, 0, patch) if 48 <= patch <= 52:
                 if await self.__is_updated_image_2(c=c, obj=c.objects.boot_image_transfer):
                     await ReadAttribute(
                         ln=c.objects.firmwares_description.logical_name,
                         index=2
                     ).exchange(c)
-                    return await self.__is_updated_image_2(c=c, obj=c.objects.firmware_image_transfer)
+                    res = await self.__is_updated_image_2(c=c, obj=c.objects.firmware_image_transfer)
+                else:
+                    return False
             case AppVersion(0, 0, patch) if 39 <= patch <= 47:
                 if await self.__is_updated_image(c=c, obj=c.objects.boot_image_transfer):
                     await ReadAttribute(
                         ln=c.objects.firmwares_description.logical_name,
                         index=2
                     ).exchange(c)
-                    return await self.__is_updated_image(c=c, obj=c.objects.firmware_image_transfer)
+                    res = await self.__is_updated_image(c=c, obj=c.objects.firmware_image_transfer)
+                else:
+                    return False
             case AppVersion(0, 0, patch) if 25 <= patch <= 38:
-                return await self.__is_updated_image(c=c, obj=c.objects.firmware_image_transfer)
+                res = await self.__is_updated_image(c=c, obj=c.objects.firmware_image_transfer)
             case AppVersion(0, 0, 0):
                 c.set_error(Transmit.EXECUTE_ERROR, F'Не могу установить номер версии счетчика')
                 return False
             case AppVersion():
                 c.set_error(Transmit.EXECUTE_ERROR, F'Невозможно обновить версию {c.objects.server_ver}')
                 return False
-        return False
+            case _:
+                return False
+        return await InitType().exchange(c)
 
     async def __is_updated_image(self, c: Client, obj: collection.ImageTransfer) -> bool:
         """ update image if blocks is fulls """
         if obj.is_image_exist:
             c.current_obj = obj
             try:
                 await c.execute_method(obj.get_meth_descriptor(1))
@@ -691,15 +680,15 @@
                 return True
             except Exception as e:
                 c.log(logL.ERR, F'unhandled update error. {e.args[0]}')
                 return False
         else:
             return True
 
-    async def __is_updated_image_2(self, c: Client, obj: collection.ImageTransfer, with_abort: bool = True) -> bool:
+    async def __is_updated_image_2(self, c: Client, obj: collection.ImageTransfer) -> bool:
         """ update image if blocks is fulls ver 2"""
         if obj.is_image_exist:
             is_activating: bool = False
             c.current_obj = obj
             try:
                 # TODO: copypast from __is_updated_image_3
                 await ReadAttributes(
@@ -753,15 +742,15 @@
             return True
 
     async def __is_updated_image_3(self, c: Client, obj: collection.ImageTransfer) -> bool:
         """ update image if blocks is fulls ver 3"""
         if obj.is_image_exist:
             # TODO: need common counter for exit from infinity loop
             c.current_obj = obj
-            self.previous_status: int | None = None
+            previous_status: i_t_status.ImageTransferStatus | None = None
             await ReadAttributes(
                 ln=obj.logical_name,
                 indexes=(6, 7)
             ).exchange(c)
             current_status = obj.image_transfer_status
             if obj.image_transfer_status in (i_t_status.TRANSFER_NOT_INITIATED, i_t_status.VERIFICATION_FAILED, i_t_status.ACTIVATION_FAILED) \
                     or len(obj.image_to_activate_info) == 0 \
@@ -786,18 +775,18 @@
                 except IndexError as e:  # Skip set block
                     await c.execute_method(obj.get_meth_descriptor(3))
                     c.log(logL.INFO, "Start Verify Transfer")
             while True:
                 c.log(logL.STATE, F"{obj.get_attr_element(6)}: {obj.image_transfer_status}")
                 try:
                     match current_status:
-                        case self.previous_status if self.previous_status == i_t_status.VERIFICATION_FAILED:
+                        case i_t_status.VERIFICATION_FAILED if current_status == previous_status:
                             c.set_error(Application.VERIFY_ERROR, 'Twice ERROR')
                             return False
-                        case self.previous_status if self.previous_status == i_t_status.TRANSFER_INITIATED:
+                        case i_t_status.TRANSFER_INITIATED if current_status == previous_status:
                             c.set_error(Application.VERIFY_ERROR, F"Expected Switch to Verification Initiated status, got Initiated")
                         case i_t_status.TRANSFER_NOT_INITIATED:
                             c.set_error(Application.ACTIVATION_ERROR, 'Got Not initiated status after call Initiation')
                         case i_t_status.TRANSFER_INITIATED:
                             while True:
                                 if c.is_stop_request:
                                     c.set_error(Transmit.ABORT, '')
@@ -884,15 +873,15 @@
                                 await c.execute_method(obj.get_meth_descriptor(1))
                                 c.log(logL.INFO, "Start initiate Image Transfer")
                                 # TODO: need wait clearing memory in device ~5 sec
                         case i_t_status.ACTIVATION_FAILED:
                             c.set_error(Application.ACTIVATION_ERROR, 'Ошибка активации...')
                             return False
                         case _: raise exc.DLMSException('Unknown image transfer status')
-                    self.previous_status = current_status
+                    previous_status = current_status
                 except Exception as e:
                     c.set_error(Transmit.EXECUTE_ERROR, F'{e.args[0]}')
                     return False
                 finally:
                     c.current_obj = None
                 time.sleep(1)  # TODO: tune it
                 await ReadAttribute(
```

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.8.7
+Version: 0.8.8
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.8.8/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.7/test/test_Client.py` & `DLMS_SPODES_client-0.8.8/test/test_Client.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         Client()
         c3 = Client()
         print(c1.id, c3.id, id_factory.value)
 
     def test_lowest_connect(self):
         t_server = TransactionServer(
             clients=[c := Client(media=AsyncSerial(
-                                port="COM13",
+                                port="COM3",
                                 inactivity_timeout=3))],
             tsk=task.Dummy()
         )
         t_server.start()
         while not t_server.results.is_complete():
             time.sleep(1)
         print(c.objects)
```

