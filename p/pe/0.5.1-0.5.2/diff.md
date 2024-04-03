# Comparing `tmp/pe-0.5.1.tar.gz` & `tmp/pe-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pe-0.5.1.tar", last modified: Sun Dec 31 22:03:47 2023, max compression
+gzip compressed data, was "pe-0.5.2.tar", last modified: Wed Apr  3 04:35:20 2024, max compression
```

## Comparing `pe-0.5.1.tar` & `pe-0.5.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 22:03:47.455930 pe-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-12-31 22:03:37.000000 pe-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2023-12-31 22:03:47.455930 pe-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6931 2023-12-31 22:03:37.000000 pe-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 22:03:47.451930 pe-0.5.1/pe/
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-31 22:03:37.000000 pe-0.5.1/pe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_autoignore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)  1499202 2023-12-31 22:03:47.000000 pe-0.5.1/pe/_cy_machine.c
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_cy_machine.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    16828 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_cy_machine.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_disarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_escape.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_grammar.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_match.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8917 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     8074 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14035 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_py_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-31 22:03:37.000000 pe-0.5.1/pe/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2023-12-31 22:03:37.000000 pe-0.5.1/pe/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2023-12-31 22:03:37.000000 pe-0.5.1/pe/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2023-12-31 22:03:37.000000 pe-0.5.1/pe/operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    13448 2023-12-31 22:03:37.000000 pe-0.5.1/pe/packrat.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-31 22:03:37.000000 pe-0.5.1/pe/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 22:03:47.455930 pe-0.5.1/pe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9508 2023-12-31 22:03:47.000000 pe-0.5.1/pe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-12-31 22:03:47.000000 pe-0.5.1/pe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-31 22:03:47.000000 pe-0.5.1/pe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-12-31 22:03:47.000000 pe-0.5.1/pe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2023-12-31 22:03:47.000000 pe-0.5.1/pe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-12-31 22:03:37.000000 pe-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-31 22:03:47.455930 pe-0.5.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2023-12-31 22:03:37.000000 pe-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-31 22:03:47.455930 pe-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)      466 2023-12-31 22:03:37.000000 pe-0.5.1/test/test__definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-12-31 22:03:37.000000 pe-0.5.1/test/test__disarm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-12-31 22:03:37.000000 pe-0.5.1/test/test__match.py
--rw-r--r--   0 runner    (1001) docker     (127)     5184 2023-12-31 22:03:37.000000 pe-0.5.1/test/test__optimize.py
--rw-r--r--   0 runner    (1001) docker     (127)     3915 2023-12-31 22:03:37.000000 pe-0.5.1/test/test__parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2023-12-31 22:03:37.000000 pe-0.5.1/test/test_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2023-12-31 22:03:37.000000 pe-0.5.1/test/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2023-12-31 22:03:37.000000 pe-0.5.1/test/test_pe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2023-12-31 22:03:37.000000 pe-0.5.1/test/test_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:35:20.309709 pe-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-03 04:35:15.000000 pe-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-03 04:35:20.309709 pe-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-04-03 04:35:15.000000 pe-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:35:20.305709 pe-0.5.2/pe/
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-03 04:35:15.000000 pe-0.5.2/pe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_autoignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1503180 2024-04-03 04:35:20.000000 pe-0.5.2/pe/_cy_machine.c
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_cy_machine.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    16911 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_cy_machine.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_disarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_escape.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_grammar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9053 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8074 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14118 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_py_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 04:35:15.000000 pe-0.5.2/pe/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-03 04:35:15.000000 pe-0.5.2/pe/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-03 04:35:15.000000 pe-0.5.2/pe/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-04-03 04:35:15.000000 pe-0.5.2/pe/operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13448 2024-04-03 04:35:15.000000 pe-0.5.2/pe/packrat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 04:35:15.000000 pe-0.5.2/pe/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:35:20.309709 pe-0.5.2/pe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9508 2024-04-03 04:35:20.000000 pe-0.5.2/pe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-03 04:35:20.000000 pe-0.5.2/pe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:35:20.000000 pe-0.5.2/pe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 04:35:20.000000 pe-0.5.2/pe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-03 04:35:20.000000 pe-0.5.2/pe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-03 04:35:15.000000 pe-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:35:20.309709 pe-0.5.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1069 2024-04-03 04:35:15.000000 pe-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:35:20.309709 pe-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-03 04:35:15.000000 pe-0.5.2/test/test__definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 04:35:15.000000 pe-0.5.2/test/test__disarm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-04-03 04:35:15.000000 pe-0.5.2/test/test__match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-03 04:35:15.000000 pe-0.5.2/test/test__optimize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-03 04:35:15.000000 pe-0.5.2/test/test__parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-03 04:35:15.000000 pe-0.5.2/test/test_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-03 04:35:15.000000 pe-0.5.2/test/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-03 04:35:15.000000 pe-0.5.2/test/test_pe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-03 04:35:15.000000 pe-0.5.2/test/test_regression.py
```

### Comparing `pe-0.5.1/LICENSE` & `pe-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/PKG-INFO` & `pe-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe
-Version: 0.5.1
+Version: 0.5.2
 Summary: Library for Parsing Expression Grammars (PEG)
 Author-email: Michael Wayne Goodman <goodman.m.w@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Michael Wayne Goodman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pe Version: 0.5.1 Summary: Library for Parsing
+Metadata-Version: 2.1 Name: pe Version: 0.5.2 Summary: Library for Parsing
 Expression Grammars (PEG) Author-email: Michael Wayne Goodman
 gmail.com> License: MIT License Copyright (c) 2020 Michael Wayne Goodman
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `pe-0.5.1/README.md` & `pe-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/__init__.py` & `pe-0.5.2/pe/__init__.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_autoignore.py` & `pe-0.5.2/pe/_autoignore.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_constants.py` & `pe-0.5.2/pe/_constants.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_cy_machine.c` & `pe-0.5.2/pe/_cy_machine.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.7 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "pe._cy_machine",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_7" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030007F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -578,22 +608,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -643,15 +673,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -729,16 +759,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1082,15 +1117,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1169,15 +1204,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1272,32 +1307,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1339,15 +1357,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1579,55 +1597,55 @@
   int marking;
   int capturing;
   PyObject *action;
   PyObject *name;
 };
 
 
-/* "pe/_cy_machine.pyx":191
+/* "pe/_cy_machine.pyx":193
  * 
  * 
  * cdef class _Parser:             # <<<<<<<<<<<<<<
  *     cdef list pi
  * 
  */
 struct __pyx_obj_2pe_11_cy_machine__Parser {
   PyObject_HEAD
   struct __pyx_vtabstruct_2pe_11_cy_machine__Parser *__pyx_vtab;
   PyObject *pi;
 };
 
 
-/* "pe/_cy_machine.pyx":529
+/* "pe/_cy_machine.pyx":531
  * # Scanners #############################################################
  * 
  * cdef class Dot(Scanner):             # <<<<<<<<<<<<<<
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:
  */
 struct __pyx_obj_2pe_11_cy_machine_Dot {
   struct __pyx_obj_2pe_11_cy_machine_Scanner __pyx_base;
 };
 
 
-/* "pe/_cy_machine.pyx":536
+/* "pe/_cy_machine.pyx":538
  * 
  * 
  * cdef class Literal(Scanner):             # <<<<<<<<<<<<<<
  *     cdef str _x
  *     cdef int _xlen
  */
 struct __pyx_obj_2pe_11_cy_machine_Literal {
   struct __pyx_obj_2pe_11_cy_machine_Scanner __pyx_base;
   PyObject *_x;
   int _xlen;
 };
 
 
-/* "pe/_cy_machine.pyx":551
+/* "pe/_cy_machine.pyx":553
  * 
  * 
  * cdef class CharacterClass(Scanner):             # <<<<<<<<<<<<<<
  *     cdef:
  *         str _chars, _ranges
  */
 struct __pyx_obj_2pe_11_cy_machine_CharacterClass {
@@ -1637,41 +1655,41 @@
   int _rangelen;
   int _negate;
   int mincount;
   int maxcount;
 };
 
 
-/* "pe/_cy_machine.pyx":603
+/* "pe/_cy_machine.pyx":605
  * 
  * 
  * cdef class Regex(Scanner):             # <<<<<<<<<<<<<<
  *     cdef object _regex
  * 
  */
 struct __pyx_obj_2pe_11_cy_machine_Regex {
   struct __pyx_obj_2pe_11_cy_machine_Scanner __pyx_base;
   PyObject *_regex;
 };
 
 
-/* "pe/_cy_machine.pyx":400
+/* "pe/_cy_machine.pyx":402
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
 struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt {
   PyObject_HEAD
   PyObject *__pyx_v_pis;
 };
 
 
-/* "pe/_cy_machine.pyx":416
+/* "pe/_cy_machine.pyx":418
  *                             capturing=pi.capturing,
  *                             action=pi.action)]
  *     return [*(pi.copy() for _ in range(mincount) for pi in pis),             # <<<<<<<<<<<<<<
  *             Instruction(BRANCH, len(pis) + 2),
  *             *pis,
  */
 struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr {
@@ -1685,30 +1703,30 @@
   PyObject *(*__pyx_t_2)(PyObject *);
   PyObject *__pyx_t_3;
   Py_ssize_t __pyx_t_4;
   PyObject *(*__pyx_t_5)(PyObject *);
 };
 
 
-/* "pe/_cy_machine.pyx":566
+/* "pe/_cy_machine.pyx":568
  *         int maxcount = 1
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)             # <<<<<<<<<<<<<<
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)
  */
 struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr {
   PyObject_HEAD
   PyObject *__pyx_genexpr_arg_0;
   PyObject *__pyx_v_a;
   PyObject *__pyx_v_b;
 };
 
 
-/* "pe/_cy_machine.pyx":567
+/* "pe/_cy_machine.pyx":569
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)
  *         self._ranges = ''.join(a+b for a, b in ranges if b)             # <<<<<<<<<<<<<<
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate
  */
 struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_3_genexpr {
@@ -1731,72 +1749,72 @@
 struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner {
   int (*scan)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int __pyx_skip_dispatch, struct __pyx_opt_args_2pe_11_cy_machine_7Scanner_scan *__pyx_optional_args);
   int (*_scan)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int);
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
 
 
-/* "pe/_cy_machine.pyx":191
+/* "pe/_cy_machine.pyx":193
  * 
  * 
  * cdef class _Parser:             # <<<<<<<<<<<<<<
  *     cdef list pi
  * 
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine__Parser {
   int (*match)(struct __pyx_obj_2pe_11_cy_machine__Parser *, int, PyObject *, int, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch);
   struct __pyx_t_2pe_11_cy_machine_State *(*_match)(struct __pyx_obj_2pe_11_cy_machine__Parser *, int, PyObject *, int, PyObject *, PyObject *, PyObject *, struct __pyx_t_2pe_11_cy_machine_State *);
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine__Parser *__pyx_vtabptr_2pe_11_cy_machine__Parser;
 
 
-/* "pe/_cy_machine.pyx":529
+/* "pe/_cy_machine.pyx":531
  * # Scanners #############################################################
  * 
  * cdef class Dot(Scanner):             # <<<<<<<<<<<<<<
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine_Dot {
   struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner __pyx_base;
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Dot *__pyx_vtabptr_2pe_11_cy_machine_Dot;
 
 
-/* "pe/_cy_machine.pyx":536
+/* "pe/_cy_machine.pyx":538
  * 
  * 
  * cdef class Literal(Scanner):             # <<<<<<<<<<<<<<
  *     cdef str _x
  *     cdef int _xlen
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine_Literal {
   struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner __pyx_base;
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_Literal *__pyx_vtabptr_2pe_11_cy_machine_Literal;
 
 
-/* "pe/_cy_machine.pyx":551
+/* "pe/_cy_machine.pyx":553
  * 
  * 
  * cdef class CharacterClass(Scanner):             # <<<<<<<<<<<<<<
  *     cdef:
  *         str _chars, _ranges
  */
 
 struct __pyx_vtabstruct_2pe_11_cy_machine_CharacterClass {
   struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner __pyx_base;
 };
 static struct __pyx_vtabstruct_2pe_11_cy_machine_CharacterClass *__pyx_vtabptr_2pe_11_cy_machine_CharacterClass;
 
 
-/* "pe/_cy_machine.pyx":603
+/* "pe/_cy_machine.pyx":605
  * 
  * 
  * cdef class Regex(Scanner):             # <<<<<<<<<<<<<<
  *     cdef object _regex
  * 
  */
 
@@ -2098,16 +2116,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -2115,16 +2133,17 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2540,15 +2559,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -2935,14 +2954,15 @@
 static const char __pyx_k_str_2[] = "_str";
 static const char __pyx_k_super[] = "super";
 static const char __pyx_k_throw[] = "throw";
 static const char __pyx_k_Action[] = "Action";
 static const char __pyx_k_COMMON[] = "COMMON";
 static const char __pyx_k_INLINE[] = "INLINE";
 static const char __pyx_k_Parser[] = "_Parser";
+static const char __pyx_k_STRICT[] = "STRICT";
 static const char __pyx_k_action[] = "action";
 static const char __pyx_k_append[] = "append";
 static const char __pyx_k_cclass[] = "cclass";
 static const char __pyx_k_common[] = "common";
 static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_ignore[] = "ignore";
@@ -3000,14 +3020,15 @@
 static const char __pyx_k_metaclass[] = "__metaclass__";
 static const char __pyx_k_pe__match[] = "pe._match";
 static const char __pyx_k_pe__types[] = "pe._types";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_Definition[] = "Definition";
 static const char __pyx_k_IndexError[] = "IndexError";
+static const char __pyx_k_ParseError[] = "ParseError";
 static const char __pyx_k_autoignore[] = "autoignore";
 static const char __pyx_k_pe__errors[] = "pe._errors";
 static const char __pyx_k_pe__parser[] = "pe._parser";
 static const char __pyx_k_pe_actions[] = "pe.actions";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_Instruction[] = "Instruction";
@@ -3113,15 +3134,15 @@
 static PyObject *__pyx_pf_2pe_11_cy_machine_11Instruction_4__reduce_cython__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_11Instruction_6__setstate_cython__(struct __pyx_obj_2pe_11_cy_machine_Instruction *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_50__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser___init__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_grammar, PyObject *__pyx_v_ignore, PyObject *__pyx_v_flags); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_2start(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_4__contains__(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_name); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_52__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_6match(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_s, int __pyx_v_pos, CYTHON_UNUSED PyObject *__pyx_v_flags); /* proto */
+static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_6match(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_s, int __pyx_v_pos, PyObject *__pyx_v_flags); /* proto */
 static int __pyx_pf_2pe_11_cy_machine_7_Parser___init__(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self, PyObject *__pyx_v_pi); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_7_Parser_2match(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self, int __pyx_v_idx, PyObject *__pyx_v_s, int __pyx_v_pos, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, PyObject *__pyx_v_memo); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_7_Parser_4__reduce_cython__(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_7_Parser_6__setstate_cython__(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine__make_program(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_grammar); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_2_dot(CYTHON_UNUSED PyObject *__pyx_self, CYTHON_UNUSED PyObject *__pyx_v_defn); /* proto */
 static PyObject *__pyx_pf_2pe_11_cy_machine_4_lit(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_defn); /* proto */
@@ -3286,14 +3307,15 @@
   PyObject *__pyx_n_s_NOT;
   PyObject *__pyx_n_s_NO_CAP_OR_ACT;
   PyObject *__pyx_n_s_OPT;
   PyObject *__pyx_n_s_Operator;
   PyObject *__pyx_n_s_Optional;
   PyObject *__pyx_kp_s_Optional_Definition;
   PyObject *__pyx_n_s_PLS;
+  PyObject *__pyx_n_s_ParseError;
   PyObject *__pyx_n_s_Parser;
   PyObject *__pyx_n_s_Parser_2;
   PyObject *__pyx_n_s_Parser___reduce_cython;
   PyObject *__pyx_n_s_Parser___setstate_cython;
   PyObject *__pyx_n_s_Parser_match;
   PyObject *__pyx_n_s_PickleError;
   PyObject *__pyx_n_s_Program;
@@ -3301,14 +3323,15 @@
   PyObject *__pyx_n_s_RUL;
   PyObject *__pyx_n_s_Regex;
   PyObject *__pyx_n_s_Regex___reduce_cython;
   PyObject *__pyx_n_s_Regex___setstate_cython;
   PyObject *__pyx_n_s_Rule;
   PyObject *__pyx_n_s_SEQ;
   PyObject *__pyx_n_s_STR;
+  PyObject *__pyx_n_s_STRICT;
   PyObject *__pyx_n_s_SYM;
   PyObject *__pyx_n_s_Scanner;
   PyObject *__pyx_n_s_Scanner___reduce_cython;
   PyObject *__pyx_n_s_Scanner___setstate_cython;
   PyObject *__pyx_n_s_Scanner_scan;
   PyObject *__pyx_n_s_Tuple;
   PyObject *__pyx_kp_s_Tuple__Program__Index;
@@ -3695,14 +3718,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_NOT);
   Py_CLEAR(clear_module_state->__pyx_n_s_NO_CAP_OR_ACT);
   Py_CLEAR(clear_module_state->__pyx_n_s_OPT);
   Py_CLEAR(clear_module_state->__pyx_n_s_Operator);
   Py_CLEAR(clear_module_state->__pyx_n_s_Optional);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Optional_Definition);
   Py_CLEAR(clear_module_state->__pyx_n_s_PLS);
+  Py_CLEAR(clear_module_state->__pyx_n_s_ParseError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Parser);
   Py_CLEAR(clear_module_state->__pyx_n_s_Parser_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_Parser___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Parser___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Parser_match);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_Program);
@@ -3710,14 +3734,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_RUL);
   Py_CLEAR(clear_module_state->__pyx_n_s_Regex);
   Py_CLEAR(clear_module_state->__pyx_n_s_Regex___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Regex___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Rule);
   Py_CLEAR(clear_module_state->__pyx_n_s_SEQ);
   Py_CLEAR(clear_module_state->__pyx_n_s_STR);
+  Py_CLEAR(clear_module_state->__pyx_n_s_STRICT);
   Py_CLEAR(clear_module_state->__pyx_n_s_SYM);
   Py_CLEAR(clear_module_state->__pyx_n_s_Scanner);
   Py_CLEAR(clear_module_state->__pyx_n_s_Scanner___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Scanner___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Scanner_scan);
   Py_CLEAR(clear_module_state->__pyx_n_s_Tuple);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Tuple__Program__Index);
@@ -4082,14 +4107,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_NOT);
   Py_VISIT(traverse_module_state->__pyx_n_s_NO_CAP_OR_ACT);
   Py_VISIT(traverse_module_state->__pyx_n_s_OPT);
   Py_VISIT(traverse_module_state->__pyx_n_s_Operator);
   Py_VISIT(traverse_module_state->__pyx_n_s_Optional);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Optional_Definition);
   Py_VISIT(traverse_module_state->__pyx_n_s_PLS);
+  Py_VISIT(traverse_module_state->__pyx_n_s_ParseError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Parser);
   Py_VISIT(traverse_module_state->__pyx_n_s_Parser_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_Parser___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Parser___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Parser_match);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_Program);
@@ -4097,14 +4123,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_RUL);
   Py_VISIT(traverse_module_state->__pyx_n_s_Regex);
   Py_VISIT(traverse_module_state->__pyx_n_s_Regex___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Regex___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Rule);
   Py_VISIT(traverse_module_state->__pyx_n_s_SEQ);
   Py_VISIT(traverse_module_state->__pyx_n_s_STR);
+  Py_VISIT(traverse_module_state->__pyx_n_s_STRICT);
   Py_VISIT(traverse_module_state->__pyx_n_s_SYM);
   Py_VISIT(traverse_module_state->__pyx_n_s_Scanner);
   Py_VISIT(traverse_module_state->__pyx_n_s_Scanner___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Scanner___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Scanner_scan);
   Py_VISIT(traverse_module_state->__pyx_n_s_Tuple);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Tuple__Program__Index);
@@ -4481,14 +4508,15 @@
 #define __pyx_n_s_NOT __pyx_mstate_global->__pyx_n_s_NOT
 #define __pyx_n_s_NO_CAP_OR_ACT __pyx_mstate_global->__pyx_n_s_NO_CAP_OR_ACT
 #define __pyx_n_s_OPT __pyx_mstate_global->__pyx_n_s_OPT
 #define __pyx_n_s_Operator __pyx_mstate_global->__pyx_n_s_Operator
 #define __pyx_n_s_Optional __pyx_mstate_global->__pyx_n_s_Optional
 #define __pyx_kp_s_Optional_Definition __pyx_mstate_global->__pyx_kp_s_Optional_Definition
 #define __pyx_n_s_PLS __pyx_mstate_global->__pyx_n_s_PLS
+#define __pyx_n_s_ParseError __pyx_mstate_global->__pyx_n_s_ParseError
 #define __pyx_n_s_Parser __pyx_mstate_global->__pyx_n_s_Parser
 #define __pyx_n_s_Parser_2 __pyx_mstate_global->__pyx_n_s_Parser_2
 #define __pyx_n_s_Parser___reduce_cython __pyx_mstate_global->__pyx_n_s_Parser___reduce_cython
 #define __pyx_n_s_Parser___setstate_cython __pyx_mstate_global->__pyx_n_s_Parser___setstate_cython
 #define __pyx_n_s_Parser_match __pyx_mstate_global->__pyx_n_s_Parser_match
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
 #define __pyx_n_s_Program __pyx_mstate_global->__pyx_n_s_Program
@@ -4496,14 +4524,15 @@
 #define __pyx_n_s_RUL __pyx_mstate_global->__pyx_n_s_RUL
 #define __pyx_n_s_Regex __pyx_mstate_global->__pyx_n_s_Regex
 #define __pyx_n_s_Regex___reduce_cython __pyx_mstate_global->__pyx_n_s_Regex___reduce_cython
 #define __pyx_n_s_Regex___setstate_cython __pyx_mstate_global->__pyx_n_s_Regex___setstate_cython
 #define __pyx_n_s_Rule __pyx_mstate_global->__pyx_n_s_Rule
 #define __pyx_n_s_SEQ __pyx_mstate_global->__pyx_n_s_SEQ
 #define __pyx_n_s_STR __pyx_mstate_global->__pyx_n_s_STR
+#define __pyx_n_s_STRICT __pyx_mstate_global->__pyx_n_s_STRICT
 #define __pyx_n_s_SYM __pyx_mstate_global->__pyx_n_s_SYM
 #define __pyx_n_s_Scanner __pyx_mstate_global->__pyx_n_s_Scanner
 #define __pyx_n_s_Scanner___reduce_cython __pyx_mstate_global->__pyx_n_s_Scanner___reduce_cython
 #define __pyx_n_s_Scanner___setstate_cython __pyx_mstate_global->__pyx_n_s_Scanner___setstate_cython
 #define __pyx_n_s_Scanner_scan __pyx_mstate_global->__pyx_n_s_Scanner_scan
 #define __pyx_n_s_Tuple __pyx_mstate_global->__pyx_n_s_Tuple
 #define __pyx_kp_s_Tuple__Program__Index __pyx_mstate_global->__pyx_kp_s_Tuple__Program__Index
@@ -8387,15 +8416,15 @@
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   PyObject *__pyx_v_self = 0;
   PyObject *__pyx_v_s = 0;
   int __pyx_v_pos;
-  CYTHON_UNUSED PyObject *__pyx_v_flags = 0;
+  PyObject *__pyx_v_flags = 0;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED Py_ssize_t __pyx_nargs;
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues;
   PyObject* values[4] = {0,0,0,0};
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
@@ -8518,15 +8547,15 @@
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_6match(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_s, int __pyx_v_pos, CYTHON_UNUSED PyObject *__pyx_v_flags) {
+static PyObject *__pyx_pf_2pe_11_cy_machine_13MachineParser_6match(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self, PyObject *__pyx_v_s, int __pyx_v_pos, PyObject *__pyx_v_flags) {
   PyObject *__pyx_v_memo = NULL;
   PyObject *__pyx_v_args = 0;
   PyObject *__pyx_v_kwargs = 0;
   PyObject *__pyx_v_idx = NULL;
   PyObject *__pyx_v_end = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
@@ -8596,15 +8625,15 @@
   __pyx_t_3 = 0;
 
   /* "pe/_cy_machine.pyx":177
  *         kwargs: List[_Binding] = []
  *         idx = self._index[self.start]
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)             # <<<<<<<<<<<<<<
  *         if end < 0:
- *             return None
+ *             if flags & Flag.STRICT:
  */
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_parser); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
@@ -8635,88 +8664,151 @@
   __pyx_v_end = __pyx_t_3;
   __pyx_t_3 = 0;
 
   /* "pe/_cy_machine.pyx":178
  *         idx = self._index[self.start]
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
  *         if end < 0:             # <<<<<<<<<<<<<<
- *             return None
- *         else:
+ *             if flags & Flag.STRICT:
+ *                 raise ParseError()
  */
   __pyx_t_3 = PyObject_RichCompare(__pyx_v_end, __pyx_int_0, Py_LT); __Pyx_XGOTREF(__pyx_t_3); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 178, __pyx_L1_error)
   __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 178, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_6) {
 
     /* "pe/_cy_machine.pyx":179
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
  *         if end < 0:
+ *             if flags & Flag.STRICT:             # <<<<<<<<<<<<<<
+ *                 raise ParseError()
+ *             return None
+ */
+    __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_Flag); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_STRICT); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    __pyx_t_3 = PyNumber_And(__pyx_v_flags, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+    if (unlikely(__pyx_t_6)) {
+
+      /* "pe/_cy_machine.pyx":180
+ *         if end < 0:
+ *             if flags & Flag.STRICT:
+ *                 raise ParseError()             # <<<<<<<<<<<<<<
+ *             return None
+ *         else:
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_ParseError); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __pyx_t_2 = NULL;
+      __pyx_t_5 = 0;
+      #if CYTHON_UNPACK_METHODS
+      if (unlikely(PyMethod_Check(__pyx_t_1))) {
+        __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_1);
+        if (likely(__pyx_t_2)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_1);
+          __Pyx_INCREF(__pyx_t_2);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_1, function);
+          __pyx_t_5 = 1;
+        }
+      }
+      #endif
+      {
+        PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
+        __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
+        __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 180, __pyx_L1_error)
+        __Pyx_GOTREF(__pyx_t_3);
+        __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+      }
+      __Pyx_Raise(__pyx_t_3, 0, 0, 0);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __PYX_ERR(0, 180, __pyx_L1_error)
+
+      /* "pe/_cy_machine.pyx":179
+ *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
+ *         if end < 0:
+ *             if flags & Flag.STRICT:             # <<<<<<<<<<<<<<
+ *                 raise ParseError()
+ *             return None
+ */
+    }
+
+    /* "pe/_cy_machine.pyx":181
+ *             if flags & Flag.STRICT:
+ *                 raise ParseError()
  *             return None             # <<<<<<<<<<<<<<
  *         else:
  *             return Match(
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
     /* "pe/_cy_machine.pyx":178
  *         idx = self._index[self.start]
  *         end = self._parser.match(idx, s, pos, args, kwargs, memo)
  *         if end < 0:             # <<<<<<<<<<<<<<
- *             return None
- *         else:
+ *             if flags & Flag.STRICT:
+ *                 raise ParseError()
  */
   }
 
-  /* "pe/_cy_machine.pyx":181
+  /* "pe/_cy_machine.pyx":183
  *             return None
  *         else:
  *             return Match(             # <<<<<<<<<<<<<<
  *                 s,
  *                 pos,
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_Match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "pe/_cy_machine.pyx":183
+    /* "pe/_cy_machine.pyx":185
  *             return Match(
  *                 s,
  *                 pos,             # <<<<<<<<<<<<<<
  *                 end,
  *                 self.grammar[self.start],
  */
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
 
-    /* "pe/_cy_machine.pyx":185
+    /* "pe/_cy_machine.pyx":187
  *                 pos,
  *                 end,
  *                 self.grammar[self.start],             # <<<<<<<<<<<<<<
  *                 args,
  *                 dict(kwargs)
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_grammar); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_grammar); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_self, __pyx_n_s_start); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_t_4, __pyx_t_7); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 187, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":187
+    /* "pe/_cy_machine.pyx":189
  *                 self.grammar[self.start],
  *                 args,
  *                 dict(kwargs)             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_kwargs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_v_kwargs); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 189, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_1))) {
       __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_1);
       if (likely(__pyx_t_4)) {
@@ -8731,15 +8823,15 @@
     {
       PyObject *__pyx_callargs[7] = {__pyx_t_4, __pyx_v_s, __pyx_t_2, __pyx_v_end, __pyx_t_8, __pyx_v_args, __pyx_t_7};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_1, __pyx_callargs+1-__pyx_t_5, 6+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 181, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 183, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     }
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
@@ -8769,15 +8861,15 @@
   __Pyx_XDECREF(__pyx_v_idx);
   __Pyx_XDECREF(__pyx_v_end);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":194
+/* "pe/_cy_machine.pyx":196
  *     cdef list pi
  * 
  *     def __init__(self, list pi):             # <<<<<<<<<<<<<<
  *         self.pi = pi
  * 
  */
 
@@ -8813,45 +8905,45 @@
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pi)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 194, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 196, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 194, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 196, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_pi = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 194, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 196, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pe._cy_machine._Parser.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pi), (&PyList_Type), 1, "pi", 1))) __PYX_ERR(0, 194, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pi), (&PyList_Type), 1, "pi", 1))) __PYX_ERR(0, 196, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_7_Parser___init__(((struct __pyx_obj_2pe_11_cy_machine__Parser *)__pyx_v_self), __pyx_v_pi);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -8866,42 +8958,42 @@
 }
 
 static int __pyx_pf_2pe_11_cy_machine_7_Parser___init__(struct __pyx_obj_2pe_11_cy_machine__Parser *__pyx_v_self, PyObject *__pyx_v_pi) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "pe/_cy_machine.pyx":195
+  /* "pe/_cy_machine.pyx":197
  * 
  *     def __init__(self, list pi):
  *         self.pi = pi             # <<<<<<<<<<<<<<
  * 
  *     cpdef int match(
  */
   __Pyx_INCREF(__pyx_v_pi);
   __Pyx_GIVEREF(__pyx_v_pi);
   __Pyx_GOTREF(__pyx_v_self->pi);
   __Pyx_DECREF(__pyx_v_self->pi);
   __pyx_v_self->pi = __pyx_v_pi;
 
-  /* "pe/_cy_machine.pyx":194
+  /* "pe/_cy_machine.pyx":196
  *     cdef list pi
  * 
  *     def __init__(self, list pi):             # <<<<<<<<<<<<<<
  *         self.pi = pi
  * 
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":197
+/* "pe/_cy_machine.pyx":199
  *         self.pi = pi
  * 
  *     cpdef int match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
 
@@ -8943,20 +9035,20 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       if (!__Pyx_IsSameCFunction(__pyx_t_1, (void*) __pyx_pw_2pe_11_cy_machine_7_Parser_3match)) {
-        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_3 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 199, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_3);
-        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_INCREF(__pyx_t_1);
         __pyx_t_5 = __pyx_t_1; __pyx_t_6 = NULL;
         __pyx_t_7 = 0;
         #if CYTHON_UNPACK_METHODS
         if (unlikely(PyMethod_Check(__pyx_t_5))) {
           __pyx_t_6 = PyMethod_GET_SELF(__pyx_t_5);
@@ -8971,19 +9063,19 @@
         #endif
         {
           PyObject *__pyx_callargs[7] = {__pyx_t_6, __pyx_t_3, __pyx_v_s, __pyx_t_4, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo};
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 6+__pyx_t_7);
           __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
           __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
         }
-        __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L1_error)
+        __pyx_t_7 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_7 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_r = __pyx_t_7;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
       __pyx_tp_dict_version = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
@@ -8994,94 +9086,94 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "pe/_cy_machine.pyx":207
+  /* "pe/_cy_machine.pyx":209
  *     ) except -2:
  *         cdef State* state
  *         cdef int retval = -1             # <<<<<<<<<<<<<<
  *         state = push(0, 0, -1, 0, 0, NULL)     # failure (top backtrack entry)
  *         state = push(-1, -1, -1, 0, 0, state)  # success
  */
   __pyx_v_retval = -1;
 
-  /* "pe/_cy_machine.pyx":208
+  /* "pe/_cy_machine.pyx":210
  *         cdef State* state
  *         cdef int retval = -1
  *         state = push(0, 0, -1, 0, 0, NULL)     # failure (top backtrack entry)             # <<<<<<<<<<<<<<
  *         state = push(-1, -1, -1, 0, 0, state)  # success
  *         try:
  */
-  __pyx_t_8 = __pyx_f_2pe_11_cy_machine_push(0, 0, -1, 0, 0, NULL); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 208, __pyx_L1_error)
+  __pyx_t_8 = __pyx_f_2pe_11_cy_machine_push(0, 0, -1, 0, 0, NULL); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 210, __pyx_L1_error)
   __pyx_v_state = __pyx_t_8;
 
-  /* "pe/_cy_machine.pyx":209
+  /* "pe/_cy_machine.pyx":211
  *         cdef int retval = -1
  *         state = push(0, 0, -1, 0, 0, NULL)     # failure (top backtrack entry)
  *         state = push(-1, -1, -1, 0, 0, state)  # success             # <<<<<<<<<<<<<<
  *         try:
  *             state = self._match(idx, s, pos, args, kwargs, memo, state)
  */
-  __pyx_t_8 = __pyx_f_2pe_11_cy_machine_push(-1, -1, -1, 0, 0, __pyx_v_state); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 209, __pyx_L1_error)
+  __pyx_t_8 = __pyx_f_2pe_11_cy_machine_push(-1, -1, -1, 0, 0, __pyx_v_state); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 211, __pyx_L1_error)
   __pyx_v_state = __pyx_t_8;
 
-  /* "pe/_cy_machine.pyx":210
+  /* "pe/_cy_machine.pyx":212
  *         state = push(0, 0, -1, 0, 0, NULL)     # failure (top backtrack entry)
  *         state = push(-1, -1, -1, 0, 0, state)  # success
  *         try:             # <<<<<<<<<<<<<<
  *             state = self._match(idx, s, pos, args, kwargs, memo, state)
  *             retval = state.pos
  */
   /*try:*/ {
 
-    /* "pe/_cy_machine.pyx":211
+    /* "pe/_cy_machine.pyx":213
  *         state = push(-1, -1, -1, 0, 0, state)  # success
  *         try:
  *             state = self._match(idx, s, pos, args, kwargs, memo, state)             # <<<<<<<<<<<<<<
  *             retval = state.pos
  *         finally:
  */
-    __pyx_t_8 = ((struct __pyx_vtabstruct_2pe_11_cy_machine__Parser *)__pyx_v_self->__pyx_vtab)->_match(__pyx_v_self, __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo, __pyx_v_state); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 211, __pyx_L4_error)
+    __pyx_t_8 = ((struct __pyx_vtabstruct_2pe_11_cy_machine__Parser *)__pyx_v_self->__pyx_vtab)->_match(__pyx_v_self, __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo, __pyx_v_state); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 213, __pyx_L4_error)
     __pyx_v_state = __pyx_t_8;
 
-    /* "pe/_cy_machine.pyx":212
+    /* "pe/_cy_machine.pyx":214
  *         try:
  *             state = self._match(idx, s, pos, args, kwargs, memo, state)
  *             retval = state.pos             # <<<<<<<<<<<<<<
  *         finally:
  *             while state:
  */
     __pyx_t_7 = __pyx_v_state->pos;
     __pyx_v_retval = __pyx_t_7;
   }
 
-  /* "pe/_cy_machine.pyx":214
+  /* "pe/_cy_machine.pyx":216
  *             retval = state.pos
  *         finally:
  *             while state:             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *         return retval
  */
   /*finally:*/ {
     /*normal exit:*/{
       while (1) {
         __pyx_t_9 = (__pyx_v_state != 0);
         if (!__pyx_t_9) break;
 
-        /* "pe/_cy_machine.pyx":215
+        /* "pe/_cy_machine.pyx":217
  *         finally:
  *             while state:
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *         return retval
  * 
  */
-        __pyx_t_8 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 215, __pyx_L1_error)
+        __pyx_t_8 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 217, __pyx_L1_error)
         __pyx_v_state = __pyx_t_8;
       }
       goto __pyx_L5;
     }
     __pyx_L4_error:;
     /*exception exit:*/{
       __Pyx_PyThreadState_declare
@@ -9100,33 +9192,33 @@
       __Pyx_XGOTREF(__pyx_t_14);
       __Pyx_XGOTREF(__pyx_t_15);
       __Pyx_XGOTREF(__pyx_t_16);
       __Pyx_XGOTREF(__pyx_t_17);
       __pyx_t_7 = __pyx_lineno; __pyx_t_10 = __pyx_clineno; __pyx_t_11 = __pyx_filename;
       {
 
-        /* "pe/_cy_machine.pyx":214
+        /* "pe/_cy_machine.pyx":216
  *             retval = state.pos
  *         finally:
  *             while state:             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *         return retval
  */
         while (1) {
           __pyx_t_9 = (__pyx_v_state != 0);
           if (!__pyx_t_9) break;
 
-          /* "pe/_cy_machine.pyx":215
+          /* "pe/_cy_machine.pyx":217
  *         finally:
  *             while state:
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *         return retval
  * 
  */
-          __pyx_t_8 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 215, __pyx_L9_error)
+          __pyx_t_8 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_8 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 217, __pyx_L9_error)
           __pyx_v_state = __pyx_t_8;
         }
       }
       if (PY_MAJOR_VERSION >= 3) {
         __Pyx_XGIVEREF(__pyx_t_15);
         __Pyx_XGIVEREF(__pyx_t_16);
         __Pyx_XGIVEREF(__pyx_t_17);
@@ -9151,25 +9243,25 @@
       __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
       __pyx_t_15 = 0; __pyx_t_16 = 0; __pyx_t_17 = 0;
       goto __pyx_L1_error;
     }
     __pyx_L5:;
   }
 
-  /* "pe/_cy_machine.pyx":216
+  /* "pe/_cy_machine.pyx":218
  *             while state:
  *                 state = pop(state)
  *         return retval             # <<<<<<<<<<<<<<
  * 
  *     cdef State* _match(
  */
   __pyx_r = __pyx_v_retval;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":197
+  /* "pe/_cy_machine.pyx":199
  *         self.pi = pi
  * 
  *     cpdef int match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
 
@@ -9252,108 +9344,108 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_idx)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_s)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 1); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 1); __PYX_ERR(0, 199, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pos)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[2]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 2); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 2); __PYX_ERR(0, 199, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_args)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[3]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 3); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 3); __PYX_ERR(0, 199, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  4:
         if (likely((values[4] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_kwargs)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[4]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 4); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 4); __PYX_ERR(0, 199, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  5:
         if (likely((values[5] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_memo)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[5]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 197, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 5); __PYX_ERR(0, 197, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, 5); __PYX_ERR(0, 199, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "match") < 0)) __PYX_ERR(0, 197, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "match") < 0)) __PYX_ERR(0, 199, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 6)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
       values[4] = __Pyx_Arg_FASTCALL(__pyx_args, 4);
       values[5] = __Pyx_Arg_FASTCALL(__pyx_args, 5);
     }
-    __pyx_v_idx = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_idx == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 199, __pyx_L3_error)
+    __pyx_v_idx = __Pyx_PyInt_As_int(values[0]); if (unlikely((__pyx_v_idx == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
     __pyx_v_s = ((PyObject*)values[1]);
-    __pyx_v_pos = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 201, __pyx_L3_error)
+    __pyx_v_pos = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_pos == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 203, __pyx_L3_error)
     __pyx_v_args = ((PyObject*)values[3]);
     __pyx_v_kwargs = ((PyObject*)values[4]);
     __pyx_v_memo = ((PyObject*)values[5]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, __pyx_nargs); __PYX_ERR(0, 197, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("match", 1, 6, 6, __pyx_nargs); __PYX_ERR(0, 199, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pe._cy_machine._Parser.match", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyUnicode_Type), 1, "s", 1))) __PYX_ERR(0, 200, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyList_Type), 1, "args", 1))) __PYX_ERR(0, 202, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyList_Type), 1, "kwargs", 1))) __PYX_ERR(0, 203, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_memo), (&PyDict_Type), 1, "memo", 1))) __PYX_ERR(0, 204, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_s), (&PyUnicode_Type), 1, "s", 1))) __PYX_ERR(0, 202, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_args), (&PyList_Type), 1, "args", 1))) __PYX_ERR(0, 204, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_kwargs), (&PyList_Type), 1, "kwargs", 1))) __PYX_ERR(0, 205, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_memo), (&PyDict_Type), 1, "memo", 1))) __PYX_ERR(0, 206, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_7_Parser_2match(((struct __pyx_obj_2pe_11_cy_machine__Parser *)__pyx_v_self), __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -9373,16 +9465,16 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("match", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __pyx_f_2pe_11_cy_machine_7_Parser_match(__pyx_v_self, __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo, 1); if (unlikely(__pyx_t_1 == ((int)-2))) __PYX_ERR(0, 197, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_2pe_11_cy_machine_7_Parser_match(__pyx_v_self, __pyx_v_idx, __pyx_v_s, __pyx_v_pos, __pyx_v_args, __pyx_v_kwargs, __pyx_v_memo, 1); if (unlikely(__pyx_t_1 == ((int)-2))) __PYX_ERR(0, 199, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -9391,15 +9483,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":218
+/* "pe/_cy_machine.pyx":220
  *         return retval
  * 
  *     cdef State* _match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
 
@@ -9427,722 +9519,722 @@
   PyObject *__pyx_t_14 = NULL;
   PyObject *(*__pyx_t_15)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_match", 1);
 
-  /* "pe/_cy_machine.pyx":228
+  /* "pe/_cy_machine.pyx":230
  *         State* state,
  *     ) except NULL:
  *         if s is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         if args is None:
  */
   __pyx_t_1 = (__pyx_v_s == ((PyObject*)Py_None));
   if (unlikely(__pyx_t_1)) {
 
-    /* "pe/_cy_machine.pyx":229
+    /* "pe/_cy_machine.pyx":231
  *     ) except NULL:
  *         if s is None:
  *             raise TypeError             # <<<<<<<<<<<<<<
  *         if args is None:
  *             raise TypeError
  */
     __Pyx_Raise(__pyx_builtin_TypeError, 0, 0, 0);
-    __PYX_ERR(0, 229, __pyx_L1_error)
+    __PYX_ERR(0, 231, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":228
+    /* "pe/_cy_machine.pyx":230
  *         State* state,
  *     ) except NULL:
  *         if s is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         if args is None:
  */
   }
 
-  /* "pe/_cy_machine.pyx":230
+  /* "pe/_cy_machine.pyx":232
  *         if s is None:
  *             raise TypeError
  *         if args is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         if kwargs is None:
  */
   __pyx_t_1 = (__pyx_v_args == ((PyObject*)Py_None));
   if (unlikely(__pyx_t_1)) {
 
-    /* "pe/_cy_machine.pyx":231
+    /* "pe/_cy_machine.pyx":233
  *             raise TypeError
  *         if args is None:
  *             raise TypeError             # <<<<<<<<<<<<<<
  *         if kwargs is None:
  *             raise TypeError
  */
     __Pyx_Raise(__pyx_builtin_TypeError, 0, 0, 0);
-    __PYX_ERR(0, 231, __pyx_L1_error)
+    __PYX_ERR(0, 233, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":230
+    /* "pe/_cy_machine.pyx":232
  *         if s is None:
  *             raise TypeError
  *         if args is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         if kwargs is None:
  */
   }
 
-  /* "pe/_cy_machine.pyx":232
+  /* "pe/_cy_machine.pyx":234
  *         if args is None:
  *             raise TypeError
  *         if kwargs is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         # lookup optimizations
  */
   __pyx_t_1 = (__pyx_v_kwargs == ((PyObject*)Py_None));
   if (unlikely(__pyx_t_1)) {
 
-    /* "pe/_cy_machine.pyx":233
+    /* "pe/_cy_machine.pyx":235
  *             raise TypeError
  *         if kwargs is None:
  *             raise TypeError             # <<<<<<<<<<<<<<
  *         # lookup optimizations
  *         pi = self.pi
  */
     __Pyx_Raise(__pyx_builtin_TypeError, 0, 0, 0);
-    __PYX_ERR(0, 233, __pyx_L1_error)
+    __PYX_ERR(0, 235, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":232
+    /* "pe/_cy_machine.pyx":234
  *         if args is None:
  *             raise TypeError
  *         if kwargs is None:             # <<<<<<<<<<<<<<
  *             raise TypeError
  *         # lookup optimizations
  */
   }
 
-  /* "pe/_cy_machine.pyx":235
+  /* "pe/_cy_machine.pyx":237
  *             raise TypeError
  *         # lookup optimizations
  *         pi = self.pi             # <<<<<<<<<<<<<<
  *         # cdef OpCode opcode
  *         cdef int slen = len(s)
  */
   __pyx_t_2 = __pyx_v_self->pi;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_pi = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":237
+  /* "pe/_cy_machine.pyx":239
  *         pi = self.pi
  *         # cdef OpCode opcode
  *         cdef int slen = len(s)             # <<<<<<<<<<<<<<
  *         cdef Instruction instr
  *         while state:
  */
   if (unlikely(__pyx_v_s == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 237, __pyx_L1_error)
+    __PYX_ERR(0, 239, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_s); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 237, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_s); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 239, __pyx_L1_error)
   __pyx_v_slen = __pyx_t_3;
 
-  /* "pe/_cy_machine.pyx":239
+  /* "pe/_cy_machine.pyx":241
  *         cdef int slen = len(s)
  *         cdef Instruction instr
  *         while state:             # <<<<<<<<<<<<<<
  *             instr = pi[idx]
  * 
  */
   while (1) {
     __pyx_t_1 = (__pyx_v_state != 0);
     if (!__pyx_t_1) break;
 
-    /* "pe/_cy_machine.pyx":240
+    /* "pe/_cy_machine.pyx":242
  *         cdef Instruction instr
  *         while state:
  *             instr = pi[idx]             # <<<<<<<<<<<<<<
  * 
  *             if instr.marking:
  */
     if (unlikely(__pyx_v_pi == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-      __PYX_ERR(0, 240, __pyx_L1_error)
+      __PYX_ERR(0, 242, __pyx_L1_error)
     }
-    __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_pi, __pyx_v_idx, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 240, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt_List(__pyx_v_pi, __pyx_v_idx, int, 1, __Pyx_PyInt_From_int, 1, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2pe_11_cy_machine_Instruction))))) __PYX_ERR(0, 240, __pyx_L1_error)
+    if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_2pe_11_cy_machine_Instruction))))) __PYX_ERR(0, 242, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_instr, ((struct __pyx_obj_2pe_11_cy_machine_Instruction *)__pyx_t_2));
     __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":242
+    /* "pe/_cy_machine.pyx":244
  *             instr = pi[idx]
  * 
  *             if instr.marking:             # <<<<<<<<<<<<<<
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)
  * 
  */
     if (__pyx_v_instr->marking) {
 
-      /* "pe/_cy_machine.pyx":243
+      /* "pe/_cy_machine.pyx":245
  * 
  *             if instr.marking:
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)             # <<<<<<<<<<<<<<
  * 
  *             if instr.opcode == SCAN:
  */
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 243, __pyx_L1_error)
+        __PYX_ERR(0, 245, __pyx_L1_error)
       }
-      __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 243, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 245, __pyx_L1_error)
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 243, __pyx_L1_error)
+        __PYX_ERR(0, 245, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 243, __pyx_L1_error)
-      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_push(0, -1, __pyx_v_pos, __pyx_t_3, __pyx_t_4, __pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 243, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 245, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_push(0, -1, __pyx_v_pos, __pyx_t_3, __pyx_t_4, __pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 245, __pyx_L1_error)
       __pyx_v_state = __pyx_t_5;
 
-      /* "pe/_cy_machine.pyx":242
+      /* "pe/_cy_machine.pyx":244
  *             instr = pi[idx]
  * 
  *             if instr.marking:             # <<<<<<<<<<<<<<
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)
  * 
  */
     }
 
-    /* "pe/_cy_machine.pyx":245
+    /* "pe/_cy_machine.pyx":247
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)
  * 
  *             if instr.opcode == SCAN:             # <<<<<<<<<<<<<<
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_SCAN);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":246
+      /* "pe/_cy_machine.pyx":248
  * 
  *             if instr.opcode == SCAN:
  *                 pos = instr.scanner._scan(s, pos, slen)             # <<<<<<<<<<<<<<
  *                 if pos < 0:
  *                     idx = FAILURE
  */
-      __pyx_t_6 = ((struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *)__pyx_v_instr->scanner->__pyx_vtab)->_scan(__pyx_v_instr->scanner, __pyx_v_s, __pyx_v_pos, __pyx_v_slen); if (unlikely(__pyx_t_6 == ((int)-2))) __PYX_ERR(0, 246, __pyx_L1_error)
+      __pyx_t_6 = ((struct __pyx_vtabstruct_2pe_11_cy_machine_Scanner *)__pyx_v_instr->scanner->__pyx_vtab)->_scan(__pyx_v_instr->scanner, __pyx_v_s, __pyx_v_pos, __pyx_v_slen); if (unlikely(__pyx_t_6 == ((int)-2))) __PYX_ERR(0, 248, __pyx_L1_error)
       __pyx_v_pos = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":247
+      /* "pe/_cy_machine.pyx":249
  *             if instr.opcode == SCAN:
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:             # <<<<<<<<<<<<<<
  *                     idx = FAILURE
  * 
  */
       __pyx_t_1 = (__pyx_v_pos < 0);
       if (__pyx_t_1) {
 
-        /* "pe/_cy_machine.pyx":248
+        /* "pe/_cy_machine.pyx":250
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:
  *                     idx = FAILURE             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == BRANCH:
  */
-        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 248, __pyx_L1_error)
+        __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
-        __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 248, __pyx_L1_error)
+        __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 250, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __pyx_v_idx = __pyx_t_6;
 
-        /* "pe/_cy_machine.pyx":247
+        /* "pe/_cy_machine.pyx":249
  *             if instr.opcode == SCAN:
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:             # <<<<<<<<<<<<<<
  *                     idx = FAILURE
  * 
  */
       }
 
-      /* "pe/_cy_machine.pyx":245
+      /* "pe/_cy_machine.pyx":247
  *                 state = push(0, -1, pos, len(args), len(kwargs), state)
  * 
  *             if instr.opcode == SCAN:             # <<<<<<<<<<<<<<
  *                 pos = instr.scanner._scan(s, pos, slen)
  *                 if pos < 0:
  */
       goto __pyx_L9;
     }
 
-    /* "pe/_cy_machine.pyx":250
+    /* "pe/_cy_machine.pyx":252
  *                     idx = FAILURE
  * 
  *             elif instr.opcode == BRANCH:             # <<<<<<<<<<<<<<
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)
  *                 idx += 1
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_BRANCH);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":251
+      /* "pe/_cy_machine.pyx":253
  * 
  *             elif instr.opcode == BRANCH:
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)             # <<<<<<<<<<<<<<
  *                 idx += 1
  *                 continue
  */
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 251, __pyx_L1_error)
+        __PYX_ERR(0, 253, __pyx_L1_error)
       }
-      __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 251, __pyx_L1_error)
+      __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(0, 253, __pyx_L1_error)
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 251, __pyx_L1_error)
+        __PYX_ERR(0, 253, __pyx_L1_error)
       }
-      __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 251, __pyx_L1_error)
-      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_push((__pyx_v_idx + __pyx_v_instr->oploc), __pyx_v_pos, -1, __pyx_t_4, __pyx_t_3, __pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 251, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 253, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_push((__pyx_v_idx + __pyx_v_instr->oploc), __pyx_v_pos, -1, __pyx_t_4, __pyx_t_3, __pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 253, __pyx_L1_error)
       __pyx_v_state = __pyx_t_5;
 
-      /* "pe/_cy_machine.pyx":252
+      /* "pe/_cy_machine.pyx":254
  *             elif instr.opcode == BRANCH:
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)
  *                 idx += 1             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + 1);
 
-      /* "pe/_cy_machine.pyx":253
+      /* "pe/_cy_machine.pyx":255
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)
  *                 idx += 1
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == CALL:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":250
+      /* "pe/_cy_machine.pyx":252
  *                     idx = FAILURE
  * 
  *             elif instr.opcode == BRANCH:             # <<<<<<<<<<<<<<
  *                 state = push(idx + instr.oploc, pos, -1, len(args), len(kwargs), state)
  *                 idx += 1
  */
     }
 
-    /* "pe/_cy_machine.pyx":255
+    /* "pe/_cy_machine.pyx":257
  *                 continue
  * 
  *             elif instr.opcode == CALL:             # <<<<<<<<<<<<<<
  *                 state = push(idx + 1, -1, -1, -1, -1, state)
  *                 idx = instr.oploc
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_CALL);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":256
+      /* "pe/_cy_machine.pyx":258
  * 
  *             elif instr.opcode == CALL:
  *                 state = push(idx + 1, -1, -1, -1, -1, state)             # <<<<<<<<<<<<<<
  *                 idx = instr.oploc
  *                 continue
  */
-      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_push((__pyx_v_idx + 1), -1, -1, -1, -1, __pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 256, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_push((__pyx_v_idx + 1), -1, -1, -1, -1, __pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 258, __pyx_L1_error)
       __pyx_v_state = __pyx_t_5;
 
-      /* "pe/_cy_machine.pyx":257
+      /* "pe/_cy_machine.pyx":259
  *             elif instr.opcode == CALL:
  *                 state = push(idx + 1, -1, -1, -1, -1, state)
  *                 idx = instr.oploc             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_t_7 = __pyx_v_instr->oploc;
       __pyx_v_idx = __pyx_t_7;
 
-      /* "pe/_cy_machine.pyx":258
+      /* "pe/_cy_machine.pyx":260
  *                 state = push(idx + 1, -1, -1, -1, -1, state)
  *                 idx = instr.oploc
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == COMMIT:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":255
+      /* "pe/_cy_machine.pyx":257
  *                 continue
  * 
  *             elif instr.opcode == CALL:             # <<<<<<<<<<<<<<
  *                 state = push(idx + 1, -1, -1, -1, -1, state)
  *                 idx = instr.oploc
  */
     }
 
-    /* "pe/_cy_machine.pyx":260
+    /* "pe/_cy_machine.pyx":262
  *                 continue
  * 
  *             elif instr.opcode == COMMIT:             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 idx += instr.oploc
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_COMMIT);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":261
+      /* "pe/_cy_machine.pyx":263
  * 
  *             elif instr.opcode == COMMIT:
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *                 idx += instr.oploc
  *                 continue
  */
-      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 261, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 263, __pyx_L1_error)
       __pyx_v_state = __pyx_t_5;
 
-      /* "pe/_cy_machine.pyx":262
+      /* "pe/_cy_machine.pyx":264
  *             elif instr.opcode == COMMIT:
  *                 state = pop(state)
  *                 idx += instr.oploc             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + __pyx_v_instr->oploc);
 
-      /* "pe/_cy_machine.pyx":263
+      /* "pe/_cy_machine.pyx":265
  *                 state = pop(state)
  *                 idx += instr.oploc
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == UPDATE:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":260
+      /* "pe/_cy_machine.pyx":262
  *                 continue
  * 
  *             elif instr.opcode == COMMIT:             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 idx += instr.oploc
  */
     }
 
-    /* "pe/_cy_machine.pyx":265
+    /* "pe/_cy_machine.pyx":267
  *                 continue
  * 
  *             elif instr.opcode == UPDATE:             # <<<<<<<<<<<<<<
  *                 state.pos = pos
  *                 state.argidx = len(args)
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_UPDATE);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":266
+      /* "pe/_cy_machine.pyx":268
  * 
  *             elif instr.opcode == UPDATE:
  *                 state.pos = pos             # <<<<<<<<<<<<<<
  *                 state.argidx = len(args)
  *                 state.kwidx = len(kwargs)
  */
       __pyx_v_state->pos = __pyx_v_pos;
 
-      /* "pe/_cy_machine.pyx":267
+      /* "pe/_cy_machine.pyx":269
  *             elif instr.opcode == UPDATE:
  *                 state.pos = pos
  *                 state.argidx = len(args)             # <<<<<<<<<<<<<<
  *                 state.kwidx = len(kwargs)
  *                 idx += instr.oploc
  */
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 267, __pyx_L1_error)
+        __PYX_ERR(0, 269, __pyx_L1_error)
       }
-      __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 267, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_args); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 269, __pyx_L1_error)
       __pyx_v_state->argidx = __pyx_t_3;
 
-      /* "pe/_cy_machine.pyx":268
+      /* "pe/_cy_machine.pyx":270
  *                 state.pos = pos
  *                 state.argidx = len(args)
  *                 state.kwidx = len(kwargs)             # <<<<<<<<<<<<<<
  *                 idx += instr.oploc
  *                 continue
  */
       if (unlikely(__pyx_v_kwargs == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-        __PYX_ERR(0, 268, __pyx_L1_error)
+        __PYX_ERR(0, 270, __pyx_L1_error)
       }
-      __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 268, __pyx_L1_error)
+      __pyx_t_3 = __Pyx_PyList_GET_SIZE(__pyx_v_kwargs); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 270, __pyx_L1_error)
       __pyx_v_state->kwidx = __pyx_t_3;
 
-      /* "pe/_cy_machine.pyx":269
+      /* "pe/_cy_machine.pyx":271
  *                 state.argidx = len(args)
  *                 state.kwidx = len(kwargs)
  *                 idx += instr.oploc             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + __pyx_v_instr->oploc);
 
-      /* "pe/_cy_machine.pyx":270
+      /* "pe/_cy_machine.pyx":272
  *                 state.kwidx = len(kwargs)
  *                 idx += instr.oploc
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == RESTORE:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":265
+      /* "pe/_cy_machine.pyx":267
  *                 continue
  * 
  *             elif instr.opcode == UPDATE:             # <<<<<<<<<<<<<<
  *                 state.pos = pos
  *                 state.argidx = len(args)
  */
     }
 
-    /* "pe/_cy_machine.pyx":272
+    /* "pe/_cy_machine.pyx":274
  *                 continue
  * 
  *             elif instr.opcode == RESTORE:             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 state = pop(state)
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_RESTORE);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":273
+      /* "pe/_cy_machine.pyx":275
  * 
  *             elif instr.opcode == RESTORE:
  *                 pos = state.pos             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 idx += instr.oploc
  */
       __pyx_t_6 = __pyx_v_state->pos;
       __pyx_v_pos = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":274
+      /* "pe/_cy_machine.pyx":276
  *             elif instr.opcode == RESTORE:
  *                 pos = state.pos
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *                 idx += instr.oploc
  *                 continue
  */
-      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 274, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 276, __pyx_L1_error)
       __pyx_v_state = __pyx_t_5;
 
-      /* "pe/_cy_machine.pyx":275
+      /* "pe/_cy_machine.pyx":277
  *                 pos = state.pos
  *                 state = pop(state)
  *                 idx += instr.oploc             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
       __pyx_v_idx = (__pyx_v_idx + __pyx_v_instr->oploc);
 
-      /* "pe/_cy_machine.pyx":276
+      /* "pe/_cy_machine.pyx":278
  *                 state = pop(state)
  *                 idx += instr.oploc
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == FAILTWICE:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":272
+      /* "pe/_cy_machine.pyx":274
  *                 continue
  * 
  *             elif instr.opcode == RESTORE:             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 state = pop(state)
  */
     }
 
-    /* "pe/_cy_machine.pyx":278
+    /* "pe/_cy_machine.pyx":280
  *                 continue
  * 
  *             elif instr.opcode == FAILTWICE:             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 state = pop(state)
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_FAILTWICE);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":279
+      /* "pe/_cy_machine.pyx":281
  * 
  *             elif instr.opcode == FAILTWICE:
  *                 pos = state.pos             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 idx = FAILURE
  */
       __pyx_t_6 = __pyx_v_state->pos;
       __pyx_v_pos = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":280
+      /* "pe/_cy_machine.pyx":282
  *             elif instr.opcode == FAILTWICE:
  *                 pos = state.pos
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *                 idx = FAILURE
  * 
  */
-      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 280, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 282, __pyx_L1_error)
       __pyx_v_state = __pyx_t_5;
 
-      /* "pe/_cy_machine.pyx":281
+      /* "pe/_cy_machine.pyx":283
  *                 pos = state.pos
  *                 state = pop(state)
  *                 idx = FAILURE             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == RETURN:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 281, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 283, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 281, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 283, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_v_idx = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":278
+      /* "pe/_cy_machine.pyx":280
  *                 continue
  * 
  *             elif instr.opcode == FAILTWICE:             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 state = pop(state)
  */
       goto __pyx_L9;
     }
 
-    /* "pe/_cy_machine.pyx":283
+    /* "pe/_cy_machine.pyx":285
  *                 idx = FAILURE
  * 
  *             elif instr.opcode == RETURN:             # <<<<<<<<<<<<<<
  *                 idx = state.opidx
  *                 state = pop(state)
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_RETURN);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":284
+      /* "pe/_cy_machine.pyx":286
  * 
  *             elif instr.opcode == RETURN:
  *                 idx = state.opidx             # <<<<<<<<<<<<<<
  *                 state = pop(state)
  *                 continue
  */
       __pyx_t_6 = __pyx_v_state->opidx;
       __pyx_v_idx = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":285
+      /* "pe/_cy_machine.pyx":287
  *             elif instr.opcode == RETURN:
  *                 idx = state.opidx
  *                 state = pop(state)             # <<<<<<<<<<<<<<
  *                 continue
  * 
  */
-      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 285, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 287, __pyx_L1_error)
       __pyx_v_state = __pyx_t_5;
 
-      /* "pe/_cy_machine.pyx":286
+      /* "pe/_cy_machine.pyx":288
  *                 idx = state.opidx
  *                 state = pop(state)
  *                 continue             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == PASS:
  */
       goto __pyx_L6_continue;
 
-      /* "pe/_cy_machine.pyx":283
+      /* "pe/_cy_machine.pyx":285
  *                 idx = FAILURE
  * 
  *             elif instr.opcode == RETURN:             # <<<<<<<<<<<<<<
  *                 idx = state.opidx
  *                 state = pop(state)
  */
     }
 
-    /* "pe/_cy_machine.pyx":288
+    /* "pe/_cy_machine.pyx":290
  *                 continue
  * 
  *             elif instr.opcode == PASS:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_PASS);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":289
+      /* "pe/_cy_machine.pyx":291
  * 
  *             elif instr.opcode == PASS:
  *                 break             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode == FAIL:
  */
       goto __pyx_L7_break;
 
-      /* "pe/_cy_machine.pyx":288
+      /* "pe/_cy_machine.pyx":290
  *                 continue
  * 
  *             elif instr.opcode == PASS:             # <<<<<<<<<<<<<<
  *                 break
  * 
  */
     }
 
-    /* "pe/_cy_machine.pyx":291
+    /* "pe/_cy_machine.pyx":293
  *                 break
  * 
  *             elif instr.opcode == FAIL:             # <<<<<<<<<<<<<<
  *                 idx = FAILURE
  * 
  */
     __pyx_t_1 = (__pyx_v_instr->opcode == __pyx_e_2pe_11_cy_machine_FAIL);
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":292
+      /* "pe/_cy_machine.pyx":294
  * 
  *             elif instr.opcode == FAIL:
  *                 idx = FAILURE             # <<<<<<<<<<<<<<
  * 
  *             elif instr.opcode != NOOP:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 292, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 294, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 292, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 294, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       __pyx_v_idx = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":291
+      /* "pe/_cy_machine.pyx":293
  *                 break
  * 
  *             elif instr.opcode == FAIL:             # <<<<<<<<<<<<<<
  *                 idx = FAILURE
  * 
  */
       goto __pyx_L9;
     }
 
-    /* "pe/_cy_machine.pyx":294
+    /* "pe/_cy_machine.pyx":296
  *                 idx = FAILURE
  * 
  *             elif instr.opcode != NOOP:             # <<<<<<<<<<<<<<
  *                 raise Error(f'invalid operation: {instr.opcode}')
  * 
  */
     __pyx_t_1 = (__pyx_v_instr->opcode != __pyx_e_2pe_11_cy_machine_NOOP);
     if (unlikely(__pyx_t_1)) {
 
-      /* "pe/_cy_machine.pyx":295
+      /* "pe/_cy_machine.pyx":297
  * 
  *             elif instr.opcode != NOOP:
  *                 raise Error(f'invalid operation: {instr.opcode}')             # <<<<<<<<<<<<<<
  * 
  *             if idx == FAILURE:
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Error); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Error); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 297, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_9 = __Pyx_PyUnicode_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_v_instr->opcode, 0, ' ', 'd'); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_9 = __Pyx_PyUnicode_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_v_instr->opcode, 0, ' ', 'd'); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 297, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_operation, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 295, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_operation, __pyx_t_9); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 297, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       __pyx_t_9 = NULL;
       __pyx_t_6 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
@@ -10156,51 +10248,51 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_10};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_6, 1+__pyx_t_6);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 295, __pyx_L1_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
       __Pyx_Raise(__pyx_t_2, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __PYX_ERR(0, 295, __pyx_L1_error)
+      __PYX_ERR(0, 297, __pyx_L1_error)
 
-      /* "pe/_cy_machine.pyx":294
+      /* "pe/_cy_machine.pyx":296
  *                 idx = FAILURE
  * 
  *             elif instr.opcode != NOOP:             # <<<<<<<<<<<<<<
  *                 raise Error(f'invalid operation: {instr.opcode}')
  * 
  */
     }
     __pyx_L9:;
 
-    /* "pe/_cy_machine.pyx":297
+    /* "pe/_cy_machine.pyx":299
  *                 raise Error(f'invalid operation: {instr.opcode}')
  * 
  *             if idx == FAILURE:             # <<<<<<<<<<<<<<
  *                 # pos is >= 0 only for backtracking entries
  *                 while state and state.pos < 0:
  */
-    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_idx); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
-    __pyx_t_10 = PyObject_RichCompare(__pyx_t_2, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_10 = PyObject_RichCompare(__pyx_t_2, __pyx_t_8, Py_EQ); __Pyx_XGOTREF(__pyx_t_10); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 297, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_t_10); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 299, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
     if (__pyx_t_1) {
 
-      /* "pe/_cy_machine.pyx":299
+      /* "pe/_cy_machine.pyx":301
  *             if idx == FAILURE:
  *                 # pos is >= 0 only for backtracking entries
  *                 while state and state.pos < 0:             # <<<<<<<<<<<<<<
  *                     state = pop(state)
  *                 idx = state.opidx
  */
       while (1) {
@@ -10211,244 +10303,244 @@
           goto __pyx_L14_bool_binop_done;
         }
         __pyx_t_11 = (__pyx_v_state->pos < 0);
         __pyx_t_1 = __pyx_t_11;
         __pyx_L14_bool_binop_done:;
         if (!__pyx_t_1) break;
 
-        /* "pe/_cy_machine.pyx":300
+        /* "pe/_cy_machine.pyx":302
  *                 # pos is >= 0 only for backtracking entries
  *                 while state and state.pos < 0:
  *                     state = pop(state)             # <<<<<<<<<<<<<<
  *                 idx = state.opidx
  *                 pos = state.pos
  */
-        __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 300, __pyx_L1_error)
+        __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 302, __pyx_L1_error)
         __pyx_v_state = __pyx_t_5;
       }
 
-      /* "pe/_cy_machine.pyx":301
+      /* "pe/_cy_machine.pyx":303
  *                 while state and state.pos < 0:
  *                     state = pop(state)
  *                 idx = state.opidx             # <<<<<<<<<<<<<<
  *                 pos = state.pos
  *                 args[state.argidx:] = []
  */
       __pyx_t_6 = __pyx_v_state->opidx;
       __pyx_v_idx = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":302
+      /* "pe/_cy_machine.pyx":304
  *                     state = pop(state)
  *                 idx = state.opidx
  *                 pos = state.pos             # <<<<<<<<<<<<<<
  *                 args[state.argidx:] = []
  *                 if kwargs:
  */
       __pyx_t_6 = __pyx_v_state->pos;
       __pyx_v_pos = __pyx_t_6;
 
-      /* "pe/_cy_machine.pyx":303
+      /* "pe/_cy_machine.pyx":305
  *                 idx = state.opidx
  *                 pos = state.pos
  *                 args[state.argidx:] = []             # <<<<<<<<<<<<<<
  *                 if kwargs:
  *                     kwargs[state.kwidx:] = []
  */
-      __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 303, __pyx_L1_error)
+      __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 305, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       if (unlikely(__pyx_v_args == Py_None)) {
         PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-        __PYX_ERR(0, 303, __pyx_L1_error)
+        __PYX_ERR(0, 305, __pyx_L1_error)
       }
-      if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_t_10, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 303, __pyx_L1_error)
+      if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_t_10, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 305, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-      /* "pe/_cy_machine.pyx":304
+      /* "pe/_cy_machine.pyx":306
  *                 pos = state.pos
  *                 args[state.argidx:] = []
  *                 if kwargs:             # <<<<<<<<<<<<<<
  *                     kwargs[state.kwidx:] = []
  *                 state = pop(state)  # pop backtracking entry
  */
       __pyx_t_1 = (__pyx_v_kwargs != Py_None)&&(PyList_GET_SIZE(__pyx_v_kwargs) != 0);
       if (__pyx_t_1) {
 
-        /* "pe/_cy_machine.pyx":305
+        /* "pe/_cy_machine.pyx":307
  *                 args[state.argidx:] = []
  *                 if kwargs:
  *                     kwargs[state.kwidx:] = []             # <<<<<<<<<<<<<<
  *                 state = pop(state)  # pop backtracking entry
  *             else:
  */
-        __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 305, __pyx_L1_error)
+        __pyx_t_10 = PyList_New(0); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 307, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
         if (unlikely(__pyx_v_kwargs == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 305, __pyx_L1_error)
+          __PYX_ERR(0, 307, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_10, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 305, __pyx_L1_error)
+        if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_10, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 307, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
 
-        /* "pe/_cy_machine.pyx":304
+        /* "pe/_cy_machine.pyx":306
  *                 pos = state.pos
  *                 args[state.argidx:] = []
  *                 if kwargs:             # <<<<<<<<<<<<<<
  *                     kwargs[state.kwidx:] = []
  *                 state = pop(state)  # pop backtracking entry
  */
       }
 
-      /* "pe/_cy_machine.pyx":306
+      /* "pe/_cy_machine.pyx":308
  *                 if kwargs:
  *                     kwargs[state.kwidx:] = []
  *                 state = pop(state)  # pop backtracking entry             # <<<<<<<<<<<<<<
  *             else:
  *                 if instr.capturing:
  */
-      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 306, __pyx_L1_error)
+      __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 308, __pyx_L1_error)
       __pyx_v_state = __pyx_t_5;
 
-      /* "pe/_cy_machine.pyx":297
+      /* "pe/_cy_machine.pyx":299
  *                 raise Error(f'invalid operation: {instr.opcode}')
  * 
  *             if idx == FAILURE:             # <<<<<<<<<<<<<<
  *                 # pos is >= 0 only for backtracking entries
  *                 while state and state.pos < 0:
  */
       goto __pyx_L11;
     }
 
-    /* "pe/_cy_machine.pyx":308
+    /* "pe/_cy_machine.pyx":310
  *                 state = pop(state)  # pop backtracking entry
  *             else:
  *                 if instr.capturing:             # <<<<<<<<<<<<<<
  *                     args[state.argidx:] = [s[state.mark:pos]]
  *                     kwargs[state.kwidx:] = []
  */
     /*else*/ {
       if (__pyx_v_instr->capturing) {
 
-        /* "pe/_cy_machine.pyx":309
+        /* "pe/_cy_machine.pyx":311
  *             else:
  *                 if instr.capturing:
  *                     args[state.argidx:] = [s[state.mark:pos]]             # <<<<<<<<<<<<<<
  *                     kwargs[state.kwidx:] = []
  *                     state = pop(state)
  */
         if (unlikely(__pyx_v_s == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 309, __pyx_L1_error)
+          __PYX_ERR(0, 311, __pyx_L1_error)
         }
-        __pyx_t_10 = __Pyx_PyUnicode_Substring(__pyx_v_s, __pyx_v_state->mark, __pyx_v_pos); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 309, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyUnicode_Substring(__pyx_v_s, __pyx_v_state->mark, __pyx_v_pos); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 311, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
-        __pyx_t_8 = PyList_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 309, __pyx_L1_error)
+        __pyx_t_8 = PyList_New(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 311, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         __Pyx_GIVEREF(__pyx_t_10);
-        if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_10)) __PYX_ERR(0, 309, __pyx_L1_error);
+        if (__Pyx_PyList_SET_ITEM(__pyx_t_8, 0, __pyx_t_10)) __PYX_ERR(0, 311, __pyx_L1_error);
         __pyx_t_10 = 0;
         if (unlikely(__pyx_v_args == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 309, __pyx_L1_error)
+          __PYX_ERR(0, 311, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_t_8, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 309, __pyx_L1_error)
+        if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_t_8, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 311, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-        /* "pe/_cy_machine.pyx":310
+        /* "pe/_cy_machine.pyx":312
  *                 if instr.capturing:
  *                     args[state.argidx:] = [s[state.mark:pos]]
  *                     kwargs[state.kwidx:] = []             # <<<<<<<<<<<<<<
  *                     state = pop(state)
  * 
  */
-        __pyx_t_8 = PyList_New(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 310, __pyx_L1_error)
+        __pyx_t_8 = PyList_New(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 312, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_8);
         if (unlikely(__pyx_v_kwargs == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 310, __pyx_L1_error)
+          __PYX_ERR(0, 312, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_8, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 310, __pyx_L1_error)
+        if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_8, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 312, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-        /* "pe/_cy_machine.pyx":311
+        /* "pe/_cy_machine.pyx":313
  *                     args[state.argidx:] = [s[state.mark:pos]]
  *                     kwargs[state.kwidx:] = []
  *                     state = pop(state)             # <<<<<<<<<<<<<<
  * 
  *                 if instr.action is not None:
  */
-        __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 311, __pyx_L1_error)
+        __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 313, __pyx_L1_error)
         __pyx_v_state = __pyx_t_5;
 
-        /* "pe/_cy_machine.pyx":308
+        /* "pe/_cy_machine.pyx":310
  *                 state = pop(state)  # pop backtracking entry
  *             else:
  *                 if instr.capturing:             # <<<<<<<<<<<<<<
  *                     args[state.argidx:] = [s[state.mark:pos]]
  *                     kwargs[state.kwidx:] = []
  */
       }
 
-      /* "pe/_cy_machine.pyx":313
+      /* "pe/_cy_machine.pyx":315
  *                     state = pop(state)
  * 
  *                 if instr.action is not None:             # <<<<<<<<<<<<<<
  *                     _args, _kwargs = instr.action(
  *                         s,
  */
       __pyx_t_1 = (__pyx_v_instr->action != Py_None);
       if (__pyx_t_1) {
 
-        /* "pe/_cy_machine.pyx":316
+        /* "pe/_cy_machine.pyx":318
  *                     _args, _kwargs = instr.action(
  *                         s,
  *                         state.mark,             # <<<<<<<<<<<<<<
  *                         pos,
  *                         args[state.argidx:],
  */
-        __pyx_t_10 = __Pyx_PyInt_From_int(__pyx_v_state->mark); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 316, __pyx_L1_error)
+        __pyx_t_10 = __Pyx_PyInt_From_int(__pyx_v_state->mark); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 318, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_10);
 
-        /* "pe/_cy_machine.pyx":317
+        /* "pe/_cy_machine.pyx":319
  *                         s,
  *                         state.mark,
  *                         pos,             # <<<<<<<<<<<<<<
  *                         args[state.argidx:],
  *                         dict(kwargs[state.kwidx:])
  */
-        __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 317, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 319, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
 
-        /* "pe/_cy_machine.pyx":318
+        /* "pe/_cy_machine.pyx":320
  *                         state.mark,
  *                         pos,
  *                         args[state.argidx:],             # <<<<<<<<<<<<<<
  *                         dict(kwargs[state.kwidx:])
  *                     )
  */
         if (unlikely(__pyx_v_args == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 318, __pyx_L1_error)
+          __PYX_ERR(0, 320, __pyx_L1_error)
         }
-        __pyx_t_9 = __Pyx_PyList_GetSlice(__pyx_v_args, __pyx_v_state->argidx, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 318, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_GetSlice(__pyx_v_args, __pyx_v_state->argidx, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 320, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_9);
 
-        /* "pe/_cy_machine.pyx":319
+        /* "pe/_cy_machine.pyx":321
  *                         pos,
  *                         args[state.argidx:],
  *                         dict(kwargs[state.kwidx:])             # <<<<<<<<<<<<<<
  *                     )
  *                     args[state.argidx:] = _args
  */
         if (unlikely(__pyx_v_kwargs == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 319, __pyx_L1_error)
+          __PYX_ERR(0, 321, __pyx_L1_error)
         }
-        __pyx_t_12 = __Pyx_PyList_GetSlice(__pyx_v_kwargs, __pyx_v_state->kwidx, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 319, __pyx_L1_error)
+        __pyx_t_12 = __Pyx_PyList_GetSlice(__pyx_v_kwargs, __pyx_v_state->kwidx, PY_SSIZE_T_MAX); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 321, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_12);
-        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_12); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 319, __pyx_L1_error)
+        __pyx_t_13 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyDict_Type)), __pyx_t_12); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 321, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         __Pyx_INCREF(__pyx_v_instr->action);
         __pyx_t_12 = __pyx_v_instr->action; __pyx_t_14 = NULL;
         __pyx_t_6 = 0;
         #if CYTHON_UNPACK_METHODS
         if (likely(PyMethod_Check(__pyx_t_12))) {
@@ -10466,136 +10558,136 @@
           PyObject *__pyx_callargs[6] = {__pyx_t_14, __pyx_v_s, __pyx_t_10, __pyx_t_2, __pyx_t_9, __pyx_t_13};
           __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_12, __pyx_callargs+1-__pyx_t_6, 5+__pyx_t_6);
           __Pyx_XDECREF(__pyx_t_14); __pyx_t_14 = 0;
           __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
           __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
-          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 314, __pyx_L1_error)
+          if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 316, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           __Pyx_DECREF(__pyx_t_12); __pyx_t_12 = 0;
         }
         if ((likely(PyTuple_CheckExact(__pyx_t_8))) || (PyList_CheckExact(__pyx_t_8))) {
           PyObject* sequence = __pyx_t_8;
           Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
           if (unlikely(size != 2)) {
             if (size > 2) __Pyx_RaiseTooManyValuesError(2);
             else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-            __PYX_ERR(0, 314, __pyx_L1_error)
+            __PYX_ERR(0, 316, __pyx_L1_error)
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
           if (likely(PyTuple_CheckExact(sequence))) {
             __pyx_t_12 = PyTuple_GET_ITEM(sequence, 0); 
             __pyx_t_13 = PyTuple_GET_ITEM(sequence, 1); 
           } else {
             __pyx_t_12 = PyList_GET_ITEM(sequence, 0); 
             __pyx_t_13 = PyList_GET_ITEM(sequence, 1); 
           }
           __Pyx_INCREF(__pyx_t_12);
           __Pyx_INCREF(__pyx_t_13);
           #else
-          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 314, __pyx_L1_error)
+          __pyx_t_12 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_12)) __PYX_ERR(0, 316, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_12);
-          __pyx_t_13 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 314, __pyx_L1_error)
+          __pyx_t_13 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 316, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_13);
           #endif
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         } else {
           Py_ssize_t index = -1;
-          __pyx_t_9 = PyObject_GetIter(__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 314, __pyx_L1_error)
+          __pyx_t_9 = PyObject_GetIter(__pyx_t_8); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 316, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_9);
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
           __pyx_t_15 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_9);
           index = 0; __pyx_t_12 = __pyx_t_15(__pyx_t_9); if (unlikely(!__pyx_t_12)) goto __pyx_L19_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_12);
           index = 1; __pyx_t_13 = __pyx_t_15(__pyx_t_9); if (unlikely(!__pyx_t_13)) goto __pyx_L19_unpacking_failed;
           __Pyx_GOTREF(__pyx_t_13);
-          if (__Pyx_IternextUnpackEndCheck(__pyx_t_15(__pyx_t_9), 2) < 0) __PYX_ERR(0, 314, __pyx_L1_error)
+          if (__Pyx_IternextUnpackEndCheck(__pyx_t_15(__pyx_t_9), 2) < 0) __PYX_ERR(0, 316, __pyx_L1_error)
           __pyx_t_15 = NULL;
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           goto __pyx_L20_unpacking_done;
           __pyx_L19_unpacking_failed:;
           __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
           __pyx_t_15 = NULL;
           if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-          __PYX_ERR(0, 314, __pyx_L1_error)
+          __PYX_ERR(0, 316, __pyx_L1_error)
           __pyx_L20_unpacking_done:;
         }
 
-        /* "pe/_cy_machine.pyx":314
+        /* "pe/_cy_machine.pyx":316
  * 
  *                 if instr.action is not None:
  *                     _args, _kwargs = instr.action(             # <<<<<<<<<<<<<<
  *                         s,
  *                         state.mark,
  */
         __Pyx_XDECREF_SET(__pyx_v__args, __pyx_t_12);
         __pyx_t_12 = 0;
         __Pyx_XDECREF_SET(__pyx_v__kwargs, __pyx_t_13);
         __pyx_t_13 = 0;
 
-        /* "pe/_cy_machine.pyx":321
+        /* "pe/_cy_machine.pyx":323
  *                         dict(kwargs[state.kwidx:])
  *                     )
  *                     args[state.argidx:] = _args             # <<<<<<<<<<<<<<
  *                     if not _kwargs:
  *                         kwargs[state.kwidx:] = []
  */
         if (unlikely(__pyx_v_args == Py_None)) {
           PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-          __PYX_ERR(0, 321, __pyx_L1_error)
+          __PYX_ERR(0, 323, __pyx_L1_error)
         }
-        if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_v__args, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 321, __pyx_L1_error)
+        if (__Pyx_PyObject_SetSlice(__pyx_v_args, __pyx_v__args, __pyx_v_state->argidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
 
-        /* "pe/_cy_machine.pyx":322
+        /* "pe/_cy_machine.pyx":324
  *                     )
  *                     args[state.argidx:] = _args
  *                     if not _kwargs:             # <<<<<<<<<<<<<<
  *                         kwargs[state.kwidx:] = []
  *                     else:
  */
-        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v__kwargs); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 322, __pyx_L1_error)
+        __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v__kwargs); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(0, 324, __pyx_L1_error)
         __pyx_t_11 = (!__pyx_t_1);
         if (__pyx_t_11) {
 
-          /* "pe/_cy_machine.pyx":323
+          /* "pe/_cy_machine.pyx":325
  *                     args[state.argidx:] = _args
  *                     if not _kwargs:
  *                         kwargs[state.kwidx:] = []             # <<<<<<<<<<<<<<
  *                     else:
  *                         kwargs[state.kwidx:] = _kwargs.items()
  */
-          __pyx_t_8 = PyList_New(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 323, __pyx_L1_error)
+          __pyx_t_8 = PyList_New(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 325, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_8);
           if (unlikely(__pyx_v_kwargs == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-            __PYX_ERR(0, 323, __pyx_L1_error)
+            __PYX_ERR(0, 325, __pyx_L1_error)
           }
-          if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_8, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 323, __pyx_L1_error)
+          if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_8, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-          /* "pe/_cy_machine.pyx":322
+          /* "pe/_cy_machine.pyx":324
  *                     )
  *                     args[state.argidx:] = _args
  *                     if not _kwargs:             # <<<<<<<<<<<<<<
  *                         kwargs[state.kwidx:] = []
  *                     else:
  */
           goto __pyx_L21;
         }
 
-        /* "pe/_cy_machine.pyx":325
+        /* "pe/_cy_machine.pyx":327
  *                         kwargs[state.kwidx:] = []
  *                     else:
  *                         kwargs[state.kwidx:] = _kwargs.items()             # <<<<<<<<<<<<<<
  *                     state = pop(state)
  * 
  */
         /*else*/ {
-          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v__kwargs, __pyx_n_s_items); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 325, __pyx_L1_error)
+          __pyx_t_13 = __Pyx_PyObject_GetAttrStr(__pyx_v__kwargs, __pyx_n_s_items); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 327, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_13);
           __pyx_t_12 = NULL;
           __pyx_t_6 = 0;
           #if CYTHON_UNPACK_METHODS
           if (likely(PyMethod_Check(__pyx_t_13))) {
             __pyx_t_12 = PyMethod_GET_SELF(__pyx_t_13);
             if (likely(__pyx_t_12)) {
@@ -10607,113 +10699,113 @@
             }
           }
           #endif
           {
             PyObject *__pyx_callargs[2] = {__pyx_t_12, NULL};
             __pyx_t_8 = __Pyx_PyObject_FastCall(__pyx_t_13, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
             __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
-            if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 325, __pyx_L1_error)
+            if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 327, __pyx_L1_error)
             __Pyx_GOTREF(__pyx_t_8);
             __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
           }
           if (unlikely(__pyx_v_kwargs == Py_None)) {
             PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-            __PYX_ERR(0, 325, __pyx_L1_error)
+            __PYX_ERR(0, 327, __pyx_L1_error)
           }
-          if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_8, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 325, __pyx_L1_error)
+          if (__Pyx_PyObject_SetSlice(__pyx_v_kwargs, __pyx_t_8, __pyx_v_state->kwidx, 0, NULL, NULL, NULL, 1, 0, 1) < 0) __PYX_ERR(0, 327, __pyx_L1_error)
           __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
         }
         __pyx_L21:;
 
-        /* "pe/_cy_machine.pyx":326
+        /* "pe/_cy_machine.pyx":328
  *                     else:
  *                         kwargs[state.kwidx:] = _kwargs.items()
  *                     state = pop(state)             # <<<<<<<<<<<<<<
  * 
  *                 idx += 1
  */
-        __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 326, __pyx_L1_error)
+        __pyx_t_5 = __pyx_f_2pe_11_cy_machine_pop(__pyx_v_state); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL) && PyErr_Occurred())) __PYX_ERR(0, 328, __pyx_L1_error)
         __pyx_v_state = __pyx_t_5;
 
-        /* "pe/_cy_machine.pyx":313
+        /* "pe/_cy_machine.pyx":315
  *                     state = pop(state)
  * 
  *                 if instr.action is not None:             # <<<<<<<<<<<<<<
  *                     _args, _kwargs = instr.action(
  *                         s,
  */
       }
 
-      /* "pe/_cy_machine.pyx":328
+      /* "pe/_cy_machine.pyx":330
  *                     state = pop(state)
  * 
  *                 idx += 1             # <<<<<<<<<<<<<<
  * 
  *         if not state:
  */
       __pyx_v_idx = (__pyx_v_idx + 1);
     }
     __pyx_L11:;
     __pyx_L6_continue:;
   }
   __pyx_L7_break:;
 
-  /* "pe/_cy_machine.pyx":330
+  /* "pe/_cy_machine.pyx":332
  *                 idx += 1
  * 
  *         if not state:             # <<<<<<<<<<<<<<
  *             state = push(0, -1, -1, 0, 0, NULL)
  *         else:
  */
   __pyx_t_11 = (!(__pyx_v_state != 0));
   if (__pyx_t_11) {
 
-    /* "pe/_cy_machine.pyx":331
+    /* "pe/_cy_machine.pyx":333
  * 
  *         if not state:
  *             state = push(0, -1, -1, 0, 0, NULL)             # <<<<<<<<<<<<<<
  *         else:
  *             state.pos = pos
  */
-    __pyx_t_5 = __pyx_f_2pe_11_cy_machine_push(0, -1, -1, 0, 0, NULL); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 331, __pyx_L1_error)
+    __pyx_t_5 = __pyx_f_2pe_11_cy_machine_push(0, -1, -1, 0, 0, NULL); if (unlikely(__pyx_t_5 == ((struct __pyx_t_2pe_11_cy_machine_State *)NULL))) __PYX_ERR(0, 333, __pyx_L1_error)
     __pyx_v_state = __pyx_t_5;
 
-    /* "pe/_cy_machine.pyx":330
+    /* "pe/_cy_machine.pyx":332
  *                 idx += 1
  * 
  *         if not state:             # <<<<<<<<<<<<<<
  *             state = push(0, -1, -1, 0, 0, NULL)
  *         else:
  */
     goto __pyx_L22;
   }
 
-  /* "pe/_cy_machine.pyx":333
+  /* "pe/_cy_machine.pyx":335
  *             state = push(0, -1, -1, 0, 0, NULL)
  *         else:
  *             state.pos = pos             # <<<<<<<<<<<<<<
  *         return state
  * 
  */
   /*else*/ {
     __pyx_v_state->pos = __pyx_v_pos;
   }
   __pyx_L22:;
 
-  /* "pe/_cy_machine.pyx":334
+  /* "pe/_cy_machine.pyx":336
  *         else:
  *             state.pos = pos
  *         return state             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_state;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":218
+  /* "pe/_cy_machine.pyx":220
  *         return retval
  * 
  *     cdef State* _match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
 
@@ -11134,15 +11226,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":344
+/* "pe/_cy_machine.pyx":346
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
 
@@ -11196,31 +11288,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_grammar)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 344, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 346, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_make_program") < 0)) __PYX_ERR(0, 344, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_make_program") < 0)) __PYX_ERR(0, 346, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_grammar = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_make_program", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 344, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_make_program", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 346, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -11263,141 +11355,141 @@
   int __pyx_t_10;
   int __pyx_t_11;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_make_program", 1);
 
-  /* "pe/_cy_machine.pyx":346
+  /* "pe/_cy_machine.pyx":348
  * def _make_program(grammar) -> Tuple[_Program, _Index]:
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}             # <<<<<<<<<<<<<<
  *     pis: _Program = []
  * 
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 348, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_index = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":347
+  /* "pe/_cy_machine.pyx":349
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  *     pis: _Program = []             # <<<<<<<<<<<<<<
  * 
  *     pis.append(Instruction(FAIL))  # special instruction for general failure
  */
-  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 347, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pis = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":349
+  /* "pe/_cy_machine.pyx":351
  *     pis: _Program = []
  * 
  *     pis.append(Instruction(FAIL))  # special instruction for general failure             # <<<<<<<<<<<<<<
  *     for name in grammar.definitions:
  *         index[name] = len(pis)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAIL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAIL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 351, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 351, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 349, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 351, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":350
+  /* "pe/_cy_machine.pyx":352
  * 
  *     pis.append(Instruction(FAIL))  # special instruction for general failure
  *     for name in grammar.definitions:             # <<<<<<<<<<<<<<
  *         index[name] = len(pis)
  *         _pis = _parsing_instructions(grammar[name])
  */
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_grammar, __pyx_n_s_definitions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_grammar, __pyx_n_s_definitions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
     __pyx_t_1 = __pyx_t_2; __Pyx_INCREF(__pyx_t_1);
     __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
   } else {
-    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_4 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 352, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 350, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 352, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   for (;;) {
     if (likely(!__pyx_t_5)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 350, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 352, __pyx_L1_error)
           #endif
           if (__pyx_t_4 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 350, __pyx_L1_error)
+        __pyx_t_2 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 352, __pyx_L1_error)
         #else
-        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 350, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 352, __pyx_L1_error)
           #endif
           if (__pyx_t_4 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 350, __pyx_L1_error)
+        __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 352, __pyx_L1_error)
         #else
-        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 350, __pyx_L1_error)
+        __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_2);
         #endif
       }
     } else {
       __pyx_t_2 = __pyx_t_5(__pyx_t_1);
       if (unlikely(!__pyx_t_2)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 350, __pyx_L1_error)
+          else __PYX_ERR(0, 352, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_2);
     }
     __Pyx_XDECREF_SET(__pyx_v_name, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":351
+    /* "pe/_cy_machine.pyx":353
  *     pis.append(Instruction(FAIL))  # special instruction for general failure
  *     for name in grammar.definitions:
  *         index[name] = len(pis)             # <<<<<<<<<<<<<<
  *         _pis = _parsing_instructions(grammar[name])
  *         pis.extend(_pis)
  */
-    __pyx_t_6 = __Pyx_PyList_GET_SIZE(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 351, __pyx_L1_error)
-    __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 351, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyList_GET_SIZE(__pyx_v_pis); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 353, __pyx_L1_error)
+    __pyx_t_2 = PyInt_FromSsize_t(__pyx_t_6); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 353, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (unlikely((PyDict_SetItem(__pyx_v_index, __pyx_v_name, __pyx_t_2) < 0))) __PYX_ERR(0, 351, __pyx_L1_error)
+    if (unlikely((PyDict_SetItem(__pyx_v_index, __pyx_v_name, __pyx_t_2) < 0))) __PYX_ERR(0, 353, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":352
+    /* "pe/_cy_machine.pyx":354
  *     for name in grammar.definitions:
  *         index[name] = len(pis)
  *         _pis = _parsing_instructions(grammar[name])             # <<<<<<<<<<<<<<
  *         pis.extend(_pis)
  *         pis.append(Instruction(RETURN))
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_grammar, __pyx_v_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 352, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_GetItem(__pyx_v_grammar, __pyx_v_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 354, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __pyx_t_9 = NULL;
     __pyx_t_10 = 0;
     #if CYTHON_UNPACK_METHODS
     if (unlikely(PyMethod_Check(__pyx_t_7))) {
       __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_7);
       if (likely(__pyx_t_9)) {
@@ -11410,169 +11502,169 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_t_8};
       __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
       __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 352, __pyx_L1_error)
+      if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 354, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     }
     __Pyx_XDECREF_SET(__pyx_v__pis, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":353
+    /* "pe/_cy_machine.pyx":355
  *         index[name] = len(pis)
  *         _pis = _parsing_instructions(grammar[name])
  *         pis.extend(_pis)             # <<<<<<<<<<<<<<
  *         pis.append(Instruction(RETURN))
  * 
  */
-    __pyx_t_3 = __Pyx_PyList_Extend(__pyx_v_pis, __pyx_v__pis); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 353, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyList_Extend(__pyx_v_pis, __pyx_v__pis); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 355, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":354
+    /* "pe/_cy_machine.pyx":356
  *         _pis = _parsing_instructions(grammar[name])
  *         pis.extend(_pis)
  *         pis.append(Instruction(RETURN))             # <<<<<<<<<<<<<<
  * 
  *     # add locations to calls
  */
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RETURN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RETURN); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_7); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 354, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_7); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 356, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":350
+    /* "pe/_cy_machine.pyx":352
  * 
  *     pis.append(Instruction(FAIL))  # special instruction for general failure
  *     for name in grammar.definitions:             # <<<<<<<<<<<<<<
  *         index[name] = len(pis)
  *         _pis = _parsing_instructions(grammar[name])
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":357
+  /* "pe/_cy_machine.pyx":359
  * 
  *     # add locations to calls
  *     for pi in pis:             # <<<<<<<<<<<<<<
  *         if pi.opcode == CALL:
  *             pi.oploc = index[pi.name]
  */
   __pyx_t_1 = __pyx_v_pis; __Pyx_INCREF(__pyx_t_1);
   __pyx_t_4 = 0;
   for (;;) {
     {
       Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
       #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 357, __pyx_L1_error)
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 359, __pyx_L1_error)
       #endif
       if (__pyx_t_4 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 357, __pyx_L1_error)
+    __pyx_t_7 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_4); __Pyx_INCREF(__pyx_t_7); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 359, __pyx_L1_error)
     #else
-    __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 357, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 359, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     #endif
     __Pyx_XDECREF_SET(__pyx_v_pi, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":358
+    /* "pe/_cy_machine.pyx":360
  *     # add locations to calls
  *     for pi in pis:
  *         if pi.opcode == CALL:             # <<<<<<<<<<<<<<
  *             pi.oploc = index[pi.name]
  * 
  */
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 358, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 358, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 358, __pyx_L1_error)
+    __pyx_t_8 = PyObject_RichCompare(__pyx_t_7, __pyx_t_2, Py_EQ); __Pyx_XGOTREF(__pyx_t_8); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 358, __pyx_L1_error)
+    __pyx_t_11 = __Pyx_PyObject_IsTrue(__pyx_t_8); if (unlikely((__pyx_t_11 < 0))) __PYX_ERR(0, 360, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     if (__pyx_t_11) {
 
-      /* "pe/_cy_machine.pyx":359
+      /* "pe/_cy_machine.pyx":361
  *     for pi in pis:
  *         if pi.opcode == CALL:
  *             pi.oploc = index[pi.name]             # <<<<<<<<<<<<<<
  * 
  *     pis.append(Instruction(PASS))  # success condition
  */
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 359, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_name); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 361, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
-      __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_index, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 359, __pyx_L1_error)
+      __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_index, __pyx_t_8); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 361, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_2);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_oploc, __pyx_t_2) < 0) __PYX_ERR(0, 359, __pyx_L1_error)
+      if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_oploc, __pyx_t_2) < 0) __PYX_ERR(0, 361, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-      /* "pe/_cy_machine.pyx":358
+      /* "pe/_cy_machine.pyx":360
  *     # add locations to calls
  *     for pi in pis:
  *         if pi.opcode == CALL:             # <<<<<<<<<<<<<<
  *             pi.oploc = index[pi.name]
  * 
  */
     }
 
-    /* "pe/_cy_machine.pyx":357
+    /* "pe/_cy_machine.pyx":359
  * 
  *     # add locations to calls
  *     for pi in pis:             # <<<<<<<<<<<<<<
  *         if pi.opcode == CALL:
  *             pi.oploc = index[pi.name]
  */
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":361
+  /* "pe/_cy_machine.pyx":363
  *             pi.oploc = index[pi.name]
  * 
  *     pis.append(Instruction(PASS))  # success condition             # <<<<<<<<<<<<<<
  * 
  *     return pis, index
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_PASS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_PASS); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 361, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyList_Append(__pyx_v_pis, __pyx_t_2); if (unlikely(__pyx_t_3 == ((int)-1))) __PYX_ERR(0, 363, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":363
+  /* "pe/_cy_machine.pyx":365
  *     pis.append(Instruction(PASS))  # success condition
  * 
  *     return pis, index             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 363, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 365, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_pis);
   __Pyx_GIVEREF(__pyx_v_pis);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_pis)) __PYX_ERR(0, 363, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_pis)) __PYX_ERR(0, 365, __pyx_L1_error);
   __Pyx_INCREF(__pyx_v_index);
   __Pyx_GIVEREF(__pyx_v_index);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_index)) __PYX_ERR(0, 363, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_index)) __PYX_ERR(0, 365, __pyx_L1_error);
   __pyx_r = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":344
+  /* "pe/_cy_machine.pyx":346
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
 
@@ -11592,15 +11684,15 @@
   __Pyx_XDECREF(__pyx_v__pis);
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":366
+/* "pe/_cy_machine.pyx":368
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
 
@@ -11653,31 +11745,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 366, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 368, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_dot") < 0)) __PYX_ERR(0, 366, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_dot") < 0)) __PYX_ERR(0, 368, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_dot", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 366, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_dot", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 368, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -11707,49 +11799,49 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_dot", 1);
 
-  /* "pe/_cy_machine.pyx":367
+  /* "pe/_cy_machine.pyx":369
  * 
  * def _dot(defn):
  *     return [Instruction(SCAN, scanner=Dot())]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Dot)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallNoArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Dot)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_3) < 0) __PYX_ERR(0, 367, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_3) < 0) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 367, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 369, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 367, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 369, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":366
+  /* "pe/_cy_machine.pyx":368
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
 
@@ -11762,15 +11854,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":370
+/* "pe/_cy_machine.pyx":372
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
 
@@ -11823,31 +11915,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 370, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 372, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_lit") < 0)) __PYX_ERR(0, 370, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_lit") < 0)) __PYX_ERR(0, 372, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_lit", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 370, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_lit", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 372, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -11878,55 +11970,55 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_lit", 1);
 
-  /* "pe/_cy_machine.pyx":371
+  /* "pe/_cy_machine.pyx":373
  * 
  * def _lit(defn):
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Literal), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Literal), __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_3) < 0) __PYX_ERR(0, 371, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_3) < 0) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 371, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 371, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_3)) __PYX_ERR(0, 373, __pyx_L1_error);
   __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":370
+  /* "pe/_cy_machine.pyx":372
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
 
@@ -11940,15 +12032,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":374
+/* "pe/_cy_machine.pyx":376
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
 
@@ -12009,34 +12101,34 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 374, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mincount);
           if (value) { values[1] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 374, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_maxcount);
           if (value) { values[2] = __Pyx_Arg_NewRef_FASTCALL(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 374, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 376, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_cls") < 0)) __PYX_ERR(0, 374, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_cls") < 0)) __PYX_ERR(0, 376, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
@@ -12047,15 +12139,15 @@
     }
     __pyx_v_defn = values[0];
     __pyx_v_mincount = values[1];
     __pyx_v_maxcount = values[2];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_cls", 0, 1, 3, __pyx_nargs); __PYX_ERR(0, 374, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_cls", 0, 1, 3, __pyx_nargs); __PYX_ERR(0, 376, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -12087,121 +12179,121 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_cls", 1);
 
-  /* "pe/_cy_machine.pyx":376
+  /* "pe/_cy_machine.pyx":378
  * def _cls(defn, mincount=1, maxcount=1):
  *     cclass = CharacterClass(
  *         defn.args[0],             # <<<<<<<<<<<<<<
  *         negate=defn.args[1],
  *         mincount=mincount,
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 378, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":375
+  /* "pe/_cy_machine.pyx":377
  * 
  * def _cls(defn, mincount=1, maxcount=1):
  *     cclass = CharacterClass(             # <<<<<<<<<<<<<<
  *         defn.args[0],
  *         negate=defn.args[1],
  */
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2)) __PYX_ERR(0, 375, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2)) __PYX_ERR(0, 377, __pyx_L1_error);
   __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":377
+  /* "pe/_cy_machine.pyx":379
  *     cclass = CharacterClass(
  *         defn.args[0],
  *         negate=defn.args[1],             # <<<<<<<<<<<<<<
  *         mincount=mincount,
  *         maxcount=maxcount
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_negate, __pyx_t_4) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_negate, __pyx_t_4) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":378
+  /* "pe/_cy_machine.pyx":380
  *         defn.args[0],
  *         negate=defn.args[1],
  *         mincount=mincount,             # <<<<<<<<<<<<<<
  *         maxcount=maxcount
  *     )
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_mincount, __pyx_v_mincount) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_mincount, __pyx_v_mincount) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":379
+  /* "pe/_cy_machine.pyx":381
  *         negate=defn.args[1],
  *         mincount=mincount,
  *         maxcount=maxcount             # <<<<<<<<<<<<<<
  *     )
  *     return [Instruction(SCAN, scanner=cclass)]
  */
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_maxcount, __pyx_v_maxcount) < 0) __PYX_ERR(0, 377, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_maxcount, __pyx_v_maxcount) < 0) __PYX_ERR(0, 379, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":375
+  /* "pe/_cy_machine.pyx":377
  * 
  * def _cls(defn, mincount=1, maxcount=1):
  *     cclass = CharacterClass(             # <<<<<<<<<<<<<<
  *         defn.args[0],
  *         negate=defn.args[1],
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_CharacterClass), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 375, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_CharacterClass), __pyx_t_1, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 377, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_cclass = ((struct __pyx_obj_2pe_11_cy_machine_CharacterClass *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":381
+  /* "pe/_cy_machine.pyx":383
  *         maxcount=maxcount
  *     )
  *     return [Instruction(SCAN, scanner=cclass)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error);
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scanner, ((PyObject *)__pyx_v_cclass)) < 0) __PYX_ERR(0, 381, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 381, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scanner, ((PyObject *)__pyx_v_cclass)) < 0) __PYX_ERR(0, 383, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 381, __pyx_L1_error)
+  __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 383, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 381, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1)) __PYX_ERR(0, 383, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":374
+  /* "pe/_cy_machine.pyx":376
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
 
@@ -12216,15 +12308,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_cclass);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":384
+/* "pe/_cy_machine.pyx":386
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
 
@@ -12277,31 +12369,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 384, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 386, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_rgx") < 0)) __PYX_ERR(0, 384, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_rgx") < 0)) __PYX_ERR(0, 386, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_rgx", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 384, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_rgx", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 386, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -12336,119 +12428,119 @@
   PyObject *(*__pyx_t_5)(PyObject *);
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_rgx", 1);
 
-  /* "pe/_cy_machine.pyx":385
+  /* "pe/_cy_machine.pyx":387
  * 
  * def _rgx(defn):
  *     pat, flags = defn.args             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  * 
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 385, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 387, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 2)) {
       if (size > 2) __Pyx_RaiseTooManyValuesError(2);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 385, __pyx_L1_error)
+      __PYX_ERR(0, 387, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
     } else {
       __pyx_t_2 = PyList_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 387, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 387, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 385, __pyx_L1_error)
+    __pyx_t_4 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 387, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4);
     index = 0; __pyx_t_2 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_5(__pyx_t_4); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 385, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_5(__pyx_t_4), 2) < 0) __PYX_ERR(0, 387, __pyx_L1_error)
     __pyx_t_5 = NULL;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_5 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 385, __pyx_L1_error)
+    __PYX_ERR(0, 387, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_pat = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_flags = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":386
+  /* "pe/_cy_machine.pyx":388
  * def _rgx(defn):
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 388, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_pat);
   __Pyx_GIVEREF(__pyx_v_pat);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_pat)) __PYX_ERR(0, 386, __pyx_L1_error);
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 386, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_pat)) __PYX_ERR(0, 388, __pyx_L1_error);
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flags, __pyx_v_flags) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
-  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Regex), __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 386, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_flags, __pyx_v_flags) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Regex), __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_6) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_scanner, __pyx_t_6) < 0) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 386, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 388, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_6);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_6)) __PYX_ERR(0, 386, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_6)) __PYX_ERR(0, 388, __pyx_L1_error);
   __pyx_t_6 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":384
+  /* "pe/_cy_machine.pyx":386
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
 
@@ -12465,15 +12557,15 @@
   __Pyx_XDECREF(__pyx_v_pat);
   __Pyx_XDECREF(__pyx_v_flags);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":389
+/* "pe/_cy_machine.pyx":391
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -12526,31 +12618,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 389, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 391, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_opt") < 0)) __PYX_ERR(0, 389, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_opt") < 0)) __PYX_ERR(0, 391, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_opt", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 389, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_opt", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 391, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -12584,26 +12676,26 @@
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_opt", 1);
 
-  /* "pe/_cy_machine.pyx":390
+  /* "pe/_cy_machine.pyx":392
  * 
  * def _opt(defn):
  *     pi = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 390, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 392, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -12617,89 +12709,89 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 390, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 392, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":391
+  /* "pe/_cy_machine.pyx":393
  * def _opt(defn):
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),             # <<<<<<<<<<<<<<
  *             *pi,
  *             Instruction(COMMIT, 1)]
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 391, __pyx_L1_error)
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 391, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 393, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 391, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 391, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 391, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":392
+  /* "pe/_cy_machine.pyx":394
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,             # <<<<<<<<<<<<<<
  *             Instruction(COMMIT, 1)]
  * 
  */
-  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 392, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 394, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":393
+  /* "pe/_cy_machine.pyx":395
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  *             Instruction(COMMIT, 1)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 395, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_1);
   __Pyx_GIVEREF(__pyx_int_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_int_1)) __PYX_ERR(0, 393, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_int_1)) __PYX_ERR(0, 395, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 393, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_3) < 0) __PYX_ERR(0, 393, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_3) < 0) __PYX_ERR(0, 395, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":389
+  /* "pe/_cy_machine.pyx":391
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -12714,15 +12806,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":396
+/* "pe/_cy_machine.pyx":398
  * 
  * 
  * def _str(defn): return _rpt(defn, 0)             # <<<<<<<<<<<<<<
  * def _pls(defn): return _rpt(defn, 1)
  * 
  */
 
@@ -12775,31 +12867,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 396, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 398, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_str") < 0)) __PYX_ERR(0, 396, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_str") < 0)) __PYX_ERR(0, 398, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_str", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 396, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_str", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 398, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -12830,15 +12922,15 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_str", 1);
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -12850,15 +12942,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_defn, __pyx_int_0};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 396, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 398, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
@@ -12871,15 +12963,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":397
+/* "pe/_cy_machine.pyx":399
  * 
  * def _str(defn): return _rpt(defn, 0)
  * def _pls(defn): return _rpt(defn, 1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
@@ -12932,31 +13024,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 397, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 399, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_pls") < 0)) __PYX_ERR(0, 397, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_pls") < 0)) __PYX_ERR(0, 399, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_pls", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 397, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_pls", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 399, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -12987,15 +13079,15 @@
   PyObject *__pyx_t_3 = NULL;
   int __pyx_t_4;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_pls", 1);
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rpt); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = NULL;
   __pyx_t_4 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_3)) {
@@ -13007,15 +13099,15 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_v_defn, __pyx_int_1};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_4, 2+__pyx_t_4);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 397, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 399, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
@@ -13028,15 +13120,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":400
+/* "pe/_cy_machine.pyx":402
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
 
@@ -13092,43 +13184,43 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 402, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mincount)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[1]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 400, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 402, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("_rpt", 1, 2, 2, 1); __PYX_ERR(0, 400, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("_rpt", 1, 2, 2, 1); __PYX_ERR(0, 402, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_rpt") < 0)) __PYX_ERR(0, 400, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_rpt") < 0)) __PYX_ERR(0, 402, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 2)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
     }
     __pyx_v_defn = values[0];
     __pyx_v_mincount = values[1];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_rpt", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 400, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_rpt", 1, 2, 2, __pyx_nargs); __PYX_ERR(0, 402, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -13148,15 +13240,15 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_2pe_11_cy_machine_4_rpt_2generator(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pe/_cy_machine.pyx":416
+/* "pe/_cy_machine.pyx":418
  *                             capturing=pi.capturing,
  *                             action=pi.action)]
  *     return [*(pi.copy() for _ in range(mincount) for pi in pis),             # <<<<<<<<<<<<<<
  *             Instruction(BRANCH, len(pis) + 2),
  *             *pis,
  */
 
@@ -13168,26 +13260,26 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr *)__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_1_genexpr(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 416, __pyx_L1_error)
+    __PYX_ERR(0, 418, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_outer_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt *) __pyx_self;
   __Pyx_INCREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
   __Pyx_GIVEREF((PyObject *)__pyx_cur_scope->__pyx_outer_scope);
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_4_rpt_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_rpt_locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_4_rpt_2generator, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_rpt_locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -13222,130 +13314,130 @@
     case 0: goto __pyx_L3_first_run;
     case 1: goto __pyx_L8_resume_from_yield;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 416, __pyx_L1_error)
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 416, __pyx_L1_error) }
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 418, __pyx_L1_error)
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 418, __pyx_L1_error) }
   if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_genexpr_arg_0)) {
     __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
     __pyx_t_2 = 0;
     __pyx_t_3 = NULL;
   } else {
-    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_2 = -1; __pyx_t_1 = PyObject_GetIter(__pyx_cur_scope->__pyx_genexpr_arg_0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 416, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 418, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_1))) {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 418, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 418, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         {
           Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_1);
           #if !CYTHON_ASSUME_SAFE_MACROS
-          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+          if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 418, __pyx_L1_error)
           #endif
           if (__pyx_t_2 >= __pyx_temp) break;
         }
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_4); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 418, __pyx_L1_error)
         #else
-        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
+        __pyx_t_4 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_1);
       if (unlikely(!__pyx_t_4)) {
         PyObject* exc_type = PyErr_Occurred();
         if (exc_type) {
           if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-          else __PYX_ERR(0, 416, __pyx_L1_error)
+          else __PYX_ERR(0, 418, __pyx_L1_error)
         }
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v__);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v__, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
-    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pis)) { __Pyx_RaiseClosureNameError("pis"); __PYX_ERR(0, 416, __pyx_L1_error) }
+    if (unlikely(!__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pis)) { __Pyx_RaiseClosureNameError("pis"); __PYX_ERR(0, 418, __pyx_L1_error) }
     if (likely(PyList_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pis)) || PyTuple_CheckExact(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pis)) {
       __pyx_t_4 = __pyx_cur_scope->__pyx_outer_scope->__pyx_v_pis; __Pyx_INCREF(__pyx_t_4);
       __pyx_t_5 = 0;
       __pyx_t_6 = NULL;
     } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pis); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
+      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_cur_scope->__pyx_outer_scope->__pyx_v_pis); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 416, __pyx_L1_error)
+      __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 418, __pyx_L1_error)
     }
     for (;;) {
       if (likely(!__pyx_t_6)) {
         if (likely(PyList_CheckExact(__pyx_t_4))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_4);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 418, __pyx_L1_error)
             #endif
             if (__pyx_t_5 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+          __pyx_t_7 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 418, __pyx_L1_error)
           #else
-          __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 416, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_4);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 418, __pyx_L1_error)
             #endif
             if (__pyx_t_5 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 416, __pyx_L1_error)
+          __pyx_t_7 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_7); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(0, 418, __pyx_L1_error)
           #else
-          __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 416, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_7);
           #endif
         }
       } else {
         __pyx_t_7 = __pyx_t_6(__pyx_t_4);
         if (unlikely(!__pyx_t_7)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 416, __pyx_L1_error)
+            else __PYX_ERR(0, 418, __pyx_L1_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_7);
       }
       __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_pi);
       __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_pi, __pyx_t_7);
       __Pyx_GIVEREF(__pyx_t_7);
       __pyx_t_7 = 0;
-      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_pi, __pyx_n_s_copy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 416, __pyx_L1_error)
+      __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_cur_scope->__pyx_v_pi, __pyx_n_s_copy); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 418, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_8);
       __pyx_t_9 = NULL;
       __pyx_t_10 = 0;
       #if CYTHON_UNPACK_METHODS
       if (likely(PyMethod_Check(__pyx_t_8))) {
         __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
         if (likely(__pyx_t_9)) {
@@ -13357,15 +13449,15 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_9, NULL};
         __pyx_t_7 = __Pyx_PyObject_FastCall(__pyx_t_8, __pyx_callargs+1-__pyx_t_10, 0+__pyx_t_10);
         __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
-        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 416, __pyx_L1_error)
+        if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 418, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       }
       __pyx_r = __pyx_t_7;
       __pyx_t_7 = 0;
       __Pyx_XGIVEREF(__pyx_t_1);
       __pyx_cur_scope->__pyx_t_0 = __pyx_t_1;
@@ -13388,15 +13480,15 @@
       __pyx_t_2 = __pyx_cur_scope->__pyx_t_1;
       __pyx_t_3 = __pyx_cur_scope->__pyx_t_2;
       __pyx_t_4 = __pyx_cur_scope->__pyx_t_3;
       __pyx_cur_scope->__pyx_t_3 = 0;
       __Pyx_XGOTREF(__pyx_t_4);
       __pyx_t_5 = __pyx_cur_scope->__pyx_t_4;
       __pyx_t_6 = __pyx_cur_scope->__pyx_t_5;
-      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 416, __pyx_L1_error)
+      if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 418, __pyx_L1_error)
     }
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
@@ -13417,15 +13509,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":400
+/* "pe/_cy_machine.pyx":402
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
 
@@ -13448,31 +13540,31 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_rpt", 0);
   __pyx_cur_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt *)__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct___rpt(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 400, __pyx_L1_error)
+    __PYX_ERR(0, 402, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
 
-  /* "pe/_cy_machine.pyx":401
+  /* "pe/_cy_machine.pyx":403
  * 
  * def _rpt(defn, mincount):
  *     pis = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     if (len(pis) == 1
  *         and pis[0].opcode == SCAN
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 401, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 403, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -13486,365 +13578,365 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 401, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_cur_scope->__pyx_v_pis = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":402
+  /* "pe/_cy_machine.pyx":404
  * def _rpt(defn, mincount):
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1             # <<<<<<<<<<<<<<
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)
  */
   __pyx_t_1 = __pyx_cur_scope->__pyx_v_pis;
   __Pyx_INCREF(__pyx_t_1);
-  __pyx_t_7 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 402, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_t_1); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 404, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_8 = (__pyx_t_7 == 1);
   if (__pyx_t_8) {
   } else {
     __pyx_t_6 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":403
+  /* "pe/_cy_machine.pyx":405
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  *         and pis[0].opcode == SCAN             # <<<<<<<<<<<<<<
  *         and isinstance(pis[0].scanner, CharacterClass)
  *         and not (pis[0].marking or pis[0].capturing)
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_opcode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_opcode); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_2, __pyx_t_1, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 403, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 405, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (__pyx_t_8) {
   } else {
     __pyx_t_6 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":404
+  /* "pe/_cy_machine.pyx":406
  *     if (len(pis) == 1
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)             # <<<<<<<<<<<<<<
  *         and not (pis[0].marking or pis[0].capturing)
  *         and pis[0].action is None
  */
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 404, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_8 = __Pyx_TypeCheck(__pyx_t_1, __pyx_ptype_2pe_11_cy_machine_CharacterClass); 
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_8) {
   } else {
     __pyx_t_6 = __pyx_t_8;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":405
+  /* "pe/_cy_machine.pyx":407
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)
  *         and not (pis[0].marking or pis[0].capturing)             # <<<<<<<<<<<<<<
  *         and pis[0].action is None
  *     ):
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_marking); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_marking); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_4); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (!__pyx_t_9) {
   } else {
     __pyx_t_8 = __pyx_t_9;
     goto __pyx_L9_bool_binop_done;
   }
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_capturing); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_capturing); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 405, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 407, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_8 = __pyx_t_9;
   __pyx_L9_bool_binop_done:;
   __pyx_t_9 = (!__pyx_t_8);
   if (__pyx_t_9) {
   } else {
     __pyx_t_6 = __pyx_t_9;
     goto __pyx_L4_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":406
+  /* "pe/_cy_machine.pyx":408
  *         and isinstance(pis[0].scanner, CharacterClass)
  *         and not (pis[0].marking or pis[0].capturing)
  *         and pis[0].action is None             # <<<<<<<<<<<<<<
  *     ):
  *         pi = pis[0]
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_action); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 406, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_action); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_9 = (__pyx_t_4 == Py_None);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_6 = __pyx_t_9;
   __pyx_L4_bool_binop_done:;
 
-  /* "pe/_cy_machine.pyx":402
+  /* "pe/_cy_machine.pyx":404
  * def _rpt(defn, mincount):
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1             # <<<<<<<<<<<<<<
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)
  */
   if (__pyx_t_6) {
 
-    /* "pe/_cy_machine.pyx":408
+    /* "pe/_cy_machine.pyx":410
  *         and pis[0].action is None
  *     ):
  *         pi = pis[0]             # <<<<<<<<<<<<<<
  *         pi.scanner.mincount = mincount
  *         pi.scanner.maxcount = -1
  */
-    __pyx_t_4 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 408, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_GetItemInt(__pyx_cur_scope->__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 410, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_v_pi = __pyx_t_4;
     __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":409
+    /* "pe/_cy_machine.pyx":411
  *     ):
  *         pi = pis[0]
  *         pi.scanner.mincount = mincount             # <<<<<<<<<<<<<<
  *         pi.scanner.maxcount = -1
  *         return [Instruction(SCAN,
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 409, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_mincount, __pyx_v_mincount) < 0) __PYX_ERR(0, 409, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_mincount, __pyx_v_mincount) < 0) __PYX_ERR(0, 411, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":410
+    /* "pe/_cy_machine.pyx":412
  *         pi = pis[0]
  *         pi.scanner.mincount = mincount
  *         pi.scanner.maxcount = -1             # <<<<<<<<<<<<<<
  *         return [Instruction(SCAN,
  *                             scanner=pi.scanner,
  */
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 410, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_maxcount, __pyx_int_neg_1) < 0) __PYX_ERR(0, 410, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_t_4, __pyx_n_s_maxcount, __pyx_int_neg_1) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":411
+    /* "pe/_cy_machine.pyx":413
  *         pi.scanner.mincount = mincount
  *         pi.scanner.maxcount = -1
  *         return [Instruction(SCAN,             # <<<<<<<<<<<<<<
  *                             scanner=pi.scanner,
  *                             marking=pi.marking,
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_SCAN); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error);
     __pyx_t_4 = 0;
 
-    /* "pe/_cy_machine.pyx":412
+    /* "pe/_cy_machine.pyx":414
  *         pi.scanner.maxcount = -1
  *         return [Instruction(SCAN,
  *                             scanner=pi.scanner,             # <<<<<<<<<<<<<<
  *                             marking=pi.marking,
  *                             capturing=pi.capturing,
  */
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 412, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_scanner); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scanner, __pyx_t_2) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_scanner, __pyx_t_2) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":413
+    /* "pe/_cy_machine.pyx":415
  *         return [Instruction(SCAN,
  *                             scanner=pi.scanner,
  *                             marking=pi.marking,             # <<<<<<<<<<<<<<
  *                             capturing=pi.capturing,
  *                             action=pi.action)]
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_marking); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_marking); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_marking, __pyx_t_2) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_marking, __pyx_t_2) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":414
+    /* "pe/_cy_machine.pyx":416
  *                             scanner=pi.scanner,
  *                             marking=pi.marking,
  *                             capturing=pi.capturing,             # <<<<<<<<<<<<<<
  *                             action=pi.action)]
  *     return [*(pi.copy() for _ in range(mincount) for pi in pis),
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_capturing); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 414, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_capturing); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_capturing, __pyx_t_2) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_capturing, __pyx_t_2) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":415
+    /* "pe/_cy_machine.pyx":417
  *                             marking=pi.marking,
  *                             capturing=pi.capturing,
  *                             action=pi.action)]             # <<<<<<<<<<<<<<
  *     return [*(pi.copy() for _ in range(mincount) for pi in pis),
  *             Instruction(BRANCH, len(pis) + 2),
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 415, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_action, __pyx_t_2) < 0) __PYX_ERR(0, 412, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_action, __pyx_t_2) < 0) __PYX_ERR(0, 414, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":411
+    /* "pe/_cy_machine.pyx":413
  *         pi.scanner.mincount = mincount
  *         pi.scanner.maxcount = -1
  *         return [Instruction(SCAN,             # <<<<<<<<<<<<<<
  *                             scanner=pi.scanner,
  *                             marking=pi.marking,
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 411, __pyx_L1_error)
+    __pyx_t_4 = PyList_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 413, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_2);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 411, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_2)) __PYX_ERR(0, 413, __pyx_L1_error);
     __pyx_t_2 = 0;
     __pyx_r = __pyx_t_4;
     __pyx_t_4 = 0;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":402
+    /* "pe/_cy_machine.pyx":404
  * def _rpt(defn, mincount):
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1             # <<<<<<<<<<<<<<
  *         and pis[0].opcode == SCAN
  *         and isinstance(pis[0].scanner, CharacterClass)
  */
   }
 
-  /* "pe/_cy_machine.pyx":416
+  /* "pe/_cy_machine.pyx":418
  *                             capturing=pi.capturing,
  *                             action=pi.action)]
  *     return [*(pi.copy() for _ in range(mincount) for pi in pis),             # <<<<<<<<<<<<<<
  *             Instruction(BRANCH, len(pis) + 2),
  *             *pis,
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_mincount); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_range, __pyx_v_mincount); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_4_rpt_genexpr(((PyObject*)__pyx_cur_scope), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_4_rpt_genexpr(((PyObject*)__pyx_cur_scope), __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PySequence_ListKeepNew(__pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 418, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":417
+  /* "pe/_cy_machine.pyx":419
  *                             action=pi.action)]
  *     return [*(pi.copy() for _ in range(mincount) for pi in pis),
  *             Instruction(BRANCH, len(pis) + 2),             # <<<<<<<<<<<<<<
  *             *pis,
  *             Instruction(UPDATE, -len(pis))]
  */
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __pyx_cur_scope->__pyx_v_pis;
   __Pyx_INCREF(__pyx_t_2);
-  __pyx_t_7 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_t_2); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_7 + 2)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_2 = PyInt_FromSsize_t((__pyx_t_7 + 2)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 417, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error);
   __pyx_t_1 = 0;
   __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 417, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_4, __pyx_t_2) < 0) __PYX_ERR(0, 417, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_4, __pyx_t_2) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":418
+  /* "pe/_cy_machine.pyx":420
  *     return [*(pi.copy() for _ in range(mincount) for pi in pis),
  *             Instruction(BRANCH, len(pis) + 2),
  *             *pis,             # <<<<<<<<<<<<<<
  *             Instruction(UPDATE, -len(pis))]
  * 
  */
-  if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_cur_scope->__pyx_v_pis) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_4, __pyx_cur_scope->__pyx_v_pis) < 0) __PYX_ERR(0, 420, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":419
+  /* "pe/_cy_machine.pyx":421
  *             Instruction(BRANCH, len(pis) + 2),
  *             *pis,
  *             Instruction(UPDATE, -len(pis))]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_UPDATE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_UPDATE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_3 = __pyx_cur_scope->__pyx_v_pis;
   __Pyx_INCREF(__pyx_t_3);
-  __pyx_t_7 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_7 = PyObject_Length(__pyx_t_3); if (unlikely(__pyx_t_7 == ((Py_ssize_t)-1))) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyInt_FromSsize_t((-__pyx_t_7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_3 = PyInt_FromSsize_t((-__pyx_t_7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2)) __PYX_ERR(0, 419, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_2)) __PYX_ERR(0, 421, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_3)) __PYX_ERR(0, 421, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 419, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_4, __pyx_t_3) < 0) __PYX_ERR(0, 419, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_4, __pyx_t_3) < 0) __PYX_ERR(0, 421, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_r = __pyx_t_4;
   __pyx_t_4 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":400
+  /* "pe/_cy_machine.pyx":402
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
 
@@ -13861,15 +13953,15 @@
   __Pyx_XDECREF(__pyx_gb_2pe_11_cy_machine_4_rpt_2generator);
   __Pyx_DECREF((PyObject *)__pyx_cur_scope);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":422
+/* "pe/_cy_machine.pyx":424
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
 
@@ -13922,31 +14014,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 422, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 424, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_sym") < 0)) __PYX_ERR(0, 422, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_sym") < 0)) __PYX_ERR(0, 424, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_sym", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 422, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_sym", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 424, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -13977,52 +14069,52 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_sym", 1);
 
-  /* "pe/_cy_machine.pyx":423
+  /* "pe/_cy_machine.pyx":425
  * 
  * def _sym(defn):
  *     return [Instruction(CALL, name=defn.args[0])]             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_1);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 423, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_name, __pyx_t_4) < 0) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 423, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 425, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 423, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 425, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":422
+  /* "pe/_cy_machine.pyx":424
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
 
@@ -14036,15 +14128,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":426
+/* "pe/_cy_machine.pyx":428
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -14097,31 +14189,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 426, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 428, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_and") < 0)) __PYX_ERR(0, 426, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_and") < 0)) __PYX_ERR(0, 428, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_and", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 426, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_and", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 428, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -14155,26 +14247,26 @@
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_and", 1);
 
-  /* "pe/_cy_machine.pyx":427
+  /* "pe/_cy_machine.pyx":429
  * 
  * def _and(defn):
  *     pi = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 427, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 429, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -14188,104 +14280,104 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 427, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 429, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":428
+  /* "pe/_cy_machine.pyx":430
  * def _and(defn):
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),             # <<<<<<<<<<<<<<
  *             *pi,
  *             Instruction(RESTORE, 2),
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 428, __pyx_L1_error)
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 428, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 430, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 430, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 428, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 428, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 430, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":429
+  /* "pe/_cy_machine.pyx":431
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,             # <<<<<<<<<<<<<<
  *             Instruction(RESTORE, 2),
  *             Instruction(FAIL)]
  */
-  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 429, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":430
+  /* "pe/_cy_machine.pyx":432
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  *             Instruction(RESTORE, 2),             # <<<<<<<<<<<<<<
  *             Instruction(FAIL)]
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RESTORE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RESTORE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_3);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error);
   __Pyx_INCREF(__pyx_int_2);
   __Pyx_GIVEREF(__pyx_int_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_int_2)) __PYX_ERR(0, 430, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_int_2)) __PYX_ERR(0, 432, __pyx_L1_error);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 430, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_4, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_3) < 0) __PYX_ERR(0, 430, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_3) < 0) __PYX_ERR(0, 432, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":431
+  /* "pe/_cy_machine.pyx":433
  *             *pi,
  *             Instruction(RESTORE, 2),
  *             Instruction(FAIL)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAIL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAIL); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 431, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_4) < 0) __PYX_ERR(0, 431, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_4) < 0) __PYX_ERR(0, 433, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":426
+  /* "pe/_cy_machine.pyx":428
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -14300,15 +14392,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":434
+/* "pe/_cy_machine.pyx":436
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -14361,31 +14453,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 434, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 436, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_not") < 0)) __PYX_ERR(0, 434, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_not") < 0)) __PYX_ERR(0, 436, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_not", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 434, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_not", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 436, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -14419,26 +14511,26 @@
   int __pyx_t_5;
   Py_ssize_t __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_not", 1);
 
-  /* "pe/_cy_machine.pyx":435
+  /* "pe/_cy_machine.pyx":437
  * 
  * def _not(defn):
  *     pi = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 437, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 437, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 435, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_3, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 437, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_2);
@@ -14452,81 +14544,81 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_t_4};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 435, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 437, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":436
+  /* "pe/_cy_machine.pyx":438
  * def _not(defn):
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),             # <<<<<<<<<<<<<<
  *             *pi,
  *             Instruction(FAILTWICE)]
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_6 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 436, __pyx_L1_error)
-  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_6 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_6 == ((Py_ssize_t)-1))) __PYX_ERR(0, 438, __pyx_L1_error)
+  __pyx_t_4 = PyInt_FromSsize_t((__pyx_t_6 + 2)); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_2);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 436, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 438, __pyx_L1_error);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error);
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error);
   __pyx_t_2 = 0;
   __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 436, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_4);
-  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 436, __pyx_L1_error);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error);
   __pyx_t_4 = 0;
   __pyx_t_1 = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":437
+  /* "pe/_cy_machine.pyx":439
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,             # <<<<<<<<<<<<<<
  *             Instruction(FAILTWICE)]
  * 
  */
-  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 437, __pyx_L1_error)
+  if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 439, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":438
+  /* "pe/_cy_machine.pyx":440
  *     return [Instruction(BRANCH, len(pi) + 2),
  *             *pi,
  *             Instruction(FAILTWICE)]             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAILTWICE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 438, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAILTWICE); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 438, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_4) < 0) __PYX_ERR(0, 438, __pyx_L1_error)
+  if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_4) < 0) __PYX_ERR(0, 440, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":434
+  /* "pe/_cy_machine.pyx":436
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
 
@@ -14541,15 +14633,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":441
+/* "pe/_cy_machine.pyx":443
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
 
@@ -14602,31 +14694,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 441, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 443, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_cap") < 0)) __PYX_ERR(0, 441, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_cap") < 0)) __PYX_ERR(0, 443, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_cap", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 441, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_cap", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 443, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -14666,52 +14758,52 @@
   int __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_cap", 1);
 
-  /* "pe/_cy_machine.pyx":442
+  /* "pe/_cy_machine.pyx":444
  * 
  * def _cap(defn):
  *     captured_choice = defn.args[0].op == Operator.CHC             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if not pis[0].marking:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_op); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_op); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Operator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_Operator); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CHC); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_CHC); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 442, __pyx_L1_error)
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_1, __pyx_t_3, Py_EQ); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_captured_choice = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":443
+  /* "pe/_cy_machine.pyx":445
  * def _cap(defn):
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])             # <<<<<<<<<<<<<<
  *     if not pis[0].marking:
  *         pis[0].marking = True
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 443, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 443, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 445, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 443, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_GetItemInt(__pyx_t_1, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 445, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = NULL;
   __pyx_t_5 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_1 = PyMethod_GET_SELF(__pyx_t_3);
@@ -14725,81 +14817,81 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_1, __pyx_t_4};
     __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 443, __pyx_L1_error)
+    if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 445, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_pis = __pyx_t_2;
   __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":444
+  /* "pe/_cy_machine.pyx":446
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  *     if not pis[0].marking:             # <<<<<<<<<<<<<<
  *         pis[0].marking = True
  *     else:
  */
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 446, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_marking); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_marking); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 446, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 444, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 446, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_7 = (!__pyx_t_6);
   if (__pyx_t_7) {
 
-    /* "pe/_cy_machine.pyx":445
+    /* "pe/_cy_machine.pyx":447
  *     pis = _parsing_instructions(defn.args[0])
  *     if not pis[0].marking:
  *         pis[0].marking = True             # <<<<<<<<<<<<<<
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))
  */
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 445, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_t_3, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 445, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_t_3, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 447, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-    /* "pe/_cy_machine.pyx":444
+    /* "pe/_cy_machine.pyx":446
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  *     if not pis[0].marking:             # <<<<<<<<<<<<<<
  *         pis[0].marking = True
  *     else:
  */
     goto __pyx_L3;
   }
 
-  /* "pe/_cy_machine.pyx":447
+  /* "pe/_cy_machine.pyx":449
  *         pis[0].marking = True
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))             # <<<<<<<<<<<<<<
  *     pi = pis[-1]
  *     if (not pi.capturing
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pis, __pyx_n_s_insert); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_pis, __pyx_n_s_insert); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 447, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 447, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 447, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 449, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 449, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_t_4 = NULL;
     __pyx_t_5 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_2))) {
@@ -14814,172 +14906,172 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_4, __pyx_int_0, __pyx_t_8};
       __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_5, 2+__pyx_t_5);
       __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 447, __pyx_L1_error)
+      if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_L3:;
 
-  /* "pe/_cy_machine.pyx":448
+  /* "pe/_cy_machine.pyx":450
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]             # <<<<<<<<<<<<<<
  *     if (not pi.capturing
  *         and pi.action is None
  */
-  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 448, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 450, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_v_pi = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "pe/_cy_machine.pyx":449
+  /* "pe/_cy_machine.pyx":451
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if (not pi.capturing             # <<<<<<<<<<<<<<
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_capturing); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_capturing); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 449, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_IsTrue(__pyx_t_3); if (unlikely((__pyx_t_6 < 0))) __PYX_ERR(0, 451, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_9 = (!__pyx_t_6);
   if (__pyx_t_9) {
   } else {
     __pyx_t_7 = __pyx_t_9;
     goto __pyx_L5_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":450
+  /* "pe/_cy_machine.pyx":452
  *     pi = pis[-1]
  *     if (not pi.capturing
  *         and pi.action is None             # <<<<<<<<<<<<<<
  *         and pi.opcode not in NO_CAP_OR_ACT
  *         and not captured_choice
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 450, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 452, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __pyx_t_9 = (__pyx_t_3 == Py_None);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   if (__pyx_t_9) {
   } else {
     __pyx_t_7 = __pyx_t_9;
     goto __pyx_L5_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":451
+  /* "pe/_cy_machine.pyx":453
  *     if (not pi.capturing
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT             # <<<<<<<<<<<<<<
  *         and not captured_choice
  *     ):
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_CAP_OR_ACT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 451, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_NO_CAP_OR_ACT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_9 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_t_2, Py_NE)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 451, __pyx_L1_error)
+  __pyx_t_9 = (__Pyx_PySequence_ContainsTF(__pyx_t_3, __pyx_t_2, Py_NE)); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 453, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   if (__pyx_t_9) {
   } else {
     __pyx_t_7 = __pyx_t_9;
     goto __pyx_L5_bool_binop_done;
   }
 
-  /* "pe/_cy_machine.pyx":452
+  /* "pe/_cy_machine.pyx":454
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT
  *         and not captured_choice             # <<<<<<<<<<<<<<
  *     ):
  *         pis[-1].capturing = True
  */
-  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_captured_choice); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 452, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_PyObject_IsTrue(__pyx_v_captured_choice); if (unlikely((__pyx_t_9 < 0))) __PYX_ERR(0, 454, __pyx_L1_error)
   __pyx_t_6 = (!__pyx_t_9);
   __pyx_t_7 = __pyx_t_6;
   __pyx_L5_bool_binop_done:;
 
-  /* "pe/_cy_machine.pyx":449
+  /* "pe/_cy_machine.pyx":451
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if (not pi.capturing             # <<<<<<<<<<<<<<
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT
  */
   if (__pyx_t_7) {
 
-    /* "pe/_cy_machine.pyx":454
+    /* "pe/_cy_machine.pyx":456
  *         and not captured_choice
  *     ):
  *         pis[-1].capturing = True             # <<<<<<<<<<<<<<
  *     else:
  *         pis.append(Instruction(NOOP, capturing=True))
  */
-    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 454, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 456, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (__Pyx_PyObject_SetAttrStr(__pyx_t_2, __pyx_n_s_capturing, Py_True) < 0) __PYX_ERR(0, 454, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_t_2, __pyx_n_s_capturing, Py_True) < 0) __PYX_ERR(0, 456, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "pe/_cy_machine.pyx":449
+    /* "pe/_cy_machine.pyx":451
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if (not pi.capturing             # <<<<<<<<<<<<<<
  *         and pi.action is None
  *         and pi.opcode not in NO_CAP_OR_ACT
  */
     goto __pyx_L4;
   }
 
-  /* "pe/_cy_machine.pyx":456
+  /* "pe/_cy_machine.pyx":458
  *         pis[-1].capturing = True
  *     else:
  *         pis.append(Instruction(NOOP, capturing=True))             # <<<<<<<<<<<<<<
  *     return pis
  * 
  */
   /*else*/ {
-    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 456, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 456, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_2);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 456, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error);
     __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 456, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_capturing, Py_True) < 0) __PYX_ERR(0, 456, __pyx_L1_error)
-    __pyx_t_8 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 456, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_capturing, Py_True) < 0) __PYX_ERR(0, 458, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_8);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Append(__pyx_v_pis, __pyx_t_8); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 456, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Append(__pyx_v_pis, __pyx_t_8); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 458, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   }
   __pyx_L4:;
 
-  /* "pe/_cy_machine.pyx":457
+  /* "pe/_cy_machine.pyx":459
  *     else:
  *         pis.append(Instruction(NOOP, capturing=True))
  *     return pis             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_pis);
   __pyx_r = __pyx_v_pis;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":441
+  /* "pe/_cy_machine.pyx":443
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
 
@@ -14997,15 +15089,15 @@
   __Pyx_XDECREF(__pyx_v_pis);
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":460
+/* "pe/_cy_machine.pyx":462
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
 
@@ -15058,31 +15150,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 460, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 462, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_bnd") < 0)) __PYX_ERR(0, 460, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_bnd") < 0)) __PYX_ERR(0, 462, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_bnd", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 460, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_bnd", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 462, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -15119,36 +15211,36 @@
   PyObject *__pyx_t_9 = NULL;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_bnd", 1);
 
-  /* "pe/_cy_machine.pyx":461
+  /* "pe/_cy_machine.pyx":463
  * 
  * def _bnd(defn):
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_rul); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Rule); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_Rule); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_5, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Bind); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_7, __pyx_n_s_Bind); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_8, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 461, __pyx_L1_error)
+  __pyx_t_9 = __Pyx_GetItemInt(__pyx_t_8, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 463, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_9);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
   __pyx_t_8 = NULL;
   __pyx_t_10 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_7))) {
     __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
@@ -15162,15 +15254,15 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_9};
     __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 461, __pyx_L1_error)
+    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
   }
   __pyx_t_7 = NULL;
   __pyx_t_10 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
@@ -15186,15 +15278,15 @@
   #endif
   {
     PyObject *__pyx_callargs[3] = {__pyx_t_7, __pyx_t_6, __pyx_t_5};
     __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_10, 2+__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 461, __pyx_L1_error)
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_t_4 = NULL;
   __pyx_t_10 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_2))) {
@@ -15209,23 +15301,23 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_t_3};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_2, __pyx_callargs+1-__pyx_t_10, 1+__pyx_t_10);
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 461, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 463, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":460
+  /* "pe/_cy_machine.pyx":462
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
 
@@ -15244,15 +15336,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":464
+/* "pe/_cy_machine.pyx":466
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
 
@@ -15305,31 +15397,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 464, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_seq") < 0)) __PYX_ERR(0, 464, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_seq") < 0)) __PYX_ERR(0, 466, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_seq", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 464, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_seq", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 466, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -15370,104 +15462,104 @@
   Py_ssize_t __pyx_t_9;
   PyObject *(*__pyx_t_10)(PyObject *);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_seq", 1);
 
-  /* "pe/_cy_machine.pyx":465
+  /* "pe/_cy_machine.pyx":467
  * 
  * def _seq(defn):
  *     head = [pi             # <<<<<<<<<<<<<<
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 465, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 467, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
 
-    /* "pe/_cy_machine.pyx":466
+    /* "pe/_cy_machine.pyx":468
  * def _seq(defn):
  *     head = [pi
  *             for d in defn.args[0][:-1]             # <<<<<<<<<<<<<<
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  */
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, -1L, NULL, NULL, &__pyx_slice_, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyObject_GetSlice(__pyx_t_3, 0, -1L, NULL, NULL, &__pyx_slice_, 0, 1, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
       __pyx_t_3 = __pyx_t_2; __Pyx_INCREF(__pyx_t_3);
       __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 466, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 466, __pyx_L5_error)
+      __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 468, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_3);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 466, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 468, __pyx_L5_error)
             #endif
             if (__pyx_t_4 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 466, __pyx_L5_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 468, __pyx_L5_error)
           #else
-          __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L5_error)
+          __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_3);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 466, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 468, __pyx_L5_error)
             #endif
             if (__pyx_t_4 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 466, __pyx_L5_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_4); __Pyx_INCREF(__pyx_t_2); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 468, __pyx_L5_error)
           #else
-          __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 466, __pyx_L5_error)
+          __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_3, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_5(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 466, __pyx_L5_error)
+            else __PYX_ERR(0, 468, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_d, __pyx_t_2);
       __pyx_t_2 = 0;
 
-      /* "pe/_cy_machine.pyx":467
+      /* "pe/_cy_machine.pyx":469
  *     head = [pi
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]             # <<<<<<<<<<<<<<
  *     tail = _parsing_instructions(defn.args[0][-1])
  *     return head + tail
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 467, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 469, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_7)) {
@@ -15479,94 +15571,94 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_8genexpr1__pyx_v_d};
         __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L5_error)
+        if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
       if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
         __pyx_t_6 = __pyx_t_2; __Pyx_INCREF(__pyx_t_6);
         __pyx_t_9 = 0;
         __pyx_t_10 = NULL;
       } else {
-        __pyx_t_9 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 467, __pyx_L5_error)
+        __pyx_t_9 = -1; __pyx_t_6 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 469, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_6);
-        __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 467, __pyx_L5_error)
+        __pyx_t_10 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 469, __pyx_L5_error)
       }
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
       for (;;) {
         if (likely(!__pyx_t_10)) {
           if (likely(PyList_CheckExact(__pyx_t_6))) {
             {
               Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_6);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 467, __pyx_L5_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 469, __pyx_L5_error)
               #endif
               if (__pyx_t_9 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 467, __pyx_L5_error)
+            __pyx_t_2 = PyList_GET_ITEM(__pyx_t_6, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 469, __pyx_L5_error)
             #else
-            __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L5_error)
+            __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L5_error)
             __Pyx_GOTREF(__pyx_t_2);
             #endif
           } else {
             {
               Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_6);
               #if !CYTHON_ASSUME_SAFE_MACROS
-              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 467, __pyx_L5_error)
+              if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 469, __pyx_L5_error)
               #endif
               if (__pyx_t_9 >= __pyx_temp) break;
             }
             #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 467, __pyx_L5_error)
+            __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_6, __pyx_t_9); __Pyx_INCREF(__pyx_t_2); __pyx_t_9++; if (unlikely((0 < 0))) __PYX_ERR(0, 469, __pyx_L5_error)
             #else
-            __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 467, __pyx_L5_error)
+            __pyx_t_2 = __Pyx_PySequence_ITEM(__pyx_t_6, __pyx_t_9); __pyx_t_9++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 469, __pyx_L5_error)
             __Pyx_GOTREF(__pyx_t_2);
             #endif
           }
         } else {
           __pyx_t_2 = __pyx_t_10(__pyx_t_6);
           if (unlikely(!__pyx_t_2)) {
             PyObject* exc_type = PyErr_Occurred();
             if (exc_type) {
               if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-              else __PYX_ERR(0, 467, __pyx_L5_error)
+              else __PYX_ERR(0, 469, __pyx_L5_error)
             }
             break;
           }
           __Pyx_GOTREF(__pyx_t_2);
         }
         __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_pi, __pyx_t_2);
         __pyx_t_2 = 0;
 
-        /* "pe/_cy_machine.pyx":465
+        /* "pe/_cy_machine.pyx":467
  * 
  * def _seq(defn):
  *     head = [pi             # <<<<<<<<<<<<<<
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]
  */
-        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr1__pyx_v_pi))) __PYX_ERR(0, 465, __pyx_L5_error)
+        if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_8genexpr1__pyx_v_pi))) __PYX_ERR(0, 467, __pyx_L5_error)
 
-        /* "pe/_cy_machine.pyx":467
+        /* "pe/_cy_machine.pyx":469
  *     head = [pi
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]             # <<<<<<<<<<<<<<
  *     tail = _parsing_instructions(defn.args[0][-1])
  *     return head + tail
  */
       }
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-      /* "pe/_cy_machine.pyx":466
+      /* "pe/_cy_machine.pyx":468
  * def _seq(defn):
  *     head = [pi
  *             for d in defn.args[0][:-1]             # <<<<<<<<<<<<<<
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  */
     }
@@ -15579,29 +15671,29 @@
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_pi); __pyx_8genexpr1__pyx_v_pi = 0;
     goto __pyx_L1_error;
     __pyx_L12_exit_scope:;
   } /* exit inner scope */
   __pyx_v_head = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":468
+  /* "pe/_cy_machine.pyx":470
  *             for d in defn.args[0][:-1]
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])             # <<<<<<<<<<<<<<
  *     return head + tail
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 468, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 468, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_t_6, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_2, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 468, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_GetItemInt(__pyx_t_2, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 470, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_t_2 = NULL;
   __pyx_t_8 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_3))) {
     __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
@@ -15615,36 +15707,36 @@
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_2, __pyx_t_6};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 468, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 470, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   }
   __pyx_v_tail = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":469
+  /* "pe/_cy_machine.pyx":471
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  *     return head + tail             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyNumber_Add(__pyx_v_head, __pyx_v_tail); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 469, __pyx_L1_error)
+  __pyx_t_1 = PyNumber_Add(__pyx_v_head, __pyx_v_tail); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 471, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":464
+  /* "pe/_cy_machine.pyx":466
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
 
@@ -15663,15 +15755,15 @@
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_d);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":472
+/* "pe/_cy_machine.pyx":474
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
 
@@ -15724,31 +15816,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 472, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 474, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_chc") < 0)) __PYX_ERR(0, 472, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_chc") < 0)) __PYX_ERR(0, 474, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_chc", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 472, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_chc", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 474, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -15788,85 +15880,85 @@
   int __pyx_t_8;
   Py_ssize_t __pyx_t_9;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_chc", 1);
 
-  /* "pe/_cy_machine.pyx":473
+  /* "pe/_cy_machine.pyx":475
  * 
  * def _chc(defn):
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]             # <<<<<<<<<<<<<<
  *     pi = pis[-1]
  *     for _pi in reversed(pis[:-1]):
  */
   { /* enter inner scope */
-    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 473, __pyx_L5_error)
+    __pyx_t_1 = PyList_New(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 473, __pyx_L5_error)
+    __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 475, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L5_error)
+    __pyx_t_3 = __Pyx_GetItemInt(__pyx_t_2, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 475, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     if (likely(PyList_CheckExact(__pyx_t_3)) || PyTuple_CheckExact(__pyx_t_3)) {
       __pyx_t_2 = __pyx_t_3; __Pyx_INCREF(__pyx_t_2);
       __pyx_t_4 = 0;
       __pyx_t_5 = NULL;
     } else {
-      __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 473, __pyx_L5_error)
+      __pyx_t_4 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 475, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_2);
-      __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 473, __pyx_L5_error)
+      __pyx_t_5 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 475, __pyx_L5_error)
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     for (;;) {
       if (likely(!__pyx_t_5)) {
         if (likely(PyList_CheckExact(__pyx_t_2))) {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 473, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 475, __pyx_L5_error)
             #endif
             if (__pyx_t_4 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 473, __pyx_L5_error)
+          __pyx_t_3 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 475, __pyx_L5_error)
           #else
-          __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L5_error)
+          __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 475, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         } else {
           {
             Py_ssize_t __pyx_temp = __Pyx_PyTuple_GET_SIZE(__pyx_t_2);
             #if !CYTHON_ASSUME_SAFE_MACROS
-            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 473, __pyx_L5_error)
+            if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 475, __pyx_L5_error)
             #endif
             if (__pyx_t_4 >= __pyx_temp) break;
           }
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 473, __pyx_L5_error)
+          __pyx_t_3 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_3); __pyx_t_4++; if (unlikely((0 < 0))) __PYX_ERR(0, 475, __pyx_L5_error)
           #else
-          __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L5_error)
+          __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 475, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_3);
           #endif
         }
       } else {
         __pyx_t_3 = __pyx_t_5(__pyx_t_2);
         if (unlikely(!__pyx_t_3)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 473, __pyx_L5_error)
+            else __PYX_ERR(0, 475, __pyx_L5_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_3);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr2__pyx_v_d, __pyx_t_3);
       __pyx_t_3 = 0;
-      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 473, __pyx_L5_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 475, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_6);
       __pyx_t_7 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_6))) {
         __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
         if (likely(__pyx_t_7)) {
@@ -15878,178 +15970,178 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_8genexpr2__pyx_v_d};
         __pyx_t_3 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 473, __pyx_L5_error)
+        if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 475, __pyx_L5_error)
         __Pyx_GOTREF(__pyx_t_3);
         __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       }
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 473, __pyx_L5_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_1, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 475, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_d); __pyx_8genexpr2__pyx_v_d = 0;
     goto __pyx_L9_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_d); __pyx_8genexpr2__pyx_v_d = 0;
     goto __pyx_L1_error;
     __pyx_L9_exit_scope:;
   } /* exit inner scope */
   __pyx_v_pis = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":474
+  /* "pe/_cy_machine.pyx":476
  * def _chc(defn):
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]             # <<<<<<<<<<<<<<
  *     for _pi in reversed(pis[:-1]):
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  */
-  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 474, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt_List(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 1, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 476, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":475
+  /* "pe/_cy_machine.pyx":477
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  *     for _pi in reversed(pis[:-1]):             # <<<<<<<<<<<<<<
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  *               *_pi,
  */
-  __pyx_t_1 = __Pyx_PyList_GetSlice(__pyx_v_pis, 0, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyList_GetSlice(__pyx_v_pis, 0, -1L); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 477, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __pyx_t_1; __Pyx_INCREF(__pyx_t_2);
   __pyx_t_4 = __Pyx_PyList_GET_SIZE(__pyx_t_2);
   #if !CYTHON_ASSUME_SAFE_MACROS
-  if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 475, __pyx_L1_error)
+  if (unlikely((__pyx_t_4 < 0))) __PYX_ERR(0, 477, __pyx_L1_error)
   #endif
   --__pyx_t_4;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   for (;;) {
     if (__pyx_t_4 < 0) break;
     {
       Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_2);
       #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 475, __pyx_L1_error)
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 477, __pyx_L1_error)
       #endif
       if (__pyx_t_4 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4--; if (unlikely((0 < 0))) __PYX_ERR(0, 475, __pyx_L1_error)
+    __pyx_t_1 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_4); __Pyx_INCREF(__pyx_t_1); __pyx_t_4--; if (unlikely((0 < 0))) __PYX_ERR(0, 477, __pyx_L1_error)
     #else
-    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4--; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 475, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PySequence_ITEM(__pyx_t_2, __pyx_t_4); __pyx_t_4--; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 477, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     #endif
     __Pyx_XDECREF_SET(__pyx_v__pi, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pe/_cy_machine.pyx":476
+    /* "pe/_cy_machine.pyx":478
  *     pi = pis[-1]
  *     for _pi in reversed(pis[:-1]):
  *         pi = [Instruction(BRANCH, len(_pi) + 2),             # <<<<<<<<<<<<<<
  *               *_pi,
  *               Instruction(COMMIT, len(pi) + 1),
  */
-    __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_BRANCH); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_9 = PyObject_Length(__pyx_v__pi); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 476, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_9 + 2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_9 = PyObject_Length(__pyx_v__pi); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_9 + 2)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_7 = PyTuple_New(2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3)) __PYX_ERR(0, 476, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 0, __pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_6)) __PYX_ERR(0, 476, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_7, 1, __pyx_t_6)) __PYX_ERR(0, 478, __pyx_L1_error);
     __pyx_t_3 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_7, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 476, __pyx_L1_error)
+    __pyx_t_7 = PyList_New(1); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 478, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_6)) __PYX_ERR(0, 476, __pyx_L1_error);
+    if (__Pyx_PyList_SET_ITEM(__pyx_t_7, 0, __pyx_t_6)) __PYX_ERR(0, 478, __pyx_L1_error);
     __pyx_t_6 = 0;
     __pyx_t_1 = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":477
+    /* "pe/_cy_machine.pyx":479
  *     for _pi in reversed(pis[:-1]):
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  *               *_pi,             # <<<<<<<<<<<<<<
  *               Instruction(COMMIT, len(pi) + 1),
  *               *pi]
  */
-    if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v__pi) < 0) __PYX_ERR(0, 477, __pyx_L1_error)
+    if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v__pi) < 0) __PYX_ERR(0, 479, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":478
+    /* "pe/_cy_machine.pyx":480
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  *               *_pi,
  *               Instruction(COMMIT, len(pi) + 1),             # <<<<<<<<<<<<<<
  *               *pi]
  *     return pi
  */
-    __pyx_t_7 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __pyx_t_9 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 478, __pyx_L1_error)
-    __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_9 + 1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_9 = PyObject_Length(__pyx_v_pi); if (unlikely(__pyx_t_9 == ((Py_ssize_t)-1))) __PYX_ERR(0, 480, __pyx_L1_error)
+    __pyx_t_6 = PyInt_FromSsize_t((__pyx_t_9 + 1)); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 480, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_7);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7)) __PYX_ERR(0, 478, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_7)) __PYX_ERR(0, 480, __pyx_L1_error);
     __Pyx_GIVEREF(__pyx_t_6);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6)) __PYX_ERR(0, 478, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error);
     __pyx_t_7 = 0;
     __pyx_t_6 = 0;
-    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 478, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_3, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 480, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_6) < 0) __PYX_ERR(0, 478, __pyx_L1_error)
+    if (__Pyx_ListComp_Append(__pyx_t_1, __pyx_t_6) < 0) __PYX_ERR(0, 480, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-    /* "pe/_cy_machine.pyx":479
+    /* "pe/_cy_machine.pyx":481
  *               *_pi,
  *               Instruction(COMMIT, len(pi) + 1),
  *               *pi]             # <<<<<<<<<<<<<<
  *     return pi
  * 
  */
-    if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 479, __pyx_L1_error)
+    if (__Pyx_PyList_Extend(__pyx_t_1, __pyx_v_pi) < 0) __PYX_ERR(0, 481, __pyx_L1_error)
     __Pyx_DECREF_SET(__pyx_v_pi, __pyx_t_1);
     __pyx_t_1 = 0;
 
-    /* "pe/_cy_machine.pyx":475
+    /* "pe/_cy_machine.pyx":477
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  *     for _pi in reversed(pis[:-1]):             # <<<<<<<<<<<<<<
  *         pi = [Instruction(BRANCH, len(_pi) + 2),
  *               *_pi,
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":480
+  /* "pe/_cy_machine.pyx":482
  *               Instruction(COMMIT, len(pi) + 1),
  *               *pi]
  *     return pi             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_pi);
   __pyx_r = __pyx_v_pi;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":472
+  /* "pe/_cy_machine.pyx":474
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
 
@@ -16068,15 +16160,15 @@
   __Pyx_XDECREF(__pyx_v__pi);
   __Pyx_XDECREF(__pyx_8genexpr2__pyx_v_d);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":483
+/* "pe/_cy_machine.pyx":485
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
 
@@ -16129,31 +16221,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 483, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 485, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_rul") < 0)) __PYX_ERR(0, 483, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_rul") < 0)) __PYX_ERR(0, 485, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_rul", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 483, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_rul", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 485, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -16195,30 +16287,30 @@
   int __pyx_t_9;
   int __pyx_t_10;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_rul", 1);
 
-  /* "pe/_cy_machine.pyx":484
+  /* "pe/_cy_machine.pyx":486
  * 
  * def _rul(defn):
  *     subdefn, action, _ = defn.args             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(subdefn)
  *     if action is None:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 484, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_args); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 486, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if ((likely(PyTuple_CheckExact(__pyx_t_1))) || (PyList_CheckExact(__pyx_t_1))) {
     PyObject* sequence = __pyx_t_1;
     Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
     if (unlikely(size != 3)) {
       if (size > 3) __Pyx_RaiseTooManyValuesError(3);
       else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-      __PYX_ERR(0, 484, __pyx_L1_error)
+      __PYX_ERR(0, 486, __pyx_L1_error)
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
     if (likely(PyTuple_CheckExact(sequence))) {
       __pyx_t_2 = PyTuple_GET_ITEM(sequence, 0); 
       __pyx_t_3 = PyTuple_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyTuple_GET_ITEM(sequence, 2); 
     } else {
@@ -16226,60 +16318,60 @@
       __pyx_t_3 = PyList_GET_ITEM(sequence, 1); 
       __pyx_t_4 = PyList_GET_ITEM(sequence, 2); 
     }
     __Pyx_INCREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_INCREF(__pyx_t_4);
     #else
-    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_2 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_3 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_4 = PySequence_ITEM(sequence, 2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     #endif
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   } else {
     Py_ssize_t index = -1;
-    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 484, __pyx_L1_error)
+    __pyx_t_5 = PyObject_GetIter(__pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 486, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_5);
     index = 0; __pyx_t_2 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_2)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_2);
     index = 1; __pyx_t_3 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_3)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_3);
     index = 2; __pyx_t_4 = __pyx_t_6(__pyx_t_5); if (unlikely(!__pyx_t_4)) goto __pyx_L3_unpacking_failed;
     __Pyx_GOTREF(__pyx_t_4);
-    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 484, __pyx_L1_error)
+    if (__Pyx_IternextUnpackEndCheck(__pyx_t_6(__pyx_t_5), 3) < 0) __PYX_ERR(0, 486, __pyx_L1_error)
     __pyx_t_6 = NULL;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     goto __pyx_L4_unpacking_done;
     __pyx_L3_unpacking_failed:;
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     __pyx_t_6 = NULL;
     if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-    __PYX_ERR(0, 484, __pyx_L1_error)
+    __PYX_ERR(0, 486, __pyx_L1_error)
     __pyx_L4_unpacking_done:;
   }
   __pyx_v_subdefn = __pyx_t_2;
   __pyx_t_2 = 0;
   __pyx_v_action = __pyx_t_3;
   __pyx_t_3 = 0;
   __pyx_v__ = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":485
+  /* "pe/_cy_machine.pyx":487
  * def _rul(defn):
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)             # <<<<<<<<<<<<<<
  *     if action is None:
  *         return pis
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 485, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_parsing_instructions); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 487, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_3 = NULL;
   __pyx_t_7 = 0;
   #if CYTHON_UNPACK_METHODS
   if (unlikely(PyMethod_Check(__pyx_t_4))) {
     __pyx_t_3 = PyMethod_GET_SELF(__pyx_t_4);
     if (likely(__pyx_t_3)) {
@@ -16291,118 +16383,118 @@
     }
   }
   #endif
   {
     PyObject *__pyx_callargs[2] = {__pyx_t_3, __pyx_v_subdefn};
     __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 485, __pyx_L1_error)
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 487, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   }
   __pyx_v_pis = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":486
+  /* "pe/_cy_machine.pyx":488
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  *     if action is None:             # <<<<<<<<<<<<<<
  *         return pis
  *     pi = pis[0]
  */
   __pyx_t_8 = (__pyx_v_action == Py_None);
   if (__pyx_t_8) {
 
-    /* "pe/_cy_machine.pyx":487
+    /* "pe/_cy_machine.pyx":489
  *     pis = _parsing_instructions(subdefn)
  *     if action is None:
  *         return pis             # <<<<<<<<<<<<<<
  *     pi = pis[0]
  *     if not pi.marking:
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_v_pis);
     __pyx_r = __pyx_v_pis;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":486
+    /* "pe/_cy_machine.pyx":488
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  *     if action is None:             # <<<<<<<<<<<<<<
  *         return pis
  *     pi = pis[0]
  */
   }
 
-  /* "pe/_cy_machine.pyx":488
+  /* "pe/_cy_machine.pyx":490
  *     if action is None:
  *         return pis
  *     pi = pis[0]             # <<<<<<<<<<<<<<
  *     if not pi.marking:
  *         pi.marking = True
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 488, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 490, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_pi = __pyx_t_1;
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":489
+  /* "pe/_cy_machine.pyx":491
  *         return pis
  *     pi = pis[0]
  *     if not pi.marking:             # <<<<<<<<<<<<<<
  *         pi.marking = True
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_marking); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_marking); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 489, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_1); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 491, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_9 = (!__pyx_t_8);
   if (__pyx_t_9) {
 
-    /* "pe/_cy_machine.pyx":490
+    /* "pe/_cy_machine.pyx":492
  *     pi = pis[0]
  *     if not pi.marking:
  *         pi.marking = True             # <<<<<<<<<<<<<<
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 490, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 492, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":489
+    /* "pe/_cy_machine.pyx":491
  *         return pis
  *     pi = pis[0]
  *     if not pi.marking:             # <<<<<<<<<<<<<<
  *         pi.marking = True
  *     else:
  */
     goto __pyx_L6;
   }
 
-  /* "pe/_cy_machine.pyx":492
+  /* "pe/_cy_machine.pyx":494
  *         pi.marking = True
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))             # <<<<<<<<<<<<<<
  *     pi = pis[-1]
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pis, __pyx_n_s_insert); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_v_pis, __pyx_n_s_insert); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_GIVEREF(__pyx_t_3);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error);
     __pyx_t_3 = 0;
-    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 492, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 492, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 492, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_marking, Py_True) < 0) __PYX_ERR(0, 494, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 494, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_t_3 = NULL;
     __pyx_t_7 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_4))) {
@@ -16417,120 +16509,120 @@
     }
     #endif
     {
       PyObject *__pyx_callargs[3] = {__pyx_t_3, __pyx_int_0, __pyx_t_5};
       __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_4, __pyx_callargs+1-__pyx_t_7, 2+__pyx_t_7);
       __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 492, __pyx_L1_error)
+      if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     }
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
   __pyx_L6:;
 
-  /* "pe/_cy_machine.pyx":493
+  /* "pe/_cy_machine.pyx":495
  *     else:
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]             # <<<<<<<<<<<<<<
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:
  *         pi.action = action
  */
-  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 493, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_GetItemInt(__pyx_v_pis, -1L, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 495, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF_SET(__pyx_v_pi, __pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":494
+  /* "pe/_cy_machine.pyx":496
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:             # <<<<<<<<<<<<<<
  *         pi.action = action
  *     else:
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_action); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_8 = (__pyx_t_1 == Py_None);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_8) {
   } else {
     __pyx_t_9 = __pyx_t_8;
     goto __pyx_L8_bool_binop_done;
   }
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_pi, __pyx_n_s_opcode); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_NO_CAP_OR_ACT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 494, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_NO_CAP_OR_ACT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_8 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_4, Py_NE)); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 494, __pyx_L1_error)
+  __pyx_t_8 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_t_4, Py_NE)); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 496, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_9 = __pyx_t_8;
   __pyx_L8_bool_binop_done:;
   if (__pyx_t_9) {
 
-    /* "pe/_cy_machine.pyx":495
+    /* "pe/_cy_machine.pyx":497
  *     pi = pis[-1]
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:
  *         pi.action = action             # <<<<<<<<<<<<<<
  *     else:
  *         pis.append(Instruction(NOOP, action=action))
  */
-    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_action, __pyx_v_action) < 0) __PYX_ERR(0, 495, __pyx_L1_error)
+    if (__Pyx_PyObject_SetAttrStr(__pyx_v_pi, __pyx_n_s_action, __pyx_v_action) < 0) __PYX_ERR(0, 497, __pyx_L1_error)
 
-    /* "pe/_cy_machine.pyx":494
+    /* "pe/_cy_machine.pyx":496
  *         pis.insert(0, Instruction(NOOP, marking=True))
  *     pi = pis[-1]
  *     if pi.action is None and pi.opcode not in NO_CAP_OR_ACT:             # <<<<<<<<<<<<<<
  *         pi.action = action
  *     else:
  */
     goto __pyx_L7;
   }
 
-  /* "pe/_cy_machine.pyx":497
+  /* "pe/_cy_machine.pyx":499
  *         pi.action = action
  *     else:
  *         pis.append(Instruction(NOOP, action=action))             # <<<<<<<<<<<<<<
  *     return pis
  * 
  */
   /*else*/ {
-    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_NOOP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 499, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 499, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_4);
-    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error);
+    if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4)) __PYX_ERR(0, 499, __pyx_L1_error);
     __pyx_t_4 = 0;
-    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 499, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_action, __pyx_v_action) < 0) __PYX_ERR(0, 497, __pyx_L1_error)
-    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 497, __pyx_L1_error)
+    if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_action, __pyx_v_action) < 0) __PYX_ERR(0, 499, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_2pe_11_cy_machine_Instruction), __pyx_t_1, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 499, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __pyx_t_10 = __Pyx_PyObject_Append(__pyx_v_pis, __pyx_t_5); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 497, __pyx_L1_error)
+    __pyx_t_10 = __Pyx_PyObject_Append(__pyx_v_pis, __pyx_t_5); if (unlikely(__pyx_t_10 == ((int)-1))) __PYX_ERR(0, 499, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   }
   __pyx_L7:;
 
-  /* "pe/_cy_machine.pyx":498
+  /* "pe/_cy_machine.pyx":500
  *     else:
  *         pis.append(Instruction(NOOP, action=action))
  *     return pis             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_pis);
   __pyx_r = __pyx_v_pis;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":483
+  /* "pe/_cy_machine.pyx":485
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
 
@@ -16550,15 +16642,15 @@
   __Pyx_XDECREF(__pyx_v_pis);
   __Pyx_XDECREF(__pyx_v_pi);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":520
+/* "pe/_cy_machine.pyx":522
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
 
@@ -16611,31 +16703,31 @@
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_defn)) != 0)) {
           (void)__Pyx_Arg_NewRef_FASTCALL(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 520, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 522, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_parsing_instructions") < 0)) __PYX_ERR(0, 520, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "_parsing_instructions") < 0)) __PYX_ERR(0, 522, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
     }
     __pyx_v_defn = values[0];
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("_parsing_instructions", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 520, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("_parsing_instructions", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 522, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_FASTCALL(values[__pyx_temp]);
@@ -16673,15 +16765,15 @@
   PyObject *__pyx_t_10 = NULL;
   PyObject *__pyx_t_11 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_parsing_instructions", 1);
 
-  /* "pe/_cy_machine.pyx":521
+  /* "pe/_cy_machine.pyx":523
  * 
  * def _parsing_instructions(defn):  # noqa: C901
  *     try:             # <<<<<<<<<<<<<<
  *         return _op_map[defn.op](defn)
  *     except KeyError:
  */
   {
@@ -16689,27 +16781,27 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "pe/_cy_machine.pyx":522
+      /* "pe/_cy_machine.pyx":524
  * def _parsing_instructions(defn):  # noqa: C901
  *     try:
  *         return _op_map[defn.op](defn)             # <<<<<<<<<<<<<<
  *     except KeyError:
  *         raise Error(f'invalid definition: {defn!r}')
  */
       __Pyx_XDECREF(__pyx_r);
-      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_op_map); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 522, __pyx_L3_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_op_map); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 524, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_5);
-      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_op); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 522, __pyx_L3_error)
+      __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_v_defn, __pyx_n_s_op); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 524, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_6);
-      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 522, __pyx_L3_error)
+      __pyx_t_7 = __Pyx_PyObject_GetItem(__pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 524, __pyx_L3_error)
       __Pyx_GOTREF(__pyx_t_7);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_6 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_7))) {
@@ -16723,63 +16815,63 @@
         }
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_6, __pyx_v_defn};
         __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
-        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 522, __pyx_L3_error)
+        if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 524, __pyx_L3_error)
         __Pyx_GOTREF(__pyx_t_4);
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
       }
       __pyx_r = __pyx_t_4;
       __pyx_t_4 = 0;
       goto __pyx_L7_try_return;
 
-      /* "pe/_cy_machine.pyx":521
+      /* "pe/_cy_machine.pyx":523
  * 
  * def _parsing_instructions(defn):  # noqa: C901
  *     try:             # <<<<<<<<<<<<<<
  *         return _op_map[defn.op](defn)
  *     except KeyError:
  */
     }
     __pyx_L3_error:;
     __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
     __Pyx_XDECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "pe/_cy_machine.pyx":523
+    /* "pe/_cy_machine.pyx":525
  *     try:
  *         return _op_map[defn.op](defn)
  *     except KeyError:             # <<<<<<<<<<<<<<
  *         raise Error(f'invalid definition: {defn!r}')
  * 
  */
     __pyx_t_8 = __Pyx_PyErr_ExceptionMatches(__pyx_builtin_KeyError);
     if (__pyx_t_8) {
       __Pyx_AddTraceback("pe._cy_machine._parsing_instructions", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_7, &__pyx_t_6) < 0) __PYX_ERR(0, 523, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_4, &__pyx_t_7, &__pyx_t_6) < 0) __PYX_ERR(0, 525, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_4);
       __Pyx_XGOTREF(__pyx_t_7);
       __Pyx_XGOTREF(__pyx_t_6);
 
-      /* "pe/_cy_machine.pyx":524
+      /* "pe/_cy_machine.pyx":526
  *         return _op_map[defn.op](defn)
  *     except KeyError:
  *         raise Error(f'invalid definition: {defn!r}')             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Error); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 524, __pyx_L5_except_error)
+      __Pyx_GetModuleGlobalName(__pyx_t_9, __pyx_n_s_Error); if (unlikely(!__pyx_t_9)) __PYX_ERR(0, 526, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_9);
-      __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_v_defn), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 524, __pyx_L5_except_error)
+      __pyx_t_10 = __Pyx_PyObject_FormatSimpleAndDecref(PyObject_Repr(__pyx_v_defn), __pyx_empty_unicode); if (unlikely(!__pyx_t_10)) __PYX_ERR(0, 526, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_10);
-      __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_definition, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 524, __pyx_L5_except_error)
+      __pyx_t_11 = __Pyx_PyUnicode_Concat(__pyx_kp_u_invalid_definition, __pyx_t_10); if (unlikely(!__pyx_t_11)) __PYX_ERR(0, 526, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_11);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __pyx_t_10 = NULL;
       __pyx_t_8 = 0;
       #if CYTHON_UNPACK_METHODS
       if (unlikely(PyMethod_Check(__pyx_t_9))) {
         __pyx_t_10 = PyMethod_GET_SELF(__pyx_t_9);
@@ -16793,25 +16885,25 @@
       }
       #endif
       {
         PyObject *__pyx_callargs[2] = {__pyx_t_10, __pyx_t_11};
         __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_9, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
         __Pyx_XDECREF(__pyx_t_10); __pyx_t_10 = 0;
         __Pyx_DECREF(__pyx_t_11); __pyx_t_11 = 0;
-        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 524, __pyx_L5_except_error)
+        if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 526, __pyx_L5_except_error)
         __Pyx_GOTREF(__pyx_t_5);
         __Pyx_DECREF(__pyx_t_9); __pyx_t_9 = 0;
       }
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-      __PYX_ERR(0, 524, __pyx_L5_except_error)
+      __PYX_ERR(0, 526, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "pe/_cy_machine.pyx":521
+    /* "pe/_cy_machine.pyx":523
  * 
  * def _parsing_instructions(defn):  # noqa: C901
  *     try:             # <<<<<<<<<<<<<<
  *         return _op_map[defn.op](defn)
  *     except KeyError:
  */
     __pyx_L5_except_error:;
@@ -16824,15 +16916,15 @@
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L0;
   }
 
-  /* "pe/_cy_machine.pyx":520
+  /* "pe/_cy_machine.pyx":522
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
 
@@ -16849,15 +16941,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":530
+/* "pe/_cy_machine.pyx":532
  * 
  * cdef class Dot(Scanner):
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         if pos < slen:
  *             return pos + 1
  */
 
@@ -16868,58 +16960,58 @@
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_scan", 1);
 
-  /* "pe/_cy_machine.pyx":531
+  /* "pe/_cy_machine.pyx":533
  * cdef class Dot(Scanner):
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:             # <<<<<<<<<<<<<<
  *             return pos + 1
  *         return FAILURE
  */
   __pyx_t_1 = (__pyx_v_pos < __pyx_v_slen);
   if (__pyx_t_1) {
 
-    /* "pe/_cy_machine.pyx":532
+    /* "pe/_cy_machine.pyx":534
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:
  *             return pos + 1             # <<<<<<<<<<<<<<
  *         return FAILURE
  * 
  */
     __pyx_r = (__pyx_v_pos + 1);
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":531
+    /* "pe/_cy_machine.pyx":533
  * cdef class Dot(Scanner):
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         if pos < slen:             # <<<<<<<<<<<<<<
  *             return pos + 1
  *         return FAILURE
  */
   }
 
-  /* "pe/_cy_machine.pyx":533
+  /* "pe/_cy_machine.pyx":535
  *         if pos < slen:
  *             return pos + 1
  *         return FAILURE             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 533, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 533, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_2); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 535, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_r = __pyx_t_3;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":530
+  /* "pe/_cy_machine.pyx":532
  * 
  * cdef class Dot(Scanner):
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         if pos < slen:
  *             return pos + 1
  */
 
@@ -17324,15 +17416,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":540
+/* "pe/_cy_machine.pyx":542
  *     cdef int _xlen
  * 
  *     def __init__(self, str x):             # <<<<<<<<<<<<<<
  *         self._x = x
  *         self._xlen = len(x)
  */
 
@@ -17368,45 +17460,45 @@
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 540, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 542, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 540, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 542, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_x = ((PyObject*)values[0]);
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 540, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 542, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pe._cy_machine.Literal.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_x), (&PyUnicode_Type), 1, "x", 1))) __PYX_ERR(0, 540, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_x), (&PyUnicode_Type), 1, "x", 1))) __PYX_ERR(0, 542, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_7Literal___init__(((struct __pyx_obj_2pe_11_cy_machine_Literal *)__pyx_v_self), __pyx_v_x);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -17425,42 +17517,42 @@
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "pe/_cy_machine.pyx":541
+  /* "pe/_cy_machine.pyx":543
  * 
  *     def __init__(self, str x):
  *         self._x = x             # <<<<<<<<<<<<<<
  *         self._xlen = len(x)
  * 
  */
   __Pyx_INCREF(__pyx_v_x);
   __Pyx_GIVEREF(__pyx_v_x);
   __Pyx_GOTREF(__pyx_v_self->_x);
   __Pyx_DECREF(__pyx_v_self->_x);
   __pyx_v_self->_x = __pyx_v_x;
 
-  /* "pe/_cy_machine.pyx":542
+  /* "pe/_cy_machine.pyx":544
  *     def __init__(self, str x):
  *         self._x = x
  *         self._xlen = len(x)             # <<<<<<<<<<<<<<
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  */
   if (unlikely(__pyx_v_x == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 542, __pyx_L1_error)
+    __PYX_ERR(0, 544, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_x); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 542, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_GET_LENGTH(__pyx_v_x); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 544, __pyx_L1_error)
   __pyx_v_self->_xlen = __pyx_t_1;
 
-  /* "pe/_cy_machine.pyx":540
+  /* "pe/_cy_machine.pyx":542
  *     cdef int _xlen
  * 
  *     def __init__(self, str x):             # <<<<<<<<<<<<<<
  *         self._x = x
  *         self._xlen = len(x)
  */
 
@@ -17471,15 +17563,15 @@
   __Pyx_AddTraceback("pe._cy_machine.Literal.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":544
+/* "pe/_cy_machine.pyx":546
  *         self._xlen = len(x)
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:
  */
 
@@ -17491,74 +17583,74 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_scan", 1);
 
-  /* "pe/_cy_machine.pyx":545
+  /* "pe/_cy_machine.pyx":547
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         cdef int end = pos + self._xlen             # <<<<<<<<<<<<<<
  *         if s[pos:end] != self._x:
  *             return FAILURE
  */
   __pyx_v_end = (__pyx_v_pos + __pyx_v_self->_xlen);
 
-  /* "pe/_cy_machine.pyx":546
+  /* "pe/_cy_machine.pyx":548
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         return end
  */
   if (unlikely(__pyx_v_s == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(0, 546, __pyx_L1_error)
+    __PYX_ERR(0, 548, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_v_s, __pyx_v_pos, __pyx_v_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyUnicode_Substring(__pyx_v_s, __pyx_v_pos, __pyx_v_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_v_self->_x, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 546, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PyUnicode_Equals(__pyx_t_1, __pyx_v_self->_x, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(0, 548, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   if (__pyx_t_2) {
 
-    /* "pe/_cy_machine.pyx":547
+    /* "pe/_cy_machine.pyx":549
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:
  *             return FAILURE             # <<<<<<<<<<<<<<
  *         return end
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 547, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 549, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 547, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_3 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 549, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_r = __pyx_t_3;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":546
+    /* "pe/_cy_machine.pyx":548
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         return end
  */
   }
 
-  /* "pe/_cy_machine.pyx":548
+  /* "pe/_cy_machine.pyx":550
  *         if s[pos:end] != self._x:
  *             return FAILURE
  *         return end             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_end;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":544
+  /* "pe/_cy_machine.pyx":546
  *         self._xlen = len(x)
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         cdef int end = pos + self._xlen
  *         if s[pos:end] != self._x:
  */
 
@@ -17974,15 +18066,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":559
+/* "pe/_cy_machine.pyx":561
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 
@@ -18027,41 +18119,41 @@
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_ranges)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 559, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_negate);
           if (value) { values[1] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 559, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_mincount);
           if (value) { values[2] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 559, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_maxcount);
           if (value) { values[3] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 559, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 561, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 559, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 561, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  4: values[3] = __Pyx_Arg_VARARGS(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_VARARGS(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
@@ -18070,57 +18162,57 @@
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_ranges = ((PyObject*)values[0]);
     if (values[1]) {
-      __pyx_v_negate = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_negate == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 562, __pyx_L3_error)
+      __pyx_v_negate = __Pyx_PyObject_IsTrue(values[1]); if (unlikely((__pyx_v_negate == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 564, __pyx_L3_error)
     } else {
 
-      /* "pe/_cy_machine.pyx":562
+      /* "pe/_cy_machine.pyx":564
  *         self,
  *         list ranges,
  *         bint negate = False,             # <<<<<<<<<<<<<<
  *         int mincount = 1,
  *         int maxcount = 1
  */
       __pyx_v_negate = ((int)0);
     }
     if (values[2]) {
-      __pyx_v_mincount = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_mincount == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 563, __pyx_L3_error)
+      __pyx_v_mincount = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_mincount == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 565, __pyx_L3_error)
     } else {
       __pyx_v_mincount = ((int)1);
     }
     if (values[3]) {
-      __pyx_v_maxcount = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_maxcount == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 564, __pyx_L3_error)
+      __pyx_v_maxcount = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_maxcount == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 566, __pyx_L3_error)
     } else {
       __pyx_v_maxcount = ((int)1);
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 4, __pyx_nargs); __PYX_ERR(0, 559, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 4, __pyx_nargs); __PYX_ERR(0, 561, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pe._cy_machine.CharacterClass.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ranges), (&PyList_Type), 1, "ranges", 1))) __PYX_ERR(0, 561, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_ranges), (&PyList_Type), 1, "ranges", 1))) __PYX_ERR(0, 563, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_14CharacterClass___init__(((struct __pyx_obj_2pe_11_cy_machine_CharacterClass *)__pyx_v_self), __pyx_v_ranges, __pyx_v_negate, __pyx_v_mincount, __pyx_v_maxcount);
 
-  /* "pe/_cy_machine.pyx":559
+  /* "pe/_cy_machine.pyx":561
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 
@@ -18136,15 +18228,15 @@
     }
   }
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___2generator1(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pe/_cy_machine.pyx":566
+/* "pe/_cy_machine.pyx":568
  *         int maxcount = 1
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)             # <<<<<<<<<<<<<<
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)
  */
 
@@ -18156,23 +18248,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr *)__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_2_genexpr(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 566, __pyx_L1_error)
+    __PYX_ERR(0, 568, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___2generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_init___locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___2generator1, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_init___locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 568, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -18205,96 +18297,96 @@
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 566, __pyx_L1_error)
-  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 566, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_r);
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 566, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 568, __pyx_L1_error) }
   if (unlikely(__pyx_cur_scope->__pyx_genexpr_arg_0 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 566, __pyx_L1_error)
+    __PYX_ERR(0, 568, __pyx_L1_error)
   }
   __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = 0;
   for (;;) {
     {
       Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
       #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 566, __pyx_L1_error)
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 568, __pyx_L1_error)
       #endif
       if (__pyx_t_2 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 568, __pyx_L1_error)
     #else
-    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 568, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 566, __pyx_L1_error)
+        __PYX_ERR(0, 568, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       #else
-      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 566, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 568, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 566, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 568, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 566, __pyx_L1_error)
+      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 568, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6);
       index = 0; __pyx_t_4 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_4)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
       index = 1; __pyx_t_5 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_5)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 566, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 568, __pyx_L1_error)
       __pyx_t_7 = NULL;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L7_unpacking_done;
       __pyx_L6_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 566, __pyx_L1_error)
+      __PYX_ERR(0, 568, __pyx_L1_error)
       __pyx_L7_unpacking_done:;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_a);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_a, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_b);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_b, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_b); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 566, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_b); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 568, __pyx_L1_error)
     __pyx_t_9 = (!__pyx_t_8);
     if (__pyx_t_9) {
-      if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_cur_scope->__pyx_v_a))) __PYX_ERR(0, 566, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_cur_scope->__pyx_v_a))) __PYX_ERR(0, 568, __pyx_L1_error)
     }
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
   goto __pyx_L0;
@@ -18315,15 +18407,15 @@
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 static PyObject *__pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___5generator2(__pyx_CoroutineObject *__pyx_generator, CYTHON_UNUSED PyThreadState *__pyx_tstate, PyObject *__pyx_sent_value); /* proto */
 
-/* "pe/_cy_machine.pyx":567
+/* "pe/_cy_machine.pyx":569
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)
  *         self._ranges = ''.join(a+b for a, b in ranges if b)             # <<<<<<<<<<<<<<
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate
  */
 
@@ -18335,23 +18427,23 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("genexpr", 0);
   __pyx_cur_scope = (struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_3_genexpr *)__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_3_genexpr(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr, __pyx_empty_tuple, NULL);
   if (unlikely(!__pyx_cur_scope)) {
     __pyx_cur_scope = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_3_genexpr *)Py_None);
     __Pyx_INCREF(Py_None);
-    __PYX_ERR(0, 567, __pyx_L1_error)
+    __PYX_ERR(0, 569, __pyx_L1_error)
   } else {
     __Pyx_GOTREF((PyObject *)__pyx_cur_scope);
   }
   __pyx_cur_scope->__pyx_genexpr_arg_0 = __pyx_genexpr_arg_0;
   __Pyx_INCREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   __Pyx_GIVEREF(__pyx_cur_scope->__pyx_genexpr_arg_0);
   {
-    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___5generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_init___locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_CoroutineObject *gen = __Pyx_Generator_New((__pyx_coroutine_body_t) __pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___5generator2, NULL, (PyObject *) __pyx_cur_scope, __pyx_n_s_genexpr, __pyx_n_s_init___locals_genexpr, __pyx_n_s_pe__cy_machine); if (unlikely(!gen)) __PYX_ERR(0, 569, __pyx_L1_error)
     __Pyx_DECREF(__pyx_cur_scope);
     __Pyx_RefNannyFinishContext();
     return (PyObject *) gen;
   }
 
   /* function exit code */
   __pyx_L1_error:;
@@ -18383,97 +18475,97 @@
   switch (__pyx_generator->resume_label) {
     case 0: goto __pyx_L3_first_run;
     default: /* CPython raises the right error here */
     __Pyx_RefNannyFinishContext();
     return NULL;
   }
   __pyx_L3_first_run:;
-  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 567, __pyx_L1_error)
-  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 567, __pyx_L1_error)
+  if (unlikely(!__pyx_sent_value)) __PYX_ERR(0, 569, __pyx_L1_error)
+  __pyx_r = PyList_New(0); if (unlikely(!__pyx_r)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_r);
-  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 567, __pyx_L1_error) }
+  if (unlikely(!__pyx_cur_scope->__pyx_genexpr_arg_0)) { __Pyx_RaiseUnboundLocalError(".0"); __PYX_ERR(0, 569, __pyx_L1_error) }
   if (unlikely(__pyx_cur_scope->__pyx_genexpr_arg_0 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-    __PYX_ERR(0, 567, __pyx_L1_error)
+    __PYX_ERR(0, 569, __pyx_L1_error)
   }
   __pyx_t_1 = __pyx_cur_scope->__pyx_genexpr_arg_0; __Pyx_INCREF(__pyx_t_1);
   __pyx_t_2 = 0;
   for (;;) {
     {
       Py_ssize_t __pyx_temp = __Pyx_PyList_GET_SIZE(__pyx_t_1);
       #if !CYTHON_ASSUME_SAFE_MACROS
-      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 567, __pyx_L1_error)
+      if (unlikely((__pyx_temp < 0))) __PYX_ERR(0, 569, __pyx_L1_error)
       #endif
       if (__pyx_t_2 >= __pyx_temp) break;
     }
     #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_3 = PyList_GET_ITEM(__pyx_t_1, __pyx_t_2); __Pyx_INCREF(__pyx_t_3); __pyx_t_2++; if (unlikely((0 < 0))) __PYX_ERR(0, 569, __pyx_L1_error)
     #else
-    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PySequence_ITEM(__pyx_t_1, __pyx_t_2); __pyx_t_2++; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     #endif
     if ((likely(PyTuple_CheckExact(__pyx_t_3))) || (PyList_CheckExact(__pyx_t_3))) {
       PyObject* sequence = __pyx_t_3;
       Py_ssize_t size = __Pyx_PySequence_SIZE(sequence);
       if (unlikely(size != 2)) {
         if (size > 2) __Pyx_RaiseTooManyValuesError(2);
         else if (size >= 0) __Pyx_RaiseNeedMoreValuesError(size);
-        __PYX_ERR(0, 567, __pyx_L1_error)
+        __PYX_ERR(0, 569, __pyx_L1_error)
       }
       #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
       if (likely(PyTuple_CheckExact(sequence))) {
         __pyx_t_4 = PyTuple_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyTuple_GET_ITEM(sequence, 1); 
       } else {
         __pyx_t_4 = PyList_GET_ITEM(sequence, 0); 
         __pyx_t_5 = PyList_GET_ITEM(sequence, 1); 
       }
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(__pyx_t_5);
       #else
-      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 567, __pyx_L1_error)
+      __pyx_t_4 = PySequence_ITEM(sequence, 0); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 569, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 567, __pyx_L1_error)
+      __pyx_t_5 = PySequence_ITEM(sequence, 1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 569, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       #endif
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     } else {
       Py_ssize_t index = -1;
-      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 567, __pyx_L1_error)
+      __pyx_t_6 = PyObject_GetIter(__pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 569, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
       __pyx_t_7 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_6);
       index = 0; __pyx_t_4 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_4)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_4);
       index = 1; __pyx_t_5 = __pyx_t_7(__pyx_t_6); if (unlikely(!__pyx_t_5)) goto __pyx_L6_unpacking_failed;
       __Pyx_GOTREF(__pyx_t_5);
-      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
+      if (__Pyx_IternextUnpackEndCheck(__pyx_t_7(__pyx_t_6), 2) < 0) __PYX_ERR(0, 569, __pyx_L1_error)
       __pyx_t_7 = NULL;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       goto __pyx_L7_unpacking_done;
       __pyx_L6_unpacking_failed:;
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __pyx_t_7 = NULL;
       if (__Pyx_IterFinish() == 0) __Pyx_RaiseNeedMoreValuesError(index);
-      __PYX_ERR(0, 567, __pyx_L1_error)
+      __PYX_ERR(0, 569, __pyx_L1_error)
       __pyx_L7_unpacking_done:;
     }
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_a);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_a, __pyx_t_4);
     __Pyx_GIVEREF(__pyx_t_4);
     __pyx_t_4 = 0;
     __Pyx_XGOTREF(__pyx_cur_scope->__pyx_v_b);
     __Pyx_XDECREF_SET(__pyx_cur_scope->__pyx_v_b, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_5);
     __pyx_t_5 = 0;
-    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_b); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 567, __pyx_L1_error)
+    __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_cur_scope->__pyx_v_b); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(0, 569, __pyx_L1_error)
     if (__pyx_t_8) {
-      __pyx_t_3 = PyNumber_Add(__pyx_cur_scope->__pyx_v_a, __pyx_cur_scope->__pyx_v_b); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 567, __pyx_L1_error)
+      __pyx_t_3 = PyNumber_Add(__pyx_cur_scope->__pyx_v_a, __pyx_cur_scope->__pyx_v_b); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 569, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_3);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 567, __pyx_L1_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_r, (PyObject*)__pyx_t_3))) __PYX_ERR(0, 569, __pyx_L1_error)
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   CYTHON_MAYBE_UNUSED_VAR(__pyx_cur_scope);
 
   /* function exit code */
@@ -18494,15 +18586,15 @@
   #endif
   __pyx_generator->resume_label = -1;
   __Pyx_Coroutine_clear((PyObject*)__pyx_generator);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":559
+/* "pe/_cy_machine.pyx":561
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 
@@ -18515,101 +18607,101 @@
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "pe/_cy_machine.pyx":566
+  /* "pe/_cy_machine.pyx":568
  *         int maxcount = 1
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)             # <<<<<<<<<<<<<<
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)
  */
-  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_14CharacterClass_8__init___genexpr(NULL, __pyx_v_ranges); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_14CharacterClass_8__init___genexpr(NULL, __pyx_v_ranges); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 566, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 566, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 568, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_chars);
   __Pyx_DECREF(__pyx_v_self->_chars);
   __pyx_v_self->_chars = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":567
+  /* "pe/_cy_machine.pyx":569
  *     ):
  *         self._chars = ''.join(a for a, b in ranges if not b)
  *         self._ranges = ''.join(a+b for a, b in ranges if b)             # <<<<<<<<<<<<<<
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate
  */
-  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_14CharacterClass_8__init___3genexpr(NULL, __pyx_v_ranges); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_t_1 = __pyx_pf_2pe_11_cy_machine_14CharacterClass_8__init___3genexpr(NULL, __pyx_v_ranges); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Generator_Next(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_Join(__pyx_kp_u__2, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 569, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->_ranges);
   __Pyx_DECREF(__pyx_v_self->_ranges);
   __pyx_v_self->_ranges = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":568
+  /* "pe/_cy_machine.pyx":570
  *         self._chars = ''.join(a for a, b in ranges if not b)
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)             # <<<<<<<<<<<<<<
  *         self._negate = negate
  *         self.mincount = mincount
  */
   __pyx_t_1 = __pyx_v_self->_ranges;
   __Pyx_INCREF(__pyx_t_1);
   if (unlikely(__pyx_t_1 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(0, 568, __pyx_L1_error)
+    __PYX_ERR(0, 570, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 568, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyUnicode_GET_LENGTH(__pyx_t_1); if (unlikely(__pyx_t_3 == ((Py_ssize_t)-1))) __PYX_ERR(0, 570, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_v_self->_rangelen = __pyx_t_3;
 
-  /* "pe/_cy_machine.pyx":569
+  /* "pe/_cy_machine.pyx":571
  *         self._ranges = ''.join(a+b for a, b in ranges if b)
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate             # <<<<<<<<<<<<<<
  *         self.mincount = mincount
  *         self.maxcount = maxcount
  */
   __pyx_v_self->_negate = __pyx_v_negate;
 
-  /* "pe/_cy_machine.pyx":570
+  /* "pe/_cy_machine.pyx":572
  *         self._rangelen = len(self._ranges)
  *         self._negate = negate
  *         self.mincount = mincount             # <<<<<<<<<<<<<<
  *         self.maxcount = maxcount
  * 
  */
   __pyx_v_self->mincount = __pyx_v_mincount;
 
-  /* "pe/_cy_machine.pyx":571
+  /* "pe/_cy_machine.pyx":573
  *         self._negate = negate
  *         self.mincount = mincount
  *         self.maxcount = maxcount             # <<<<<<<<<<<<<<
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  */
   __pyx_v_self->maxcount = __pyx_v_maxcount;
 
-  /* "pe/_cy_machine.pyx":559
+  /* "pe/_cy_machine.pyx":561
  *         int mincount, maxcount
  * 
  *     def __init__(             # <<<<<<<<<<<<<<
  *         self,
  *         list ranges,
  */
 
@@ -18624,15 +18716,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___2generator1);
   __Pyx_XDECREF(__pyx_gb_2pe_11_cy_machine_14CharacterClass_8__init___5generator2);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":573
+/* "pe/_cy_machine.pyx":575
  *         self.maxcount = maxcount
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         cdef Py_UCS4 c
  *         cdef str ranges = self._ranges
  */
 
@@ -18653,56 +18745,56 @@
   long __pyx_t_6;
   Py_UCS4 __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_scan", 1);
 
-  /* "pe/_cy_machine.pyx":575
+  /* "pe/_cy_machine.pyx":577
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         cdef Py_UCS4 c
  *         cdef str ranges = self._ranges             # <<<<<<<<<<<<<<
  *         cdef bint matched
  *         cdef int mincount = self.mincount
  */
   __pyx_t_1 = __pyx_v_self->_ranges;
   __Pyx_INCREF(__pyx_t_1);
   __pyx_v_ranges = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "pe/_cy_machine.pyx":577
+  /* "pe/_cy_machine.pyx":579
  *         cdef str ranges = self._ranges
  *         cdef bint matched
  *         cdef int mincount = self.mincount             # <<<<<<<<<<<<<<
  *         cdef int maxcount = self.maxcount
  *         cdef int i = 0
  */
   __pyx_t_2 = __pyx_v_self->mincount;
   __pyx_v_mincount = __pyx_t_2;
 
-  /* "pe/_cy_machine.pyx":578
+  /* "pe/_cy_machine.pyx":580
  *         cdef bint matched
  *         cdef int mincount = self.mincount
  *         cdef int maxcount = self.maxcount             # <<<<<<<<<<<<<<
  *         cdef int i = 0
  *         while maxcount and pos < slen:
  */
   __pyx_t_2 = __pyx_v_self->maxcount;
   __pyx_v_maxcount = __pyx_t_2;
 
-  /* "pe/_cy_machine.pyx":579
+  /* "pe/_cy_machine.pyx":581
  *         cdef int mincount = self.mincount
  *         cdef int maxcount = self.maxcount
  *         cdef int i = 0             # <<<<<<<<<<<<<<
  *         while maxcount and pos < slen:
  *             c = s[pos]
  */
   __pyx_v_i = 0;
 
-  /* "pe/_cy_machine.pyx":580
+  /* "pe/_cy_machine.pyx":582
  *         cdef int maxcount = self.maxcount
  *         cdef int i = 0
  *         while maxcount and pos < slen:             # <<<<<<<<<<<<<<
  *             c = s[pos]
  *             matched = False
  */
   while (1) {
@@ -18713,248 +18805,248 @@
       goto __pyx_L5_bool_binop_done;
     }
     __pyx_t_4 = (__pyx_v_pos < __pyx_v_slen);
     __pyx_t_3 = __pyx_t_4;
     __pyx_L5_bool_binop_done:;
     if (!__pyx_t_3) break;
 
-    /* "pe/_cy_machine.pyx":581
+    /* "pe/_cy_machine.pyx":583
  *         cdef int i = 0
  *         while maxcount and pos < slen:
  *             c = s[pos]             # <<<<<<<<<<<<<<
  *             matched = False
  *             if c in self._chars:
  */
-    __pyx_t_5 = __Pyx_GetItemInt_Unicode(__pyx_v_s, __pyx_v_pos, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_5 == (Py_UCS4)-1)) __PYX_ERR(0, 581, __pyx_L1_error)
+    __pyx_t_5 = __Pyx_GetItemInt_Unicode(__pyx_v_s, __pyx_v_pos, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_5 == (Py_UCS4)-1)) __PYX_ERR(0, 583, __pyx_L1_error)
     __pyx_v_c = __pyx_t_5;
 
-    /* "pe/_cy_machine.pyx":582
+    /* "pe/_cy_machine.pyx":584
  *         while maxcount and pos < slen:
  *             c = s[pos]
  *             matched = False             # <<<<<<<<<<<<<<
  *             if c in self._chars:
  *                 matched = True
  */
     __pyx_v_matched = 0;
 
-    /* "pe/_cy_machine.pyx":583
+    /* "pe/_cy_machine.pyx":585
  *             c = s[pos]
  *             matched = False
  *             if c in self._chars:             # <<<<<<<<<<<<<<
  *                 matched = True
  *             else:
  */
     if (unlikely(__pyx_v_self->_chars == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "argument of type 'NoneType' is not iterable");
-      __PYX_ERR(0, 583, __pyx_L1_error)
+      __PYX_ERR(0, 585, __pyx_L1_error)
     }
     __pyx_t_3 = (__Pyx_UnicodeContainsUCS4(__pyx_v_self->_chars, __pyx_v_c));
     if (__pyx_t_3) {
 
-      /* "pe/_cy_machine.pyx":584
+      /* "pe/_cy_machine.pyx":586
  *             matched = False
  *             if c in self._chars:
  *                 matched = True             # <<<<<<<<<<<<<<
  *             else:
  *                 while i < self._rangelen:
  */
       __pyx_v_matched = 1;
 
-      /* "pe/_cy_machine.pyx":583
+      /* "pe/_cy_machine.pyx":585
  *             c = s[pos]
  *             matched = False
  *             if c in self._chars:             # <<<<<<<<<<<<<<
  *                 matched = True
  *             else:
  */
       goto __pyx_L7;
     }
 
-    /* "pe/_cy_machine.pyx":586
+    /* "pe/_cy_machine.pyx":588
  *                 matched = True
  *             else:
  *                 while i < self._rangelen:             # <<<<<<<<<<<<<<
  *                     if ranges[i] <= c <= ranges[i+1]:
  *                         matched = True
  */
     /*else*/ {
       while (1) {
         __pyx_t_3 = (__pyx_v_i < __pyx_v_self->_rangelen);
         if (!__pyx_t_3) break;
 
-        /* "pe/_cy_machine.pyx":587
+        /* "pe/_cy_machine.pyx":589
  *             else:
  *                 while i < self._rangelen:
  *                     if ranges[i] <= c <= ranges[i+1]:             # <<<<<<<<<<<<<<
  *                         matched = True
  *                         break
  */
-        __pyx_t_5 = __Pyx_GetItemInt_Unicode(__pyx_v_ranges, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_5 == (Py_UCS4)-1)) __PYX_ERR(0, 587, __pyx_L1_error)
+        __pyx_t_5 = __Pyx_GetItemInt_Unicode(__pyx_v_ranges, __pyx_v_i, int, 1, __Pyx_PyInt_From_int, 0, 1, 1); if (unlikely(__pyx_t_5 == (Py_UCS4)-1)) __PYX_ERR(0, 589, __pyx_L1_error)
         __pyx_t_3 = (__pyx_t_5 <= __pyx_v_c);
         if (__pyx_t_3) {
           __pyx_t_6 = (__pyx_v_i + 1);
-          __pyx_t_7 = __Pyx_GetItemInt_Unicode(__pyx_v_ranges, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(__pyx_t_7 == (Py_UCS4)-1)) __PYX_ERR(0, 587, __pyx_L1_error)
+          __pyx_t_7 = __Pyx_GetItemInt_Unicode(__pyx_v_ranges, __pyx_t_6, long, 1, __Pyx_PyInt_From_long, 0, 1, 1); if (unlikely(__pyx_t_7 == (Py_UCS4)-1)) __PYX_ERR(0, 589, __pyx_L1_error)
           __pyx_t_3 = (__pyx_v_c <= __pyx_t_7);
         }
         if (__pyx_t_3) {
 
-          /* "pe/_cy_machine.pyx":588
+          /* "pe/_cy_machine.pyx":590
  *                 while i < self._rangelen:
  *                     if ranges[i] <= c <= ranges[i+1]:
  *                         matched = True             # <<<<<<<<<<<<<<
  *                         break
  *                     i += 2
  */
           __pyx_v_matched = 1;
 
-          /* "pe/_cy_machine.pyx":589
+          /* "pe/_cy_machine.pyx":591
  *                     if ranges[i] <= c <= ranges[i+1]:
  *                         matched = True
  *                         break             # <<<<<<<<<<<<<<
  *                     i += 2
  *             if matched ^ self._negate:
  */
           goto __pyx_L9_break;
 
-          /* "pe/_cy_machine.pyx":587
+          /* "pe/_cy_machine.pyx":589
  *             else:
  *                 while i < self._rangelen:
  *                     if ranges[i] <= c <= ranges[i+1]:             # <<<<<<<<<<<<<<
  *                         matched = True
  *                         break
  */
         }
 
-        /* "pe/_cy_machine.pyx":590
+        /* "pe/_cy_machine.pyx":592
  *                         matched = True
  *                         break
  *                     i += 2             # <<<<<<<<<<<<<<
  *             if matched ^ self._negate:
  *                 pos += 1
  */
         __pyx_v_i = (__pyx_v_i + 2);
       }
       __pyx_L9_break:;
     }
     __pyx_L7:;
 
-    /* "pe/_cy_machine.pyx":591
+    /* "pe/_cy_machine.pyx":593
  *                         break
  *                     i += 2
  *             if matched ^ self._negate:             # <<<<<<<<<<<<<<
  *                 pos += 1
  *                 maxcount -= 1
  */
     __pyx_t_3 = (__pyx_v_matched ^ __pyx_v_self->_negate);
     if (__pyx_t_3) {
 
-      /* "pe/_cy_machine.pyx":592
+      /* "pe/_cy_machine.pyx":594
  *                     i += 2
  *             if matched ^ self._negate:
  *                 pos += 1             # <<<<<<<<<<<<<<
  *                 maxcount -= 1
  *                 mincount -= 1
  */
       __pyx_v_pos = (__pyx_v_pos + 1);
 
-      /* "pe/_cy_machine.pyx":593
+      /* "pe/_cy_machine.pyx":595
  *             if matched ^ self._negate:
  *                 pos += 1
  *                 maxcount -= 1             # <<<<<<<<<<<<<<
  *                 mincount -= 1
  *                 i = 0
  */
       __pyx_v_maxcount = (__pyx_v_maxcount - 1);
 
-      /* "pe/_cy_machine.pyx":594
+      /* "pe/_cy_machine.pyx":596
  *                 pos += 1
  *                 maxcount -= 1
  *                 mincount -= 1             # <<<<<<<<<<<<<<
  *                 i = 0
  *             else:
  */
       __pyx_v_mincount = (__pyx_v_mincount - 1);
 
-      /* "pe/_cy_machine.pyx":595
+      /* "pe/_cy_machine.pyx":597
  *                 maxcount -= 1
  *                 mincount -= 1
  *                 i = 0             # <<<<<<<<<<<<<<
  *             else:
  *                 break
  */
       __pyx_v_i = 0;
 
-      /* "pe/_cy_machine.pyx":591
+      /* "pe/_cy_machine.pyx":593
  *                         break
  *                     i += 2
  *             if matched ^ self._negate:             # <<<<<<<<<<<<<<
  *                 pos += 1
  *                 maxcount -= 1
  */
       goto __pyx_L11;
     }
 
-    /* "pe/_cy_machine.pyx":597
+    /* "pe/_cy_machine.pyx":599
  *                 i = 0
  *             else:
  *                 break             # <<<<<<<<<<<<<<
  *         if mincount > 0:
  *             return FAILURE
  */
     /*else*/ {
       goto __pyx_L4_break;
     }
     __pyx_L11:;
   }
   __pyx_L4_break:;
 
-  /* "pe/_cy_machine.pyx":598
+  /* "pe/_cy_machine.pyx":600
  *             else:
  *                 break
  *         if mincount > 0:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         return pos
  */
   __pyx_t_3 = (__pyx_v_mincount > 0);
   if (__pyx_t_3) {
 
-    /* "pe/_cy_machine.pyx":599
+    /* "pe/_cy_machine.pyx":601
  *                 break
  *         if mincount > 0:
  *             return FAILURE             # <<<<<<<<<<<<<<
  *         return pos
  * 
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 599, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 601, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 599, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_As_int(__pyx_t_1); if (unlikely((__pyx_t_2 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 601, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __pyx_r = __pyx_t_2;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":598
+    /* "pe/_cy_machine.pyx":600
  *             else:
  *                 break
  *         if mincount > 0:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         return pos
  */
   }
 
-  /* "pe/_cy_machine.pyx":600
+  /* "pe/_cy_machine.pyx":602
  *         if mincount > 0:
  *             return FAILURE
  *         return pos             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_pos;
   goto __pyx_L0;
 
-  /* "pe/_cy_machine.pyx":573
+  /* "pe/_cy_machine.pyx":575
  *         self.maxcount = maxcount
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         cdef Py_UCS4 c
  *         cdef str ranges = self._ranges
  */
 
@@ -18965,15 +19057,15 @@
   __pyx_r = -2;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_ranges);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":557
+/* "pe/_cy_machine.pyx":559
  *         bint _negate
  *     cdef public:
  *         int mincount, maxcount             # <<<<<<<<<<<<<<
  * 
  *     def __init__(
  */
 
@@ -18997,15 +19089,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->mincount); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->mincount); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19035,15 +19127,15 @@
 
 static int __pyx_pf_2pe_11_cy_machine_14CharacterClass_8mincount_2__set__(struct __pyx_obj_2pe_11_cy_machine_CharacterClass *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 559, __pyx_L1_error)
   __pyx_v_self->mincount = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pe._cy_machine.CharacterClass.mincount.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -19072,15 +19164,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 1);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->maxcount); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->maxcount); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 559, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -19110,15 +19202,15 @@
 
 static int __pyx_pf_2pe_11_cy_machine_14CharacterClass_8maxcount_2__set__(struct __pyx_obj_2pe_11_cy_machine_CharacterClass *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 557, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_int(__pyx_v_value); if (unlikely((__pyx_t_1 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 559, __pyx_L1_error)
   __pyx_v_self->maxcount = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("pe._cy_machine.CharacterClass.maxcount.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -19560,15 +19652,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":606
+/* "pe/_cy_machine.pyx":608
  *     cdef object _regex
  * 
  *     def __init__(self, str pattern, int flags=0):             # <<<<<<<<<<<<<<
  *         self._regex = re.compile(pattern, flags=flags)
  * 
  */
 
@@ -19607,61 +19699,61 @@
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pattern)) != 0)) {
           (void)__Pyx_Arg_NewRef_VARARGS(values[0]);
           kw_args--;
         }
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 608, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_flags);
           if (value) { values[1] = __Pyx_Arg_NewRef_VARARGS(value); kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 608, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 606, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 608, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_pattern = ((PyObject*)values[0]);
     if (values[1]) {
-      __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 606, __pyx_L3_error)
+      __pyx_v_flags = __Pyx_PyInt_As_int(values[1]); if (unlikely((__pyx_v_flags == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 608, __pyx_L3_error)
     } else {
       __pyx_v_flags = ((int)0);
     }
   }
   goto __pyx_L6_skip;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 606, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 0, 1, 2, __pyx_nargs); __PYX_ERR(0, 608, __pyx_L3_error)
   __pyx_L6_skip:;
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   {
     Py_ssize_t __pyx_temp;
     for (__pyx_temp=0; __pyx_temp < (Py_ssize_t)(sizeof(values)/sizeof(values[0])); ++__pyx_temp) {
       __Pyx_Arg_XDECREF_VARARGS(values[__pyx_temp]);
     }
   }
   __Pyx_AddTraceback("pe._cy_machine.Regex.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pattern), (&PyUnicode_Type), 1, "pattern", 1))) __PYX_ERR(0, 606, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_pattern), (&PyUnicode_Type), 1, "pattern", 1))) __PYX_ERR(0, 608, __pyx_L1_error)
   __pyx_r = __pyx_pf_2pe_11_cy_machine_5Regex___init__(((struct __pyx_obj_2pe_11_cy_machine_Regex *)__pyx_v_self), __pyx_v_pattern, __pyx_v_flags);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -19683,49 +19775,49 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 1);
 
-  /* "pe/_cy_machine.pyx":607
+  /* "pe/_cy_machine.pyx":609
  * 
  *     def __init__(self, str pattern, int flags=0):
  *         self._regex = re.compile(pattern, flags=flags)             # <<<<<<<<<<<<<<
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_re); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_re); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_compile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_compile); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_v_pattern);
   __Pyx_GIVEREF(__pyx_v_pattern);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_pattern)) __PYX_ERR(0, 607, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 607, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_pattern)) __PYX_ERR(0, 609, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_flags); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flags, __pyx_t_4) < 0) __PYX_ERR(0, 607, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_flags, __pyx_t_4) < 0) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 607, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 609, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_GIVEREF(__pyx_t_4);
   __Pyx_GOTREF(__pyx_v_self->_regex);
   __Pyx_DECREF(__pyx_v_self->_regex);
   __pyx_v_self->_regex = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":606
+  /* "pe/_cy_machine.pyx":608
  *     cdef object _regex
  * 
  *     def __init__(self, str pattern, int flags=0):             # <<<<<<<<<<<<<<
  *         self._regex = re.compile(pattern, flags=flags)
  * 
  */
 
@@ -19740,15 +19832,15 @@
   __Pyx_AddTraceback("pe._cy_machine.Regex.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "pe/_cy_machine.pyx":609
+/* "pe/_cy_machine.pyx":611
  *         self._regex = re.compile(pattern, flags=flags)
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:
  */
 
@@ -19763,84 +19855,84 @@
   int __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_scan", 1);
 
-  /* "pe/_cy_machine.pyx":610
+  /* "pe/_cy_machine.pyx":612
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         m = self._regex.match(s, pos=pos)             # <<<<<<<<<<<<<<
  *         if m is None:
  *             return FAILURE
  */
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_regex, __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_v_self->_regex, __pyx_n_s_match); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_v_s);
   __Pyx_GIVEREF(__pyx_v_s);
-  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_s)) __PYX_ERR(0, 610, __pyx_L1_error);
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 610, __pyx_L1_error)
+  if (__Pyx_PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_s)) __PYX_ERR(0, 612, __pyx_L1_error);
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_pos); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_pos, __pyx_t_4) < 0) __PYX_ERR(0, 610, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_pos, __pyx_t_4) < 0) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 610, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 612, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_m = __pyx_t_4;
   __pyx_t_4 = 0;
 
-  /* "pe/_cy_machine.pyx":611
+  /* "pe/_cy_machine.pyx":613
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         else:
  */
   __pyx_t_5 = (__pyx_v_m == Py_None);
   if (__pyx_t_5) {
 
-    /* "pe/_cy_machine.pyx":612
+    /* "pe/_cy_machine.pyx":614
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:
  *             return FAILURE             # <<<<<<<<<<<<<<
  *         else:
  *             return m.end()
  */
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 612, __pyx_L1_error)
+    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_FAILURE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 614, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 612, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 614, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_6;
     goto __pyx_L0;
 
-    /* "pe/_cy_machine.pyx":611
+    /* "pe/_cy_machine.pyx":613
  *     cdef int _scan(self, str s, int pos, int slen) except -2:
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:             # <<<<<<<<<<<<<<
  *             return FAILURE
  *         else:
  */
   }
 
-  /* "pe/_cy_machine.pyx":614
+  /* "pe/_cy_machine.pyx":616
  *             return FAILURE
  *         else:
  *             return m.end()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
-    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_m, __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 614, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_m, __pyx_n_s_end); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 616, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_2 = NULL;
     __pyx_t_6 = 0;
     #if CYTHON_UNPACK_METHODS
     if (likely(PyMethod_Check(__pyx_t_3))) {
       __pyx_t_2 = PyMethod_GET_SELF(__pyx_t_3);
       if (likely(__pyx_t_2)) {
@@ -19852,25 +19944,25 @@
       }
     }
     #endif
     {
       PyObject *__pyx_callargs[2] = {__pyx_t_2, NULL};
       __pyx_t_4 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_6, 0+__pyx_t_6);
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
-      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 614, __pyx_L1_error)
+      if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 616, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     }
-    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 614, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_PyInt_As_int(__pyx_t_4); if (unlikely((__pyx_t_6 == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 616, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __pyx_r = __pyx_t_6;
     goto __pyx_L0;
   }
 
-  /* "pe/_cy_machine.pyx":609
+  /* "pe/_cy_machine.pyx":611
  *         self._regex = re.compile(pattern, flags=flags)
  * 
  *     cdef int _scan(self, str s, int pos, int slen) except -2:             # <<<<<<<<<<<<<<
  *         m = self._regex.match(s, pos=pos)
  *         if m is None:
  */
 
@@ -24615,24 +24707,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt *__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct___rpt[8];
 static int __pyx_freecount_2pe_11_cy_machine___pyx_scope_struct___rpt = 0;
+#endif
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct___rpt(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct___rpt > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt)))) {
     o = (PyObject*)__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct___rpt[--__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct___rpt];
     memset(o, 0, sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -24651,15 +24745,15 @@
     if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_2pe_11_cy_machine___pyx_scope_struct___rpt) {
       if (PyObject_CallFinalizerFromDealloc(o)) return;
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_v_pis);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct___rpt < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt)))) {
     __pyx_freelist_2pe_11_cy_machine___pyx_scope_struct___rpt[__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct___rpt++] = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct___rpt *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -24784,24 +24878,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr *__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_1_genexpr[8];
 static int __pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_1_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_1_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_1_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr)))) {
     o = (PyObject*)__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_1_genexpr[--__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_1_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -24825,15 +24921,15 @@
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_outer_scope);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v__);
   Py_CLEAR(p->__pyx_v_pi);
   Py_CLEAR(p->__pyx_t_0);
   Py_CLEAR(p->__pyx_t_3);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_1_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr)))) {
     __pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_1_genexpr[__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_1_genexpr++] = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_1_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -24963,24 +25059,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr *__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_2_genexpr[8];
 static int __pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_2_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_2_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_2_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr)))) {
     o = (PyObject*)__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_2_genexpr[--__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_2_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -25001,15 +25099,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_a);
   Py_CLEAR(p->__pyx_v_b);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_2_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr)))) {
     __pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_2_genexpr[__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_2_genexpr++] = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_2_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -25130,24 +25228,26 @@
   #endif
   #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 #endif
 
+#if CYTHON_USE_FREELISTS
 static struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_3_genexpr *__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_3_genexpr[8];
 static int __pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_3_genexpr = 0;
+#endif
 
 static PyObject *__pyx_tp_new_2pe_11_cy_machine___pyx_scope_struct_3_genexpr(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   PyObject *o;
   #if CYTHON_COMPILING_IN_LIMITED_API
   allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
   o = alloc_func(t, 0);
   #else
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (likely((int)(__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_3_genexpr > 0) & (int)(t->tp_basicsize == sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_3_genexpr)))) {
     o = (PyObject*)__pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_3_genexpr[--__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_3_genexpr];
     memset(o, 0, sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_3_genexpr));
     (void) PyObject_INIT(o, t);
     PyObject_GC_Track(o);
   } else
   #endif
@@ -25168,15 +25268,15 @@
     }
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->__pyx_genexpr_arg_0);
   Py_CLEAR(p->__pyx_v_a);
   Py_CLEAR(p->__pyx_v_b);
-  #if CYTHON_COMPILING_IN_CPYTHON
+  #if CYTHON_USE_FREELISTS
   if (((int)(__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_3_genexpr < 8) & (int)(Py_TYPE(o)->tp_basicsize == sizeof(struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_3_genexpr)))) {
     __pyx_freelist_2pe_11_cy_machine___pyx_scope_struct_3_genexpr[__pyx_freecount_2pe_11_cy_machine___pyx_scope_struct_3_genexpr++] = ((struct __pyx_obj_2pe_11_cy_machine___pyx_scope_struct_3_genexpr *)o);
   } else
   #endif
   {
     #if CYTHON_USE_TYPE_SLOTS || CYTHON_COMPILING_IN_PYPY
     (*Py_TYPE(o)->tp_free)(o);
@@ -25374,14 +25474,15 @@
     {&__pyx_n_s_NOT, __pyx_k_NOT, sizeof(__pyx_k_NOT), 0, 0, 1, 1},
     {&__pyx_n_s_NO_CAP_OR_ACT, __pyx_k_NO_CAP_OR_ACT, sizeof(__pyx_k_NO_CAP_OR_ACT), 0, 0, 1, 1},
     {&__pyx_n_s_OPT, __pyx_k_OPT, sizeof(__pyx_k_OPT), 0, 0, 1, 1},
     {&__pyx_n_s_Operator, __pyx_k_Operator, sizeof(__pyx_k_Operator), 0, 0, 1, 1},
     {&__pyx_n_s_Optional, __pyx_k_Optional, sizeof(__pyx_k_Optional), 0, 0, 1, 1},
     {&__pyx_kp_s_Optional_Definition, __pyx_k_Optional_Definition, sizeof(__pyx_k_Optional_Definition), 0, 0, 1, 0},
     {&__pyx_n_s_PLS, __pyx_k_PLS, sizeof(__pyx_k_PLS), 0, 0, 1, 1},
+    {&__pyx_n_s_ParseError, __pyx_k_ParseError, sizeof(__pyx_k_ParseError), 0, 0, 1, 1},
     {&__pyx_n_s_Parser, __pyx_k_Parser, sizeof(__pyx_k_Parser), 0, 0, 1, 1},
     {&__pyx_n_s_Parser_2, __pyx_k_Parser_2, sizeof(__pyx_k_Parser_2), 0, 0, 1, 1},
     {&__pyx_n_s_Parser___reduce_cython, __pyx_k_Parser___reduce_cython, sizeof(__pyx_k_Parser___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Parser___setstate_cython, __pyx_k_Parser___setstate_cython, sizeof(__pyx_k_Parser___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Parser_match, __pyx_k_Parser_match, sizeof(__pyx_k_Parser_match), 0, 0, 1, 1},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_Program, __pyx_k_Program, sizeof(__pyx_k_Program), 0, 0, 1, 1},
@@ -25389,14 +25490,15 @@
     {&__pyx_n_s_RUL, __pyx_k_RUL, sizeof(__pyx_k_RUL), 0, 0, 1, 1},
     {&__pyx_n_s_Regex, __pyx_k_Regex, sizeof(__pyx_k_Regex), 0, 0, 1, 1},
     {&__pyx_n_s_Regex___reduce_cython, __pyx_k_Regex___reduce_cython, sizeof(__pyx_k_Regex___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Regex___setstate_cython, __pyx_k_Regex___setstate_cython, sizeof(__pyx_k_Regex___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Rule, __pyx_k_Rule, sizeof(__pyx_k_Rule), 0, 0, 1, 1},
     {&__pyx_n_s_SEQ, __pyx_k_SEQ, sizeof(__pyx_k_SEQ), 0, 0, 1, 1},
     {&__pyx_n_s_STR, __pyx_k_STR, sizeof(__pyx_k_STR), 0, 0, 1, 1},
+    {&__pyx_n_s_STRICT, __pyx_k_STRICT, sizeof(__pyx_k_STRICT), 0, 0, 1, 1},
     {&__pyx_n_s_SYM, __pyx_k_SYM, sizeof(__pyx_k_SYM), 0, 0, 1, 1},
     {&__pyx_n_s_Scanner, __pyx_k_Scanner, sizeof(__pyx_k_Scanner), 0, 0, 1, 1},
     {&__pyx_n_s_Scanner___reduce_cython, __pyx_k_Scanner___reduce_cython, sizeof(__pyx_k_Scanner___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Scanner___setstate_cython, __pyx_k_Scanner___setstate_cython, sizeof(__pyx_k_Scanner___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_Scanner_scan, __pyx_k_Scanner_scan, sizeof(__pyx_k_Scanner_scan), 0, 0, 1, 1},
     {&__pyx_n_s_Tuple, __pyx_k_Tuple, sizeof(__pyx_k_Tuple), 0, 0, 1, 1},
     {&__pyx_kp_s_Tuple__Program__Index, __pyx_k_Tuple__Program__Index, sizeof(__pyx_k_Tuple__Program__Index), 0, 0, 1, 0},
@@ -25572,36 +25674,36 @@
 }
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_property = __Pyx_GetBuiltinName(__pyx_n_s_property); if (!__pyx_builtin_property) __PYX_ERR(0, 162, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(0, 65, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(0, 91, __pyx_L1_error)
   __pyx_builtin_super = __Pyx_GetBuiltinName(__pyx_n_s_super); if (!__pyx_builtin_super) __PYX_ERR(0, 146, __pyx_L1_error)
-  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 229, __pyx_L1_error)
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 416, __pyx_L1_error)
-  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 475, __pyx_L1_error)
-  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 523, __pyx_L1_error)
+  __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 231, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 418, __pyx_L1_error)
+  __pyx_builtin_reversed = __Pyx_GetBuiltinName(__pyx_n_s_reversed); if (!__pyx_builtin_reversed) __PYX_ERR(0, 477, __pyx_L1_error)
+  __pyx_builtin_KeyError = __Pyx_GetBuiltinName(__pyx_n_s_KeyError); if (!__pyx_builtin_KeyError) __PYX_ERR(0, 525, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "pe/_cy_machine.pyx":466
+  /* "pe/_cy_machine.pyx":468
  * def _seq(defn):
  *     head = [pi
  *             for d in defn.args[0][:-1]             # <<<<<<<<<<<<<<
  *             for pi in _parsing_instructions(d)]
  *     tail = _parsing_instructions(defn.args[0][-1])
  */
-  __pyx_slice_ = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 466, __pyx_L1_error)
+  __pyx_slice_ = PySlice_New(Py_None, __pyx_int_neg_1, Py_None); if (unlikely(!__pyx_slice_)) __PYX_ERR(0, 468, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_slice_);
   __Pyx_GIVEREF(__pyx_slice_);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xe3b0c44, 0xda39a3e, 0xd41d8cd):             # <<<<<<<<<<<<<<
@@ -25731,25 +25833,25 @@
  *               int pos = 0,
  */
   __pyx_tuple__27 = PyTuple_Pack(9, __pyx_n_s_self, __pyx_n_s_s, __pyx_n_s_pos, __pyx_n_s_flags, __pyx_n_s_memo, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_idx, __pyx_n_s_end); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(0, 169, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__27);
   __Pyx_GIVEREF(__pyx_tuple__27);
   __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_match, 169, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(0, 169, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":197
+  /* "pe/_cy_machine.pyx":199
  *         self.pi = pi
  * 
  *     cpdef int match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
-  __pyx_tuple__29 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_idx, __pyx_n_s_s, __pyx_n_s_pos, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_memo); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(7, __pyx_n_s_self, __pyx_n_s_idx, __pyx_n_s_s, __pyx_n_s_pos, __pyx_n_s_args, __pyx_n_s_kwargs, __pyx_n_s_memo); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
-  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_match, 197, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_codeobj__30 = (PyObject*)__Pyx_PyCode_New(7, 0, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__29, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_match, 199, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__30)) __PYX_ERR(0, 199, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
   __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -25758,208 +25860,208 @@
  *     else:
  *         return __pyx_unpickle__Parser, (type(self), 0x85b42e1, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle__Parser__set_state(self, __pyx_state)
  */
   __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__16, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(1, 16, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":344
+  /* "pe/_cy_machine.pyx":346
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
-  __pyx_tuple__33 = PyTuple_Pack(6, __pyx_n_s_grammar, __pyx_n_s_index_2, __pyx_n_s_pis, __pyx_n_s_name, __pyx_n_s_pis_2, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(6, __pyx_n_s_grammar, __pyx_n_s_index_2, __pyx_n_s_pis, __pyx_n_s_name, __pyx_n_s_pis_2, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__33);
   __Pyx_GIVEREF(__pyx_tuple__33);
-  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_make_program, 344, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_make_program, 346, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 346, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":366
+  /* "pe/_cy_machine.pyx":368
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
-  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_n_s_defn); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__35);
   __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_dot, 366, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_dot, 368, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 368, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":370
+  /* "pe/_cy_machine.pyx":372
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
-  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_lit, 370, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_codeobj__37 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_lit, 372, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__37)) __PYX_ERR(0, 372, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":374
+  /* "pe/_cy_machine.pyx":376
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
-  __pyx_tuple__38 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_maxcount, __pyx_n_s_cclass); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_tuple__38 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_maxcount, __pyx_n_s_cclass); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__38);
   __Pyx_GIVEREF(__pyx_tuple__38);
-  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cls, 374, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 374, __pyx_L1_error)
-  __pyx_tuple__40 = PyTuple_Pack(2, ((PyObject *)__pyx_int_1), ((PyObject *)__pyx_int_1)); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_codeobj__39 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__38, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cls, 376, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__39)) __PYX_ERR(0, 376, __pyx_L1_error)
+  __pyx_tuple__40 = PyTuple_Pack(2, ((PyObject *)__pyx_int_1), ((PyObject *)__pyx_int_1)); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__40);
   __Pyx_GIVEREF(__pyx_tuple__40);
 
-  /* "pe/_cy_machine.pyx":384
+  /* "pe/_cy_machine.pyx":386
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
-  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_n_s_defn, __pyx_n_s_pat, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_tuple__41 = PyTuple_Pack(3, __pyx_n_s_defn, __pyx_n_s_pat, __pyx_n_s_flags); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__41);
   __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rgx, 384, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rgx, 386, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(0, 386, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":389
+  /* "pe/_cy_machine.pyx":391
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_tuple__43 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_tuple__43 = PyTuple_Pack(2, __pyx_n_s_defn, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__43);
   __Pyx_GIVEREF(__pyx_tuple__43);
-  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_opt, 389, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_codeobj__44 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_opt, 391, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__44)) __PYX_ERR(0, 391, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":396
+  /* "pe/_cy_machine.pyx":398
  * 
  * 
  * def _str(defn): return _rpt(defn, 0)             # <<<<<<<<<<<<<<
  * def _pls(defn): return _rpt(defn, 1)
  * 
  */
-  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_str_2, 396, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_str_2, 398, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(0, 398, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":397
+  /* "pe/_cy_machine.pyx":399
  * 
  * def _str(defn): return _rpt(defn, 0)
  * def _pls(defn): return _rpt(defn, 1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_pls, 397, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_codeobj__46 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_pls, 399, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__46)) __PYX_ERR(0, 399, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":400
+  /* "pe/_cy_machine.pyx":402
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
-  __pyx_tuple__47 = PyTuple_Pack(6, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_pis, __pyx_n_s_pi, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_tuple__47 = PyTuple_Pack(6, __pyx_n_s_defn, __pyx_n_s_mincount, __pyx_n_s_pis, __pyx_n_s_pi, __pyx_n_s_genexpr, __pyx_n_s_genexpr); if (unlikely(!__pyx_tuple__47)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__47);
   __Pyx_GIVEREF(__pyx_tuple__47);
-  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rpt, 400, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_codeobj__48 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__47, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rpt, 402, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__48)) __PYX_ERR(0, 402, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":422
+  /* "pe/_cy_machine.pyx":424
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
-  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_sym, 422, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_codeobj__49 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_sym, 424, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__49)) __PYX_ERR(0, 424, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":426
+  /* "pe/_cy_machine.pyx":428
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_and, 426, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_codeobj__50 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_and, 428, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__50)) __PYX_ERR(0, 428, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":434
+  /* "pe/_cy_machine.pyx":436
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_not, 434, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 434, __pyx_L1_error)
+  __pyx_codeobj__51 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__43, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_not, 436, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__51)) __PYX_ERR(0, 436, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":441
+  /* "pe/_cy_machine.pyx":443
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
-  __pyx_tuple__52 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_captured_choice, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_tuple__52 = PyTuple_Pack(4, __pyx_n_s_defn, __pyx_n_s_captured_choice, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__52)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__52);
   __Pyx_GIVEREF(__pyx_tuple__52);
-  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cap, 441, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_codeobj__53 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__52, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_cap, 443, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__53)) __PYX_ERR(0, 443, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":460
+  /* "pe/_cy_machine.pyx":462
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
-  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_bnd, 460, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_codeobj__54 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_bnd, 462, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__54)) __PYX_ERR(0, 462, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":464
+  /* "pe/_cy_machine.pyx":466
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
-  __pyx_tuple__55 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_head, __pyx_n_s_tail, __pyx_n_s_d, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_tuple__55 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_head, __pyx_n_s_tail, __pyx_n_s_d, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__55)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__55);
   __Pyx_GIVEREF(__pyx_tuple__55);
-  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_seq, 464, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_codeobj__56 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__55, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_seq, 466, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__56)) __PYX_ERR(0, 466, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":472
+  /* "pe/_cy_machine.pyx":474
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
-  __pyx_tuple__57 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_pis, __pyx_n_s_pi, __pyx_n_s_pi_2, __pyx_n_s_d); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 472, __pyx_L1_error)
+  __pyx_tuple__57 = PyTuple_Pack(5, __pyx_n_s_defn, __pyx_n_s_pis, __pyx_n_s_pi, __pyx_n_s_pi_2, __pyx_n_s_d); if (unlikely(!__pyx_tuple__57)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__57);
   __Pyx_GIVEREF(__pyx_tuple__57);
-  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_chc, 472, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 472, __pyx_L1_error)
+  __pyx_codeobj__58 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__57, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_chc, 474, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__58)) __PYX_ERR(0, 474, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":483
+  /* "pe/_cy_machine.pyx":485
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
-  __pyx_tuple__60 = PyTuple_Pack(6, __pyx_n_s_defn, __pyx_n_s_subdefn, __pyx_n_s_action, __pyx_n_s__59, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_tuple__60 = PyTuple_Pack(6, __pyx_n_s_defn, __pyx_n_s_subdefn, __pyx_n_s_action, __pyx_n_s__59, __pyx_n_s_pis, __pyx_n_s_pi); if (unlikely(!__pyx_tuple__60)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__60);
   __Pyx_GIVEREF(__pyx_tuple__60);
-  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rul, 483, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_codeobj__61 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__60, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_rul, 485, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__61)) __PYX_ERR(0, 485, __pyx_L1_error)
 
-  /* "pe/_cy_machine.pyx":520
+  /* "pe/_cy_machine.pyx":522
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
-  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_parsing_instructions, 520, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_codeobj__62 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_pe__cy_machine_pyx, __pyx_n_s_parsing_instructions, 522, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__62)) __PYX_ERR(0, 522, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
   __pyx_codeobj__63 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__14, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__63)) __PYX_ERR(1, 1, __pyx_L1_error)
@@ -26168,247 +26270,247 @@
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_Instruction) < 0) __PYX_ERR(0, 98, __pyx_L1_error)
   #endif
   __pyx_vtabptr_2pe_11_cy_machine__Parser = &__pyx_vtable_2pe_11_cy_machine__Parser;
   __pyx_vtable_2pe_11_cy_machine__Parser.match = (int (*)(struct __pyx_obj_2pe_11_cy_machine__Parser *, int, PyObject *, int, PyObject *, PyObject *, PyObject *, int __pyx_skip_dispatch))__pyx_f_2pe_11_cy_machine_7_Parser_match;
   __pyx_vtable_2pe_11_cy_machine__Parser._match = (struct __pyx_t_2pe_11_cy_machine_State *(*)(struct __pyx_obj_2pe_11_cy_machine__Parser *, int, PyObject *, int, PyObject *, PyObject *, PyObject *, struct __pyx_t_2pe_11_cy_machine_State *))__pyx_f_2pe_11_cy_machine_7_Parser__match;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_2pe_11_cy_machine__Parser = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine__Parser_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine__Parser)) __PYX_ERR(0, 191, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine__Parser_spec, __pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_ptype_2pe_11_cy_machine__Parser = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine__Parser_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine__Parser)) __PYX_ERR(0, 193, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine__Parser_spec, __pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine__Parser = &__pyx_type_2pe_11_cy_machine__Parser;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine__Parser->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine__Parser->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine__Parser->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine__Parser->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine__Parser, __pyx_vtabptr_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine__Parser, __pyx_vtabptr_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Parser, (PyObject *) __pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Parser, (PyObject *) __pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine__Parser) < 0) __PYX_ERR(0, 193, __pyx_L1_error)
   #endif
   __pyx_vtabptr_2pe_11_cy_machine_Dot = &__pyx_vtable_2pe_11_cy_machine_Dot;
   __pyx_vtable_2pe_11_cy_machine_Dot.__pyx_base = *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_Dot.__pyx_base._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_3Dot__scan;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 529, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 531, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2pe_11_cy_machine_Dot = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine_Dot_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_2pe_11_cy_machine_Dot)) __PYX_ERR(0, 529, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine_Dot_spec, __pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_2pe_11_cy_machine_Dot)) __PYX_ERR(0, 531, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine_Dot_spec, __pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine_Dot = &__pyx_type_2pe_11_cy_machine_Dot;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_2pe_11_cy_machine_Dot->tp_base = __pyx_ptype_2pe_11_cy_machine_Scanner;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine_Dot->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine_Dot->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine_Dot->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine_Dot->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine_Dot, __pyx_vtabptr_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine_Dot, __pyx_vtabptr_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Dot, (PyObject *) __pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Dot, (PyObject *) __pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 529, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_Dot) < 0) __PYX_ERR(0, 531, __pyx_L1_error)
   #endif
   __pyx_vtabptr_2pe_11_cy_machine_Literal = &__pyx_vtable_2pe_11_cy_machine_Literal;
   __pyx_vtable_2pe_11_cy_machine_Literal.__pyx_base = *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_Literal.__pyx_base._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_7Literal__scan;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 536, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 538, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2pe_11_cy_machine_Literal = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine_Literal_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_2pe_11_cy_machine_Literal)) __PYX_ERR(0, 536, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine_Literal_spec, __pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_2pe_11_cy_machine_Literal)) __PYX_ERR(0, 538, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine_Literal_spec, __pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine_Literal = &__pyx_type_2pe_11_cy_machine_Literal;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_2pe_11_cy_machine_Literal->tp_base = __pyx_ptype_2pe_11_cy_machine_Scanner;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine_Literal->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine_Literal->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine_Literal->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine_Literal->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine_Literal, __pyx_vtabptr_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine_Literal, __pyx_vtabptr_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Literal, (PyObject *) __pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Literal, (PyObject *) __pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 536, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_Literal) < 0) __PYX_ERR(0, 538, __pyx_L1_error)
   #endif
   __pyx_vtabptr_2pe_11_cy_machine_CharacterClass = &__pyx_vtable_2pe_11_cy_machine_CharacterClass;
   __pyx_vtable_2pe_11_cy_machine_CharacterClass.__pyx_base = *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_CharacterClass.__pyx_base._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_14CharacterClass__scan;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 551, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 553, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2pe_11_cy_machine_CharacterClass = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine_CharacterClass_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_2pe_11_cy_machine_CharacterClass)) __PYX_ERR(0, 551, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine_CharacterClass_spec, __pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_2pe_11_cy_machine_CharacterClass)) __PYX_ERR(0, 553, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine_CharacterClass_spec, __pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine_CharacterClass = &__pyx_type_2pe_11_cy_machine_CharacterClass;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_2pe_11_cy_machine_CharacterClass->tp_base = __pyx_ptype_2pe_11_cy_machine_Scanner;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine_CharacterClass->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine_CharacterClass->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine_CharacterClass->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine_CharacterClass->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine_CharacterClass, __pyx_vtabptr_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine_CharacterClass, __pyx_vtabptr_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CharacterClass, (PyObject *) __pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_CharacterClass, (PyObject *) __pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 551, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_CharacterClass) < 0) __PYX_ERR(0, 553, __pyx_L1_error)
   #endif
   __pyx_vtabptr_2pe_11_cy_machine_Regex = &__pyx_vtable_2pe_11_cy_machine_Regex;
   __pyx_vtable_2pe_11_cy_machine_Regex.__pyx_base = *__pyx_vtabptr_2pe_11_cy_machine_Scanner;
   __pyx_vtable_2pe_11_cy_machine_Regex.__pyx_base._scan = (int (*)(struct __pyx_obj_2pe_11_cy_machine_Scanner *, PyObject *, int, int))__pyx_f_2pe_11_cy_machine_5Regex__scan;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 603, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_2pe_11_cy_machine_Scanner); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 605, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_2pe_11_cy_machine_Regex = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine_Regex_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_2pe_11_cy_machine_Regex)) __PYX_ERR(0, 603, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine_Regex_spec, __pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_2pe_11_cy_machine_Regex)) __PYX_ERR(0, 605, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine_Regex_spec, __pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 605, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine_Regex = &__pyx_type_2pe_11_cy_machine_Regex;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_2pe_11_cy_machine_Regex->tp_base = __pyx_ptype_2pe_11_cy_machine_Scanner;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 605, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine_Regex->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine_Regex->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine_Regex->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine_Regex->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine_Regex, __pyx_vtabptr_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_2pe_11_cy_machine_Regex, __pyx_vtabptr_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 605, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 605, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Regex, (PyObject *) __pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Regex, (PyObject *) __pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 605, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 603, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_2pe_11_cy_machine_Regex) < 0) __PYX_ERR(0, 605, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine___pyx_scope_struct___rpt_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt)) __PYX_ERR(0, 400, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct___rpt_spec, __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine___pyx_scope_struct___rpt_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt)) __PYX_ERR(0, 402, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct___rpt_spec, __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt = &__pyx_type_2pe_11_cy_machine___pyx_scope_struct___rpt;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct___rpt->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 416, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 416, __pyx_L1_error)
+  __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr)) __PYX_ERR(0, 418, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr_spec, __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr = &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_1_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 416, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr) < 0) __PYX_ERR(0, 418, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_1_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr)) __PYX_ERR(0, 566, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr_spec, __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 566, __pyx_L1_error)
+  __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr)) __PYX_ERR(0, 568, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr_spec, __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 568, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr = &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_2_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 566, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr) < 0) __PYX_ERR(0, 568, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_2_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_3_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr)) __PYX_ERR(0, 567, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_3_genexpr_spec, __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
+  __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_3_genexpr_spec, NULL); if (unlikely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr)) __PYX_ERR(0, 569, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_2pe_11_cy_machine___pyx_scope_struct_3_genexpr_spec, __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 569, __pyx_L1_error)
   #else
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr = &__pyx_type_2pe_11_cy_machine___pyx_scope_struct_3_genexpr;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 567, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr) < 0) __PYX_ERR(0, 569, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr->tp_dictoffset && __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_2pe_11_cy_machine___pyx_scope_struct_3_genexpr->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
@@ -26820,15 +26922,15 @@
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pe/_cy_machine.pyx":15
  * from cpython.mem cimport PyMem_Malloc, PyMem_Free
  * 
  * from pe._constants import Operator, Flag, FAIL as FAILURE             # <<<<<<<<<<<<<<
- * from pe._errors import Error
+ * from pe._errors import Error, ParseError
  * from pe._match import Match
  */
   __pyx_t_2 = PyList_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Operator);
   __Pyx_GIVEREF(__pyx_n_s_Operator);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_Operator)) __PYX_ERR(0, 15, __pyx_L1_error);
@@ -26854,35 +26956,42 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_FAILURE, __pyx_t_2) < 0) __PYX_ERR(0, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pe/_cy_machine.pyx":16
  * 
  * from pe._constants import Operator, Flag, FAIL as FAILURE
- * from pe._errors import Error             # <<<<<<<<<<<<<<
+ * from pe._errors import Error, ParseError             # <<<<<<<<<<<<<<
  * from pe._match import Match
  * from pe._types import Memo
  */
-  __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __pyx_t_3 = PyList_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_n_s_Error);
   __Pyx_GIVEREF(__pyx_n_s_Error);
   if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 0, __pyx_n_s_Error)) __PYX_ERR(0, 16, __pyx_L1_error);
+  __Pyx_INCREF(__pyx_n_s_ParseError);
+  __Pyx_GIVEREF(__pyx_n_s_ParseError);
+  if (__Pyx_PyList_SET_ITEM(__pyx_t_3, 1, __pyx_n_s_ParseError)) __PYX_ERR(0, 16, __pyx_L1_error);
   __pyx_t_2 = __Pyx_Import(__pyx_n_s_pe__errors, __pyx_t_3, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_Error); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Error, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_ParseError); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_ParseError, __pyx_t_3) < 0) __PYX_ERR(0, 16, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "pe/_cy_machine.pyx":17
  * from pe._constants import Operator, Flag, FAIL as FAILURE
- * from pe._errors import Error
+ * from pe._errors import Error, ParseError
  * from pe._match import Match             # <<<<<<<<<<<<<<
  * from pe._types import Memo
  * from pe._definition import Definition
  */
   __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_Match);
@@ -26894,15 +27003,15 @@
   __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_Match); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_Match, __pyx_t_2) < 0) __PYX_ERR(0, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "pe/_cy_machine.pyx":18
- * from pe._errors import Error
+ * from pe._errors import Error, ParseError
  * from pe._match import Match
  * from pe._types import Memo             # <<<<<<<<<<<<<<
  * from pe._definition import Definition
  * from pe._grammar import Grammar
  */
   __pyx_t_3 = PyList_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
@@ -27398,24 +27507,24 @@
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_MachineParser, __pyx_t_6) < 0) __PYX_ERR(0, 141, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "pe/_cy_machine.pyx":197
+  /* "pe/_cy_machine.pyx":199
  *         self.pi = pi
  * 
  *     cpdef int match(             # <<<<<<<<<<<<<<
  *         self,
  *         int idx,
  */
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_7_Parser_3match, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_match, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_7_Parser_3match, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser_match, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__30)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_2pe_11_cy_machine__Parser, __pyx_n_s_match, __pyx_t_2) < 0) __PYX_ERR(0, 197, __pyx_L1_error)
+  if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_2pe_11_cy_machine__Parser, __pyx_n_s_match, __pyx_t_2) < 0) __PYX_ERR(0, 199, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2pe_11_cy_machine__Parser);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
@@ -27434,544 +27543,544 @@
  */
   __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_7_Parser_7__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Parser___setstate_cython, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (__Pyx_SetItemOnTypeDict((PyObject *)__pyx_ptype_2pe_11_cy_machine__Parser, __pyx_n_s_setstate_cython, __pyx_t_2) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_2pe_11_cy_machine__Parser);
 
-  /* "pe/_cy_machine.pyx":341
+  /* "pe/_cy_machine.pyx":343
  * # Captures and actions cannot be placed on these operators because of
  * # their effect on the stack
  * NO_CAP_OR_ACT = {CALL, COMMIT, UPDATE, RESTORE, FAILTWICE, RETURN}             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_CALL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_COMMIT); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_5 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_UPDATE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_UPDATE); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
-  __pyx_t_6 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RESTORE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RESTORE); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
-  __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAILTWICE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_FAILTWICE); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_7 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RETURN); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_enum____pyx_t_2pe_11_cy_machine_OpCode(__pyx_e_2pe_11_cy_machine_RETURN); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __pyx_t_8 = PySet_New(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 341, __pyx_L1_error)
+  __pyx_t_8 = PySet_New(0); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PySet_Add(__pyx_t_8, __pyx_t_2) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_8, __pyx_t_2) < 0) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PySet_Add(__pyx_t_8, __pyx_t_3) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_8, __pyx_t_3) < 0) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PySet_Add(__pyx_t_8, __pyx_t_5) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_8, __pyx_t_5) < 0) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  if (PySet_Add(__pyx_t_8, __pyx_t_6) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_8, __pyx_t_6) < 0) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  if (PySet_Add(__pyx_t_8, __pyx_t_4) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_8, __pyx_t_4) < 0) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PySet_Add(__pyx_t_8, __pyx_t_7) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (PySet_Add(__pyx_t_8, __pyx_t_7) < 0) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NO_CAP_OR_ACT, __pyx_t_8) < 0) __PYX_ERR(0, 341, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_NO_CAP_OR_ACT, __pyx_t_8) < 0) __PYX_ERR(0, 343, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":344
+  /* "pe/_cy_machine.pyx":346
  * 
  * 
  * def _make_program(grammar) -> Tuple[_Program, _Index]:             # <<<<<<<<<<<<<<
  *     """A "program" is a set of instructions and mappings."""
  *     index = {}
  */
-  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 344, __pyx_L1_error)
+  __pyx_t_8 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_return, __pyx_kp_s_Tuple__Program__Index) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_1_make_program, 0, __pyx_n_s_make_program, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 344, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_8, __pyx_n_s_return, __pyx_kp_s_Tuple__Program__Index) < 0) __PYX_ERR(0, 346, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_1_make_program, 0, __pyx_n_s_make_program, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_7, __pyx_t_8);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_make_program, __pyx_t_7) < 0) __PYX_ERR(0, 344, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_make_program, __pyx_t_7) < 0) __PYX_ERR(0, 346, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":366
+  /* "pe/_cy_machine.pyx":368
  * 
  * 
  * def _dot(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Dot())]
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_3_dot, 0, __pyx_n_s_dot, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 366, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_3_dot, 0, __pyx_n_s_dot, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dot, __pyx_t_7) < 0) __PYX_ERR(0, 366, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_dot, __pyx_t_7) < 0) __PYX_ERR(0, 368, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":370
+  /* "pe/_cy_machine.pyx":372
  * 
  * 
  * def _lit(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(SCAN, scanner=Literal(defn.args[0]))]
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_5_lit, 0, __pyx_n_s_lit, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 370, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_5_lit, 0, __pyx_n_s_lit, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__37)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lit, __pyx_t_7) < 0) __PYX_ERR(0, 370, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_lit, __pyx_t_7) < 0) __PYX_ERR(0, 372, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":374
+  /* "pe/_cy_machine.pyx":376
  * 
  * 
  * def _cls(defn, mincount=1, maxcount=1):             # <<<<<<<<<<<<<<
  *     cclass = CharacterClass(
  *         defn.args[0],
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_7_cls, 0, __pyx_n_s_cls, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 374, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_7_cls, 0, __pyx_n_s_cls, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__39)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__40);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cls, __pyx_t_7) < 0) __PYX_ERR(0, 374, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cls, __pyx_t_7) < 0) __PYX_ERR(0, 376, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":384
+  /* "pe/_cy_machine.pyx":386
  * 
  * 
  * def _rgx(defn):             # <<<<<<<<<<<<<<
  *     pat, flags = defn.args
  *     return [Instruction(SCAN, scanner=Regex(pat, flags=flags))]
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_9_rgx, 0, __pyx_n_s_rgx, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 384, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_9_rgx, 0, __pyx_n_s_rgx, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__42)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rgx, __pyx_t_7) < 0) __PYX_ERR(0, 384, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rgx, __pyx_t_7) < 0) __PYX_ERR(0, 386, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":389
+  /* "pe/_cy_machine.pyx":391
  * 
  * 
  * def _opt(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_11_opt, 0, __pyx_n_s_opt, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 389, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_11_opt, 0, __pyx_n_s_opt, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__44)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_opt, __pyx_t_7) < 0) __PYX_ERR(0, 389, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_opt, __pyx_t_7) < 0) __PYX_ERR(0, 391, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":396
+  /* "pe/_cy_machine.pyx":398
  * 
  * 
  * def _str(defn): return _rpt(defn, 0)             # <<<<<<<<<<<<<<
  * def _pls(defn): return _rpt(defn, 1)
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13_str, 0, __pyx_n_s_str_2, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 396, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_13_str, 0, __pyx_n_s_str_2, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__45)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_str_2, __pyx_t_7) < 0) __PYX_ERR(0, 396, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_str_2, __pyx_t_7) < 0) __PYX_ERR(0, 398, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":397
+  /* "pe/_cy_machine.pyx":399
  * 
  * def _str(defn): return _rpt(defn, 0)
  * def _pls(defn): return _rpt(defn, 1)             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_15_pls, 0, __pyx_n_s_pls, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 397, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_15_pls, 0, __pyx_n_s_pls, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__46)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pls, __pyx_t_7) < 0) __PYX_ERR(0, 397, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pls, __pyx_t_7) < 0) __PYX_ERR(0, 399, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":400
+  /* "pe/_cy_machine.pyx":402
  * 
  * 
  * def _rpt(defn, mincount):             # <<<<<<<<<<<<<<
  *     pis = _parsing_instructions(defn.args[0])
  *     if (len(pis) == 1
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_17_rpt, 0, __pyx_n_s_rpt, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 400, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_17_rpt, 0, __pyx_n_s_rpt, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__48)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rpt, __pyx_t_7) < 0) __PYX_ERR(0, 400, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rpt, __pyx_t_7) < 0) __PYX_ERR(0, 402, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":422
+  /* "pe/_cy_machine.pyx":424
  * 
  * 
  * def _sym(defn):             # <<<<<<<<<<<<<<
  *     return [Instruction(CALL, name=defn.args[0])]
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_19_sym, 0, __pyx_n_s_sym, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 422, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_19_sym, 0, __pyx_n_s_sym, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__49)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sym, __pyx_t_7) < 0) __PYX_ERR(0, 422, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sym, __pyx_t_7) < 0) __PYX_ERR(0, 424, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":426
+  /* "pe/_cy_machine.pyx":428
  * 
  * 
  * def _and(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_21_and, 0, __pyx_n_s_and, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 426, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_21_and, 0, __pyx_n_s_and, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__50)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_and, __pyx_t_7) < 0) __PYX_ERR(0, 426, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_and, __pyx_t_7) < 0) __PYX_ERR(0, 428, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":434
+  /* "pe/_cy_machine.pyx":436
  * 
  * 
  * def _not(defn):             # <<<<<<<<<<<<<<
  *     pi = _parsing_instructions(defn.args[0])
  *     return [Instruction(BRANCH, len(pi) + 2),
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_23_not, 0, __pyx_n_s_not, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 434, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_23_not, 0, __pyx_n_s_not, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__51)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_not, __pyx_t_7) < 0) __PYX_ERR(0, 434, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_not, __pyx_t_7) < 0) __PYX_ERR(0, 436, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":441
+  /* "pe/_cy_machine.pyx":443
  * 
  * 
  * def _cap(defn):             # <<<<<<<<<<<<<<
  *     captured_choice = defn.args[0].op == Operator.CHC
  *     pis = _parsing_instructions(defn.args[0])
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_25_cap, 0, __pyx_n_s_cap, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 441, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_25_cap, 0, __pyx_n_s_cap, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__53)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cap, __pyx_t_7) < 0) __PYX_ERR(0, 441, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_cap, __pyx_t_7) < 0) __PYX_ERR(0, 443, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":460
+  /* "pe/_cy_machine.pyx":462
  * 
  * 
  * def _bnd(defn):             # <<<<<<<<<<<<<<
  *     return _rul(Rule(defn.args[0], Bind(defn.args[1])))
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_27_bnd, 0, __pyx_n_s_bnd, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_27_bnd, 0, __pyx_n_s_bnd, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__54)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_bnd, __pyx_t_7) < 0) __PYX_ERR(0, 460, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_bnd, __pyx_t_7) < 0) __PYX_ERR(0, 462, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":464
+  /* "pe/_cy_machine.pyx":466
  * 
  * 
  * def _seq(defn):             # <<<<<<<<<<<<<<
  *     head = [pi
  *             for d in defn.args[0][:-1]
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_29_seq, 0, __pyx_n_s_seq, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 464, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_29_seq, 0, __pyx_n_s_seq, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__56)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_seq, __pyx_t_7) < 0) __PYX_ERR(0, 464, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_seq, __pyx_t_7) < 0) __PYX_ERR(0, 466, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":472
+  /* "pe/_cy_machine.pyx":474
  * 
  * 
  * def _chc(defn):             # <<<<<<<<<<<<<<
  *     pis = [_parsing_instructions(d) for d in defn.args[0]]
  *     pi = pis[-1]
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_31_chc, 0, __pyx_n_s_chc, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 472, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_31_chc, 0, __pyx_n_s_chc, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__58)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_chc, __pyx_t_7) < 0) __PYX_ERR(0, 472, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_chc, __pyx_t_7) < 0) __PYX_ERR(0, 474, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":483
+  /* "pe/_cy_machine.pyx":485
  * 
  * 
  * def _rul(defn):             # <<<<<<<<<<<<<<
  *     subdefn, action, _ = defn.args
  *     pis = _parsing_instructions(subdefn)
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_33_rul, 0, __pyx_n_s_rul, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 483, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_33_rul, 0, __pyx_n_s_rul, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__61)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rul, __pyx_t_7) < 0) __PYX_ERR(0, 483, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_rul, __pyx_t_7) < 0) __PYX_ERR(0, 485, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":502
+  /* "pe/_cy_machine.pyx":504
  * 
  * _op_map = {
  *     Operator.DOT: _dot,             # <<<<<<<<<<<<<<
  *     Operator.LIT: _lit,
  *     Operator.CLS: _cls,
  */
-  __pyx_t_7 = __Pyx_PyDict_NewPresized(15); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyDict_NewPresized(15); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_DOT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_DOT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_dot); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 502, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_dot); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":503
+  /* "pe/_cy_machine.pyx":505
  * _op_map = {
  *     Operator.DOT: _dot,
  *     Operator.LIT: _lit,             # <<<<<<<<<<<<<<
  *     Operator.CLS: _cls,
  *     Operator.RGX: _rgx,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_LIT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_LIT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_lit); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 503, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_lit); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":504
+  /* "pe/_cy_machine.pyx":506
  *     Operator.DOT: _dot,
  *     Operator.LIT: _lit,
  *     Operator.CLS: _cls,             # <<<<<<<<<<<<<<
  *     Operator.RGX: _rgx,
  *     Operator.OPT: _opt,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CLS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CLS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_cls); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 504, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_cls); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 506, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":505
+  /* "pe/_cy_machine.pyx":507
  *     Operator.LIT: _lit,
  *     Operator.CLS: _cls,
  *     Operator.RGX: _rgx,             # <<<<<<<<<<<<<<
  *     Operator.OPT: _opt,
  *     Operator.STR: _str,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 507, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_RGX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_RGX); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_rgx); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 505, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_rgx); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 507, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":506
+  /* "pe/_cy_machine.pyx":508
  *     Operator.CLS: _cls,
  *     Operator.RGX: _rgx,
  *     Operator.OPT: _opt,             # <<<<<<<<<<<<<<
  *     Operator.STR: _str,
  *     Operator.PLS: _pls,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_OPT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_OPT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_opt); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 506, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_opt); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 508, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":507
+  /* "pe/_cy_machine.pyx":509
  *     Operator.RGX: _rgx,
  *     Operator.OPT: _opt,
  *     Operator.STR: _str,             # <<<<<<<<<<<<<<
  *     Operator.PLS: _pls,
  *     Operator.SYM: _sym,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_STR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_STR); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_str_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 507, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_str_2); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 509, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":508
+  /* "pe/_cy_machine.pyx":510
  *     Operator.OPT: _opt,
  *     Operator.STR: _str,
  *     Operator.PLS: _pls,             # <<<<<<<<<<<<<<
  *     Operator.SYM: _sym,
  *     Operator.AND: _and,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 510, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_PLS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_PLS); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 510, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_pls); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 508, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_pls); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 510, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":509
+  /* "pe/_cy_machine.pyx":511
  *     Operator.STR: _str,
  *     Operator.PLS: _pls,
  *     Operator.SYM: _sym,             # <<<<<<<<<<<<<<
  *     Operator.AND: _and,
  *     Operator.NOT: _not,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_SYM); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_SYM); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_sym); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 509, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_sym); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 511, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":510
+  /* "pe/_cy_machine.pyx":512
  *     Operator.PLS: _pls,
  *     Operator.SYM: _sym,
  *     Operator.AND: _and,             # <<<<<<<<<<<<<<
  *     Operator.NOT: _not,
  *     Operator.CAP: _cap,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_AND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_AND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_and); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 510, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_and); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 512, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":511
+  /* "pe/_cy_machine.pyx":513
  *     Operator.SYM: _sym,
  *     Operator.AND: _and,
  *     Operator.NOT: _not,             # <<<<<<<<<<<<<<
  *     Operator.CAP: _cap,
  *     Operator.BND: _bnd,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_NOT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_NOT); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_not); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 511, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_not); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 513, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":512
+  /* "pe/_cy_machine.pyx":514
  *     Operator.AND: _and,
  *     Operator.NOT: _not,
  *     Operator.CAP: _cap,             # <<<<<<<<<<<<<<
  *     Operator.BND: _bnd,
  *     Operator.SEQ: _seq,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CAP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CAP); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_cap); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 512, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_cap); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 514, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":513
+  /* "pe/_cy_machine.pyx":515
  *     Operator.NOT: _not,
  *     Operator.CAP: _cap,
  *     Operator.BND: _bnd,             # <<<<<<<<<<<<<<
  *     Operator.SEQ: _seq,
  *     Operator.CHC: _chc,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_BND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_BND); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_bnd); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 513, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_bnd); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 515, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":514
+  /* "pe/_cy_machine.pyx":516
  *     Operator.CAP: _cap,
  *     Operator.BND: _bnd,
  *     Operator.SEQ: _seq,             # <<<<<<<<<<<<<<
  *     Operator.CHC: _chc,
  *     Operator.RUL: _rul,
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_SEQ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_SEQ); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_seq); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 514, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_seq); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 516, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":515
+  /* "pe/_cy_machine.pyx":517
  *     Operator.BND: _bnd,
  *     Operator.SEQ: _seq,
  *     Operator.CHC: _chc,             # <<<<<<<<<<<<<<
  *     Operator.RUL: _rul,
  * }
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CHC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_CHC); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_chc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 515, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_chc); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 517, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
 
-  /* "pe/_cy_machine.pyx":516
+  /* "pe/_cy_machine.pyx":518
  *     Operator.SEQ: _seq,
  *     Operator.CHC: _chc,
  *     Operator.RUL: _rul,             # <<<<<<<<<<<<<<
  * }
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_Operator); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_RUL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_8, __pyx_n_s_RUL); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_rul); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_8, __pyx_n_s_rul); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 518, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_8);
-  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 502, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_7, __pyx_t_4, __pyx_t_8) < 0) __PYX_ERR(0, 504, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_op_map, __pyx_t_7) < 0) __PYX_ERR(0, 501, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_op_map, __pyx_t_7) < 0) __PYX_ERR(0, 503, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "pe/_cy_machine.pyx":520
+  /* "pe/_cy_machine.pyx":522
  * 
  * 
  * def _parsing_instructions(defn):  # noqa: C901             # <<<<<<<<<<<<<<
  *     try:
  *         return _op_map[defn.op](defn)
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_35_parsing_instructions, 0, __pyx_n_s_parsing_instructions, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 520, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_2pe_11_cy_machine_35_parsing_instructions, 0, __pyx_n_s_parsing_instructions, NULL, __pyx_n_s_pe__cy_machine, __pyx_d, ((PyObject *)__pyx_codeobj__62)); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parsing_instructions, __pyx_t_7) < 0) __PYX_ERR(0, 520, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_parsing_instructions, __pyx_t_7) < 0) __PYX_ERR(0, 522, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
@@ -29236,19 +29345,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -29327,15 +29436,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -29346,15 +29455,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -29378,15 +29487,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -29651,17 +29760,18 @@
     PyErr_Format(PyExc_ValueError,
                  "need more than %" CYTHON_FORMAT_SSIZE_T "d value%.1s to unpack",
                  index, (index == 1) ? "" : "s");
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
@@ -32364,15 +32474,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -33192,15 +33302,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
```

### Comparing `pe-0.5.1/pe/_cy_machine.pyx` & `pe-0.5.2/pe/_cy_machine.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from typing import Union, Tuple, List, Dict, Optional, Any
 import re
 from enum import IntEnum
 
 from cpython.mem cimport PyMem_Malloc, PyMem_Free
 
 from pe._constants import Operator, Flag, FAIL as FAILURE
-from pe._errors import Error
+from pe._errors import Error, ParseError
 from pe._match import Match
 from pe._types import Memo
 from pe._definition import Definition
 from pe._grammar import Grammar
 from pe._parser import Parser
 from pe._optimize import optimize
 from pe._autoignore import autoignore
@@ -172,14 +172,16 @@
               flags: Flag = Flag.NONE) -> Union[Match, None]:
         memo: Union[Memo, None] = None
         args: List[Any] = []
         kwargs: List[_Binding] = []
         idx = self._index[self.start]
         end = self._parser.match(idx, s, pos, args, kwargs, memo)
         if end < 0:
+            if flags & Flag.STRICT:
+                raise ParseError()
             return None
         else:
             return Match(
                 s,
                 pos,
                 end,
                 self.grammar[self.start],
```

### Comparing `pe-0.5.1/pe/_debug.py` & `pe-0.5.2/pe/_debug.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_definition.py` & `pe-0.5.2/pe/_definition.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_disarm.py` & `pe-0.5.2/pe/_disarm.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_errors.py` & `pe-0.5.2/pe/_errors.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_escape.py` & `pe-0.5.2/pe/_escape.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_functions.py` & `pe-0.5.2/pe/_functions.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_grammar.py` & `pe-0.5.2/pe/_grammar.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_match.py` & `pe-0.5.2/pe/_match.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_optimize.py` & `pe-0.5.2/pe/_optimize.py`

 * *Files 8% similar despite different names*

```diff
@@ -124,30 +124,26 @@
     # [.]  ->  "."  (only 1-char class, not a range, not negated)
     if op == CLS:
         ranges = defn.args[0]
         negated = defn.args[1]
         if len(ranges) == 1 and ranges[0][1] is None and not negated:
             defn = Literal(ranges[0][0])
 
-    if op == SEQ:
-        _common_sequence(defn.args[0])
+    elif op == SEQ:
+        defn = _common_sequence(defn)
 
-    if op == CHC:
-        _common_choice(defn.args[0])
-
-    # Sequence(x)  ->  x  OR  Choice(x)  ->  x
-    if op in (SEQ, CHC) and len(defn.args[0]) == 1:
-        defn = defn.args[0][0]
-        op = defn.op
+    elif op == CHC:
+        defn = _common_choice(defn)
 
     return defn
 
 
-def _common_sequence(subdefs):
+def _common_sequence(defn):
     i = 0
+    subdefs = list(defn.args[0])
     while i < len(subdefs) - 1:
         d = subdefs[i]
         # ![...] .  ->  [^...]
         # !"." .    ->  [^.]
         if (d.op == NOT and subdefs[i+1].op == DOT):
             notd = d.args[0]
             if notd.op == CLS:
@@ -159,37 +155,45 @@
         elif d.op == LIT:
             j = i + 1
             while j < len(subdefs) and subdefs[j].op == LIT:
                 j += 1
             if j - i > 1:
                 subdefs[i:j] = [Literal(''.join(x.args[0] for x in subdefs[i:j]))]
         i += 1
+    return Sequence(*subdefs)
 
 
-def _common_choice(subdefs):
+def _common_choice(defn):
     i = 0
+    subdefs = list(defn.args[0])
     while i < len(subdefs) - 1:
         d = subdefs[i]
         # [..] / [..]  ->  [....]
         # [..] / "."   ->  [...]
         if (d.op == CLS and not d.args[1]) or (d.op == LIT and len(d.args[0]) == 1):
-            ranges = d.args[0] if d.op == CLS else [(d.args[0], None)]
+            ranges = list(d.args[0]) if d.op == CLS else [(d.args[0], None)]
             j = i + 1
             while j < len(subdefs):
                 d2 = subdefs[j]
                 if d2.op == CLS and not d2.args[1]:
                     ranges.extend(d2.args[0])
                 elif d2.op == LIT and len(d2.args[0]) == 1:
                     ranges.append((d2.args[0], None))
                 else:
                     break
                 j += 1
             if j - i > 1:
-                subdefs[i:j] = [Class(ranges)]
+                subdefs[i:j] = [Class(sorted(set(ranges), key=_range_sort_key))]
         i += 1
+    return Choice(*subdefs)
+
+
+def _range_sort_key(range):
+    """Ensure single hyphen characters are the first."""
+    return (range != ("-", None), range)
 
 
 def _regex_dot(defn, defs, grpid):
     return Regex('(?s:.)')
 
 
 def _regex_literal(defn, defs, grpid):
```

### Comparing `pe-0.5.1/pe/_parse.py` & `pe-0.5.2/pe/_parse.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_parser.py` & `pe-0.5.2/pe/_parser.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/_py_machine.py` & `pe-0.5.2/pe/_py_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 """
 
 from typing import Union, Tuple, List, Dict, Optional, Any
 from enum import IntEnum
 import re
 
 from pe._constants import FAIL as FAILURE, Operator, Flag
-from pe._errors import Error
+from pe._errors import Error, ParseError
 from pe._match import Match
 from pe._types import Memo
 from pe._definition import Definition
 from pe._grammar import Grammar
 from pe._parser import Parser
 from pe._optimize import optimize
 from pe._autoignore import autoignore
@@ -128,14 +128,16 @@
               flags: Flag = Flag.NONE) -> Union[Match, None]:
         memo: Union[Memo, None] = None
         args: List[Any] = []
         kwargs: List[_Binding] = []
         idx = self._index[self.start]
         end = _match(self.pi, idx, s, pos, args, kwargs, memo)
         if end < 0:
+            if flags & Flag.STRICT:
+                raise ParseError()
             return None
         else:
             return Match(
                 s,
                 pos,
                 end,
                 self.grammar[self.start],
```

### Comparing `pe-0.5.1/pe/actions.py` & `pe-0.5.2/pe/actions.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/operators.py` & `pe-0.5.2/pe/operators.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe/packrat.py` & `pe-0.5.2/pe/packrat.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pe.egg-info/PKG-INFO` & `pe-0.5.2/pe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pe
-Version: 0.5.1
+Version: 0.5.2
 Summary: Library for Parsing Expression Grammars (PEG)
 Author-email: Michael Wayne Goodman <goodman.m.w@gmail.com>
 License: MIT License
         
         Copyright (c) 2020 Michael Wayne Goodman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pe Version: 0.5.1 Summary: Library for Parsing
+Metadata-Version: 2.1 Name: pe Version: 0.5.2 Summary: Library for Parsing
 Expression Grammars (PEG) Author-email: Michael Wayne Goodman
 gmail.com> License: MIT License Copyright (c) 2020 Michael Wayne Goodman
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
 of the Software, and to permit persons to whom the Software is furnished to do
```

### Comparing `pe-0.5.1/pe.egg-info/SOURCES.txt` & `pe-0.5.2/pe.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/pyproject.toml` & `pe-0.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/setup.py` & `pe-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/test/test__match.py` & `pe-0.5.2/test/test__match.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/test/test__optimize.py` & `pe-0.5.2/test/test__optimize.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,24 @@
 )
 from pe._grammar import Grammar
 from pe._parse import loads
 from pe._optimize import optimize
 
 
 def gload(s, inline=False, common=False, regex=False):
+    _, original = loads(s)
     start, defmap = loads(s)
-    return optimize(Grammar(defmap, start=start),
-                    inline=inline,
-                    common=common,
-                    regex=regex)
+    optimized = optimize(
+        Grammar(defmap, start=start),
+        inline=inline,
+        common=common,
+        regex=regex
+    )
+    assert original == defmap
+    return optimized
 
 
 def iload(s):
     return gload(s, inline=True)
 
 
 def cload(s):
@@ -63,42 +68,52 @@
 
 
 def test_common():
     assert (cload(r'A <- "a"') ==
             gload(r'A <- "a"'))
     assert (cload(r'A <- !"a"') ==
             gload(r'A <- !"a"'))
-    assert (cload(r'A <- !"a"') ==
-            gload(r'A <- !"a"'))
     # single-char classes to literals
     assert (cload(r'A <- [a]') ==
             gload(r'A <- "a"'))
-    # but not single-range
+    # but not multi-char class
+    assert (cload(r'A <- [ab]') ==
+            gload(r'A <- [ab]'))
+    # and not ranges
     assert (cload(r'A <- [a-c]') ==
             gload(r'A <- [a-c]'))
     # add "b" to avoid dropping the sequence
     assert (cload(r'A <- !"a" . "b"') ==
             cload(r'A <- ![a] . "b"') ==
             grm({'A': Sequence(Class('a', negate=True), Literal('b'))}))
     # now show the dropped sequence
     assert (cload(r'A <- !"a" .') ==
             cload(r'A <- ![a] .') ==
             grm({'A': Class('a', negate=True)}))
     # sequence of literals to literal
     assert (cload(r'A <- "a" "bc" "d"') ==
             gload(r'A <- "abcd"'))
-    # but not sequence with classes
+    # or sequence of literals or single-char classes
+    assert (cload(r'A <- "a" [b] "c"') ==
+            gload(r'A <- "abc"'))
+    # but not sequence with multi-char classes
     assert (cload(r'A <- "a" [bc] "d"') ==
             gload(r'A <- "a" [bc] "d"'))
-    # choice of classes or single-char literals
+    # choice of classes
+    assert (cload(r'A <- [ab] / [bc]') ==
+            gload(r'A <- [abc]'))
+    # or choice of classes or single-char literals
     assert (cload(r'A <- [ab] / "m" / [yz]') ==
             gload(r'A <- [abmyz]'))
     # not negated classes though
     assert (cload(r'A <- (![ab] .) / "m" / [yz]') ==
             grm({'A': Choice(Class('ab', negate=True), Class('myz'))}))
+    # hyphen characters are moved to start of class
+    assert (cload(r'A <- [(-,] / [-.]') ==
+            gload(r'A <- [-(-,.]'))
 
 
 def test_regex():
     assert (rload(r'A <- "a"') ==
             grm({'A': Regex(r'a')}))
     assert (rload(r'A <- "a" [bc]') ==
             grm({'A': Regex(r'a[bc]')}))
```

### Comparing `pe-0.5.1/test/test__parse.py` & `pe-0.5.2/test/test__parse.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/test/test_operators.py` & `pe-0.5.2/test/test_operators.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/test/test_parsers.py` & `pe-0.5.2/test/test_parsers.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/test/test_pe.py` & `pe-0.5.2/test/test_pe.py`

 * *Files identical despite different names*

### Comparing `pe-0.5.1/test/test_regression.py` & `pe-0.5.2/test/test_regression.py`

 * *Files identical despite different names*

