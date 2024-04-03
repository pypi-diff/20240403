# Comparing `tmp/pygame_util-1.0.0.tar.gz` & `tmp/pygame_util-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_util-1.0.0.tar", max compression
+gzip compressed data, was "pygame_util-1.0.1.tar", max compression
```

## Comparing `pygame_util-1.0.0.tar` & `pygame_util-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2024-04-01 21:23:18.515915 pygame_util-1.0.0/LICENSE
--rw-r--r--   0        0        0     1067 2024-04-01 22:28:43.746940 pygame_util-1.0.0/LICENSE.txt
--rw-r--r--   0        0        0       14 2024-04-01 22:03:58.556792 pygame_util-1.0.0/README.md
--rw-r--r--   0        0        0      241 2024-04-01 22:08:08.689356 pygame_util-1.0.0/pygame_util/__init__.py
--rw-r--r--   0        0        0      606 2024-04-01 21:25:21.373656 pygame_util-1.0.0/pygame_util/color.py
--rw-r--r--   0        0        0       67 2024-04-01 22:37:21.939093 pygame_util-1.0.0/pygame_util/dist/pygame_util-0.1.0.tar.gz
--rw-r--r--   0        0        0      657 2024-04-01 21:33:07.078073 pygame_util-1.0.0/pygame_util/image.py
--rw-r--r--   0        0        0     9123 2024-04-01 22:36:15.629750 pygame_util-1.0.0/pygame_util/poetry.lock
--rw-r--r--   0        0        0     2223 2024-04-01 21:25:21.374293 pygame_util-1.0.0/pygame_util/position.py
--rw-r--r--   0        0        0     3695 2024-04-01 21:33:07.031327 pygame_util-1.0.0/pygame_util/text.py
--rw-r--r--   0        0        0     1843 2024-04-01 21:25:21.374949 pygame_util-1.0.0/pygame_util/timer.py
--rw-r--r--   0        0        0     1091 2024-04-01 21:33:06.978483 pygame_util-1.0.0/pygame_util/window.py
--rw-r--r--   0        0        0      314 2024-04-01 22:39:15.262032 pygame_util-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 pygame_util-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-01 21:23:18.515915 pygame_util-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1067 2024-04-01 22:28:43.746940 pygame_util-1.0.1/LICENSE.txt
+-rw-r--r--   0        0        0       14 2024-04-01 22:03:58.556792 pygame_util-1.0.1/README.md
+-rw-r--r--   0        0        0      241 2024-04-01 22:08:08.689356 pygame_util-1.0.1/pygame_util/__init__.py
+-rw-r--r--   0        0        0      606 2024-04-01 21:25:21.373656 pygame_util-1.0.1/pygame_util/color.py
+-rw-r--r--   0        0        0       67 2024-04-01 22:37:21.939093 pygame_util-1.0.1/pygame_util/dist/pygame_util-0.1.0.tar.gz
+-rw-r--r--   0        0        0      659 2024-04-03 16:26:44.962419 pygame_util-1.0.1/pygame_util/image.py
+-rw-r--r--   0        0        0     9123 2024-04-01 22:36:15.629750 pygame_util-1.0.1/pygame_util/poetry.lock
+-rw-r--r--   0        0        0     2223 2024-04-01 21:25:21.374293 pygame_util-1.0.1/pygame_util/position.py
+-rw-r--r--   0        0        0     3697 2024-04-03 16:26:44.905329 pygame_util-1.0.1/pygame_util/text.py
+-rw-r--r--   0        0        0     1843 2024-04-01 21:25:21.374949 pygame_util-1.0.1/pygame_util/timer.py
+-rw-r--r--   0        0        0     1093 2024-04-03 16:26:43.341380 pygame_util-1.0.1/pygame_util/window.py
+-rw-r--r--   0        0        0      314 2024-04-03 16:29:09.999849 pygame_util-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 pygame_util-1.0.1/PKG-INFO
```

### Comparing `pygame_util-1.0.0/LICENSE` & `pygame_util-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.0/LICENSE.txt` & `pygame_util-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.0/pygame_util/color.py` & `pygame_util-1.0.1/pygame_util/color.py`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.0/pygame_util/image.py` & `pygame_util-1.0.1/pygame_util/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from os import path
 
 import pygame
-from color import Color
+
+from .color import Color
 
 
 def load_image(
     img_name: str,
     img_dir: str,
     ext: str = ".png",
     colorkey: tuple[int, int, int] = None,
```

### Comparing `pygame_util-1.0.0/pygame_util/poetry.lock` & `pygame_util-1.0.1/pygame_util/poetry.lock`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.0/pygame_util/position.py` & `pygame_util-1.0.1/pygame_util/position.py`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.0/pygame_util/text.py` & `pygame_util-1.0.1/pygame_util/text.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
 import pygame
-from color import Color
+
+from .color import Color
 
 
 @dataclass
 class TextStyle:
     font_file: str = pygame.font.get_default_font()
     size: int = 30
     antialias: bool = True
```

### Comparing `pygame_util-1.0.0/pygame_util/timer.py` & `pygame_util-1.0.1/pygame_util/timer.py`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.0/pygame_util/window.py` & `pygame_util-1.0.1/pygame_util/window.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from dataclasses import dataclass
 
 import pygame
-from color import Color
+
+from .color import Color
 
 
 @dataclass
 class Window:
     """
     A class for handling window settings.
     """
```

