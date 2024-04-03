# Comparing `tmp/getpublicipv4-0.10.tar.gz` & `tmp/getpublicipv4-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "getpublicipv4-0.10.tar", last modified: Mon Sep  4 18:31:46 2023, max compression
+gzip compressed data, was "getpublicipv4-0.12.tar", last modified: Wed Apr  3 01:59:38 2024, max compression
```

## Comparing `getpublicipv4-0.10.tar` & `getpublicipv4-0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-09-04 18:31:46.669453 getpublicipv4-0.10/
--rw-rw-rw-   0        0        0     1148 2023-09-04 18:31:39.000000 getpublicipv4-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      110 2023-09-04 18:31:38.000000 getpublicipv4-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0      877 2023-09-04 18:31:46.669453 getpublicipv4-0.10/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-09-04 18:30:07.000000 getpublicipv4-0.10/README.md
-drwxrwxrwx   0        0        0        0 2023-09-04 18:31:46.665720 getpublicipv4-0.10/getpublicipv4/
--rw-rw-rw-   0        0        0      258 2023-09-04 18:30:07.000000 getpublicipv4-0.10/getpublicipv4/README.MD
--rw-rw-rw-   0        0        0     1085 2023-09-04 18:25:47.000000 getpublicipv4-0.10/getpublicipv4/__init__.py
--rw-rw-rw-   0        0        0        8 2023-09-04 18:31:45.000000 getpublicipv4-0.10/getpublicipv4/requirements.txt
--rw-rw-rw-   0        0        0    10447 2023-09-04 18:31:45.000000 getpublicipv4-0.10/getpublicipv4/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-09-04 18:31:46.668707 getpublicipv4-0.10/getpublicipv4.egg-info/
--rw-rw-rw-   0        0        0      877 2023-09-04 18:31:46.000000 getpublicipv4-0.10/getpublicipv4.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-09-04 18:31:46.000000 getpublicipv4-0.10/getpublicipv4.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-09-04 18:31:46.000000 getpublicipv4-0.10/getpublicipv4.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-09-04 18:31:46.000000 getpublicipv4-0.10/getpublicipv4.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-09-04 18:31:46.000000 getpublicipv4-0.10/getpublicipv4.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-09-04 18:31:46.670200 getpublicipv4-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1278 2023-09-04 18:31:45.000000 getpublicipv4-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 01:59:38.009717 getpublicipv4-0.12/
+-rw-rw-rw-   0        0        0     1148 2024-04-03 01:59:29.000000 getpublicipv4-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      110 2024-04-03 01:59:29.000000 getpublicipv4-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     1577 2024-04-03 01:59:38.009717 getpublicipv4-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2024-04-03 01:58:44.000000 getpublicipv4-0.12/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 01:59:38.002216 getpublicipv4-0.12/getpublicipv4/
+-rw-rw-rw-   0        0        0      933 2024-04-03 01:58:44.000000 getpublicipv4-0.12/getpublicipv4/README.MD
+-rw-rw-rw-   0        0        0     2631 2024-04-03 01:47:39.000000 getpublicipv4-0.12/getpublicipv4/__init__.py
+-rw-rw-rw-   0        0        0        8 2024-04-03 01:59:36.000000 getpublicipv4-0.12/getpublicipv4/requirements.txt
+-rw-rw-rw-   0        0        0    10447 2024-04-03 01:59:36.000000 getpublicipv4-0.12/getpublicipv4/thirdparty.json
+drwxrwxrwx   0        0        0        0 2024-04-03 01:59:38.008218 getpublicipv4-0.12/getpublicipv4.egg-info/
+-rw-rw-rw-   0        0        0     1577 2024-04-03 01:59:37.000000 getpublicipv4-0.12/getpublicipv4.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-03 01:59:37.000000 getpublicipv4-0.12/getpublicipv4.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 01:59:37.000000 getpublicipv4-0.12/getpublicipv4.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-03 01:59:37.000000 getpublicipv4-0.12/getpublicipv4.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-03 01:59:37.000000 getpublicipv4-0.12/getpublicipv4.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-03 01:59:38.011216 getpublicipv4-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1278 2024-04-03 01:59:36.000000 getpublicipv4-0.12/setup.py
```

### Comparing `getpublicipv4-0.10/LICENSE.rst` & `getpublicipv4-0.12/LICENSE.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
  The MIT License (MIT)
- Copyright (c) 2023 Johannes Fischer
+ Copyright (c) 2024 Johannes Fischer
  
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `getpublicipv4-0.10/getpublicipv4/thirdparty.json` & `getpublicipv4-0.12/getpublicipv4/thirdparty.json`

 * *Files identical despite different names*

### Comparing `getpublicipv4-0.10/setup.py` & `getpublicipv4-0.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.12'''
 DESCRIPTION = '''script to get the public IP (v4) of a PC'''
 
 # Setting up
 setup(
     name="getpublicipv4",
     version=VERSION,
     license='MIT',
```

