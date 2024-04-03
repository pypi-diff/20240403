# Comparing `tmp/dataclasses_hjson-0.0.2.tar.gz` & `tmp/dataclasses_hjson-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_hjson-0.0.2.tar", max compression
+gzip compressed data, was "dataclasses_hjson-0.0.3.tar", max compression
```

## Comparing `dataclasses_hjson-0.0.2.tar` & `dataclasses_hjson-0.0.3.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1496 2024-04-03 17:54:59.926484 dataclasses_hjson-0.0.2/dataclasses_hjson.py
--rw-r--r--   0        0        0      421 2024-04-03 17:55:51.168689 dataclasses_hjson-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2088 2024-04-03 17:54:18.565788 dataclasses_hjson-0.0.2/README.md
--rw-r--r--   0        0        0     2551 1970-01-01 00:00:00.000000 dataclasses_hjson-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-04-03 17:54:59.926484 dataclasses_hjson-0.0.3/dataclasses_hjson.py
+-rw-r--r--   0        0        0     1085 2024-04-03 17:58:13.018747 dataclasses_hjson-0.0.3/LICENSE
+-rw-r--r--   0        0        0      583 2024-04-03 18:14:55.365490 dataclasses_hjson-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2165 2024-04-03 18:15:29.327383 dataclasses_hjson-0.0.3/README.md
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 dataclasses_hjson-0.0.3/PKG-INFO
```

### Comparing `dataclasses_hjson-0.0.2/dataclasses_hjson.py` & `dataclasses_hjson-0.0.3/dataclasses_hjson.py`

 * *Files identical despite different names*

### Comparing `dataclasses_hjson-0.0.2/README.md` & `dataclasses_hjson-0.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # dataclasses-hjson
 
-This package provides a simple way to serialize and deserialize dataclasses to and from Hjson, using ``dataclasses-json`` and ``hjson``.
+This package provides a simple way to serialize and deserialize dataclasses to and from Hjson.
+
+This uses ``dataclasses-json`` to serialize and deserialize dataclasses, and ``hjson`` to parse and generate Hjson.
 
 Opposed to ``dataclasses-json``, this package does only provide a mixin class to add the functionality to a dataclass, instead of a decorator. You can change the configuration of ``dataclasses-json`` by either using the ``using_config`` decorator or by manually setting the ``dataclasses_json_config`` attribute on the dataclass, using the ``hjson_config`` function.
 
 If you have any problems, ideas or suggestions, feel free to open an issue or a pull request!
 
 ## Installation
```

### Comparing `dataclasses_hjson-0.0.2/PKG-INFO` & `dataclasses_hjson-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,34 @@
 Metadata-Version: 2.1
 Name: dataclasses-hjson
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple mixin that adds .to_hjson and .from_hjson to the dataclasses-json mixin
+Home-page: https://github.com/J0J0HA/dataclasses-hjson
 License: MIT
+Keywords: dataclasses,json,hjson
 Author: J0J0HA
 Author-email: johannes@jojojux.de
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
+Project-URL: Repository, https://github.com/J0J0HA/dataclasses-hjson
 Description-Content-Type: text/markdown
 
 # dataclasses-hjson
 
-This package provides a simple way to serialize and deserialize dataclasses to and from Hjson, using ``dataclasses-json`` and ``hjson``.
+This package provides a simple way to serialize and deserialize dataclasses to and from Hjson.
+
+This uses ``dataclasses-json`` to serialize and deserialize dataclasses, and ``hjson`` to parse and generate Hjson.
 
 Opposed to ``dataclasses-json``, this package does only provide a mixin class to add the functionality to a dataclass, instead of a decorator. You can change the configuration of ``dataclasses-json`` by either using the ``using_config`` decorator or by manually setting the ``dataclasses_json_config`` attribute on the dataclass, using the ``hjson_config`` function.
 
 If you have any problems, ideas or suggestions, feel free to open an issue or a pull request!
 
 ## Installation
```

