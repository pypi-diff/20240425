# Comparing `tmp/RsCMPX_Gprf-5.0.90.tar.gz` & `tmp/RsCMPX_Gprf-5.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\RsCMPX_Gprf-5.0.90.tar", last modified: Thu Apr 18 11:06:37 2024, max compression
+gzip compressed data, was "dist\RsCMPX_Gprf-5.0.91.tar", last modified: Wed Apr 24 14:08:01 2024, max compression
```

## Comparing `RsCMPX_Gprf-5.0.90.tar` & `RsCMPX_Gprf-5.0.91.tar`

### file list

```diff
@@ -1,1073 +1,1131 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.841157 RsCMPX_Gprf-5.0.90/
--rw-rw-rw-   0        0        0     3349 2024-04-18 11:06:37.840160 RsCMPX_Gprf-5.0.90/PKG-INFO
--rw-rw-rw-   0        0        0     1770 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/README.rst
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.728681 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.751120 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/CustomFiles/
--rw-rw-rw-   0        0        0       90 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/CustomFiles/__init__.py
--rw-rw-rw-   0        0        0     3725 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/CustomFiles/events.py
--rw-rw-rw-   0        0        0     4916 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/CustomFiles/reliability.py
--rw-rw-rw-   0        0        0    21844 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/CustomFiles/utilities.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.757879 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.758844 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.758844 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.758844 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.768838 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/
--rw-rw-rw-   0        0        0     1338 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0     1372 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1363 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.778834 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.778834 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.788828 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/
--rw-rw-rw-   0        0        0     1219 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Rx.py
--rw-rw-rw-   0        0        0     1219 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Tx.py
--rw-rw-rw-   0        0        0     1243 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/__init__.py
--rw-rw-rw-   0        0        0     1044 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/__init__.py
--rw-rw-rw-   0        0        0     1289 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.792714 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.795705 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.798697 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.806675 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/
--rw-rw-rw-   0        0        0     2920 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/Zero.py
--rw-rw-rw-   0        0        0     1040 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/__init__.py
--rw-rw-rw-   0        0        0     1097 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/__init__.py
--rw-rw-rw-   0        0        0     1029 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.809964 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.812955 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.818940 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/
--rw-rw-rw-   0        0        0     2351 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1077 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.821932 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Cdma/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.825996 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.825996 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.825996 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.835990 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/
--rw-rw-rw-   0        0        0     1896 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py
--rw-rw-rw-   0        0        0     2676 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py
--rw-rw-rw-   0        0        0     1031 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.841288 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/
--rw-rw-rw-   0        0        0     2406 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1312 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.841288 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gsm/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.851278 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/
--rw-rw-rw-   0        0        0     2333 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.857662 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Lte/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.867662 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/
--rw-rw-rw-   0        0        0     2333 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.857662 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/LteDl/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.857662 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/
--rw-rw-rw-   0        0        0     2339 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.874693 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Niot/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.874693 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Niot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.874693 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrDl/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.884693 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.891198 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrMmw/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.891198 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/
--rw-rw-rw-   0        0        0     2339 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrMmw/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.891198 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrSub/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.908100 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/
--rw-rw-rw-   0        0        0     2339 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrSub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.916896 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.916896 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/
--rw-rw-rw-   0        0        0     1238 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/CorrectionTable.py
--rw-rw-rw-   0        0        0     1121 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0      813 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Reset.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.925450 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/
--rw-rw-rw-   0        0        0      926 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/Box.py
--rw-rw-rw-   0        0        0      990 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/__init__.py
--rw-rw-rw-   0        0        0     1236 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Rrhead.py
--rw-rw-rw-   0        0        0     1746 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.925450 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/
--rw-rw-rw-   0        0        0     1241 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/Connectors.py
--rw-rw-rw-   0        0        0     1496 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.935445 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Uwb/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.943496 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/
--rw-rw-rw-   0        0        0     2333 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Uwb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.946488 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wcdma/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.953470 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/
--rw-rw-rw-   0        0        0     2339 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wcdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.955464 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wlan/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.959979 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wlan/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.962970 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wpan/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.968955 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/
--rw-rw-rw-   0        0        0     2336 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wpan/__init__.py
--rw-rw-rw-   0        0        0     4439 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.971955 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.973942 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.976973 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.976973 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.976973 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.976973 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.986968 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/
--rw-rw-rw-   0        0        0     2556 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/Single.py
--rw-rw-rw-   0        0        0     1012 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/__init__.py
--rw-rw-rw-   0        0        0     3626 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/__init__.py
--rw-rw-rw-   0        0        0     2709 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/__init__.py
--rw-rw-rw-   0        0        0     1958 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/__init__.py
--rw-rw-rw-   0        0        0     2022 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.996964 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.006958 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/
--rw-rw-rw-   0        0        0     1377 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/IqFile.py
--rw-rw-rw-   0        0        0     3152 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/Sall.py
--rw-rw-rw-   0        0        0     4093 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/__init__.py
--rw-rw-rw-   0        0        0     1259 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Correction.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.016952 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/
--rw-rw-rw-   0        0        0     2461 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Attenuation.py
--rw-rw-rw-   0        0        0     2082 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py
--rw-rw-rw-   0        0        0     3239 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py
--rw-rw-rw-   0        0        0     8936 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.016952 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/
--rw-rw-rw-   0        0        0     6166 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py
--rw-rw-rw-   0        0        0    12393 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.024461 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/
--rw-rw-rw-   0        0        0     2570 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.040973 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/
--rw-rw-rw-   0        0        0     1907 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py
--rw-rw-rw-   0        0        0     1645 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py
--rw-rw-rw-   0        0        0     2459 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py
--rw-rw-rw-   0        0        0     1370 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.050966 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/
--rw-rw-rw-   0        0        0     2731 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py
--rw-rw-rw-   0        0        0     2675 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py
--rw-rw-rw-   0        0        0     2143 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py
--rw-rw-rw-   0        0        0     5475 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py
--rw-rw-rw-   0        0        0    14933 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.050966 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.060961 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/
--rw-rw-rw-   0        0        0     3789 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py
--rw-rw-rw-   0        0        0     3053 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py
--rw-rw-rw-   0        0        0     3118 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py
--rw-rw-rw-   0        0        0     2425 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py
--rw-rw-rw-   0        0        0     5646 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py
--rw-rw-rw-   0        0        0    10717 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.060961 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.070955 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/
--rw-rw-rw-   0        0        0     1969 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py
--rw-rw-rw-   0        0        0     1891 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py
--rw-rw-rw-   0        0        0     6078 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.080950 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.080950 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/
--rw-rw-rw-   0        0        0     3270 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py
--rw-rw-rw-   0        0        0     1904 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py
--rw-rw-rw-   0        0        0     3320 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.090955 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/
--rw-rw-rw-   0        0        0      900 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.100955 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/
--rw-rw-rw-   0        0        0     1469 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py
--rw-rw-rw-   0        0        0     1445 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py
--rw-rw-rw-   0        0        0     2945 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.128652 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/
--rw-rw-rw-   0        0        0     3755 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py
--rw-rw-rw-   0        0        0     3019 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py
--rw-rw-rw-   0        0        0     3464 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py
--rw-rw-rw-   0        0        0     3204 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py
--rw-rw-rw-   0        0        0     2828 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py
--rw-rw-rw-   0        0        0     3080 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py
--rw-rw-rw-   0        0        0     2419 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py
--rw-rw-rw-   0        0        0    12594 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.146416 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/
--rw-rw-rw-   0        0        0     1126 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.154634 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.160908 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/
--rw-rw-rw-   0        0        0     3261 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/Bandwidth.py
--rw-rw-rw-   0        0        0     1066 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/__init__.py
--rw-rw-rw-   0        0        0     2729 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.160908 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/
--rw-rw-rw-   0        0        0     3285 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/Bandwidth.py
--rw-rw-rw-   0        0        0     1051 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/__init__.py
--rw-rw-rw-   0        0        0     4452 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py
--rw-rw-rw-   0        0        0     1780 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/__init__.py
--rw-rw-rw-   0        0        0     3391 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py
--rw-rw-rw-   0        0        0     2509 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py
--rw-rw-rw-   0        0        0     3053 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py
--rw-rw-rw-   0        0        0     3387 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py
--rw-rw-rw-   0        0        0    10920 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.170902 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/
--rw-rw-rw-   0        0        0     1285 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/LrStart.py
--rw-rw-rw-   0        0        0     9793 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/__init__.py
--rw-rw-rw-   0        0        0     1431 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Scenario.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.170902 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.186342 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/
--rw-rw-rw-   0        0        0     2118 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Rbw.py
--rw-rw-rw-   0        0        0     2188 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Swt.py
--rw-rw-rw-   0        0        0     2196 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Vbw.py
--rw-rw-rw-   0        0        0     3640 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.191330 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/
--rw-rw-rw-   0        0        0     2365 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/Span.py
--rw-rw-rw-   0        0        0     4653 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.203484 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/
--rw-rw-rw-   0        0        0     3239 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Rbw.py
--rw-rw-rw-   0        0        0     2184 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Vbw.py
--rw-rw-rw-   0        0        0     3844 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/__init__.py
--rw-rw-rw-   0        0        0     5241 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/__init__.py
--rw-rw-rw-   0        0        0     3857 2024-04-18 11:06:28.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1315 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.217773 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.220765 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.222760 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.226916 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/
--rw-rw-rw-   0        0        0     1672 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py
--rw-rw-rw-   0        0        0     1706 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py
--rw-rw-rw-   0        0        0     1310 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py
--rw-rw-rw-   0        0        0     1055 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.240918 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/
--rw-rw-rw-   0        0        0     1162 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py
--rw-rw-rw-   0        0        0     1171 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py
--rw-rw-rw-   0        0        0     1180 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py
--rw-rw-rw-   0        0        0     1525 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py
--rw-rw-rw-   0        0        0     2171 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Edevice.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.250918 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Recall/
--rw-rw-rw-   0        0        0     1723 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py
--rw-rw-rw-   0        0        0     1032 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py
--rw-rw-rw-   0        0        0      891 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Reset.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.250918 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.257930 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.260969 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/
--rw-rw-rw-   0        0        0     1861 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py
--rw-rw-rw-   0        0        0     1825 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py
--rw-rw-rw-   0        0        0     1205 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py
--rw-rw-rw-   0        0        0     1817 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py
--rw-rw-rw-   0        0        0      990 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.270936 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.270936 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.280932 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/
--rw-rw-rw-   0        0        0     1729 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Rx.py
--rw-rw-rw-   0        0        0     1729 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Tx.py
--rw-rw-rw-   0        0        0     1200 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/__init__.py
--rw-rw-rw-   0        0        0     1006 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/__init__.py
--rw-rw-rw-   0        0        0      992 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.290926 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Save/
--rw-rw-rw-   0        0        0     1173 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Save/Partial.py
--rw-rw-rw-   0        0        0     1022 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Save/__init__.py
--rw-rw-rw-   0        0        0     1856 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Vse.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.300920 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z310/
--rw-rw-rw-   0        0        0     1323 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z310/Attenuation.py
--rw-rw-rw-   0        0        0     1054 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z310/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.300920 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z320/
--rw-rw-rw-   0        0        0     1323 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z320/Attenuation.py
--rw-rw-rw-   0        0        0     1054 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z320/__init__.py
--rw-rw-rw-   0        0        0     3344 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.307927 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.307927 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.324433 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/
--rw-rw-rw-   0        0        0     1689 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Rx.py
--rw-rw-rw-   0        0        0     1689 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Tx.py
--rw-rw-rw-   0        0        0     1223 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.339768 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/
--rw-rw-rw-   0        0        0     1828 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Rx.py
--rw-rw-rw-   0        0        0     1828 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Tx.py
--rw-rw-rw-   0        0        0     1243 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1914 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Direction.py
--rw-rw-rw-   0        0        0     2359 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Info.py
--rw-rw-rw-   0        0        0     1847 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/__init__.py
--rw-rw-rw-   0        0        0     1044 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/__init__.py
--rw-rw-rw-   0        0        0     1542 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.344241 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.348230 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.351222 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.361103 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/
--rw-rw-rw-   0        0        0     1327 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0     1381 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1363 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.361103 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/Tenvironment/
--rw-rw-rw-   0        0        0     1405 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py
--rw-rw-rw-   0        0        0     1044 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.361103 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.371096 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.371096 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/
--rw-rw-rw-   0        0        0     1263 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py
--rw-rw-rw-   0        0        0     1056 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py
--rw-rw-rw-   0        0        0     1027 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.383312 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.386303 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.388297 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.390292 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.393283 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.400468 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/
--rw-rw-rw-   0        0        0     2337 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py
--rw-rw-rw-   0        0        0     2757 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.405454 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/
--rw-rw-rw-   0        0        0     2325 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py
--rw-rw-rw-   0        0        0     2740 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/__init__.py
--rw-rw-rw-   0        0        0     1216 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.407449 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.409481 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/
--rw-rw-rw-   0        0        0     2337 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/FilterPy.py
--rw-rw-rw-   0        0        0     2757 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.409481 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/
--rw-rw-rw-   0        0        0     2325 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/FilterPy.py
--rw-rw-rw-   0        0        0     2740 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/__init__.py
--rw-rw-rw-   0        0        0     1216 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/__init__.py
--rw-rw-rw-   0        0        0     1238 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py
--rw-rw-rw-   0        0        0     1025 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.419476 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/
--rw-rw-rw-   0        0        0     1981 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/Logging.py
--rw-rw-rw-   0        0        0     1024 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/__init__.py
--rw-rw-rw-   0        0        0     1229 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py
--rw-rw-rw-   0        0        0     1038 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.419476 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.429472 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/
--rw-rw-rw-   0        0        0     2255 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/State.py
--rw-rw-rw-   0        0        0     1011 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/__init__.py
--rw-rw-rw-   0        0        0     1009 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.429472 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Generic/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.439467 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/
--rw-rw-rw-   0        0        0     1191 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/Dapi.py
--rw-rw-rw-   0        0        0     1033 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1067 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Generic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.439467 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.461043 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/
--rw-rw-rw-   0        0        0     1231 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Correction.py
--rw-rw-rw-   0        0        0      834 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfProperty.py
--rw-rw-rw-   0        0        0     1314 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSettings.py
--rw-rw-rw-   0        0        0     1311 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSetttings.py
--rw-rw-rw-   0        0        0     1211 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Rms.py
--rw-rw-rw-   0        0        0     2062 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Snumber.py
--rw-rw-rw-   0        0        0     3120 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.461043 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.470978 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/
--rw-rw-rw-   0        0        0     1320 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/Rnames.py
--rw-rw-rw-   0        0        0     2409 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.491277 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.491277 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/
--rw-rw-rw-   0        0        0     2357 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/Bandwidth.py
--rw-rw-rw-   0        0        0     1062 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/__init__.py
--rw-rw-rw-   0        0        0      865 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Franges.py
--rw-rw-rw-   0        0        0     2308 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Frequency.py
--rw-rw-rw-   0        0        0     2252 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Fspan.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.501277 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/
--rw-rw-rw-   0        0        0     2339 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/Bandwidth.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.507784 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.517783 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/
--rw-rw-rw-   0        0        0     2430 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/Bandwidth.py
--rw-rw-rw-   0        0        0     1064 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.524621 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/
--rw-rw-rw-   0        0        0     2412 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/Bandwidth.py
--rw-rw-rw-   0        0        0     1049 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/__init__.py
--rw-rw-rw-   0        0        0     2353 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Samples.py
--rw-rw-rw-   0        0        0     1536 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.524621 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/
--rw-rw-rw-   0        0        0     2321 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/Iranges.py
--rw-rw-rw-   0        0        0     1036 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/__init__.py
--rw-rw-rw-   0        0        0     1342 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/LoFrequency.py
--rw-rw-rw-   0        0        0     2280 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/NbLevel.py
--rw-rw-rw-   0        0        0     2302 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/SymbolRate.py
--rw-rw-rw-   0        0        0     4160 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/__init__.py
--rw-rw-rw-   0        0        0     2046 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Snumber.py
--rw-rw-rw-   0        0        0     3133 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1313 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.524621 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Meas/
--rw-rw-rw-   0        0        0     1125 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Meas/Scpi.py
--rw-rw-rw-   0        0        0      996 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Meas/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.538484 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.549136 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/
--rw-rw-rw-   0        0        0     1301 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Generator.py
--rw-rw-rw-   0        0        0     1319 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Measurement.py
--rw-rw-rw-   0        0        0     1314 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.554122 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/
--rw-rw-rw-   0        0        0     1325 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/Measurement.py
--rw-rw-rw-   0        0        0     1059 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.561267 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/
--rw-rw-rw-   0        0        0     1313 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/Measurement.py
--rw-rw-rw-   0        0        0     1049 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/__init__.py
--rw-rw-rw-   0        0        0     1441 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.561267 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.561267 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.571261 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/
--rw-rw-rw-   0        0        0     2310 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/Output.py
--rw-rw-rw-   0        0        0     1021 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/__init__.py
--rw-rw-rw-   0        0        0     1001 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/__init__.py
--rw-rw-rw-   0        0        0     1003 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/__init__.py
--rw-rw-rw-   0        0        0     2693 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.571261 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.571261 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.581802 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.586788 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/
--rw-rw-rw-   0        0        0     2115 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/All.py
--rw-rw-rw-   0        0        0     2756 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/__init__.py
--rw-rw-rw-   0        0        0     3733 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.589779 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.594766 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/
--rw-rw-rw-   0        0        0     2116 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/All.py
--rw-rw-rw-   0        0        0     2757 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/__init__.py
--rw-rw-rw-   0        0        0     6124 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.605932 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/
--rw-rw-rw-   0        0        0     1845 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Icomponent.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.609964 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/
--rw-rw-rw-   0        0        0     2613 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Average.py
--rw-rw-rw-   0        0        0     2613 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Current.py
--rw-rw-rw-   0        0        0     1273 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.619959 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/
--rw-rw-rw-   0        0        0     2034 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Average.py
--rw-rw-rw-   0        0        0     2034 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Current.py
--rw-rw-rw-   0        0        0     2034 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Maximum.py
--rw-rw-rw-   0        0        0     2034 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Minimum.py
--rw-rw-rw-   0        0        0     1761 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/__init__.py
--rw-rw-rw-   0        0        0     1845 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Qcomponent.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.629954 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/
--rw-rw-rw-   0        0        0     2121 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/All.py
--rw-rw-rw-   0        0        0     2762 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/__init__.py
--rw-rw-rw-   0        0        0     4744 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.640904 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/
--rw-rw-rw-   0        0        0     1553 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Bin.py
--rw-rw-rw-   0        0        0      944 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Reliability.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.650905 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/
--rw-rw-rw-   0        0        0     2118 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/All.py
--rw-rw-rw-   0        0        0     2759 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/__init__.py
--rw-rw-rw-   0        0        0      920 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/SymbolRate.py
--rw-rw-rw-   0        0        0     1656 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Talignment.py
--rw-rw-rw-   0        0        0     7279 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.671424 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/
--rw-rw-rw-   0        0        0     1792 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/FreqError.py
--rw-rw-rw-   0        0        0     1731 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Icomponent.py
--rw-rw-rw-   0        0        0     1708 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Level.py
--rw-rw-rw-   0        0        0     3029 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/OfError.py
--rw-rw-rw-   0        0        0     1708 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Phase.py
--rw-rw-rw-   0        0        0     1731 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Qcomponent.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.671424 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/
--rw-rw-rw-   0        0        0     2110 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/All.py
--rw-rw-rw-   0        0        0     2751 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/__init__.py
--rw-rw-rw-   0        0        0     5210 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.681420 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.691007 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/
--rw-rw-rw-   0        0        0     4990 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/Power.py
--rw-rw-rw-   0        0        0     1855 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.691007 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/
--rw-rw-rw-   0        0        0     2100 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/All.py
--rw-rw-rw-   0        0        0     2741 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/__init__.py
--rw-rw-rw-   0        0        0     3899 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.701006 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/
--rw-rw-rw-   0        0        0     1254 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.708013 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/
--rw-rw-rw-   0        0        0     1062 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py
--rw-rw-rw-   0        0        0     1062 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py
--rw-rw-rw-   0        0        0     1062 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py
--rw-rw-rw-   0        0        0     1097 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py
--rw-rw-rw-   0        0        0     1686 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.718013 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/
--rw-rw-rw-   0        0        0     2103 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py
--rw-rw-rw-   0        0        0     2744 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py
--rw-rw-rw-   0        0        0     2659 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.724264 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/
--rw-rw-rw-   0        0        0     1152 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.734266 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/
--rw-rw-rw-   0        0        0     1620 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py
--rw-rw-rw-   0        0        0     4648 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.741272 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/
--rw-rw-rw-   0        0        0     1741 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Power.py
--rw-rw-rw-   0        0        0     1340 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Probability.py
--rw-rw-rw-   0        0        0     1485 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Sample.py
--rw-rw-rw-   0        0        0     2322 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.764045 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/
--rw-rw-rw-   0        0        0     1656 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Maximum.py
--rw-rw-rw-   0        0        0     1656 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Minimum.py
--rw-rw-rw-   0        0        0     1620 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Rms.py
--rw-rw-rw-   0        0        0     5136 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/__init__.py
--rw-rw-rw-   0        0        0     1170 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.770456 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/
--rw-rw-rw-   0        0        0     1518 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/Bin.py
--rw-rw-rw-   0        0        0     3002 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/__init__.py
--rw-rw-rw-   0        0        0     1998 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.785531 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/
--rw-rw-rw-   0        0        0     4420 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Average.py
--rw-rw-rw-   0        0        0     4420 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Current.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.792262 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/
--rw-rw-rw-   0        0        0     4498 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/Current.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.797248 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/
--rw-rw-rw-   0        0        0     4498 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/Current.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.806224 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/
--rw-rw-rw-   0        0        0     4471 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Maximum.py
--rw-rw-rw-   0        0        0     4471 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Minimum.py
--rw-rw-rw-   0        0        0     1270 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/__init__.py
--rw-rw-rw-   0        0        0     4462 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/StandardDev.py
--rw-rw-rw-   0        0        0     2263 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.814523 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/
--rw-rw-rw-   0        0        0     4111 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Current.py
--rw-rw-rw-   0        0        0     1656 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Maximum.py
--rw-rw-rw-   0        0        0     1283 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.823500 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/
--rw-rw-rw-   0        0        0     4111 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Current.py
--rw-rw-rw-   0        0        0     1656 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Minimum.py
--rw-rw-rw-   0        0        0     1283 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.826525 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/
--rw-rw-rw-   0        0        0     4084 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Maximum.py
--rw-rw-rw-   0        0        0     4084 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Minimum.py
--rw-rw-rw-   0        0        0     1268 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.836520 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/
--rw-rw-rw-   0        0        0     1676 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/Current.py
--rw-rw-rw-   0        0        0     4730 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.836520 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/
--rw-rw-rw-   0        0        0     2103 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/All.py
--rw-rw-rw-   0        0        0     2744 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/__init__.py
--rw-rw-rw-   0        0        0     6839 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.846516 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.862289 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Average.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Current.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Maximum.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Minimum.py
--rw-rw-rw-   0        0        0     1771 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.862289 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/
--rw-rw-rw-   0        0        0     2350 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/Npeak.py
--rw-rw-rw-   0        0        0     1855 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.872282 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Average.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Current.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Maximum.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Minimum.py
--rw-rw-rw-   0        0        0     1771 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.891281 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Average.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Current.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Maximum.py
--rw-rw-rw-   0        0        0     1650 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Minimum.py
--rw-rw-rw-   0        0        0     1771 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.891281 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/
--rw-rw-rw-   0        0        0     2059 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Npeak.py
--rw-rw-rw-   0        0        0     2059 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Speak.py
--rw-rw-rw-   0        0        0     1291 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.907544 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/
--rw-rw-rw-   0        0        0     1626 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Average.py
--rw-rw-rw-   0        0        0     1626 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Current.py
--rw-rw-rw-   0        0        0     1626 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Maximum.py
--rw-rw-rw-   0        0        0     1626 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Minimum.py
--rw-rw-rw-   0        0        0     1751 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.924551 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/
--rw-rw-rw-   0        0        0     1644 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Average.py
--rw-rw-rw-   0        0        0     1644 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Current.py
--rw-rw-rw-   0        0        0     1644 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Maximum.py
--rw-rw-rw-   0        0        0     1644 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Minimum.py
--rw-rw-rw-   0        0        0     1766 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.924551 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/
--rw-rw-rw-   0        0        0     1804 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/All.py
--rw-rw-rw-   0        0        0     2368 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/__init__.py
--rw-rw-rw-   0        0        0     3902 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/__init__.py
--rw-rw-rw-   0        0        0     3066 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.924551 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.934550 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.934550 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.941189 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/
--rw-rw-rw-   0        0        0     1329 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0     1363 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1363 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/__init__.py
--rw-rw-rw-   0        0        0     1020 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.941189 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.954532 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.958777 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.966026 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/
--rw-rw-rw-   0        0        0     1293 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0     1327 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1363 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1121 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/__init__.py
--rw-rw-rw-   0        0        0     1062 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.966026 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.974739 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.981721 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/
--rw-rw-rw-   0        0        0     1237 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Rx.py
--rw-rw-rw-   0        0        0     1237 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Tx.py
--rw-rw-rw-   0        0        0     1243 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1091 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/__init__.py
--rw-rw-rw-   0        0        0     1044 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/__init__.py
--rw-rw-rw-   0        0        0     1304 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.982828 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.982828 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.982828 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.992536 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/
--rw-rw-rw-   0        0        0     1633 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/Current.py
--rw-rw-rw-   0        0        0     1029 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/__init__.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/__init__.py
--rw-rw-rw-   0        0        0     1009 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.992536 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:36.992536 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Bluetooth/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.002531 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/
--rw-rw-rw-   0        0        0     1670 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1077 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Bluetooth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.011015 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Cdma/
--rw-rw-rw-   0        0        0     1250 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Cdma/Measurement.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Cdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.013009 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.017996 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/
--rw-rw-rw-   0        0        0     1449 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/RfSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.022982 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/
--rw-rw-rw-   0        0        0     2377 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/Group.py
--rw-rw-rw-   0        0        0     2525 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/__init__.py
--rw-rw-rw-   0        0        0     1299 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.030502 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/
--rw-rw-rw-   0        0        0     1441 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/RfSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.036487 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/
--rw-rw-rw-   0        0        0      888 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/Catalog.py
--rw-rw-rw-   0        0        0     1044 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/__init__.py
--rw-rw-rw-   0        0        0     3754 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1561 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1312 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.038483 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gsm/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.043503 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/
--rw-rw-rw-   0        0        0     1616 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gsm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.043503 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Lte/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.053497 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/
--rw-rw-rw-   0        0        0     1616 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Lte/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.043503 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/LteDl/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.043503 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/
--rw-rw-rw-   0        0        0     1634 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/LteDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.053497 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Niot/
--rw-rw-rw-   0        0        0     1250 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Niot/Measurement.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Niot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.063493 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrDl/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.063493 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/
--rw-rw-rw-   0        0        0     1625 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.073488 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrMmw/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.073488 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/
--rw-rw-rw-   0        0        0     1634 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrMmw/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.073488 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrSub/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.083482 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/
--rw-rw-rw-   0        0        0     1634 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrSub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.083482 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Uwb/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.090991 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/
--rw-rw-rw-   0        0        0     1616 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Uwb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.090991 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wcdma/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.090991 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/
--rw-rw-rw-   0        0        0     1634 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wcdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.100989 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wlan/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.107997 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/
--rw-rw-rw-   0        0        0     1625 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wlan/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.107997 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wpan/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.107997 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/
--rw-rw-rw-   0        0        0     1625 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py
--rw-rw-rw-   0        0        0     1041 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wpan/__init__.py
--rw-rw-rw-   0        0        0     3909 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.107997 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.117995 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.117995 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.124500 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/
--rw-rw-rw-   0        0        0     1813 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py
--rw-rw-rw-   0        0        0     1049 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/__init__.py
--rw-rw-rw-   0        0        0      999 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.124500 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.124500 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.141006 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.159936 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/
--rw-rw-rw-   0        0        0     4136 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.165898 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/
--rw-rw-rw-   0        0        0     2565 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/Delays.py
--rw-rw-rw-   0        0        0     1028 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/__init__.py
--rw-rw-rw-   0        0        0     3268 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Msegment.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.168925 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/
--rw-rw-rw-   0        0        0     2372 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/Range.py
--rw-rw-rw-   0        0        0     1536 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/__init__.py
--rw-rw-rw-   0        0        0     2323 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Segments.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.175990 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/
--rw-rw-rw-   0        0        0     1253 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/Clist.py
--rw-rw-rw-   0        0        0     3222 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/__init__.py
--rw-rw-rw-   0        0        0     9112 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.185986 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/
--rw-rw-rw-   0        0        0     2628 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Level.py
--rw-rw-rw-   0        0        0     3652 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Ofrequency.py
--rw-rw-rw-   0        0        0     2150 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/__init__.py
--rw-rw-rw-   0        0        0     3390 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.226688 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/
--rw-rw-rw-   0        0        0     2475 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dgain.py
--rw-rw-rw-   0        0        0     2448 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dtime.py
--rw-rw-rw-   0        0        0     1225 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Esingle.py
--rw-rw-rw-   0        0        0     3782 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Fill.py
--rw-rw-rw-   0        0        0     2507 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Frequency.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.226688 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/
--rw-rw-rw-   0        0        0     1811 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/Enabling.py
--rw-rw-rw-   0        0        0     2412 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/__init__.py
--rw-rw-rw-   0        0        0     2531 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Irepetition.py
--rw-rw-rw-   0        0        0     2539 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Modulation.py
--rw-rw-rw-   0        0        0     2529 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Reenabling.py
--rw-rw-rw-   0        0        0     2607 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/RfLevel.py
--rw-rw-rw-   0        0        0     1207 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Rlist.py
--rw-rw-rw-   0        0        0     1207 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Slist.py
--rw-rw-rw-   0        0        0     2189 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Sstop.py
--rw-rw-rw-   0        0        0    10413 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/__init__.py
--rw-rw-rw-   0        0        0     2717 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py
--rw-rw-rw-   0        0        0     5682 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.236684 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.283906 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/
--rw-rw-rw-   0        0        0     1635 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Check.py
--rw-rw-rw-   0        0        0     1762 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/CrcProtect.py
--rw-rw-rw-   0        0        0     1364 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Download.py
--rw-rw-rw-   0        0        0     1515 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Duration.py
--rw-rw-rw-   0        0        0     1544 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Paratio.py
--rw-rw-rw-   0        0        0     1627 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Path.py
--rw-rw-rw-   0        0        0     1518 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Poffset.py
--rw-rw-rw-   0        0        0     1694 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Reliability.py
--rw-rw-rw-   0        0        0     1733 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Rmessage.py
--rw-rw-rw-   0        0        0     1589 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Roption.py
--rw-rw-rw-   0        0        0     1510 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Samples.py
--rw-rw-rw-   0        0        0     1525 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/SymbolRate.py
--rw-rw-rw-   0        0        0     1591 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Waveform.py
--rw-rw-rw-   0        0        0     8460 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.283906 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/
--rw-rw-rw-   0        0        0     3565 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/Ofrequency.py
--rw-rw-rw-   0        0        0     1985 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.307920 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/
--rw-rw-rw-   0        0        0     2846 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Acycles.py
--rw-rw-rw-   0        0        0     2850 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dgain.py
--rw-rw-rw-   0        0        0     2810 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dtime.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.324692 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/
--rw-rw-rw-   0        0        0     1418 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Call.py
--rw-rw-rw-   0        0        0     1136 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Insert.py
--rw-rw-rw-   0        0        0     1126 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mdown.py
--rw-rw-rw-   0        0        0     1110 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mup.py
--rw-rw-rw-   0        0        0     2484 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.341197 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/
--rw-rw-rw-   0        0        0     1519 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Apply.py
--rw-rw-rw-   0        0        0     3570 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Dgain.py
--rw-rw-rw-   0        0        0     3758 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Frequency.py
--rw-rw-rw-   0        0        0     3507 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Lrms.py
--rw-rw-rw-   0        0        0     3555 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/__init__.py
--rw-rw-rw-   0        0        0     3163 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Frequency.py
--rw-rw-rw-   0        0        0     3702 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Itransition.py
--rw-rw-rw-   0        0        0     5060 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lincrement.py
--rw-rw-rw-   0        0        0     2772 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lrms.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.355088 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.365350 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/
--rw-rw-rw-   0        0        0     1312 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Cw.py
--rw-rw-rw-   0        0        0     1339 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Dtone.py
--rw-rw-rw-   0        0        0     1321 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Off.py
--rw-rw-rw-   0        0        0     5147 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Catalog.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.365350 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/
--rw-rw-rw-   0        0        0     2186 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/All.py
--rw-rw-rw-   0        0        0     2969 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/__init__.py
--rw-rw-rw-   0        0        0     2097 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Range.py
--rw-rw-rw-   0        0        0     3415 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.376247 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.376247 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.376247 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.386243 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/
--rw-rw-rw-   0        0        0     3080 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/Single.py
--rw-rw-rw-   0        0        0     1016 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/__init__.py
--rw-rw-rw-   0        0        0     4245 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/__init__.py
--rw-rw-rw-   0        0        0     3224 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/__init__.py
--rw-rw-rw-   0        0        0     1017 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/__init__.py
--rw-rw-rw-   0        0        0     1538 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/SymbolRate.py
--rw-rw-rw-   0        0        0     1519 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Ttime.py
--rw-rw-rw-   0        0        0     5939 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.386243 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.386243 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/
--rw-rw-rw-   0        0        0     2880 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/All.py
--rw-rw-rw-   0        0        0     3365 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/__init__.py
--rw-rw-rw-   0        0        0     1028 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/__init__.py
--rw-rw-rw-   0        0        0     2786 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Reliability.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.404148 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/
--rw-rw-rw-   0        0        0     2299 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/Spath.py
--rw-rw-rw-   0        0        0     1040 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/__init__.py
--rw-rw-rw-   0        0        0     1298 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Rmarker.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.408138 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/
--rw-rw-rw-   0        0        0     2146 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/All.py
--rw-rw-rw-   0        0        0     2133 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/__init__.py
--rw-rw-rw-   0        0        0     1343 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Tdd.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.411130 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.416307 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/
--rw-rw-rw-   0        0        0     2592 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/All.py
--rw-rw-rw-   0        0        0     2470 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/__init__.py
--rw-rw-rw-   0        0        0     1864 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/__init__.py
--rw-rw-rw-   0        0        0     7520 2024-04-18 11:06:27.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.421294 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/
--rw-rw-rw-   0        0        0     2088 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/All.py
--rw-rw-rw-   0        0        0     1983 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/__init__.py
--rw-rw-rw-   0        0        0     3944 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py
--rw-rw-rw-   0        0        0     1038 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py
--rw-rw-rw-   0        0        0     1006 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.423288 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.426384 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.426384 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.440885 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/
--rw-rw-rw-   0        0        0     1256 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Globale.py
--rw-rw-rw-   0        0        0     1309 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Tenvironment.py
--rw-rw-rw-   0        0        0     1303 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/__init__.py
--rw-rw-rw-   0        0        0      805 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Globale.py
--rw-rw-rw-   0        0        0      839 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Tenvironment.py
--rw-rw-rw-   0        0        0     1573 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/__init__.py
--rw-rw-rw-   0        0        0     1119 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.440885 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Date/
--rw-rw-rw-   0        0        0     1988 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Date/Local.py
--rw-rw-rw-   0        0        0     1004 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Date/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.450884 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Time/
--rw-rw-rw-   0        0        0     2020 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Time/Local.py
--rw-rw-rw-   0        0        0     2496 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Time/__init__.py
--rw-rw-rw-   0        0        0     1500 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.457898 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Tenvironment/
--rw-rw-rw-   0        0        0      789 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Tenvironment/Spath.py
--rw-rw-rw-   0        0        0     1042 2024-04-18 11:06:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Tenvironment/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.457898 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.464963 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.464963 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.474608 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/
--rw-rw-rw-   0        0        0      899 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/Catalog.py
--rw-rw-rw-   0        0        0     1932 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.474608 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/
--rw-rw-rw-   0        0        0      890 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/Catalog.py
--rw-rw-rw-   0        0        0     1899 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.484607 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/
--rw-rw-rw-   0        0        0      893 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/Catalog.py
--rw-rw-rw-   0        0        0     1910 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.491113 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      912 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1973 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1741 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1077 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.491113 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.491113 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.501112 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.507771 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.507771 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.507771 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.517771 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/
--rw-rw-rw-   0        0        0     1265 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py
--rw-rw-rw-   0        0        0     1036 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.524276 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.524276 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/
--rw-rw-rw-   0        0        0     1321 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py
--rw-rw-rw-   0        0        0     1038 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py
--rw-rw-rw-   0        0        0     2034 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py
--rw-rw-rw-   0        0        0     4485 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.524276 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.534275 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/
--rw-rw-rw-   0        0        0     1383 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py
--rw-rw-rw-   0        0        0     1036 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py
--rw-rw-rw-   0        0        0     2080 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py
--rw-rw-rw-   0        0        0     2270 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.551347 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.557860 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/
--rw-rw-rw-   0        0        0     2344 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py
--rw-rw-rw-   0        0        0     7702 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py
--rw-rw-rw-   0        0        0     8887 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder.py
--rw-rw-rw-   0        0        0     7158 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.557860 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.569807 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/
--rw-rw-rw-   0        0        0     2941 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py
--rw-rw-rw-   0        0        0     1078 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py
--rw-rw-rw-   0        0        0     7843 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py
--rw-rw-rw-   0        0        0     4768 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py
--rw-rw-rw-   0        0        0     2074 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1313 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.571936 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.576773 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.581336 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      894 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1937 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.581336 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.592804 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.610179 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      894 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1937 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.615165 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/
--rw-rw-rw-   0        0        0      878 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1885 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.620152 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/
--rw-rw-rw-   0        0        0      872 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/Catalog.py
--rw-rw-rw-   0        0        0     1863 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.581336 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.592804 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.592804 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      900 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1949 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.623144 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.625459 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.630446 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.636429 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/
--rw-rw-rw-   0        0        0      881 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1891 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/__init__.py
--rw-rw-rw-   0        0        0     1301 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.638425 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.641416 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.643447 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.643447 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.643447 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.659214 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      900 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1949 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.664727 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/
--rw-rw-rw-   0        0        0      884 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1897 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/__init__.py
--rw-rw-rw-   0        0        0     1301 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.664727 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.664727 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.674234 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      900 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1949 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.684234 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/
--rw-rw-rw-   0        0        0      884 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1897 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.684234 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/
--rw-rw-rw-   0        0        0      878 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/Catalog.py
--rw-rw-rw-   0        0        0     1875 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/__init__.py
--rw-rw-rw-   0        0        0     1513 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1057 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.684234 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.691241 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.691241 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      894 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1937 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1047 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.701240 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.701240 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.707745 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      900 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1949 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.707745 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/
--rw-rw-rw-   0        0        0      899 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/Catalog.py
--rw-rw-rw-   0        0        0     1952 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.717745 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/
--rw-rw-rw-   0        0        0      887 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/Catalog.py
--rw-rw-rw-   0        0        0     1908 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.724234 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/
--rw-rw-rw-   0        0        0      884 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/Catalog.py
--rw-rw-rw-   0        0        0     1897 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.724234 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/
--rw-rw-rw-   0        0        0      878 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/Catalog.py
--rw-rw-rw-   0        0        0     1875 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/__init__.py
--rw-rw-rw-   0        0        0     2018 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1058 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.734233 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.734233 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.741241 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.741241 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.741241 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.751239 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/
--rw-rw-rw-   0        0        0      897 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/Catalog.py
--rw-rw-rw-   0        0        0     1943 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/__init__.py
--rw-rw-rw-   0        0        0     1073 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/__init__.py
--rw-rw-rw-   0        0        0     1052 2024-04-18 11:06:30.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/__init__.py
--rw-rw-rw-   0        0        0     3919 2024-04-18 11:06:29.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/__init__.py
--rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:37.838166 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/
--rw-rw-rw-   0        0        0      586 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py
--rw-rw-rw-   0        0        0     4165 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgSingle.py
--rw-rw-rw-   0        0        0     1116 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgSingleList.py
--rw-rw-rw-   0        0        0     1145 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py
--rw-rw-rw-   0        0        0     9097 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgStringComposer.py
--rw-rw-rw-   0        0        0     5751 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgStruct.py
--rw-rw-rw-   0        0        0     3439 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgStructList.py
--rw-rw-rw-   0        0        0     2546 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgStructStringParser.py
--rw-rw-rw-   0        0        0     5238 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/CommandsGroup.py
--rw-rw-rw-   0        0        0    25419 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Conversions.py
--rw-rw-rw-   0        0        0     3775 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ConverterFromScpiString.py
--rw-rw-rw-   0        0        0     4768 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ConverterToScpiString.py
--rw-rw-rw-   0        0        0    14213 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Core.py
--rw-rw-rw-   0        0        0     1386 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/GlobalData.py
--rw-rw-rw-   0        0        0    60862 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Instrument.py
--rw-rw-rw-   0        0        0     4785 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/InstrumentErrors.py
--rw-rw-rw-   0        0        0     2225 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/InstrumentOptions.py
--rw-rw-rw-   0        0        0    16156 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/InstrumentSettings.py
--rw-rw-rw-   0        0        0     3518 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/InternalLinker.py
--rw-rw-rw-   0        0        0     4390 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/IoTransferEventArgs.py
--rw-rw-rw-   0        0        0      387 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Properties.py
--rw-rw-rw-   0        0        0     4289 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/RepeatedCapability.py
--rw-rw-rw-   0        0        0     4745 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ScpiEnums.py
--rw-rw-rw-   0        0        0    35525 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ScpiLogger.py
--rw-rw-rw-   0        0        0     5098 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/StreamReader.py
--rw-rw-rw-   0        0        0     5856 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/StreamWriter.py
--rw-rw-rw-   0        0        0     1114 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/StructBase.py
--rw-rw-rw-   0        0        0     3608 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Types.py
--rw-rw-rw-   0        0        0     5498 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Utilities.py
--rw-rw-rw-   0        0        0     5716 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py
--rw-rw-rw-   0        0        0    51976 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/VisaSession.py
--rw-rw-rw-   0        0        0     7512 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/VisaSessionSim.py
--rw-rw-rw-   0        0        0       29 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/__init__.py
--rw-rw-rw-   0        0        0    15874 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/RsCMPX_Gprf.py
--rw-rw-rw-   0        0        0      899 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/__init__.py
--rw-rw-rw-   0        0        0    11017 2024-04-18 11:06:26.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/enums.py
--rw-rw-rw-   0        0        0     2748 2024-04-18 11:06:24.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/repcap.py
-drwxrwxrwx   0        0        0        0 2024-04-18 11:06:35.738678 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf.egg-info/
--rw-rw-rw-   0        0        0     3349 2024-04-18 11:06:34.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    49994 2024-04-18 11:06:35.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 11:06:34.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-18 11:06:34.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-18 11:06:34.000000 RsCMPX_Gprf-5.0.90/RsCMPX_Gprf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 11:06:37.842157 RsCMPX_Gprf-5.0.90/setup.cfg
--rw-rw-rw-   0        0        0     1480 2024-04-18 11:06:32.000000 RsCMPX_Gprf-5.0.90/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.938099 RsCMPX_Gprf-5.0.91/
+-rw-rw-rw-   0        0        0     3474 2024-04-24 14:08:01.937101 RsCMPX_Gprf-5.0.91/PKG-INFO
+-rw-rw-rw-   0        0        0     1868 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/README.rst
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.397885 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.423816 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/
+-rw-rw-rw-   0        0        0       90 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/__init__.py
+-rw-rw-rw-   0        0        0     3725 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/events.py
+-rw-rw-rw-   0        0        0     4916 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/reliability.py
+-rw-rw-rw-   0        0        0    21844 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/utilities.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.426807 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.428803 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.431795 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.433789 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.441768 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/
+-rw-rw-rw-   0        0        0     1338 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0     1372 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.443764 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.446754 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.453736 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/
+-rw-rw-rw-   0        0        0     1219 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Rx.py
+-rw-rw-rw-   0        0        0     1219 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Tx.py
+-rw-rw-rw-   0        0        0     1243 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/__init__.py
+-rw-rw-rw-   0        0        0     1289 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.455731 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.459720 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.461714 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.466701 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/
+-rw-rw-rw-   0        0        0     2920 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/Zero.py
+-rw-rw-rw-   0        0        0     1040 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/__init__.py
+-rw-rw-rw-   0        0        0     1097 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/__init__.py
+-rw-rw-rw-   0        0        0     1029 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.469693 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.472685 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.478670 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/
+-rw-rw-rw-   0        0        0     2351 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1077 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.480664 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.486649 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.489640 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.492632 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.497618 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/
+-rw-rw-rw-   0        0        0     1896 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py
+-rw-rw-rw-   0        0        0     2676 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1031 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.505598 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/
+-rw-rw-rw-   0        0        0      891 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Ploss.py
+-rw-rw-rw-   0        0        0     2406 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1269 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1312 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.508590 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.513576 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/
+-rw-rw-rw-   0        0        0     2333 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.515571 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.530530 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/
+-rw-rw-rw-   0        0        0     2333 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.518563 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.524546 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/
+-rw-rw-rw-   0        0        0     2339 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.532525 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.540504 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.544494 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.552473 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.555465 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.560451 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/
+-rw-rw-rw-   0        0        0     2339 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.563444 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.570425 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/
+-rw-rw-rw-   0        0        0     2339 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.578403 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.589374 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/
+-rw-rw-rw-   0        0        0     1238 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/CorrectionTable.py
+-rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0      813 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Reset.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.605331 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/
+-rw-rw-rw-   0        0        0      926 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/Box.py
+-rw-rw-rw-   0        0        0      990 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/__init__.py
+-rw-rw-rw-   0        0        0     1236 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rrhead.py
+-rw-rw-rw-   0        0        0     2122 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.611314 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/
+-rw-rw-rw-   0        0        0     1241 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/Connectors.py
+-rw-rw-rw-   0        0        0     1496 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.614307 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.621289 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/
+-rw-rw-rw-   0        0        0     2333 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.624280 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.629267 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/
+-rw-rw-rw-   0        0        0     2339 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.632260 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.638243 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.641235 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.647220 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/
+-rw-rw-rw-   0        0        0     2336 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/__init__.py
+-rw-rw-rw-   0        0        0     4439 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.650211 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.653203 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.656195 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.659187 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.662179 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.665171 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.671155 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/
+-rw-rw-rw-   0        0        0     2556 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/Single.py
+-rw-rw-rw-   0        0        0     1012 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/__init__.py
+-rw-rw-rw-   0        0        0     3626 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/__init__.py
+-rw-rw-rw-   0        0        0     2709 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/__init__.py
+-rw-rw-rw-   0        0        0     1958 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/__init__.py
+-rw-rw-rw-   0        0        0     2022 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.681128 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.691101 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/
+-rw-rw-rw-   0        0        0     1377 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/IqFile.py
+-rw-rw-rw-   0        0        0     3152 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/Sall.py
+-rw-rw-rw-   0        0        0     4093 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/__init__.py
+-rw-rw-rw-   0        0        0     1259 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Correction.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.703070 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/
+-rw-rw-rw-   0        0        0     2461 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Attenuation.py
+-rw-rw-rw-   0        0        0     2082 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py
+-rw-rw-rw-   0        0        0     3239 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py
+-rw-rw-rw-   0        0        0     8936 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.710051 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/
+-rw-rw-rw-   0        0        0     6166 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py
+-rw-rw-rw-   0        0        0    12393 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.723016 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/
+-rw-rw-rw-   0        0        0     2570 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.732989 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/
+-rw-rw-rw-   0        0        0     1907 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py
+-rw-rw-rw-   0        0        0     1645 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py
+-rw-rw-rw-   0        0        0     2459 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py
+-rw-rw-rw-   0        0        0     1370 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.746953 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/
+-rw-rw-rw-   0        0        0     2731 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py
+-rw-rw-rw-   0        0        0     2675 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py
+-rw-rw-rw-   0        0        0     2143 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py
+-rw-rw-rw-   0        0        0     5475 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     1479 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Trigger.py
+-rw-rw-rw-   0        0        0    15177 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.755929 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.775876 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/
+-rw-rw-rw-   0        0        0     3789 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py
+-rw-rw-rw-   0        0        0     3053 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py
+-rw-rw-rw-   0        0        0     3118 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py
+-rw-rw-rw-   0        0        0     2425 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py
+-rw-rw-rw-   0        0        0     5646 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     1463 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/Trigger.py
+-rw-rw-rw-   0        0        0    10961 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.780862 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.787843 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/
+-rw-rw-rw-   0        0        0     1969 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py
+-rw-rw-rw-   0        0        0     1891 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py
+-rw-rw-rw-   0        0        0     6078 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.795822 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.801806 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/
+-rw-rw-rw-   0        0        0     3163 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/Frequency.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.808787 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/
+-rw-rw-rw-   0        0        0     3270 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py
+-rw-rw-rw-   0        0        0     1904 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py
+-rw-rw-rw-   0        0        0     3556 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.818761 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/
+-rw-rw-rw-   0        0        0      900 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.829732 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/
+-rw-rw-rw-   0        0        0     1469 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py
+-rw-rw-rw-   0        0        0     1445 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py
+-rw-rw-rw-   0        0        0     2945 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.860648 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/
+-rw-rw-rw-   0        0        0     2423 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Cidx.py
+-rw-rw-rw-   0        0        0     3755 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py
+-rw-rw-rw-   0        0        0     3019 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.866633 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.875609 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/
+-rw-rw-rw-   0        0        0     1302 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/Connection.py
+-rw-rw-rw-   0        0        0     1069 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/__init__.py
+-rw-rw-rw-   0        0        0     2342 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Connection.py
+-rw-rw-rw-   0        0        0     2119 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/__init__.py
+-rw-rw-rw-   0        0        0     3464 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py
+-rw-rw-rw-   0        0        0     3204 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py
+-rw-rw-rw-   0        0        0     2828 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py
+-rw-rw-rw-   0        0        0     3080 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py
+-rw-rw-rw-   0        0        0     2419 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py
+-rw-rw-rw-   0        0        0    15308 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.891566 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/
+-rw-rw-rw-   0        0        0     1126 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.899545 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.907523 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/
+-rw-rw-rw-   0        0        0     3261 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/Bandwidth.py
+-rw-rw-rw-   0        0        0     1066 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/__init__.py
+-rw-rw-rw-   0        0        0     2729 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.913507 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/
+-rw-rw-rw-   0        0        0     3285 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/Bandwidth.py
+-rw-rw-rw-   0        0        0     1051 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/__init__.py
+-rw-rw-rw-   0        0        0     4452 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py
+-rw-rw-rw-   0        0        0     1780 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/__init__.py
+-rw-rw-rw-   0        0        0     3391 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py
+-rw-rw-rw-   0        0        0     2509 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py
+-rw-rw-rw-   0        0        0     3053 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py
+-rw-rw-rw-   0        0        0     3387 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py
+-rw-rw-rw-   0        0        0     1449 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Trigger.py
+-rw-rw-rw-   0        0        0    11165 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.920489 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/
+-rw-rw-rw-   0        0        0     1285 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/LrStart.py
+-rw-rw-rw-   0        0        0     9793 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/__init__.py
+-rw-rw-rw-   0        0        0     1431 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Scenario.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.924478 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.936447 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/
+-rw-rw-rw-   0        0        0     2118 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Rbw.py
+-rw-rw-rw-   0        0        0     2188 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Swt.py
+-rw-rw-rw-   0        0        0     2196 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Vbw.py
+-rw-rw-rw-   0        0        0     3640 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.942430 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/
+-rw-rw-rw-   0        0        0     2365 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/Span.py
+-rw-rw-rw-   0        0        0     4653 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.952404 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/
+-rw-rw-rw-   0        0        0     3239 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Rbw.py
+-rw-rw-rw-   0        0        0     2184 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Vbw.py
+-rw-rw-rw-   0        0        0     3844 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/__init__.py
+-rw-rw-rw-   0        0        0     5241 2024-04-24 14:07:50.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/__init__.py
+-rw-rw-rw-   0        0        0     3857 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1315 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.963374 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.967364 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.971353 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.983321 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/
+-rw-rw-rw-   0        0        0     1672 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py
+-rw-rw-rw-   0        0        0     1706 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py
+-rw-rw-rw-   0        0        0     1310 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py
+-rw-rw-rw-   0        0        0     1055 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.996287 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/
+-rw-rw-rw-   0        0        0     1162 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py
+-rw-rw-rw-   0        0        0     1171 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py
+-rw-rw-rw-   0        0        0     1180 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py
+-rw-rw-rw-   0        0        0     1525 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py
+-rw-rw-rw-   0        0        0     2171 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Edevice.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.009251 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/
+-rw-rw-rw-   0        0        0     1645 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/HwProperties.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.017230 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/
+-rw-rw-rw-   0        0        0     1377 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/To.py
+-rw-rw-rw-   0        0        0      984 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/__init__.py
+-rw-rw-rw-   0        0        0     1876 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Moving.py
+-rw-rw-rw-   0        0        0     1669 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/Versions.py
+-rw-rw-rw-   0        0        0     2687 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Positioner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.024212 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/
+-rw-rw-rw-   0        0        0     1723 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py
+-rw-rw-rw-   0        0        0     1032 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py
+-rw-rw-rw-   0        0        0      891 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Reset.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.028202 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.031193 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.040169 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/
+-rw-rw-rw-   0        0        0     1861 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py
+-rw-rw-rw-   0        0        0     1825 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py
+-rw-rw-rw-   0        0        0     1205 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py
+-rw-rw-rw-   0        0        0     1817 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py
+-rw-rw-rw-   0        0        0      990 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.043161 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.046153 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.055131 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/
+-rw-rw-rw-   0        0        0     1729 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Rx.py
+-rw-rw-rw-   0        0        0     1729 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Tx.py
+-rw-rw-rw-   0        0        0     1200 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/__init__.py
+-rw-rw-rw-   0        0        0     1006 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/__init__.py
+-rw-rw-rw-   0        0        0      992 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.062111 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/
+-rw-rw-rw-   0        0        0     1173 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/Partial.py
+-rw-rw-rw-   0        0        0     1022 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/__init__.py
+-rw-rw-rw-   0        0        0     1856 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Vse.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.069092 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/
+-rw-rw-rw-   0        0        0     1323 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/Attenuation.py
+-rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.075077 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/
+-rw-rw-rw-   0        0        0     1323 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/Attenuation.py
+-rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/__init__.py
+-rw-rw-rw-   0        0        0     3612 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.077071 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.086047 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.094026 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/
+-rw-rw-rw-   0        0        0     1689 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Rx.py
+-rw-rw-rw-   0        0        0     1689 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Tx.py
+-rw-rw-rw-   0        0        0     1223 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.103002 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/
+-rw-rw-rw-   0        0        0     1828 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Rx.py
+-rw-rw-rw-   0        0        0     1828 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Tx.py
+-rw-rw-rw-   0        0        0     1243 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1914 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Direction.py
+-rw-rw-rw-   0        0        0     2359 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Info.py
+-rw-rw-rw-   0        0        0     1847 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/__init__.py
+-rw-rw-rw-   0        0        0     1542 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.105993 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.108985 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.111977 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.120953 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/
+-rw-rw-rw-   0        0        0     1327 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0     1381 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.126937 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/
+-rw-rw-rw-   0        0        0     1405 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py
+-rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.129930 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.131924 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.138905 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/
+-rw-rw-rw-   0        0        0     1263 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py
+-rw-rw-rw-   0        0        0     1056 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py
+-rw-rw-rw-   0        0        0     1027 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.140899 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.145886 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/
+-rw-rw-rw-   0        0        0     1225 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/Measurement.py
+-rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.147882 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.151872 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.153865 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.156857 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.161844 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/
+-rw-rw-rw-   0        0        0     2337 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py
+-rw-rw-rw-   0        0        0     2757 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.167828 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/
+-rw-rw-rw-   0        0        0     2325 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py
+-rw-rw-rw-   0        0        0     2740 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/__init__.py
+-rw-rw-rw-   0        0        0     1216 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.171818 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.177802 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/
+-rw-rw-rw-   0        0        0     2337 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/FilterPy.py
+-rw-rw-rw-   0        0        0     2757 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.198747 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/
+-rw-rw-rw-   0        0        0     2325 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/FilterPy.py
+-rw-rw-rw-   0        0        0     2740 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/__init__.py
+-rw-rw-rw-   0        0        0     1216 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/__init__.py
+-rw-rw-rw-   0        0        0     1238 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py
+-rw-rw-rw-   0        0        0     1025 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.213705 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/
+-rw-rw-rw-   0        0        0     1981 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/Logging.py
+-rw-rw-rw-   0        0        0     1024 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/__init__.py
+-rw-rw-rw-   0        0        0     1229 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py
+-rw-rw-rw-   0        0        0     1258 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.217695 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.224676 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/
+-rw-rw-rw-   0        0        0     2255 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/State.py
+-rw-rw-rw-   0        0        0     1011 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/__init__.py
+-rw-rw-rw-   0        0        0     1009 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.228665 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.236645 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/
+-rw-rw-rw-   0        0        0     1191 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/Dapi.py
+-rw-rw-rw-   0        0        0     1033 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1067 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.239636 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.261577 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/
+-rw-rw-rw-   0        0        0     1231 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Correction.py
+-rw-rw-rw-   0        0        0      834 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfProperty.py
+-rw-rw-rw-   0        0        0     1314 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSettings.py
+-rw-rw-rw-   0        0        0     1311 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSetttings.py
+-rw-rw-rw-   0        0        0     1211 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Rms.py
+-rw-rw-rw-   0        0        0     2062 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Snumber.py
+-rw-rw-rw-   0        0        0     3120 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.267562 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.273546 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/
+-rw-rw-rw-   0        0        0     1320 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/Rnames.py
+-rw-rw-rw-   0        0        0     2409 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.294489 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.300473 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/
+-rw-rw-rw-   0        0        0     2381 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/Bandwidth.py
+-rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/__init__.py
+-rw-rw-rw-   0        0        0      865 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Franges.py
+-rw-rw-rw-   0        0        0     2332 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Frequency.py
+-rw-rw-rw-   0        0        0     2276 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Fspan.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.307454 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/
+-rw-rw-rw-   0        0        0     2363 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/Bandwidth.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.313438 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.319423 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/
+-rw-rw-rw-   0        0        0     2454 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/Bandwidth.py
+-rw-rw-rw-   0        0        0     1064 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.325406 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/
+-rw-rw-rw-   0        0        0     2436 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/Bandwidth.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/__init__.py
+-rw-rw-rw-   0        0        0     2377 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Samples.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.331390 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/
+-rw-rw-rw-   0        0        0     2345 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/Iranges.py
+-rw-rw-rw-   0        0        0     1036 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     1357 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/LoFrequency.py
+-rw-rw-rw-   0        0        0     2304 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/NbLevel.py
+-rw-rw-rw-   0        0        0     2326 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/SymbolRate.py
+-rw-rw-rw-   0        0        0     4175 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/__init__.py
+-rw-rw-rw-   0        0        0     2046 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Snumber.py
+-rw-rw-rw-   0        0        0     3535 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1313 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.337375 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/
+-rw-rw-rw-   0        0        0     1125 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/Scpi.py
+-rw-rw-rw-   0        0        0      996 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.339369 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.348345 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/
+-rw-rw-rw-   0        0        0     1301 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Generator.py
+-rw-rw-rw-   0        0        0     1319 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Measurement.py
+-rw-rw-rw-   0        0        0     1314 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.354330 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/
+-rw-rw-rw-   0        0        0     1325 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/Measurement.py
+-rw-rw-rw-   0        0        0     1059 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.360313 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/
+-rw-rw-rw-   0        0        0     1313 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/Measurement.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/__init__.py
+-rw-rw-rw-   0        0        0     1441 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.363306 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.366298 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.372282 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/
+-rw-rw-rw-   0        0        0     2310 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/Output.py
+-rw-rw-rw-   0        0        0     1021 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/__init__.py
+-rw-rw-rw-   0        0        0     1001 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/__init__.py
+-rw-rw-rw-   0        0        0     1003 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/__init__.py
+-rw-rw-rw-   0        0        0     2693 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.375273 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.378265 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.381258 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.387242 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/
+-rw-rw-rw-   0        0        0     2115 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/All.py
+-rw-rw-rw-   0        0        0     2756 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/__init__.py
+-rw-rw-rw-   0        0        0     3733 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.390234 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.396217 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/
+-rw-rw-rw-   0        0        0     2116 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/All.py
+-rw-rw-rw-   0        0        0     2757 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/__init__.py
+-rw-rw-rw-   0        0        0     6124 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.410180 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/
+-rw-rw-rw-   0        0        0     1845 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Icomponent.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.419158 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/
+-rw-rw-rw-   0        0        0     2613 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Average.py
+-rw-rw-rw-   0        0        0     2613 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Current.py
+-rw-rw-rw-   0        0        0     1273 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.436111 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/
+-rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Average.py
+-rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Current.py
+-rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Maximum.py
+-rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Minimum.py
+-rw-rw-rw-   0        0        0     1761 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/__init__.py
+-rw-rw-rw-   0        0        0     1845 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Qcomponent.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.442095 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/
+-rw-rw-rw-   0        0        0     2121 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/All.py
+-rw-rw-rw-   0        0        0     2762 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/__init__.py
+-rw-rw-rw-   0        0        0     4744 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.459050 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/
+-rw-rw-rw-   0        0        0     1553 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Bin.py
+-rw-rw-rw-   0        0        0      944 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Reliability.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.465034 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/
+-rw-rw-rw-   0        0        0     2118 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/All.py
+-rw-rw-rw-   0        0        0     2759 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/__init__.py
+-rw-rw-rw-   0        0        0      920 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/SymbolRate.py
+-rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Talignment.py
+-rw-rw-rw-   0        0        0     7279 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.486976 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/
+-rw-rw-rw-   0        0        0     1792 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/FreqError.py
+-rw-rw-rw-   0        0        0     1731 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Icomponent.py
+-rw-rw-rw-   0        0        0     1708 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Level.py
+-rw-rw-rw-   0        0        0     3029 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/OfError.py
+-rw-rw-rw-   0        0        0     1708 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Phase.py
+-rw-rw-rw-   0        0        0     1731 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Qcomponent.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.492959 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/
+-rw-rw-rw-   0        0        0     2110 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/All.py
+-rw-rw-rw-   0        0        0     2751 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/__init__.py
+-rw-rw-rw-   0        0        0     5210 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.495952 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.502933 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/
+-rw-rw-rw-   0        0        0     4990 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/Power.py
+-rw-rw-rw-   0        0        0     1855 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.508917 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/
+-rw-rw-rw-   0        0        0     2100 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/All.py
+-rw-rw-rw-   0        0        0     2741 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/__init__.py
+-rw-rw-rw-   0        0        0     3899 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.513903 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/
+-rw-rw-rw-   0        0        0     1254 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.528864 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/
+-rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py
+-rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py
+-rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py
+-rw-rw-rw-   0        0        0     1097 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py
+-rw-rw-rw-   0        0        0     1686 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.541828 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/
+-rw-rw-rw-   0        0        0     1708 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Frequency.py
+-rw-rw-rw-   0        0        0     1452 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Gain.py
+-rw-rw-rw-   0        0        0     1652 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/State.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.550805 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/
+-rw-rw-rw-   0        0        0     1733 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Frequency.py
+-rw-rw-rw-   0        0        0     1477 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Gain.py
+-rw-rw-rw-   0        0        0     1267 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/__init__.py
+-rw-rw-rw-   0        0        0     2778 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.556789 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/
+-rw-rw-rw-   0        0        0     1348 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/State.py
+-rw-rw-rw-   0        0        0     1861 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.563770 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/
+-rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/State.py
+-rw-rw-rw-   0        0        0     2026 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.568757 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/
+-rw-rw-rw-   0        0        0     1638 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/State.py
+-rw-rw-rw-   0        0        0     2037 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.574741 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/
+-rw-rw-rw-   0        0        0     2103 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py
+-rw-rw-rw-   0        0        0     2744 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py
+-rw-rw-rw-   0        0        0     3588 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.587707 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/
+-rw-rw-rw-   0        0        0     1152 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.594689 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/
+-rw-rw-rw-   0        0        0     1620 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py
+-rw-rw-rw-   0        0        0     4648 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.609648 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/
+-rw-rw-rw-   0        0        0     1741 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Power.py
+-rw-rw-rw-   0        0        0     1340 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Probability.py
+-rw-rw-rw-   0        0        0     1485 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Sample.py
+-rw-rw-rw-   0        0        0     2322 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.625605 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/
+-rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Maximum.py
+-rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Minimum.py
+-rw-rw-rw-   0        0        0     1620 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Rms.py
+-rw-rw-rw-   0        0        0     5136 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/__init__.py
+-rw-rw-rw-   0        0        0     1170 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.631589 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/
+-rw-rw-rw-   0        0        0     1518 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/Bin.py
+-rw-rw-rw-   0        0        0     3002 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/__init__.py
+-rw-rw-rw-   0        0        0     1998 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.646549 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/
+-rw-rw-rw-   0        0        0     4420 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Average.py
+-rw-rw-rw-   0        0        0     4420 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Current.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.652535 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/
+-rw-rw-rw-   0        0        0     4498 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.659514 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/
+-rw-rw-rw-   0        0        0     4498 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/Current.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.669489 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/
+-rw-rw-rw-   0        0        0     4471 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     4471 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Minimum.py
+-rw-rw-rw-   0        0        0     1270 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/__init__.py
+-rw-rw-rw-   0        0        0     4462 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/StandardDev.py
+-rw-rw-rw-   0        0        0     2263 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.679461 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/
+-rw-rw-rw-   0        0        0     4111 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Current.py
+-rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Maximum.py
+-rw-rw-rw-   0        0        0     1283 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.689434 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/
+-rw-rw-rw-   0        0        0     4111 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Current.py
+-rw-rw-rw-   0        0        0     1656 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Minimum.py
+-rw-rw-rw-   0        0        0     1283 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.698410 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/
+-rw-rw-rw-   0        0        0     4084 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Maximum.py
+-rw-rw-rw-   0        0        0     4084 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Minimum.py
+-rw-rw-rw-   0        0        0     1268 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.704394 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/
+-rw-rw-rw-   0        0        0     1676 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/Current.py
+-rw-rw-rw-   0        0        0     4730 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.710379 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/
+-rw-rw-rw-   0        0        0     2103 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/All.py
+-rw-rw-rw-   0        0        0     2744 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/__init__.py
+-rw-rw-rw-   0        0        0     6839 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.713370 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.733317 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Average.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Current.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Maximum.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Minimum.py
+-rw-rw-rw-   0        0        0     1771 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.740299 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/
+-rw-rw-rw-   0        0        0     2350 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/Npeak.py
+-rw-rw-rw-   0        0        0     1855 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.756256 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Average.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Current.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Maximum.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Minimum.py
+-rw-rw-rw-   0        0        0     1771 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.775206 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Average.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Current.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Maximum.py
+-rw-rw-rw-   0        0        0     1650 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Minimum.py
+-rw-rw-rw-   0        0        0     1771 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.791162 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/
+-rw-rw-rw-   0        0        0     2059 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Npeak.py
+-rw-rw-rw-   0        0        0     2059 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Speak.py
+-rw-rw-rw-   0        0        0     1291 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.809115 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/
+-rw-rw-rw-   0        0        0     1626 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Average.py
+-rw-rw-rw-   0        0        0     1626 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Current.py
+-rw-rw-rw-   0        0        0     1626 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Maximum.py
+-rw-rw-rw-   0        0        0     1626 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Minimum.py
+-rw-rw-rw-   0        0        0     1751 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.828064 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/
+-rw-rw-rw-   0        0        0     1644 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Average.py
+-rw-rw-rw-   0        0        0     1644 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Current.py
+-rw-rw-rw-   0        0        0     1644 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Maximum.py
+-rw-rw-rw-   0        0        0     1644 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Minimum.py
+-rw-rw-rw-   0        0        0     1766 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.834047 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/
+-rw-rw-rw-   0        0        0     1804 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/All.py
+-rw-rw-rw-   0        0        0     2368 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/__init__.py
+-rw-rw-rw-   0        0        0     3902 2024-04-24 14:07:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/__init__.py
+-rw-rw-rw-   0        0        0     3066 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.837041 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.840032 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.844021 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.853995 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/
+-rw-rw-rw-   0        0        0     1329 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/__init__.py
+-rw-rw-rw-   0        0        0     1020 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.856986 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.859979 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.863969 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.873942 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/
+-rw-rw-rw-   0        0        0     1293 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0     1327 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1363 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1121 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/__init__.py
+-rw-rw-rw-   0        0        0     1062 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.876933 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.879926 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.889899 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/
+-rw-rw-rw-   0        0        0     1237 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Rx.py
+-rw-rw-rw-   0        0        0     1237 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Tx.py
+-rw-rw-rw-   0        0        0     1243 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1091 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/__init__.py
+-rw-rw-rw-   0        0        0     1304 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.893888 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.896880 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.899873 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.906853 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/
+-rw-rw-rw-   0        0        0     1633 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/Current.py
+-rw-rw-rw-   0        0        0     1029 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/__init__.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/__init__.py
+-rw-rw-rw-   0        0        0     1009 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.909846 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.912837 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.917823 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/
+-rw-rw-rw-   0        0        0     1670 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1077 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.924805 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/
+-rw-rw-rw-   0        0        0     1250 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/Measurement.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.927797 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.933781 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/
+-rw-rw-rw-   0        0        0     1449 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/RfSettings.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.941760 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/
+-rw-rw-rw-   0        0        0     2377 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/Group.py
+-rw-rw-rw-   0        0        0     2525 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1299 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.950736 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/
+-rw-rw-rw-   0        0        0     1441 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/RfSettings.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.956719 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/
+-rw-rw-rw-   0        0        0      888 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/Catalog.py
+-rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/__init__.py
+-rw-rw-rw-   0        0        0     3754 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1561 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1312 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.959712 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.965696 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/
+-rw-rw-rw-   0        0        0     1616 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.968688 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.985643 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/
+-rw-rw-rw-   0        0        0     1616 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.972678 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.978661 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/
+-rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.991627 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/
+-rw-rw-rw-   0        0        0     1250 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/Measurement.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:00.995616 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.001600 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/
+-rw-rw-rw-   0        0        0     1625 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.004593 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.010576 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/
+-rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.013568 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.022545 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/
+-rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.025536 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.034513 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/
+-rw-rw-rw-   0        0        0     1616 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.038503 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.043488 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/
+-rw-rw-rw-   0        0        0     1634 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.046480 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.053463 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/
+-rw-rw-rw-   0        0        0     1625 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.055456 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.061440 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/
+-rw-rw-rw-   0        0        0     1625 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py
+-rw-rw-rw-   0        0        0     1041 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/__init__.py
+-rw-rw-rw-   0        0        0     3909 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.064432 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.067428 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.070417 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.076400 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/
+-rw-rw-rw-   0        0        0     1813 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py
+-rw-rw-rw-   0        0        0     1049 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.079393 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.088368 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/
+-rw-rw-rw-   0        0        0     1124 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/IsMoving.py
+-rw-rw-rw-   0        0        0     1619 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/Position.py
+-rw-rw-rw-   0        0        0     2199 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/Positioner/__init__.py
+-rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/__init__.py
+-rw-rw-rw-   0        0        0     1235 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.091360 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.095349 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.107318 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.121281 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/
+-rw-rw-rw-   0        0        0     4136 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.127264 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/
+-rw-rw-rw-   0        0        0     2565 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/Delays.py
+-rw-rw-rw-   0        0        0     1028 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/__init__.py
+-rw-rw-rw-   0        0        0     3268 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Msegment.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.133248 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/
+-rw-rw-rw-   0        0        0     2372 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/Range.py
+-rw-rw-rw-   0        0        0     1536 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/__init__.py
+-rw-rw-rw-   0        0        0     2323 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Segments.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.139232 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/
+-rw-rw-rw-   0        0        0     1253 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/Clist.py
+-rw-rw-rw-   0        0        0     3222 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/__init__.py
+-rw-rw-rw-   0        0        0     9112 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.148209 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/
+-rw-rw-rw-   0        0        0     2628 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Level.py
+-rw-rw-rw-   0        0        0     3652 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Ofrequency.py
+-rw-rw-rw-   0        0        0     2150 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/__init__.py
+-rw-rw-rw-   0        0        0     3390 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.189099 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/
+-rw-rw-rw-   0        0        0     2475 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dgain.py
+-rw-rw-rw-   0        0        0     2448 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dtime.py
+-rw-rw-rw-   0        0        0     1225 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Esingle.py
+-rw-rw-rw-   0        0        0     3782 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Fill.py
+-rw-rw-rw-   0        0        0     2507 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Frequency.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.195083 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/
+-rw-rw-rw-   0        0        0     1811 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/Enabling.py
+-rw-rw-rw-   0        0        0     2412 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/__init__.py
+-rw-rw-rw-   0        0        0     2531 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Irepetition.py
+-rw-rw-rw-   0        0        0     2539 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Modulation.py
+-rw-rw-rw-   0        0        0     2529 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Reenabling.py
+-rw-rw-rw-   0        0        0     2607 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/RfLevel.py
+-rw-rw-rw-   0        0        0     1207 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Rlist.py
+-rw-rw-rw-   0        0        0     1207 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Slist.py
+-rw-rw-rw-   0        0        0     2189 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Sstop.py
+-rw-rw-rw-   0        0        0    10413 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/__init__.py
+-rw-rw-rw-   0        0        0     2717 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py
+-rw-rw-rw-   0        0        0     5682 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.207051 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.254924 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/
+-rw-rw-rw-   0        0        0     1635 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Check.py
+-rw-rw-rw-   0        0        0     1762 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/CrcProtect.py
+-rw-rw-rw-   0        0        0     1364 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Download.py
+-rw-rw-rw-   0        0        0     1515 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Duration.py
+-rw-rw-rw-   0        0        0     1544 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Paratio.py
+-rw-rw-rw-   0        0        0     1627 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Path.py
+-rw-rw-rw-   0        0        0     1518 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Poffset.py
+-rw-rw-rw-   0        0        0     1694 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Reliability.py
+-rw-rw-rw-   0        0        0     1733 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Rmessage.py
+-rw-rw-rw-   0        0        0     1589 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Roption.py
+-rw-rw-rw-   0        0        0     1510 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Samples.py
+-rw-rw-rw-   0        0        0     1525 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/SymbolRate.py
+-rw-rw-rw-   0        0        0     1591 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Waveform.py
+-rw-rw-rw-   0        0        0     8460 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.260907 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/
+-rw-rw-rw-   0        0        0     3565 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/Ofrequency.py
+-rw-rw-rw-   0        0        0     1985 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.289830 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/
+-rw-rw-rw-   0        0        0     2846 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Acycles.py
+-rw-rw-rw-   0        0        0     2850 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dgain.py
+-rw-rw-rw-   0        0        0     2810 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dtime.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.306785 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/
+-rw-rw-rw-   0        0        0     1418 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Call.py
+-rw-rw-rw-   0        0        0     1136 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Insert.py
+-rw-rw-rw-   0        0        0     1126 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mdown.py
+-rw-rw-rw-   0        0        0     1110 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mup.py
+-rw-rw-rw-   0        0        0     2484 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.320748 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/
+-rw-rw-rw-   0        0        0     1519 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Apply.py
+-rw-rw-rw-   0        0        0     3570 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Dgain.py
+-rw-rw-rw-   0        0        0     3758 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Frequency.py
+-rw-rw-rw-   0        0        0     3507 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Lrms.py
+-rw-rw-rw-   0        0        0     3555 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/__init__.py
+-rw-rw-rw-   0        0        0     3163 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Frequency.py
+-rw-rw-rw-   0        0        0     3702 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Itransition.py
+-rw-rw-rw-   0        0        0     5060 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lincrement.py
+-rw-rw-rw-   0        0        0     2772 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lrms.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.330721 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.341691 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/
+-rw-rw-rw-   0        0        0     1312 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Cw.py
+-rw-rw-rw-   0        0        0     1339 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Dtone.py
+-rw-rw-rw-   0        0        0     1321 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Off.py
+-rw-rw-rw-   0        0        0     5147 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.350668 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/
+-rw-rw-rw-   0        0        0     2186 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/All.py
+-rw-rw-rw-   0        0        0     2969 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/__init__.py
+-rw-rw-rw-   0        0        0     2097 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Range.py
+-rw-rw-rw-   0        0        0     3415 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.359644 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.364631 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.368619 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.376599 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/
+-rw-rw-rw-   0        0        0     3080 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/Single.py
+-rw-rw-rw-   0        0        0     1016 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/__init__.py
+-rw-rw-rw-   0        0        0     4245 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/__init__.py
+-rw-rw-rw-   0        0        0     3224 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/__init__.py
+-rw-rw-rw-   0        0        0     1017 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/__init__.py
+-rw-rw-rw-   0        0        0     1538 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/SymbolRate.py
+-rw-rw-rw-   0        0        0     1519 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Ttime.py
+-rw-rw-rw-   0        0        0     5939 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.379590 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.385574 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/
+-rw-rw-rw-   0        0        0     2880 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/All.py
+-rw-rw-rw-   0        0        0     3365 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/__init__.py
+-rw-rw-rw-   0        0        0     1028 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/__init__.py
+-rw-rw-rw-   0        0        0     2786 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Reliability.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.391559 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/
+-rw-rw-rw-   0        0        0     2299 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/Spath.py
+-rw-rw-rw-   0        0        0     1040 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/__init__.py
+-rw-rw-rw-   0        0        0     1298 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Rmarker.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.397542 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/
+-rw-rw-rw-   0        0        0     2146 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/All.py
+-rw-rw-rw-   0        0        0     2133 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/__init__.py
+-rw-rw-rw-   0        0        0     1343 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Tdd.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.400535 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.407515 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/
+-rw-rw-rw-   0        0        0     2592 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/All.py
+-rw-rw-rw-   0        0        0     2470 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/__init__.py
+-rw-rw-rw-   0        0        0     1864 2024-04-24 14:07:49.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/__init__.py
+-rw-rw-rw-   0        0        0     7520 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.427462 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/
+-rw-rw-rw-   0        0        0     2088 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/All.py
+-rw-rw-rw-   0        0        0     1983 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/__init__.py
+-rw-rw-rw-   0        0        0     3944 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py
+-rw-rw-rw-   0        0        0     1038 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py
+-rw-rw-rw-   0        0        0     1006 2024-04-24 14:07:48.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.431452 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.434443 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.447409 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.460374 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/
+-rw-rw-rw-   0        0        0     1256 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Globale.py
+-rw-rw-rw-   0        0        0     1309 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Tenvironment.py
+-rw-rw-rw-   0        0        0     1303 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/__init__.py
+-rw-rw-rw-   0        0        0      805 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Globale.py
+-rw-rw-rw-   0        0        0      839 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Tenvironment.py
+-rw-rw-rw-   0        0        0     1573 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/__init__.py
+-rw-rw-rw-   0        0        0     1119 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.468354 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/
+-rw-rw-rw-   0        0        0     1988 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/Local.py
+-rw-rw-rw-   0        0        0     1004 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.476332 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/
+-rw-rw-rw-   0        0        0     2020 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/Local.py
+-rw-rw-rw-   0        0        0     2496 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/__init__.py
+-rw-rw-rw-   0        0        0     1500 2024-04-24 14:07:54.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.483313 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/
+-rw-rw-rw-   0        0        0      789 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/Spath.py
+-rw-rw-rw-   0        0        0     1042 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.488300 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.491291 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.495281 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.502262 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/
+-rw-rw-rw-   0        0        0      899 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/Catalog.py
+-rw-rw-rw-   0        0        0     1932 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.508246 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/
+-rw-rw-rw-   0        0        0      890 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/Catalog.py
+-rw-rw-rw-   0        0        0     1899 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.516232 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/
+-rw-rw-rw-   0        0        0      893 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/Catalog.py
+-rw-rw-rw-   0        0        0     1910 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.522209 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      912 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1973 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1741 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1077 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.526199 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.529191 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.535174 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.538167 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.541159 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.548140 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/
+-rw-rw-rw-   0        0        0     1020 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.555122 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/
+-rw-rw-rw-   0        0        0     1265 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py
+-rw-rw-rw-   0        0        0     1036 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.558115 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.566092 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/
+-rw-rw-rw-   0        0        0     1321 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py
+-rw-rw-rw-   0        0        0     1038 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py
+-rw-rw-rw-   0        0        0     2034 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py
+-rw-rw-rw-   0        0        0     5898 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.577063 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/
+-rw-rw-rw-   0        0        0     2189 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsMeas.py
+-rw-rw-rw-   0        0        0     2238 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsTrigger.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.583047 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/
+-rw-rw-rw-   0        0        0     1383 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py
+-rw-rw-rw-   0        0        0     1036 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py
+-rw-rw-rw-   0        0        0     2576 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py
+-rw-rw-rw-   0        0        0     2270 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.590028 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.599004 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/
+-rw-rw-rw-   0        0        0     1056 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/Catalog.py
+-rw-rw-rw-   0        0        0     2344 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py
+-rw-rw-rw-   0        0        0     9301 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.604988 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/
+-rw-rw-rw-   0        0        0     1054 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/Catalog.py
+-rw-rw-rw-   0        0        0    10924 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.610972 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/
+-rw-rw-rw-   0        0        0     1044 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/Catalog.py
+-rw-rw-rw-   0        0        0     9138 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.616956 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/
+-rw-rw-rw-   0        0        0     1034 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/Catalog.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.623937 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/
+-rw-rw-rw-   0        0        0     2941 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py
+-rw-rw-rw-   0        0        0     1078 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py
+-rw-rw-rw-   0        0        0     9407 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py
+-rw-rw-rw-   0        0        0     4768 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py
+-rw-rw-rw-   0        0        0     2074 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1313 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.626929 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.629921 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.636903 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      894 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1937 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.639894 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.654855 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.660838 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      894 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1937 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.666822 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/
+-rw-rw-rw-   0        0        0      878 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1885 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.673804 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/
+-rw-rw-rw-   0        0        0      872 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/Catalog.py
+-rw-rw-rw-   0        0        0     1863 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/__init__.py
+-rw-rw-rw-   0        0        0     1513 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.642886 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.645879 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.651862 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      900 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1949 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.678791 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.683777 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.689761 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.695745 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/
+-rw-rw-rw-   0        0        0      881 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1891 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/__init__.py
+-rw-rw-rw-   0        0        0     1301 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.700733 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.703725 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.709708 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.712700 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.716690 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.722673 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      900 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1949 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.728657 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/
+-rw-rw-rw-   0        0        0      884 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/__init__.py
+-rw-rw-rw-   0        0        0     1301 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.731650 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.734641 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.740625 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      900 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1949 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.747607 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/
+-rw-rw-rw-   0        0        0      884 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.754589 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/
+-rw-rw-rw-   0        0        0      878 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/Catalog.py
+-rw-rw-rw-   0        0        0     1875 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/__init__.py
+-rw-rw-rw-   0        0        0     1513 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1057 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.757581 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.760573 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.767554 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      894 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1937 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1047 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.770546 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.773537 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.780521 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      900 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1949 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.786503 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/
+-rw-rw-rw-   0        0        0      899 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/Catalog.py
+-rw-rw-rw-   0        0        0     1952 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.792488 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/
+-rw-rw-rw-   0        0        0      887 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/Catalog.py
+-rw-rw-rw-   0        0        0     1908 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.799468 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/
+-rw-rw-rw-   0        0        0      884 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/Catalog.py
+-rw-rw-rw-   0        0        0     1897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.805452 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/
+-rw-rw-rw-   0        0        0      878 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/Catalog.py
+-rw-rw-rw-   0        0        0     1875 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/__init__.py
+-rw-rw-rw-   0        0        0     2018 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1058 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.809442 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.812434 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.819415 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.822407 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.826396 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.832380 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/
+-rw-rw-rw-   0        0        0      897 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/Catalog.py
+-rw-rw-rw-   0        0        0     1943 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/__init__.py
+-rw-rw-rw-   0        0        0     1073 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/__init__.py
+-rw-rw-rw-   0        0        0     1052 2024-04-24 14:07:52.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/__init__.py
+-rw-rw-rw-   0        0        0     3920 2024-04-24 14:07:51.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/__init__.py
+-rw-rw-rw-   0        0        0        0 2019-11-18 07:28:01.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:08:01.934108 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/
+-rw-rw-rw-   0        0        0      586 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py
+-rw-rw-rw-   0        0        0     4165 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingle.py
+-rw-rw-rw-   0        0        0     1116 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingleList.py
+-rw-rw-rw-   0        0        0     1145 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py
+-rw-rw-rw-   0        0        0     9097 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStringComposer.py
+-rw-rw-rw-   0        0        0     5751 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStruct.py
+-rw-rw-rw-   0        0        0     3439 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStructList.py
+-rw-rw-rw-   0        0        0     2546 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStructStringParser.py
+-rw-rw-rw-   0        0        0     5238 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/CommandsGroup.py
+-rw-rw-rw-   0        0        0    25419 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Conversions.py
+-rw-rw-rw-   0        0        0     3775 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ConverterFromScpiString.py
+-rw-rw-rw-   0        0        0     4768 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ConverterToScpiString.py
+-rw-rw-rw-   0        0        0    14213 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Core.py
+-rw-rw-rw-   0        0        0     1386 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/GlobalData.py
+-rw-rw-rw-   0        0        0    60862 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Instrument.py
+-rw-rw-rw-   0        0        0     4785 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentErrors.py
+-rw-rw-rw-   0        0        0     2225 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentOptions.py
+-rw-rw-rw-   0        0        0    16156 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentSettings.py
+-rw-rw-rw-   0        0        0     3518 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InternalLinker.py
+-rw-rw-rw-   0        0        0     4390 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/IoTransferEventArgs.py
+-rw-rw-rw-   0        0        0      387 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Properties.py
+-rw-rw-rw-   0        0        0     4289 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/RepeatedCapability.py
+-rw-rw-rw-   0        0        0     4745 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ScpiEnums.py
+-rw-rw-rw-   0        0        0    35525 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ScpiLogger.py
+-rw-rw-rw-   0        0        0     5098 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StreamReader.py
+-rw-rw-rw-   0        0        0     5856 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StreamWriter.py
+-rw-rw-rw-   0        0        0     1114 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StructBase.py
+-rw-rw-rw-   0        0        0     3608 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Types.py
+-rw-rw-rw-   0        0        0     5498 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Utilities.py
+-rw-rw-rw-   0        0        0     5716 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py
+-rw-rw-rw-   0        0        0    51976 2024-04-03 11:15:31.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaSession.py
+-rw-rw-rw-   0        0        0     7512 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaSessionSim.py
+-rw-rw-rw-   0        0        0       29 2024-02-28 16:27:53.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/__init__.py
+-rw-rw-rw-   0        0        0    15874 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/RsCMPX_Gprf.py
+-rw-rw-rw-   0        0        0      899 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/__init__.py
+-rw-rw-rw-   0        0        0    11429 2024-04-24 14:07:47.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/enums.py
+-rw-rw-rw-   0        0        0     3704 2024-04-24 14:07:45.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/repcap.py
+drwxrwxrwx   0        0        0        0 2024-04-24 14:07:59.411848 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/
+-rw-rw-rw-   0        0        0     3474 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    53104 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-24 14:07:58.000000 RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 14:08:01.938099 RsCMPX_Gprf-5.0.91/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2024-04-24 14:07:55.000000 RsCMPX_Gprf-5.0.91/setup.py
```

### Comparing `RsCMPX_Gprf-5.0.90/PKG-INFO` & `RsCMPX_Gprf-5.0.91/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RsCMPX_Gprf
-Version: 5.0.90
+Version: 5.0.91
 Summary: CMX/CMP/PVT Global Purpose RF Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_Gprf
         ==================================
@@ -44,15 +44,18 @@
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
         Version history
         ----------------
         
-        	Latest release notes summary: Update for CMP FW 5.0.90
+        	Latest release notes summary: Added missing measurement SCPI from MMI sub-system
+        
+        	Version 5.0.91
+        		- Added missing measurement SCPI from MMI sub-system
         
         	Version 5.0.90
         		- Update for CMP FW 5.0.90
         
         	Version 5.0.20
         		- Update for CMP200 5.0.20
```

### Comparing `RsCMPX_Gprf-5.0.90/README.rst` & `RsCMPX_Gprf-5.0.91/README.rst`

 * *Files 21% similar despite different names*

```diff
@@ -37,15 +37,18 @@
 
 Examples: https://github.com/Rohde-Schwarz/Examples/
 
 
 Version history
 ----------------
 
-	Latest release notes summary: Update for CMP FW 5.0.90
+	Latest release notes summary: Added missing measurement SCPI from MMI sub-system
+
+	Version 5.0.91
+		- Added missing measurement SCPI from MMI sub-system
 
 	Version 5.0.90
 		- Update for CMP FW 5.0.90
 
 	Version 5.0.20
 		- Update for CMP200 5.0.20
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/CustomFiles/events.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/events.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/CustomFiles/reliability.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/CustomFiles/utilities.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/CustomFiles/utilities.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Rx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Tx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Add/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Add/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/Zero.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/Zero.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/ExtPwrSensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Calibration/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Calibration/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class GprfCls:
-	"""Gprf commands group definition. 4 total commands, 2 Subgroups, 0 group commands"""
+	"""Gprf commands group definition. 5 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("gprf", core, parent)
 
 	@property
 	def measurement(self):
-		"""measurement commands group. 1 Sub-classes, 0 commands."""
+		"""measurement commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_measurement'):
 			from .Measurement import MeasurementCls
 			self._measurement = MeasurementCls(self._core, self._cmd_group)
 		return self._measurement
 
 	@property
 	def generator(self):
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Lte/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/LteDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Niot/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Niot/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Niot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrDl/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrMmw/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrMmw/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrMmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrSub/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/NrSub/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/NrSub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/CorrectionTable.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/CorrectionTable.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Reset.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Reset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/Box.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/Box.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rf42/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/Rrhead.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/System/Rrhead.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,43 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class SystemCls:
-	"""System commands group definition. 5 total commands, 4 Subgroups, 0 group commands"""
+	"""System commands group definition. 8 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("system", core, parent)
 
 	@property
-	def reset(self):
-		"""reset commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_reset'):
-			from .Reset import ResetCls
-			self._reset = ResetCls(self._core, self._cmd_group)
-		return self._reset
+	def time(self):
+		"""time commands group. 1 Sub-classes, 2 commands."""
+		if not hasattr(self, '_time'):
+			from .Time import TimeCls
+			self._time = TimeCls(self._core, self._cmd_group)
+		return self._time
 
 	@property
-	def rrhead(self):
-		"""rrhead commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_rrhead'):
-			from .Rrhead import RrheadCls
-			self._rrhead = RrheadCls(self._core, self._cmd_group)
-		return self._rrhead
+	def date(self):
+		"""date commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_date'):
+			from .Date import DateCls
+			self._date = DateCls(self._core, self._cmd_group)
+		return self._date
 
 	@property
 	def attenuation(self):
 		"""attenuation commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_attenuation'):
 			from .Attenuation import AttenuationCls
 			self._attenuation = AttenuationCls(self._core, self._cmd_group)
 		return self._attenuation
 
-	@property
-	def rf42(self):
-		"""rf42 commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_rf42'):
-			from .Rf42 import Rf42Cls
-			self._rf42 = Rf42Cls(self._core, self._cmd_group)
-		return self._rf42
-
 	def clone(self) -> 'SystemCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = SystemCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/Connectors.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/Connectors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Uwb/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Uwb/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Uwb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wcdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wcdma/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wcdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wlan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wlan/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wlan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wpan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class MeasurementCls:
-	"""Measurement commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
+	"""Measurement commands group definition. 2 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("measurement", core, parent)
 
 	@property
+	def ploss(self):
+		"""ploss commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_ploss'):
+			from .Ploss import PlossCls
+			self._ploss = PlossCls(self._core, self._cmd_group)
+		return self._ploss
+
+	@property
 	def spath(self):
 		"""spath commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_spath'):
 			from .Spath import SpathCls
 			self._spath = SpathCls(self._core, self._cmd_group)
 		return self._spath
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/Wpan/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/Wpan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Catalog/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Catalog/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class CatalogCls:
-	"""Catalog commands group definition. 24 total commands, 16 Subgroups, 0 group commands"""
+	"""Catalog commands group definition. 26 total commands, 16 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("catalog", core, parent)
 
 	@property
 	def system(self):
-		"""system commands group. 4 Sub-classes, 0 commands."""
+		"""system commands group. 4 Sub-classes, 1 commands."""
 		if not hasattr(self, '_system'):
 			from .System import SystemCls
 			self._system = SystemCls(self._core, self._cmd_group)
 		return self._system
 
 	@property
 	def gprf(self):
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/Single.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/Single.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/Tx/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/Bench/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/Usage/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/IqFile.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/IqFile.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/Sall.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/Sall.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Canalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Correction.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Attenuation.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ......Internal import Conversions
 from ......Internal.Utilities import trim_str_response
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class IqRecorderCls:
-	"""IqRecorder commands group definition. 26 total commands, 4 Subgroups, 11 group commands"""
+	"""IqRecorder commands group definition. 27 total commands, 5 Subgroups, 11 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("iqRecorder", core, parent)
 
 	@property
 	def capture(self):
@@ -41,14 +41,22 @@
 	def listPy(self):
 		"""listPy commands group. 3 Sub-classes, 5 commands."""
 		if not hasattr(self, '_listPy'):
 			from .ListPy import ListPyCls
 			self._listPy = ListPyCls(self._core, self._cmd_group)
 		return self._listPy
 
+	@property
+	def trigger(self):
+		"""trigger commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_trigger'):
+			from .Trigger import TriggerCls
+			self._trigger = TriggerCls(self._core, self._cmd_group)
+		return self._trigger
+
 	def get_symbol_rate(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQRecorder:SRATe \n
 		Snippet: value: float = driver.configure.gprf.measurement.iqRecorder.get_symbol_rate() \n
 		No command help available \n
 			:return: sample_rate: No help available
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:IQRecorder:SRATe?')
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,36 @@
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class IqVsSlotCls:
-	"""IqVsSlot commands group definition. 18 total commands, 1 Subgroups, 7 group commands"""
+	"""IqVsSlot commands group definition. 19 total commands, 2 Subgroups, 7 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("iqVsSlot", core, parent)
 
 	@property
 	def listPy(self):
 		"""listPy commands group. 4 Sub-classes, 4 commands."""
 		if not hasattr(self, '_listPy'):
 			from .ListPy import ListPyCls
 			self._listPy = ListPyCls(self._core, self._cmd_group)
 		return self._listPy
 
+	@property
+	def trigger(self):
+		"""trigger commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_trigger'):
+			from .Trigger import TriggerCls
+			self._trigger = TriggerCls(self._core, self._cmd_group)
+		return self._trigger
+
 	def get_timeout(self) -> float:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:IQVSlot:TOUT \n
 		Snippet: value: float = driver.configure.gprf.measurement.iqVsSlot.get_timeout() \n
 		Defines a timeout for the measurement. The timer is started when the measurement is initiated via a READ or INIT command.
 		It is not started if the measurement is initiated manually. When the measurement has completed the first measurement
 		cycle (first single shot) , the statistical depth is reached and the timer is reset. If the first measurement cycle has
 		not been completed when the timer expires, the measurement is stopped. The measurement state changes to RDY.
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class PlossCls:
-	"""Ploss commands group definition. 7 total commands, 2 Subgroups, 2 group commands"""
+	"""Ploss commands group definition. 8 total commands, 3 Subgroups, 2 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("ploss", core, parent)
 
 	@property
 	def tsTone(self):
@@ -24,14 +24,22 @@
 	def view(self):
 		"""view commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_view'):
 			from .View import ViewCls
 			self._view = ViewCls(self._core, self._cmd_group)
 		return self._view
 
+	@property
+	def listPy(self):
+		"""listPy commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_listPy'):
+			from .ListPy import ListPyCls
+			self._listPy = ListPyCls(self._core, self._cmd_group)
+		return self._listPy
+
 	def get_trace(self) -> bool:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:PLOSs:TRACe \n
 		Snippet: value: bool = driver.configure.gprf.measurement.ploss.get_trace() \n
 		Selects whether a result diagram is provided. \n
 			:return: trace_mode: OFF: no result diagram, faster measurement ON: result diagram, slower measurement
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:PLOSs:TRACe?')
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .......Internal.StructBase import StructBase
 from .......Internal.ArgStruct import ArgStruct
 from ....... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class ListPyCls:
-	"""ListPy commands group definition. 22 total commands, 7 Subgroups, 8 group commands"""
+	"""ListPy commands group definition. 27 total commands, 9 Subgroups, 10 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("listPy", core, parent)
 
 	@property
 	def iqData(self):
@@ -66,14 +66,30 @@
 	def parameterSetList(self):
 		"""parameterSetList commands group. 0 Sub-classes, 2 commands."""
 		if not hasattr(self, '_parameterSetList'):
 			from .ParameterSetList import ParameterSetListCls
 			self._parameterSetList = ParameterSetListCls(self._core, self._cmd_group)
 		return self._parameterSetList
 
+	@property
+	def idx(self):
+		"""idx commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_idx'):
+			from .Idx import IdxCls
+			self._idx = IdxCls(self._core, self._cmd_group)
+		return self._idx
+
+	@property
+	def cidx(self):
+		"""cidx commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_cidx'):
+			from .Cidx import CidxCls
+			self._cidx = CidxCls(self._core, self._cmd_group)
+		return self._cidx
+
 	# noinspection PyTypeChecker
 	def get_txi_mode(self) -> enums.TxiMode:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:TXIMode \n
 		Snippet: value: enums.TxiMode = driver.configure.gprf.measurement.power.listPy.get_txi_mode() \n
 		Selects the repetition of the GPRF Meas<i>:Power trigger signal, generated by the power measurement for a repeated
 		segment. \n
 			:return: mode:
@@ -234,14 +250,51 @@
 		Selects the last segment to be measured (the end of a sweep) . The total number of segments per sweep, including
 		repetitions, must not be higher than 10000. \n
 			:param stop_index: No help available
 		"""
 		param = Conversions.decimal_value_to_str(stop_index)
 		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:STOP {param}')
 
+	# noinspection PyTypeChecker
+	def get_csource(self) -> enums.ConnectionSource:
+		"""SCPI: [CONFigure]:GPRF:MEASurement<instance>:POWer:LIST:CSOurce \n
+		Snippet: value: enums.ConnectionSource = driver.configure.gprf.measurement.power.listPy.get_csource() \n
+		Selects whether all list mode segments use the same RF connection. \n
+			:return: connection_source: GLOBal: Use the same RF connection for all segments. INDex: Assign a connection index to each segment.
+		"""
+		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:CSOurce?')
+		return Conversions.str_to_scalar_enum(response, enums.ConnectionSource)
+
+	def set_csource(self, connection_source: enums.ConnectionSource) -> None:
+		"""SCPI: [CONFigure]:GPRF:MEASurement<instance>:POWer:LIST:CSOurce \n
+		Snippet: driver.configure.gprf.measurement.power.listPy.set_csource(connection_source = enums.ConnectionSource.GLOBal) \n
+		Selects whether all list mode segments use the same RF connection. \n
+			:param connection_source: GLOBal: Use the same RF connection for all segments. INDex: Assign a connection index to each segment.
+		"""
+		param = Conversions.enum_scalar_to_str(connection_source, enums.ConnectionSource)
+		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:CSOurce {param}')
+
+	def get_nidx(self) -> int:
+		"""SCPI: [CONFigure]:GPRF:MEASurement<instance>:POWer:LIST:NIDX \n
+		Snippet: value: int = driver.configure.gprf.measurement.power.listPy.get_nidx() \n
+		Sets the number of connection indices for the list mode, for the connection source INDex. \n
+			:return: number_of_indices: No help available
+		"""
+		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:NIDX?')
+		return Conversions.str_to_int(response)
+
+	def set_nidx(self, number_of_indices: int) -> None:
+		"""SCPI: [CONFigure]:GPRF:MEASurement<instance>:POWer:LIST:NIDX \n
+		Snippet: driver.configure.gprf.measurement.power.listPy.set_nidx(number_of_indices = 1) \n
+		Sets the number of connection indices for the list mode, for the connection source INDex. \n
+			:param number_of_indices: No help available
+		"""
+		param = Conversions.decimal_value_to_str(number_of_indices)
+		self._core.io.write(f'CONFigure:GPRF:MEASurement<Instance>:POWer:LIST:NIDX {param}')
+
 	def get_value(self) -> bool:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:LIST \n
 		Snippet: value: bool = driver.configure.gprf.measurement.power.listPy.get_value() \n
 		Enables or disables the list mode for the power measurement. \n
 			:return: enable_list_mode: OFF: list mode off ON: list mode on
 		"""
 		response = self._core.io.query_str('CONFigure:GPRF:MEASurement<Instance>:POWer:LIST?')
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/Bandwidth.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandpass/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/Bandwidth.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/Bandwidth.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Gauss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from ......Internal import Conversions
 from ......Internal.Utilities import trim_str_response
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class PowerCls:
-	"""Power commands group definition. 48 total commands, 4 Subgroups, 7 group commands"""
+	"""Power commands group definition. 54 total commands, 5 Subgroups, 7 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("power", core, parent)
 
 	@property
 	def parameterSetList(self):
@@ -35,20 +35,28 @@
 		if not hasattr(self, '_filterPy'):
 			from .FilterPy import FilterPyCls
 			self._filterPy = FilterPyCls(self._core, self._cmd_group)
 		return self._filterPy
 
 	@property
 	def listPy(self):
-		"""listPy commands group. 7 Sub-classes, 8 commands."""
+		"""listPy commands group. 9 Sub-classes, 10 commands."""
 		if not hasattr(self, '_listPy'):
 			from .ListPy import ListPyCls
 			self._listPy = ListPyCls(self._core, self._cmd_group)
 		return self._listPy
 
+	@property
+	def trigger(self):
+		"""trigger commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_trigger'):
+			from .Trigger import TriggerCls
+			self._trigger = TriggerCls(self._core, self._cmd_group)
+		return self._trigger
+
 	# noinspection PyTypeChecker
 	def get_mode(self) -> enums.CcdfMode:
 		"""SCPI: CONFigure:GPRF:MEASurement<Instance>:POWer:MODE \n
 		Snippet: value: enums.CcdfMode = driver.configure.gprf.measurement.power.get_mode() \n
 		Selects the measurement mode for measurements without list mode. Select the mode before starting the power measurement. \n
 			:return: ccdf_mode: No help available
 		"""
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/LrStart.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/LrStart.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/RfSettings/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Scenario.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Scenario.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Rbw.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Rbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Swt.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Swt.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Vbw.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/Vbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/FreqSweep/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/Span.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/Span.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/Frequency/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Rbw.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Rbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Vbw.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/Vbw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/ZeroSpan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class MeasurementCls:
-	"""Measurement commands group definition. 167 total commands, 12 Subgroups, 0 group commands"""
+	"""Measurement commands group definition. 176 total commands, 12 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("measurement", core, parent)
 
 	@property
 	def rfSettings(self):
@@ -32,23 +32,23 @@
 		if not hasattr(self, '_correction'):
 			from .Correction import CorrectionCls
 			self._correction = CorrectionCls(self._core, self._cmd_group)
 		return self._correction
 
 	@property
 	def power(self):
-		"""power commands group. 4 Sub-classes, 7 commands."""
+		"""power commands group. 5 Sub-classes, 7 commands."""
 		if not hasattr(self, '_power'):
 			from .Power import PowerCls
 			self._power = PowerCls(self._core, self._cmd_group)
 		return self._power
 
 	@property
 	def iqVsSlot(self):
-		"""iqVsSlot commands group. 1 Sub-classes, 7 commands."""
+		"""iqVsSlot commands group. 2 Sub-classes, 7 commands."""
 		if not hasattr(self, '_iqVsSlot'):
 			from .IqVsSlot import IqVsSlotCls
 			self._iqVsSlot = IqVsSlotCls(self._core, self._cmd_group)
 		return self._iqVsSlot
 
 	@property
 	def extPwrSensor(self):
@@ -64,15 +64,15 @@
 		if not hasattr(self, '_nrpm'):
 			from .Nrpm import NrpmCls
 			self._nrpm = NrpmCls(self._core, self._cmd_group)
 		return self._nrpm
 
 	@property
 	def iqRecorder(self):
-		"""iqRecorder commands group. 4 Sub-classes, 11 commands."""
+		"""iqRecorder commands group. 5 Sub-classes, 11 commands."""
 		if not hasattr(self, '_iqRecorder'):
 			from .IqRecorder import IqRecorderCls
 			self._iqRecorder = IqRecorderCls(self._core, self._cmd_group)
 		return self._iqRecorder
 
 	@property
 	def spectrum(self):
@@ -96,15 +96,15 @@
 		if not hasattr(self, '_canalyzer'):
 			from .Canalyzer import CanalyzerCls
 			self._canalyzer = CanalyzerCls(self._core, self._cmd_group)
 		return self._canalyzer
 
 	@property
 	def ploss(self):
-		"""ploss commands group. 2 Sub-classes, 2 commands."""
+		"""ploss commands group. 3 Sub-classes, 2 commands."""
 		if not hasattr(self, '_ploss'):
 			from .Ploss import PlossCls
 			self._ploss = PlossCls(self._core, self._cmd_group)
 		return self._ploss
 
 	def clone(self) -> 'MeasurementCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Gprf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class GprfCls:
-	"""Gprf commands group definition. 172 total commands, 2 Subgroups, 0 group commands"""
+	"""Gprf commands group definition. 181 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("gprf", core, parent)
 
 	@property
 	def generator(self):
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Edevice.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Edevice.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Reset.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Reset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Rx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Tx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/Source/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/Lo/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Rrhead/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Save/Partial.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/Partial.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Save/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Save/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Vse.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Vse.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z310/Attenuation.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z310/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z310/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z320/Attenuation.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/Attenuation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/Z320/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/Z320/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/System/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class SystemCls:
-	"""System commands group definition. 17 total commands, 11 Subgroups, 0 group commands"""
+	"""System commands group definition. 21 total commands, 12 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("system", core, parent)
 
 	@property
+	def positioner(self):
+		"""positioner commands group. 4 Sub-classes, 0 commands."""
+		if not hasattr(self, '_positioner'):
+			from .Positioner import PositionerCls
+			self._positioner = PositionerCls(self._core, self._cmd_group)
+		return self._positioner
+
+	@property
 	def reset(self):
 		"""reset commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_reset'):
 			from .Reset import ResetCls
 			self._reset = ResetCls(self._core, self._cmd_group)
 		return self._reset
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Rx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Tx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Rx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Tx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Direction.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Direction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Info.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/Info.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Configure/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Configure/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class ConfigureCls:
-	"""Configure commands group definition. 195 total commands, 3 Subgroups, 0 group commands"""
+	"""Configure commands group definition. 208 total commands, 3 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("configure", core, parent)
 
 	@property
 	def gprf(self):
@@ -16,15 +16,15 @@
 		if not hasattr(self, '_gprf'):
 			from .Gprf import GprfCls
 			self._gprf = GprfCls(self._core, self._cmd_group)
 		return self._gprf
 
 	@property
 	def system(self):
-		"""system commands group. 11 Sub-classes, 0 commands."""
+		"""system commands group. 12 Sub-classes, 0 commands."""
 		if not hasattr(self, '_system'):
 			from .System import SystemCls
 			self._system = SystemCls(self._core, self._cmd_group)
 		return self._system
 
 	@property
 	def tenvironment(self):
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Create/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Create/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/FilterPy.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Psub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/FilterPy.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/FilterPy.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/Rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/Mars/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/Logging.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/Logging.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Scpi/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class ConfigureCls:
-	"""Configure commands group definition. 18 total commands, 1 Subgroups, 0 group commands"""
+class AddCls:
+	"""Add commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("configure", core, parent)
+		self._cmd_group = CommandsGroup("add", core, parent)
 
 	@property
-	def system(self):
-		"""system commands group. 2 Sub-classes, 0 commands."""
-		if not hasattr(self, '_system'):
-			from .System import SystemCls
-			self._system = SystemCls(self._core, self._cmd_group)
-		return self._system
+	def debug(self):
+		"""debug commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_debug'):
+			from .Debug import DebugCls
+			self._debug = DebugCls(self._core, self._cmd_group)
+		return self._debug
 
-	def clone(self) -> 'ConfigureCls':
+	def clone(self) -> 'AddCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = ConfigureCls(self._core, self._cmd_group.parent)
+		new_group = AddCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/State.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/State.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Fetch/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/Dapi.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/Dapi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Generic/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Generic/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Correction.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Correction.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfProperty.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfProperty.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSettings.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSetttings.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/RfSetttings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Rms.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Snumber.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/Snumber.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/Rnames.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/Rnames.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Ploss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/Bandwidth.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/Bandwidth.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class BandwidthCls:
 	"""Bandwidth commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("bandwidth", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:BANDpass:BWIDth \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.bandpass.bandwidth.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.bandpass.bandwidth.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:BANDpass:BWIDth {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class BandwidthStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> BandwidthStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:BANDpass:BWIDth \n
 		Snippet: value: BandwidthStruct = driver.diagnostic.gprf.measurement.rfProperty.bandpass.bandwidth.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for BandwidthStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:BANDpass:BWIDth?', self.__class__.BandwidthStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Bandpass/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Franges.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Franges.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Frequency.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class FrequencyCls:
 	"""Frequency commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("frequency", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:FREQuency \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.frequency.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.frequency.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:FREQuency {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class FrequencyStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> FrequencyStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:FREQuency \n
 		Snippet: value: FrequencyStruct = driver.diagnostic.gprf.measurement.rfProperty.frequency.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for FrequencyStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:FREQuency?', self.__class__.FrequencyStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Fspan.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Fspan.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class FspanCls:
 	"""Fspan commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("fspan", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:FSPan \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.fspan.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.fspan.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:FSPan {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class FspanStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> FspanStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:FSPan \n
 		Snippet: value: FspanStruct = driver.diagnostic.gprf.measurement.rfProperty.fspan.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for FspanStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:FSPan?', self.__class__.FspanStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/Bandwidth.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/Bandwidth.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class BandwidthCls:
 	"""Bandwidth commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("bandwidth", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:GAUSs:BWIDth \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.gauss.bandwidth.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.gauss.bandwidth.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:GAUSs:BWIDth {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class BandwidthStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> BandwidthStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:GAUSs:BWIDth \n
 		Snippet: value: BandwidthStruct = driver.diagnostic.gprf.measurement.rfProperty.gauss.bandwidth.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for BandwidthStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:GAUSs:BWIDth?', self.__class__.BandwidthStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/Gauss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/Bandwidth.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/Bandwidth.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class BandwidthCls:
 	"""Bandwidth commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("bandwidth", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:BANDpass:BWIDth \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.bandpass.bandwidth.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.bandpass.bandwidth.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:BANDpass:BWIDth {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class BandwidthStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> BandwidthStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:BANDpass:BWIDth \n
 		Snippet: value: BandwidthStruct = driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.bandpass.bandwidth.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for BandwidthStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:BANDpass:BWIDth?', self.__class__.BandwidthStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Bandpass/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/Bandwidth.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/Bandwidth.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class BandwidthCls:
 	"""Bandwidth commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("bandwidth", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:GAUSs:BWIDth \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.gauss.bandwidth.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.gauss.bandwidth.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:GAUSs:BWIDth {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class BandwidthStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> BandwidthStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:GAUSs:BWIDth \n
 		Snippet: value: BandwidthStruct = driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.gauss.bandwidth.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for BandwidthStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:GAUSs:BWIDth?', self.__class__.BandwidthStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Gauss/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Samples.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/Samples.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class SamplesCls:
 	"""Samples commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("samples", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:SAMPles \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.samples.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.samples.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:SAMPles {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class SamplesStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> SamplesStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:SAMPles \n
 		Snippet: value: SamplesStruct = driver.diagnostic.gprf.measurement.rfProperty.iqRecorder.samples.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for SamplesStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:IQRecorder:SAMPles?', self.__class__.SamplesStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/IqRecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/Iranges.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/Iranges.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class IrangesCls:
 	"""Iranges commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("iranges", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:LIST:IRANges \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.listPy.iranges.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.listPy.iranges.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:LIST:IRANges {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class IrangesStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> IrangesStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:LIST:IRANges \n
 		Snippet: value: IrangesStruct = driver.diagnostic.gprf.measurement.rfProperty.listPy.iranges.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for IrangesStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:LIST:IRANges?', self.__class__.IrangesStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/LoFrequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/LoFrequency.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 		self._core = core
 		self._cmd_group = CommandsGroup("loFrequency", core, parent)
 
 	def get_available(self) -> bool:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:LOFRequency:AVAilable \n
 		Snippet: value: bool = driver.diagnostic.gprf.measurement.rfProperty.loFrequency.get_available() \n
 		No command help available \n
-			:return: def: No help available
+			:return: def_py: No help available
 		"""
 		response = self._core.io.query_str('DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:LOFRequency:AVAilable?')
 		return Conversions.str_to_bool(response)
 
-	def set_available(self, def: bool) -> None:
+	def set_available(self, def_py: bool) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:LOFRequency:AVAilable \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.loFrequency.set_available(def = False) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.loFrequency.set_available(def_py = False) \n
 		No command help available \n
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = Conversions.bool_to_str(def)
+		param = Conversions.bool_to_str(def_py)
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:LOFRequency:AVAilable {param}')
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/NbLevel.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/NbLevel.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class NbLevelCls:
 	"""NbLevel commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("nbLevel", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:NBLevel \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.nbLevel.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.nbLevel.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:NBLevel {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class NbLevelStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> NbLevelStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:NBLevel \n
 		Snippet: value: NbLevelStruct = driver.diagnostic.gprf.measurement.rfProperty.nbLevel.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for NbLevelStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:NBLevel?', self.__class__.NbLevelStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/SymbolRate.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/SymbolRate.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,41 +11,41 @@
 class SymbolRateCls:
 	"""SymbolRate commands group definition. 1 total commands, 0 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("symbolRate", core, parent)
 
-	def set(self, min_py: float, max_py: float, def: float) -> None:
+	def set(self, min_py: float, max_py: float, def_py: float) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:SRATe \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.symbolRate.set(min_py = 1.0, max_py = 1.0, def = 1.0) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.symbolRate.set(min_py = 1.0, max_py = 1.0, def_py = 1.0) \n
 		No command help available \n
 			:param min_py: No help available
 			:param max_py: No help available
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def', def, DataType.Float))
+		param = ArgSingleList().compose_cmd_string(ArgSingle('min_py', min_py, DataType.Float), ArgSingle('max_py', max_py, DataType.Float), ArgSingle('def_py', def_py, DataType.Float))
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:SRATe {param}'.rstrip())
 
 	# noinspection PyTypeChecker
 	class SymbolRateStruct(StructBase):
 		"""Response structure. Fields: \n
 			- Min_Py: float: No parameter help available
 			- Max_Py: float: No parameter help available
-			- Def: float: No parameter help available"""
+			- Def_Py: float: No parameter help available"""
 		__meta_args_list = [
 			ArgStruct.scalar_float('Min_Py'),
 			ArgStruct.scalar_float('Max_Py'),
-			ArgStruct.scalar_float('Def')]
+			ArgStruct.scalar_float('Def_Py')]
 
 		def __init__(self):
 			StructBase.__init__(self, self)
 			self.Min_Py: float = None
 			self.Max_Py: float = None
-			self.Def: float = None
+			self.Def_Py: float = None
 
 	def get(self) -> SymbolRateStruct:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:SRATe \n
 		Snippet: value: SymbolRateStruct = driver.diagnostic.gprf.measurement.rfProperty.symbolRate.get() \n
 		No command help available \n
 			:return: structure: for return value, see the help for SymbolRateStruct structure arguments."""
 		return self._core.io.query_struct(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:SRATe?', self.__class__.SymbolRateStruct())
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/RfProperty/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,26 +91,26 @@
 			self._loFrequency = LoFrequencyCls(self._core, self._cmd_group)
 		return self._loFrequency
 
 	def get_tfilter(self) -> bool:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:TFILter \n
 		Snippet: value: bool = driver.diagnostic.gprf.measurement.rfProperty.get_tfilter() \n
 		No command help available \n
-			:return: def: No help available
+			:return: def_py: No help available
 		"""
 		response = self._core.io.query_str('DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:TFILter?')
 		return Conversions.str_to_bool(response)
 
-	def set_tfilter(self, def: bool) -> None:
+	def set_tfilter(self, def_py: bool) -> None:
 		"""SCPI: DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:TFILter \n
-		Snippet: driver.diagnostic.gprf.measurement.rfProperty.set_tfilter(def = False) \n
+		Snippet: driver.diagnostic.gprf.measurement.rfProperty.set_tfilter(def_py = False) \n
 		No command help available \n
-			:param def: No help available
+			:param def_py: No help available
 		"""
-		param = Conversions.bool_to_str(def)
+		param = Conversions.bool_to_str(def_py)
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:RFPRoperty:TFILter {param}')
 
 	def clone(self) -> 'RfPropertyCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = RfPropertyCls(self._core, self._cmd_group.parent)
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Snumber.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/Snumber.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/Measurement/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
+from .....Internal.Utilities import trim_str_response
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class MeasurementCls:
-	"""Measurement commands group definition. 20 total commands, 3 Subgroups, 2 group commands"""
+	"""Measurement commands group definition. 21 total commands, 3 Subgroups, 3 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("measurement", core, parent)
 
 	@property
 	def rfProperty(self):
@@ -67,14 +68,23 @@
 		Snippet: driver.diagnostic.gprf.measurement.set_debug(enable = False) \n
 		No command help available \n
 			:param enable: No help available
 		"""
 		param = Conversions.bool_to_str(enable)
 		self._core.io.write(f'DIAGnostic:GPRF:MEASurement<Instance>:DEBug {param}')
 
+	def get_version(self) -> str:
+		"""SCPI: DIAGnostic:GPRF:MEASurement:VERSion \n
+		Snippet: value: str = driver.diagnostic.gprf.measurement.get_version() \n
+		No command help available \n
+			:return: version: No help available
+		"""
+		response = self._core.io.query_str('DIAGnostic:GPRF:MEASurement:VERSion?')
+		return trim_str_response(response)
+
 	def clone(self) -> 'MeasurementCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = MeasurementCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Gprf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class GprfCls:
-	"""Gprf commands group definition. 28 total commands, 2 Subgroups, 0 group commands"""
+	"""Gprf commands group definition. 29 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("gprf", core, parent)
 
 	@property
 	def generator(self):
@@ -16,15 +16,15 @@
 		if not hasattr(self, '_generator'):
 			from .Generator import GeneratorCls
 			self._generator = GeneratorCls(self._core, self._cmd_group)
 		return self._generator
 
 	@property
 	def measurement(self):
-		"""measurement commands group. 3 Sub-classes, 2 commands."""
+		"""measurement commands group. 3 Sub-classes, 3 commands."""
 		if not hasattr(self, '_measurement'):
 			from .Measurement import MeasurementCls
 			self._measurement = MeasurementCls(self._core, self._cmd_group)
 		return self._measurement
 
 	def clone(self) -> 'GprfCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Meas/Scpi.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/Scpi.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Meas/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Meas/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Generator.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Generator.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Measurement.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/Measurement.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/NrMmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/Measurement.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/Uwb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Route/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Route/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/Output.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/Output.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/Debug/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/Add/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class AddCls:
-	"""Add commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
+class TenvironmentCls:
+	"""Tenvironment commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("add", core, parent)
+		self._cmd_group = CommandsGroup("tenvironment", core, parent)
 
 	@property
-	def debug(self):
-		"""debug commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_debug'):
-			from .Debug import DebugCls
-			self._debug = DebugCls(self._core, self._cmd_group)
-		return self._debug
+	def spath(self):
+		"""spath commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_spath'):
+			from .Spath import SpathCls
+			self._spath = SpathCls(self._core, self._cmd_group)
+		return self._spath
 
-	def clone(self) -> 'AddCls':
+	def clone(self) -> 'TenvironmentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = AddCls(self._core, self._cmd_group.parent)
+		new_group = TenvironmentCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Trigger/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Diagnostic/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class DiagnosticCls:
-	"""Diagnostic commands group definition. 56 total commands, 8 Subgroups, 0 group commands"""
+	"""Diagnostic commands group definition. 58 total commands, 8 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("diagnostic", core, parent)
 
 	@property
 	def gprf(self):
 		"""gprf commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_gprf'):
 			from .Gprf import GprfCls
 			self._gprf = GprfCls(self._core, self._cmd_group)
 		return self._gprf
 
 	@property
+	def configure(self):
+		"""configure commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_configure'):
+			from .Configure import ConfigureCls
+			self._configure = ConfigureCls(self._core, self._cmd_group)
+		return self._configure
+
+	@property
 	def generic(self):
 		"""generic commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_generic'):
 			from .Generic import GenericCls
 			self._generic = GenericCls(self._core, self._cmd_group)
 		return self._generic
 
@@ -39,22 +47,14 @@
 		"""fetch commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_fetch'):
 			from .Fetch import FetchCls
 			self._fetch = FetchCls(self._core, self._cmd_group)
 		return self._fetch
 
 	@property
-	def configure(self):
-		"""configure commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_configure'):
-			from .Configure import ConfigureCls
-			self._configure = ConfigureCls(self._core, self._cmd_group)
-		return self._configure
-
-	@property
 	def route(self):
 		"""route commands group. 3 Sub-classes, 0 commands."""
 		if not hasattr(self, '_route'):
 			from .Route import RouteCls
 			self._route = RouteCls(self._core, self._cmd_group)
 		return self._route
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Canalyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/ExtPwrSensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Icomponent.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Icomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Peaks/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Qcomponent.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/Qcomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/FftSpecAn/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Bin.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Bin.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Reliability.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/SymbolRate.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Talignment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/Talignment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqRecorder/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/FreqError.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/FreqError.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Icomponent.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Icomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Level.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Level.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/OfError.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/OfError.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Phase.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Phase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Qcomponent.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/Qcomponent.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/IqVsSlot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/Power.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/Sensor/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Nrpm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,61 +1,66 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class PlossCls:
-	"""Ploss commands group definition. 9 total commands, 3 Subgroups, 2 group commands"""
+class EvaluateCls:
+	"""Evaluate commands group definition. 6 total commands, 4 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("ploss", core, parent)
+		self._cmd_group = CommandsGroup("evaluate", core, parent)
 
 	@property
 	def state(self):
-		"""state commands group. 1 Sub-classes, 1 commands."""
+		"""state commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_state'):
 			from .State import StateCls
 			self._state = StateCls(self._core, self._cmd_group)
 		return self._state
 
 	@property
-	def clear(self):
-		"""clear commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_clear'):
-			from .Clear import ClearCls
-			self._clear = ClearCls(self._core, self._cmd_group)
-		return self._clear
+	def gain(self):
+		"""gain commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_gain'):
+			from .Gain import GainCls
+			self._gain = GainCls(self._core, self._cmd_group)
+		return self._gain
 
 	@property
-	def eeprom(self):
-		"""eeprom commands group. 4 Sub-classes, 0 commands."""
-		if not hasattr(self, '_eeprom'):
-			from .Eeprom import EepromCls
-			self._eeprom = EepromCls(self._core, self._cmd_group)
-		return self._eeprom
-
-	def stop(self, opc_timeout_ms: int = -1) -> None:
-		"""SCPI: STOP:GPRF:MEASurement<Instance>:PLOSs \n
-		Snippet: driver.gprf.measurement.ploss.stop() \n
-			INTRO_CMD_HELP: Stops or aborts the measurement: \n
-			- STOP...: The measurement enters the 'RDY' state. The resources remain allocated to the measurement.
-			- ABORt...: The measurement enters the 'OFF' state. Allocated resources are released.  \n
-			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
-		self._core.io.write_with_opc(f'STOP:GPRF:MEASurement<Instance>:PLOSs', opc_timeout_ms)
+	def frequency(self):
+		"""frequency commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_frequency'):
+			from .Frequency import FrequencyCls
+			self._frequency = FrequencyCls(self._core, self._cmd_group)
+		return self._frequency
 
-	def abort(self, opc_timeout_ms: int = -1) -> None:
-		"""SCPI: ABORt:GPRF:MEASurement<Instance>:PLOSs \n
-		Snippet: driver.gprf.measurement.ploss.abort() \n
-			INTRO_CMD_HELP: Stops or aborts the measurement: \n
-			- STOP...: The measurement enters the 'RDY' state. The resources remain allocated to the measurement.
-			- ABORt...: The measurement enters the 'OFF' state. Allocated resources are released.  \n
+	@property
+	def trace(self):
+		"""trace commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_trace'):
+			from .Trace import TraceCls
+			self._trace = TraceCls(self._core, self._cmd_group)
+		return self._trace
+
+	def initiate(self) -> None:
+		"""SCPI: INITiate:GPRF:MEASurement<instance>:PLOSs:EVALuate \n
+		Snippet: driver.gprf.measurement.ploss.evaluate.initiate() \n
+		Selects a measurement step according to the last mnemonic (Open, Short or Evaluation) and starts the measurement. \n
+		"""
+		self._core.io.write(f'INITiate:GPRF:MEASurement<Instance>:PLOSs:EVALuate')
+
+	def initiate_with_opc(self, opc_timeout_ms: int = -1) -> None:
+		"""SCPI: INITiate:GPRF:MEASurement<instance>:PLOSs:EVALuate \n
+		Snippet: driver.gprf.measurement.ploss.evaluate.initiate_with_opc() \n
+		Selects a measurement step according to the last mnemonic (Open, Short or Evaluation) and starts the measurement. \n
+		Same as initiate, but waits for the operation to complete before continuing further. Use the RsCMPX_Gprf.utilities.opc_timeout_set() to set the timeout value. \n
 			:param opc_timeout_ms: Maximum time to wait in milliseconds, valid only for this call."""
-		self._core.io.write_with_opc(f'ABORt:GPRF:MEASurement<Instance>:PLOSs', opc_timeout_ms)
+		self._core.io.write_with_opc(f'INITiate:GPRF:MEASurement<Instance>:PLOSs:EVALuate', opc_timeout_ms)
 
-	def clone(self) -> 'PlossCls':
+	def clone(self) -> 'EvaluateCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = PlossCls(self._core, self._cmd_group.parent)
+		new_group = EvaluateCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Power.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Power.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Probability.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Probability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Sample.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/Sample.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/CumulativeDistribFnc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Rms.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/Rms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Current/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/Bin.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/Bin.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqData/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Maximum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Minimum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/StandardDev.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/StandardDev.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Maximum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Minimum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Peak/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/StandardDev/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Average/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/Npeak.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/Npeak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Marker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Maximum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Minimum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Npeak.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Npeak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Speak.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/Speak.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/ReferenceMarker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Rms/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Average.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Average.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Maximum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Maximum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Minimum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/Minimum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/Sample/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/Spectrum/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/Measurement/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class MeasurementCls:
-	"""Measurement commands group definition. 201 total commands, 9 Subgroups, 0 group commands"""
+	"""Measurement commands group definition. 213 total commands, 9 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("measurement", core, parent)
 
 	@property
 	def power(self):
@@ -72,15 +72,15 @@
 		if not hasattr(self, '_canalyzer'):
 			from .Canalyzer import CanalyzerCls
 			self._canalyzer = CanalyzerCls(self._core, self._cmd_group)
 		return self._canalyzer
 
 	@property
 	def ploss(self):
-		"""ploss commands group. 3 Sub-classes, 2 commands."""
+		"""ploss commands group. 7 Sub-classes, 2 commands."""
 		if not hasattr(self, '_ploss'):
 			from .Ploss import PlossCls
 			self._ploss = PlossCls(self._core, self._cmd_group)
 		return self._ploss
 
 	def clone(self) -> 'MeasurementCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Gprf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class GprfCls:
-	"""Gprf commands group definition. 201 total commands, 1 Subgroups, 0 group commands"""
+	"""Gprf commands group definition. 213 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("gprf", core, parent)
 
 	@property
 	def measurement(self):
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Modify/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Modify/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/System/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Rx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Rx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Tx.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/Tx.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/Tenvironment/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from ....Internal.Core import Core
-from ....Internal.CommandsGroup import CommandsGroup
+from ...Internal.Core import Core
+from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class TenvironmentCls:
-	"""Tenvironment commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
+	"""Tenvironment commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("tenvironment", core, parent)
 
 	@property
 	def spath(self):
-		"""spath commands group. 1 Sub-classes, 0 commands."""
+		"""spath commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_spath'):
 			from .Spath import SpathCls
 			self._spath = SpathCls(self._core, self._cmd_group)
 		return self._spath
 
 	def clone(self) -> 'TenvironmentCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Remove/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Remove/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/Current.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/Current.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/Power/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Results/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Results/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Bluetooth/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Cdma/Measurement.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Cdma/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Cdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/RfSettings.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/Group.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/Group.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/RfSettings.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Gsm/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Gsm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Lte/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Lte/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/LteDl/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/LteDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Niot/Measurement.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/Measurement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Niot/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Niot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrDl/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrMmw/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrMmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/NrSub/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/NrSub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Uwb/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Uwb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wcdma/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wcdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wlan/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wlan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/Wpan/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/Wpan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Route/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Route/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/Base/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/Base/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Sense/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from .......Internal.Core import Core
+from .......Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SenseCls:
-	"""Sense commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
+class ManualCls:
+	"""Manual commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("sense", core, parent)
+		self._cmd_group = CommandsGroup("manual", core, parent)
 
 	@property
-	def base(self):
-		"""base commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_base'):
-			from .Base import BaseCls
-			self._base = BaseCls(self._core, self._cmd_group)
-		return self._base
+	def execute(self):
+		"""execute commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_execute'):
+			from .Execute import ExecuteCls
+			self._execute = ExecuteCls(self._core, self._cmd_group)
+		return self._execute
 
-	def clone(self) -> 'SenseCls':
+	def clone(self) -> 'ManualCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = SenseCls(self._core, self._cmd_group.parent)
+		new_group = ManualCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/Delays.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/Delays.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Marker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Msegment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Msegment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/Range.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/Range.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Samples/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Segments.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/Segments.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/Clist.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/Clist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/UdMarker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Level.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Level.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Ofrequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/Ofrequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Dtone/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dgain.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dtime.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Dtime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Esingle.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Esingle.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Fill.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Fill.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/Enabling.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/Enabling.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Increment/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Irepetition.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Irepetition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Modulation.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Modulation.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Reenabling.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Reenabling.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/RfLevel.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/RfLevel.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Rlist.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Rlist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Slist.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Slist.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Sstop.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/Sstop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Check.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Check.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/CrcProtect.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/CrcProtect.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Download.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Download.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Duration.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Duration.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Paratio.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Paratio.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Path.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Path.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Poffset.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Poffset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Reliability.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Rmessage.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Rmessage.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Roption.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Roption.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Samples.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Samples.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/SymbolRate.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Waveform.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/Waveform.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Apool/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/Ofrequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/Ofrequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Dtone/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Acycles.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Acycles.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dgain.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dtime.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Dtime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Call.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Call.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Insert.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Insert.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mdown.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mdown.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mup.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/Mup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Entry/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Apply.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Apply.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Dgain.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Dgain.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Lrms.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/Lrms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Fill/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Frequency.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Frequency.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Itransition.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Itransition.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lincrement.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lincrement.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lrms.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Lrms.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Cw.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Cw.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Dtone.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Dtone.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Off.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/Off.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/All/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Index/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Range.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/Range.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Signal/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/Single.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/Single.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/Tx/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/Bench/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/Usage/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Spath/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/SymbolRate.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/SymbolRate.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Ttime.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/Ttime.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/ListPy/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/Delays/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Marker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Reliability.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Reliability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/RfSettings/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Rmarker.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Rmarker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Tdd.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Tdd.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/Delay/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/Wmarker/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Sequencer/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/All.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/All.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/State/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Source/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Source/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Globale.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Tenvironment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/All/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Globale.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Globale.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Tenvironment.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/Tenvironment.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/CorrectionTable/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Attenuation/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Attenuation/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Date/Local.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/Local.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Date/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Date/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Time/Local.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/Local.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/Time/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/System/Time/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/System/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,43 +1,35 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class SystemCls:
-	"""System commands group definition. 8 total commands, 3 Subgroups, 0 group commands"""
+class ConfigureCls:
+	"""Configure commands group definition. 19 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("system", core, parent)
+		self._cmd_group = CommandsGroup("configure", core, parent)
 
 	@property
-	def attenuation(self):
-		"""attenuation commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_attenuation'):
-			from .Attenuation import AttenuationCls
-			self._attenuation = AttenuationCls(self._core, self._cmd_group)
-		return self._attenuation
+	def gprf(self):
+		"""gprf commands group. 1 Sub-classes, 0 commands."""
+		if not hasattr(self, '_gprf'):
+			from .Gprf import GprfCls
+			self._gprf = GprfCls(self._core, self._cmd_group)
+		return self._gprf
 
 	@property
-	def time(self):
-		"""time commands group. 1 Sub-classes, 2 commands."""
-		if not hasattr(self, '_time'):
-			from .Time import TimeCls
-			self._time = TimeCls(self._core, self._cmd_group)
-		return self._time
+	def system(self):
+		"""system commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_system'):
+			from .System import SystemCls
+			self._system = SystemCls(self._core, self._cmd_group)
+		return self._system
 
-	@property
-	def date(self):
-		"""date commands group. 1 Sub-classes, 0 commands."""
-		if not hasattr(self, '_date'):
-			from .Date import DateCls
-			self._date = DateCls(self._core, self._cmd_group)
-		return self._date
-
-	def clone(self) -> 'SystemCls':
+	def clone(self) -> 'ConfigureCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = SystemCls(self._core, self._cmd_group.parent)
+		new_group = ConfigureCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Tenvironment/Spath.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Tenvironment/Spath.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Tenvironment/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Sense/System/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from ...Internal.Core import Core
-from ...Internal.CommandsGroup import CommandsGroup
+from ....Internal.Core import Core
+from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class TenvironmentCls:
-	"""Tenvironment commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
+class SystemCls:
+	"""System commands group definition. 2 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("tenvironment", core, parent)
+		self._cmd_group = CommandsGroup("system", core, parent)
 
 	@property
-	def spath(self):
-		"""spath commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_spath'):
-			from .Spath import SpathCls
-			self._spath = SpathCls(self._core, self._cmd_group)
-		return self._spath
+	def positioner(self):
+		"""positioner commands group. 2 Sub-classes, 0 commands."""
+		if not hasattr(self, '_positioner'):
+			from .Positioner import PositionerCls
+			self._positioner = PositionerCls(self._core, self._cmd_group)
+		return self._positioner
 
-	def clone(self) -> 'TenvironmentCls':
+	def clone(self) -> 'SystemCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = TenvironmentCls(self._core, self._cmd_group.parent)
+		new_group = SystemCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/BhRate/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdr/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/Hdrp/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
+from ......Internal.Utilities import trim_str_response
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class ArbCls:
-	"""Arb commands group definition. 7 total commands, 2 Subgroups, 4 group commands"""
+	"""Arb commands group definition. 9 total commands, 3 Subgroups, 5 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("arb", core, parent)
 
 	@property
 	def manual(self):
@@ -24,14 +25,22 @@
 	def segments(self):
 		"""segments commands group. 1 Sub-classes, 1 commands."""
 		if not hasattr(self, '_segments'):
 			from .Segments import SegmentsCls
 			self._segments = SegmentsCls(self._core, self._cmd_group)
 		return self._segments
 
+	@property
+	def catalog(self):
+		"""catalog commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_catalog'):
+			from .Catalog import CatalogCls
+			self._catalog = CatalogCls(self._core, self._cmd_group)
+		return self._catalog
+
 	def get_delay(self) -> float:
 		"""SCPI: TRIGger:GPRF:GENerator<Instance>:ARB:DELay \n
 		Snippet: value: float = driver.trigger.gprf.generator.arb.get_delay() \n
 		Sets the trigger delay. \n
 			:return: delay: No help available
 		"""
 		response = self._core.io.query_str('TRIGger:GPRF:GENerator<Instance>:ARB:DELay?')
@@ -97,14 +106,34 @@
 		Snippet: driver.trigger.gprf.generator.arb.set_autostart(autostart = False) \n
 		No command help available \n
 			:param autostart: No help available
 		"""
 		param = Conversions.bool_to_str(autostart)
 		self._core.io.write(f'TRIGger:GPRF:GENerator<Instance>:ARB:AUTostart {param}')
 
+	def get_source(self) -> str:
+		"""SCPI: TRIGger:GPRF:GENerator<Instance>[:ARB]:SOURce \n
+		Snippet: value: str = driver.trigger.gprf.generator.arb.get_source() \n
+		Selects the source of the trigger events. The supported values depend on the installed options. You can query a list of
+		all supported values via method RsCMPX_Gprf.Trigger.Gprf.Generator.Arb.Catalog.source. \n
+			:return: trigger: No help available
+		"""
+		response = self._core.io.query_str('TRIGger:GPRF:GENerator<Instance>:ARB:SOURce?')
+		return trim_str_response(response)
+
+	def set_source(self, trigger: str) -> None:
+		"""SCPI: TRIGger:GPRF:GENerator<Instance>[:ARB]:SOURce \n
+		Snippet: driver.trigger.gprf.generator.arb.set_source(trigger = 'abc') \n
+		Selects the source of the trigger events. The supported values depend on the installed options. You can query a list of
+		all supported values via method RsCMPX_Gprf.Trigger.Gprf.Generator.Arb.Catalog.source. \n
+			:param trigger: No help available
+		"""
+		param = Conversions.value_to_quoted_str(trigger)
+		self._core.io.write(f'TRIGger:GPRF:GENerator<Instance>:ARB:SOURce {param}')
+
 	def clone(self) -> 'ArbCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = ArbCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from .......Internal.Core import Core
-from .......Internal.CommandsGroup import CommandsGroup
+from .....Internal.Core import Core
+from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
-class ManualCls:
-	"""Manual commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
+class GprfCls:
+	"""Gprf commands group definition. 1 total commands, 1 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
-		self._cmd_group = CommandsGroup("manual", core, parent)
+		self._cmd_group = CommandsGroup("gprf", core, parent)
 
 	@property
-	def execute(self):
-		"""execute commands group. 0 Sub-classes, 1 commands."""
-		if not hasattr(self, '_execute'):
-			from .Execute import ExecuteCls
-			self._execute = ExecuteCls(self._core, self._cmd_group)
-		return self._execute
+	def measurement(self):
+		"""measurement commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_measurement'):
+			from .Measurement import MeasurementCls
+			self._measurement = MeasurementCls(self._core, self._cmd_group)
+		return self._measurement
 
-	def clone(self) -> 'ManualCls':
+	def clone(self) -> 'GprfCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
-		new_group = ManualCls(self._core, self._cmd_group.parent)
+		new_group = GprfCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class SequencerCls:
-	"""Sequencer commands group definition. 2 total commands, 1 Subgroups, 1 group commands"""
+	"""Sequencer commands group definition. 6 total commands, 3 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("sequencer", core, parent)
 
 	@property
 	def manual(self):
 		"""manual commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_manual'):
 			from .Manual import ManualCls
 			self._manual = ManualCls(self._core, self._cmd_group)
 		return self._manual
 
+	@property
+	def isMeas(self):
+		"""isMeas commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_isMeas'):
+			from .IsMeas import IsMeasCls
+			self._isMeas = IsMeasCls(self._core, self._cmd_group)
+		return self._isMeas
+
+	@property
+	def isTrigger(self):
+		"""isTrigger commands group. 0 Sub-classes, 2 commands."""
+		if not hasattr(self, '_isTrigger'):
+			from .IsTrigger import IsTriggerCls
+			self._isTrigger = IsTriggerCls(self._core, self._cmd_group)
+		return self._isTrigger
+
 	def get_timeout(self) -> float or bool:
 		"""SCPI: TRIGger:GPRF:GENerator<Instance>:SEQuencer:TOUT \n
 		Snippet: value: float or bool = driver.trigger.gprf.generator.sequencer.get_timeout() \n
 		Sets a timeout for waiting for a trigger event for List Increment = MEASUREMENT and TRIGGER. \n
 			:return: timeout: (float or boolean) No help available
 		"""
 		response = self._core.io.query_str('TRIGger:GPRF:GENerator<Instance>:SEQuencer:TOUT?')
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 from .....Internal import Conversions
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class GeneratorCls:
-	"""Generator commands group definition. 10 total commands, 2 Subgroups, 1 group commands"""
+	"""Generator commands group definition. 16 total commands, 2 Subgroups, 1 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("generator", core, parent)
 
 	@property
 	def arb(self):
-		"""arb commands group. 2 Sub-classes, 4 commands."""
+		"""arb commands group. 3 Sub-classes, 5 commands."""
 		if not hasattr(self, '_arb'):
 			from .Arb import ArbCls
 			self._arb = ArbCls(self._core, self._cmd_group)
 		return self._arb
 
 	@property
 	def sequencer(self):
-		"""sequencer commands group. 1 Sub-classes, 1 commands."""
+		"""sequencer commands group. 3 Sub-classes, 1 commands."""
 		if not hasattr(self, '_sequencer'):
 			from .Sequencer import SequencerCls
 			self._sequencer = SequencerCls(self._core, self._cmd_group)
 		return self._sequencer
 
 	def get_timeout(self) -> float or bool:
 		"""SCPI: TRIGger:GPRF:GENerator<Instance>:TOUT \n
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
+from ......Internal.Utilities import trim_str_response
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class FftSpecAnCls:
-	"""FftSpecAn commands group definition. 7 total commands, 1 Subgroups, 6 group commands"""
+	"""FftSpecAn commands group definition. 9 total commands, 2 Subgroups, 7 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("fftSpecAn", core, parent)
 
 	@property
 	def osStop(self):
 		"""osStop commands group. 0 Sub-classes, 1 commands."""
 		if not hasattr(self, '_osStop'):
 			from .OsStop import OsStopCls
 			self._osStop = OsStopCls(self._core, self._cmd_group)
 		return self._osStop
 
+	@property
+	def catalog(self):
+		"""catalog commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_catalog'):
+			from .Catalog import CatalogCls
+			self._catalog = CatalogCls(self._core, self._cmd_group)
+		return self._catalog
+
 	# noinspection PyTypeChecker
 	def get_omode(self) -> enums.OffsetMode:
 		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:FFTSanalyzer:OMODe \n
 		Snippet: value: enums.OffsetMode = driver.trigger.gprf.measurement.fftSpecAn.get_omode() \n
 		Selects the trigger offset mode. \n
 			:return: offset_mode: No help available
 		"""
@@ -134,14 +143,36 @@
 		Qualifies whether the trigger event is generated at the rising or at the falling edge of the trigger pulse (valid for
 		external and power trigger sources) . \n
 			:param event: REDGe: rising edge FEDGe: falling edge
 		"""
 		param = Conversions.enum_scalar_to_str(event, enums.SignalSlopeExt)
 		self._core.io.write(f'TRIGger:GPRF:MEASurement<Instance>:FFTSanalyzer:SLOPe {param}')
 
+	def get_source(self) -> str:
+		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:FFTSanalyzer:SOURce \n
+		Snippet: value: str = driver.trigger.gprf.measurement.fftSpecAn.get_source() \n
+		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
+		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
+		:CATalog:SOURce?. \n
+			:return: trigger: No help available
+		"""
+		response = self._core.io.query_str('TRIGger:GPRF:MEASurement<Instance>:FFTSanalyzer:SOURce?')
+		return trim_str_response(response)
+
+	def set_source(self, trigger: str) -> None:
+		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:FFTSanalyzer:SOURce \n
+		Snippet: driver.trigger.gprf.measurement.fftSpecAn.set_source(trigger = 'abc') \n
+		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
+		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
+		:CATalog:SOURce?. \n
+			:param trigger: 'IF Power': IF power trigger 'Free Run': free run (untriggered)
+		"""
+		param = Conversions.value_to_quoted_str(trigger)
+		self._core.io.write(f'TRIGger:GPRF:MEASurement<Instance>:FFTSanalyzer:SOURce {param}')
+
 	def clone(self) -> 'FftSpecAnCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = FftSpecAnCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal import Conversions
-from ..... import enums
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ......Internal.Utilities import trim_str_response
+from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class IqRecorderCls:
-	"""IqRecorder commands group definition. 7 total commands, 0 Subgroups, 7 group commands"""
+	"""IqRecorder commands group definition. 9 total commands, 1 Subgroups, 8 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("iqRecorder", core, parent)
 
+	@property
+	def catalog(self):
+		"""catalog commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_catalog'):
+			from .Catalog import CatalogCls
+			self._catalog = CatalogCls(self._core, self._cmd_group)
+		return self._catalog
+
 	def get_offset(self) -> int:
 		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:IQRecorder:OFFSet \n
 		Snippet: value: int = driver.trigger.gprf.measurement.iqRecorder.get_offset() \n
 		Defines a delay time for triggered measurements. The trigger offset delays the start of the measurement relative to the
 		trigger event. \n
 			:return: trigger_offset: Trigger offset in samples.
 		"""
@@ -150,7 +159,37 @@
 		Snippet: driver.trigger.gprf.measurement.iqRecorder.set_slope(event = enums.SignalSlopeExt.FALLing) \n
 		Qualifies whether the trigger event is generated at the rising or at the falling edge of the trigger pulse (valid for
 		external and power trigger sources) . \n
 			:param event: REDGe: rising edge FEDGe: falling edge
 		"""
 		param = Conversions.enum_scalar_to_str(event, enums.SignalSlopeExt)
 		self._core.io.write(f'TRIGger:GPRF:MEASurement<Instance>:IQRecorder:SLOPe {param}')
+
+	def get_source(self) -> str:
+		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:IQRecorder:SOURce \n
+		Snippet: value: str = driver.trigger.gprf.measurement.iqRecorder.get_source() \n
+		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
+		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
+		:CATalog:SOURce?. \n
+			:return: trigger: No help available
+		"""
+		response = self._core.io.query_str('TRIGger:GPRF:MEASurement<Instance>:IQRecorder:SOURce?')
+		return trim_str_response(response)
+
+	def set_source(self, trigger: str) -> None:
+		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:IQRecorder:SOURce \n
+		Snippet: driver.trigger.gprf.measurement.iqRecorder.set_source(trigger = 'abc') \n
+		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
+		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
+		:CATalog:SOURce?. \n
+			:param trigger: 'IF Power': IF power trigger 'Free Run': free run (untriggered) 'Phase Change': phase change trigger
+		"""
+		param = Conversions.value_to_quoted_str(trigger)
+		self._core.io.write(f'TRIGger:GPRF:MEASurement<Instance>:IQRecorder:SOURce {param}')
+
+	def clone(self) -> 'IqRecorderCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
+		Also copies all the existing default Repeated Capabilities setting,
+		which you can change independently without affecting the original group"""
+		new_group = IqRecorderCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
+		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-from .....Internal.Core import Core
-from .....Internal.CommandsGroup import CommandsGroup
-from .....Internal import Conversions
-from ..... import enums
+from ......Internal.Core import Core
+from ......Internal.CommandsGroup import CommandsGroup
+from ......Internal import Conversions
+from ......Internal.Utilities import trim_str_response
+from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class IqVsSlotCls:
-	"""IqVsSlot commands group definition. 6 total commands, 0 Subgroups, 6 group commands"""
+	"""IqVsSlot commands group definition. 8 total commands, 1 Subgroups, 7 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("iqVsSlot", core, parent)
 
+	@property
+	def catalog(self):
+		"""catalog commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_catalog'):
+			from .Catalog import CatalogCls
+			self._catalog = CatalogCls(self._core, self._cmd_group)
+		return self._catalog
+
 	def get_mgap(self) -> float:
 		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:IQVSlot:MGAP \n
 		Snippet: value: float = driver.trigger.gprf.measurement.iqVsSlot.get_mgap() \n
 		Sets a minimum time during which the IF signal must be below the trigger threshold before the trigger is armed so that an
 		IF power trigger event can be generated. \n
 			:return: minimum_gap: No help available
 		"""
@@ -127,7 +136,37 @@
 		Snippet: driver.trigger.gprf.measurement.iqVsSlot.set_mode(mode = enums.TriggerSequenceMode.ONCE) \n
 		Selects the measurement sequence that is triggered by each single trigger event. This setting is not valid for free run
 		measurements. \n
 			:param mode: ONCE: Trigger Once PRESelect: Retrigger Preselect
 		"""
 		param = Conversions.enum_scalar_to_str(mode, enums.TriggerSequenceMode)
 		self._core.io.write(f'TRIGger:GPRF:MEASurement<Instance>:IQVSlot:MODE {param}')
+
+	def get_source(self) -> str:
+		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:IQVSlot:SOURce \n
+		Snippet: value: str = driver.trigger.gprf.measurement.iqVsSlot.get_source() \n
+		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
+		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
+		:CATalog:SOURce?. \n
+			:return: trigger: No help available
+		"""
+		response = self._core.io.query_str('TRIGger:GPRF:MEASurement<Instance>:IQVSlot:SOURce?')
+		return trim_str_response(response)
+
+	def set_source(self, trigger: str) -> None:
+		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:IQVSlot:SOURce \n
+		Snippet: driver.trigger.gprf.measurement.iqVsSlot.set_source(trigger = 'abc') \n
+		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
+		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
+		:CATalog:SOURce?. \n
+			:param trigger: 'IF Power': IF power trigger 'Free Run': free run (untriggered)
+		"""
+		param = Conversions.value_to_quoted_str(trigger)
+		self._core.io.write(f'TRIGger:GPRF:MEASurement<Instance>:IQVSlot:SOURce {param}')
+
+	def clone(self) -> 'IqVsSlotCls':
+		"""Clones the group by creating new object from it and its whole existing subgroups
+		Also copies all the existing default Repeated Capabilities setting,
+		which you can change independently without affecting the original group"""
+		new_group = IqVsSlotCls(self._core, self._cmd_group.parent)
+		self._cmd_group.synchronize_repcaps(new_group)
+		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 from ......Internal.Core import Core
 from ......Internal.CommandsGroup import CommandsGroup
 from ......Internal import Conversions
+from ......Internal.Utilities import trim_str_response
 from ...... import enums
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class PowerCls:
-	"""Power commands group definition. 8 total commands, 1 Subgroups, 6 group commands"""
+	"""Power commands group definition. 10 total commands, 2 Subgroups, 7 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("power", core, parent)
 
 	@property
 	def parameterSetList(self):
 		"""parameterSetList commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_parameterSetList'):
 			from .ParameterSetList import ParameterSetListCls
 			self._parameterSetList = ParameterSetListCls(self._core, self._cmd_group)
 		return self._parameterSetList
 
+	@property
+	def catalog(self):
+		"""catalog commands group. 0 Sub-classes, 1 commands."""
+		if not hasattr(self, '_catalog'):
+			from .Catalog import CatalogCls
+			self._catalog = CatalogCls(self._core, self._cmd_group)
+		return self._catalog
+
 	def get_mgap(self) -> float:
 		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:POWer:MGAP \n
 		Snippet: value: float = driver.trigger.gprf.measurement.power.get_mgap() \n
 		Sets a minimum time during which the IF signal must be below the trigger threshold before the trigger is armed so that an
 		IF power trigger event can be generated. \n
 			:return: minimum_gap: No help available
 		"""
@@ -136,14 +145,36 @@
 		Qualifies whether the trigger event is generated at the rising or at the falling edge of the trigger pulse (valid for
 		external and power trigger sources) . \n
 			:param event: REDGe: rising edge FEDGe: falling edge
 		"""
 		param = Conversions.enum_scalar_to_str(event, enums.SignalSlopeExt)
 		self._core.io.write(f'TRIGger:GPRF:MEASurement<Instance>:POWer:SLOPe {param}')
 
+	def get_source(self) -> str:
+		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:POWer:SOURce \n
+		Snippet: value: str = driver.trigger.gprf.measurement.power.get_source() \n
+		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
+		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
+		:CATalog:SOURce?. \n
+			:return: trigger: No help available
+		"""
+		response = self._core.io.query_str('TRIGger:GPRF:MEASurement<Instance>:POWer:SOURce?')
+		return trim_str_response(response)
+
+	def set_source(self, trigger: str) -> None:
+		"""SCPI: TRIGger:GPRF:MEASurement<Instance>:POWer:SOURce \n
+		Snippet: driver.trigger.gprf.measurement.power.set_source(trigger = 'abc') \n
+		Selects the source of the trigger events. Some values are always available. They are listed below. Depending on the
+		installed options, additional values are available. You can query a list of all supported values via TRIGger:...
+		:CATalog:SOURce?. \n
+			:param trigger: 'IF Power': IF power trigger 'Free Run': free run (untriggered)
+		"""
+		param = Conversions.value_to_quoted_str(trigger)
+		self._core.io.write(f'TRIGger:GPRF:MEASurement<Instance>:POWer:SOURce {param}')
+
 	def clone(self) -> 'PowerCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
 		Also copies all the existing default Repeated Capabilities setting,
 		which you can change independently without affecting the original group"""
 		new_group = PowerCls(self._core, self._cmd_group.parent)
 		self._cmd_group.synchronize_repcaps(new_group)
 		return new_group
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from .....Internal.Core import Core
 from .....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class MeasurementCls:
-	"""Measurement commands group definition. 33 total commands, 5 Subgroups, 0 group commands"""
+	"""Measurement commands group definition. 41 total commands, 5 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("measurement", core, parent)
 
 	@property
 	def power(self):
-		"""power commands group. 1 Sub-classes, 6 commands."""
+		"""power commands group. 2 Sub-classes, 7 commands."""
 		if not hasattr(self, '_power'):
 			from .Power import PowerCls
 			self._power = PowerCls(self._core, self._cmd_group)
 		return self._power
 
 	@property
 	def iqVsSlot(self):
-		"""iqVsSlot commands group. 0 Sub-classes, 6 commands."""
+		"""iqVsSlot commands group. 1 Sub-classes, 7 commands."""
 		if not hasattr(self, '_iqVsSlot'):
 			from .IqVsSlot import IqVsSlotCls
 			self._iqVsSlot = IqVsSlotCls(self._core, self._cmd_group)
 		return self._iqVsSlot
 
 	@property
 	def iqRecorder(self):
-		"""iqRecorder commands group. 0 Sub-classes, 7 commands."""
+		"""iqRecorder commands group. 1 Sub-classes, 8 commands."""
 		if not hasattr(self, '_iqRecorder'):
 			from .IqRecorder import IqRecorderCls
 			self._iqRecorder = IqRecorderCls(self._core, self._cmd_group)
 		return self._iqRecorder
 
 	@property
 	def spectrum(self):
@@ -40,15 +40,15 @@
 		if not hasattr(self, '_spectrum'):
 			from .Spectrum import SpectrumCls
 			self._spectrum = SpectrumCls(self._core, self._cmd_group)
 		return self._spectrum
 
 	@property
 	def fftSpecAn(self):
-		"""fftSpecAn commands group. 1 Sub-classes, 6 commands."""
+		"""fftSpecAn commands group. 2 Sub-classes, 7 commands."""
 		if not hasattr(self, '_fftSpecAn'):
 			from .FftSpecAn import FftSpecAnCls
 			self._fftSpecAn = FftSpecAnCls(self._core, self._cmd_group)
 		return self._fftSpecAn
 
 	def clone(self) -> 'MeasurementCls':
 		"""Clones the group by creating new object from it and its whole existing subgroups
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ....Internal.Core import Core
 from ....Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class GprfCls:
-	"""Gprf commands group definition. 43 total commands, 2 Subgroups, 0 group commands"""
+	"""Gprf commands group definition. 57 total commands, 2 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("gprf", core, parent)
 
 	@property
 	def generator(self):
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/Srs/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Lte/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Lte/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/LteDl/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/LteDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Niot/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Niot/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrDl/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrDl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrMmw/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrMmw/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/Srs/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/NrSub/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/NrSub/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Uwb/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Uwb/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OlpControl/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/OoSync/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Prach/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/Tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wcdma/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wcdma/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wlan/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wlan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/Catalog.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/Catalog.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/MultiEval/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/Measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/Wpan/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/Wpan/__init__.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Implementations/Trigger/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Implementations/Trigger/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from ...Internal.Core import Core
 from ...Internal.CommandsGroup import CommandsGroup
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class TriggerCls:
-	"""Trigger commands group definition. 95 total commands, 14 Subgroups, 0 group commands"""
+	"""Trigger commands group definition. 109 total commands, 14 Subgroups, 0 group commands"""
 
 	def __init__(self, core: Core, parent):
 		self._core = core
 		self._cmd_group = CommandsGroup("trigger", core, parent)
 
 	@property
 	def gprf(self):
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgLinkedEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgSingle.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingle.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgSingleList.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingleList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgSingleSuppressed.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgStringComposer.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStringComposer.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgStruct.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStruct.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgStructList.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStructList.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ArgStructStringParser.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ArgStructStringParser.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/CommandsGroup.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/CommandsGroup.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Conversions.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Conversions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ConverterFromScpiString.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ConverterFromScpiString.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ConverterToScpiString.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ConverterToScpiString.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Core.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Core.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/GlobalData.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/GlobalData.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Instrument.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Instrument.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/InstrumentErrors.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentErrors.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/InstrumentOptions.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentOptions.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/InstrumentSettings.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InstrumentSettings.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/InternalLinker.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/InternalLinker.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/IoTransferEventArgs.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/IoTransferEventArgs.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/RepeatedCapability.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/RepeatedCapability.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ScpiEnums.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ScpiEnums.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/ScpiLogger.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/ScpiLogger.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/StreamReader.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StreamReader.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/StreamWriter.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StreamWriter.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/StructBase.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/StructBase.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Types.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Types.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/Utilities.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/Utilities.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaPluginSocketIo.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/VisaSession.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaSession.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/Internal/VisaSessionSim.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/Internal/VisaSessionSim.py`

 * *Files identical despite different names*

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/RsCMPX_Gprf.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/RsCMPX_Gprf.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from datetime import datetime, timedelta
 from . import repcap
 from .Internal.RepeatedCapability import RepeatedCapability
 
 
 # noinspection PyPep8Naming,PyAttributeOutsideInit,SpellCheckingInspection
 class RsCMPX_Gprf:
-	"""814 total commands, 16 Subgroups, 0 group commands"""
-	_driver_options = "SupportedInstrModels = CMX/CMP/CMW/PVT, SupportedIdnPatterns = CMX/CMP/CMW/PVT, SimulationIdnString = 'Rohde&Schwarz,CMX500,100001,5.0.90.0043'"
+	"""859 total commands, 16 Subgroups, 0 group commands"""
+	_driver_options = "SupportedInstrModels = CMX/CMP/CMW/PVT, SupportedIdnPatterns = CMX/CMP/CMW/PVT, SimulationIdnString = 'Rohde&Schwarz,CMX500,100001,5.0.91.0048'"
 	_global_logging_relative_timestamp: ClassVar[datetime] = None
 	_global_logging_target_stream: ClassVar = None
 
 	def __init__(self, resource_name: str, id_query: bool = True, reset: bool = False, options: str = None, direct_session: object = None):
 		"""Initializes new RsCMPX_Gprf session. \n
 		Parameter options tokens examples:
 			- ``Simulate=True`` - starts the session in simulation mode. Default: ``False``
@@ -44,15 +44,15 @@
 			- ``LoggingUdpPort = 49200`` - UDP port to log to. Default: 49200
 		:param resource_name: VISA resource name, e.g. 'TCPIP::192.168.2.1::INSTR'
 		:param id_query: if True, the instrument's model name is verified against the models supported by the driver and eventually throws an exception.
 		:param reset: Resets the instrument (sends *RST command) and clears its status sybsystem.
 		:param options: string tokens alternating the driver settings.
 		:param direct_session: Another driver object or pyVisa object to reuse the session instead of opening a new session."""
 		self._core = Core(resource_name, id_query, reset, RsCMPX_Gprf._driver_options, options, direct_session)
-		self._core.driver_version = '5.0.90.0043'
+		self._core.driver_version = '5.0.91.0048'
 		self._options = options
 		self._add_all_global_repcaps()
 		self._custom_properties_init()
 		self.utilities.default_instrument_setup()
 		# noinspection PyTypeChecker
 		self._cmd_group = CommandsGroup("ROOT", self._core, None)
 
@@ -124,25 +124,25 @@
 		self._core.io.reset_time_statistics()
 
 	@staticmethod
 	def assert_minimum_version(min_version: str) -> None:
 		"""Asserts that the driver version fulfills the minimum required version you have entered.
 		This way you make sure your installed driver is of the entered version or newer."""
 		min_version_list = min_version.split('.')
-		curr_version_list = '5.0.90.0043'.split('.')
+		curr_version_list = '5.0.91.0048'.split('.')
 		count_min = len(min_version_list)
 		count_curr = len(curr_version_list)
 		count = count_min if count_min < count_curr else count_curr
 		for i in range(count):
 			minimum = int(min_version_list[i])
 			curr = int(curr_version_list[i])
 			if curr > minimum:
 				break
 			if curr < minimum:
-				raise RsInstrException(f"Assertion for minimum RsCMPX_Gprf version failed. Current version: '5.0.90.0043', minimum required version: '{min_version}'")
+				raise RsInstrException(f"Assertion for minimum RsCMPX_Gprf version failed. Current version: '5.0.91.0048', minimum required version: '{min_version}'")
 
 	@staticmethod
 	def list_resources(expression: str = '?*::INSTR', visa_select: str = None) -> List[str]:
 		"""Finds all the resources defined by the expression
 			- '?*' - matches all the available instruments
 			- 'USB::?*' - matches all the USB instruments
 			- 'TCPIP::192?*' - matches all the LAN instruments with the IP address starting with 192
@@ -252,28 +252,36 @@
 		"""calibration commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_calibration'):
 			from .Implementations.Calibration import CalibrationCls
 			self._calibration = CalibrationCls(self._core, self._cmd_group)
 		return self._calibration
 
 	@property
+	def catalog(self):
+		"""catalog commands group. 16 Sub-classes, 0 commands."""
+		if not hasattr(self, '_catalog'):
+			from .Implementations.Catalog import CatalogCls
+			self._catalog = CatalogCls(self._core, self._cmd_group)
+		return self._catalog
+
+	@property
 	def sense(self):
-		"""sense commands group. 1 Sub-classes, 0 commands."""
+		"""sense commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_sense'):
 			from .Implementations.Sense import SenseCls
 			self._sense = SenseCls(self._core, self._cmd_group)
 		return self._sense
 
 	@property
-	def catalog(self):
-		"""catalog commands group. 16 Sub-classes, 0 commands."""
-		if not hasattr(self, '_catalog'):
-			from .Implementations.Catalog import CatalogCls
-			self._catalog = CatalogCls(self._core, self._cmd_group)
-		return self._catalog
+	def system(self):
+		"""system commands group. 3 Sub-classes, 0 commands."""
+		if not hasattr(self, '_system'):
+			from .Implementations.System import SystemCls
+			self._system = SystemCls(self._core, self._cmd_group)
+		return self._system
 
 	@property
 	def create(self):
 		"""create commands group. 2 Sub-classes, 0 commands."""
 		if not hasattr(self, '_create'):
 			from .Implementations.Create import CreateCls
 			self._create = CreateCls(self._core, self._cmd_group)
@@ -307,22 +315,14 @@
 	def modify(self):
 		"""modify commands group. 1 Sub-classes, 0 commands."""
 		if not hasattr(self, '_modify'):
 			from .Implementations.Modify import ModifyCls
 			self._modify = ModifyCls(self._core, self._cmd_group)
 		return self._modify
 
-	@property
-	def system(self):
-		"""system commands group. 3 Sub-classes, 0 commands."""
-		if not hasattr(self, '_system'):
-			from .Implementations.System import SystemCls
-			self._system = SystemCls(self._core, self._cmd_group)
-		return self._system
-
 	def clone(self) -> 'RsCMPX_Gprf':
 		"""Creates a deep copy of the RsCMPX_Gprf object. Also copies:
 			- All the existing Global repeated capability values
 			- All the default group repeated capabilities setting \n
 		Does not check the *IDN? response, and does not perform Reset.
 		After cloning, you can set all the repeated capabilities settings independentely from the original group.
 		Calling close() on the new object does not close the original VISA session"""
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/__init__.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """RsCMPX_Gprf instrument driver
-	:version: 5.0.90.43
+	:version: 5.0.91.48
 	:copyright: 2023 by Rohde & Schwarz GMBH & Co. KG
 	:license: MIT, see LICENSE for more details.
 """
 
-__version__ = '5.0.90.43'
+__version__ = '5.0.91.48'
 
 # Main class
 from RsCMPX_Gprf.RsCMPX_Gprf import RsCMPX_Gprf
 
 # Bin data format
 from RsCMPX_Gprf.Internal.Conversions import BinIntFormat, BinFloatFormat
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/enums.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/enums.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,21 @@
 class CcdfMode(Enum):
 	"""2 Members, POWer ... STATistic"""
 	POWer = 0
 	STATistic = 1
 
 
 # noinspection SpellCheckingInspection
+class ConnectionSource(Enum):
+	"""2 Members, GLOBal ... INDex"""
+	GLOBal = 0
+	INDex = 1
+
+
+# noinspection SpellCheckingInspection
 class Detector(Enum):
 	"""6 Members, AUTopeak ... SAMPle"""
 	AUTopeak = 0
 	AVERage = 1
 	MAXPeak = 2
 	MINPeak = 3
 	RMS = 4
@@ -262,14 +269,22 @@
 class ParameterSetMode(Enum):
 	"""2 Members, GLOBal ... LIST"""
 	GLOBal = 0
 	LIST = 1
 
 
 # noinspection SpellCheckingInspection
+class PathLossState(Enum):
+	"""3 Members, NCAP ... RDY"""
+	NCAP = 0
+	PEND = 1
+	RDY = 2
+
+
+# noinspection SpellCheckingInspection
 class PwrSensorResolution(Enum):
 	"""4 Members, PD0 ... PD3"""
 	PD0 = 0
 	PD1 = 1
 	PD2 = 2
 	PD3 = 3
 
@@ -619,14 +634,23 @@
 class TriggerSequenceMode(Enum):
 	"""2 Members, ONCE ... PRESelect"""
 	ONCE = 0
 	PRESelect = 1
 
 
 # noinspection SpellCheckingInspection
+class TriggerSource(Enum):
+	"""4 Members, EXTernal ... IFPower"""
+	EXTernal = 0
+	FREerun = 1
+	IF = 2
+	IFPower = 3
+
+
+# noinspection SpellCheckingInspection
 class TxConnector(Enum):
 	"""86 Members, I12O ... RH18"""
 	I12O = 0
 	I14O = 1
 	I16O = 2
 	I18O = 3
 	I22O = 4
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf/repcap.py` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf/repcap.py`

 * *Files 21% similar despite different names*

```diff
@@ -116,14 +116,53 @@
 	Empty = EmptyRepCap
 	Default = DefaultRepCap
 	Src1 = 1
 	Src2 = 2
 
 
 # noinspection SpellCheckingInspection
+class Index(Enum):
+	"""Repeated capability Index"""
+	Empty = EmptyRepCap
+	Default = DefaultRepCap
+	Ix1 = 1
+	Ix2 = 2
+	Ix3 = 3
+	Ix4 = 4
+	Ix5 = 5
+	Ix6 = 6
+	Ix7 = 7
+	Ix8 = 8
+	Ix9 = 9
+	Ix10 = 10
+	Ix11 = 11
+	Ix12 = 12
+	Ix13 = 13
+	Ix14 = 14
+	Ix15 = 15
+	Ix16 = 16
+	Ix17 = 17
+	Ix18 = 18
+	Ix19 = 19
+	Ix20 = 20
+	Ix21 = 21
+	Ix22 = 22
+	Ix23 = 23
+	Ix24 = 24
+	Ix25 = 25
+	Ix26 = 26
+	Ix27 = 27
+	Ix28 = 28
+	Ix29 = 29
+	Ix30 = 30
+	Ix31 = 31
+	Ix32 = 32
+
+
+# noinspection SpellCheckingInspection
 class LevelSource(Enum):
 	"""Repeated capability LevelSource"""
 	Empty = EmptyRepCap
 	Default = DefaultRepCap
 	Src1 = 1
 	Src2 = 2
 
@@ -136,14 +175,53 @@
 	Nr1 = 1
 	Nr2 = 2
 	Nr3 = 3
 	Nr4 = 4
 
 
 # noinspection SpellCheckingInspection
+class Positioner(Enum):
+	"""Repeated capability Positioner"""
+	Empty = EmptyRepCap
+	Default = DefaultRepCap
+	Ix1 = 1
+	Ix2 = 2
+	Ix3 = 3
+	Ix4 = 4
+	Ix5 = 5
+	Ix6 = 6
+	Ix7 = 7
+	Ix8 = 8
+	Ix9 = 9
+	Ix10 = 10
+	Ix11 = 11
+	Ix12 = 12
+	Ix13 = 13
+	Ix14 = 14
+	Ix15 = 15
+	Ix16 = 16
+	Ix17 = 17
+	Ix18 = 18
+	Ix19 = 19
+	Ix20 = 20
+	Ix21 = 21
+	Ix22 = 22
+	Ix23 = 23
+	Ix24 = 24
+	Ix25 = 25
+	Ix26 = 26
+	Ix27 = 27
+	Ix28 = 28
+	Ix29 = 29
+	Ix30 = 30
+	Ix31 = 31
+	Ix32 = 32
+
+
+# noinspection SpellCheckingInspection
 class Sensor(Enum):
 	"""Repeated capability Sensor"""
 	Empty = EmptyRepCap
 	Default = DefaultRepCap
 	Nr1 = 1
 	Nr2 = 2
 	Nr3 = 3
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf.egg-info/PKG-INFO` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RsCMPX-Gprf
-Version: 5.0.90
+Version: 5.0.91
 Summary: CMX/CMP/PVT Global Purpose RF Remote-control module
 Home-page: UNKNOWN
 Author: Rohde & Schwarz GmbH & Co. KG
 License: MIT
 Description: ==================================
          RsCMPX_Gprf
         ==================================
@@ -44,15 +44,18 @@
         
         Examples: https://github.com/Rohde-Schwarz/Examples/
         
         
         Version history
         ----------------
         
-        	Latest release notes summary: Update for CMP FW 5.0.90
+        	Latest release notes summary: Added missing measurement SCPI from MMI sub-system
+        
+        	Version 5.0.91
+        		- Added missing measurement SCPI from MMI sub-system
         
         	Version 5.0.90
         		- Update for CMP FW 5.0.90
         
         	Version 5.0.20
         		- Update for CMP200 5.0.20
```

### Comparing `RsCMPX_Gprf-5.0.90/RsCMPX_Gprf.egg-info/SOURCES.txt` & `RsCMPX_Gprf-5.0.91/RsCMPX_Gprf.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 RsCMPX_Gprf/Implementations/Catalog/Cdma/__init__.py
 RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/Spath.py
 RsCMPX_Gprf/Implementations/Catalog/Cdma/Measurement/__init__.py
 RsCMPX_Gprf/Implementations/Catalog/Gprf/__init__.py
 RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/__init__.py
 RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/Group.py
 RsCMPX_Gprf/Implementations/Catalog/Gprf/Generator/Spath/__init__.py
+RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Ploss.py
 RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/Spath.py
 RsCMPX_Gprf/Implementations/Catalog/Gprf/Measurement/__init__.py
 RsCMPX_Gprf/Implementations/Catalog/Gsm/__init__.py
 RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/Spath.py
 RsCMPX_Gprf/Implementations/Catalog/Gsm/Measurement/__init__.py
 RsCMPX_Gprf/Implementations/Catalog/Lte/__init__.py
 RsCMPX_Gprf/Implementations/Catalog/LteDl/__init__.py
@@ -103,48 +104,58 @@
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Auto.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/Average.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/ExtPwrSensor/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/PeakSearch.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/FftSpecAn/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Capture.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/IqSettings.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/Trigger.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Bandpass.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/Gauss.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/FilterPy/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/EnvelopePower.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Frequency.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/Sstop.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqRecorder/ListPy/__init__.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/Trigger.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/EnvelopePower.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Frequency.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Retrigger.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/Sstop.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/IqVsSlot/ListPy/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/Frequency.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Nrpm/Sensor/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/View.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/__init__.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/Frequency.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/ListPy/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/File.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Ploss/TsTone/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Catalog.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/Trigger.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Bandpass.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/Gauss.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/FilterPy/__init__.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Cidx.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/EnvelopePower.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Frequency.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/IqData.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Irepetition.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/ParameterSetList.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Retrigger.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Sstop.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/__init__.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Connection.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/__init__.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/Connection.py
+RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ListPy/Idx/Catalog/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Catalog.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Mlength.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/PdefSet.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/Slength.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/__init__.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/Bandwidth.py
 RsCMPX_Gprf/Implementations/Configure/Gprf/Measurement/Power/ParameterSetList/FilterPy/TypePy.py
@@ -174,14 +185,20 @@
 RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Globale.py
 RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/Tenvironment.py
 RsCMPX_Gprf/Implementations/Configure/System/Attenuation/CorrectionTable/Info/__init__.py
 RsCMPX_Gprf/Implementations/Configure/System/Control/Reboot.py
 RsCMPX_Gprf/Implementations/Configure/System/Control/Restart.py
 RsCMPX_Gprf/Implementations/Configure/System/Control/Shutdown.py
 RsCMPX_Gprf/Implementations/Configure/System/Control/__init__.py
+RsCMPX_Gprf/Implementations/Configure/System/Positioner/HwProperties.py
+RsCMPX_Gprf/Implementations/Configure/System/Positioner/Moving.py
+RsCMPX_Gprf/Implementations/Configure/System/Positioner/Versions.py
+RsCMPX_Gprf/Implementations/Configure/System/Positioner/__init__.py
+RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/To.py
+RsCMPX_Gprf/Implementations/Configure/System/Positioner/Move/__init__.py
 RsCMPX_Gprf/Implementations/Configure/System/Recall/Partial.py
 RsCMPX_Gprf/Implementations/Configure/System/Recall/__init__.py
 RsCMPX_Gprf/Implementations/Configure/System/Rf42/__init__.py
 RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/__init__.py
 RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Rx.py
 RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/Tx.py
 RsCMPX_Gprf/Implementations/Configure/System/Rf42/Box/Apreset/__init__.py
@@ -215,14 +232,16 @@
 RsCMPX_Gprf/Implementations/Create/Tenvironment/Spath.py
 RsCMPX_Gprf/Implementations/Create/Tenvironment/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Catalog/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/Connectors.py
 RsCMPX_Gprf/Implementations/Diagnostic/Catalog/System/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Configure/__init__.py
+RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/Measurement.py
+RsCMPX_Gprf/Implementations/Diagnostic/Configure/Gprf/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/FilterPy.py
 RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Psub/__init__.py
 RsCMPX_Gprf/Implementations/Diagnostic/Configure/System/Dapi/Logging/File/Rpc/FilterPy.py
@@ -330,14 +349,27 @@
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Clear.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/__init__.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Eoo.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezo.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Ezz.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/Frequency.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Eeprom/__init__.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Frequency.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Gain.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/State.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/__init__.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Frequency.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/Gain.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Evaluate/Trace/__init__.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/State.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Match/__init__.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/State.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Open/__init__.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/State.py
+RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/Short/__init__.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/All.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Ploss/State/__init__.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/AmplitudeProbDensity.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/ElapsedStats.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/IqInfo.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/__init__.py
 RsCMPX_Gprf/Implementations/Gprf/Measurement/Power/Average/Rms.py
@@ -480,14 +512,18 @@
 RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/Spath.py
 RsCMPX_Gprf/Implementations/Route/Wpan/Measurement/__init__.py
 RsCMPX_Gprf/Implementations/Sense/__init__.py
 RsCMPX_Gprf/Implementations/Sense/Base/__init__.py
 RsCMPX_Gprf/Implementations/Sense/Base/Temperature/__init__.py
 RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/Ambient.py
 RsCMPX_Gprf/Implementations/Sense/Base/Temperature/Operating/__init__.py
+RsCMPX_Gprf/Implementations/Sense/System/__init__.py
+RsCMPX_Gprf/Implementations/Sense/System/Positioner/IsMoving.py
+RsCMPX_Gprf/Implementations/Sense/System/Positioner/Position.py
+RsCMPX_Gprf/Implementations/Sense/System/Positioner/__init__.py
 RsCMPX_Gprf/Implementations/Source/__init__.py
 RsCMPX_Gprf/Implementations/Source/Gprf/__init__.py
 RsCMPX_Gprf/Implementations/Source/Gprf/Generator/IqSettings.py
 RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Reliability.py
 RsCMPX_Gprf/Implementations/Source/Gprf/Generator/RfSettings.py
 RsCMPX_Gprf/Implementations/Source/Gprf/Generator/__init__.py
 RsCMPX_Gprf/Implementations/Source/Gprf/Generator/Arb/File.py
@@ -611,29 +647,36 @@
 RsCMPX_Gprf/Implementations/Trigger/Bluetooth/Measurement/MultiEval/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Cdma/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/Catalog.py
 RsCMPX_Gprf/Implementations/Trigger/Cdma/Measurement/MultiEval/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/__init__.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Catalog.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/Execute.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Manual/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/Execute.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Arb/Segments/Manual/__init__.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsMeas.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/IsTrigger.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/Execute.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Generator/Sequencer/Manual/__init__.py
-RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder.py
-RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Spectrum.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/__init__.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/Catalog.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/OsStop.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/FftSpecAn/__init__.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/Catalog.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqRecorder/__init__.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/Catalog.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/IqVsSlot/__init__.py
+RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/Catalog.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/Offset.py
 RsCMPX_Gprf/Implementations/Trigger/Gprf/Measurement/Power/ParameterSetList/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gsm/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/__init__.py
 RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/Catalog.py
 RsCMPX_Gprf/Implementations/Trigger/Gsm/Measurement/MultiEval/__init__.py
```

### Comparing `RsCMPX_Gprf-5.0.90/setup.py` & `RsCMPX_Gprf-5.0.91/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.rst").read_text()
 
 # This call to setup() does all the work
 setup(
     name="RsCMPX_Gprf",
-    version="5.0.90",
+    version="5.0.91",
     description="CMX/CMP/PVT Global Purpose RF Remote-control module",
     long_description=README,
     long_description_content_type="text/x-rst",
     author="Rohde & Schwarz GmbH & Co. KG",
     copyright="Copyright © Rohde & Schwarz GmbH & Co. KG 2022",
     license="MIT",
     classifiers=['License :: OSI Approved :: MIT License',
```

