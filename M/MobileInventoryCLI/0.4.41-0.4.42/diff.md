# Comparing `tmp/MobileInventoryCLI-0.4.41.tar.gz` & `tmp/MobileInventoryCLI-0.4.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.41.tar", last modified: Wed Apr  3 03:27:32 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.42.tar", last modified: Wed Apr  3 04:03:23 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.41.tar` & `MobileInventoryCLI-0.4.42.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.060331 MobileInventoryCLI-0.4.41/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.040331 MobileInventoryCLI-0.4.41/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.043664 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.046998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.046998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.046998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.046998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.050331 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   102681 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5623 2024-04-03 03:26:10.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.050331 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
--rwxr-xr-x   0 carl      (1000) carl      (1000)   296284 2024-04-03 03:23:06.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.050331 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.050331 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.050331 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.050331 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.053664 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.053664 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.053664 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.053664 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34801 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.053664 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.053664 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.053664 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-03 03:27:23.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.056998 MobileInventoryCLI-0.4.41/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-03 03:05:16.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:32.060331 MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-03 03:27:31.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-03 03:27:31.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-03 03:27:31.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-03 03:27:31.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-03 03:27:31.000000 MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-03 03:27:32.060331 MobileInventoryCLI-0.4.41/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-03 03:27:32.060331 MobileInventoryCLI-0.4.41/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      810 2024-04-03 03:27:31.000000 MobileInventoryCLI-0.4.41/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.540377 MobileInventoryCLI-0.4.42/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.520377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.523711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.527044 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.530377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.530377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.530377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.530377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   102681 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5678 2024-04-03 04:02:31.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.530377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   915212 2022-09-16 02:34:37.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Default.TTF
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.530377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.530377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.533711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.533711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.533711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.533711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.533711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.533711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34801 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.533711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.533711 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.537044 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.537044 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-03 04:03:15.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.537044 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.537044 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.537044 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.537044 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.537044 MobileInventoryCLI-0.4.42/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.540377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.540377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.540377 MobileInventoryCLI-0.4.42/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-03 03:27:43.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-03 04:03:23.540377 MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      698 2024-04-03 04:03:23.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4874 2024-04-03 04:03:23.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-03 04:03:23.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      125 2024-04-03 04:03:23.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-03 04:03:23.000000 MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      698 2024-04-03 04:03:23.540377 MobileInventoryCLI-0.4.42/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-03 04:03:23.540377 MobileInventoryCLI-0.4.42/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      817 2024-04-03 04:03:23.000000 MobileInventoryCLI-0.4.42/setup.py
```

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,17 +11,18 @@
         old=0
         for line in lines:
             if len(line) > old:
                 old=len(line)
         return int(old*(self.fontsize*1.0))
 
     def setHeightFromLines(self,text):
+        #set self.size
         lines=text.split("\n")
         print(len(lines))
-        f=(self.fontsize*1.333)
+        f=(self.fontsize*1.75)
         ff=f*len(lines)
         return int(ff)
 
 
     def __init__(self,filename,text,barcode_file=None,code_file=None,img_file=None):
         self.barcode_file=barcode_file
         self.barcode_file_name=barcode_file
@@ -89,31 +90,34 @@
         self.dt=datetime.strftime(datetime.now(),"%m%d%Y")
         self.filename=filename
         self.white=(255,255,255)
         self.black=(0,0,0)
         self.padded=(20,20)
         
         self.text=text
-        
+        self.font_name=Path(__file__).parent.parent/Path("Default.TTF")
 
+        self.font=ImageFont.truetype(str(self.font_name),16)
         self.image=Image.new("RGB",self.size,self.white)
         self.draw=ImageDraw.Draw(self.image)
-        self.font_name=Path(__file__).parent.parent/Path("Default.TTF")
+        
         print(self.font_name)
-        self.font=ImageFont.truetype(str(self.font_name),16)
+        
+        '''
         try:
             raise Exception("e")
             self.font=ImageFont.load_default(size=16)
             print()
         except Exception as e:
             try:
                 self.font=ImageFont.truetype("/system/fonts/DroidSansMono.ttf",16)
             except Exception as e:
                 print(e)
                 self.font=ImageFont.load_default() 
+        '''
         self.save()
 
     def save(self):
         try:
             self.draw.text(self.padded,self.text,self.black,font=self.font)
             if self.barcode_file not in [True,False,None]:
                 w=self.width-self.barcode_file.size[0]
```

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.41
+Version: 0.4.42
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Requires-Dist: pint
 Requires-Dist: pyupc-ean
 Requires-Dist: openpyxl
 Requires-Dist: plyer
 Requires-Dist: colored
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: Pillow
+Requires-Dist: Pillow==9.5.0
 Requires-Dist: python-barcode
 Requires-Dist: qrcode
 Requires-Dist: requests
 Requires-Dist: sqlalchemy
 Requires-Dist: argparse
 Requires-Dist: geocoder
```

### Comparing `MobileInventoryCLI-0.4.41/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.42/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.41/PKG-INFO` & `MobileInventoryCLI-0.4.42/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.41
+Version: 0.4.42
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Requires-Dist: pint
 Requires-Dist: pyupc-ean
 Requires-Dist: openpyxl
 Requires-Dist: plyer
 Requires-Dist: colored
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: Pillow
+Requires-Dist: Pillow==9.5.0
 Requires-Dist: python-barcode
 Requires-Dist: qrcode
 Requires-Dist: requests
 Requires-Dist: sqlalchemy
 Requires-Dist: argparse
 Requires-Dist: geocoder
```

### Comparing `MobileInventoryCLI-0.4.41/setup.py` & `MobileInventoryCLI-0.4.42/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.41'
+version='0.4.42'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
 
           ],
       packages=find_packages(),
       python_requires='>=3.6',
-      install_requires=['pint','pyupc-ean','openpyxl','plyer','colored','numpy','pandas','Pillow','python-barcode','qrcode','requests','sqlalchemy','argparse','geocoder'],
+      install_requires=['pint','pyupc-ean','openpyxl','plyer','colored','numpy','pandas','Pillow==9.5.0','python-barcode','qrcode','requests','sqlalchemy','argparse','geocoder'],
       package_data={
         '':["*.config","*.txt","*.README","*.TTF"],
         }
       )
```

