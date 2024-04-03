# Comparing `tmp/colorez-1.1.1.tar.gz` & `tmp/colorez-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorez-1.1.1.tar", last modified: Tue Mar 26 21:50:49 2024, max compression
+gzip compressed data, was "colorez-1.1.2.tar", last modified: Wed Apr  3 13:44:53 2024, max compression
```

## Comparing `colorez-1.1.1.tar` & `colorez-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 21:50:49.736111 colorez-1.1.1/
--rw-rw-rw-   0        0        0     2561 2024-03-26 21:50:49.735106 colorez-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1950 2024-03-26 21:34:28.000000 colorez-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 21:50:49.723545 colorez-1.1.1/colorez/
--rw-rw-rw-   0        0        0      774 2024-03-26 21:50:38.000000 colorez-1.1.1/colorez/__init__.py
--rw-rw-rw-   0        0        0    60559 2024-03-26 21:50:27.000000 colorez-1.1.1/colorez/colorez.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:50:49.734604 colorez-1.1.1/colorez.egg-info/
--rw-rw-rw-   0        0        0     2561 2024-03-26 21:50:49.000000 colorez-1.1.1/colorez.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      187 2024-03-26 21:50:49.000000 colorez-1.1.1/colorez.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 21:50:49.000000 colorez-1.1.1/colorez.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-03-26 21:50:49.000000 colorez-1.1.1/colorez.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      794 2024-03-26 21:50:44.000000 colorez-1.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-26 21:50:49.736111 colorez-1.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 13:44:53.614513 colorez-1.1.2/
+-rw-rw-rw-   0        0        0     2561 2024-04-03 13:44:53.614010 colorez-1.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1950 2024-03-26 21:34:28.000000 colorez-1.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 13:44:53.600438 colorez-1.1.2/colorez/
+-rw-rw-rw-   0        0        0      774 2024-04-03 13:44:30.000000 colorez-1.1.2/colorez/__init__.py
+-rw-rw-rw-   0        0        0    60652 2024-04-03 13:42:11.000000 colorez-1.1.2/colorez/colorez.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:44:53.613004 colorez-1.1.2/colorez.egg-info/
+-rw-rw-rw-   0        0        0     2561 2024-04-03 13:44:53.000000 colorez-1.1.2/colorez.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      187 2024-04-03 13:44:53.000000 colorez-1.1.2/colorez.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 13:44:53.000000 colorez-1.1.2/colorez.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 13:44:53.000000 colorez-1.1.2/colorez.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      794 2024-04-03 13:44:36.000000 colorez-1.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 13:44:53.614513 colorez-1.1.2/setup.cfg
```

### Comparing `colorez-1.1.1/PKG-INFO` & `colorez-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorez
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple addition of color to the builtin print and input functions
 Author: CodingYuno
 Project-URL: Source Code, https://github.com/CodingYuno/colorez/
 Project-URL: Issue Tracker, https://github.com/CodingYuno/colorez/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `colorez-1.1.1/README.md` & `colorez-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `colorez-1.1.1/colorez/__init__.py` & `colorez-1.1.2/colorez/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 
 colorez.py adds simple addition of color to the builtin print and input functions
 
 """
 
 __title__ = 'colorez'
 __description__ = "Simple addition of color to the builtin print and input functions"
-__version__ = '1.1.1'
+__version__ = '1.1.2'
 __author__ = 'CodingYuno'
 
 from .colorez import color_print, color_input, Color, line_print, reset_style, print_gradient, test_terminal_color_set, view_color_names, object_print, style
```

### Comparing `colorez-1.1.1/colorez/colorez.py` & `colorez-1.1.2/colorez/colorez.py`

 * *Files 1% similar despite different names*

```diff
@@ -585,14 +585,18 @@
 
     def __repr__(self):
         return f"<Color string='{self.string}'>"
 
     def __iadd__(self, other):
         self.string += str(other)
         return self
+    
+    def __add__(self, other):
+        self.string += str(other)
+        return self
 
 
 _last_identifier = None
 _first_ever_print = True
 
 
 def line_print(*args, sep: str = " ", color: str = "#FFFFFF", bg_color: str or int = None, bold: bool = False,
```

### Comparing `colorez-1.1.1/colorez.egg-info/PKG-INFO` & `colorez-1.1.2/colorez.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorez
-Version: 1.1.1
+Version: 1.1.2
 Summary: Simple addition of color to the builtin print and input functions
 Author: CodingYuno
 Project-URL: Source Code, https://github.com/CodingYuno/colorez/
 Project-URL: Issue Tracker, https://github.com/CodingYuno/colorez/issues/
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `colorez-1.1.1/pyproject.toml` & `colorez-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "colorez"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="CodingYuno"},
 ]
 description = "Simple addition of color to the builtin print and input functions"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

