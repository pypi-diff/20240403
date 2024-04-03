# Comparing `tmp/byte_triggers-0.2.0.tar.gz` & `tmp/byte_triggers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byte_triggers-0.2.0.tar", last modified: Thu Nov  2 16:04:48 2023, max compression
+gzip compressed data, was "byte_triggers-0.3.0.tar", last modified: Wed Apr  3 14:29:28 2024, max compression
```

## Comparing `byte_triggers-0.2.0.tar` & `byte_triggers-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:04:48.571239 byte_triggers-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2023-11-02 16:04:48.571239 byte_triggers-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:04:48.567239 byte_triggers-0.2.0/byte_triggers/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)       98 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:04:48.567239 byte_triggers-0.2.0/byte_triggers/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/commands/sys_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      499 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:04:48.567239 byte_triggers-0.2.0/byte_triggers/io/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5691 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/io/_dlportio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/io/_inpout.py
--rw-r--r--   0 runner    (1001) docker     (127)     3514 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/io/_linux.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/lsl.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    10042 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:04:48.571239 byte_triggers-0.2.0/byte_triggers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/utils/_checks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4179 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/utils/_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/utils/_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/utils/_imports.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/utils/_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4112 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4352 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/byte_triggers/utils/logs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-02 16:04:48.567239 byte_triggers-0.2.0/byte_triggers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5660 2023-11-02 16:04:48.000000 byte_triggers-0.2.0/byte_triggers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-11-02 16:04:48.000000 byte_triggers-0.2.0/byte_triggers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-02 16:04:48.000000 byte_triggers-0.2.0/byte_triggers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-11-02 16:04:48.000000 byte_triggers-0.2.0/byte_triggers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-02 16:04:48.000000 byte_triggers-0.2.0/byte_triggers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-02 16:04:48.000000 byte_triggers-0.2.0/byte_triggers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3450 2023-11-02 16:04:02.000000 byte_triggers-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-02 16:04:48.575239 byte_triggers-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.240423 byte_triggers-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-03 14:29:28.240423 byte_triggers-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.232423 byte_triggers-0.3.0/byte_triggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.232423 byte_triggers-0.3.0/byte_triggers/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/commands/sys_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.236423 byte_triggers-0.3.0/byte_triggers/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5691 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/io/_dlportio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/io/_inpout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/io/_linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/lsl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10074 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.236423 byte_triggers-0.3.0/byte_triggers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7060 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_checks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/byte_triggers/utils/logs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:29:28.236423 byte_triggers-0.3.0/byte_triggers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 14:29:28.000000 byte_triggers-0.3.0/byte_triggers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3450 2024-04-03 14:28:46.000000 byte_triggers-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:29:28.240423 byte_triggers-0.3.0/setup.cfg
```

### Comparing `byte_triggers-0.2.0/LICENSE` & `byte_triggers-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/PKG-INFO` & `byte_triggers-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: byte_triggers
-Version: 0.2.0
+Version: 0.3.0
 Summary: Provides byte (0 to 255) triggers on serial/parallel ports and on LSL streams.
 Author-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: MIT License
         
         Copyright (c) 2022 Mathieu Scheltienne
         
@@ -89,15 +89,15 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![codecov](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers/graph/badge.svg?token=rSGaJehUMl)](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers)
 [![tests](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml)
 [![doc](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml)
 
 # Byte-triggers
 
-Delviers integer triggers between 0 and 255 on a parallel port or on an LSL marker
+Delivers integer triggers between 0 and 255 on a parallel port or on an LSL marker
 stream.
 
 ## Install
 
 `byte_triggers` is available on [PyPI](https://pypi.org/project/byte_triggers/).
 
 ```
```

### Comparing `byte_triggers-0.2.0/README.md` & `byte_triggers-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![codecov](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers/graph/badge.svg?token=rSGaJehUMl)](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers)
 [![tests](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml)
 [![doc](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml)
 
 # Byte-triggers
 
-Delviers integer triggers between 0 and 255 on a parallel port or on an LSL marker
+Delivers integer triggers between 0 and 255 on a parallel port or on an LSL marker
 stream.
 
 ## Install
 
 `byte_triggers` is available on [PyPI](https://pypi.org/project/byte_triggers/).
 
 ```
```

### Comparing `byte_triggers-0.2.0/byte_triggers/_base.py` & `byte_triggers-0.3.0/byte_triggers/_base.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/io/__init__.py` & `byte_triggers-0.3.0/byte_triggers/io/__init__.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/io/_dlportio.py` & `byte_triggers-0.3.0/byte_triggers/io/_dlportio.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/io/_inpout.py` & `byte_triggers-0.3.0/byte_triggers/io/_inpout.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/io/_linux.py` & `byte_triggers-0.3.0/byte_triggers/io/_linux.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/lsl.py` & `byte_triggers-0.3.0/byte_triggers/lsl.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,18 +68,19 @@
                 "The argument 'value' of an LSL trigger must be an integer "
                 "between 1 and 127 included."
             )
         self._outlet.push_sample(np.array([value], dtype=np.int8))
 
     def close(self) -> None:
         """Close the LSL outlet."""
-        try:
-            del self._outlet
-        except Exception:  # pragma: no cover
-            pass
+        if hasattr(self, "_outlet"):
+            try:
+                del self._outlet
+            except Exception:  # pragma: no cover
+                pass
 
     def __del__(self):  # noqa: D105
         self.close()
 
     # --------------------------------------------------------------------
     @property
     def name(self) -> str:
```

### Comparing `byte_triggers-0.2.0/byte_triggers/parallel.py` & `byte_triggers-0.3.0/byte_triggers/parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,15 +235,15 @@
 
     def close(self) -> None:
         """Disconnect the parallel port.
 
         This method should free the parallel or serial port and let other
         application or python process use it.
         """
-        if self._port_type == "arduino":
+        if hasattr(self, "_port_type") and self._port_type == "arduino":
             try:
                 self._port.close()
             except Exception:
                 pass
         if hasattr(self, "_port"):
             try:
                 del self._port
```

### Comparing `byte_triggers-0.2.0/byte_triggers/utils/_checks.py` & `byte_triggers-0.3.0/byte_triggers/utils/_checks.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,31 +89,31 @@
     Raises
     ------
     TypeError
         When the type of the item is not one of the valid options.
     """
     check_types = sum(
         (
-            (type(None),)
-            if type_ is None
-            else (type_,)
-            if not isinstance(type_, str)
-            else _types[type_]
+            (
+                (type(None),)
+                if type_ is None
+                else (type_,) if not isinstance(type_, str) else _types[type_]
+            )
             for type_ in types
         ),
         (),
     )
 
     if not isinstance(item, check_types):
         type_name = [
-            "None"
-            if cls_ is None
-            else cls_.__name__
-            if not isinstance(cls_, str)
-            else cls_
+            (
+                "None"
+                if cls_ is None
+                else cls_.__name__ if not isinstance(cls_, str) else cls_
+            )
             for cls_ in types
         ]
         if len(type_name) == 1:
             type_name = type_name[0]
         elif len(type_name) == 2:
             type_name = " or ".join(type_name)
         else:
```

### Comparing `byte_triggers-0.2.0/byte_triggers/utils/_docs.py` & `byte_triggers-0.3.0/byte_triggers/utils/_docs.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/utils/_fixes.py` & `byte_triggers-0.3.0/byte_triggers/utils/_fixes.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/utils/_imports.py` & `byte_triggers-0.3.0/byte_triggers/utils/_imports.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/utils/_tests.py` & `byte_triggers-0.3.0/byte_triggers/utils/_tests.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers/utils/config.py` & `byte_triggers-0.3.0/byte_triggers/utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,16 +111,18 @@
                 backend = "Not found"
 
             output += f" (backend: {backend})"
         out(output + "\n")
 
     if len(not_found) != 0:
         not_found = [
-            f"{dep.name} ({str(dep.specifier)})"
-            if len(dep.specifier) != 0
-            else dep.name
+            (
+                f"{dep.name} ({str(dep.specifier)})"
+                if len(dep.specifier) != 0
+                else dep.name
+            )
             for dep in not_found
         ]
         if unicode:
             out(f"✘ Not installed: {', '.join(not_found)}\n")
         else:
             out(f"Not installed: {', '.join(not_found)}\n")
```

### Comparing `byte_triggers-0.2.0/byte_triggers/utils/logs.py` & `byte_triggers-0.3.0/byte_triggers/utils/logs.py`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/byte_triggers.egg-info/PKG-INFO` & `byte_triggers-0.3.0/byte_triggers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: byte-triggers
-Version: 0.2.0
+Name: byte_triggers
+Version: 0.3.0
 Summary: Provides byte (0 to 255) triggers on serial/parallel ports and on LSL streams.
 Author-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 Maintainer-email: Mathieu Scheltienne <mathieu.scheltienne@fcbg.ch>
 License: MIT License
         
         Copyright (c) 2022 Mathieu Scheltienne
         
@@ -89,15 +89,15 @@
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 [![codecov](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers/graph/badge.svg?token=rSGaJehUMl)](https://codecov.io/gh/fcbg-hnp-meeg/byte-triggers)
 [![tests](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/pytest.yml)
 [![doc](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml/badge.svg?branch=main)](https://github.com/fcbg-hnp-meeg/byte-triggers/actions/workflows/doc.yml)
 
 # Byte-triggers
 
-Delviers integer triggers between 0 and 255 on a parallel port or on an LSL marker
+Delivers integer triggers between 0 and 255 on a parallel port or on an LSL marker
 stream.
 
 ## Install
 
 `byte_triggers` is available on [PyPI](https://pypi.org/project/byte_triggers/).
 
 ```
```

### Comparing `byte_triggers-0.2.0/byte_triggers.egg-info/SOURCES.txt` & `byte_triggers-0.3.0/byte_triggers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `byte_triggers-0.2.0/pyproject.toml` & `byte_triggers-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 license = {file = 'LICENSE'}
 maintainers = [
   {email = 'mathieu.scheltienne@fcbg.ch', name = 'Mathieu Scheltienne'},
 ]
 name = 'byte_triggers'
 readme = 'README.md'
 requires-python = '>=3.9'
-version = '0.2.0'
+version = '0.3.0'
 
 [project.optional-dependencies]
 all = [
   'byte_triggers[build]',
   'byte_triggers[doc]',
   'byte_triggers[style]',
   'byte_triggers[test]',
```

