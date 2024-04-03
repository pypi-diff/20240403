# Comparing `tmp/quackosm-0.5.1.tar.gz` & `tmp/quackosm-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quackosm-0.5.1.tar", last modified: Sat Mar 23 11:09:21 2024, max compression
+gzip compressed data, was "quackosm-0.5.2.tar", last modified: Wed Apr  3 13:01:15 2024, max compression
```

## Comparing `quackosm-0.5.1.tar` & `quackosm-0.5.2.tar`

### file list

```diff
@@ -1,39 +1,40 @@
--rw-r--r--   0        0        0    11339 2024-03-23 11:08:58.175459 quackosm-0.5.1/LICENSE
--rw-r--r--   0        0        0    25727 2024-03-23 11:08:58.175459 quackosm-0.5.1/README.md
--rw-r--r--   0        0        0     4326 2024-03-23 11:09:21.727473 quackosm-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      560 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/__init__.py
--rw-r--r--   0        0        0      464 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/__main__.py
--rw-r--r--   0        0        0      127 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/_constants.py
--rw-r--r--   0        0        0     4406 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/_osm_tags_filters.py
--rw-r--r--   0        0        0     1188 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/_osm_way_polygon_features.py
--rw-r--r--   0        0        0     5513 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/_rich_progress.py
--rw-r--r--   0        0        0      717 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/_typing.py
--rw-r--r--   0        0        0    23638 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/cli.py
--rw-r--r--   0        0        0     1875 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/conftest.py
--rw-r--r--   0        0        0    50323 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/functions.py
--rw-r--r--   0        0        0    16047 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/osm_extracts/__init__.py
--rw-r--r--   0        0        0     2320 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/osm_extracts/_poly_parser.py
--rw-r--r--   0        0        0     3141 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/osm_extracts/bbbike.py
--rw-r--r--   0        0        0      251 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/osm_extracts/extract.py
--rw-r--r--   0        0        0     1687 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/osm_extracts/geofabrik.py
--rw-r--r--   0        0        0     4098 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/osm_extracts/osm_fr.py
--rw-r--r--   0        0        0     3362 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/osm_way_polygon_features.json
--rw-r--r--   0        0        0   104476 2024-03-23 11:08:58.183459 quackosm-0.5.1/quackosm/pbf_file_reader.py
--rw-r--r--   0        0        0       33 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0       38 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/base/__init__.py
--rw-r--r--   0        0        0    24267 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/base/test_cli.py
--rw-r--r--   0        0        0     4511 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/base/test_osm_extracts.py
--rw-r--r--   0        0        0    38527 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/base/test_pbf_file_reader.py
--rw-r--r--   0        0        0       43 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/benchmark/__init__.py
--rw-r--r--   0        0        0      919 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/benchmark/test_big_file.py
--rw-r--r--   0        0        0     1472 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/optional_imports/test_optional_cli_dependency.py
--rw-r--r--   0        0        0      342 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
--rw-r--r--   0        0        0      100 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
--rw-r--r--   0        0        0      770 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
--rw-r--r--   0        0        0    73746 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
--rw-r--r--   0        0        0     1013 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
--rw-r--r--   0        0        0   537903 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/monaco.osm.pbf
--rw-r--r--   0        0        0    91717 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/monaco_boundary.geojson
--rw-r--r--   0        0        0      112 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/osm_tags_filter.json
--rw-r--r--   0        0        0     5405 2024-03-23 11:08:58.187459 quackosm-0.5.1/tests/test_files/osmconf.ini
--rw-r--r--   0        0        0    27504 1970-01-01 00:00:00.000000 quackosm-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-04-03 13:00:45.769424 quackosm-0.5.2/LICENSE
+-rw-r--r--   0        0        0    25727 2024-04-03 13:00:45.769424 quackosm-0.5.2/README.md
+-rw-r--r--   0        0        0     4326 2024-04-03 13:01:15.233232 quackosm-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      560 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/__init__.py
+-rw-r--r--   0        0        0      464 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/__main__.py
+-rw-r--r--   0        0        0      127 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_constants.py
+-rw-r--r--   0        0        0      135 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_exceptions.py
+-rw-r--r--   0        0        0     4406 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_osm_tags_filters.py
+-rw-r--r--   0        0        0     1188 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_osm_way_polygon_features.py
+-rw-r--r--   0        0        0     6013 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_rich_progress.py
+-rw-r--r--   0        0        0      717 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/_typing.py
+-rw-r--r--   0        0        0    23859 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/cli.py
+-rw-r--r--   0        0        0     1875 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/conftest.py
+-rw-r--r--   0        0        0    51009 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/functions.py
+-rw-r--r--   0        0        0    19065 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/__init__.py
+-rw-r--r--   0        0        0     2320 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/_poly_parser.py
+-rw-r--r--   0        0        0     3141 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/bbbike.py
+-rw-r--r--   0        0        0      251 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/extract.py
+-rw-r--r--   0        0        0     1687 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/geofabrik.py
+-rw-r--r--   0        0        0     4098 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_extracts/osm_fr.py
+-rw-r--r--   0        0        0     3362 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/osm_way_polygon_features.json
+-rw-r--r--   0        0        0   106840 2024-04-03 13:00:45.777424 quackosm-0.5.2/quackosm/pbf_file_reader.py
+-rw-r--r--   0        0        0       33 2024-04-03 13:00:45.777424 quackosm-0.5.2/tests/__init__.py
+-rw-r--r--   0        0        0       38 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/base/__init__.py
+-rw-r--r--   0        0        0    24681 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/base/test_cli.py
+-rw-r--r--   0        0        0     5422 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/base/test_osm_extracts.py
+-rw-r--r--   0        0        0    39391 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/base/test_pbf_file_reader.py
+-rw-r--r--   0        0        0       43 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/benchmark/__init__.py
+-rw-r--r--   0        0        0      919 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/benchmark/test_big_file.py
+-rw-r--r--   0        0        0     1472 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/optional_imports/test_optional_cli_dependency.py
+-rw-r--r--   0        0        0      342 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/529cdcbb7a3cc103658ef31b39bed24984e421127d319c867edf2f86ff3bb098.osm.pbf
+-rw-r--r--   0        0        0      100 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/7a0163cb721992d6219d486b3d29517d06aa0db19dd7be049f4f1fabf6146073.osm.pbf
+-rw-r--r--   0        0        0      770 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf
+-rw-r--r--   0        0        0    73746 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf
+-rw-r--r--   0        0        0     1013 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf
+-rw-r--r--   0        0        0   537903 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/monaco.osm.pbf
+-rw-r--r--   0        0        0    91717 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/monaco_boundary.geojson
+-rw-r--r--   0        0        0      112 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/osm_tags_filter.json
+-rw-r--r--   0        0        0     5405 2024-04-03 13:00:45.781424 quackosm-0.5.2/tests/test_files/osmconf.ini
+-rw-r--r--   0        0        0    27504 1970-01-01 00:00:00.000000 quackosm-0.5.2/PKG-INFO
```

### Comparing `quackosm-0.5.1/LICENSE` & `quackosm-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/README.md` & `quackosm-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/pyproject.toml` & `quackosm-0.5.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "QuackOSM"
-version = "0.5.1"
+version = "0.5.2"
 description = "An open-source tool for reading OpenStreetMap PBF files using DuckDB"
 authors = [
     { name = "Kamil Raczycki", email = "kraczycki@kraina.ai" },
 ]
 dependencies = [
     "geopandas",
     "shapely>=2",
@@ -184,15 +184,15 @@
 tab-width = 4
 blank = false
 pre-summary-newline = true
 close-quotes-on-newline = true
 wrap-one-line = true
 
 [tool.bumpver]
-current_version = "0.5.1"
+current_version = "0.5.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "chore(CI/CD): bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `quackosm-0.5.1/quackosm/__init__.py` & `quackosm-0.5.2/quackosm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     convert_pbf_to_gpq,
     get_features_gdf,
     get_features_gdf_from_geometry,
 )
 from quackosm.pbf_file_reader import PbfFileReader
 
 __app_name__ = "QuackOSM"
-__version__ = "0.5.1"
+__version__ = "0.5.2"
 
 __all__ = [
     "PbfFileReader",
     "convert_pbf_to_gpq",
     "convert_geometry_to_gpq",
     "get_features_gdf",
     "get_features_gdf_from_geometry",
```

### Comparing `quackosm-0.5.1/quackosm/_osm_tags_filters.py` & `quackosm-0.5.2/quackosm/_osm_tags_filters.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/_osm_way_polygon_features.py` & `quackosm-0.5.2/quackosm/_osm_way_polygon_features.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/_rich_progress.py` & `quackosm-0.5.2/quackosm/_rich_progress.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # type: ignore
 """Wrapper over Rich progress bar."""
+
 import os
 from collections.abc import Iterable
 from contextlib import suppress
 from datetime import timedelta
 
 __all__ = ["TaskProgressSpinner", "TaskProgressBar"]
 
@@ -24,18 +25,21 @@
         from rich import print as rprint
 
         elapsed_time_formatted = str(timedelta(seconds=int(elapsed_seconds)))
         rprint(f"Finished operation in [progress.elapsed]{elapsed_time_formatted}")
 
 
 class TaskProgressSpinner:
-    def __init__(self, step_name: str, step_number: str, silent_mode: bool):
+    def __init__(
+        self, step_name: str, step_number: str, silent_mode: bool, skip_step_number: bool = False
+    ):
         self.step_name = step_name
         self.step_number = step_number
         self.silent_mode = silent_mode
+        self.skip_step_number = skip_step_number
         self.progress = None
         self.force_terminal = os.getenv("FORCE_TERMINAL_MODE", "false").lower() == "true"
 
     def __enter__(self):
         try:  # pragma: no cover
             if self.silent_mode:
                 self.progress = None
@@ -44,20 +48,27 @@
                     Console,
                     Progress,
                     SpinnerColumn,
                     TextColumn,
                     TimeElapsedColumn,
                 )
 
-                self.progress = Progress(
+                columns = [
                     SpinnerColumn(),
                     TextColumn(f"[{self.step_number: >4}/{TOTAL_STEPS}]"),
                     TextColumn("[progress.description]{task.description}"),
                     TextColumn("•"),
                     TimeElapsedColumn(),
+                ]
+
+                if self.skip_step_number:
+                    columns.pop(1)
+
+                self.progress = Progress(
+                    *columns,
                     refresh_per_second=1,
                     transient=False,
                     console=Console(
                         force_interactive=False if self.force_terminal else None,
                         force_jupyter=False if self.force_terminal else None,
                         force_terminal=True if self.force_terminal else None,
                     ),
@@ -73,23 +84,25 @@
         if self.progress:
             self.progress.__exit__(exc_type, exc_value, exc_tb)
 
         self.progress = None
 
 
 class TaskProgressBar:
-    def __init__(self, step_name: str, step_number: str, silent_mode: bool):
+    def __init__(
+        self, step_name: str, step_number: str, silent_mode: bool, skip_step_number: bool = False
+    ):
         self.step_name = step_name
         self.step_number = step_number
         self.silent_mode = silent_mode
+        self.skip_step_number = skip_step_number
         self.progress = None
         self.force_terminal = os.getenv("FORCE_TERMINAL_MODE", "false").lower() == "true"
 
     def __enter__(self):
-
         try:  # pragma: no cover
             if self.silent_mode:
                 self.progress = None
             else:
                 from rich.progress import (
                     BarColumn,
                     Console,
@@ -109,29 +122,36 @@
                         if task.speed is None:
                             return Text("")
                         elif task.speed >= 1:
                             return Text(f"{task.speed:.2f} it/s")
                         else:
                             return Text(f"{1/task.speed:.2f} s/it")  # noqa: FURB126
 
-                self.progress = Progress(
+                columns = [
                     SpinnerColumn(),
                     TextColumn(f"[{self.step_number: >4}/{TOTAL_STEPS}]"),
                     TextColumn(
                         "[progress.description]{task.description}"
                         " [progress.percentage]{task.percentage:>3.0f}%"
                     ),
                     BarColumn(),
                     MofNCompleteColumn(),
                     TextColumn("•"),
                     TimeElapsedColumn(),
                     TextColumn("<"),
                     TimeRemainingColumn(),
                     TextColumn("•"),
                     SpeedColumn(),
+                ]
+
+                if self.skip_step_number:
+                    columns.pop(1)
+
+                self.progress = Progress(
+                    *columns,
                     refresh_per_second=1,
                     transient=False,
                     speed_estimate_period=1800,
                     console=Console(
                         force_interactive=False if self.force_terminal else None,
                         force_jupyter=False if self.force_terminal else None,
                         force_terminal=True if self.force_terminal else None,
```

### Comparing `quackosm-0.5.1/quackosm/_typing.py` & `quackosm-0.5.2/quackosm/_typing.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/cli.py` & `quackosm-0.5.2/quackosm/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """CLI module for parsing pbf file to geoparquet."""
 
 import json
 import logging
 import re
-import warnings
 from pathlib import Path
 from typing import Annotated, Optional, Union, cast
 
 import click
 import geopandas as gpd
 import h3
 import osmnx as ox
@@ -513,14 +512,25 @@
         bool,
         typer.Option(
             "--silent/",
             help="Whether to disable progress reporting.",
             show_default=False,
         ),
     ] = False,
+    allow_uncovered_geometry: Annotated[
+        bool,
+        typer.Option(
+            "--allow-uncovered-geometry/",
+            help=(
+                "Suppresses an error if some geometry parts aren't covered by any OSM extract."
+                " Works only when PbfFileReader is asked to download OSM extracts automatically."
+            ),
+            show_default=False,
+        ),
+    ] = False,
     version: Annotated[
         Optional[bool],
         typer.Option(
             "--version",
             "-v",
             help="Show the application's version and exit.",
             callback=_version_callback,
@@ -569,49 +579,48 @@
             ),
             param=Argument(["pbf_file"], type=Path, metavar="PBF file path"),
         )
 
     if osm_tags_filter is not None and osm_tags_filter_file is not None:
         raise typer.BadParameter("Provided more than one osm tags filter parameter")
 
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        logging.disable(logging.CRITICAL)
-        if pbf_file:
-            geoparquet_path = convert_pbf_to_gpq(
-                pbf_path=pbf_file,
-                tags_filter=osm_tags_filter or osm_tags_filter_file,  # type: ignore
-                keep_all_tags=keep_all_tags,
-                geometry_filter=geometry_filter_value,
-                explode_tags=explode_tags,
-                ignore_cache=ignore_cache,
-                working_directory=working_directory,
-                result_file_path=result_file_path,
-                osm_way_polygon_features_config=(
-                    json.loads(Path(osm_way_polygon_features_config).read_text())
-                    if osm_way_polygon_features_config
-                    else None
-                ),
-                filter_osm_ids=filter_osm_ids,  # type: ignore
-                save_as_wkt=wkt_result,
-                silent_mode=silent_mode,
-            )
-        else:
-            geoparquet_path = convert_geometry_to_gpq(
-                geometry_filter=geometry_filter_value,
-                osm_extract_source=osm_extract_source,
-                tags_filter=osm_tags_filter or osm_tags_filter_file,  # type: ignore
-                keep_all_tags=keep_all_tags,
-                explode_tags=explode_tags,
-                ignore_cache=ignore_cache,
-                working_directory=working_directory,
-                result_file_path=result_file_path,
-                osm_way_polygon_features_config=(
-                    json.loads(Path(osm_way_polygon_features_config).read_text())
-                    if osm_way_polygon_features_config
-                    else None
-                ),
-                filter_osm_ids=filter_osm_ids,  # type: ignore
-                save_as_wkt=wkt_result,
-                silent_mode=silent_mode,
-            )
+    logging.disable(logging.CRITICAL)
+    if pbf_file:
+        geoparquet_path = convert_pbf_to_gpq(
+            pbf_path=pbf_file,
+            tags_filter=osm_tags_filter or osm_tags_filter_file,  # type: ignore
+            keep_all_tags=keep_all_tags,
+            geometry_filter=geometry_filter_value,
+            explode_tags=explode_tags,
+            ignore_cache=ignore_cache,
+            working_directory=working_directory,
+            result_file_path=result_file_path,
+            osm_way_polygon_features_config=(
+                json.loads(Path(osm_way_polygon_features_config).read_text())
+                if osm_way_polygon_features_config
+                else None
+            ),
+            filter_osm_ids=filter_osm_ids,  # type: ignore
+            save_as_wkt=wkt_result,
+            silent_mode=silent_mode,
+        )
+    else:
+        geoparquet_path = convert_geometry_to_gpq(
+            geometry_filter=geometry_filter_value,
+            osm_extract_source=osm_extract_source,
+            tags_filter=osm_tags_filter or osm_tags_filter_file,  # type: ignore
+            keep_all_tags=keep_all_tags,
+            explode_tags=explode_tags,
+            ignore_cache=ignore_cache,
+            working_directory=working_directory,
+            result_file_path=result_file_path,
+            osm_way_polygon_features_config=(
+                json.loads(Path(osm_way_polygon_features_config).read_text())
+                if osm_way_polygon_features_config
+                else None
+            ),
+            filter_osm_ids=filter_osm_ids,  # type: ignore
+            save_as_wkt=wkt_result,
+            silent_mode=silent_mode,
+            allow_uncovered_geometry=allow_uncovered_geometry,
+        )
     typer.secho(geoparquet_path, fg="green")
```

### Comparing `quackosm-0.5.1/quackosm/conftest.py` & `quackosm-0.5.2/quackosm/conftest.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/functions.py` & `quackosm-0.5.2/quackosm/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,25 +246,26 @@
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     save_as_wkt: bool = False,
     silent_mode: bool = False,
+    allow_uncovered_geometry: bool = False,
 ) -> Path:
     """
     Get a GeoParquet file with OpenStreetMap features within given geometry.
 
     Automatically downloads matching OSM extracts from different sources and returns a single file
     as a result.
 
     Args:
         geometry_filter (BaseGeometry): Geometry filter used to download matching OSM extracts.
         osm_extract_source (OsmExtractSource): A source for automatic downloading of
-            OSM extracts. Can be Geofabrik, BBBike, OSM_fr or any. Defaults to `any`.
+            OSM extracts. Can be Geofabrik, BBBike, OSMfr or any. Defaults to `any`.
         tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
             specifying which tags to download.
             The keys should be OSM tags (e.g. `building`, `amenity`).
             The values should either be `True` for retrieving all objects with the tag,
             string for retrieving a single tag-value pair
             or list of strings for retrieving all values specified in the list.
             `tags={'leisure': 'park}` would return parks from the area.
@@ -293,14 +294,17 @@
             Config used to determine which closed way features are polygons.
             Modifications to this config left are left for experienced OSM users.
             Defaults to predefined "osm_way_polygon_features.json".
         save_as_wkt (bool): Whether to save the file with geometry in the WKT form instead of WKB.
             If `True`, it will be saved as a `.parquet` file, because it won't be in the GeoParquet
             standard. Defaults to `False`.
         silent_mode (bool): Disable progress bars. Defaults to `False`.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Works only when PbfFileReader is asked to download OSM extracts
+            automatically. Defaults to `False`.
 
     Returns:
         Path: Path to the generated GeoParquet file.
 
     Examples:
         Get OSM data from the center of Monaco.
 
@@ -398,14 +402,15 @@
     return PbfFileReader(
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
         silent_mode=silent_mode,
+        allow_uncovered_geometry=allow_uncovered_geometry,
     ).convert_geometry_filter_to_gpq(
         result_file_path=result_file_path,
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
         save_as_wkt=save_as_wkt,
@@ -600,25 +605,26 @@
     keep_all_tags: bool = False,
     explode_tags: Optional[bool] = None,
     ignore_cache: bool = False,
     filter_osm_ids: Optional[list[str]] = None,
     working_directory: Union[str, Path] = "files",
     osm_way_polygon_features_config: Optional[Union[OsmWayPolygonConfig, dict[str, Any]]] = None,
     silent_mode: bool = False,
+    allow_uncovered_geometry: bool = False,
 ) -> gpd.GeoDataFrame:
     """
     Get a GeoParquet file with OpenStreetMap features within given geometry.
 
     Automatically downloads matching OSM extracts from different sources and returns a single file
     as a result.
 
     Args:
         geometry_filter (BaseGeometry): Geometry filter used to download matching OSM extracts.
         osm_extract_source (OsmExtractSource): A source for automatic downloading of
-            OSM extracts. Can be Geofabrik, BBBike, OSM_fr or any. Defaults to `any`.
+            OSM extracts. Can be Geofabrik, BBBike, OSMfr or any. Defaults to `any`.
         tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
             specifying which tags to download.
             The keys should be OSM tags (e.g. `building`, `amenity`).
             The values should either be `True` for retrieving all objects with the tag,
             string for retrieving a single tag-value pair
             or list of strings for retrieving all values specified in the list.
             `tags={'leisure': 'park}` would return parks from the area.
@@ -641,14 +647,17 @@
         working_directory (Union[str, Path], optional): Directory where to save
             the parsed `*.parquet` files. Defaults to "files".
         osm_way_polygon_features_config (Union[OsmWayPolygonConfig, dict[str, Any]], optional):
             Config used to determine which closed way features are polygons.
             Modifications to this config left are left for experienced OSM users.
             Defaults to predefined "osm_way_polygon_features.json".
         silent_mode (bool): Disable progress bars. Defaults to `False`.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Works only when PbfFileReader is asked to download OSM extracts
+            automatically. Defaults to `False`.
 
     Returns:
         gpd.GeoDataFrame: GeoDataFrame with OSM features.
 
     Examples:
         Get OSM data from the center of Monaco.
 
@@ -700,13 +709,14 @@
     return PbfFileReader(
         tags_filter=tags_filter,
         geometry_filter=geometry_filter,
         working_directory=working_directory,
         osm_way_polygon_features_config=osm_way_polygon_features_config,
         osm_extract_source=osm_extract_source,
         silent_mode=silent_mode,
+        allow_uncovered_geometry=allow_uncovered_geometry,
     ).get_features_gdf_from_geometry(
         keep_all_tags=keep_all_tags,
         explode_tags=explode_tags,
         ignore_cache=ignore_cache,
         filter_osm_ids=filter_osm_ids,
     )
```

### Comparing `quackosm-0.5.1/quackosm/osm_extracts/__init__.py` & `quackosm-0.5.2/quackosm/osm_extracts/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,27 +2,29 @@
 OpenStreetMap extracts.
 
 This module contains iterators for publically available OpenStreetMap `*.osm.pbf` files
 repositories.
 """
 
 import os
+import warnings
 from collections.abc import Iterable
 from enum import Enum
 from functools import partial
 from math import ceil
 from multiprocessing import cpu_count
 from pathlib import Path
 from typing import Optional, Union
 
 import geopandas as gpd
 from pooch import retrieve
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 from tqdm.contrib.concurrent import process_map
 
+from quackosm._exceptions import GeometryNotCoveredError, GeometryNotCoveredWarning
 from quackosm.osm_extracts.bbbike import _get_bbbike_index
 from quackosm.osm_extracts.extract import OpenStreetMapExtract
 from quackosm.osm_extracts.geofabrik import _get_geofabrik_index
 from quackosm.osm_extracts.osm_fr import _get_openstreetmap_fr_index
 
 __all__ = [
     "download_extracts_pbf_files",
@@ -75,107 +77,147 @@
         )
         downloaded_extracts_paths.append(Path(file_path))
     return downloaded_extracts_paths
 
 
 def find_smallest_containing_extracts_total(
     geometry: Union[BaseGeometry, BaseMultipartGeometry],
+    allow_uncovered_geometry: bool = False,
 ) -> list[OpenStreetMapExtract]:
     """
     Find smallest extracts from all OSM extract indexes that contains given polygon.
 
     Iterates all indexes and finds smallest extracts that covers a given geometry.
 
     Args:
         geometry (Union[BaseGeometry, BaseMultipartGeometry]): Geometry to be covered.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Defaults to `False`.
 
     Returns:
         List[OpenStreetMapExtract]: List of extracts name, URL to download it and boundary polygon.
     """
     indexes = gpd.pd.concat(
         [_get_bbbike_index(), _get_geofabrik_index(), _get_openstreetmap_fr_index()]
     )
     indexes.sort_values(by="area", ignore_index=True, inplace=True)
-    return _find_smallest_containing_extracts(geometry, indexes)
+    return _find_smallest_containing_extracts(
+        geometry, indexes, allow_uncovered_geometry=allow_uncovered_geometry
+    )
 
 
 def find_smallest_containing_geofabrik_extracts(
     geometry: Union[BaseGeometry, BaseMultipartGeometry],
+    allow_uncovered_geometry: bool = False,
 ) -> list[OpenStreetMapExtract]:
     """
     Find smallest extracts from Geofabrik that contains given geometry.
 
     Iterates a geofabrik index and finds smallest extracts that covers a given geometry.
 
     Args:
         geometry (Union[BaseGeometry, BaseMultipartGeometry]): Geometry to be covered.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Defaults to `False`.
 
     Returns:
         List[OpenStreetMapExtract]: List of extracts name, URL to download it and boundary polygon.
     """
-    return _find_smallest_containing_extracts(geometry, _get_geofabrik_index())
+    return _find_smallest_containing_extracts(
+        geometry, _get_geofabrik_index(), allow_uncovered_geometry=allow_uncovered_geometry
+    )
 
 
 def find_smallest_containing_openstreetmap_fr_extracts(
     geometry: Union[BaseGeometry, BaseMultipartGeometry],
+    allow_uncovered_geometry: bool = False,
 ) -> list[OpenStreetMapExtract]:
     """
     Find smallest extracts from OpenStreetMap.fr that contains given polygon.
 
     Iterates an osm.fr index and finds smallest extracts that covers a given geometry.
 
     Args:
         geometry (Union[BaseGeometry, BaseMultipartGeometry]): Geometry to be covered.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Defaults to `False`.
 
     Returns:
         List[OpenStreetMapExtract]: List of extracts name, URL to download it and boundary polygon.
     """
-    return _find_smallest_containing_extracts(geometry, _get_openstreetmap_fr_index())
+    return _find_smallest_containing_extracts(
+        geometry, _get_openstreetmap_fr_index(), allow_uncovered_geometry=allow_uncovered_geometry
+    )
 
 
 def find_smallest_containing_bbbike_extracts(
     geometry: Union[BaseGeometry, BaseMultipartGeometry],
+    allow_uncovered_geometry: bool = False,
 ) -> list[OpenStreetMapExtract]:
     """
     Find smallest extracts from BBBike that contains given polygon.
 
     Iterates an BBBike index and finds smallest extracts that covers a given geometry.
 
     Args:
         geometry (Union[BaseGeometry, BaseMultipartGeometry]): Geometry to be covered.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Defaults to `False`.
 
     Returns:
         List[OpenStreetMapExtract]: List of extracts name, URL to download it and boundary polygon.
     """
-    return _find_smallest_containing_extracts(geometry, _get_bbbike_index())
+    return _find_smallest_containing_extracts(
+        geometry, _get_bbbike_index(), allow_uncovered_geometry=allow_uncovered_geometry
+    )
 
 
 OSM_EXTRACT_SOURCE_MATCHING_FUNCTION = {
     OsmExtractSource.any: find_smallest_containing_extracts_total,
     OsmExtractSource.bbbike: find_smallest_containing_bbbike_extracts,
     OsmExtractSource.geofabrik: find_smallest_containing_geofabrik_extracts,
     OsmExtractSource.osm_fr: find_smallest_containing_openstreetmap_fr_extracts,
 }
 
 
 def find_smallest_containing_extract(
-    geometry: Union[BaseGeometry, BaseMultipartGeometry], source: Union[OsmExtractSource, str]
+    geometry: Union[BaseGeometry, BaseMultipartGeometry],
+    source: Union[OsmExtractSource, str],
+    allow_uncovered_geometry: bool = False,
 ) -> list[OpenStreetMapExtract]:
+    """
+    Find smallest extracts from a given OSM source that contains given polygon.
+
+    Iterates an OSM source index and finds smallest extracts that covers a given geometry.
+
+    Args:
+        geometry (Union[BaseGeometry, BaseMultipartGeometry]): Geometry to be covered.
+        source (Union[OsmExtractSource, str]): OSM source name. Can be one of: 'any', 'Geofabrik',
+            'BBBike', 'OSM_fr'.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Defaults to `False`.
+
+    Returns:
+        List[OpenStreetMapExtract]: List of extracts name, URL to download it and boundary polygon.
+    """
     try:
         source_enum = OsmExtractSource(source)
-        return OSM_EXTRACT_SOURCE_MATCHING_FUNCTION[source_enum](geometry)
+        return OSM_EXTRACT_SOURCE_MATCHING_FUNCTION[source_enum](
+            geometry, allow_uncovered_geometry=allow_uncovered_geometry
+        )
     except ValueError as ex:
         raise ValueError(f"Unknown OSM extracts source: {source}.") from ex
 
 
 def _find_smallest_containing_extracts(
     geometry: Union[BaseGeometry, BaseMultipartGeometry],
     polygons_index_gdf: gpd.GeoDataFrame,
     num_of_multiprocessing_workers: int = -1,
     multiprocessing_activation_threshold: Optional[int] = None,
+    allow_uncovered_geometry: bool = False,
 ) -> list[OpenStreetMapExtract]:
     """
     Find smallest set of extracts covering a given geometry.
 
     Iterates a provided extracts index and searches for a smallest set that cover a given geometry.
     It's not guaranteed that this set will be the smallest and there will be no overlaps.
 
@@ -187,14 +229,16 @@
         num_of_multiprocessing_workers (int, optional): Number of workers used for multiprocessing.
             Defaults to -1 which results in a total number of available cpu threads.
             `0` and `1` values disable multiprocessing.
             Similar to `n_jobs` parameter from `scikit-learn` library.
         multiprocessing_activation_threshold (int, optional): Number of gometries required to start
             processing on multiple processes. Activating multiprocessing for a small
             amount of points might not be feasible. Defaults to 100.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Defaults to `False`.
 
     Returns:
         List[OpenStreetMapExtract]: List of extracts covering a given geometry.
     """
     if num_of_multiprocessing_workers == 0:
         num_of_multiprocessing_workers = 1
     elif num_of_multiprocessing_workers < 0:
@@ -212,31 +256,34 @@
     if (
         num_of_multiprocessing_workers > 1
         and total_polygons >= multiprocessing_activation_threshold
     ):
         find_extracts_func = partial(
             _find_smallest_containing_extracts_for_single_geometry,
             polygons_index_gdf=polygons_index_gdf,
+            allow_uncovered_geometry=allow_uncovered_geometry,
         )
 
         force_terminal = os.getenv("FORCE_TERMINAL_MODE", "false").lower() == "true"
         for extract_ids_list in process_map(
             find_extracts_func,
             geometries,
             desc="Finding matching extracts",
             max_workers=num_of_multiprocessing_workers,
             chunksize=ceil(total_polygons / (4 * num_of_multiprocessing_workers)),
-            tqdm_kwargs=dict(disable=True if force_terminal else None),
+            disable=True if force_terminal else None,
         ):
             unique_extracts_ids.update(extract_ids_list)
     else:
         for sub_geometry in geometries:
             unique_extracts_ids.update(
                 _find_smallest_containing_extracts_for_single_geometry(
-                    sub_geometry, polygons_index_gdf
+                    geometry=sub_geometry,
+                    polygons_index_gdf=polygons_index_gdf,
+                    allow_uncovered_geometry=allow_uncovered_geometry,
                 )
             )
 
     extracts_filtered = _filter_extracts(
         geometry,
         unique_extracts_ids,
         polygons_index_gdf,
@@ -244,22 +291,26 @@
         multiprocessing_activation_threshold,
     )
 
     return extracts_filtered
 
 
 def _find_smallest_containing_extracts_for_single_geometry(
-    geometry: BaseGeometry, polygons_index_gdf: gpd.GeoDataFrame
+    geometry: BaseGeometry,
+    polygons_index_gdf: gpd.GeoDataFrame,
+    allow_uncovered_geometry: bool = False,
 ) -> set[str]:
     """
     Find smallest set of extracts covering a given singular geometry.
 
     Args:
         geometry (BaseGeometry): Geometry to be covered.
         polygons_index_gdf (gpd.GeoDataFrame): Index of available extracts.
+        allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't covered
+            by any OSM extract. Defaults to `False`.
 
     Raises:
         RuntimeError: If provided extracts index is empty.
         RuntimeError: If there is no extracts covering a given geometry (singularly or in group).
 
     Returns:
         Set[str]: Selected extract index string values.
@@ -283,15 +334,27 @@
     iterations = 100
     while not geometry_to_cover.is_empty and iterations > 0:
         matching_rows = polygons_index_gdf.loc[
             (~polygons_index_gdf["id"].isin(extracts_ids))
             & (polygons_index_gdf.intersects(geometry_to_cover))
         ]
         if 0 in (len(matching_rows), iterations):
-            raise RuntimeError("Couldn't find extracts matching given geometry.")
+            if not allow_uncovered_geometry:
+                raise GeometryNotCoveredError(
+                    "Couldn't find extracts covering given geometry."
+                    " If it's expected behaviour, you can suppress this error by passing"
+                    " the `allow_uncovered_geometry=True` argument"
+                    " or add `--allow-uncovered-geometry` flag to the CLI command."
+                )
+            warnings.warn(
+                "Couldn't find extracts covering given geometry.",
+                GeometryNotCoveredWarning,
+                stacklevel=0,
+            )
+            break
 
         smallest_extract = matching_rows.iloc[0]
         geometry_to_cover = geometry_to_cover.difference(smallest_extract.geometry)
         extracts_ids.add(smallest_extract.id)
         iterations -= 1
     return extracts_ids
 
@@ -347,15 +410,15 @@
         force_terminal = os.getenv("FORCE_TERMINAL_MODE", "false").lower() == "true"
         for extract_ids_list in process_map(
             filter_extracts_func,
             geometries,
             desc="Filtering extracts",
             max_workers=num_of_multiprocessing_workers,
             chunksize=ceil(total_geometries / (4 * num_of_multiprocessing_workers)),
-            tqdm_kwargs=dict(disable=True if force_terminal else None),
+            disable=True if force_terminal else None,
         ):
             filtered_extracts_ids.update(extract_ids_list)
     else:
         for sub_geometry in geometries:
             filtered_extracts_ids.update(
                 _filter_extracts_for_single_geometry(sub_geometry, sorted_extracts_gdf)
             )
```

### Comparing `quackosm-0.5.1/quackosm/osm_extracts/_poly_parser.py` & `quackosm-0.5.2/quackosm/osm_extracts/_poly_parser.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/osm_extracts/bbbike.py` & `quackosm-0.5.2/quackosm/osm_extracts/bbbike.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/osm_extracts/geofabrik.py` & `quackosm-0.5.2/quackosm/osm_extracts/geofabrik.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/osm_extracts/osm_fr.py` & `quackosm-0.5.2/quackosm/osm_extracts/osm_fr.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/osm_way_polygon_features.json` & `quackosm-0.5.2/quackosm/osm_way_polygon_features.json`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/quackosm/pbf_file_reader.py` & `quackosm-0.5.2/quackosm/pbf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 import shapely.wkt as wktlib
 from geoarrow.pyarrow import io
 from pyarrow_ops import drop_duplicates
 from shapely.geometry import LinearRing, Polygon
 from shapely.geometry.base import BaseGeometry, BaseMultipartGeometry
 
 from quackosm._constants import FEATURES_INDEX, GEOMETRY_COLUMN, WGS84_CRS
+from quackosm._exceptions import EmptyResultWarning
 from quackosm._osm_tags_filters import GroupedOsmTagsFilter, OsmTagsFilter, merge_osm_tags_filter
 from quackosm._osm_way_polygon_features import OsmWayPolygonConfig, parse_dict_to_config_object
 from quackosm._rich_progress import (  # type: ignore[attr-defined]
     TaskProgressBar,
     TaskProgressSpinner,
     log_message,
     show_total_elapsed_time,
@@ -99,14 +100,15 @@
         working_directory: Union[str, Path] = "files",
         osm_way_polygon_features_config: Optional[
             Union[OsmWayPolygonConfig, dict[str, Any]]
         ] = None,
         parquet_compression: str = "snappy",
         osm_extract_source: OsmExtractSource = OsmExtractSource.any,
         silent_mode: bool = False,
+        allow_uncovered_geometry: bool = False,
     ) -> None:
         """
         Initialize PbfFileReader.
 
         Args:
             tags_filter (Union[OsmTagsFilter, GroupedOsmTagsFilter], optional): A dictionary
                 specifying which tags to download.
@@ -126,20 +128,23 @@
                 Config used to determine which closed way features are polygons.
                 Modifications to this config left are left for experienced OSM users.
                 Defaults to predefined "osm_way_polygon_features.json".
             parquet_compression (str): Compression of intermediate parquet files.
                 Check https://duckdb.org/docs/sql/statements/copy#parquet-options for more info.
                 Defaults to "snappy".
             osm_extract_source (OsmExtractSource): A source for automatic downloading of
-                OSM extracts. Can be Geofabrik, BBBike, OSM_fr or any. Defaults to `any`.
+                OSM extracts. Can be Geofabrik, BBBike, OSMfr or any. Defaults to `any`.
             silent_mode (bool): Disable progress bars.
+            allow_uncovered_geometry (bool): Suppress an error if some geometry parts aren't
+                covered by any OSM extract. Defaults to `False`.
         """
         self.tags_filter = tags_filter
         self.merged_tags_filter = merge_osm_tags_filter(tags_filter) if tags_filter else None
         self.geometry_filter = geometry_filter
+        self.allow_uncovered_geometry = allow_uncovered_geometry
         self.osm_extract_source = osm_extract_source
         self.working_directory = Path(working_directory)
         self.working_directory.mkdir(parents=True, exist_ok=True)
         self.connection: duckdb.DuckDBPyConnection = None
         self.encountered_query_exception = False
         self.silent_mode = silent_mode
 
@@ -298,15 +303,17 @@
                 keep_all_tags=keep_all_tags,
                 explode_tags=explode_tags,
                 save_as_wkt=save_as_wkt,
             )
         )
 
         matching_extracts = find_smallest_containing_extract(
-            self.geometry_filter, self.osm_extract_source
+            self.geometry_filter,
+            self.osm_extract_source,
+            allow_uncovered_geometry=self.allow_uncovered_geometry,
         )
 
         if len(matching_extracts) == 1:
             pbf_files = download_extracts_pbf_files(matching_extracts, self.working_directory)
             return self.convert_pbf_to_gpq(
                 pbf_files[0],
                 result_file_path=result_file_path,
@@ -314,52 +321,64 @@
                 explode_tags=explode_tags,
                 ignore_cache=ignore_cache,
                 filter_osm_ids=filter_osm_ids,
                 save_as_wkt=save_as_wkt,
             )
         else:
             if not result_file_path.exists() or ignore_cache:
-                matching_extracts = find_smallest_containing_extract(
-                    self.geometry_filter, self.osm_extract_source
-                )
                 pbf_files = download_extracts_pbf_files(matching_extracts, self.working_directory)
 
                 parsed_geoparquet_files = []
                 for file_path in pbf_files:
                     parsed_geoparquet_file = self.convert_pbf_to_gpq(
                         file_path,
                         keep_all_tags=keep_all_tags,
                         explode_tags=explode_tags,
                         ignore_cache=ignore_cache,
                         filter_osm_ids=filter_osm_ids,
                         save_as_wkt=save_as_wkt,
                     )
                     parsed_geoparquet_files.append(parsed_geoparquet_file)
 
-                with tempfile.TemporaryDirectory(
-                    dir=self.working_directory.resolve()
-                ) as tmp_dir_name:
-                    try:
-                        joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
-                            parsed_geoparquet_files
-                        )
-                    except pa.ArrowInvalid:
-                        tmp_dir_path = Path(tmp_dir_name)
-                        joined_parquet_table = self._drop_duplicated_features_in_joined_table(
-                            parsed_geoparquet_files, tmp_dir_path
-                        )
-
+                if parsed_geoparquet_files:
+                    with tempfile.TemporaryDirectory(
+                        dir=self.working_directory.resolve()
+                    ) as tmp_dir_name:
+                        try:
+                            joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
+                                parsed_geoparquet_files
+                            )
+                        except pa.ArrowInvalid:
+                            tmp_dir_path = Path(tmp_dir_name)
+                            joined_parquet_table = self._drop_duplicated_features_in_joined_table(
+                                parsed_geoparquet_files, tmp_dir_path
+                            )
+                else:
+                    warnings.warn(
+                        "Found 0 extracts covering the geometry. Returning empty result.",
+                        EmptyResultWarning,
+                        stacklevel=0,
+                    )
                     if save_as_wkt:
-                        pq.write_table(joined_parquet_table, result_file_path)
+                        geometry_column = ga.as_wkt(gpd.GeoSeries([], crs=WGS84_CRS))
                     else:
-                        io.write_geoparquet_table(
-                            joined_parquet_table,
-                            result_file_path,
-                            primary_geometry_column=GEOMETRY_COLUMN,
-                        )
+                        geometry_column = ga.as_wkb(gpd.GeoSeries([], crs=WGS84_CRS))
+                    joined_parquet_table = pa.table(
+                        [pa.array([], type=pa.string()), geometry_column],
+                        names=[FEATURES_INDEX, GEOMETRY_COLUMN],
+                    )
+
+                if save_as_wkt:
+                    pq.write_table(joined_parquet_table, result_file_path)
+                else:
+                    io.write_geoparquet_table(
+                        joined_parquet_table,
+                        result_file_path,
+                        primary_geometry_column=GEOMETRY_COLUMN,
+                    )
 
         return Path(result_file_path)
 
     def get_features_gdf(
         self,
         file_paths: Union[str, Path, Iterable[Union[str, Path]]],
         keep_all_tags: bool = False,
@@ -409,28 +428,41 @@
                 keep_all_tags=keep_all_tags,
                 explode_tags=explode_tags,
                 ignore_cache=ignore_cache,
                 filter_osm_ids=filter_osm_ids,
             )
             parsed_geoparquet_files.append(parsed_geoparquet_file)
 
-        with tempfile.TemporaryDirectory(dir=self.working_directory.resolve()) as tmp_dir_name:
-            try:
-                joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
-                    parsed_geoparquet_files
-                )
-            except pa.ArrowInvalid:
-                tmp_dir_path = Path(tmp_dir_name)
-                joined_parquet_table = self._drop_duplicated_features_in_joined_table(
-                    parsed_geoparquet_files, tmp_dir_path
-                )
+        if parsed_geoparquet_files:
+            with tempfile.TemporaryDirectory(dir=self.working_directory.resolve()) as tmp_dir_name:
+                try:
+                    joined_parquet_table = self._drop_duplicated_features_in_pyarrow_table(
+                        parsed_geoparquet_files
+                    )
+                except pa.ArrowInvalid:
+                    tmp_dir_path = Path(tmp_dir_name)
+                    joined_parquet_table = self._drop_duplicated_features_in_joined_table(
+                        parsed_geoparquet_files, tmp_dir_path
+                    )
 
+                gdf_parquet = gpd.GeoDataFrame(
+                    data=joined_parquet_table.drop(GEOMETRY_COLUMN).to_pandas(
+                        maps_as_pydicts="strict"
+                    ),
+                    geometry=ga.to_geopandas(joined_parquet_table.column(GEOMETRY_COLUMN)),
+                ).set_index(FEATURES_INDEX)
+        else:
+            warnings.warn(
+                "Found 0 extracts covering the geometry. Returning empty result.",
+                EmptyResultWarning,
+                stacklevel=0,
+            )
             gdf_parquet = gpd.GeoDataFrame(
-                data=joined_parquet_table.drop(GEOMETRY_COLUMN).to_pandas(maps_as_pydicts="strict"),
-                geometry=ga.to_geopandas(joined_parquet_table.column(GEOMETRY_COLUMN)),
+                data={FEATURES_INDEX: []},
+                geometry=gpd.GeoSeries([], crs=WGS84_CRS),
             ).set_index(FEATURES_INDEX)
 
         return gdf_parquet
 
     def get_features_gdf_from_geometry(
         self,
         keep_all_tags: bool = False,
@@ -475,23 +507,27 @@
         ).set_index(FEATURES_INDEX)
 
         return gdf_parquet
 
     def _drop_duplicated_features_in_pyarrow_table(
         self, parsed_geoparquet_files: list[Path]
     ) -> pa.Table:
-        parquet_tables = [
-            pq.read_table(parsed_parquet_file) for parsed_parquet_file in parsed_geoparquet_files
-        ]
-        joined_parquet_table: pa.Table = pa.concat_tables(parquet_tables, promote_options="default")
-        if joined_parquet_table.num_rows > 0:
-            joined_parquet_table = drop_duplicates(
-                joined_parquet_table, on=["feature_id"], keep="first"
+        with TaskProgressSpinner("Combining results", "", self.silent_mode, skip_step_number=True):
+            parquet_tables = [
+                pq.read_table(parsed_parquet_file)
+                for parsed_parquet_file in parsed_geoparquet_files
+            ]
+            joined_parquet_table: pa.Table = pa.concat_tables(
+                parquet_tables, promote_options="default"
             )
-        return joined_parquet_table
+            if joined_parquet_table.num_rows > 0:
+                joined_parquet_table = drop_duplicates(
+                    joined_parquet_table, on=["feature_id"], keep="first"
+                )
+            return joined_parquet_table
 
     def _drop_duplicated_features_in_joined_table(
         self, parsed_geoparquet_files: list[Path], tmp_dir_path: Path
     ) -> pa.Table:
         if len(parsed_geoparquet_files) == 1:
             return pq.read_table(parsed_geoparquet_files[0])
 
@@ -499,55 +535,68 @@
             parsed_geoparquet_files, key=lambda pq_file: pq_file.stat().st_size, reverse=True
         )
 
         connection = _set_up_duckdb_connection(tmp_dir_path=tmp_dir_path)
 
         try:
             # Attempt 1: read all at once
-            output_file_name = tmp_dir_path / "joined_features_without_duplicates.parquet"
-            parquet_relation = connection.read_parquet(
-                [
-                    str(parsed_geoparquet_file)
-                    for parsed_geoparquet_file in sorted_parsed_geoparquet_files
-                ],
-                union_by_name=True,
-            )
-            query = f"""
-                COPY (
-                    {parquet_relation.sql_query()}
-                    QUALIFY row_number() OVER (PARTITION BY feature_id) = 1
-                ) TO '{output_file_name}' (
-                    FORMAT 'parquet',
-                    PER_THREAD_OUTPUT true,
-                    ROW_GROUP_SIZE 25000,
-                    COMPRESSION '{self.parquet_compression}'
+            with TaskProgressSpinner(
+                "Combining results", "", self.silent_mode, skip_step_number=True
+            ):
+                output_file_name = tmp_dir_path / "joined_features_without_duplicates.parquet"
+                parquet_relation = connection.read_parquet(
+                    [
+                        str(parsed_geoparquet_file)
+                        for parsed_geoparquet_file in sorted_parsed_geoparquet_files
+                    ],
+                    union_by_name=True,
                 )
-            """
-            self._run_query(query, run_in_separate_process=True, tmp_dir_path=tmp_dir_path)
-            return pq.read_table(output_file_name)
-        except MemoryError:
-            # Attempt 2: read one by one
-            result_parquet_files = [sorted_parsed_geoparquet_files[0]]
-            for idx, parsed_geoparquet_file in enumerate(sorted_parsed_geoparquet_files[1:]):
-                current_parquet_file_relation = connection.read_parquet(str(parsed_geoparquet_file))
-                filtered_result_parquet_file = tmp_dir_path / f"sub_file_{idx}"
                 query = f"""
                     COPY (
-                        {current_parquet_file_relation.sql_query()}
-                        ANTI JOIN read_parquet({[str(pq_file) for pq_file in result_parquet_files]})
-                        USING (feature_id)
-                    ) TO '{filtered_result_parquet_file}' (
+                        {parquet_relation.sql_query()}
+                        QUALIFY row_number() OVER (PARTITION BY feature_id) = 1
+                    ) TO '{output_file_name}' (
                         FORMAT 'parquet',
                         PER_THREAD_OUTPUT true,
                         ROW_GROUP_SIZE 25000,
                         COMPRESSION '{self.parquet_compression}'
                     )
                 """
-                connection.sql(query)
-                result_parquet_files.extend(filtered_result_parquet_file.glob("*.parquet"))
+                self._run_query(query, run_in_separate_process=True, tmp_dir_path=tmp_dir_path)
+                return pq.read_table(output_file_name)
+        except MemoryError:
+            # Attempt 2: read one by one
+            result_parquet_files = [sorted_parsed_geoparquet_files[0]]
+            with TaskProgressBar(
+                "Combining results", "", self.silent_mode, skip_step_number=True
+            ) as bar:
+                for idx, parsed_geoparquet_file in bar.track(
+                    enumerate(sorted_parsed_geoparquet_files[1:])
+                ):
+                    current_parquet_file_relation = connection.read_parquet(
+                        str(parsed_geoparquet_file)
+                    )
+                    filtered_result_parquet_file = tmp_dir_path / f"sub_file_{idx}"
+                    result_parquet_files_strings = [
+                        str(pq_file) for pq_file in result_parquet_files
+                    ]
+                    query = f"""
+                        COPY (
+                            {current_parquet_file_relation.sql_query()}
+                            ANTI JOIN read_parquet({result_parquet_files_strings})
+                            USING (feature_id)
+                        ) TO '{filtered_result_parquet_file}' (
+                            FORMAT 'parquet',
+                            PER_THREAD_OUTPUT true,
+                            ROW_GROUP_SIZE 25000,
+                            COMPRESSION '{self.parquet_compression}'
+                        )
+                    """
+                    connection.sql(query)
+                    result_parquet_files.extend(filtered_result_parquet_file.glob("*.parquet"))
         return pq.read_table(result_parquet_files)
 
     def _parse_pbf_file(
         self,
         pbf_path: Union[str, Path],
         result_file_path: Path,
         filter_osm_ids: list[str],
```

### Comparing `quackosm-0.5.1/tests/base/test_cli.py` & `quackosm-0.5.2/tests/base/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -514,14 +514,27 @@
         "--geom-filter-file",
         geometry_boundary_file_path(),
         "--osm-way-polygon-config",
         osm_way_config_file_path(),
     ],
     "files/6e3ec5872bf41c2c44698fcf71266971c552d13feea19c3714e171bcd7a2b2c8_nofilter_compact.geoparquet",
 )  # type: ignore
+@P.case(
+    "Allow not covered geometry",
+    [
+        "--geom-filter-wkt",
+        (
+            "POLYGON ((-43.064 29.673, -43.064 29.644, -43.017 29.644,"
+            " -43.017 29.673, -43.064 29.673))"
+        ),
+        "--allow-uncovered-geometry",
+        "--ignore-cache",
+    ],
+    "files/fa44926c5f128cd438ecbe06d29644849a9de323703076b8ac62ffd7a0747e50_nofilter_compact.geoparquet",
+)  # type: ignore
 def test_proper_args_without_pbf(args: list[str], expected_result: str) -> None:
     """Test if runs properly with options."""
     result = runner.invoke(cli.app, [*args])
     print(result.stdout)
 
     assert result.exit_code == 0
     assert str(Path(expected_result)) in result.stdout
```

### Comparing `quackosm-0.5.1/tests/base/test_osm_extracts.py` & `quackosm-0.5.2/tests/base/test_osm_extracts.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,20 @@
 from unittest import TestCase
 
 import pytest
 from parametrization import Parametrization as P
 from shapely import from_wkt
 from shapely.geometry.base import BaseGeometry
 
-from quackosm.osm_extracts import OsmExtractSource, find_smallest_containing_extract
+from quackosm._exceptions import GeometryNotCoveredError, GeometryNotCoveredWarning
+from quackosm.osm_extracts import (
+    OsmExtractSource,
+    find_smallest_containing_extract,
+    find_smallest_containing_extracts_total,
+)
 
 ut = TestCase()
 
 
 @P.parameters("value")  # type: ignore
 @P.case(
     "Base any",
@@ -25,14 +30,18 @@
     "Base Geofabrik",
     "Geofabrik",
 )  # type: ignore
 @P.case(
     "Case insensitive Geofabrik",
     "GEOFABRIK",
 )  # type: ignore
+@P.case(
+    "OSM fr without underscore",
+    "osmfr",
+)  # type: ignore
 def test_proper_osm_extract_source(value: str):
     """Test if OsmExtractSource is parsed correctly."""
     OsmExtractSource(value)
 
 
 def test_wrong_osm_extract_source():  # type: ignore
     """Test if cannot load incorrect OsmExtractSource."""
@@ -128,7 +137,26 @@
 def test_multiple_smallest_extracts(
     source: str, geometry: BaseGeometry, expected_extract_ids: list[str]
 ):
     """Test if extracts matching works correctly for geometries between borders."""
     extracts = find_smallest_containing_extract(geometry, source)
     assert len(extracts) == len(expected_extract_ids)
     ut.assertListEqual([extract.id for extract in extracts], expected_extract_ids)
+
+
+@pytest.mark.parametrize(
+    "expectation,allow_uncovered_geometry",
+    [
+        (pytest.raises(GeometryNotCoveredError), False),
+        (pytest.warns(GeometryNotCoveredWarning), True),
+    ],
+)  # type: ignore
+def test_uncovered_geometry_extract(expectation, allow_uncovered_geometry: bool):
+    """Test if raises errors as expected when geometry can't be covered."""
+    with expectation:
+        geometry = from_wkt(
+            "POLYGON ((-43.064 29.673, -43.064 29.644, -43.017 29.644,"
+            " -43.017 29.673, -43.064 29.673))"
+        )
+        find_smallest_containing_extracts_total(
+            geometry=geometry, allow_uncovered_geometry=allow_uncovered_geometry
+        )
```

### Comparing `quackosm-0.5.1/tests/base/test_pbf_file_reader.py` & `quackosm-0.5.2/tests/base/test_pbf_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from shapely.geometry.base import BaseGeometry
 from shapely.ops import unary_union
 from srai.geometry import remove_interiors
 from srai.loaders.download import download_file
 from srai.loaders.osm_loaders.filters import GEOFABRIK_LAYERS, HEX2VEC_FILTER
 
 from quackosm._constants import FEATURES_INDEX
+from quackosm._exceptions import GeometryNotCoveredError, GeometryNotCoveredWarning
 from quackosm._osm_tags_filters import GroupedOsmTagsFilter, OsmTagsFilter
 from quackosm.cli import (
     GeocodeGeometryParser,
     GeohashGeometryParser,
     H3GeometryParser,
     S2GeometryParser,
 )
@@ -207,14 +208,34 @@
         file_paths=[Path(__file__).parent.parent / "test_files" / file_name],
         ignore_cache=True,
         filter_osm_ids=filter_osm_ids,
     )
     assert len(features_gdf) == expected_result_length
 
 
+@pytest.mark.parametrize(
+    "expectation,allow_uncovered_geometry",
+    [
+        (pytest.raises(GeometryNotCoveredError), False),
+        (pytest.warns(GeometryNotCoveredWarning), True),
+    ],
+)  # type: ignore
+def test_uncovered_geometry_extract(expectation, allow_uncovered_geometry: bool):
+    """Test if raises errors as expected when geometry can't be covered."""
+    with expectation:
+        geometry = from_wkt(
+            "POLYGON ((-43.064 29.673, -43.064 29.644, -43.017 29.644,"
+            " -43.017 29.673, -43.064 29.673))"
+        )
+        features_gdf = PbfFileReader(
+            geometry_filter=geometry, allow_uncovered_geometry=allow_uncovered_geometry
+        ).get_features_gdf_from_geometry(ignore_cache=True)
+        assert len(features_gdf) == 0
+
+
 @pytest.mark.parametrize(  # type: ignore
     "filter_osm_id,osm_tags_filter,keep_all_tags,expected_tags_keys",
     [
         ("way/389888402", {"building": "apartments"}, False, ["building"]),
         (
             "way/389888402",
             {"building": "apartments"},
```

### Comparing `quackosm-0.5.1/tests/benchmark/test_big_file.py` & `quackosm-0.5.2/tests/benchmark/test_big_file.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/tests/optional_imports/test_optional_cli_dependency.py` & `quackosm-0.5.2/tests/optional_imports/test_optional_cli_dependency.py`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf` & `quackosm-0.5.2/tests/test_files/aa756ad3a961ba6d9da46c712b0d979d0c7d4768641ceea7409b287e2d18a48f.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf` & `quackosm-0.5.2/tests/test_files/d17f922ed15e9609013a6b895e1e7af2d49158f03586f2c675d17b760af3452e.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf` & `quackosm-0.5.2/tests/test_files/eb2848d259345ce7dfe8af34fd1ab24503bb0b952e04e872c87c55550fa50fbf.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/tests/test_files/monaco.osm.pbf` & `quackosm-0.5.2/tests/test_files/monaco.osm.pbf`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/tests/test_files/monaco_boundary.geojson` & `quackosm-0.5.2/tests/test_files/monaco_boundary.geojson`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/tests/test_files/osmconf.ini` & `quackosm-0.5.2/tests/test_files/osmconf.ini`

 * *Files identical despite different names*

### Comparing `quackosm-0.5.1/PKG-INFO` & `quackosm-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuackOSM
-Version: 0.5.1
+Version: 0.5.2
 Summary: An open-source tool for reading OpenStreetMap PBF files using DuckDB
 Author-Email: Kamil Raczycki <kraczycki@kraina.ai>
 License: Apache-2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: GIS
```

