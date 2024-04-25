# Comparing `tmp/MobileInventoryCLI-0.4.65.tar.gz` & `tmp/MobileInventoryCLI-0.4.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.65.tar", last modified: Thu Apr 25 02:25:22 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.66.tar", last modified: Thu Apr 25 13:28:14 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.65.tar` & `MobileInventoryCLI-0.4.66.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.661335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.661335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.661335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   106666 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.664668 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-25 02:22:54.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
--rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    67488 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
--rw-r--r--   0 carl      (1000) carl      (1000)     1642 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-25 02:25:18.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1601 2024-04-25 02:24:50.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.668002 MobileInventoryCLI-0.4.65/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-24 23:45:34.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     5283 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 02:25:22.671335 MobileInventoryCLI-0.4.65/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-25 02:25:22.000000 MobileInventoryCLI-0.4.65/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.438771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.442104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    37397 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     9817 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4937 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   106666 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.445437 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4606 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6098 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34799 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3078 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    17392 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    21197 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    69631 2024-04-25 13:24:18.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.448771 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    28428 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1642 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-25 13:28:08.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1988 2024-04-25 13:27:53.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5767 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1042 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-25 02:25:29.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     5283 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      854 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 13:28:14.452104 MobileInventoryCLI-0.4.66/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      956 2024-04-25 13:28:14.000000 MobileInventoryCLI-0.4.66/setup.py
```

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/DatePicker.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/ResetTools.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/CalcTimePad.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,20 +174,20 @@
                         if reset == False:
                             break
             except Exception as e:
                 print(e)
 
 
     def setFieldInList(self,fieldname,load=False):
+        tmp_fieldname=fieldname
         while True:
             if (fieldname not in self.special or fieldname in ['Facings'] )or (load==True and fieldname in ['ListQty',]):
                 m=f"Item Num |Name|Barcode|Code|{fieldname}|EID"
                 hr='-'*len(m)
-                print(f"{m}\n{hr}")
-                if (fieldname in self.valid_fields) or (load==True and fieldname in ['ListQty',]):
+                if (fieldname in self.valid_fields) or (load==True and fieldname in ['ListQty',]) or fieldname == None:
                     with Session(self.engine) as session:
                         code=''
                         
                         def mkT(text,self):
                             return str(text)
                         code=Prompt.__init2__(None,func=mkT,ptext="barcode|code",helpText=self.helpText_barcodes,data=self)
                         if code == None:
@@ -211,14 +211,50 @@
                                             text=text[:-1]
                                             break
 
                                 return float(eval(text)),text,suffix
                             except Exception as e:
                                 print(e)
                                 return float(0),text,''
+                        if fieldname == None:
+                            hstring=f'''
+Location Fields:
+{Fore.deep_pink_3b}Shelf{Style.reset}
+{Fore.light_steel_blue}BackRoom{Style.reset}
+{Fore.cyan}Display_1{Style.reset}
+{Fore.cyan}Display_2{Style.reset}
+{Fore.cyan}Display_3{Style.reset}
+{Fore.cyan}Display_4{Style.reset}
+{Fore.cyan}Display_5{Style.reset}
+{Fore.cyan}Display_6{Style.reset}
+{Fore.cyan}SBX_WTR_DSPLY{Style.reset}
+{Fore.cyan}SBX_CHP_DSPLY{Style.reset}
+{Fore.cyan}SBX_WTR_KLR{Style.reset}
+{Fore.violet}FLRL_CHP_DSPLY{Style.reset}
+{Fore.violet}FLRL_WTR_DSPLY{Style.reset}
+{Fore.grey_50}WD_DSPLY{Style.reset}
+{Fore.grey_50}CHKSTND_SPLY{Style.reset}'''
+                            def mkfields(text,data):
+                                try:
+                                    fields=tuple([i.name for i in Entry.__table__.columns])
+                                    fields_lower=tuple([i.lower() for i in fields])
+                                    if text.lower() in fields_lower:
+                                        index=fields_lower.index(text.lower())
+                                        return fields[index]
+                                except Exception as e:
+                                    print(e)
+                            while True:
+                                fieldname=Prompt.__init2__(None,func=mkfields,ptext="Location Field(see h|help)",helpText=hstring,data=self)
+                                if fieldname in [None,]:
+                                    break
+                                break
+                            if fieldname in [None,]:
+                                continue
+                            m=f"Item Num |Name|Barcode|Code|{fieldname}|EID"
+                            hr='-'*len(m)
 
                         p=Prompt.__init2__(None,func=mkT,ptext="amount|+amount|-amount",helpText=self.helpText_barcodes,data=self)
                         if p:
                             value,text,suffix=p
                         else:
                             continue
                         try:
@@ -348,14 +384,16 @@
                                     #raise Exception(result)
                         except Exception as e:
                             print(e)
             else:
                 #code for tags,caseId[br,6w,ld],
                 self.processSpecial(fieldname)
                 break
+            if tmp_fieldname == None:
+                fieldname=None
     helpText_barcodes=f"""
 1. Enter the EntryId into the prompt
 2. if an entry is found you will be prompted for a code to be saved
 Quantity Modifiers:
 (SEP=',' or No Sep) Suffixes Singles: s|e|u|' '|'' == units/singles/eaches/no multipliers
 (SEP=',' or No Sep) Suffixes CaseCount: c == (qty*casecount+old_value_if_any
 Valid Examples:
@@ -1109,14 +1147,20 @@
         count+=1
         self.options["lus"]={
                     'cmds':["#"+str(count),f"lookup_short","lus","lu-","check","ck-","ls"],
                     'desc':f'get total for valid fields short view',
                     'exec':lambda self=self,entry=entry: self.getTotalwithBreakDownForScan(short=True),
                     }
         count+=1
+        self.options["b1"]={
+                    'cmds':["#"+str(count),f"barcode_first","b1"],
+                    'desc':f'list mode where barcode is asked first',
+                    'exec':lambda self=self: self.setFieldInList(None,load=True),
+                    }
+        count+=1
 
 
         while True:
             def mkT(text,self):
                 return text
             command=Prompt.__init2__(None,func=mkT,ptext='Do What[help/??/?]',helpText=self.parent.help(print_no=True),data=self)
             if not command:
```

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/WebSearchFrameWork/SearchMethods.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,8 +7,17 @@
 06:37 am 04-9-2024 -- add a new field userUpdated to entry so if Entry is edited with 'ie' then field will be marked true, for reference on Entries the User has edited, import will add duplicated codes to Inlist==True so Entries can be reviewed, added total_entries to unified to shortlist total entries
 09:30 am 04-13-2024 -- added new functionalty for task mode whereby if a code
 is not found a search prompt is presented, with 'r' to rset search or 'b' to
 cancel entry; added new prompts for PunchCard
 11:48 am 04-13-2024 -- replaced unified's factory_reset with a class based toolset to reset only certain, or all, components
 12:41 pm 04-21-2024 -- add DatePkr() to edit_punchcard as was not initially built-in, now is, add a websearchframework module for later development
 08:06 pm 04-23-2024 -- haulted dev of web search framework as go-upc is not free
-07:23 pm 04-24-2024 -- added new calculator module to PunchCard, CalcTimePad to add addition tool functionality, for better planning, or other
+07:23 pm 04-24-2024 -- added new calculator module to PunchCard, CalcTimePad to add addition tool functionality, for better planning, or other
+06:26 am 04-25-2024 -- scan barcode/code -> search for item
+						if not item:
+							begin similar process to t->#40 and create new item
+						if item:
+							prompt for location field to set
+							prompt for amount, or leave blank to skip
+							set InList==True so le-img can export the Entry, or qsl
+								can be used to quick-show-list
+6:27 am 04-25-2024 -- added version value
```

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/x.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.65
+Version: 0.4.66
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.65/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.66/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.65/PKG-INFO` & `MobileInventoryCLI-0.4.66/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.65
+Version: 0.4.66
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Android
```

### Comparing `MobileInventoryCLI-0.4.65/setup.py` & `MobileInventoryCLI-0.4.66/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.65'
+version='0.4.66'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

