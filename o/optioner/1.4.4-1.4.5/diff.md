# Comparing `tmp/optioner-1.4.4.tar.gz` & `tmp/optioner-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optioner-1.4.4.tar", last modified: Wed Apr  3 15:58:22 2024, max compression
+gzip compressed data, was "optioner-1.4.5.tar", last modified: Wed Apr  3 21:25:51 2024, max compression
```

## Comparing `optioner-1.4.4.tar` & `optioner-1.4.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:58:22.728927 optioner-1.4.4/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 15:46:41.000000 optioner-1.4.4/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-03 15:58:22.728479 optioner-1.4.4/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3910 2024-04-03 15:58:08.000000 optioner-1.4.4/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-03 15:57:06.000000 optioner-1.4.4/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 15:58:22.728994 optioner-1.4.4/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:58:22.723728 optioner-1.4.4/src/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:46:41.000000 optioner-1.4.4/src/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:58:22.728052 optioner-1.4.4/src/optioner.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-03 15:58:22.000000 optioner-1.4.4/src/optioner.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-04-03 15:58:22.000000 optioner-1.4.4/src/optioner.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 15:58:22.000000 optioner-1.4.4/src/optioner.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-03 15:58:22.000000 optioner-1.4.4/src/optioner.egg-info/top_level.txt
--rw-r--r--   0 d33pster   (501) staff       (20)     6376 2024-04-03 15:55:00.000000 optioner-1.4.4/src/optioner.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:25:51.342683 optioner-1.4.5/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 21:17:25.000000 optioner-1.4.5/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-03 21:25:51.342313 optioner-1.4.5/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     3910 2024-04-03 21:25:18.000000 optioner-1.4.5/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-03 21:17:34.000000 optioner-1.4.5/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 21:25:51.342752 optioner-1.4.5/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:25:51.335663 optioner-1.4.5/src/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 21:17:25.000000 optioner-1.4.5/src/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 21:25:51.341920 optioner-1.4.5/src/optioner.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-03 21:25:51.000000 optioner-1.4.5/src/optioner.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-04-03 21:25:51.000000 optioner-1.4.5/src/optioner.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 21:25:51.000000 optioner-1.4.5/src/optioner.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-03 21:25:51.000000 optioner-1.4.5/src/optioner.egg-info/top_level.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)     6973 2024-04-03 21:24:07.000000 optioner-1.4.5/src/optioner.py
```

### Comparing `optioner-1.4.4/LICENSE` & `optioner-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `optioner-1.4.4/PKG-INFO` & `optioner-1.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.4
+Version: 1.4.5
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -47,15 +47,15 @@
 
 ![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 <br><br><br>
-v1.4.4
+v1.4.5
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.4 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.5 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -32,15 +32,15 @@
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.4
+v1.4.5
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
 ```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
 Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
 optioner import options >>> help(options) Help on class options in module
```

### Comparing `optioner-1.4.4/README.md` & `optioner-1.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 <br><br><br>
-v1.4.4
+v1.4.5
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.4
+v1.4.5
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
 ```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
 Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
 optioner import options >>> help(options) Help on class options in module
```

### Comparing `optioner-1.4.4/pyproject.toml` & `optioner-1.4.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optioner"
-version = "1.4.4"
+version = "1.4.5"
 description = "Argument Parser"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
```

### Comparing `optioner-1.4.4/src/optioner.egg-info/PKG-INFO` & `optioner-1.4.5/src/optioner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.4
+Version: 1.4.5
 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 Maintainer-email: Soumyo Deep Gupta <deep.main.ac@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Soumyo Deep Gupta
         
@@ -47,15 +47,15 @@
 
 ![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 <br><br><br>
-v1.4.4
+v1.4.5
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.4 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.5 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -32,15 +32,15 @@
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.4
+v1.4.5
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
 ```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
 Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
 optioner import options >>> help(options) Help on class options in module
```

### Comparing `optioner-1.4.4/src/optioner.py` & `optioner-1.4.5/src/optioner.py`

 * *Files 4% similar despite different names*

```diff
@@ -109,14 +109,23 @@
             self._argerror = 'ifthisthennotthat param value mismatch.'
         
         # if ignore args are present then ignore the errors
         for x in self._ignore:
             if x in self._gotargs:
                 self._argerror = 'no error'
                 self._argcheck = True
+                # but if other args are present, raise an error
+                for y in self._shortargs:
+                    if y!=x and y in self._gotargs:
+                        self._argcheck = False
+                        self._argerror = f'when {x} argument is passed, No other argument should be there. Please remove {y}'
+                for y in self._longargs:
+                    if y!=x and y in self._gotargs:
+                        self._argcheck = False
+                        self._argerror = f'when {x} argument is passed, No other argument should be there. Please remove {y}'
         
         return self._gotargs, self._argcheck, self._argerror, self._falseargs
     
     def _what_is_(self, arg: str, count=1):
         """
         Returns the value of the argument that is passed.
```

