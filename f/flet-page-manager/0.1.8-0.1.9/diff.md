# Comparing `tmp/flet_page_manager-0.1.8-py312-none-any.whl.zip` & `tmp/flet_page_manager-0.1.9-py312-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 3712 bytes, number of entries: 10
+Zip file size: 3703 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        2 b- defN 16-Jan-01 00:00 .gitignore
--rw-r--r--  2.0 unx      426 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx      426 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.9.dist-info/WHEEL
 -rw-r--r--  2.0 unx      220 b- defN 16-Jan-01 00:00 page_manager/__init__.py
 -rw-r--r--  2.0 unx       84 b- defN 16-Jan-01 00:00 page_manager/exception.py
--rw-r--r--  2.0 unx     2827 b- defN 16-Jan-01 00:00 page_manager/manager.py
+-rw-r--r--  2.0 unx     2804 b- defN 16-Jan-01 00:00 page_manager/manager.py
 -rw-r--r--  2.0 unx       51 b- defN 16-Jan-01 00:00 page_manager/pages/__init__.py
--rw-r--r--  2.0 unx      607 b- defN 16-Jan-01 00:00 page_manager/pages/base.py
+-rw-r--r--  2.0 unx      603 b- defN 16-Jan-01 00:00 page_manager/pages/base.py
 -rw-r--r--  2.0 unx      234 b- defN 16-Jan-01 00:00 page_manager/state.py
-?rw-------  2.0 unx      783 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.8.dist-info/RECORD
-10 files, 5326 bytes uncompressed, 2370 bytes compressed:  55.5%
+?rw-------  2.0 unx      783 b- defN 16-Jan-01 00:00 flet_page_manager-0.1.9.dist-info/RECORD
+10 files, 5299 bytes uncompressed, 2361 bytes compressed:  55.4%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
 Filename: .gitignore
 Comment: 
 
-Filename: flet_page_manager-0.1.8.dist-info/METADATA
+Filename: flet_page_manager-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: flet_page_manager-0.1.8.dist-info/WHEEL
+Filename: flet_page_manager-0.1.9.dist-info/WHEEL
 Comment: 
 
 Filename: page_manager/__init__.py
 Comment: 
 
 Filename: page_manager/exception.py
 Comment: 
@@ -21,11 +21,11 @@
 
 Filename: page_manager/pages/base.py
 Comment: 
 
 Filename: page_manager/state.py
 Comment: 
 
-Filename: flet_page_manager-0.1.8.dist-info/RECORD
+Filename: flet_page_manager-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## page_manager/manager.py

```diff
@@ -3,17 +3,15 @@
 from flet import AppView
 import asyncio
 from typing import TYPE_CHECKING, TypeVar
 from loguru import logger
 import sys
 from .exception import PageException
 from .state import StateBase
-
-if TYPE_CHECKING:
-    from .pages import PageBase
+from .pages import PageBase
 
 
 class PageManager[StateT: StateBase]:
     logger = logger
 
     page_mapping: dict[str, type[PageBase]] = {}
```

## page_manager/pages/base.py

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import flet as ft
 from typing import TYPE_CHECKING
+from ..state import StateBase
 
 if TYPE_CHECKING:
     from ..manager import PageManager
-    from ..state import StateBase
 
 
 class PageBase[StateT: StateBase]:
     async def init(self, page: ft.Page, pm: PageManager[StateT]):
         pm.state.running_pages.append(page)
         await page.window_center_async()
```

