# Comparing `tmp/optioner-1.4.2.tar.gz` & `tmp/optioner-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optioner-1.4.2.tar", last modified: Thu Mar 28 19:46:01 2024, max compression
+gzip compressed data, was "optioner-1.4.3.tar", last modified: Wed Apr  3 15:55:25 2024, max compression
```

## Comparing `optioner-1.4.2.tar` & `optioner-1.4.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-03-28 19:46:01.622377 optioner-1.4.2/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-03-27 09:25:27.000000 optioner-1.4.2/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     6081 2024-03-28 19:46:01.621905 optioner-1.4.2/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3845 2024-03-28 19:41:35.000000 optioner-1.4.2/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-03-28 19:43:52.000000 optioner-1.4.2/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-03-28 19:46:01.622446 optioner-1.4.2/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-03-28 19:46:01.617898 optioner-1.4.2/src/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-03-27 09:25:27.000000 optioner-1.4.2/src/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-03-28 19:46:01.621418 optioner-1.4.2/src/optioner.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     6081 2024-03-28 19:46:01.000000 optioner-1.4.2/src/optioner.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-03-28 19:46:01.000000 optioner-1.4.2/src/optioner.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-03-28 19:46:01.000000 optioner-1.4.2/src/optioner.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-03-28 19:46:01.000000 optioner-1.4.2/src/optioner.egg-info/top_level.txt
--rw-r--r--   0 d33pster   (501) staff       (20)     5951 2024-03-28 19:19:23.000000 optioner-1.4.2/src/optioner.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:55:25.884060 optioner-1.4.3/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 15:46:41.000000 optioner-1.4.3/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     6081 2024-04-03 15:55:25.883609 optioner-1.4.3/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     3845 2024-04-03 15:46:41.000000 optioner-1.4.3/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-03 15:46:54.000000 optioner-1.4.3/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 15:55:25.884120 optioner-1.4.3/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:55:25.873376 optioner-1.4.3/src/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:46:41.000000 optioner-1.4.3/src/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:55:25.883181 optioner-1.4.3/src/optioner.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     6081 2024-04-03 15:55:25.000000 optioner-1.4.3/src/optioner.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-04-03 15:55:25.000000 optioner-1.4.3/src/optioner.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 15:55:25.000000 optioner-1.4.3/src/optioner.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-03 15:55:25.000000 optioner-1.4.3/src/optioner.egg-info/top_level.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)     6376 2024-04-03 15:55:00.000000 optioner-1.4.3/src/optioner.py
```

### Comparing `optioner-1.4.2/LICENSE` & `optioner-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `optioner-1.4.2/PKG-INFO` & `optioner-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.2
+Version: 1.4.3
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.2 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.3 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `optioner-1.4.2/README.md` & `optioner-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `optioner-1.4.2/pyproject.toml` & `optioner-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optioner"
-version = "1.4.2"
+version = "1.4.3"
 description = "Argument Parser"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
```

### Comparing `optioner-1.4.2/src/optioner.egg-info/PKG-INFO` & `optioner-1.4.3/src/optioner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.2
+Version: 1.4.3
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.2 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.3 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `optioner-1.4.2/src/optioner.py` & `optioner-1.4.3/src/optioner.py`

 * *Files 4% similar despite different names*

```diff
@@ -77,33 +77,40 @@
                 if (self._compulsory_short[i] not in self._gotargs) and (self._compulsory_long[i] not in self._gotargs):
                     self._argerror = f'\'{self._compulsory_short[i]}\' argument is Compulsory'
                     self._argcheck = False
                     break
         
         # if this then not that
         ## ifthisthennotthat = [[if this], [this cannot be there]]
-        ifthis = self._ifthisnotthat[0]
-        thennotthat = self._ifthisnotthat[1]
         
-        for x in ifthis:
-            if len(x)>2:
-                x = '--' + x
-            else:
-                x = '-' + x
-            
-            if x in self._gotargs:
-                for y in thennotthat:
-                    if len(y)>2:
-                        y = '--' + y
+        # if ifthisthennotthat has pairs
+        if len(self._ifthisnotthat)%2==0:
+            for i in range(0,len(self._ifthisnotthat), 2):
+                ifthis = self._ifthisnotthat[i]
+                thennotthat = self._ifthisnotthat[i+1]
+                
+                for x in ifthis:
+                    if len(x)>2:
+                        x = '--' + x
                     else:
-                        y = '-' + y
+                        x = '-' + x
                     
-                    if y in self._gotargs:
-                        self._argcheck = False
-                        self._argerror = f'\'{x}\' and \'{y}\' cannot be used together.'
+                    if x in self._gotargs:
+                        for y in thennotthat:
+                            if len(y)>2:
+                                y = '--' + y
+                            else:
+                                y = '-' + y
+                            
+                            if y in self._gotargs:
+                                self._argcheck = False
+                                self._argerror = f'\'{x}\' and \'{y}\' cannot be used together.'
+        else:
+            self._argcheck = False
+            self._argerror = 'ifthisthennotthat param value mismatch.'
         
         # if ignore args are present then ignore the errors
         for x in self._ignore:
             if x in self._gotargs:
                 self._argerror = 'no error'
                 self._argcheck = True
```

