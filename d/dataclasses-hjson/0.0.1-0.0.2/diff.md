# Comparing `tmp/dataclasses_hjson-0.0.1.tar.gz` & `tmp/dataclasses_hjson-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataclasses_hjson-0.0.1.tar", max compression
+gzip compressed data, was "dataclasses_hjson-0.0.2.tar", max compression
```

## Comparing `dataclasses_hjson-0.0.1.tar` & `dataclasses_hjson-0.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1496 2024-04-03 17:42:14.532213 dataclasses_hjson-0.0.1/dataclasses_hjson.py
--rw-r--r--   0        0        0      421 2024-04-03 17:33:11.574409 dataclasses_hjson-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1988 2024-04-03 17:46:35.015338 dataclasses_hjson-0.0.1/README.md
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 dataclasses_hjson-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1496 2024-04-03 17:54:59.926484 dataclasses_hjson-0.0.2/dataclasses_hjson.py
+-rw-r--r--   0        0        0      421 2024-04-03 17:55:51.168689 dataclasses_hjson-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2088 2024-04-03 17:54:18.565788 dataclasses_hjson-0.0.2/README.md
+-rw-r--r--   0        0        0     2551 1970-01-01 00:00:00.000000 dataclasses_hjson-0.0.2/PKG-INFO
```

### Comparing `dataclasses_hjson-0.0.1/dataclasses_hjson.py` & `dataclasses_hjson-0.0.2/dataclasses_hjson.py`

 * *Files identical despite different names*

### Comparing `dataclasses_hjson-0.0.1/README.md` & `dataclasses_hjson-0.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,71 @@
 # dataclasses-hjson
 
 This package provides a simple way to serialize and deserialize dataclasses to and from Hjson, using ``dataclasses-json`` and ``hjson``.
 
-Opposed to ``dataclasses-json``, this package does only provide a mixin class to add the functionality to a dataclass, instead of a decorator. You can change the configuration of ``dataclasses-json`` by either using the ``with_config`` decorator or by manually setting the ``dataclasses_json_config`` attribute on the dataclass, using the ``hjson_config`` function.
+Opposed to ``dataclasses-json``, this package does only provide a mixin class to add the functionality to a dataclass, instead of a decorator. You can change the configuration of ``dataclasses-json`` by either using the ``using_config`` decorator or by manually setting the ``dataclasses_json_config`` attribute on the dataclass, using the ``hjson_config`` function.
 
 If you have any problems, ideas or suggestions, feel free to open an issue or a pull request!
 
 ## Installation
 
 ```bash
 pip install dataclasses-hjson
 ```
 
 ## Usage
 
-Example adding config using the ``with_config`` decorator:
+Example adding config using the ``using_config`` decorator:
 
 ```python
 from dataclasses import dataclass
 from dataclasses_json import Undefined, LetterCase
-from dataclasses_hjson import DataClassHjsonMixin, with_config
+from dataclasses_hjson import DataClassHjsonMixin, using_config
 
 
-@with_config(undefined=Undefined.EXCLUDE, letter_case=LetterCase.CAMEL) # (These are the default values)
+@using_config(
+    undefined=Undefined.EXCLUDE, letter_case=LetterCase.CAMEL
+)  # (These are the default values)
 @dataclass
 class Person(DataClassHjsonMixin):
-    name: str
+    first_name: str
     age: int
 
 ```
 
 Alternatively, you can use the ``hjson_config`` function:
 
 ```python
 from dataclasses import dataclass
 from dataclasses_json import Undefined, LetterCase
-from dataclasses_hjson import DataclassHjsonMixin, hjson_config
+from dataclasses_hjson import DataClassHjsonMixin, hjson_config
 
 
 @dataclass
-class Person(DataclassHjsonMixin):
+class Person(DataClassHjsonMixin):
     dataclasses_json_config = hjson_config(undefined=Undefined.EXCLUDE, letter_case=LetterCase.CAMEL) # (These are the default values)
 
-    name: str
+    first_name: str
     age: int
-
 ```
 
 Adding the config is optional however!
 
 Now you can serialize and deserialize the dataclass to and from Hjson:
 
 ```python
-person = Person(name='John Doe', age=30)
-
-# Serialize to Hjson
-hjson_str = person.to_hjson()
-
-# Deserialize from Hjson
-person = Person.from_hjson(hjson_str)
+person = Person(first_name="Guido", age=42)
+person_json = person.to_hjson()
+print(person_json)
+# {
+#   firstName: Guido
+#   age: 42
+# }
+person_copy = Person.from_hjson(person_json)
+print(person_copy)
+# Person(name='Guido', age=42)
 
 ```
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Comparing `dataclasses_hjson-0.0.1/PKG-INFO` & `dataclasses_hjson-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataclasses-hjson
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple mixin that adds .to_hjson and .from_hjson to the dataclasses-json mixin
 License: MIT
 Author: J0J0HA
 Author-email: johannes@jojojux.de
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -13,71 +13,75 @@
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
 Description-Content-Type: text/markdown
 
 # dataclasses-hjson
 
 This package provides a simple way to serialize and deserialize dataclasses to and from Hjson, using ``dataclasses-json`` and ``hjson``.
 
-Opposed to ``dataclasses-json``, this package does only provide a mixin class to add the functionality to a dataclass, instead of a decorator. You can change the configuration of ``dataclasses-json`` by either using the ``with_config`` decorator or by manually setting the ``dataclasses_json_config`` attribute on the dataclass, using the ``hjson_config`` function.
+Opposed to ``dataclasses-json``, this package does only provide a mixin class to add the functionality to a dataclass, instead of a decorator. You can change the configuration of ``dataclasses-json`` by either using the ``using_config`` decorator or by manually setting the ``dataclasses_json_config`` attribute on the dataclass, using the ``hjson_config`` function.
 
 If you have any problems, ideas or suggestions, feel free to open an issue or a pull request!
 
 ## Installation
 
 ```bash
 pip install dataclasses-hjson
 ```
 
 ## Usage
 
-Example adding config using the ``with_config`` decorator:
+Example adding config using the ``using_config`` decorator:
 
 ```python
 from dataclasses import dataclass
 from dataclasses_json import Undefined, LetterCase
-from dataclasses_hjson import DataClassHjsonMixin, with_config
+from dataclasses_hjson import DataClassHjsonMixin, using_config
 
 
-@with_config(undefined=Undefined.EXCLUDE, letter_case=LetterCase.CAMEL) # (These are the default values)
+@using_config(
+    undefined=Undefined.EXCLUDE, letter_case=LetterCase.CAMEL
+)  # (These are the default values)
 @dataclass
 class Person(DataClassHjsonMixin):
-    name: str
+    first_name: str
     age: int
 
 ```
 
 Alternatively, you can use the ``hjson_config`` function:
 
 ```python
 from dataclasses import dataclass
 from dataclasses_json import Undefined, LetterCase
-from dataclasses_hjson import DataclassHjsonMixin, hjson_config
+from dataclasses_hjson import DataClassHjsonMixin, hjson_config
 
 
 @dataclass
-class Person(DataclassHjsonMixin):
+class Person(DataClassHjsonMixin):
     dataclasses_json_config = hjson_config(undefined=Undefined.EXCLUDE, letter_case=LetterCase.CAMEL) # (These are the default values)
 
-    name: str
+    first_name: str
     age: int
-
 ```
 
 Adding the config is optional however!
 
 Now you can serialize and deserialize the dataclass to and from Hjson:
 
 ```python
-person = Person(name='John Doe', age=30)
-
-# Serialize to Hjson
-hjson_str = person.to_hjson()
-
-# Deserialize from Hjson
-person = Person.from_hjson(hjson_str)
+person = Person(first_name="Guido", age=42)
+person_json = person.to_hjson()
+print(person_json)
+# {
+#   firstName: Guido
+#   age: 42
+# }
+person_copy = Person.from_hjson(person_json)
+print(person_copy)
+# Person(name='Guido', age=42)
 
 ```
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

