# Comparing `tmp/mypy-boto3-medialive-1.34.70.tar.gz` & `tmp/mypy-boto3-medialive-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-medialive-1.34.70.tar", last modified: Mon Mar 25 19:34:01 2024, max compression
+gzip compressed data, was "mypy-boto3-medialive-1.34.77.tar", last modified: Wed Apr  3 19:32:40 2024, max compression
```

## Comparing `mypy-boto3-medialive-1.34.70.tar` & `mypy-boto3-medialive-1.34.77.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:01.533655 mypy-boto3-medialive-1.34.70/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-03-25 19:34:01.533655 mypy-boto3-medialive-1.34.70/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14177 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:01.529655 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54614 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    54611 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    42019 2024-03-25 19:33:23.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    42019 2024-03-25 19:33:23.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   155364 2024-03-25 19:33:26.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   155364 2024-03-25 19:33:26.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/version.py
--rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 19:34:01.533655 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-03-25 19:34:01.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-03-25 19:34:01.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 19:34:01.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 19:34:01.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-25 19:34:01.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-25 19:34:01.000000 mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 19:34:01.533655 mypy-boto3-medialive-1.34.70/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-25 19:33:22.000000 mypy-boto3-medialive-1.34.70/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14177 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54614 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54611 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    43209 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43209 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12116 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   156623 2024-04-03 19:32:23.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   156623 2024-04-03 19:32:23.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10441 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-03 19:32:20.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15740 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 19:32:40.000000 mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:40.200160 mypy-boto3-medialive-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-03 19:32:19.000000 mypy-boto3-medialive-1.34.77/setup.py
```

### Comparing `mypy-boto3-medialive-1.34.70/LICENSE` & `mypy-boto3-medialive-1.34.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/PKG-INFO` & `mypy-boto3-medialive-1.34.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.34.70
-Summary: Type annotations for boto3.MediaLive 1.34.70 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.MediaLive 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-medialive-1.34.70/README.md` & `mypy-boto3-medialive-1.34.77/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/__init__.py` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/__init__.pyi` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/__main__.py` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MediaLive 1.34.70\n"
-        "Version:         1.34.70\n"
+        "Type annotations for boto3.MediaLive 1.34.77\n"
+        "Version:         1.34.77\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.70")
+    print("1.34.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/client.py` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/client.pyi` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/literals.py` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,20 +58,25 @@
     "ChannelClassType",
     "ChannelCreatedWaiterName",
     "ChannelDeletedWaiterName",
     "ChannelPipelineIdToRestartType",
     "ChannelRunningWaiterName",
     "ChannelStateType",
     "ChannelStoppedWaiterName",
+    "CmafIngestSegmentLengthUnitsType",
+    "CmafNielsenId3BehaviorType",
     "ColorSpaceType",
     "ContentTypeType",
+    "DashRoleAudioType",
+    "DashRoleCaptionType",
     "DescribeSchedulePaginatorName",
     "DeviceSettingsSyncStateType",
     "DeviceUpdateStatusType",
     "DolbyEProgramSelectionType",
+    "DvbDashAccessibilityType",
     "DvbSdtOutputSdtType",
     "DvbSubDestinationAlignmentType",
     "DvbSubDestinationBackgroundColorType",
     "DvbSubDestinationFontColorType",
     "DvbSubDestinationOutlineColorType",
     "DvbSubDestinationShadowColorType",
     "DvbSubDestinationTeletextGridControlType",
@@ -293,14 +298,15 @@
     "Scte35ArchiveAllowedFlagType",
     "Scte35DeviceRestrictionsType",
     "Scte35InputModeType",
     "Scte35NoRegionalBlackoutFlagType",
     "Scte35SegmentationCancelIndicatorType",
     "Scte35SpliceInsertNoRegionalBlackoutBehaviorType",
     "Scte35SpliceInsertWebDeliveryAllowedBehaviorType",
+    "Scte35TypeType",
     "Scte35WebDeliveryAllowedFlagType",
     "SmoothGroupAudioOnlyTimecodeControlType",
     "SmoothGroupCertificateModeType",
     "SmoothGroupEventIdModeType",
     "SmoothGroupEventStopBehaviorType",
     "SmoothGroupSegmentationModeType",
     "SmoothGroupSparseTrackTypeType",
@@ -402,30 +408,67 @@
     "RUNNING",
     "STARTING",
     "STOPPING",
     "UPDATE_FAILED",
     "UPDATING",
 ]
 ChannelStoppedWaiterName = Literal["channel_stopped"]
+CmafIngestSegmentLengthUnitsType = Literal["MILLISECONDS", "SECONDS"]
+CmafNielsenId3BehaviorType = Literal["NO_PASSTHROUGH", "PASSTHROUGH"]
 ColorSpaceType = Literal["HDR10", "HLG_2020", "REC_601", "REC_709"]
 ContentTypeType = Literal["image/jpeg"]
+DashRoleAudioType = Literal[
+    "ALTERNATE",
+    "COMMENTARY",
+    "DESCRIPTION",
+    "DUB",
+    "EMERGENCY",
+    "ENHANCED-AUDIO-INTELLIGIBILITY",
+    "KARAOKE",
+    "MAIN",
+    "SUPPLEMENTARY",
+]
+DashRoleCaptionType = Literal[
+    "ALTERNATE",
+    "CAPTION",
+    "COMMENTARY",
+    "DESCRIPTION",
+    "DUB",
+    "EASYREADER",
+    "EMERGENCY",
+    "FORCED-SUBTITLE",
+    "KARAOKE",
+    "MAIN",
+    "METADATA",
+    "SUBTITLE",
+    "SUPPLEMENTARY",
+]
 DescribeSchedulePaginatorName = Literal["describe_schedule"]
 DeviceSettingsSyncStateType = Literal["SYNCED", "SYNCING"]
 DeviceUpdateStatusType = Literal["NOT_UP_TO_DATE", "UPDATING", "UP_TO_DATE"]
 DolbyEProgramSelectionType = Literal[
     "ALL_CHANNELS",
     "PROGRAM_1",
     "PROGRAM_2",
     "PROGRAM_3",
     "PROGRAM_4",
     "PROGRAM_5",
     "PROGRAM_6",
     "PROGRAM_7",
     "PROGRAM_8",
 ]
+DvbDashAccessibilityType = Literal[
+    "DVBDASH_1_VISUALLY_IMPAIRED",
+    "DVBDASH_2_HARD_OF_HEARING",
+    "DVBDASH_3_SUPPLEMENTAL_COMMENTARY",
+    "DVBDASH_4_DIRECTORS_COMMENTARY",
+    "DVBDASH_5_EDUCATIONAL_NOTES",
+    "DVBDASH_6_MAIN_PROGRAM",
+    "DVBDASH_7_CLEAN_FEED",
+]
 DvbSdtOutputSdtType = Literal["SDT_FOLLOW", "SDT_FOLLOW_IF_PRESENT", "SDT_MANUAL", "SDT_NONE"]
 DvbSubDestinationAlignmentType = Literal["CENTERED", "LEFT", "SMART"]
 DvbSubDestinationBackgroundColorType = Literal["BLACK", "NONE", "WHITE"]
 DvbSubDestinationFontColorType = Literal["BLACK", "BLUE", "GREEN", "RED", "WHITE", "YELLOW"]
 DvbSubDestinationOutlineColorType = Literal["BLACK", "BLUE", "GREEN", "RED", "WHITE", "YELLOW"]
 DvbSubDestinationShadowColorType = Literal["BLACK", "NONE", "WHITE"]
 DvbSubDestinationTeletextGridControlType = Literal["FIXED", "SCALED"]
@@ -766,14 +809,15 @@
 Scte35InputModeType = Literal["FIXED", "FOLLOW_ACTIVE"]
 Scte35NoRegionalBlackoutFlagType = Literal["NO_REGIONAL_BLACKOUT", "REGIONAL_BLACKOUT"]
 Scte35SegmentationCancelIndicatorType = Literal[
     "SEGMENTATION_EVENT_CANCELED", "SEGMENTATION_EVENT_NOT_CANCELED"
 ]
 Scte35SpliceInsertNoRegionalBlackoutBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35SpliceInsertWebDeliveryAllowedBehaviorType = Literal["FOLLOW", "IGNORE"]
+Scte35TypeType = Literal["NONE", "SCTE_35_WITHOUT_SEGMENTATION"]
 Scte35WebDeliveryAllowedFlagType = Literal["WEB_DELIVERY_ALLOWED", "WEB_DELIVERY_NOT_ALLOWED"]
 SmoothGroupAudioOnlyTimecodeControlType = Literal["PASSTHROUGH", "USE_CONFIGURED_CLOCK"]
 SmoothGroupCertificateModeType = Literal["SELF_SIGNED", "VERIFY_AUTHENTICITY"]
 SmoothGroupEventIdModeType = Literal["NO_EVENT_ID", "USE_CONFIGURED", "USE_TIMESTAMP"]
 SmoothGroupEventStopBehaviorType = Literal["NONE", "SEND_EOS"]
 SmoothGroupSegmentationModeType = Literal["USE_INPUT_SEGMENTATION", "USE_SEGMENT_DURATION"]
 SmoothGroupSparseTrackTypeType = Literal["NONE", "SCTE_35", "SCTE_35_WITHOUT_SEGMENTATION"]
@@ -893,14 +937,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -923,14 +968,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -1245,21 +1291,23 @@
     "multiplex_stopped",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/literals.pyi` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -58,20 +58,25 @@
     "ChannelClassType",
     "ChannelCreatedWaiterName",
     "ChannelDeletedWaiterName",
     "ChannelPipelineIdToRestartType",
     "ChannelRunningWaiterName",
     "ChannelStateType",
     "ChannelStoppedWaiterName",
+    "CmafIngestSegmentLengthUnitsType",
+    "CmafNielsenId3BehaviorType",
     "ColorSpaceType",
     "ContentTypeType",
+    "DashRoleAudioType",
+    "DashRoleCaptionType",
     "DescribeSchedulePaginatorName",
     "DeviceSettingsSyncStateType",
     "DeviceUpdateStatusType",
     "DolbyEProgramSelectionType",
+    "DvbDashAccessibilityType",
     "DvbSdtOutputSdtType",
     "DvbSubDestinationAlignmentType",
     "DvbSubDestinationBackgroundColorType",
     "DvbSubDestinationFontColorType",
     "DvbSubDestinationOutlineColorType",
     "DvbSubDestinationShadowColorType",
     "DvbSubDestinationTeletextGridControlType",
@@ -293,14 +298,15 @@
     "Scte35ArchiveAllowedFlagType",
     "Scte35DeviceRestrictionsType",
     "Scte35InputModeType",
     "Scte35NoRegionalBlackoutFlagType",
     "Scte35SegmentationCancelIndicatorType",
     "Scte35SpliceInsertNoRegionalBlackoutBehaviorType",
     "Scte35SpliceInsertWebDeliveryAllowedBehaviorType",
+    "Scte35TypeType",
     "Scte35WebDeliveryAllowedFlagType",
     "SmoothGroupAudioOnlyTimecodeControlType",
     "SmoothGroupCertificateModeType",
     "SmoothGroupEventIdModeType",
     "SmoothGroupEventStopBehaviorType",
     "SmoothGroupSegmentationModeType",
     "SmoothGroupSparseTrackTypeType",
@@ -402,30 +408,67 @@
     "RUNNING",
     "STARTING",
     "STOPPING",
     "UPDATE_FAILED",
     "UPDATING",
 ]
 ChannelStoppedWaiterName = Literal["channel_stopped"]
+CmafIngestSegmentLengthUnitsType = Literal["MILLISECONDS", "SECONDS"]
+CmafNielsenId3BehaviorType = Literal["NO_PASSTHROUGH", "PASSTHROUGH"]
 ColorSpaceType = Literal["HDR10", "HLG_2020", "REC_601", "REC_709"]
 ContentTypeType = Literal["image/jpeg"]
+DashRoleAudioType = Literal[
+    "ALTERNATE",
+    "COMMENTARY",
+    "DESCRIPTION",
+    "DUB",
+    "EMERGENCY",
+    "ENHANCED-AUDIO-INTELLIGIBILITY",
+    "KARAOKE",
+    "MAIN",
+    "SUPPLEMENTARY",
+]
+DashRoleCaptionType = Literal[
+    "ALTERNATE",
+    "CAPTION",
+    "COMMENTARY",
+    "DESCRIPTION",
+    "DUB",
+    "EASYREADER",
+    "EMERGENCY",
+    "FORCED-SUBTITLE",
+    "KARAOKE",
+    "MAIN",
+    "METADATA",
+    "SUBTITLE",
+    "SUPPLEMENTARY",
+]
 DescribeSchedulePaginatorName = Literal["describe_schedule"]
 DeviceSettingsSyncStateType = Literal["SYNCED", "SYNCING"]
 DeviceUpdateStatusType = Literal["NOT_UP_TO_DATE", "UPDATING", "UP_TO_DATE"]
 DolbyEProgramSelectionType = Literal[
     "ALL_CHANNELS",
     "PROGRAM_1",
     "PROGRAM_2",
     "PROGRAM_3",
     "PROGRAM_4",
     "PROGRAM_5",
     "PROGRAM_6",
     "PROGRAM_7",
     "PROGRAM_8",
 ]
+DvbDashAccessibilityType = Literal[
+    "DVBDASH_1_VISUALLY_IMPAIRED",
+    "DVBDASH_2_HARD_OF_HEARING",
+    "DVBDASH_3_SUPPLEMENTAL_COMMENTARY",
+    "DVBDASH_4_DIRECTORS_COMMENTARY",
+    "DVBDASH_5_EDUCATIONAL_NOTES",
+    "DVBDASH_6_MAIN_PROGRAM",
+    "DVBDASH_7_CLEAN_FEED",
+]
 DvbSdtOutputSdtType = Literal["SDT_FOLLOW", "SDT_FOLLOW_IF_PRESENT", "SDT_MANUAL", "SDT_NONE"]
 DvbSubDestinationAlignmentType = Literal["CENTERED", "LEFT", "SMART"]
 DvbSubDestinationBackgroundColorType = Literal["BLACK", "NONE", "WHITE"]
 DvbSubDestinationFontColorType = Literal["BLACK", "BLUE", "GREEN", "RED", "WHITE", "YELLOW"]
 DvbSubDestinationOutlineColorType = Literal["BLACK", "BLUE", "GREEN", "RED", "WHITE", "YELLOW"]
 DvbSubDestinationShadowColorType = Literal["BLACK", "NONE", "WHITE"]
 DvbSubDestinationTeletextGridControlType = Literal["FIXED", "SCALED"]
@@ -766,14 +809,15 @@
 Scte35InputModeType = Literal["FIXED", "FOLLOW_ACTIVE"]
 Scte35NoRegionalBlackoutFlagType = Literal["NO_REGIONAL_BLACKOUT", "REGIONAL_BLACKOUT"]
 Scte35SegmentationCancelIndicatorType = Literal[
     "SEGMENTATION_EVENT_CANCELED", "SEGMENTATION_EVENT_NOT_CANCELED"
 ]
 Scte35SpliceInsertNoRegionalBlackoutBehaviorType = Literal["FOLLOW", "IGNORE"]
 Scte35SpliceInsertWebDeliveryAllowedBehaviorType = Literal["FOLLOW", "IGNORE"]
+Scte35TypeType = Literal["NONE", "SCTE_35_WITHOUT_SEGMENTATION"]
 Scte35WebDeliveryAllowedFlagType = Literal["WEB_DELIVERY_ALLOWED", "WEB_DELIVERY_NOT_ALLOWED"]
 SmoothGroupAudioOnlyTimecodeControlType = Literal["PASSTHROUGH", "USE_CONFIGURED_CLOCK"]
 SmoothGroupCertificateModeType = Literal["SELF_SIGNED", "VERIFY_AUTHENTICITY"]
 SmoothGroupEventIdModeType = Literal["NO_EVENT_ID", "USE_CONFIGURED", "USE_TIMESTAMP"]
 SmoothGroupEventStopBehaviorType = Literal["NONE", "SEND_EOS"]
 SmoothGroupSegmentationModeType = Literal["USE_INPUT_SEGMENTATION", "USE_SEGMENT_DURATION"]
 SmoothGroupSparseTrackTypeType = Literal["NONE", "SCTE_35", "SCTE_35_WITHOUT_SEGMENTATION"]
@@ -893,14 +937,15 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
+    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -923,14 +968,15 @@
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
+    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -1245,21 +1291,23 @@
     "multiplex_stopped",
 ]
 RegionName = Literal[
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
+    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-north-1",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "me-central-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/paginator.py` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/paginator.pyi` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/type_defs.py` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,23 @@
     BurnInOutlineColorType,
     BurnInShadowColorType,
     BurnInTeletextGridControlType,
     CdiInputResolutionType,
     ChannelClassType,
     ChannelPipelineIdToRestartType,
     ChannelStateType,
+    CmafIngestSegmentLengthUnitsType,
+    CmafNielsenId3BehaviorType,
     ColorSpaceType,
+    DashRoleAudioType,
+    DashRoleCaptionType,
     DeviceSettingsSyncStateType,
     DeviceUpdateStatusType,
     DolbyEProgramSelectionType,
+    DvbDashAccessibilityType,
     DvbSdtOutputSdtType,
     DvbSubDestinationAlignmentType,
     DvbSubDestinationBackgroundColorType,
     DvbSubDestinationFontColorType,
     DvbSubDestinationOutlineColorType,
     DvbSubDestinationShadowColorType,
     DvbSubDestinationTeletextGridControlType,
@@ -264,14 +269,15 @@
     Scte35ArchiveAllowedFlagType,
     Scte35DeviceRestrictionsType,
     Scte35InputModeType,
     Scte35NoRegionalBlackoutFlagType,
     Scte35SegmentationCancelIndicatorType,
     Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
     Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
+    Scte35TypeType,
     Scte35WebDeliveryAllowedFlagType,
     SmoothGroupAudioOnlyTimecodeControlType,
     SmoothGroupCertificateModeType,
     SmoothGroupEventIdModeType,
     SmoothGroupEventStopBehaviorType,
     SmoothGroupSegmentationModeType,
     SmoothGroupSparseTrackTypeType,
@@ -352,14 +358,15 @@
     "CdiInputSpecificationTypeDef",
     "ChannelEgressEndpointTypeDef",
     "InputSpecificationTypeDef",
     "MaintenanceStatusTypeDef",
     "VpcOutputSettingsDescriptionTypeDef",
     "PipelineDetailTypeDef",
     "ClaimDeviceRequestRequestTypeDef",
+    "CmafIngestOutputSettingsTypeDef",
     "ColorCorrectionTypeDef",
     "MaintenanceCreateSettingsTypeDef",
     "VpcOutputSettingsTypeDef",
     "InputDestinationRequestTypeDef",
     "InputDeviceSettingsTypeDef",
     "InputSourceRequestTypeDef",
     "InputVpcRequestTypeDef",
@@ -482,14 +489,15 @@
     "StopMultiplexRequestRequestTypeDef",
     "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
     "VideoSelectorPidTypeDef",
     "VideoSelectorProgramIdTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "ArchiveCdnSettingsTypeDef",
+    "CmafIngestGroupSettingsTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
     "MultiplexOutputSettingsTypeDef",
     "RtmpOutputSettingsTypeDef",
     "AudioChannelMappingTypeDef",
     "AudioCodecSettingsTypeDef",
     "AudioOnlyHlsSettingsTypeDef",
@@ -1078,14 +1086,20 @@
 )
 ClaimDeviceRequestRequestTypeDef = TypedDict(
     "ClaimDeviceRequestRequestTypeDef",
     {
         "Id": NotRequired[str],
     },
 )
+CmafIngestOutputSettingsTypeDef = TypedDict(
+    "CmafIngestOutputSettingsTypeDef",
+    {
+        "NameModifier": NotRequired[str],
+    },
+)
 ColorCorrectionTypeDef = TypedDict(
     "ColorCorrectionTypeDef",
     {
         "InputColorSpace": ColorSpaceType,
         "OutputColorSpace": ColorSpaceType,
         "Uri": str,
     },
@@ -2070,14 +2084,25 @@
 )
 ArchiveCdnSettingsTypeDef = TypedDict(
     "ArchiveCdnSettingsTypeDef",
     {
         "ArchiveS3Settings": NotRequired[ArchiveS3SettingsTypeDef],
     },
 )
+CmafIngestGroupSettingsTypeDef = TypedDict(
+    "CmafIngestGroupSettingsTypeDef",
+    {
+        "Destination": OutputLocationRefTypeDef,
+        "NielsenId3Behavior": NotRequired[CmafNielsenId3BehaviorType],
+        "Scte35Type": NotRequired[Scte35TypeType],
+        "SegmentLength": NotRequired[int],
+        "SegmentLengthUnits": NotRequired[CmafIngestSegmentLengthUnitsType],
+        "SendDelayMs": NotRequired[int],
+    },
+)
 MediaPackageGroupSettingsTypeDef = TypedDict(
     "MediaPackageGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 MsSmoothGroupSettingsTypeDef = TypedDict(
@@ -3652,14 +3677,16 @@
     {
         "CaptionSelectorName": str,
         "Name": str,
         "Accessibility": NotRequired[AccessibilityTypeType],
         "DestinationSettings": NotRequired[CaptionDestinationSettingsTypeDef],
         "LanguageCode": NotRequired[str],
         "LanguageDescription": NotRequired[str],
+        "CaptionDashRoles": NotRequired[Sequence[DashRoleCaptionType]],
+        "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
     },
 )
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
         "AdMarkers": NotRequired[Sequence[HlsAdMarkersType]],
@@ -3899,14 +3926,16 @@
         "AudioTypeControl": NotRequired[AudioDescriptionAudioTypeControlType],
         "AudioWatermarkingSettings": NotRequired[AudioWatermarkSettingsTypeDef],
         "CodecSettings": NotRequired[AudioCodecSettingsTypeDef],
         "LanguageCode": NotRequired[str],
         "LanguageCodeControl": NotRequired[AudioDescriptionLanguageCodeControlType],
         "RemixSettings": NotRequired[RemixSettingsTypeDef],
         "StreamName": NotRequired[str],
+        "AudioDashRoles": NotRequired[Sequence[DashRoleAudioType]],
+        "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
     },
 )
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
@@ -3918,14 +3947,15 @@
         "FrameCaptureGroupSettings": NotRequired[FrameCaptureGroupSettingsTypeDef],
         "HlsGroupSettings": NotRequired[HlsGroupSettingsTypeDef],
         "MediaPackageGroupSettings": NotRequired[MediaPackageGroupSettingsTypeDef],
         "MsSmoothGroupSettings": NotRequired[MsSmoothGroupSettingsTypeDef],
         "MultiplexGroupSettings": NotRequired[Mapping[str, Any]],
         "RtmpGroupSettings": NotRequired[RtmpGroupSettingsTypeDef],
         "UdpGroupSettings": NotRequired[UdpGroupSettingsTypeDef],
+        "CmafIngestGroupSettings": NotRequired[CmafIngestGroupSettingsTypeDef],
     },
 )
 InputSettingsPaginatorTypeDef = TypedDict(
     "InputSettingsPaginatorTypeDef",
     {
         "AudioSelectors": NotRequired[List[AudioSelectorPaginatorTypeDef]],
         "CaptionSelectors": NotRequired[List[CaptionSelectorPaginatorTypeDef]],
@@ -3975,14 +4005,15 @@
         "FrameCaptureOutputSettings": NotRequired[FrameCaptureOutputSettingsTypeDef],
         "HlsOutputSettings": NotRequired[HlsOutputSettingsTypeDef],
         "MediaPackageOutputSettings": NotRequired[Mapping[str, Any]],
         "MsSmoothOutputSettings": NotRequired[MsSmoothOutputSettingsTypeDef],
         "MultiplexOutputSettings": NotRequired[MultiplexOutputSettingsTypeDef],
         "RtmpOutputSettings": NotRequired[RtmpOutputSettingsTypeDef],
         "UdpOutputSettings": NotRequired[UdpOutputSettingsTypeDef],
+        "CmafIngestOutputSettings": NotRequired[CmafIngestOutputSettingsTypeDef],
     },
 )
 CreateMultiplexProgramResponseTypeDef = TypedDict(
     "CreateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/type_defs.pyi` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -51,18 +51,23 @@
     BurnInOutlineColorType,
     BurnInShadowColorType,
     BurnInTeletextGridControlType,
     CdiInputResolutionType,
     ChannelClassType,
     ChannelPipelineIdToRestartType,
     ChannelStateType,
+    CmafIngestSegmentLengthUnitsType,
+    CmafNielsenId3BehaviorType,
     ColorSpaceType,
+    DashRoleAudioType,
+    DashRoleCaptionType,
     DeviceSettingsSyncStateType,
     DeviceUpdateStatusType,
     DolbyEProgramSelectionType,
+    DvbDashAccessibilityType,
     DvbSdtOutputSdtType,
     DvbSubDestinationAlignmentType,
     DvbSubDestinationBackgroundColorType,
     DvbSubDestinationFontColorType,
     DvbSubDestinationOutlineColorType,
     DvbSubDestinationShadowColorType,
     DvbSubDestinationTeletextGridControlType,
@@ -264,14 +269,15 @@
     Scte35ArchiveAllowedFlagType,
     Scte35DeviceRestrictionsType,
     Scte35InputModeType,
     Scte35NoRegionalBlackoutFlagType,
     Scte35SegmentationCancelIndicatorType,
     Scte35SpliceInsertNoRegionalBlackoutBehaviorType,
     Scte35SpliceInsertWebDeliveryAllowedBehaviorType,
+    Scte35TypeType,
     Scte35WebDeliveryAllowedFlagType,
     SmoothGroupAudioOnlyTimecodeControlType,
     SmoothGroupCertificateModeType,
     SmoothGroupEventIdModeType,
     SmoothGroupEventStopBehaviorType,
     SmoothGroupSegmentationModeType,
     SmoothGroupSparseTrackTypeType,
@@ -352,14 +358,15 @@
     "CdiInputSpecificationTypeDef",
     "ChannelEgressEndpointTypeDef",
     "InputSpecificationTypeDef",
     "MaintenanceStatusTypeDef",
     "VpcOutputSettingsDescriptionTypeDef",
     "PipelineDetailTypeDef",
     "ClaimDeviceRequestRequestTypeDef",
+    "CmafIngestOutputSettingsTypeDef",
     "ColorCorrectionTypeDef",
     "MaintenanceCreateSettingsTypeDef",
     "VpcOutputSettingsTypeDef",
     "InputDestinationRequestTypeDef",
     "InputDeviceSettingsTypeDef",
     "InputSourceRequestTypeDef",
     "InputVpcRequestTypeDef",
@@ -482,14 +489,15 @@
     "StopMultiplexRequestRequestTypeDef",
     "ThumbnailTypeDef",
     "TransferInputDeviceRequestRequestTypeDef",
     "VideoSelectorPidTypeDef",
     "VideoSelectorProgramIdTypeDef",
     "UpdateAccountConfigurationRequestRequestTypeDef",
     "ArchiveCdnSettingsTypeDef",
+    "CmafIngestGroupSettingsTypeDef",
     "MediaPackageGroupSettingsTypeDef",
     "MsSmoothGroupSettingsTypeDef",
     "MultiplexOutputSettingsTypeDef",
     "RtmpOutputSettingsTypeDef",
     "AudioChannelMappingTypeDef",
     "AudioCodecSettingsTypeDef",
     "AudioOnlyHlsSettingsTypeDef",
@@ -1078,14 +1086,20 @@
 )
 ClaimDeviceRequestRequestTypeDef = TypedDict(
     "ClaimDeviceRequestRequestTypeDef",
     {
         "Id": NotRequired[str],
     },
 )
+CmafIngestOutputSettingsTypeDef = TypedDict(
+    "CmafIngestOutputSettingsTypeDef",
+    {
+        "NameModifier": NotRequired[str],
+    },
+)
 ColorCorrectionTypeDef = TypedDict(
     "ColorCorrectionTypeDef",
     {
         "InputColorSpace": ColorSpaceType,
         "OutputColorSpace": ColorSpaceType,
         "Uri": str,
     },
@@ -2070,14 +2084,25 @@
 )
 ArchiveCdnSettingsTypeDef = TypedDict(
     "ArchiveCdnSettingsTypeDef",
     {
         "ArchiveS3Settings": NotRequired[ArchiveS3SettingsTypeDef],
     },
 )
+CmafIngestGroupSettingsTypeDef = TypedDict(
+    "CmafIngestGroupSettingsTypeDef",
+    {
+        "Destination": OutputLocationRefTypeDef,
+        "NielsenId3Behavior": NotRequired[CmafNielsenId3BehaviorType],
+        "Scte35Type": NotRequired[Scte35TypeType],
+        "SegmentLength": NotRequired[int],
+        "SegmentLengthUnits": NotRequired[CmafIngestSegmentLengthUnitsType],
+        "SendDelayMs": NotRequired[int],
+    },
+)
 MediaPackageGroupSettingsTypeDef = TypedDict(
     "MediaPackageGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
     },
 )
 MsSmoothGroupSettingsTypeDef = TypedDict(
@@ -3652,14 +3677,16 @@
     {
         "CaptionSelectorName": str,
         "Name": str,
         "Accessibility": NotRequired[AccessibilityTypeType],
         "DestinationSettings": NotRequired[CaptionDestinationSettingsTypeDef],
         "LanguageCode": NotRequired[str],
         "LanguageDescription": NotRequired[str],
+        "CaptionDashRoles": NotRequired[Sequence[DashRoleCaptionType]],
+        "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
     },
 )
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "Destination": OutputLocationRefTypeDef,
         "AdMarkers": NotRequired[Sequence[HlsAdMarkersType]],
@@ -3899,14 +3926,16 @@
         "AudioTypeControl": NotRequired[AudioDescriptionAudioTypeControlType],
         "AudioWatermarkingSettings": NotRequired[AudioWatermarkSettingsTypeDef],
         "CodecSettings": NotRequired[AudioCodecSettingsTypeDef],
         "LanguageCode": NotRequired[str],
         "LanguageCodeControl": NotRequired[AudioDescriptionLanguageCodeControlType],
         "RemixSettings": NotRequired[RemixSettingsTypeDef],
         "StreamName": NotRequired[str],
+        "AudioDashRoles": NotRequired[Sequence[DashRoleAudioType]],
+        "DvbDashAccessibility": NotRequired[DvbDashAccessibilityType],
     },
 )
 Scte35DescriptorTypeDef = TypedDict(
     "Scte35DescriptorTypeDef",
     {
         "Scte35DescriptorSettings": Scte35DescriptorSettingsTypeDef,
     },
@@ -3918,14 +3947,15 @@
         "FrameCaptureGroupSettings": NotRequired[FrameCaptureGroupSettingsTypeDef],
         "HlsGroupSettings": NotRequired[HlsGroupSettingsTypeDef],
         "MediaPackageGroupSettings": NotRequired[MediaPackageGroupSettingsTypeDef],
         "MsSmoothGroupSettings": NotRequired[MsSmoothGroupSettingsTypeDef],
         "MultiplexGroupSettings": NotRequired[Mapping[str, Any]],
         "RtmpGroupSettings": NotRequired[RtmpGroupSettingsTypeDef],
         "UdpGroupSettings": NotRequired[UdpGroupSettingsTypeDef],
+        "CmafIngestGroupSettings": NotRequired[CmafIngestGroupSettingsTypeDef],
     },
 )
 InputSettingsPaginatorTypeDef = TypedDict(
     "InputSettingsPaginatorTypeDef",
     {
         "AudioSelectors": NotRequired[List[AudioSelectorPaginatorTypeDef]],
         "CaptionSelectors": NotRequired[List[CaptionSelectorPaginatorTypeDef]],
@@ -3975,14 +4005,15 @@
         "FrameCaptureOutputSettings": NotRequired[FrameCaptureOutputSettingsTypeDef],
         "HlsOutputSettings": NotRequired[HlsOutputSettingsTypeDef],
         "MediaPackageOutputSettings": NotRequired[Mapping[str, Any]],
         "MsSmoothOutputSettings": NotRequired[MsSmoothOutputSettingsTypeDef],
         "MultiplexOutputSettings": NotRequired[MultiplexOutputSettingsTypeDef],
         "RtmpOutputSettings": NotRequired[RtmpOutputSettingsTypeDef],
         "UdpOutputSettings": NotRequired[UdpOutputSettingsTypeDef],
+        "CmafIngestOutputSettings": NotRequired[CmafIngestOutputSettingsTypeDef],
     },
 )
 CreateMultiplexProgramResponseTypeDef = TypedDict(
     "CreateMultiplexProgramResponseTypeDef",
     {
         "MultiplexProgram": MultiplexProgramTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/waiter.py` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive/waiter.pyi` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/PKG-INFO` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-medialive
-Version: 1.34.70
-Summary: Type annotations for boto3.MediaLive 1.34.70 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.MediaLive 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-medialive.svg?color=blue)](https://pypi.org/project/mypy-boto3-medialive)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_medialive/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-medialive)](https://pepy.tech/project/mypy-boto3-medialive)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MediaLive 1.34.70](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
+[boto3.MediaLive 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/medialive.html#MediaLive)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
```

### Comparing `mypy-boto3-medialive-1.34.70/mypy_boto3_medialive.egg-info/SOURCES.txt` & `mypy-boto3-medialive-1.34.77/mypy_boto3_medialive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-medialive-1.34.70/setup.py` & `mypy-boto3-medialive-1.34.77/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-medialive",
-    version="1.34.70",
+    version="1.34.77",
     packages=["mypy_boto3_medialive"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.MediaLive 1.34.70 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.MediaLive 1.34.77 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

