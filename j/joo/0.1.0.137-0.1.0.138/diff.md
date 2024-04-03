# Comparing `tmp/joo-0.1.0.137.tar.gz` & `tmp/joo-0.1.0.138.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joo-0.1.0.137.tar", last modified: Sat Mar 30 12:03:54 2024, max compression
+gzip compressed data, was "joo-0.1.0.138.tar", last modified: Wed Apr  3 08:50:30 2024, max compression
```

## Comparing `joo-0.1.0.137.tar` & `joo-0.1.0.138.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-30 12:03:54.968357 joo-0.1.0.137/
--rw-rw-rw-   0        0        0      625 2024-03-30 12:03:54.966203 joo-0.1.0.137/PKG-INFO
--rw-rw-rw-   0        0        0       78 2024-03-30 12:03:52.000000 joo-0.1.0.137/README.md
-drwxrwxrwx   0        0        0        0 2024-03-30 12:03:54.890831 joo-0.1.0.137/lib/
-drwxrwxrwx   0        0        0        0 2024-03-30 12:03:54.928307 joo-0.1.0.137/lib/joo/
--rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.137/lib/joo/LICENSE
--rw-rw-rw-   0        0        0     3421 2024-03-30 08:30:13.000000 joo-0.1.0.137/lib/joo/__init__.py
--rw-rw-rw-   0        0        0      759 2024-03-30 12:03:52.000000 joo-0.1.0.137/lib/joo/__version__.py
--rw-rw-rw-   0        0        0     3060 2024-03-30 11:42:36.000000 joo-0.1.0.137/lib/joo/cli.py
--rw-rw-rw-   0        0        0    11405 2024-03-30 08:30:13.000000 joo-0.1.0.137/lib/joo/logging.py
-drwxrwxrwx   0        0        0        0 2024-03-30 12:03:54.964209 joo-0.1.0.137/lib/joo/scraping/
--rw-rw-rw-   0        0        0     4374 2024-03-30 08:30:13.000000 joo-0.1.0.137/lib/joo/scraping/__init__.py
--rw-rw-rw-   0        0        0     4927 2024-03-30 08:30:13.000000 joo-0.1.0.137/lib/joo/scraping/http.py
--rw-rw-rw-   0        0        0    10402 2024-03-30 08:30:13.000000 joo-0.1.0.137/lib/joo/scraping/selenium.py
--rw-rw-rw-   0        0        0    12263 2024-03-30 11:54:03.000000 joo-0.1.0.137/lib/joo/sysutil.py
-drwxrwxrwx   0        0        0        0 2024-03-30 12:03:54.956232 joo-0.1.0.137/lib/joo.egg-info/
--rw-rw-rw-   0        0        0      625 2024-03-30 12:03:53.000000 joo-0.1.0.137/lib/joo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2024-03-30 12:03:54.000000 joo-0.1.0.137/lib/joo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-30 12:03:53.000000 joo-0.1.0.137/lib/joo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-03-30 12:03:53.000000 joo-0.1.0.137/lib/joo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-30 12:03:54.968357 joo-0.1.0.137/setup.cfg
--rw-rw-rw-   0        0        0     1424 2024-03-30 12:03:52.000000 joo-0.1.0.137/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.627232 joo-0.1.0.138/
+-rw-rw-rw-   0        0        0      625 2024-04-03 08:50:30.624237 joo-0.1.0.138/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2024-04-03 08:50:27.000000 joo-0.1.0.138/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.542096 joo-0.1.0.138/lib/
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.569032 joo-0.1.0.138/lib/joo/
+-rw-rw-rw-   0        0        0     1102 2024-03-27 11:42:14.000000 joo-0.1.0.138/lib/joo/LICENSE
+-rw-rw-rw-   0        0        0     4178 2024-04-03 08:50:27.000000 joo-0.1.0.138/lib/joo/__init__.py
+-rw-rw-rw-   0        0        0      759 2024-04-03 08:50:27.000000 joo-0.1.0.138/lib/joo/__version__.py
+-rw-rw-rw-   0        0        0     2780 2024-04-03 08:50:27.000000 joo-0.1.0.138/lib/joo/cli.py
+-rw-rw-rw-   0        0        0    11405 2024-03-30 08:30:13.000000 joo-0.1.0.138/lib/joo/logging.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.620250 joo-0.1.0.138/lib/joo/scraping/
+-rw-rw-rw-   0        0        0     4374 2024-03-30 08:30:13.000000 joo-0.1.0.138/lib/joo/scraping/__init__.py
+-rw-rw-rw-   0        0        0     4927 2024-03-30 08:30:13.000000 joo-0.1.0.138/lib/joo/scraping/http.py
+-rw-rw-rw-   0        0        0    10402 2024-03-30 08:30:13.000000 joo-0.1.0.138/lib/joo/scraping/selenium.py
+-rw-rw-rw-   0        0        0    12263 2024-03-30 12:37:13.000000 joo-0.1.0.138/lib/joo/sysutil.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:50:30.606935 joo-0.1.0.138/lib/joo.egg-info/
+-rw-rw-rw-   0        0        0      625 2024-04-03 08:50:28.000000 joo-0.1.0.138/lib/joo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2024-04-03 08:50:29.000000 joo-0.1.0.138/lib/joo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:50:28.000000 joo-0.1.0.138/lib/joo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-03 08:50:28.000000 joo-0.1.0.138/lib/joo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:50:30.627232 joo-0.1.0.138/setup.cfg
+-rw-rw-rw-   0        0        0     1424 2024-04-03 08:50:27.000000 joo-0.1.0.138/setup.py
```

### Comparing `joo-0.1.0.137/PKG-INFO` & `joo-0.1.0.138/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.137
+Version: 0.1.0.138
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.137/lib/joo/LICENSE` & `joo-0.1.0.138/lib/joo/LICENSE`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.137/lib/joo/__init__.py` & `joo-0.1.0.138/lib/joo/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,25 @@
     This file is part of joo library.
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 import time
 from abc import ABC, abstractmethod
 
-#-------------------------------------------------------------------------------
 class ManagedObject:
     def __init__(self):
         self._state = None
 
     def __del__(self):
         if self._state != None:
             raise Exception("Object must be released explicitly.")
         
     @property
     def state(self): return self._state
 
-#-------------------------------------------------------------------------------
 class ManagedObjects(ABC):
     def __init__(self):
         self._objects = []
 
     def register_object(self, obj):
         if obj not in self._objects: self._objects.append(obj)
 
@@ -32,15 +30,14 @@
     def gc(self):
         # assume object supports the delete(gc) method
         # gc=True means it's in gc() process, so should not make
         # any call of register_object() or unregister_object().
         for obj in self._objects: obj.delete(gc=True)
         self._objects.clear()
 
-#-------------------------------------------------------------------------------
 class DebugTimer:
     def __init__(self):
         self._checkpoints = []
         self.reset()
 
     def reset(self):
         self._checkpoints.clear()
@@ -95,8 +92,37 @@
                 t += " ({:.2f}%)".format(step_duration / total_duration * 100.0)
             index += 1
         
         # total
         if show_total_duration:
             t += "\r\nTotal: {:.4f} seconds".format(total_duration)
         #
-        return t
+        return t
+    
+class DebugBlock:
+    def __init__(self, name, logger=None, mode="b/e"):
+        self.name = name
+        self.logger = logger
+        if mode in ["b/e", "begin/end"]:
+            self.verbs = ("Begin", "End")
+        elif mode in ["s/e", "start/end"]:
+            self.verbs = ("Start", "End")
+        elif mode in ["o/c", "open/close"]:
+            self.verbs = ("Open", "Close")
+        elif mode in ["e/l", "enter/leave"]:
+            self.verbs = ("Enter", "Leave")
+        else:
+            self.verbs = ("", "")
+
+    def __enter__(self):
+        text = ">>>>>>>> {} >>>>>>>>".format((self.verbs[0] + " " + self.name).strip())
+        if self.logger:
+            self.logger.debug(text)
+        else:
+            print(text)
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        text = "<<<<<<<< {} <<<<<<<<".format((self.verbs[1] + " " + self.name).strip())
+        if self.logger:
+            self.logger.debug(text)
+        else:
+            print(text)
```

### Comparing `joo-0.1.0.137/lib/joo/__version__.py` & `joo-0.1.0.138/lib/joo/__version__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     :copyright: Copyright 1993-2024 Wooloo Studio.  All rights reserved.
     :license: MIT, check LICENSE for details.
 """
 __VERSION__ = {
     "name": "joo",
     "description": "joo library",
     "version": "0.1.0",
-    "build": 137,
+    "build": 138,
     "license": "MIT License",
     "author": "Wooloo Studio",
     "author_email": "max.wu@wooloostudio.com",
     "url": "https://github.com/metatutu/joo",
     "project_urls": {
         "Documentation": "https://github.com/metatutu/joo",
         "Source Code": "https://github.com/metatutu/joo",
```

### Comparing `joo-0.1.0.137/lib/joo/cli.py` & `joo-0.1.0.138/lib/joo/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,37 +39,31 @@
         this with below code:
 
             def _globals(self): return globals()
         """
         return None
 
     def run_workflow(self, workflow_name):
-        def find_workflow_handler(workflow_name):
-            try:
-                #handler name
-                handler_name = "workflow_" + workflow_name
-
-                #find handler in members
-                if hasattr(self, handler_name):
-                    f = getattr(self, handler_name)
-                    if callable(f): return f
-
-                #find handler in globals
-                x_globals = self._globals()
-                if x_globals:
-                    f = x_globals.get(handler_name)
-                    if callable(f): return f
-            except Exception as ex:
-                self.exception(ex)
-            return None
-
         try:
-            f = find_workflow_handler(workflow_name)
-            if f is None: return 1
-            return f()
+            #handler name
+            handler_name = "workflow_" + workflow_name
+
+            #find handler in members
+            if hasattr(self, handler_name):
+                f = getattr(self, handler_name)
+                if callable(f): return f()
+
+            #find handler in globals
+            x_globals = self._globals()
+            if x_globals:
+                f = x_globals.get(handler_name)
+                if callable(f): return f(self)
+
+            #
+            return 1
         except Exception as ex:
             self.exception(ex)
             return 1
 
     def workflow_default(self):
         return self.simple_main_proc(self) if self.simple_main_proc else 0
```

### Comparing `joo-0.1.0.137/lib/joo/logging.py` & `joo-0.1.0.138/lib/joo/logging.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.137/lib/joo/scraping/__init__.py` & `joo-0.1.0.138/lib/joo/scraping/__init__.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.137/lib/joo/scraping/http.py` & `joo-0.1.0.138/lib/joo/scraping/http.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.137/lib/joo/scraping/selenium.py` & `joo-0.1.0.138/lib/joo/scraping/selenium.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.137/lib/joo/sysutil.py` & `joo-0.1.0.138/lib/joo/sysutil.py`

 * *Files identical despite different names*

### Comparing `joo-0.1.0.137/lib/joo.egg-info/PKG-INFO` & `joo-0.1.0.138/lib/joo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joo
-Version: 0.1.0.137
+Version: 0.1.0.138
 Summary: joo library
 Home-page: https://github.com/metatutu/joo
 Author: Wooloo Studio
 Author-email: max.wu@wooloostudio.com
 License: MIT License
 Project-URL: Documentation, https://github.com/metatutu/joo
 Project-URL: Source Code, https://github.com/metatutu/joo
```

### Comparing `joo-0.1.0.137/setup.py` & `joo-0.1.0.138/setup.py`

 * *Files identical despite different names*

