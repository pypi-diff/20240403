# Comparing `tmp/PygameToolsBox-1.0.2.tar.gz` & `tmp/PygameToolsBox-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PygameToolsBox-1.0.2.tar", last modified: Tue Mar 26 21:00:05 2024, max compression
+gzip compressed data, was "PygameToolsBox-1.0.3.tar", last modified: Wed Apr  3 15:11:23 2024, max compression
```

## Comparing `PygameToolsBox-1.0.2.tar` & `PygameToolsBox-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 21:00:05.737959 PygameToolsBox-1.0.2/
--rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2524 2024-03-26 21:00:05.736954 PygameToolsBox-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-03-26 21:00:05.702958 PygameToolsBox-1.0.2/PygameToolsBox/
--rw-rw-rw-   0        0        0       21 2024-03-26 20:55:09.000000 PygameToolsBox-1.0.2/PygameToolsBox/__init__.py
--rw-rw-rw-   0        0        0     2672 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.2/PygameToolsBox/parallax_bg.py
--rw-rw-rw-   0        0        0     3691 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.2/PygameToolsBox/spritesheet.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:00:05.725969 PygameToolsBox-1.0.2/PygameToolsBox.egg-info/
--rw-rw-rw-   0        0        0     2524 2024-03-26 21:00:05.000000 PygameToolsBox-1.0.2/PygameToolsBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2024-03-26 21:00:05.000000 PygameToolsBox-1.0.2/PygameToolsBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 21:00:05.000000 PygameToolsBox-1.0.2/PygameToolsBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-03-26 21:00:05.000000 PygameToolsBox-1.0.2/PygameToolsBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-03-26 21:00:05.000000 PygameToolsBox-1.0.2/PygameToolsBox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1918 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.2/README.md
--rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-26 21:00:05.737959 PygameToolsBox-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.619131 PygameToolsBox-1.0.3/
+-rw-rw-rw-   0        0        0     1091 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2524 2024-04-03 15:11:23.618010 PygameToolsBox-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.594207 PygameToolsBox-1.0.3/PygameToolsBox/
+-rw-rw-rw-   0        0        0       21 2024-04-03 15:10:42.000000 PygameToolsBox-1.0.3/PygameToolsBox/__init__.py
+-rw-rw-rw-   0        0        0     3098 2024-04-03 15:09:03.000000 PygameToolsBox-1.0.3/PygameToolsBox/animated_object.py
+-rw-rw-rw-   0        0        0      225 2024-03-27 00:15:04.000000 PygameToolsBox-1.0.3/PygameToolsBox/mask_image.py
+-rw-rw-rw-   0        0        0     2834 2024-04-01 23:37:04.000000 PygameToolsBox-1.0.3/PygameToolsBox/parallax_bg.py
+-rw-rw-rw-   0        0        0     3691 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.3/PygameToolsBox/spritesheet.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.616969 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/
+-rw-rw-rw-   0        0        0     2524 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      371 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-04-03 15:11:23.000000 PygameToolsBox-1.0.3/PygameToolsBox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1918 2024-03-26 20:21:58.000000 PygameToolsBox-1.0.3/README.md
+-rw-rw-rw-   0        0        0      773 2024-03-26 20:57:41.000000 PygameToolsBox-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 15:11:23.619131 PygameToolsBox-1.0.3/setup.cfg
```

### Comparing `PygameToolsBox-1.0.2/LICENSE` & `PygameToolsBox-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.2/PKG-INFO` & `PygameToolsBox-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.0.2/PygameToolsBox/parallax_bg.py` & `PygameToolsBox-1.0.3/PygameToolsBox/parallax_bg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import math
 from pathlib import Path
 
 import pygame.image
 from pygame import Surface, Rect
 
 
-class Background:
-    def __init__(self, image: Surface):
+class _Background:
+    def __init__(self, image: Surface, offset_y: int):
         self.image = image
+        self.offset_y = offset_y
         self.width = image.get_width()
         self.height = image.get_height()
         self.scroll = 0
         self.speed = 1
 
     def update(self, scroll: int):
         self.scroll += scroll
@@ -36,23 +36,25 @@
     This class allows you to manage background images and apply a parallax effect.
     We must add the background images starting with the one that will be most in the background.
     Then we stack the images to finish with the one on top.
     By default, the speed is adjusted to 5, but it can be changed
     """
 
     def __init__(self):
-        self._backgrounds = list[Background]()
+        self._backgrounds = list[_Background]()
         self.speed: int = 5
 
-    def add_background(self, image: Path):
+    def add_background(self, image: Path, offset_y: int = 0):
         """
-        :param image: Image source path with filename
+        Params:
+            image: Image source path with filename
+            offset_y: Shifting the image in vertical position
         """
 
-        image = Background(pygame.image.load(image).convert_alpha())
+        image = _Background(pygame.image.load(image).convert_alpha(), offset_y)
         image.speed += len(self._backgrounds) * 0.2
         self._backgrounds.append(image)
 
     def update(self, scroll_direction: int):
         """
         Params:
             scroll_direction (int):width = {int} 1782
@@ -66,11 +68,11 @@
     def draw(self, win: Surface):
         """
         Params win (pygame.Surface):
             The object takes care of stacking the background images in the order of insertion.
             Each image scrolls faster and faster as it nears the top of the stack
         """
         for i, image in enumerate(self._backgrounds):
-            rect = Rect(image.scroll * image.speed, 0, image.scroll + image.width, image.height)
+            rect = Rect(image.scroll * image.speed, 0 + image.offset_y, image.scroll + image.width, image.height)
             win.blit(image.image, rect)  # Dessiner l'image avec le scrolling
             image.cover_left(win)
             image.cover_right(win)
```

### Comparing `PygameToolsBox-1.0.2/PygameToolsBox/spritesheet.py` & `PygameToolsBox-1.0.3/PygameToolsBox/spritesheet.py`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.2/PygameToolsBox.egg-info/PKG-INFO` & `PygameToolsBox-1.0.3/PygameToolsBox.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PygameToolsBox
-Version: 1.0.2
+Version: 1.0.3
 Summary: Library for manage sprite sheet, and pallax background
 Author-email: FranckSix <francksix@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FranckSix/PygameSpriteTools
 Project-URL: Issues, https://github.com/FranckSix/PygameSpriteTools/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `PygameToolsBox-1.0.2/README.md` & `PygameToolsBox-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `PygameToolsBox-1.0.2/pyproject.toml` & `PygameToolsBox-1.0.3/pyproject.toml`

 * *Files identical despite different names*

