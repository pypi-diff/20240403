# Comparing `tmp/enum_with_dict-0.1.0.tar.gz` & `tmp/enum_with_dict-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_with_dict-0.1.0.tar", last modified: Wed Apr  3 18:23:48 2024, max compression
+gzip compressed data, was "enum_with_dict-0.1.1.tar", last modified: Wed Apr  3 18:41:29 2024, max compression
```

## Comparing `enum_with_dict-0.1.0.tar` & `enum_with_dict-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 18:23:48.561942 enum_with_dict-0.1.0/
--rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.1.0/LICENSE
--rw-r--r--   0 administrator   (501) staff       (20)     1695 2024-04-03 18:23:48.561822 enum_with_dict-0.1.0/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      734 2024-04-03 18:13:22.000000 enum_with_dict-0.1.0/README.md
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 18:23:48.560945 enum_with_dict-0.1.0/enum_with_dict/
--rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.1.0/enum_with_dict/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)      367 2024-04-03 17:47:28.000000 enum_with_dict-0.1.0/enum_with_dict/enum_with_dict.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 18:23:48.561438 enum_with_dict-0.1.0/enum_with_dict.egg-info/
--rw-r--r--   0 administrator   (501) staff       (20)     1695 2024-04-03 18:23:48.000000 enum_with_dict-0.1.0/enum_with_dict.egg-info/PKG-INFO
--rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 18:23:48.000000 enum_with_dict-0.1.0/enum_with_dict.egg-info/SOURCES.txt
--rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 18:23:48.000000 enum_with_dict-0.1.0/enum_with_dict.egg-info/dependency_links.txt
--rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 18:23:48.000000 enum_with_dict-0.1.0/enum_with_dict.egg-info/top_level.txt
--rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 18:23:48.561977 enum_with_dict-0.1.0/setup.cfg
--rw-r--r--   0 administrator   (501) staff       (20)     1123 2024-04-03 17:57:15.000000 enum_with_dict-0.1.0/setup.py
-drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 18:23:48.561662 enum_with_dict-0.1.0/test/
--rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.1.0/test/__init__.py
--rw-r--r--   0 administrator   (501) staff       (20)     1444 2024-04-03 17:50:23.000000 enum_with_dict-0.1.0/test/test_enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 18:41:29.957371 enum_with_dict-0.1.1/
+-rw-r--r--   0 administrator   (501) staff       (20)     1070 2024-04-03 17:59:38.000000 enum_with_dict-0.1.1/LICENSE
+-rw-r--r--   0 administrator   (501) staff       (20)     2206 2024-04-03 18:41:29.957171 enum_with_dict-0.1.1/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)     1295 2024-04-03 18:35:00.000000 enum_with_dict-0.1.1/README.md
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 18:41:29.956209 enum_with_dict-0.1.1/enum_with_dict/
+-rw-r--r--   0 administrator   (501) staff       (20)       41 2024-04-03 17:23:01.000000 enum_with_dict-0.1.1/enum_with_dict/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)      367 2024-04-03 17:47:28.000000 enum_with_dict-0.1.1/enum_with_dict/enum_with_dict.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 18:41:29.956678 enum_with_dict-0.1.1/enum_with_dict.egg-info/
+-rw-r--r--   0 administrator   (501) staff       (20)     2206 2024-04-03 18:41:29.000000 enum_with_dict-0.1.1/enum_with_dict.egg-info/PKG-INFO
+-rw-r--r--   0 administrator   (501) staff       (20)      283 2024-04-03 18:41:29.000000 enum_with_dict-0.1.1/enum_with_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 administrator   (501) staff       (20)        1 2024-04-03 18:41:29.000000 enum_with_dict-0.1.1/enum_with_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       20 2024-04-03 18:41:29.000000 enum_with_dict-0.1.1/enum_with_dict.egg-info/top_level.txt
+-rw-r--r--   0 administrator   (501) staff       (20)       38 2024-04-03 18:41:29.957409 enum_with_dict-0.1.1/setup.cfg
+-rw-r--r--   0 administrator   (501) staff       (20)     1074 2024-04-03 18:41:07.000000 enum_with_dict-0.1.1/setup.py
+drwxr-xr-x   0 administrator   (501) staff       (20)        0 2024-04-03 18:41:29.956894 enum_with_dict-0.1.1/test/
+-rw-r--r--   0 administrator   (501) staff       (20)        0 2024-04-03 17:24:07.000000 enum_with_dict-0.1.1/test/__init__.py
+-rw-r--r--   0 administrator   (501) staff       (20)     1444 2024-04-03 17:50:23.000000 enum_with_dict-0.1.1/test/test_enum_with_dict.py
```

### Comparing `enum_with_dict-0.1.0/LICENSE` & `enum_with_dict-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_with_dict-0.1.0/PKG-INFO` & `enum_with_dict-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: enum_with_dict
-Version: 0.1.0
+Version: 0.1.1
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EnumWithDict
 
 `EnumWithDict` is a Python package that extends the standard library's `Enum` class to include `to_dict` and `get_initial` class methods. This enhancement allows for straightforward conversion of enum classes to dictionaries and provides easy access to the initial enum value, facilitating a more versatile use of enumerations in Python applications.
 
@@ -36,10 +35,41 @@
 
 Install `EnumWithDict` using pip:
 
 ```bash
 pip install enum_with_dict
 ```
 
+## Usage
+
+### Defining an Enum with `EnumWithDict`
+
+```python
+from enum_with_dict import EnumWithDict
+
+class Color(EnumWithDict):
+    RED = 'red'
+    GREEN = 'green'
+    BLUE = 'blue'
+
+```
+
+### Converting an Enum to a Dictionary
+
+```python
+color_dict = Color.to_dict()
+print(color_dict)
+# Output: {'RED': 'red', 'GREEN': 'green', 'BLUE': 'blue'}
+```
+
+### Getting the Initial Enum Value
+
+```python
+initial_color = Color.get_initial()
+print(initial_color)
+# Output: 'red'
+```
+
 ## LICENSE
 
-[MIT](LICENSE)
+`EnumWithDict` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
+
```

### Comparing `enum_with_dict-0.1.0/enum_with_dict.egg-info/PKG-INFO` & `enum_with_dict-0.1.1/enum_with_dict.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: enum-with-dict
-Version: 0.1.0
+Version: 0.1.1
 Summary: Enum with to_dict method.
 Home-page: https://github.com/jzombie/enum_with_dict
 Author: Jeremy Harris
 Author-email: jeremy.harris@zenosmosis.com
 License: MIT
 Keywords: enum python utilities enum-to-dict enum-with-dict
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # EnumWithDict
 
 `EnumWithDict` is a Python package that extends the standard library's `Enum` class to include `to_dict` and `get_initial` class methods. This enhancement allows for straightforward conversion of enum classes to dictionaries and provides easy access to the initial enum value, facilitating a more versatile use of enumerations in Python applications.
 
@@ -36,10 +35,41 @@
 
 Install `EnumWithDict` using pip:
 
 ```bash
 pip install enum_with_dict
 ```
 
+## Usage
+
+### Defining an Enum with `EnumWithDict`
+
+```python
+from enum_with_dict import EnumWithDict
+
+class Color(EnumWithDict):
+    RED = 'red'
+    GREEN = 'green'
+    BLUE = 'blue'
+
+```
+
+### Converting an Enum to a Dictionary
+
+```python
+color_dict = Color.to_dict()
+print(color_dict)
+# Output: {'RED': 'red', 'GREEN': 'green', 'BLUE': 'blue'}
+```
+
+### Getting the Initial Enum Value
+
+```python
+initial_color = Color.get_initial()
+print(initial_color)
+# Output: 'red'
+```
+
 ## LICENSE
 
-[MIT](LICENSE)
+`EnumWithDict` is released under the MIT License. See the [LICENSE](LICENSE) file for more details.
+
```

### Comparing `enum_with_dict-0.1.0/setup.py` & `enum_with_dict-0.1.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='enum_with_dict',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     author='Jeremy Harris',
     author_email='jeremy.harris@zenosmosis.com',
     description='Enum with to_dict method.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/jzombie/enum_with_dict',
     license='MIT',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     keywords='enum python utilities enum-to-dict enum-with-dict',
 )
```

### Comparing `enum_with_dict-0.1.0/test/test_enum_with_dict.py` & `enum_with_dict-0.1.1/test/test_enum_with_dict.py`

 * *Files identical despite different names*

