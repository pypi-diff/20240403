# Comparing `tmp/pdfdol-0.1.2.tar.gz` & `tmp/pdfdol-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfdol-0.1.2.tar", last modified: Tue Jan  2 15:00:12 2024, max compression
+gzip compressed data, was "pdfdol-0.1.3.tar", last modified: Wed Apr  3 12:29:25 2024, max compression
```

## Comparing `pdfdol-0.1.2.tar` & `pdfdol-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:00:12.161297 pdfdol-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-02 14:59:43.000000 pdfdol-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-01-02 15:00:12.161297 pdfdol-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-01-02 14:59:43.000000 pdfdol-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:00:12.157297 pdfdol-0.1.2/pdfdol/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-02 14:59:43.000000 pdfdol-0.1.2/pdfdol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-01-02 14:59:43.000000 pdfdol-0.1.2/pdfdol/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:00:12.157297 pdfdol-0.1.2/pdfdol/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-01-02 14:59:43.000000 pdfdol-0.1.2/pdfdol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-01-02 14:59:43.000000 pdfdol-0.1.2/pdfdol/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-02 14:59:43.000000 pdfdol-0.1.2/pdfdol/tests/utils_for_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-02 15:00:12.157297 pdfdol-0.1.2/pdfdol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-01-02 15:00:12.000000 pdfdol-0.1.2/pdfdol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-01-02 15:00:12.000000 pdfdol-0.1.2/pdfdol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 15:00:12.000000 pdfdol-0.1.2/pdfdol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-02 15:00:12.000000 pdfdol-0.1.2/pdfdol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-02 15:00:12.000000 pdfdol-0.1.2/pdfdol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-02 15:00:12.000000 pdfdol-0.1.2/pdfdol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-02 15:00:12.161297 pdfdol-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-01-02 14:59:43.000000 pdfdol-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:29:25.600716 pdfdol-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 12:28:54.000000 pdfdol-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 12:29:25.600716 pdfdol-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 12:28:54.000000 pdfdol-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:29:25.600716 pdfdol-0.1.3/pdfdol/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 12:28:54.000000 pdfdol-0.1.3/pdfdol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-03 12:28:54.000000 pdfdol-0.1.3/pdfdol/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:29:25.600716 pdfdol-0.1.3/pdfdol/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 12:28:54.000000 pdfdol-0.1.3/pdfdol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-03 12:28:54.000000 pdfdol-0.1.3/pdfdol/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 12:28:54.000000 pdfdol-0.1.3/pdfdol/tests/utils_for_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:29:25.600716 pdfdol-0.1.3/pdfdol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 12:29:25.000000 pdfdol-0.1.3/pdfdol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-03 12:29:25.000000 pdfdol-0.1.3/pdfdol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:29:25.000000 pdfdol-0.1.3/pdfdol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:29:25.000000 pdfdol-0.1.3/pdfdol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 12:29:25.000000 pdfdol-0.1.3/pdfdol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 12:29:25.000000 pdfdol-0.1.3/pdfdol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-03 12:29:25.600716 pdfdol-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 12:28:54.000000 pdfdol-0.1.3/setup.py
```

### Comparing `pdfdol-0.1.2/LICENSE` & `pdfdol-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfdol-0.1.2/PKG-INFO` & `pdfdol-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfdol
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data Object Layer for PDF data
 Author: OtoSense
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pdfdol-0.1.2/README.md` & `pdfdol-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pdfdol-0.1.2/pdfdol/base.py` & `pdfdol-0.1.3/pdfdol/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 from dol import Files, wrap_kvs, Pipe, KeyCodecs, add_ipython_key_completions
 from pypdf import PdfReader
 from io import BytesIO
 
 bytes_to_pdf_reader_obj = Pipe(BytesIO, PdfReader)
 
 
-def _read_pdf_text(pdf_reader):
+def read_pdf_text(pdf_reader):
     text_pages = []
     for page in pdf_reader.pages:
         text_pages.append(page.extract_text())
     return text_pages
 
 
 bytes_to_pdf_obj_wrap = wrap_kvs(obj_of_data=bytes_to_pdf_reader_obj)
 
 filter_for_pdf_extension = KeyCodecs.suffixed('.pdf')
 
 bytes_to_pdf_text_pages = Pipe(
-    bytes_to_pdf_obj_wrap, wrap_kvs(obj_of_data=_read_pdf_text)
+    bytes_to_pdf_obj_wrap, wrap_kvs(obj_of_data=read_pdf_text)
 )
 
 pdf_files_reader_wrap = Pipe(
     filter_for_pdf_extension, bytes_to_pdf_text_pages, add_ipython_key_completions
 )
 
 PdfFilesReader = pdf_files_reader_wrap(Files)
```

### Comparing `pdfdol-0.1.2/pdfdol.egg-info/PKG-INFO` & `pdfdol-0.1.3/pdfdol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfdol
-Version: 0.1.2
+Version: 0.1.3
 Summary: Data Object Layer for PDF data
 Author: OtoSense
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

