# Comparing `tmp/pywebasto-1.0.4.tar.gz` & `tmp/pywebasto-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywebasto-1.0.4.tar", max compression
+gzip compressed data, was "pywebasto-1.0.5.tar", max compression
```

## Comparing `pywebasto-1.0.4.tar` & `pywebasto-1.0.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-04-02 07:50:54.806967 pywebasto-1.0.4/LICENSE
--rw-r--r--   0        0        0       55 2024-04-02 07:50:54.806967 pywebasto-1.0.4/README.md
--rw-r--r--   0        0        0      582 2024-04-02 07:51:06.874885 pywebasto-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    16559 2024-04-02 07:50:54.806967 pywebasto-1.0.4/pywebasto/__init__.py
--rw-r--r--   0        0        0      314 2024-04-02 07:50:54.806967 pywebasto-1.0.4/pywebasto/consts.py
--rw-r--r--   0        0        0      447 2024-04-02 07:50:54.806967 pywebasto-1.0.4/pywebasto/enums.py
--rw-r--r--   0        0        0      205 2024-04-02 07:50:54.806967 pywebasto-1.0.4/pywebasto/exceptions.py
--rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 pywebasto-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-02 08:55:29.365419 pywebasto-1.0.5/LICENSE
+-rw-r--r--   0        0        0       55 2024-04-02 08:55:29.365419 pywebasto-1.0.5/README.md
+-rw-r--r--   0        0        0      582 2024-04-02 08:55:38.845422 pywebasto-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    16609 2024-04-02 08:55:29.365419 pywebasto-1.0.5/pywebasto/__init__.py
+-rw-r--r--   0        0        0      314 2024-04-02 08:55:29.365419 pywebasto-1.0.5/pywebasto/consts.py
+-rw-r--r--   0        0        0      447 2024-04-02 08:55:29.365419 pywebasto-1.0.5/pywebasto/enums.py
+-rw-r--r--   0        0        0      205 2024-04-02 08:55:29.365419 pywebasto-1.0.5/pywebasto/exceptions.py
+-rw-r--r--   0        0        0      833 1970-01-01 00:00:00.000000 pywebasto-1.0.5/PKG-INFO
```

### Comparing `pywebasto-1.0.4/LICENSE` & `pywebasto-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pywebasto-1.0.4/pyproject.toml` & `pywebasto-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pywebasto"
-version = "v1.0.4"
+version = "v1.0.5"
 description = "API library for Webasto ThermoConnect devices"
 authors = ["Malene Trab <malene@trab.dk>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
```

### Comparing `pywebasto-1.0.4/pywebasto/__init__.py` & `pywebasto-1.0.5/pywebasto/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,16 @@
                     ).total_seconds() / 3600
                     if time_diff > 0:
                         self._speed = (distance / 1000) / time_diff
                     else:
                         self._speed = 0
                 else:
                     self._speed = 0
+            else:
+                self._speed = 0
 
         if self._last_data["temperature"][-1] == "C":
             self._iscelcius = True
 
         for output in self._last_data["outputs"]:
             if output["line"] == "OUTH" or output["line"] == "OUTV":
                 self._output_main = output
```

### Comparing `pywebasto-1.0.4/PKG-INFO` & `pywebasto-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pywebasto
-Version: 1.0.4
+Version: 1.0.5
 Summary: API library for Webasto ThermoConnect devices
 License: MIT
 Author: Malene Trab
 Author-email: malene@trab.dk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

