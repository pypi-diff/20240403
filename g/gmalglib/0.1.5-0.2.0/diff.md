# Comparing `tmp/gmalglib-0.1.5.tar.gz` & `tmp/gmalglib-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmalglib-0.1.5.tar", last modified: Mon Apr  1 15:48:32 2024, max compression
+gzip compressed data, was "gmalglib-0.2.0.tar", last modified: Wed Apr  3 13:30:36 2024, max compression
```

## Comparing `gmalglib-0.1.5.tar` & `gmalglib-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:48:32.960622 gmalglib-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 15:48:27.000000 gmalglib-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-01 15:48:32.960622 gmalglib-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 15:48:27.000000 gmalglib-0.1.5/README.en.md
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-01 15:48:27.000000 gmalglib-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-01 15:48:27.000000 gmalglib-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:48:32.960622 gmalglib-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-01 15:48:27.000000 gmalglib-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:48:32.960622 gmalglib-0.1.5/sm3/
--rw-r--r--   0 runner    (1001) docker     (127)     5899 2024-04-01 15:48:27.000000 gmalglib-0.1.5/sm3/sm3.c
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-01 15:48:27.000000 gmalglib-0.1.5/sm3/sm3.h
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-04-01 15:48:27.000000 gmalglib-0.1.5/sm3/sm3module.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:48:32.956622 gmalglib-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:48:32.960622 gmalglib-0.1.5/src/gmalglib/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-01 15:48:27.000000 gmalglib-0.1.5/src/gmalglib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-01 15:48:27.000000 gmalglib-0.1.5/src/gmalglib/sm3.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:48:32.960622 gmalglib-0.1.5/src/gmalglib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-01 15:48:32.000000 gmalglib-0.1.5/src/gmalglib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-01 15:48:32.000000 gmalglib-0.1.5/src/gmalglib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:48:32.000000 gmalglib-0.1.5/src/gmalglib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 15:48:32.000000 gmalglib-0.1.5/src/gmalglib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 13:30:30.000000 gmalglib-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-03 13:30:36.495877 gmalglib-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 13:30:30.000000 gmalglib-0.2.0/README.en.md
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 13:30:30.000000 gmalglib-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.491877 gmalglib-0.2.0/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/include/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 13:30:30.000000 gmalglib-0.2.0/include/gmalglib/sm3.h
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-03 13:30:30.000000 gmalglib-0.2.0/include/gmalglib/sm4.h
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-03 13:30:30.000000 gmalglib-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:30:36.495877 gmalglib-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 13:30:30.000000 gmalglib-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/src/gmalglib/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5862 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm3.c
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm3module.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm4.c
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm4.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-04-03 13:30:30.000000 gmalglib-0.2.0/src/gmalglib/sm4module.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:36.495877 gmalglib-0.2.0/src/gmalglib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-03 13:30:36.000000 gmalglib-0.2.0/src/gmalglib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-03 13:30:36.000000 gmalglib-0.2.0/src/gmalglib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:30:36.000000 gmalglib-0.2.0/src/gmalglib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 13:30:36.000000 gmalglib-0.2.0/src/gmalglib.egg-info/top_level.txt
```

### Comparing `gmalglib-0.1.5/LICENSE` & `gmalglib-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.5/PKG-INFO` & `gmalglib-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.1.5
+Version: 0.2.0
 Summary: GM algorithms C extension for python.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gmalglib
 
 [![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
 [![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
```

### Comparing `gmalglib-0.1.5/pyproject.toml` & `gmalglib-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "gmalglib"
 authors = [
     {name = "ww-rm", email = "ww-rm@qq.com"},
 ]
 description = "GM algorithms C extension for python."
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: C",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Security :: Cryptography",
 ]
@@ -20,10 +20,17 @@
 dynamic = ["version", "readme"]
 
 [project.urls]
 "Homepage" = "https://github.com/ww-rm/gmalglib"
 "Issues" = "https://github.com/ww-rm/gmalglib/issues"
 "Documentation" = "https://gmalglib.readthedocs.io"
 
+[tool.setuptools.packages.find]
+where = ["src"]
+include = ["gmalglib"]
+
+[tool.setuptools.exclude-package-data]
+gmalglib = ["*.c"]
+
 [tool.setuptools.dynamic]
 version = {attr = "gmalglib.__version__"}
 readme = {file = ["README.en.md"], content-type = "text/markdown"}
```

### Comparing `gmalglib-0.1.5/sm3/sm3.c` & `gmalglib-0.2.0/src/gmalglib/sm3.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #include <stdint.h>
-#include "sm3.h"
+#include <gmalglib/sm3.h>
 
 static const
 uint32_t ROL_T_TABLE[64] = {
     0x79cc4519, 0xf3988a32, 0xe7311465, 0xce6228cb, 0x9cc45197, 0x3988a32f, 0x7311465e, 0xe6228cbc,
     0xcc451979, 0x988a32f3, 0x311465e7, 0x6228cbce, 0xc451979c, 0x88a32f39, 0x11465e73, 0x228cbce6,
     0x9d8a7a87, 0x3b14f50f, 0x7629ea1e, 0xec53d43c, 0xd8a7a879, 0xb14f50f3, 0x629ea1e7, 0xc53d43ce,
     0x8a7a879d, 0x14f50f3b, 0x29ea1e76, 0x53d43cec, 0xa7a879d8, 0x4f50f3b1, 0x9ea1e762, 0x3d43cec5,
@@ -23,15 +23,18 @@
 {
     return (X << count) | (X >> (32 - count));
 }
 
 static inline
 uint32_t FROM_BE(const uint8_t* bytes)
 {
-    return (((uint32_t)bytes[0]) << 24) | (((uint32_t)bytes[1]) << 16) | (((uint32_t)bytes[2]) << 8) | (((uint32_t)bytes[3]));
+    return ((uint32_t)bytes[0] << 24) | 
+           ((uint32_t)bytes[1] << 16) | 
+           ((uint32_t)bytes[2] << 8)  |
+           ((uint32_t)bytes[3]);
 }
 
 static inline
 void TO_BE(uint32_t word, uint8_t* bytes)
 {
     bytes[0] = (uint8_t)(word >> 24);
     bytes[1] = (uint8_t)(word >> 16);
@@ -139,18 +142,14 @@
 void SM3_Init(SM3* self)
 {
     uint32_t i;
     for (i = 0; i < 8; i++)
     {
         self->value[i] = INIT_TABLE[i];
     }
-    for (i = 0; i < 64; i++)
-    {
-        self->msg_buffer[i] = 0;
-    }
     self->msg_buffer_length = 0;
     self->msg_bitlen = 0;
 }
 
 int SM3_Update(SM3* self, const uint8_t* data, uint64_t data_len)
 {
     uint64_t data_idx;
```

### Comparing `gmalglib-0.1.5/sm3/sm3.h` & `gmalglib-0.2.0/include/gmalglib/sm3.h`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.5/sm3/sm3module.c` & `gmalglib-0.2.0/src/gmalglib/sm3module.c`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #define PY_SSIZE_T_CLEAN
 
 #include <Python.h>
-#include "sm3.h"
+#include <gmalglib/sm3.h>
 
 typedef struct _PySM3Object {
     PyObject_HEAD
     SM3 sm3;
 } PySM3Object;
 
 static int PySM3_init(PySM3Object* self, PyObject* args, PyObject* kwargs);
@@ -21,27 +21,27 @@
     {"copy", (PyCFunction)PySM3_copy, METH_NOARGS, PyDoc_STR("Copy state to a new object.")},
     {NULL}
 };
 
 static PyTypeObject py_type_SM3 = {
     .ob_base = PyVarObject_HEAD_INIT(NULL, 0)
     .tp_name = "sm3.SM3",
-    .tp_doc = PyDoc_STR("SM3 Object"),
+    .tp_doc = PyDoc_STR("SM3 Object."),
     .tp_basicsize = sizeof(PySM3Object),
     .tp_itemsize = 0,
-    .tp_flags = Py_TPFLAGS_DEFAULT,
+    .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
     .tp_new = PyType_GenericNew,
     .tp_init = (initproc)PySM3_init,
     .tp_methods = py_methods_def_SM3,
 };
 
 static PyModuleDef py_module_def_sm3 = {
     .m_base = PyModuleDef_HEAD_INIT,
     .m_name = "sm3",
-    .m_doc = PyDoc_STR("SM3 Algorithm Implemented in C"),
+    .m_doc = PyDoc_STR("SM3 Algorithm Implemented in C."),
     .m_size = 0,
 };
 
 static int PySM3_init(PySM3Object* self, PyObject* args, PyObject* kwargs)
 {
     char* keys[] = { "data", NULL };
     Py_buffer py_buffer_data = { 0 };
@@ -106,41 +106,41 @@
 
     other->sm3 = self->sm3;
     return (PyObject*)other;
 }
 
 PyMODINIT_FUNC PyInit_sm3() {
     PyObject* py_module = NULL;
-    PyObject* py_long_sm3_max_msg_bitlen = NULL;
-    PyObject* py_long_sm3_digest_length = NULL;
+    PyObject* py_long_SM3_MAX_MSG_BITLEN = NULL;
+    PyObject* py_long_SM3_DIGEST_LENGTH = NULL;
 
     if (PyType_Ready(&py_type_SM3) < 0)
         return NULL;
 
     if (!(py_module = PyModule_Create(&py_module_def_sm3)))
         return NULL;
 
     Py_INCREF(&py_type_SM3);
     if (PyModule_AddObject(py_module, "SM3", (PyObject*)&py_type_SM3) < 0)
         goto error;
 
-    if (!(py_long_sm3_max_msg_bitlen = PyLong_FromUnsignedLongLong(SM3_MAX_MSG_BITLEN)))
+    if (!(py_long_SM3_MAX_MSG_BITLEN = PyLong_FromUnsignedLongLong(SM3_MAX_MSG_BITLEN)))
         goto error;
 
-    if (PyModule_AddObject(py_module, "SM3_MAX_MSG_BITLEN", py_long_sm3_max_msg_bitlen) < 0)
+    if (PyModule_AddObject(py_module, "SM3_MAX_MSG_BITLEN", py_long_SM3_MAX_MSG_BITLEN) < 0)
         goto error;
 
-    if (!(py_long_sm3_digest_length = PyLong_FromUnsignedLongLong(SM3_DIGEST_LENGTH)))
+    if (!(py_long_SM3_DIGEST_LENGTH = PyLong_FromUnsignedLongLong(SM3_DIGEST_LENGTH)))
         goto error;
 
-    if (PyModule_AddObject(py_module, "SM3_DIGEST_LENGTH", py_long_sm3_digest_length) < 0)
+    if (PyModule_AddObject(py_module, "SM3_DIGEST_LENGTH", py_long_SM3_DIGEST_LENGTH) < 0)
         goto error;
 
     return py_module;
 
 error:
-    Py_XDECREF(py_long_sm3_digest_length);
-    Py_XDECREF(py_long_sm3_max_msg_bitlen);
+    Py_XDECREF(py_long_SM3_DIGEST_LENGTH);
+    Py_XDECREF(py_long_SM3_MAX_MSG_BITLEN);
     Py_DECREF(&py_type_SM3);
     Py_DECREF(py_module);
     return NULL;
 }
```

### Comparing `gmalglib-0.1.5/src/gmalglib/sm3.pyi` & `gmalglib-0.2.0/src/gmalglib/sm3.pyi`

 * *Files identical despite different names*

### Comparing `gmalglib-0.1.5/src/gmalglib.egg-info/PKG-INFO` & `gmalglib-0.2.0/src/gmalglib.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: gmalglib
-Version: 0.1.5
+Version: 0.2.0
 Summary: GM algorithms C extension for python.
 Author-email: ww-rm <ww-rm@qq.com>
 Project-URL: Homepage, https://github.com/ww-rm/gmalglib
 Project-URL: Issues, https://github.com/ww-rm/gmalglib/issues
 Project-URL: Documentation, https://gmalglib.readthedocs.io
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # gmalglib
 
 [![Unittest](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-test.yml)
 [![PyPI](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ww-rm/gmalglib/actions/workflows/python-publish.yml)
```

