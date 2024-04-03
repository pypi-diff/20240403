# Comparing `tmp/MobileInventoryCLI-0.4.38.tar.gz` & `tmp/MobileInventoryCLI-0.4.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MobileInventoryCLI-0.4.38.tar", last modified: Tue Apr  2 20:16:42 2024, max compression
+gzip compressed data, was "MobileInventoryCLI-0.4.39.tar", last modified: Tue Apr  2 21:47:03 2024, max compression
```

## Comparing `MobileInventoryCLI-0.4.38.tar` & `MobileInventoryCLI-0.4.39.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.444238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.444238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.447572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.447572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
--rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.447572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
--rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.447572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
--rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
--rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)   101415 2024-04-02 20:05:34.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
--rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
--rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
--rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-02 19:58:57.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
--rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
--rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
--rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
--rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.450905 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
--rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
--rw-r--r--   0 carl      (1000) carl      (1000)    34423 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
--rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
--rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
--rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
--rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
--rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
--rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-02 20:16:36.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
--rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.454238 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
--rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
--rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
--rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/__init__.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/collected/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/collected/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/dbpath.config
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/error/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/error/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/error/error.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/lookup/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/lookup/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/lookup/lookup.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/mainloop/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/mainloop/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/mainloop/mainloop.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI/updateCfg/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/updateCfg/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-02 19:05:45.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI/updateCfg/updateCfg.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)     4805 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-02 20:16:42.000000 MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-02 20:16:42.457572 MobileInventoryCLI-0.4.38/setup.cfg
--rw-r--r--   0 carl      (1000) carl      (1000)      802 2024-04-02 20:16:41.000000 MobileInventoryCLI-0.4.38/setup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.820014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.823348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.823348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.823348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/
+-rw-r--r--   0 carl      (1000) carl      (1000)    24225 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.823348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2931 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.826681 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3705 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      499 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/codep.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.826681 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/
+-rw-r--r--   0 carl      (1000) carl      (1000)     2347 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)   101486 2024-04-02 21:32:36.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5460 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.826681 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12259 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.826681 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/
+-rw-r--r--   0 carl      (1000) carl      (1000)     3695 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.826681 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/
+-rw-r--r--   0 carl      (1000) carl      (1000)     4238 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.826681 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1365 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.826681 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/
+-rw-r--r--   0 carl      (1000) carl      (1000)    12354 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.826681 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/
+-rw-r--r--   0 carl      (1000) carl      (1000)     6019 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      108 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.830014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)     5641 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.830014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1139 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.830014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/
+-rw-r--r--   0 carl      (1000) carl      (1000)    34801 2024-04-02 21:45:53.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.830014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/
+-rw-r--r--   0 carl      (1000) carl      (1000)    15997 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)    19940 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      122 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Run.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.830014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/
+-rw-r--r--   0 carl      (1000) carl      (1000)    54712 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.830014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/
+-rw-r--r--   0 carl      (1000) carl      (1000)    18522 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       12 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.830014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/
+-rw-r--r--   0 carl      (1000) carl      (1000)    25645 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       18 2024-04-02 21:46:59.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      390 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/changelog.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     5104 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)     4346 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     5077 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      718 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.830014 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2616 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      301 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/t.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      146 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/te.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1387 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Images/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1709 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/__init__.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/collected/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/collected/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1383 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)       91 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/dbpath.config
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/error/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/error/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)      290 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/error/error.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/lookup/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/lookup/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     2912 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/lookup/lookup.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/mainloop/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/mainloop/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     1429 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/mainloop/mainloop.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/MobileInventoryCLI/updateCfg/
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/updateCfg/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     3066 2024-04-02 20:16:51.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI/updateCfg/updateCfg.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 21:47:03.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)     4805 2024-04-02 21:47:03.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-02-15 17:26:38.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-02 21:47:03.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      118 2024-04-02 21:47:03.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       19 2024-04-02 21:47:03.000000 MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      691 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-02 21:47:03.833348 MobileInventoryCLI-0.4.39/setup.cfg
+-rw-r--r--   0 carl      (1000) carl      (1000)      802 2024-04-02 21:47:03.000000 MobileInventoryCLI-0.4.39/setup.py
```

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Collector2/Collector2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Conversion/Conversion.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ConvertCode/ConvertCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/Prompt.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -2353,14 +2353,17 @@
     Date=Column(Date)
     EntryCode=Column(String)
     EntryBarcode=Column(String)
     EntryName=Column(String)
     EntryId=Column(Integer)
     EntryPrice=Column(Float)
     QtySold=Column(Float)
+    CRV=Column(Float)
+    Tax=Column(Float)
+    TaxNote=Column(String)
     def __init__(self,**kwargs):
         kwargs['__tablename__']=self.__tablename__
         self.init(**kwargs)
 
 class AdditionalExpenseOrFee(BASE,Template):
     __tablename__="AdditionalExpenseOrFee"
     AdditionalExpenseId=Column(Integer,primary_key=True)
```

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DB/renderText2Png.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/DayLog/DayLogger.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExportList/ExportListCurrent.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ExtractPkg/ExtractPkg2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ListMode2/ListMode2.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/LocationSequencer/LocationSequencer.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Locator/Locator.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Lookup/Lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/ModuleTemplate/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/POS/POS.py`

 * *Files 2% similar despite different names*

```diff
@@ -204,19 +204,23 @@
     ReceiptId={reciept.RecieptId}
     """
             text.append(btext)
             ct=len(entries)
             total=0
             for num,r in enumerate(entries):
                 total+=(r.EntryPrice*r.QtySold)
-                specific=f"{r.EntryName} - {r.EntryBarcode} - {round(r.EntryPrice,2)}*{r.QtySold}={round(r.EntryPrice*r.QtySold,2)}"
+                if r.Tax == None:
+                    r.Tax=0
+                if r.CRV == None:
+                    r.CRV=0
+                specific=f"{r.EntryName} - {r.EntryBarcode} - {round(r.EntryPrice,2)}*QTY({r.QtySold})={round(r.EntryPrice*r.QtySold,2)} + Tax[{r.TaxNote}]({r.Tax*r.QtySold}) + CRV({r.CRV*r.QtySold}) = {round((r.EntryPrice*r.QtySold)+(r.Tax*r.QtySold)+(r.CRV*r.QtySold),2)}"
                 msg=f"{num}/{ct} -> {specific}"
                 text.append(msg)
 
-            text.append(f"Total Due: ${round(total,2)}")
+            text.append(f"Total Due: ${round(total+(r.Tax*r.QtySold)+(r.CRV*r.QtySold),2)}")
             print('\n'.join(text))
             def mkBool(text,self):
                 try:
                     if text in ['y','yes','true','True','1','t']:
                         return True
                     else:
                         return False
@@ -296,15 +300,15 @@
                                     return int(text)
                                 except Exception as e:
                                     print(e)
                             which=Prompt.__init2__(None,func=mkint,ptext=f"Which Entry Would you like to use?",helpText=f"use a integer between 0-{ct-1}",data=self)
                             if which in [None,]:
                                 return
                             e=entry[which]
-                            nre=RecieptEntry(RecieptId=reciept.RecieptId,Date=date.today(),EntryName=e.Name,EntryCode=e.Code,EntryBarcode=e.Barcode,EntryId=e.EntryId,EntryPrice=e.Price,QtySold=1)
+                            nre=RecieptEntry(RecieptId=reciept.RecieptId,Date=date.today(),EntryName=e.Name,EntryCode=e.Code,EntryBarcode=e.Barcode,EntryId=e.EntryId,EntryPrice=e.Price,QtySold=1,CRV=e.CRV,Tax=e.Tax,TaxNote=e.TaxNote)
                             session.add(nre)
                             session.commit()
                             session.flush()
                             session.refresh(nre)
                             print(f"Added {nre}!")
                         else:
                             print(f"{Fore.light_red}No Such Item!{Style.reset}")
@@ -383,15 +387,15 @@
                                             return int(text)
                                         except Exception as e:
                                             print(e)
                                     which=Prompt.__init2__(None,func=mkint,ptext=f"Which Entry Would you like to use?",helpText=f"use a integer between 0-{ct-1}",data=self)
                                     if which in [None,]:
                                         return
                                     e=entry[which]
-                                    nre=RecieptEntry(RecieptId=reciept.RecieptId,Date=date.today(),EntryName=e.Name,EntryCode=e.Code,EntryBarcode=e.Barcode,EntryId=e.EntryId,EntryPrice=e.Price,QtySold=1)
+                                    nre=RecieptEntry(RecieptId=reciept.RecieptId,Date=date.today(),EntryName=e.Name,EntryCode=e.Code,EntryBarcode=e.Barcode,EntryId=e.EntryId,EntryPrice=e.Price,QtySold=1,CRV=e.CRV,Tax=e.Tax,TaxNote=e.TaxNote)
                                     session.add(nre)
                                     session.commit()
                                     session.flush()
                                     session.refresh(nre)
                                     print(f"Added {nre}!")
                                 else:
                                     print(f"{Fore.light_red}No Such Item!{Style.reset}")
```

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/PunchCard/PunchCard.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/RecordMyCodes.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TasksMode/Tasks.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/TouchStampC/TouchStampC.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/Unified/Unified.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/helpMsg.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/possibleCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/renderQR.py.README`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/setCode/setCode.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/BeginnersLuck.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/CodeProcessing/RecordCodesAndBarcodes/tkGui/Review.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/__init__.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/__init__.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/lookup/lookup.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/lookup/lookup.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/mainloop/mainloop.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/mainloop/mainloop.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI/updateCfg/updateCfg.py` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI/updateCfg/updateCfg.py`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/PKG-INFO` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.38
+Version: 0.4.39
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.38/MobileInventoryCLI.egg-info/SOURCES.txt` & `MobileInventoryCLI-0.4.39/MobileInventoryCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MobileInventoryCLI-0.4.38/PKG-INFO` & `MobileInventoryCLI-0.4.39/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MobileInventoryCLI
-Version: 0.4.38
+Version: 0.4.39
 Summary: modify/update/use MobileInventoryPro *.bck files
 Author: Carl Joseph Hirner III
 Author-email: k.j.hirner.wisdom@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `MobileInventoryCLI-0.4.38/setup.py` & `MobileInventoryCLI-0.4.39/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup,find_packages
 from datetime import datetime
-version='0.4.38'
+version='0.4.39'
 
 setup(name='MobileInventoryCLI',
       version=version,
       author="Carl Joseph Hirner III",
       author_email="k.j.hirner.wisdom@gmail.com",
       description="modify/update/use MobileInventoryPro *.bck files",
       classifiers=[
```

