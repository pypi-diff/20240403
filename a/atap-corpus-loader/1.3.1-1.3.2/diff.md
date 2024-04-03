# Comparing `tmp/atap_corpus_loader-1.3.1.tar.gz` & `tmp/atap_corpus_loader-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atap_corpus_loader-1.3.1.tar", max compression
+gzip compressed data, was "atap_corpus_loader-1.3.2.tar", max compression
```

## Comparing `atap_corpus_loader-1.3.1.tar` & `atap_corpus_loader-1.3.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1091 2023-12-21 02:04:16.054274 atap_corpus_loader-1.3.1/LICENSE
--rw-r--r--   0        0        0     1121 2024-03-26 05:34:13.109832 atap_corpus_loader-1.3.1/README.md
--rw-r--r--   0        0        0     3034 2024-03-28 05:36:33.585396 atap_corpus_loader-1.3.1/atap_corpus_loader/CorpusLoader.py
--rw-r--r--   0        0        0       39 2024-01-31 23:37:31.659710 atap_corpus_loader-1.3.1/atap_corpus_loader/__init__.py
--rw-r--r--   0        0        0    15416 2024-04-03 01:49:20.162500 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/Controller.py
--rw-r--r--   0        0        0     2165 2024-04-02 05:16:29.554696 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/CorpusExportService.py
--rw-r--r--   0        0        0    10508 2024-04-03 00:47:02.926020 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/FileLoaderService.py
--rw-r--r--   0        0        0      120 2024-01-31 04:39:45.157422 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/OniAPIService.py
--rw-r--r--   0        0        0       35 2024-01-31 04:39:45.157711 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/__init__.py
--rw-r--r--   0        0        0      869 2024-03-26 23:51:50.596436 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/CorpusHeader.py
--rw-r--r--   0        0        0      269 2024-02-07 03:45:55.625849 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/DataType.py
--rw-r--r--   0        0        0    10360 2024-04-03 00:34:17.992814 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/FileReference.py
--rw-r--r--   0        0        0     4113 2024-04-01 23:58:39.235829 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py
--rw-r--r--   0        0        0      556 2024-04-02 01:55:47.521647 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py
--rw-r--r--   0        0        0      243 2024-03-26 05:34:13.113505 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/__init__.py
--rw-r--r--   0        0        0       42 2024-01-31 04:39:45.159548 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/FileLoadError.py
--rw-r--r--   0        0        0     2854 2024-04-03 01:49:20.162871 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py
--rw-r--r--   0        0        0     2333 2024-02-01 00:33:21.789787 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py
--rw-r--r--   0        0        0      141 2024-01-31 04:39:45.160266 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/__init__.py
--rw-r--r--   0        0        0     1258 2024-04-03 00:34:17.993483 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py
--rw-r--r--   0        0        0     1388 2024-04-03 01:49:20.163247 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py
--rw-r--r--   0        0        0     1295 2024-03-26 23:51:50.585036 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py
--rw-r--r--   0        0        0     1495 2024-04-03 01:49:20.163576 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py
--rw-r--r--   0        0        0     2120 2024-03-26 23:51:50.591361 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py
--rw-r--r--   0        0        0     1278 2024-04-03 00:15:00.851696 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py
--rw-r--r--   0        0        0     1271 2024-04-03 01:49:20.163973 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py
--rw-r--r--   0        0        0     1253 2024-04-03 00:15:00.852579 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py
--rw-r--r--   0        0        0     1644 2024-04-03 01:49:20.164171 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py
--rw-r--r--   0        0        0      441 2024-04-03 01:49:20.164466 atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/__init__.py
--rw-r--r--   0        0        0     2394 2024-03-28 05:27:29.294201 atap_corpus_loader-1.3.1/atap_corpus_loader/view/ViewWrapperWidget.py
--rw-r--r--   0        0        0      108 2024-01-31 04:39:45.163251 atap_corpus_loader-1.3.1/atap_corpus_loader/view/__init__.py
--rw-r--r--   0        0        0      908 2024-03-26 05:34:13.115036 atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/AbstractWidget.py
--rw-r--r--   0        0        0     5737 2024-04-03 01:49:20.164863 atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/CorpusInfoWidget.py
--rw-r--r--   0        0        0     6626 2024-04-02 04:47:12.414631 atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/FileLoaderWidget.py
--rw-r--r--   0        0        0     5339 2024-03-28 00:37:16.585867 atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/FileSelectorWidget.py
--rw-r--r--   0        0        0     8527 2024-03-28 03:29:31.348900 atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/MetaEditorWidget.py
--rw-r--r--   0        0        0      368 2024-01-31 04:42:43.574976 atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/OniLoaderWidget.py
--rw-r--r--   0        0        0      182 2024-01-31 04:39:45.165382 atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/__init__.py
--rw-r--r--   0        0        0      884 2024-03-28 04:28:43.163463 atap_corpus_loader-1.3.1/atap_corpus_loader/view/notifications/NotifierService.py
--rw-r--r--   0        0        0       45 2024-01-31 04:39:45.165968 atap_corpus_loader-1.3.1/atap_corpus_loader/view/notifications/__init__.py
--rw-r--r--   0        0        0     1620 2024-04-03 01:49:20.165187 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/TooltipManager.py
--rw-r--r--   0        0        0       43 2024-03-27 23:21:38.983306 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/__init__.py
--rw-r--r--   0        0        0      156 2024-03-27 23:35:47.897183 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/build_button.md
--rw-r--r--   0        0        0      972 2024-03-28 02:04:53.521402 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md
--rw-r--r--   0        0        0      271 2024-03-28 01:27:53.108446 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/file_filter_input.md
--rw-r--r--   0        0        0      425 2024-03-28 03:09:31.422589 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/linking_selectors.md
--rw-r--r--   0        0        0      889 2024-03-28 01:52:42.823366 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/load_buttons.md
--rw-r--r--   0        0        0      234 2024-03-28 01:08:20.066821 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/load_corpus_button.md
--rw-r--r--   0        0        0     1182 2024-03-28 03:09:31.426273 atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/meta_editor.md
--rw-r--r--   0        0        0      637 2024-04-03 01:49:25.096180 atap_corpus_loader-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 atap_corpus_loader-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-12-21 02:04:16.054274 atap_corpus_loader-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1121 2024-03-26 05:34:13.109832 atap_corpus_loader-1.3.2/README.md
+-rw-r--r--   0        0        0     3034 2024-03-28 05:36:33.585396 atap_corpus_loader-1.3.2/atap_corpus_loader/CorpusLoader.py
+-rw-r--r--   0        0        0       39 2024-01-31 23:37:31.659710 atap_corpus_loader-1.3.2/atap_corpus_loader/__init__.py
+-rw-r--r--   0        0        0    15416 2024-04-03 01:49:20.162500 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/Controller.py
+-rw-r--r--   0        0        0     2165 2024-04-03 02:11:09.116021 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/CorpusExportService.py
+-rw-r--r--   0        0        0    10879 2024-04-03 02:05:16.581687 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/FileLoaderService.py
+-rw-r--r--   0        0        0      120 2024-01-31 04:39:45.157422 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/OniAPIService.py
+-rw-r--r--   0        0        0       35 2024-01-31 04:39:45.157711 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/__init__.py
+-rw-r--r--   0        0        0      869 2024-03-26 23:51:50.596436 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/CorpusHeader.py
+-rw-r--r--   0        0        0      269 2024-02-07 03:45:55.625849 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/DataType.py
+-rw-r--r--   0        0        0    10450 2024-04-03 02:09:59.092870 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/FileReference.py
+-rw-r--r--   0        0        0     4113 2024-04-01 23:58:39.235829 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py
+-rw-r--r--   0        0        0      556 2024-04-02 01:55:47.521647 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py
+-rw-r--r--   0        0        0      243 2024-03-26 05:34:13.113505 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/__init__.py
+-rw-r--r--   0        0        0       42 2024-01-31 04:39:45.159548 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/FileLoadError.py
+-rw-r--r--   0        0        0     2854 2024-04-03 01:49:20.162871 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py
+-rw-r--r--   0        0        0     2333 2024-02-01 00:33:21.789787 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py
+-rw-r--r--   0        0        0      141 2024-01-31 04:39:45.160266 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/__init__.py
+-rw-r--r--   0        0        0     1258 2024-04-03 00:34:17.993483 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py
+-rw-r--r--   0        0        0     1388 2024-04-03 01:49:20.163247 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py
+-rw-r--r--   0        0        0     1295 2024-03-26 23:51:50.585036 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py
+-rw-r--r--   0        0        0     1495 2024-04-03 01:49:20.163576 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py
+-rw-r--r--   0        0        0     2120 2024-03-26 23:51:50.591361 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py
+-rw-r--r--   0        0        0     1278 2024-04-03 00:15:00.851696 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py
+-rw-r--r--   0        0        0     1271 2024-04-03 01:49:20.163973 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py
+-rw-r--r--   0        0        0     1253 2024-04-03 00:15:00.852579 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py
+-rw-r--r--   0        0        0     1644 2024-04-03 01:49:20.164171 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py
+-rw-r--r--   0        0        0      441 2024-04-03 01:49:20.164466 atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/__init__.py
+-rw-r--r--   0        0        0     2394 2024-03-28 05:27:29.294201 atap_corpus_loader-1.3.2/atap_corpus_loader/view/ViewWrapperWidget.py
+-rw-r--r--   0        0        0      108 2024-01-31 04:39:45.163251 atap_corpus_loader-1.3.2/atap_corpus_loader/view/__init__.py
+-rw-r--r--   0        0        0      908 2024-03-26 05:34:13.115036 atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/AbstractWidget.py
+-rw-r--r--   0        0        0     5737 2024-04-03 01:49:20.164863 atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/CorpusInfoWidget.py
+-rw-r--r--   0        0        0     6626 2024-04-02 04:47:12.414631 atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/FileLoaderWidget.py
+-rw-r--r--   0        0        0     5339 2024-03-28 00:37:16.585867 atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/FileSelectorWidget.py
+-rw-r--r--   0        0        0     8527 2024-03-28 03:29:31.348900 atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/MetaEditorWidget.py
+-rw-r--r--   0        0        0      368 2024-01-31 04:42:43.574976 atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/OniLoaderWidget.py
+-rw-r--r--   0        0        0      182 2024-01-31 04:39:45.165382 atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/__init__.py
+-rw-r--r--   0        0        0      884 2024-03-28 04:28:43.163463 atap_corpus_loader-1.3.2/atap_corpus_loader/view/notifications/NotifierService.py
+-rw-r--r--   0        0        0       45 2024-01-31 04:39:45.165968 atap_corpus_loader-1.3.2/atap_corpus_loader/view/notifications/__init__.py
+-rw-r--r--   0        0        0     1620 2024-04-03 01:49:20.165187 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/TooltipManager.py
+-rw-r--r--   0        0        0       43 2024-03-27 23:21:38.983306 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/__init__.py
+-rw-r--r--   0        0        0      156 2024-03-27 23:35:47.897183 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/build_button.md
+-rw-r--r--   0        0        0      972 2024-03-28 02:04:53.521402 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md
+-rw-r--r--   0        0        0      271 2024-03-28 01:27:53.108446 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/file_filter_input.md
+-rw-r--r--   0        0        0      425 2024-03-28 03:09:31.422589 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/linking_selectors.md
+-rw-r--r--   0        0        0      889 2024-03-28 01:52:42.823366 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/load_buttons.md
+-rw-r--r--   0        0        0      234 2024-03-28 01:08:20.066821 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/load_corpus_button.md
+-rw-r--r--   0        0        0     1182 2024-03-28 03:09:31.426273 atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/meta_editor.md
+-rw-r--r--   0        0        0      637 2024-04-03 02:14:04.041824 atap_corpus_loader-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 atap_corpus_loader-1.3.2/PKG-INFO
```

### Comparing `atap_corpus_loader-1.3.1/LICENSE` & `atap_corpus_loader-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/README.md` & `atap_corpus_loader-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/CorpusLoader.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/CorpusLoader.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/Controller.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/Controller.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/CorpusExportService.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/CorpusExportService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/FileLoaderService.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/FileLoaderService.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from glob import iglob
 from os import R_OK, access
 from os.path import normpath, sep, isdir, exists
 from typing import Optional, Iterator
+from zipfile import BadZipFile
 
 from pandas import DataFrame, merge, concat
 from panel.widgets import Tqdm
 from atap_corpus.corpus.corpus import DataFrameCorpus
 
 from atap_corpus_loader.controller.data_objects import FileReference, CorpusHeader, FileReferenceFactory
 from atap_corpus_loader.controller.file_loader_strategy import FileLoaderStrategy, FileLoaderFactory, FileLoadError
@@ -66,15 +67,18 @@
                 continue
             if not include_hidden and file_ref.is_hidden():
                 continue
             FileLoaderService._check_filepath_permissions(file_ref)
 
             self.loaded_corpus_files.add(file_ref)
             if file_ref.is_archive():
-                zip_refs: list[FileReference] = self.file_ref_factory.get_zip_file_refs(filepath)
+                try:
+                    zip_refs: list[FileReference] = self.file_ref_factory.get_zip_file_refs(filepath)
+                except BadZipFile:
+                    raise FileLoadError(f"Can't read Zip file as it is malformed: {file_ref.get_filename()}")
                 for zip_ref in zip_refs:
                     if not zip_ref.is_hidden() or include_hidden:
                         self.loaded_corpus_files.add(zip_ref)
 
     def add_meta_files(self, meta_filepaths: list[str], include_hidden: bool, tqdm_obj: Tqdm):
         for filepath in tqdm_obj(meta_filepaths, desc="Loading metadata files", unit="files", leave=False):
             file_ref: FileReference = self.file_ref_factory.get_file_ref(filepath)
@@ -82,15 +86,18 @@
                 continue
             if not include_hidden and file_ref.is_hidden():
                 continue
             FileLoaderService._check_filepath_permissions(file_ref)
 
             self.loaded_meta_files.add(file_ref)
             if file_ref.is_archive():
-                zip_refs: list[FileReference] = self.file_ref_factory.get_zip_file_refs(filepath)
+                try:
+                    zip_refs: list[FileReference] = self.file_ref_factory.get_zip_file_refs(filepath)
+                except BadZipFile:
+                    raise FileLoadError(f"Can't read Zip file as it is malformed: {file_ref.get_filename()}")
                 for zip_ref in zip_refs:
                     if not zip_ref.is_hidden() or include_hidden:
                         self.loaded_meta_files.add(zip_ref)
 
     def remove_corpus_filepath(self, corpus_filepath: str):
         file_ref: FileReference = self.file_ref_factory.get_file_ref(corpus_filepath)
         if file_ref in self.loaded_corpus_files:
```

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/CorpusHeader.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/CorpusHeader.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/FileReference.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/FileReference.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from io import BytesIO
 from os.path import join, dirname, basename
 from tempfile import NamedTemporaryFile
 from typing import Optional
-from zipfile import ZipFile
+from zipfile import ZipFile, BadZipFile
 
 
 class FileReference:
     """
     A general purpose object to hold information regarding a specific file in the file system.
     Folder structure is preserved as a path-like string
     """
@@ -220,15 +220,18 @@
         """
         self.file_ref_cache = {}
 
     def get_file_refs_from_path(self, path: str, expand_archived: bool) -> list[FileReference]:
         file_refs: list[FileReference]
         curr_file_ref = [self.get_file_ref(path)]
         if path.endswith('.zip'):
-            file_refs = self.get_zip_file_refs(path)
+            try:
+                file_refs = self.get_zip_file_refs(path)
+            except BadZipFile:
+                return []
             if not expand_archived:
                 file_refs = curr_file_ref
         else:
             file_refs = curr_file_ref
 
         return file_refs
```

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/UniqueNameCorpora.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/data_objects/ViewCorpusInfo.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/FileLoaderFactory.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/FileLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/CSVLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/DOCXLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODSLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/ODTLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/RLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TSVLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/TXTLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XLSXLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/controller/file_loader_strategy/concrete_strategies/XMLLoaderStrategy.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/ViewWrapperWidget.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/ViewWrapperWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/AbstractWidget.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/AbstractWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/CorpusInfoWidget.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/CorpusInfoWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/FileLoaderWidget.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/FileLoaderWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/FileSelectorWidget.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/FileSelectorWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/gui/MetaEditorWidget.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/gui/MetaEditorWidget.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/notifications/NotifierService.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/notifications/NotifierService.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/TooltipManager.py` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/TooltipManager.py`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/corpus_editor.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/load_buttons.md` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/load_buttons.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/atap_corpus_loader/view/tooltips/markdown/meta_editor.md` & `atap_corpus_loader-1.3.2/atap_corpus_loader/view/tooltips/markdown/meta_editor.md`

 * *Files identical despite different names*

### Comparing `atap_corpus_loader-1.3.1/pyproject.toml` & `atap_corpus_loader-1.3.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atap-corpus-loader"
-version = "1.3.1"
+version = "1.3.2"
 description = " A GUI loader for atap_corpus using the Panel library."
 authors = ["Hamish Croser <hamish.croser@sydney.edu.au>"]
 readme = "README.md"
 license = "MIT"
 packages = [{include = "atap_corpus_loader"}]
 
 [tool.poetry.dependencies]
```

### Comparing `atap_corpus_loader-1.3.1/PKG-INFO` & `atap_corpus_loader-1.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atap-corpus-loader
-Version: 1.3.1
+Version: 1.3.2
 Summary:  A GUI loader for atap_corpus using the Panel library.
 License: MIT
 Author: Hamish Croser
 Author-email: hamish.croser@sydney.edu.au
 Requires-Python: >=3.10.0,<3.12.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

