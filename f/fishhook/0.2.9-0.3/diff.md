# Comparing `tmp/fishhook-0.2.9.tar.gz` & `tmp/fishhook-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fishhook-0.2.9.tar", last modified: Thu Aug 10 03:51:40 2023, max compression
+gzip compressed data, was "fishhook-0.3.tar", last modified: Wed Apr  3 01:53:49 2024, max compression
```

## Comparing `fishhook-0.2.9.tar` & `fishhook-0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2023-08-10 03:51:40.691188 fishhook-0.2.9/
--rw-r--r--   0 chilaxan   (501) staff       (20)     1065 2023-02-05 02:31:28.000000 fishhook-0.2.9/LICENSE
--rw-r--r--   0 chilaxan   (501) staff       (20)     1653 2023-08-10 03:51:40.691095 fishhook-0.2.9/PKG-INFO
--rw-r--r--   0 chilaxan   (501) staff       (20)     1209 2022-12-01 04:16:15.000000 fishhook-0.2.9/README.md
-drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2023-08-10 03:51:40.690491 fishhook-0.2.9/fishhook/
--rw-r--r--   0 chilaxan   (501) staff       (20)      601 2023-02-04 22:40:02.000000 fishhook-0.2.9/fishhook/__init__.py
--rw-r--r--   0 chilaxan   (501) staff       (20)     1702 2022-12-01 23:24:21.000000 fishhook-0.2.9/fishhook/asm.py
--rw-r--r--   0 chilaxan   (501) staff       (20)    16540 2023-08-10 03:41:07.000000 fishhook-0.2.9/fishhook/fishhook.py
--rw-r--r--   0 chilaxan   (501) staff       (20)     3609 2023-08-10 03:42:20.000000 fishhook-0.2.9/fishhook/tests.py
-drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2023-08-10 03:51:40.690937 fishhook-0.2.9/fishhook.egg-info/
--rwxrwxrwx   0 chilaxan   (501) staff       (20)     1653 2023-08-10 03:51:40.000000 fishhook-0.2.9/fishhook.egg-info/PKG-INFO
--rwxrwxrwx   0 chilaxan   (501) staff       (20)      230 2023-08-10 03:51:40.000000 fishhook-0.2.9/fishhook.egg-info/SOURCES.txt
--rwxrwxrwx   0 chilaxan   (501) staff       (20)        1 2023-08-10 03:51:40.000000 fishhook-0.2.9/fishhook.egg-info/dependency_links.txt
--rwxrwxrwx   0 chilaxan   (501) staff       (20)        9 2023-08-10 03:51:40.000000 fishhook-0.2.9/fishhook.egg-info/top_level.txt
--rw-r--r--   0 chilaxan   (501) staff       (20)       38 2023-08-10 03:51:40.691223 fishhook-0.2.9/setup.cfg
--rw-r--r--   0 chilaxan   (501) staff       (20)      660 2023-08-10 03:08:10.000000 fishhook-0.2.9/setup.py
+drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 01:53:49.003678 fishhook-0.3/
+-rw-r--r--   0 chilaxan   (501) staff       (20)     1065 2023-02-05 02:31:28.000000 fishhook-0.3/LICENSE
+-rw-r--r--   0 chilaxan   (501) staff       (20)     2378 2024-04-03 01:53:49.003399 fishhook-0.3/PKG-INFO
+-rw-r--r--   0 chilaxan   (501) staff       (20)     1881 2024-04-03 01:45:54.000000 fishhook-0.3/README.md
+drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 01:53:49.002057 fishhook-0.3/fishhook/
+-rw-r--r--   0 chilaxan   (501) staff       (20)      601 2023-08-24 22:03:59.000000 fishhook-0.3/fishhook/__init__.py
+-rw-r--r--   0 chilaxan   (501) staff       (20)     3639 2024-04-03 00:58:11.000000 fishhook-0.3/fishhook/_asmmodule.c
+-rw-r--r--   0 chilaxan   (501) staff       (20)     3592 2024-04-03 01:02:38.000000 fishhook-0.3/fishhook/asm.py
+-rw-r--r--   0 chilaxan   (501) staff       (20)    16540 2023-08-10 03:41:07.000000 fishhook-0.3/fishhook/fishhook.py
+-rw-r--r--   0 chilaxan   (501) staff       (20)     3609 2023-08-10 03:42:20.000000 fishhook-0.3/fishhook/tests.py
+drwxr-xr-x   0 chilaxan   (501) staff       (20)        0 2024-04-03 01:53:49.003114 fishhook-0.3/fishhook.egg-info/
+-rw-r--r--   0 chilaxan   (501) staff       (20)     2378 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/PKG-INFO
+-rw-r--r--   0 chilaxan   (501) staff       (20)      283 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/SOURCES.txt
+-rw-r--r--   0 chilaxan   (501) staff       (20)        1 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/dependency_links.txt
+-rw-r--r--   0 chilaxan   (501) staff       (20)       25 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/requires.txt
+-rw-r--r--   0 chilaxan   (501) staff       (20)        9 2024-04-03 01:53:48.000000 fishhook-0.3/fishhook.egg-info/top_level.txt
+-rw-r--r--   0 chilaxan   (501) staff       (20)       38 2024-04-03 01:53:49.003743 fishhook-0.3/setup.cfg
+-rw-r--r--   0 chilaxan   (501) staff       (20)      789 2024-04-03 01:39:01.000000 fishhook-0.3/setup.py
```

### Comparing `fishhook-0.2.9/LICENSE` & `fishhook-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fishhook-0.2.9/PKG-INFO` & `fishhook-0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: fishhook
-Version: 0.2.9
+Version: 0.3
 Summary: Allows for runtime hooking of static class functions
 Home-page: https://github.com/chilaxan/fishhook
 Author: chilaxan
 Author-email: chilaxan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: capstone
+Requires-Dist: keystone-engine
 
 # Fishhook
 
 This module allows for swapping out the slot pointers contained in static
 classes with the **generic** slot pointers used by python for heap classes.
 This allows for assigning arbitrary python functions to static class dunders
 using *hook* and *hook_cls* and for applying new functionality to previously
@@ -47,12 +49,33 @@
 ### hooking descriptors
 ```py
 @hook.property(int)
 def imag(self):
   ...
   return orig.imag
 ```
+
+# fishhook.asm
+
+This submodule allows for more in-depth C level hooks.
+For obvious reasons, this is vastly unstable, mostly provided as an experiment.
+Originally created as a way to grab a reference to the Interned strings dictionary.
+
+```py
+from fishhook import asm
+from ctypes import py_object, pythonapi
+
+@asm.hook(pythonapi.PyDict_SetDefault, restype=py_object, argtypes=[py_object, py_object, py_object])
+def setdefault(self, key, value):
+    if key == 'MAGICVAL':
+        return self
+    return pythonapi.PyDict_SetDefault(self, key, value)
+
+pythonapi.PyUnicode_InternFromString.restype = py_object
+interned = pythonapi.PyUnicode_InternFromString(b'MAGICVAL')
+```
+
 #### Links
 
 [Github](https://github.com/chilaxan/fishhook)
 
 [PyPi](https://pypi.org/project/fishhook/)
```

### Comparing `fishhook-0.2.9/README.md` & `fishhook-0.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -33,12 +33,33 @@
 ### hooking descriptors
 ```py
 @hook.property(int)
 def imag(self):
   ...
   return orig.imag
 ```
+
+# fishhook.asm
+
+This submodule allows for more in-depth C level hooks.
+For obvious reasons, this is vastly unstable, mostly provided as an experiment.
+Originally created as a way to grab a reference to the Interned strings dictionary.
+
+```py
+from fishhook import asm
+from ctypes import py_object, pythonapi
+
+@asm.hook(pythonapi.PyDict_SetDefault, restype=py_object, argtypes=[py_object, py_object, py_object])
+def setdefault(self, key, value):
+    if key == 'MAGICVAL':
+        return self
+    return pythonapi.PyDict_SetDefault(self, key, value)
+
+pythonapi.PyUnicode_InternFromString.restype = py_object
+interned = pythonapi.PyUnicode_InternFromString(b'MAGICVAL')
+```
+
 #### Links
 
 [Github](https://github.com/chilaxan/fishhook)
 
 [PyPi](https://pypi.org/project/fishhook/)
```

### Comparing `fishhook-0.2.9/fishhook/__init__.py` & `fishhook-0.3/fishhook/__init__.py`

 * *Files identical despite different names*

### Comparing `fishhook-0.2.9/fishhook/fishhook.py` & `fishhook-0.3/fishhook/fishhook.py`

 * *Files identical despite different names*

### Comparing `fishhook-0.2.9/fishhook/tests.py` & `fishhook-0.3/fishhook/tests.py`

 * *Files identical despite different names*

### Comparing `fishhook-0.2.9/fishhook.egg-info/PKG-INFO` & `fishhook-0.3/fishhook.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: fishhook
-Version: 0.2.9
+Version: 0.3
 Summary: Allows for runtime hooking of static class functions
 Home-page: https://github.com/chilaxan/fishhook
 Author: chilaxan
 Author-email: chilaxan@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: capstone
+Requires-Dist: keystone-engine
 
 # Fishhook
 
 This module allows for swapping out the slot pointers contained in static
 classes with the **generic** slot pointers used by python for heap classes.
 This allows for assigning arbitrary python functions to static class dunders
 using *hook* and *hook_cls* and for applying new functionality to previously
@@ -47,12 +49,33 @@
 ### hooking descriptors
 ```py
 @hook.property(int)
 def imag(self):
   ...
   return orig.imag
 ```
+
+# fishhook.asm
+
+This submodule allows for more in-depth C level hooks.
+For obvious reasons, this is vastly unstable, mostly provided as an experiment.
+Originally created as a way to grab a reference to the Interned strings dictionary.
+
+```py
+from fishhook import asm
+from ctypes import py_object, pythonapi
+
+@asm.hook(pythonapi.PyDict_SetDefault, restype=py_object, argtypes=[py_object, py_object, py_object])
+def setdefault(self, key, value):
+    if key == 'MAGICVAL':
+        return self
+    return pythonapi.PyDict_SetDefault(self, key, value)
+
+pythonapi.PyUnicode_InternFromString.restype = py_object
+interned = pythonapi.PyUnicode_InternFromString(b'MAGICVAL')
+```
+
 #### Links
 
 [Github](https://github.com/chilaxan/fishhook)
 
 [PyPi](https://pypi.org/project/fishhook/)
```

