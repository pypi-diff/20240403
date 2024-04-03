# Comparing `tmp/pub.tools-5.0.1.tar.gz` & `tmp/pub.tools-5.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pub.tools-5.0.1.tar", last modified: Fri Mar 29 16:59:10 2024, max compression
+gzip compressed data, was "pub.tools-5.0.2.tar", last modified: Wed Apr  3 17:10:34 2024, max compression
```

## Comparing `pub.tools-5.0.1.tar` & `pub.tools-5.0.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:59:10.168382 pub.tools-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-29 16:59:03.000000 pub.tools-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-29 16:59:10.168382 pub.tools-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-03-29 16:59:03.000000 pub.tools-5.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:59:10.164382 pub.tools-5.0.1/pub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:59:10.168382 pub.tools-5.0.1/pub/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/citations.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/cooking.py
--rw-r--r--   0 runner    (1001) docker     (127)    22699 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/entrez.py
--rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/isbn.py
--rw-r--r--   0 runner    (1001) docker     (127)  1443107 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/journals.json
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/journals.py
--rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:59:10.168382 pub.tools-5.0.1/pub/tools/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/tests/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/tests/test_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    25755 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/tests/test_entrez.py
--rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pub/tools/tests/test_journals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 16:59:10.168382 pub.tools-5.0.1/pub.tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-03-29 16:59:10.000000 pub.tools-5.0.1/pub.tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-03-29 16:59:10.000000 pub.tools-5.0.1/pub.tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 16:59:10.000000 pub.tools-5.0.1/pub.tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-29 16:59:10.000000 pub.tools-5.0.1/pub.tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-29 16:59:10.000000 pub.tools-5.0.1/pub.tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-29 16:59:03.000000 pub.tools-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 16:59:10.168382 pub.tools-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.686735 pub.tools-5.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 17:10:29.000000 pub.tools-5.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-03 17:10:34.686735 pub.tools-5.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-03 17:10:29.000000 pub.tools-5.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.682736 pub.tools-5.0.2/pub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.686735 pub.tools-5.0.2/pub/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2245 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/cooking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22699 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/entrez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8431 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/isbn.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1443107 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/journals.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/journals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.686735 pub.tools-5.0.2/pub/tools/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23689 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17851 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25755 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_entrez.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7902 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pub/tools/tests/test_journals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:34.686735 pub.tools-5.0.2/pub.tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 17:10:34.000000 pub.tools-5.0.2/pub.tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-03 17:10:29.000000 pub.tools-5.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:10:34.686735 pub.tools-5.0.2/setup.cfg
```

### Comparing `pub.tools-5.0.1/PKG-INFO` & `pub.tools-5.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pub.tools
-Version: 5.0.1
+Version: 5.0.2
 Summary: Get publication metadata from NCBI's eUtils and generate citations.
 Author-email: Eric Wohnlich <wohnlice@imsweb.com>
 License: GPL
 Project-URL: homepage, https://github.com/imsweb/pub.tools
 Project-URL: documentation, https://imsweb.github.io/pub.tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pub.tools-5.0.1/README.md` & `pub.tools-5.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/citations.py` & `pub.tools-5.0.2/pub/tools/citations.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/cooking.py` & `pub.tools-5.0.2/pub/tools/cooking.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/entrez.py` & `pub.tools-5.0.2/pub/tools/entrez.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/formatting.py` & `pub.tools-5.0.2/pub/tools/formatting.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/isbn.py` & `pub.tools-5.0.2/pub/tools/isbn.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/journals.json` & `pub.tools-5.0.2/pub/tools/journals.json`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/journals.py` & `pub.tools-5.0.2/pub/tools/journals.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/schema.py` & `pub.tools-5.0.2/pub/tools/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,16 @@
                     setattr(val, f.name, munge(getattr(val, f.name), escape))
                 return val
             elif isinstance(val, str):
                 if escape:
                     return unescape(str(val))  # this removes the BioPython StringElement class
                 else:
                     return str(val)
+            elif isinstance(val, bool):
+                return val
             else:
                 logger.info(f'Unknown type from Biopython: {type(val)}')
                 return val
 
         for field in dataclasses.fields(self):
             field = field.name
             if escape and field not in ['title', 'abstract']:
```

### Comparing `pub.tools-5.0.1/pub/tools/tests/test_citations.py` & `pub.tools-5.0.2/pub/tools/tests/test_citations.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/tests/test_compatibility.py` & `pub.tools-5.0.2/pub/tools/tests/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/tests/test_entrez.py` & `pub.tools-5.0.2/pub/tools/tests/test_entrez.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/tests/test_formatting.py` & `pub.tools-5.0.2/pub/tools/tests/test_formatting.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub/tools/tests/test_journals.py` & `pub.tools-5.0.2/pub/tools/tests/test_journals.py`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pub.tools.egg-info/PKG-INFO` & `pub.tools-5.0.2/pub.tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pub.tools
-Version: 5.0.1
+Version: 5.0.2
 Summary: Get publication metadata from NCBI's eUtils and generate citations.
 Author-email: Eric Wohnlich <wohnlice@imsweb.com>
 License: GPL
 Project-URL: homepage, https://github.com/imsweb/pub.tools
 Project-URL: documentation, https://imsweb.github.io/pub.tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `pub.tools-5.0.1/pub.tools.egg-info/SOURCES.txt` & `pub.tools-5.0.2/pub.tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pub.tools-5.0.1/pyproject.toml` & `pub.tools-5.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pub.tools"
-version = "5.0.1"
+version = "5.0.2"
 readme = "README.md"
 requires-python = ">=3.11"
 description = "Get publication metadata from NCBI's eUtils and generate citations."
 classifiers = [
           "Programming Language :: Python :: 3",
           "Topic :: Scientific/Engineering",
           "Topic :: Scientific/Engineering :: Bio-Informatics",
```

