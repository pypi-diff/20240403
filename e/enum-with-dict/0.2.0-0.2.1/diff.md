# Comparing `tmp/enum_with_dict-0.2.0.tar.gz` & `tmp/enum_with_dict-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.2.0.tar", last modified: Wed Apr  3 19:05:46 2024, max compression
+gzip compressed data, was "enum_with_dict-0.2.1.tar", last modified: Wed Apr  3 19:12:12 2024, max compression
```

## Comparing `enum_with_dict-0.2.0.tar` & `enum_with_dict-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 19:05:46.798500 enum_with_dict-0.2.0/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.2.0/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     2205 2024-04-03 19:05:46.798256 enum_with_dict-0.2.0/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     1294 2024-04-03 18:42:51.000000 enum_with_dict-0.2.0/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 19:05:46.796669 enum_with_dict-0.2.0/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.2.0/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)      677 2024-04-03 18:58:53.000000 enum_with_dict-0.2.0/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 19:05:46.797412 enum_with_dict-0.2.0/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     2205 2024-04-03 19:05:46.000000 enum_with_dict-0.2.0/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 19:05:46.000000 enum_with_dict-0.2.0/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 19:05:46.000000 enum_with_dict-0.2.0/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 19:05:46.000000 enum_with_dict-0.2.0/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 19:05:46.798545 enum_with_dict-0.2.0/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 19:03:17.000000 enum_with_dict-0.2.0/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 19:05:46.797642 enum_with_dict-0.2.0/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.2.0/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     2318 2024-04-03 19:01:56.000000 enum_with_dict-0.2.0/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 19:12:12.907341 enum_with_dict-0.2.1/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.2.1/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     2825 2024-04-03 19:12:12.907046 enum_with_dict-0.2.1/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     1914 2024-04-03 19:09:13.000000 enum_with_dict-0.2.1/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 19:12:12.905497 enum_with_dict-0.2.1/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.2.1/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)      677 2024-04-03 18:58:53.000000 enum_with_dict-0.2.1/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 19:12:12.906232 enum_with_dict-0.2.1/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     2825 2024-04-03 19:12:12.000000 enum_with_dict-0.2.1/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 19:12:12.000000 enum_with_dict-0.2.1/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 19:12:12.000000 enum_with_dict-0.2.1/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 19:12:12.000000 enum_with_dict-0.2.1/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 19:12:12.907395 enum_with_dict-0.2.1/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 19:10:10.000000 enum_with_dict-0.2.1/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 19:12:12.906458 enum_with_dict-0.2.1/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.2.1/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     2318 2024-04-03 19:01:56.000000 enum_with_dict-0.2.1/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.2.0/LICENSE` & `enum_with_dict-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.2.0/PKG-INFO` & `enum_with_dict-0.2.1/enum_with_dict.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: enum_with_dict
-Version: 0.2.0
+Name: enum-with-dict
+Version: 0.2.1
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,16 @@
 
 `EnumWithDict` is a Python package that extends the standard library's `Enum` class to include `to_dict` and `get_initial` class methods. This enhancement allows for straightforward conversion of enum classes to dictionaries and provides easy access to the initial enum value, facilitating a more versatile use of enumerations in Python applications.
 
 ## Features
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
+- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
+
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
 pip install enum_with_dict
@@ -65,10 +67,33 @@
 
 ```python
 initial_color = Color.get_initial()
 print(initial_color)
 # Output: 'red'
 ```
 
+### Using the `get` Method
+
+Retrieve an enum value by its name, with an option to specify a default value if the name does not exist.
+
+## Get a value for an existing key
+
+```python
+print(Color.get('RED'))  # Output: 'red'
+```
+
+## Get a value for a non-existing key with a default value
+
+```python
+print(Color.get('PURPLE', default='unknown'))  # Output: 'unknown'
+```
+
+## Get a value for a non-existing key, falling back to the initial value
+
+```python
+print(Color.get('PURPLE'))  # Output: 'red'
+```
+
+
 ## LICENSE
 
 `EnumWithDict` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `enum_with_dict-0.2.0/README.md` & `enum_with_dict-0.2.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 `EnumWithDict` is a Python package that extends the standard library's `Enum` class to include `to_dict` and `get_initial` class methods. This enhancement allows for straightforward conversion of enum classes to dictionaries and provides easy access to the initial enum value, facilitating a more versatile use of enumerations in Python applications.
 
 ## Features
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
+- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
+
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
 pip install enum_with_dict
@@ -41,10 +43,33 @@
 
 ```python
 initial_color = Color.get_initial()
 print(initial_color)
 # Output: 'red'
 ```
 
+### Using the `get` Method
+
+Retrieve an enum value by its name, with an option to specify a default value if the name does not exist.
+
+## Get a value for an existing key
+
+```python
+print(Color.get('RED'))  # Output: 'red'
+```
+
+## Get a value for a non-existing key with a default value
+
+```python
+print(Color.get('PURPLE', default='unknown'))  # Output: 'unknown'
+```
+
+## Get a value for a non-existing key, falling back to the initial value
+
+```python
+print(Color.get('PURPLE'))  # Output: 'red'
+```
+
+
 ## LICENSE
 
 `EnumWithDict` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `enum_with_dict-0.2.0/enum_with_dict/enum_with_dict.py` & `enum_with_dict-0.2.1/enum_with_dict/enum_with_dict.py`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.2.0/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: enum-with-dict
-Version: 0.2.0
+Name: enum_with_dict
+Version: 0.2.1
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -26,14 +26,16 @@
 
 `EnumWithDict` is a Python package that extends the standard library's `Enum` class to include `to_dict` and `get_initial` class methods. This enhancement allows for straightforward conversion of enum classes to dictionaries and provides easy access to the initial enum value, facilitating a more versatile use of enumerations in Python applications.
 
 ## Features
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
+- **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
+
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
 pip install enum_with_dict
@@ -65,10 +67,33 @@
 
 ```python
 initial_color = Color.get_initial()
 print(initial_color)
 # Output: 'red'
 ```
 
+### Using the `get` Method
+
+Retrieve an enum value by its name, with an option to specify a default value if the name does not exist.
+
+## Get a value for an existing key
+
+```python
+print(Color.get('RED'))  # Output: 'red'
+```
+
+## Get a value for a non-existing key with a default value
+
+```python
+print(Color.get('PURPLE', default='unknown'))  # Output: 'unknown'
+```
+
+## Get a value for a non-existing key, falling back to the initial value
+
+```python
+print(Color.get('PURPLE'))  # Output: 'red'
+```
+
+
 ## LICENSE
 
 `EnumWithDict` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `enum_with_dict-0.2.0/setup.py` & `enum_with_dict-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.2.0',
+    version='0.2.1',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/enum_with_dict',
```

### Comparing `enum_with_dict-0.2.0/test/test_enum_with_dict.py` & `enum_with_dict-0.2.1/test/test_enum_with_dict.py`

 * *Files identical despite different names*

