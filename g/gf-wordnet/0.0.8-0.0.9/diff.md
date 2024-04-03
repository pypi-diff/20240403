# Comparing `tmp/gf-wordnet-0.0.8.tar.gz` & `tmp/gf-wordnet-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gf-wordnet-0.0.8.tar", last modified: Mon Sep 18 11:31:02 2023, max compression
+gzip compressed data, was "gf-wordnet-0.0.9.tar", last modified: Mon Sep 18 11:35:25 2023, max compression
```

## Comparing `gf-wordnet-0.0.8.tar` & `gf-wordnet-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:31:02.329132 gf-wordnet-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    21930 2023-09-18 11:31:02.329132 gf-wordnet-0.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:31:02.329132 gf-wordnet-0.0.8/gf_wordnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21930 2023-09-18 11:31:02.000000 gf-wordnet-0.0.8/gf_wordnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-09-18 11:31:02.000000 gf-wordnet-0.0.8/gf_wordnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 11:31:02.000000 gf-wordnet-0.0.8/gf_wordnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 11:31:02.000000 gf-wordnet-0.0.8/gf_wordnet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-18 11:31:02.000000 gf-wordnet-0.0.8/gf_wordnet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-18 11:31:02.000000 gf-wordnet-0.0.8/gf_wordnet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-18 11:31:02.329132 gf-wordnet-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-09-18 11:30:53.000000 gf-wordnet-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:31:02.329132 gf-wordnet-0.0.8/wordnet/
--rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-09-18 11:30:53.000000 gf-wordnet-0.0.8/wordnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    70377 2023-09-18 11:30:53.000000 gf-wordnet-0.0.8/wordnet/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13111 2023-09-18 11:30:53.000000 gf-wordnet-0.0.8/wordnet/_semantics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:35:25.642263 gf-wordnet-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2023-09-18 11:35:25.642263 gf-wordnet-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21644 2023-09-18 11:35:17.000000 gf-wordnet-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:35:25.642263 gf-wordnet-0.0.9/gf_wordnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21930 2023-09-18 11:35:25.000000 gf-wordnet-0.0.9/gf_wordnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2023-09-18 11:35:25.000000 gf-wordnet-0.0.9/gf_wordnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 11:35:25.000000 gf-wordnet-0.0.9/gf_wordnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-18 11:35:25.000000 gf-wordnet-0.0.9/gf_wordnet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-09-18 11:35:25.000000 gf-wordnet-0.0.9/gf_wordnet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2023-09-18 11:35:25.000000 gf-wordnet-0.0.9/gf_wordnet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-18 11:35:25.642263 gf-wordnet-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2023-09-18 11:35:17.000000 gf-wordnet-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-18 11:35:25.642263 gf-wordnet-0.0.9/wordnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     5584 2023-09-18 11:35:17.000000 gf-wordnet-0.0.9/wordnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70377 2023-09-18 11:35:17.000000 gf-wordnet-0.0.9/wordnet/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13111 2023-09-18 11:35:17.000000 gf-wordnet-0.0.9/wordnet/_semantics.py
```

### Comparing `gf-wordnet-0.0.8/PKG-INFO` & `gf-wordnet-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gf-wordnet
-Version: 0.0.8
+Version: 0.0.9
 Summary: An API to the GF WordNet.
 Home-page: https://github.com/GrammaticalFramework/gf-wordnet
 Author: Krasimir Angelov
 Author-email: kr.angelov@gmail.com
 License: BSD
 Keywords: GF WordNet
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gf-wordnet Version: 0.0.8 Summary: An API to the GF
+Metadata-Version: 2.1 Name: gf-wordnet Version: 0.0.9 Summary: An API to the GF
 WordNet. Home-page: https://github.com/GrammaticalFramework/gf-wordnet Author:
 Krasimir Angelov Author-email: kr.angelov@gmail.com License: BSD Keywords: GF
 WordNet Description-Content-Type: text/markdown # GF WordNet 1. [The Lexicon]
 (#the-lexicon) 2. [WordNet Domains](#wordnet-domains) 3. [Treebank](#treebank)
 4. [VerbNet](#verbnet) 5. [Wikipedia Images](#wikipedia-images) 6. [Browsing
 and Editing](#browsing-and-editing) 7. [The Python Interface](#the-python-
 interface) - [Words](#words) - [Synsets](#synsets) - [Lexemes](#lexemes) -
```

### Comparing `gf-wordnet-0.0.8/gf_wordnet.egg-info/PKG-INFO` & `gf-wordnet-0.0.9/gf_wordnet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gf-wordnet
-Version: 0.0.8
+Version: 0.0.9
 Summary: An API to the GF WordNet.
 Home-page: https://github.com/GrammaticalFramework/gf-wordnet
 Author: Krasimir Angelov
 Author-email: kr.angelov@gmail.com
 License: BSD
 Keywords: GF WordNet
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gf-wordnet Version: 0.0.8 Summary: An API to the GF
+Metadata-Version: 2.1 Name: gf-wordnet Version: 0.0.9 Summary: An API to the GF
 WordNet. Home-page: https://github.com/GrammaticalFramework/gf-wordnet Author:
 Krasimir Angelov Author-email: kr.angelov@gmail.com License: BSD Keywords: GF
 WordNet Description-Content-Type: text/markdown # GF WordNet 1. [The Lexicon]
 (#the-lexicon) 2. [WordNet Domains](#wordnet-domains) 3. [Treebank](#treebank)
 4. [VerbNet](#verbnet) 5. [Wikipedia Images](#wikipedia-images) 6. [Browsing
 and Editing](#browsing-and-editing) 7. [The Python Interface](#the-python-
 interface) - [Words](#words) - [Synsets](#synsets) - [Lexemes](#lexemes) -
```

### Comparing `gf-wordnet-0.0.8/setup.py` & `gf-wordnet-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 def read(fname):
     import os
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name = "gf-wordnet",
-    version = "0.0.8",
+    version = "0.0.9",
     author = "Krasimir Angelov",
     author_email = "kr.angelov@gmail.com",
     description = ("An API to the GF WordNet."),
     license = "BSD",
     keywords = "GF WordNet",
     url = "https://github.com/GrammaticalFramework/gf-wordnet",
     packages=['wordnet'],
     install_requires=['pgf','daison'],
-    long_description=read("../README.md"),
+    long_description=read("README.md"),
     long_description_content_type="text/markdown",
     zip_safe=False
 )
```

### Comparing `gf-wordnet-0.0.8/wordnet/__init__.py` & `gf-wordnet-0.0.9/wordnet/__init__.py`

 * *Files identical despite different names*

### Comparing `gf-wordnet-0.0.8/wordnet/_api.py` & `gf-wordnet-0.0.9/wordnet/_api.py`

 * *Files identical despite different names*

### Comparing `gf-wordnet-0.0.8/wordnet/_semantics.py` & `gf-wordnet-0.0.9/wordnet/_semantics.py`

 * *Files identical despite different names*

