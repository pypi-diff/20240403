# Comparing `tmp/haruka_parser-0.4.5.tar.gz` & `tmp/haruka_parser-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haruka_parser-0.4.5.tar", last modified: Wed Apr  3 18:24:17 2024, max compression
+gzip compressed data, was "haruka_parser-0.4.6.tar", last modified: Wed Apr  3 18:38:36 2024, max compression
```

## Comparing `haruka_parser-0.4.5.tar` & `haruka_parser-0.4.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.311299 haruka_parser-0.4.5/haruka_parser/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/haruka_parser/dictionary/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/dictionary/banned_selectors.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/dictionary/boilerplate_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/dictionary/latex_words.txt
--rw-r--r--   0 runner    (1001) docker     (127)    15852 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/latex_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/line_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/meta_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/haruka_parser/mmltex/
--rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/cmarkup.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/entities.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/glayout.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/mmltex.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/scripts.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/tables.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/mmltex/tokens.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/readablity_lxml.py
--rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/time_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/tree_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/tree_processing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/haruka_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/haruka_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 18:24:17.000000 haruka_parser-0.4.5/haruka_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:24:17.315299 haruka_parser-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 18:24:10.000000 haruka_parser-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.269381 haruka_parser-0.4.6/haruka_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/haruka_parser/dictionary/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/dictionary/banned_selectors.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/dictionary/boilerplate_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/dictionary/latex_words.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    15963 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33604 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/latex_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/line_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23265 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/meta_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/haruka_parser/mmltex/
+-rw-r--r--   0 runner    (1001) docker     (127)    36723 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/cmarkup.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    71528 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/entities.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/glayout.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/mmltex.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/scripts.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     4327 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/tables.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    10654 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/mmltex/tokens.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    35530 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/readablity_lxml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14291 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/time_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15057 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/tree_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27039 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/tree_processing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9599 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/haruka_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/haruka_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 18:38:36.000000 haruka_parser-0.4.6/haruka_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:38:36.273381 haruka_parser-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 18:38:32.000000 haruka_parser-0.4.6/setup.py
```

### Comparing `haruka_parser-0.4.5/PKG-INFO` & `haruka_parser-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.5
+Version: 0.4.6
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.5 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.6 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.5/README.md` & `haruka_parser-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/dictionary/banned_selectors.txt` & `haruka_parser-0.4.6/haruka_parser/dictionary/banned_selectors.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/dictionary/boilerplate_words.txt` & `haruka_parser-0.4.6/haruka_parser/dictionary/boilerplate_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/dictionary/latex_words.txt` & `haruka_parser-0.4.6/haruka_parser/dictionary/latex_words.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/extract.py` & `haruka_parser-0.4.6/haruka_parser/extract.py`

 * *Files 0% similar despite different names*

```diff
@@ -321,14 +321,18 @@
         info["encode_type"] = encode_type
     else:
         raise TypeError("html must be str or bytes")
     
     if not html:
         return "", info
 
+    # this is a html parsing checking
+    get_lxml_tree(html)
+
+    # because this may cause segmentation fault
     pre_process_resiliparse_tree = HTMLTree.parse(html)
 
     # TODO: Using the same tree parser
     try: info["title"] = get_title(pre_process_resiliparse_tree)
     except: pass
 
     pre_process_resiliparse_tree, info = filter_tree(pre_process_resiliparse_tree, config, info)
```

### Comparing `haruka_parser-0.4.5/haruka_parser/latex_processing.py` & `haruka_parser-0.4.6/haruka_parser/latex_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/line_processing.py` & `haruka_parser-0.4.6/haruka_parser/line_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/meta_processing.py` & `haruka_parser-0.4.6/haruka_parser/meta_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/mmltex/cmarkup.xsl` & `haruka_parser-0.4.6/haruka_parser/mmltex/cmarkup.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/mmltex/entities.xsl` & `haruka_parser-0.4.6/haruka_parser/mmltex/entities.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/mmltex/glayout.xsl` & `haruka_parser-0.4.6/haruka_parser/mmltex/glayout.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/mmltex/mmltex.xsl` & `haruka_parser-0.4.6/haruka_parser/mmltex/mmltex.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/mmltex/scripts.xsl` & `haruka_parser-0.4.6/haruka_parser/mmltex/scripts.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/mmltex/tables.xsl` & `haruka_parser-0.4.6/haruka_parser/mmltex/tables.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/mmltex/tokens.xsl` & `haruka_parser-0.4.6/haruka_parser/mmltex/tokens.xsl`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/readablity_lxml.py` & `haruka_parser-0.4.6/haruka_parser/readablity_lxml.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/time_formatter.py` & `haruka_parser-0.4.6/haruka_parser/time_formatter.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/tree_cleaning.py` & `haruka_parser-0.4.6/haruka_parser/tree_cleaning.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/tree_processing.py` & `haruka_parser-0.4.6/haruka_parser/tree_processing.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser/utils.py` & `haruka_parser-0.4.6/haruka_parser/utils.py`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/haruka_parser.egg-info/PKG-INFO` & `haruka_parser-0.4.6/haruka_parser.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haruka_parser
-Version: 0.4.5
+Version: 0.4.6
 Summary: A simple HTML Parser
 Home-page: https://github.com/prnake/haruka-parser
 Author: papersnake
 Author-email: prnake@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.5 Summary: A simple HTML
+Metadata-Version: 2.1 Name: haruka_parser Version: 0.4.6 Summary: A simple HTML
 Parser Home-page: https://github.com/prnake/haruka-parser Author: papersnake
 Author-email: prnake@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Text Processing Classifier: Topic ::
 Text Processing :: Markup :: HTML Classifier: Topic :: Utilities Description-
 Content-Type: text/markdown Requires-Dist: py_asciimath Requires-Dist:
 inscriptis Requires-Dist: tabulate Requires-Dist: numpy Requires-Dist:
```

### Comparing `haruka_parser-0.4.5/haruka_parser.egg-info/SOURCES.txt` & `haruka_parser-0.4.6/haruka_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haruka_parser-0.4.5/setup.py` & `haruka_parser-0.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 # 0.1 version from OpenWebMath: https://github.com/keirp/OpenWebMath
 # OpenWebMath is made available under an ODC-By 1.0 license; users should also abide by the CommonCrawl ToU: https://commoncrawl.org/terms-of-use/. We do not alter the license of any of the underlying data.
 setup(
     name="haruka_parser",
-    version="0.4.5",
+    version="0.4.6",
     description="A simple HTML Parser",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="papersnake",
     author_email="prnake@gmail.com",
     url="https://github.com/prnake/haruka-parser",
     packages=["haruka_parser"],
```

