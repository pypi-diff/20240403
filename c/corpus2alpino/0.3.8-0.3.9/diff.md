# Comparing `tmp/corpus2alpino-0.3.8.tar.gz` & `tmp/corpus2alpino-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/corpus2alpino-0.3.8.tar", last modified: Mon Feb  7 16:52:07 2022, max compression
+gzip compressed data, was "dist/corpus2alpino-0.3.9.tar", last modified: Thu Jul 14 14:16:49 2022, max compression
```

## Comparing `corpus2alpino-0.3.8.tar` & `corpus2alpino-0.3.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/
--rw-r--r--   0 3248526    (502) staff       (20)     1082 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/LICENSE
--rw-r--r--   0 3248526    (502) staff       (20)     3511 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/PKG-INFO
--rw-r--r--   0 3248526    (502) staff       (20)     2967 2022-01-27 15:35:33.000000 corpus2alpino-0.3.8/README.md
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino/
--rw-r--r--   0 3248526    (502) staff       (20)        0 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/__init__.py
--rw-r--r--   0 3248526    (502) staff       (20)     4216 2020-10-22 16:33:48.000000 corpus2alpino-0.3.8/corpus2alpino/__main__.py
--rw-r--r--   0 3248526    (502) staff       (20)     2327 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/abstracts.py
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino/annotators/
--rw-r--r--   0 3248526    (502) staff       (20)        0 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/annotators/__init__.py
--rw-r--r--   0 3248526    (502) staff       (20)     2072 2020-10-22 16:33:48.000000 corpus2alpino-0.3.8/corpus2alpino/annotators/alpino.py
--rw-r--r--   0 3248526    (502) staff       (20)     5779 2020-10-22 16:33:48.000000 corpus2alpino-0.3.8/corpus2alpino/annotators/alpino_client.py
--rw-r--r--   0 3248526    (502) staff       (20)     4459 2020-10-22 16:33:48.000000 corpus2alpino-0.3.8/corpus2alpino/annotators/enrich_lassy.py
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino/collectors/
--rw-r--r--   0 3248526    (502) staff       (20)        0 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/collectors/__init__.py
--rw-r--r--   0 3248526    (502) staff       (20)     1655 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/collectors/filesystem.py
--rw-r--r--   0 3248526    (502) staff       (20)     1345 2022-01-27 15:35:33.000000 corpus2alpino-0.3.8/corpus2alpino/converter.py
--rw-r--r--   0 3248526    (502) staff       (20)     1653 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/models.py
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino/readers/
--rw-r--r--   0 3248526    (502) staff       (20)        0 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/readers/__init__.py
--rw-r--r--   0 3248526    (502) staff       (20)      760 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/readers/alpino_brackets.py
--rw-r--r--   0 3248526    (502) staff       (20)     1140 2022-01-27 15:35:33.000000 corpus2alpino-0.3.8/corpus2alpino/readers/auto.py
--rw-r--r--   0 3248526    (502) staff       (20)     2446 2020-06-09 14:21:16.000000 corpus2alpino-0.3.8/corpus2alpino/readers/chat.py
--rw-r--r--   0 3248526    (502) staff       (20)     5557 2022-01-27 15:35:33.000000 corpus2alpino-0.3.8/corpus2alpino/readers/folia.py
--rw-r--r--   0 3248526    (502) staff       (20)     2919 2021-05-03 10:30:11.000000 corpus2alpino-0.3.8/corpus2alpino/readers/lassy.py
--rw-r--r--   0 3248526    (502) staff       (20)     3832 2022-01-27 15:35:33.000000 corpus2alpino-0.3.8/corpus2alpino/readers/paqu.py
--rw-r--r--   0 3248526    (502) staff       (20)    10629 2022-01-27 15:35:33.000000 corpus2alpino-0.3.8/corpus2alpino/readers/tei.py
--rw-r--r--   0 3248526    (502) staff       (20)      636 2022-01-27 15:35:33.000000 corpus2alpino-0.3.8/corpus2alpino/readers/tokenizer.py
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino/targets/
--rw-r--r--   0 3248526    (502) staff       (20)        0 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/targets/__init__.py
--rw-r--r--   0 3248526    (502) staff       (20)      548 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/targets/console.py
--rw-r--r--   0 3248526    (502) staff       (20)     2603 2020-10-22 16:33:48.000000 corpus2alpino-0.3.8/corpus2alpino/targets/filesystem.py
--rw-r--r--   0 3248526    (502) staff       (20)      616 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/targets/memory.py
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino/writers/
--rw-r--r--   0 3248526    (502) staff       (20)        0 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/writers/__init__.py
--rw-r--r--   0 3248526    (502) staff       (20)     3910 2020-10-22 16:33:48.000000 corpus2alpino-0.3.8/corpus2alpino/writers/lassy.py
--rw-r--r--   0 3248526    (502) staff       (20)     2257 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/corpus2alpino/writers/paqu.py
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino.egg-info/
--rw-r--r--   0 3248526    (502) staff       (20)     3511 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino.egg-info/PKG-INFO
--rw-r--r--   0 3248526    (502) staff       (20)     1266 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino.egg-info/SOURCES.txt
--rw-r--r--   0 3248526    (502) staff       (20)        1 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino.egg-info/dependency_links.txt
--rw-r--r--   0 3248526    (502) staff       (20)       63 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino.egg-info/entry_points.txt
--rw-r--r--   0 3248526    (502) staff       (20)       50 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino.egg-info/requires.txt
--rw-r--r--   0 3248526    (502) staff       (20)       20 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/corpus2alpino.egg-info/top_level.txt
--rw-r--r--   0 3248526    (502) staff       (20)        1 2020-01-21 12:51:37.000000 corpus2alpino-0.3.8/corpus2alpino.egg-info/zip-safe
--rw-r--r--   0 3248526    (502) staff       (20)       38 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/setup.cfg
--rw-r--r--   0 3248526    (502) staff       (20)     1203 2022-02-07 16:51:21.000000 corpus2alpino-0.3.8/setup.py
-drwxr-xr-x   0 3248526    (502) staff       (20)        0 2022-02-07 16:52:07.000000 corpus2alpino-0.3.8/tests/
--rw-r--r--   0 3248526    (502) staff       (20)        0 2020-01-09 15:05:41.000000 corpus2alpino-0.3.8/tests/__init__.py
--rw-r--r--   0 3248526    (502) staff       (20)     1496 2020-10-22 16:33:48.000000 corpus2alpino-0.3.8/tests/test_corpus2alpino.py
--rw-r--r--   0 3248526    (502) staff       (20)     1237 2020-10-22 16:33:48.000000 corpus2alpino-0.3.8/tests/test_enrich_lassy.py
--rwxr-xr-x   0 3248526    (502) staff       (20)     1387 2022-01-27 15:35:33.000000 corpus2alpino-0.3.8/tests/update_test_outputs.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1082 2018-03-02 15:06:23.000000 corpus2alpino-0.3.9/LICENSE
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     3485 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/PKG-INFO
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2941 2022-07-14 14:15:26.000000 corpus2alpino-0.3.9/README.md
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2018-03-02 15:06:23.000000 corpus2alpino-0.3.9/corpus2alpino/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     4190 2022-07-14 14:15:26.000000 corpus2alpino-0.3.9/corpus2alpino/__main__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2327 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/abstracts.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino/annotators/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/annotators/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2072 2022-01-27 13:04:05.000000 corpus2alpino-0.3.9/corpus2alpino/annotators/alpino.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     5779 2022-01-27 13:04:05.000000 corpus2alpino-0.3.9/corpus2alpino/annotators/alpino_client.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     4459 2022-01-27 13:04:05.000000 corpus2alpino-0.3.9/corpus2alpino/annotators/enrich_lassy.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino/collectors/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/collectors/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1655 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/collectors/filesystem.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1345 2022-07-14 14:15:23.000000 corpus2alpino-0.3.9/corpus2alpino/converter.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1653 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/models.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino/readers/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/readers/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      760 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/readers/alpino_brackets.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1140 2022-07-14 14:15:23.000000 corpus2alpino-0.3.9/corpus2alpino/readers/auto.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2446 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/readers/chat.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     5557 2022-07-14 14:15:23.000000 corpus2alpino-0.3.9/corpus2alpino/readers/folia.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2919 2022-01-27 13:04:05.000000 corpus2alpino-0.3.9/corpus2alpino/readers/lassy.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     3832 2022-07-14 14:15:23.000000 corpus2alpino-0.3.9/corpus2alpino/readers/paqu.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)    10629 2022-07-14 14:15:23.000000 corpus2alpino-0.3.9/corpus2alpino/readers/tei.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      636 2022-07-14 14:15:23.000000 corpus2alpino-0.3.9/corpus2alpino/readers/tokenizer.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino/targets/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/targets/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      548 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/targets/console.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2692 2022-07-14 14:15:26.000000 corpus2alpino-0.3.9/corpus2alpino/targets/filesystem.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)      616 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/targets/memory.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino/writers/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/writers/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     3910 2022-01-27 13:04:05.000000 corpus2alpino-0.3.9/corpus2alpino/writers/lassy.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     2257 2020-05-07 09:34:48.000000 corpus2alpino-0.3.9/corpus2alpino/writers/paqu.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino.egg-info/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     3485 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino.egg-info/PKG-INFO
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1266 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino.egg-info/SOURCES.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        1 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino.egg-info/dependency_links.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)       63 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino.egg-info/entry_points.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)       50 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino.egg-info/requires.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)       20 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/corpus2alpino.egg-info/top_level.txt
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        1 2018-10-31 10:08:53.000000 corpus2alpino-0.3.9/corpus2alpino.egg-info/zip-safe
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)       38 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/setup.cfg
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1203 2022-07-14 14:15:30.000000 corpus2alpino-0.3.9/setup.py
+drwxrwxr-x   0 sheean    (1000) sheean    (1000)        0 2022-07-14 14:16:49.000000 corpus2alpino-0.3.9/tests/
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)        0 2018-03-02 15:06:23.000000 corpus2alpino-0.3.9/tests/__init__.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1496 2022-01-27 13:04:05.000000 corpus2alpino-0.3.9/tests/test_corpus2alpino.py
+-rw-rw-r--   0 sheean    (1000) sheean    (1000)     1237 2022-01-27 13:04:05.000000 corpus2alpino-0.3.9/tests/test_enrich_lassy.py
+-rwxrwxr-x   0 sheean    (1000) sheean    (1000)     1387 2022-07-14 14:15:23.000000 corpus2alpino-0.3.9/tests/update_test_outputs.py
```

### Comparing `corpus2alpino-0.3.8/LICENSE` & `corpus2alpino-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/PKG-INFO` & `corpus2alpino-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corpus2alpino
-Version: 0.3.8
+Version: 0.3.9
 Summary: Converts FoLiA and TEI files to Alpino XML files
 Home-page: https://github.com/UUDigitalHumanitieslab/corpus2alpino
 Author: Sheean Spoel, Digital Humanities Lab, Utrecht University
 Author-email: s.j.j.spoel@uu.nl
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -90,15 +90,15 @@
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
 
 ## Requirements
 
 * [Alpino parser](http://www.let.rug.nl/vannoord/alp/Alpino) running as a server: `Alpino batch_command=alpino_server -notk server_port=7001`
-* Python 3.6 or higher (developed using 3.7.12).
+* Python 3.7 or higher
 * [libfolia-dev](https://packages.ubuntu.com/bionic/libfolia-dev)
 * [libxml2-dev](https://packages.ubuntu.com/bionic/libxml2-dev)
 
 ### Installation Instructions for Ubuntu
 
 ```bash
 sudo apt install libfolia-dev libxml2-dev
```

### Comparing `corpus2alpino-0.3.8/README.md` & `corpus2alpino-0.3.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
 
 ## Requirements
 
 * [Alpino parser](http://www.let.rug.nl/vannoord/alp/Alpino) running as a server: `Alpino batch_command=alpino_server -notk server_port=7001`
-* Python 3.6 or higher (developed using 3.7.12).
+* Python 3.7 or higher
 * [libfolia-dev](https://packages.ubuntu.com/bionic/libfolia-dev)
 * [libxml2-dev](https://packages.ubuntu.com/bionic/libxml2-dev)
 
 ### Installation Instructions for Ubuntu
 
 ```bash
 sudo apt install libfolia-dev libxml2-dev
```

### Comparing `corpus2alpino-0.3.8/corpus2alpino/__main__.py` & `corpus2alpino-0.3.9/corpus2alpino/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,21 +45,21 @@
             help='Output path')
         parser.add_argument(
             '-of', '--output_format', metavar='OUTPUT_FORMAT', type=str,
             default='paqu',
             help='Output format: can be lassy, paqu (default)'
         )
         parser.add_argument(
-            '-p', '--progress', metavar="BOOL", type=bool,
+            '-p', '--progress',
+            action='store_true',
             help='Show progress bar, automatically turned on file output')
-        parser.add_argument('-t', '--split_treebanks', action='store_true',
+        parser.add_argument('-t', '--split_treebanks',
+                            action='store_true',
                             help='Split treebanks to separate files')
 
-        parser.set_defaults(split_treebanks=False)
-
         # passthrough the subprocess arguments
         subprocess = None
         for i, arg in enumerate(args):
             if arg == "-sp" or arg == "--subprocess":
                 subprocess = args[i+1:]
                 args = args[:i]
                 break
@@ -76,15 +76,15 @@
                 executable = subprocess[0]
                 arguments = [arg for arg in subprocess[1:]] \
                     + subprocess[2:]
                 converter.annotators.append(
                     AlpinoAnnotator(executable, arguments))
 
             converter.writer = LassyWriter(not options.split_treebanks)
-        
+
         if options.enrichment != None:
             converter.annotators.append(EnrichLassyAnnotator(options.enrichment))
 
         if options.output_path != None:
             converter.target = FilesystemTarget(
                 options.output_path, not options.split_treebanks)
```

### Comparing `corpus2alpino-0.3.8/corpus2alpino/abstracts.py` & `corpus2alpino-0.3.9/corpus2alpino/abstracts.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/annotators/alpino.py` & `corpus2alpino-0.3.9/corpus2alpino/annotators/alpino.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/annotators/alpino_client.py` & `corpus2alpino-0.3.9/corpus2alpino/annotators/alpino_client.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/annotators/enrich_lassy.py` & `corpus2alpino-0.3.9/corpus2alpino/annotators/enrich_lassy.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/collectors/filesystem.py` & `corpus2alpino-0.3.9/corpus2alpino/collectors/filesystem.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/converter.py` & `corpus2alpino-0.3.9/corpus2alpino/converter.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/models.py` & `corpus2alpino-0.3.9/corpus2alpino/models.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/readers/alpino_brackets.py` & `corpus2alpino-0.3.9/corpus2alpino/readers/alpino_brackets.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/readers/auto.py` & `corpus2alpino-0.3.9/corpus2alpino/readers/auto.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/readers/chat.py` & `corpus2alpino-0.3.9/corpus2alpino/readers/chat.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/readers/folia.py` & `corpus2alpino-0.3.9/corpus2alpino/readers/folia.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/readers/lassy.py` & `corpus2alpino-0.3.9/corpus2alpino/readers/lassy.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/readers/paqu.py` & `corpus2alpino-0.3.9/corpus2alpino/readers/paqu.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/readers/tei.py` & `corpus2alpino-0.3.9/corpus2alpino/readers/tei.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/readers/tokenizer.py` & `corpus2alpino-0.3.9/corpus2alpino/readers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/targets/console.py` & `corpus2alpino-0.3.9/corpus2alpino/targets/console.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/targets/filesystem.py` & `corpus2alpino-0.3.9/corpus2alpino/targets/filesystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,24 @@
 
             if filename != None:
                 output_path = path.join(output_path, cast(str, filename))
             if suffix != None:
                 output_path = str(
                     Path(output_path).with_suffix(cast(str, suffix)))
 
-            if self.__current_output_path != output_path:
-                if self.file:  # type: ignore
-                    self.file.close()  # type: ignore
-                self.__current_output_path = output_path  # type: ignore
-                directory, filename = path.split(output_path)
-                makedirs(directory, exist_ok=True)
-                self.file = self.__open_unique(directory, filename)
+            # always open a new file when splitting in separate files
+            self.__current_output_path = None
+
+        if self.__current_output_path != output_path:
+            if self.file:  # type: ignore
+                self.file.close()  # type: ignore
+            self.__current_output_path = output_path  # type: ignore
+            directory, filename = path.split(output_path)
+            makedirs(directory, exist_ok=True)
+            self.file = self.__open_unique(directory, filename)
 
     def __open_unique(self, directory: str, filename: str):
         attempts = 0
         prefix = ""
         while True:
             if attempts > 0:
                 prefix = f"{attempts}-"
```

### Comparing `corpus2alpino-0.3.8/corpus2alpino/targets/memory.py` & `corpus2alpino-0.3.9/corpus2alpino/targets/memory.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/writers/lassy.py` & `corpus2alpino-0.3.9/corpus2alpino/writers/lassy.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino/writers/paqu.py` & `corpus2alpino-0.3.9/corpus2alpino/writers/paqu.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/corpus2alpino.egg-info/PKG-INFO` & `corpus2alpino-0.3.9/corpus2alpino.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corpus2alpino
-Version: 0.3.8
+Version: 0.3.9
 Summary: Converts FoLiA and TEI files to Alpino XML files
 Home-page: https://github.com/UUDigitalHumanitieslab/corpus2alpino
 Author: Sheean Spoel, Digital Humanities Lab, Utrecht University
 Author-email: s.j.j.spoel@uu.nl
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -90,15 +90,15 @@
 python setup.py sdist bdist_wheel
 twine upload dist/*
 ```
 
 ## Requirements
 
 * [Alpino parser](http://www.let.rug.nl/vannoord/alp/Alpino) running as a server: `Alpino batch_command=alpino_server -notk server_port=7001`
-* Python 3.6 or higher (developed using 3.7.12).
+* Python 3.7 or higher
 * [libfolia-dev](https://packages.ubuntu.com/bionic/libfolia-dev)
 * [libxml2-dev](https://packages.ubuntu.com/bionic/libxml2-dev)
 
 ### Installation Instructions for Ubuntu
 
 ```bash
 sudo apt install libfolia-dev libxml2-dev
```

### Comparing `corpus2alpino-0.3.8/corpus2alpino.egg-info/SOURCES.txt` & `corpus2alpino-0.3.9/corpus2alpino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/setup.py` & `corpus2alpino-0.3.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='corpus2alpino',
-                 version='0.3.8',
+                 version='0.3.9',
       description='Converts FoLiA and TEI files to Alpino XML files',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/UUDigitalHumanitieslab/corpus2alpino',
       author='Sheean Spoel, Digital Humanities Lab, Utrecht University',
       author_email='s.j.j.spoel@uu.nl',
       license='MIT',
       packages=setuptools.find_packages(),
       classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
           "Operating System :: OS Independent",
       ],
-      install_requires=['argparse', 'chamd>=0.5.1', 'folia',
+      install_requires=['argparse', 'chamd>=0.5.8', 'folia',
                         'spacy', 'tei-reader', 'tqdm'],
       python_requires='>=3.6',
       zip_safe=True,
       entry_points={
           'console_scripts': [
               'corpus2alpino = corpus2alpino.__main__:main'
           ]
```

### Comparing `corpus2alpino-0.3.8/tests/test_corpus2alpino.py` & `corpus2alpino-0.3.9/tests/test_corpus2alpino.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/tests/test_enrich_lassy.py` & `corpus2alpino-0.3.9/tests/test_enrich_lassy.py`

 * *Files identical despite different names*

### Comparing `corpus2alpino-0.3.8/tests/update_test_outputs.py` & `corpus2alpino-0.3.9/tests/update_test_outputs.py`

 * *Files identical despite different names*

