# Comparing `tmp/bblame-0.6.4.tar.gz` & `tmp/bblame-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblame-0.6.4.tar", last modified: Tue Sep 20 00:13:43 2022, max compression
+gzip compressed data, was "bblame-0.7.0.tar", last modified: Wed Apr  3 21:12:30 2024, max compression
```

## Comparing `bblame-0.6.4.tar` & `bblame-0.7.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 onikolas (628462427) domain^users (600260513)        0 2022-09-20 00:13:43.239872 bblame-0.6.4/
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)     1084 2022-01-06 00:55:53.000000 bblame-0.6.4/LICENSE.txt
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)       27 2022-01-06 00:55:53.000000 bblame-0.6.4/MANIFEST.in
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)     4869 2022-09-20 00:13:43.239872 bblame-0.6.4/PKG-INFO
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)     4256 2022-01-06 00:55:53.000000 bblame-0.6.4/README.rst
--rwxr-xr-x   0 onikolas (628462427) domain^users (600260513)      109 2022-01-06 00:55:53.000000 bblame-0.6.4/bblame
-drwxr-xr-x   0 onikolas (628462427) domain^users (600260513)        0 2022-09-20 00:13:43.235872 bblame-0.6.4/bblame.egg-info/
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)     4869 2022-09-20 00:13:43.000000 bblame-0.6.4/bblame.egg-info/PKG-INFO
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)      519 2022-09-20 00:13:43.000000 bblame-0.6.4/bblame.egg-info/SOURCES.txt
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)        1 2022-09-20 00:13:43.000000 bblame-0.6.4/bblame.egg-info/dependency_links.txt
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)        1 2022-09-20 00:13:43.000000 bblame-0.6.4/bblame.egg-info/not-zip-safe
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)       35 2022-09-20 00:13:43.000000 bblame-0.6.4/bblame.egg-info/requires.txt
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)       12 2022-09-20 00:13:43.000000 bblame-0.6.4/bblame.egg-info/top_level.txt
-drwxr-xr-x   0 onikolas (628462427) domain^users (600260513)        0 2022-09-20 00:13:43.239872 bblame-0.6.4/betterblame/
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)        0 2022-01-06 00:55:53.000000 bblame-0.6.4/betterblame/__init__.py
--rwxr-xr-x   0 onikolas (628462427) domain^users (600260513)      208 2022-01-06 00:55:53.000000 bblame-0.6.4/betterblame/__main__.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)    16247 2022-01-06 00:55:53.000000 bblame-0.6.4/betterblame/actions.py
--rwxr-xr-x   0 onikolas (628462427) domain^users (600260513)     7868 2022-08-31 21:13:21.000000 bblame-0.6.4/betterblame/bblame.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)    18285 2022-08-31 21:13:21.000000 bblame-0.6.4/betterblame/content.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)    17178 2022-08-31 21:13:21.000000 bblame-0.6.4/betterblame/git.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)    12286 2022-08-31 21:13:21.000000 bblame-0.6.4/betterblame/highlight.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)      460 2022-01-06 00:55:53.000000 bblame-0.6.4/betterblame/modes.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)     3454 2022-01-06 00:55:53.000000 bblame-0.6.4/betterblame/options.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)    32328 2022-09-20 00:00:38.000000 bblame-0.6.4/betterblame/screen.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)     5701 2022-08-31 21:13:21.000000 bblame-0.6.4/betterblame/search.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)     4794 2022-01-06 00:55:53.000000 bblame-0.6.4/betterblame/util.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)      190 2022-09-20 00:08:29.000000 bblame-0.6.4/betterblame/version.py
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)       38 2022-09-20 00:13:43.239872 bblame-0.6.4/setup.cfg
--rw-r--r--   0 onikolas (628462427) domain^users (600260513)     1788 2022-08-31 21:13:21.000000 bblame-0.6.4/setup.py
+drwxr-xr-x   0 onikolas (628462427) domain^users (600260513)        0 2024-04-03 21:12:30.869111 bblame-0.7.0/
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)     1084 2023-07-14 21:21:08.000000 bblame-0.7.0/LICENSE.txt
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)       27 2023-07-14 21:21:08.000000 bblame-0.7.0/MANIFEST.in
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)     4869 2024-04-03 21:12:30.869111 bblame-0.7.0/PKG-INFO
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)     4256 2023-07-14 21:21:08.000000 bblame-0.7.0/README.rst
+-rwxr-xr-x   0 onikolas (628462427) domain^users (600260513)      109 2023-07-14 21:21:08.000000 bblame-0.7.0/bblame
+drwxr-xr-x   0 onikolas (628462427) domain^users (600260513)        0 2024-04-03 21:12:30.865111 bblame-0.7.0/bblame.egg-info/
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)     4869 2024-04-03 21:12:30.000000 bblame-0.7.0/bblame.egg-info/PKG-INFO
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)      537 2024-04-03 21:12:30.000000 bblame-0.7.0/bblame.egg-info/SOURCES.txt
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)        1 2024-04-03 21:12:30.000000 bblame-0.7.0/bblame.egg-info/dependency_links.txt
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)        1 2024-04-03 21:12:30.000000 bblame-0.7.0/bblame.egg-info/not-zip-safe
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)       38 2024-04-03 21:12:30.000000 bblame-0.7.0/bblame.egg-info/requires.txt
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)       12 2024-04-03 21:12:30.000000 bblame-0.7.0/bblame.egg-info/top_level.txt
+drwxr-xr-x   0 onikolas (628462427) domain^users (600260513)        0 2024-04-03 21:12:30.865111 bblame-0.7.0/betterblame/
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)        0 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/__init__.py
+-rwxr-xr-x   0 onikolas (628462427) domain^users (600260513)      208 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/__main__.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)    16247 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/actions.py
+-rwxr-xr-x   0 onikolas (628462427) domain^users (600260513)     7876 2024-04-03 17:49:56.000000 bblame-0.7.0/betterblame/bblame.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)    18285 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/content.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)    17187 2024-04-03 17:49:59.000000 bblame-0.7.0/betterblame/git.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)    12286 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/highlight.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)      460 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/modes.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)     3454 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/options.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)    32328 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/screen.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)     5701 2023-07-14 21:21:08.000000 bblame-0.7.0/betterblame/search.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)      106 2024-04-03 18:34:01.000000 bblame-0.7.0/betterblame/sh.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)     4819 2024-04-03 18:37:03.000000 bblame-0.7.0/betterblame/util.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)      190 2024-04-03 17:37:20.000000 bblame-0.7.0/betterblame/version.py
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)       38 2024-04-03 21:12:30.869111 bblame-0.7.0/setup.cfg
+-rw-r--r--   0 onikolas (628462427) domain^users (600260513)     1791 2024-04-03 17:37:23.000000 bblame-0.7.0/setup.py
```

### Comparing `bblame-0.6.4/LICENSE.txt` & `bblame-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bblame-0.6.4/PKG-INFO` & `bblame-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblame
-Version: 0.6.4
+Version: 0.7.0
 Summary: An ncurses app for browsing file git history
 Home-page: https://bitbucket.org/niko333/betterblame
 Author: Niko Oliveira
 Author-email: oliveira.n3@gmail.com
 License: MIT
 Keywords: better git blame history curses ncurses
 Platform: UNKNOWN
```

### Comparing `bblame-0.6.4/README.rst` & `bblame-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `bblame-0.6.4/bblame.egg-info/PKG-INFO` & `bblame-0.7.0/bblame.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblame
-Version: 0.6.4
+Version: 0.7.0
 Summary: An ncurses app for browsing file git history
 Home-page: https://bitbucket.org/niko333/betterblame
 Author: Niko Oliveira
 Author-email: oliveira.n3@gmail.com
 License: MIT
 Keywords: better git blame history curses ncurses
 Platform: UNKNOWN
```

### Comparing `bblame-0.6.4/bblame.egg-info/SOURCES.txt` & `bblame-0.7.0/bblame.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -16,9 +16,10 @@
 betterblame/content.py
 betterblame/git.py
 betterblame/highlight.py
 betterblame/modes.py
 betterblame/options.py
 betterblame/screen.py
 betterblame/search.py
+betterblame/sh.py
 betterblame/util.py
 betterblame/version.py
```

### Comparing `bblame-0.6.4/betterblame/actions.py` & `bblame-0.7.0/betterblame/actions.py`

 * *Files identical despite different names*

### Comparing `bblame-0.6.4/betterblame/bblame.py` & `bblame-0.7.0/betterblame/bblame.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 import sys
 import errno
 import argparse
 import logging
 import traceback
 import tempfile
 
-import sh
-
 from . import screen
 from . import git
 from . import actions
 from . import version
+from .sh import sh
 
 # Setup logging to a temporary dir if we can find one
 TEMP_DIR = tempfile.gettempdir()
 LOG_FORMAT = ('%(asctime)s|%(levelname)s|'
               '%(module)s.%(funcName)s:%(lineno)d|'
               '%(message)s')
 DATE_FORMAT = '%b-%d %H:%M'
```

### Comparing `bblame-0.6.4/betterblame/content.py` & `bblame-0.7.0/betterblame/content.py`

 * *Files identical despite different names*

### Comparing `bblame-0.6.4/betterblame/git.py` & `bblame-0.7.0/betterblame/git.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 import os
 import re
 import curses
 import logging
 from datetime import datetime
 from collections import namedtuple
 
-import sh
 
 from .highlight import get_lexer, highlight_lines
 from .content import Line, BaseContent
 from .util import left_str_strip
+from .sh import sh
 
 
 class BadRevException(Exception):
     """Simple custom exception to make exception handling easier up the
     stack"""
     pass
```

### Comparing `bblame-0.6.4/betterblame/highlight.py` & `bblame-0.7.0/betterblame/highlight.py`

 * *Files identical despite different names*

### Comparing `bblame-0.6.4/betterblame/options.py` & `bblame-0.7.0/betterblame/options.py`

 * *Files identical despite different names*

### Comparing `bblame-0.6.4/betterblame/screen.py` & `bblame-0.7.0/betterblame/screen.py`

 * *Files identical despite different names*

### Comparing `bblame-0.6.4/betterblame/search.py` & `bblame-0.7.0/betterblame/search.py`

 * *Files identical despite different names*

### Comparing `bblame-0.6.4/betterblame/util.py` & `bblame-0.7.0/betterblame/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     return string[len(str_to_strip):]
 
 
 def check_string(string, msg):
     """Checks if <string> is a string type in a python 2 and 3 compatible way.
     Raises <msg> in the AssertionError """
     try:
-        basestring
+        basestring  # pylint: disable=E0601
     except NameError:
         basestring = str
     assert isinstance(string, basestring), msg
 
 
 # In this case I really do want an object pylint, but thanks...
 # pylint: disable=R0903
```

### Comparing `bblame-0.6.4/setup.py` & `bblame-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                    'Programming Language :: Python :: 3'],
       keywords=['better git blame history curses ncurses'],
       packages=[PACKAGE_NAME],
       install_requires=[
           'texteditpad',
           'pygments',
           'future',
-          'sh',
+          'sh>=2',
           'six',
       ],
       scripts=[PROG_NAME],
       # entry_points={
       #     'console_scripts': [
       #         'bblame = bblame.bblame:main',
       #     ]
```

