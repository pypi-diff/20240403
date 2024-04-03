# Comparing `tmp/enum_with_dict-0.3.0.tar.gz` & `tmp/enum_with_dict-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.3.0.tar", last modified: Wed Apr  3 20:31:25 2024, max compression
+gzip compressed data, was "enum_with_dict-0.4.0.tar", last modified: Wed Apr  3 21:14:05 2024, max compression
```

## Comparing `enum_with_dict-0.3.0.tar` & `enum_with_dict-0.4.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 20:31:25.002238 enum_with_dict-0.3.0/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.3.0/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     4233 2024-04-03 20:31:25.001971 enum_with_dict-0.3.0/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)     3322 2024-04-03 20:27:57.000000 enum_with_dict-0.3.0/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 20:31:25.000470 enum_with_dict-0.3.0/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.3.0/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     2712 2024-04-03 20:27:57.000000 enum_with_dict-0.3.0/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 20:31:25.001205 enum_with_dict-0.3.0/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     4233 2024-04-03 20:31:24.000000 enum_with_dict-0.3.0/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 20:31:24.000000 enum_with_dict-0.3.0/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 20:31:24.000000 enum_with_dict-0.3.0/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 20:31:24.000000 enum_with_dict-0.3.0/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 20:31:25.002278 enum_with_dict-0.3.0/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 19:26:42.000000 enum_with_dict-0.3.0/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 20:31:25.001436 enum_with_dict-0.3.0/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.3.0/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     5067 2024-04-03 20:27:57.000000 enum_with_dict-0.3.0/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 21:14:05.925396 enum_with_dict-0.4.0/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.4.0/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     4835 2024-04-03 21:14:05.925166 enum_with_dict-0.4.0/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     3924 2024-04-03 21:13:51.000000 enum_with_dict-0.4.0/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 21:14:05.923592 enum_with_dict-0.4.0/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.4.0/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     4574 2024-04-03 21:13:51.000000 enum_with_dict-0.4.0/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 21:14:05.924417 enum_with_dict-0.4.0/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     4835 2024-04-03 21:14:05.000000 enum_with_dict-0.4.0/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 21:14:05.000000 enum_with_dict-0.4.0/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 21:14:05.000000 enum_with_dict-0.4.0/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 21:14:05.000000 enum_with_dict-0.4.0/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 21:14:05.925438 enum_with_dict-0.4.0/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 21:13:51.000000 enum_with_dict-0.4.0/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 21:14:05.924646 enum_with_dict-0.4.0/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.4.0/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     5832 2024-04-03 21:13:51.000000 enum_with_dict-0.4.0/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.3.0/LICENSE` & `enum_with_dict-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.3.0/PKG-INFO` & `enum_with_dict-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.3.0
+Version: 0.4.0
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -29,15 +29,16 @@
 ## Features
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
 - **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
-
+- **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
+- **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
 pip install enum_with_dict
@@ -124,23 +125,51 @@
     TestEnum.VALUE_2: "another_new_value",
     TestEnum.VALUE_3: "a new value"
 }
 
 # Perform the mapping and validate
 mapped_values = TestEnum.map(key_mapping)
 
-# ----- The above is slightly easier to write than the following -----
+# ----- The above is equivalent to the following: -----
 
 # Validate the mapped values
 expected_values = {
     TestEnum.VALUE_1.value: "some_new_value",
     TestEnum.VALUE_2.value: "another_new_value",
     TestEnum.VALUE_3.value: "a new value"
 }
 
 assert mapped_values == expected_values
 
 ```
 
+## Retrieving Keys and Values with `keys()` and `values()`
+
+Retrieve the keys and values of the enum class as a list or as a `KeysView` or `ValuesView`.
+
+### Get keys as a list
+
+```python
+keys_list = Color.keys()
+```
+
+### Get keys as a `KeysView`
+
+```python
+keys_view = Color.keys(as_list=False)
+```
+
+### Get values as a list
+
+```python
+values_list = Color.values()
+```
+
+### Get values as a ValuesView
+
+```python
+values_view = Color.values(as_list=False)
+```
+
 ## LICENSE
 
 `EnumWithDict` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `enum_with_dict-0.3.0/README.md` & `enum_with_dict-0.4.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 ## Features
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
 - **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
-
+- **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
+- **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
 pip install enum_with_dict
@@ -100,23 +101,51 @@
     TestEnum.VALUE_2: "another_new_value",
     TestEnum.VALUE_3: "a new value"
 }
 
 # Perform the mapping and validate
 mapped_values = TestEnum.map(key_mapping)
 
-# ----- The above is slightly easier to write than the following -----
+# ----- The above is equivalent to the following: -----
 
 # Validate the mapped values
 expected_values = {
     TestEnum.VALUE_1.value: "some_new_value",
     TestEnum.VALUE_2.value: "another_new_value",
     TestEnum.VALUE_3.value: "a new value"
 }
 
 assert mapped_values == expected_values
 
 ```
 
+## Retrieving Keys and Values with `keys()` and `values()`
+
+Retrieve the keys and values of the enum class as a list or as a `KeysView` or `ValuesView`.
+
+### Get keys as a list
+
+```python
+keys_list = Color.keys()
+```
+
+### Get keys as a `KeysView`
+
+```python
+keys_view = Color.keys(as_list=False)
+```
+
+### Get values as a list
+
+```python
+values_list = Color.values()
+```
+
+### Get values as a ValuesView
+
+```python
+values_view = Color.values(as_list=False)
+```
+
 ## LICENSE
 
 `EnumWithDict` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `enum_with_dict-0.3.0/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.4.0/enum_with_dict.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.3.0
+Version: 0.4.0
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
@@ -29,15 +29,16 @@
 ## Features
 
 - **to_dict**: Convert an enum class to a dictionary representation, mapping member names to their values.
 - **get_initial**: Retrieve the first value defined in the enum, useful for cases where a default or initial value is needed.
 - **get**: Mimics the dictionary `get` method, allowing retrieval of enum values with an optional default fallback.
 - **validate_mapping_keys**: Ensure that a provided mapping includes all enum values, raising an error for any missing mappings.
 - **map**: Map enum members to values based on the provided dictionary.
-
+- **keys**: Retrieve the keys of the enum class as a list or as a KeysView.
+- **values**: Retrieve the values of the enum class as a list or as a ValuesView.
 
 ## Installation
 
 Install `EnumWithDict` using pip:
 
 ```bash
 pip install enum_with_dict
@@ -124,23 +125,51 @@
     TestEnum.VALUE_2: "another_new_value",
     TestEnum.VALUE_3: "a new value"
 }
 
 # Perform the mapping and validate
 mapped_values = TestEnum.map(key_mapping)
 
-# ----- The above is slightly easier to write than the following -----
+# ----- The above is equivalent to the following: -----
 
 # Validate the mapped values
 expected_values = {
     TestEnum.VALUE_1.value: "some_new_value",
     TestEnum.VALUE_2.value: "another_new_value",
     TestEnum.VALUE_3.value: "a new value"
 }
 
 assert mapped_values == expected_values
 
 ```
 
+## Retrieving Keys and Values with `keys()` and `values()`
+
+Retrieve the keys and values of the enum class as a list or as a `KeysView` or `ValuesView`.
+
+### Get keys as a list
+
+```python
+keys_list = Color.keys()
+```
+
+### Get keys as a `KeysView`
+
+```python
+keys_view = Color.keys(as_list=False)
+```
+
+### Get values as a list
+
+```python
+values_list = Color.values()
+```
+
+### Get values as a ValuesView
+
+```python
+values_view = Color.values(as_list=False)
+```
+
 ## LICENSE
 
 `EnumWithDict` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
```

### Comparing `enum_with_dict-0.3.0/setup.py` & `enum_with_dict-0.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.3.0',
+    version='0.4.0',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/enum_with_dict',
```

### Comparing `enum_with_dict-0.3.0/test/test_enum_with_dict.py` & `enum_with_dict-0.4.0/test/test_enum_with_dict.py`

 * *Files 12% similar despite different names*

```diff
@@ -135,10 +135,31 @@
             TestEnum.VALUE_3.value: "a new value"
         }
 
         # Perform the mapping and validate
         with self.assertRaises(AttributeError):
             TestEnum.map(key_mapping)
 
+    def test_keys_retrieval(self):
+        class TestEnum(EnumWithDict):
+            VALUE_1 = 1
+            VALUE_2 = 2
+            VALUE_3 = 3
+
+        self.assertEqual(TestEnum.keys(), ['VALUE_1', 'VALUE_2', 'VALUE_3'])
+
+        self.assertNotEqual(TestEnum.keys(as_list = False), ['VALUE_1', 'VALUE_2', 'VALUE_3'])
+        self.assertEqual(list(TestEnum.keys(as_list = False)), ['VALUE_1', 'VALUE_2', 'VALUE_3'])
+
+    def test_values_retrieval(self):
+        class TestEnum(EnumWithDict):
+            VALUE_1 = 1
+            VALUE_2 = 2
+            VALUE_3 = 3
+
+        self.assertEqual(TestEnum.values(), [1,2,3])
+
+        self.assertNotEqual(TestEnum.values(as_list = False), [1,2,3])
+        self.assertEqual(list(TestEnum.values(as_list = False)), [1,2,3])
 
 if __name__ == '__main__':
     unittest.main()
```

