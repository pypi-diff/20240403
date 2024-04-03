# Comparing `tmp/optioner-1.4.3.tar.gz` & `tmp/optioner-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optioner-1.4.3.tar", last modified: Wed Apr  3 15:55:25 2024, max compression
+gzip compressed data, was "optioner-1.4.4.tar", last modified: Wed Apr  3 15:58:22 2024, max compression
```

## Comparing `optioner-1.4.3.tar` & `optioner-1.4.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:55:25.884060 optioner-1.4.3/
--rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 15:46:41.000000 optioner-1.4.3/LICENSE
--rw-r--r--   0 d33pster   (501) staff       (20)     6081 2024-04-03 15:55:25.883609 optioner-1.4.3/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)     3845 2024-04-03 15:46:41.000000 optioner-1.4.3/README.md
--rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-03 15:46:54.000000 optioner-1.4.3/pyproject.toml
--rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 15:55:25.884120 optioner-1.4.3/setup.cfg
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:55:25.873376 optioner-1.4.3/src/
--rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:46:41.000000 optioner-1.4.3/src/__init__.py
-drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:55:25.883181 optioner-1.4.3/src/optioner.egg-info/
--rw-r--r--   0 d33pster   (501) staff       (20)     6081 2024-04-03 15:55:25.000000 optioner-1.4.3/src/optioner.egg-info/PKG-INFO
--rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-04-03 15:55:25.000000 optioner-1.4.3/src/optioner.egg-info/SOURCES.txt
--rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 15:55:25.000000 optioner-1.4.3/src/optioner.egg-info/dependency_links.txt
--rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-03 15:55:25.000000 optioner-1.4.3/src/optioner.egg-info/top_level.txt
--rw-r--r--   0 d33pster   (501) staff       (20)     6376 2024-04-03 15:55:00.000000 optioner-1.4.3/src/optioner.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:58:22.728927 optioner-1.4.4/
+-rw-r--r--   0 d33pster   (501) staff       (20)     1074 2024-04-03 15:46:41.000000 optioner-1.4.4/LICENSE
+-rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-03 15:58:22.728479 optioner-1.4.4/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)     3910 2024-04-03 15:58:08.000000 optioner-1.4.4/README.md
+-rw-r--r--   0 d33pster   (501) staff       (20)     1131 2024-04-03 15:57:06.000000 optioner-1.4.4/pyproject.toml
+-rw-r--r--   0 d33pster   (501) staff       (20)       38 2024-04-03 15:58:22.728994 optioner-1.4.4/setup.cfg
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:58:22.723728 optioner-1.4.4/src/
+-rw-r--r--   0 d33pster   (501) staff       (20)        0 2024-04-03 15:46:41.000000 optioner-1.4.4/src/__init__.py
+drwxr-xr-x   0 d33pster   (501) staff       (20)        0 2024-04-03 15:58:22.728052 optioner-1.4.4/src/optioner.egg-info/
+-rw-r--r--   0 d33pster   (501) staff       (20)     6146 2024-04-03 15:58:22.000000 optioner-1.4.4/src/optioner.egg-info/PKG-INFO
+-rw-r--r--   0 d33pster   (501) staff       (20)      208 2024-04-03 15:58:22.000000 optioner-1.4.4/src/optioner.egg-info/SOURCES.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)        1 2024-04-03 15:58:22.000000 optioner-1.4.4/src/optioner.egg-info/dependency_links.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)       18 2024-04-03 15:58:22.000000 optioner-1.4.4/src/optioner.egg-info/top_level.txt
+-rw-r--r--   0 d33pster   (501) staff       (20)     6376 2024-04-03 15:55:00.000000 optioner-1.4.4/src/optioner.py
```

### Comparing `optioner-1.4.3/LICENSE` & `optioner-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `optioner-1.4.3/PKG-INFO` & `optioner-1.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.3
+Version: 1.4.4
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
-v1.4.2
+v1.4.4
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
 
@@ -66,14 +66,17 @@
 ```console
 $ pip install optioner
 ```
 
 ## Usage
 
 ###### initialization
+
+[ [Full Documentation](https://d33pster.github.io/optioner/) ]
+
 ```console
 >>> from optioner import options
 >>> help(options)
 
 Help on class options in module optioner:
 
 class options(builtins.object)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.3 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.4 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -32,24 +32,25 @@
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.2
+v1.4.4
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
-```console $ pip install optioner ``` ## Usage ###### initialization ```console
->>> from optioner import options >>> help(options) Help on class options in
-module optioner: class options(builtins.object) | options(shortargs: list,
-longargs: list, gotargs: list) | | Methods defined here: | | __init__(self,
-shortargs: list, longargs: list, gotargs: list, compulsory_short_args:list =[],
+```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
+Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
+optioner import options >>> help(options) Help on class options in module
+optioner: class options(builtins.object) | options(shortargs: list, longargs:
+list, gotargs: list) | | Methods defined here: | | __init__(self, shortargs:
+list, longargs: list, gotargs: list, compulsory_short_args:list =[],
 compulsory_long_args:list =[], ignore: list[str] [], ifthisthennotthat:list
 [list[str]] = [[],[]]) | init function: This runs everytime the class is
 called. | | Args: | shortargs (list): example: ['h', 'l', 'i', ...] | longargs
 (list): example: ['help', 'lock', 'init', ...] | gotargs (list): sys.argv[1:] |
 compulsory_short_args (list | optional): optional compulsory arguments |
 compulsory_long_args (list | optional): corresponding optional compulsory
 arguments | ignore (list[str] | optional): if these args are found, compulsion
```

### Comparing `optioner-1.4.3/README.md` & `optioner-1.4.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ![Static Badge](https://img.shields.io/badge/pypi-available-brightgreen?style=flat&logo=python&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Linux-supported-blue?style=flat&logo=Linux&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/Windows-supported-blue?style=flat&logo=Windows&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/MacOS-supported-blue?style=flat&logo=Macintosh&logoColor=red)
 ![Static Badge](https://img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 <br><br><br>
-v1.4.2
+v1.4.4
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
 
@@ -21,14 +21,17 @@
 ```console
 $ pip install optioner
 ```
 
 ## Usage
 
 ###### initialization
+
+[ [Full Documentation](https://d33pster.github.io/optioner/) ]
+
 ```console
 >>> from optioner import options
 >>> help(options)
 
 Help on class options in module optioner:
 
 class options(builtins.object)
```

#### html2text {}

```diff
@@ -4,24 +4,25 @@
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.2
+v1.4.4
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
-```console $ pip install optioner ``` ## Usage ###### initialization ```console
->>> from optioner import options >>> help(options) Help on class options in
-module optioner: class options(builtins.object) | options(shortargs: list,
-longargs: list, gotargs: list) | | Methods defined here: | | __init__(self,
-shortargs: list, longargs: list, gotargs: list, compulsory_short_args:list =[],
+```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
+Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
+optioner import options >>> help(options) Help on class options in module
+optioner: class options(builtins.object) | options(shortargs: list, longargs:
+list, gotargs: list) | | Methods defined here: | | __init__(self, shortargs:
+list, longargs: list, gotargs: list, compulsory_short_args:list =[],
 compulsory_long_args:list =[], ignore: list[str] [], ifthisthennotthat:list
 [list[str]] = [[],[]]) | init function: This runs everytime the class is
 called. | | Args: | shortargs (list): example: ['h', 'l', 'i', ...] | longargs
 (list): example: ['help', 'lock', 'init', ...] | gotargs (list): sys.argv[1:] |
 compulsory_short_args (list | optional): optional compulsory arguments |
 compulsory_long_args (list | optional): corresponding optional compulsory
 arguments | ignore (list[str] | optional): if these args are found, compulsion
```

### Comparing `optioner-1.4.3/pyproject.toml` & `optioner-1.4.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "optioner"
-version = "1.4.3"
+version = "1.4.4"
 description = "Argument Parser"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3.9",
```

### Comparing `optioner-1.4.3/src/optioner.egg-info/PKG-INFO` & `optioner-1.4.4/src/optioner.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optioner
-Version: 1.4.3
+Version: 1.4.4
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
-v1.4.2
+v1.4.4
 
 <p align='center'>
     <a href='#Installation'>Installation</a>
     &nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
     <a href='#Usage'>Usage</a>
 </p><br>
 
@@ -66,14 +66,17 @@
 ```console
 $ pip install optioner
 ```
 
 ## Usage
 
 ###### initialization
+
+[ [Full Documentation](https://d33pster.github.io/optioner/) ]
+
 ```console
 >>> from optioner import options
 >>> help(options)
 
 Help on class options in module optioner:
 
 class options(builtins.object)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: optioner Version: 1.4.3 Summary: Argument Parser
+Metadata-Version: 2.1 Name: optioner Version: 1.4.4 Summary: Argument Parser
 Author-email: Soumyo Deep Gupta
 gmail.com> Maintainer-email: Soumyo Deep Gupta
 gmail.com> License: MIT License Copyright (c) 2024 Soumyo Deep Gupta Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
@@ -32,24 +32,25 @@
 ![Static Badge](https://img.shields.io/badge/Windows-supported-
 blue?style=flat&logo=Windows&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/MacOS-supported-
 blue?style=flat&logo=Macintosh&logoColor=red) ![Static Badge](https://
 img.shields.io/badge/python-only-green?style=flat&logo=python&logoColor=red)
 
 
-v1.4.2
+v1.4.4
                           _I_n_s_t_a_l_l_a_t_i_o_n    |    _U_s_a_g_e
 
 ## About Optioner is a lightweight Argument Parser and easy to use. Full
 documentation [here](https://d33pster.github.io/optioner/) ## Installation
-```console $ pip install optioner ``` ## Usage ###### initialization ```console
->>> from optioner import options >>> help(options) Help on class options in
-module optioner: class options(builtins.object) | options(shortargs: list,
-longargs: list, gotargs: list) | | Methods defined here: | | __init__(self,
-shortargs: list, longargs: list, gotargs: list, compulsory_short_args:list =[],
+```console $ pip install optioner ``` ## Usage ###### initialization [ [Full
+Documentation](https://d33pster.github.io/optioner/) ] ```console >>> from
+optioner import options >>> help(options) Help on class options in module
+optioner: class options(builtins.object) | options(shortargs: list, longargs:
+list, gotargs: list) | | Methods defined here: | | __init__(self, shortargs:
+list, longargs: list, gotargs: list, compulsory_short_args:list =[],
 compulsory_long_args:list =[], ignore: list[str] [], ifthisthennotthat:list
 [list[str]] = [[],[]]) | init function: This runs everytime the class is
 called. | | Args: | shortargs (list): example: ['h', 'l', 'i', ...] | longargs
 (list): example: ['help', 'lock', 'init', ...] | gotargs (list): sys.argv[1:] |
 compulsory_short_args (list | optional): optional compulsory arguments |
 compulsory_long_args (list | optional): corresponding optional compulsory
 arguments | ignore (list[str] | optional): if these args are found, compulsion
```

### Comparing `optioner-1.4.3/src/optioner.py` & `optioner-1.4.4/src/optioner.py`

 * *Files identical despite different names*

