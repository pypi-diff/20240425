# Comparing `tmp/MobileInventoryCLI-0.4.64.tar.gz` & `tmp/MobileInventoryCLI-0.4.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.64.tar", last modified: Wed Apr 24 23:45:26 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.65.tar", last modified: Thu Apr 25 02:25:22 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.64.tar` & `MobileInventoryCLI-0.4.65.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.484256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.484256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.487589 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.487589 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.487589 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.487589 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.487589 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   106666 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.487589 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     2231 2024-04-24 23:42:28.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-24 23:27:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    67488 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.490922 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1642 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-24 23:45:21.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1458 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-23 20:46:10.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-23 20:46:11.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-24 23:45:26.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5283 2024-04-24 23:45:26.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-24 23:45:26.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-24 23:45:26.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-24 23:45:26.000000 MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-24 23:45:26.494256 MobileInventoryCLI-0.4.64/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-24 23:45:26.000000 MobileInventoryCLI-0.4.64/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.661335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.661335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.661335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   106666 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-25 02:22:54.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    67488 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1642 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-25 02:25:18.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1601 2024-04-25 02:24:50.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5283 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/setup.py
```

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from colored import Style,Fore
 
 
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.DatePicker import *
 from MobileInventoryCLI.CodeProcessing.RecordCodesAndBarcodes.DB.Prompt import *
 
 class CalcNetFrom2Pt:
+	tax_rate=0.178
 	def __init__(self,rate=False):
 		print("END DATETIME")
 		try:
 			end=DateTimePkr()
 		except Exception as e:
 			print(e)
 			return
@@ -19,15 +20,15 @@
 		except Exception as e:
 			print(e)
 			return
 		print(f"{Fore.light_green}A break of {Fore.dark_goldenrod}60 Minutes is {Fore.light_yellow}Subtracted from {Fore.light_red}{Style.bold}{Style.underline}Total Duration{Style.reset}")
 		breakt=timedelta(seconds=60*60)
 		print(f'{Fore.spring_green_2a}{(end-start)-breakt}{Style.reset}')
 
-		print(f"{Fore.light_red}{Style.bold}{Style.underline}Be Aware {Fore.light_yellow}Not Used in Rate Calculations!{Style.reset}\n{Fore.light_green}A break of {Fore.dark_goldenrod}30 Minutes is {Fore.light_yellow}Subtracted from {Fore.light_red}{Style.bold}{Style.underline}Total Duration{Style.reset}")
+		print(f"{Fore.light_red}{Style.bold}{Style.underline}Be Aware {Fore.light_yellow} that 30M will be paid in check for shorter lunch!{Style.reset}\n{Fore.light_green}A break of {Fore.dark_goldenrod}30 Minutes is {Fore.light_yellow}Subtracted from {Fore.light_red}{Style.bold}{Style.underline}Total Duration{Style.reset}")
 		breakt30=timedelta(seconds=60*30)
 		print(f'{Fore.light_magenta}{(end-start)-breakt30}{Style.reset}')
 		
 		if not rate:
 			return
 			
 		def mkFloat(text,data):
@@ -39,30 +40,43 @@
 				print(e)
 		while True:
 		 rate=Prompt.__init2__(None,func=mkFloat,ptext='Rate of pay $/Hr',helpText="How Much do you make an hour?",data=1)
 		 if rate in (None,):
 		 	break
 		 gross=round(((((end-start)-breakt).total_seconds()/60)/60)*rate,2)
 		 print(gross)
-		 tax=gross*0.178
+		 tax=gross*self.tax_rate
 		 print(gross-tax)
 		 wwd=Prompt.__init2__(None,func=mkFloat,ptext='days in work week(to calculate union dues per day)',helpText="How Many days are in your work week?",data=4)
 		 if wwd in (None,):
 		 	break
 		 union=10/wwd
 		 net=gross-tax
 		 net-=union
-		 print('gross:',gross)
-		 print('net income: ',net)
-		 print('tax:',-tax)
-		 print('union dues:',-union)
-		 print('duration:',(end-start)-breakt)
+
+		 gross30=round(((((end-start)-breakt30).total_seconds()/60)/60)*rate,2)
+		 tax30=gross30*self.tax_rate
+		 net30=gross30-tax30-union
+		 endC=Style.reset
+		 value=Fore.light_green
+		 add30value=Fore.sea_green_1a
+		 add30name=Fore.light_yellow
+		 fieldname=Fore.dark_goldenrod
+		 m='Your Rate Calculation Results are below'
+		 header=f"{Fore.light_magenta}{Style.bold}{Style.underline}{m}{Style.reset}\n{Style.bold}{Fore.red_3a}{'.'*len(m)}{Style.reset}"
+		 msg=f'''{header}
+{fieldname}gross{endC} ({add30name}+30M={add30value}{gross30}{endC}):{value} {gross}{endC}
+{fieldname}net income{endC}({add30name}+30M={add30value}{net30}{endC}):{value} {net}{endC}
+{fieldname}tax{endC}({add30name}+30M={add30value}{tax30}{endC}):{value} {-tax}{endC}
+{fieldname}union dues{endC}:{value} {-union}{endC}
+{fieldname}duration{endC}({add30name}+30M={add30value}{(end-start)-breakt30}{endC}):{value}{(end-start)-breakt}{endC}\n{Style.bold}{Fore.cyan}{'.'*len(m)}{Style.reset}'''
+
+		 print(msg)
 		 break
 		 
 		 #how many days in work week
 		 #divide 10 by work week days
 		 #subtract from gross-tax
-		print((end-start)-breakt)
 		
 if __name__=='__main__':
 	state=True
 	CalcNetFrom2Pt(rate=state)
```

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,8 +6,9 @@
 11:59 am 04-4-2024 -- add protective measures in plus versions of Collect Mode (11) to prevent duplicate entries of data, with non-plus versions retaining initial duplicity issues should duplicity be required
 06:37 am 04-9-2024 -- add a new field userUpdated to entry so if Entry is edited with 'ie' then field will be marked true, for reference on Entries the User has edited, import will add duplicated codes to Inlist==True so Entries can be reviewed, added total_entries to unified to shortlist total entries
 09:30 am 04-13-2024 -- added new functionalty for task mode whereby if a code
 is not found a search prompt is presented, with 'r' to rset search or 'b' to
 cancel entry; added new prompts for PunchCard
 11:48 am 04-13-2024 -- replaced unified's factory_reset with a class based toolset to reset only certain, or all, components
 12:41 pm 04-21-2024 -- add DatePkr() to edit_punchcard as was not initially built-in, now is, add a websearchframework module for later development
-08:06 pm 04-23-2024 -- haulted dev of web search framework as go-upc is not free
+08:06 pm 04-23-2024 -- haulted dev of web search framework as go-upc is not free
+07:23 pm 04-24-2024 -- added new calculator module to PunchCard, CalcTimePad to add addition tool functionality, for better planning, or other
```

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.64
+Version: 0.4.65
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.64/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.64/PKG-INFO` & `MobileInventoryCLI-0.4.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.64
+Version: 0.4.65
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.64/setup.py` & `MobileInventoryCLI-0.4.65/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.64'
+version='0.4.65'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

