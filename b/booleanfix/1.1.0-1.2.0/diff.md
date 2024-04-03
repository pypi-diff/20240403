# Comparing `tmp/booleanfix-1.1.0.tar.gz` & `tmp/booleanfix-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "booleanfix-1.1.0.tar", last modified: Sat Oct 14 12:18:00 2023, max compression
+gzip compressed data, was "booleanfix-1.2.0.tar", last modified: Wed Apr  3 14:55:18 2024, max compression
```

## Comparing `booleanfix-1.1.0.tar` & `booleanfix-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-10-14 12:18:00.643729 booleanfix-1.1.0/
--rw-rw-rw-   0        0        0     1084 2023-10-14 08:10:18.000000 booleanfix-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4393 2023-10-14 12:18:00.641152 booleanfix-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-10-14 12:16:05.000000 booleanfix-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-10-14 12:18:00.623344 booleanfix-1.1.0/booleanfix/
--rw-rw-rw-   0        0        0       87 2023-10-14 11:49:32.000000 booleanfix-1.1.0/booleanfix/__init__.py
-drwxrwxrwx   0        0        0        0 2023-10-14 12:18:00.632919 booleanfix-1.1.0/booleanfix.egg-info/
--rw-rw-rw-   0        0        0     4393 2023-10-14 12:18:00.000000 booleanfix-1.1.0/booleanfix.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2023-10-14 12:18:00.000000 booleanfix-1.1.0/booleanfix.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-14 12:18:00.000000 booleanfix-1.1.0/booleanfix.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-10-14 12:18:00.000000 booleanfix-1.1.0/booleanfix.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      811 2023-10-14 12:13:48.000000 booleanfix-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-10-14 12:18:00.645181 booleanfix-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1032 2023-10-14 12:01:00.000000 booleanfix-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-14 12:18:00.638113 booleanfix-1.1.0/tests/
--rw-rw-rw-   0        0        0     2913 2023-10-14 12:07:49.000000 booleanfix-1.1.0/tests/test_booleanfix.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:55:18.775081 booleanfix-1.2.0/
+-rw-rw-rw-   0        0        0     1084 2023-10-14 08:10:18.000000 booleanfix-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4595 2024-04-03 14:55:18.773068 booleanfix-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2416 2024-04-03 14:53:40.000000 booleanfix-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 14:55:18.762066 booleanfix-1.2.0/booleanfix/
+-rw-rw-rw-   0        0        0      100 2024-04-03 14:42:26.000000 booleanfix-1.2.0/booleanfix/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:55:18.772082 booleanfix-1.2.0/booleanfix.egg-info/
+-rw-rw-rw-   0        0        0     4595 2024-04-03 14:55:18.000000 booleanfix-1.2.0/booleanfix.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-04-03 14:55:18.000000 booleanfix-1.2.0/booleanfix.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 14:55:18.000000 booleanfix-1.2.0/booleanfix.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-03 14:55:18.000000 booleanfix-1.2.0/booleanfix.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      811 2024-04-03 14:54:20.000000 booleanfix-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 14:55:18.775081 booleanfix-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1032 2024-04-03 14:54:37.000000 booleanfix-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:55:18.770073 booleanfix-1.2.0/tests/
+-rw-rw-rw-   0        0        0     3831 2024-04-03 14:50:52.000000 booleanfix-1.2.0/tests/test_booleanfix.py
```

### Comparing `booleanfix-1.1.0/LICENSE` & `booleanfix-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `booleanfix-1.1.0/PKG-INFO` & `booleanfix-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: booleanfix
-Version: 1.1.0
+Version: 1.2.0
 Summary: Fix for boolean variables in Python
 Home-page: https://github.com/EDM115/booleanfix
 Author: EDM115
 Author-email: EDM115 <dev@edm115.eu.org>
 License: MIT License
         
         Copyright (c) 2023 EDM115
@@ -39,72 +39,83 @@
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # booleanfix
 
 The most useless pip package so far  
-[![PyPI version](https://badge.fury.io/py/booleanfix.svg)](https://pypi.org/project/booleanfix)
+![PyPI - Version](https://img.shields.io/pypi/v/booleanfix) ![PyPI - Downloads](https://img.shields.io/pypi/dm/booleanfix) ![Pepy Total Downlods](https://img.shields.io/pepy/dt/booleanfix)
   
 ## The problem
 
 If you come from another programming language, you may have noticed that Python's boolean variables are a bit different. This module aims to fix that, by giving you boolean variables like you're used to.
 
 ## The solution
 
 This very simple project gives you boolean variables like you're used to. It's as simple as that.  
-*Note* : Since v1.1.0, booleanfix also allows you to use `null` and `undefined` as `None`.
+
+> [!NOTE]
+> v1.1.0 added the ability to use `null` and `undefined` as `None`.
+> v1.2.0 added the ability to use `none` as `None`.
 
 #### Behind the scenes
 
 ```python
 true = True
 false = False
+none = None
 null = None
 undefined = None
 ```
 
 ## Usage
 
 1. Install the package in your repo
 
 ```bash
-pip install booleanfix==1.1.0
+pip install booleanfix
 ```
 
 **If you use a requirements file, add this line to it :**
 
 ```bash
-booleanfix==1.1.0
+booleanfix==1.2.0
 ```
 
-1. Use it in your code
+1. The classic way
 
-	a. The classic way
+```python
+import booleanfix as bf
 
-	```python
-	import booleanfix as bf
+print(isinstance(bf.true, bool))
+print(bf.false == False)
+```
 
-	print(isinstance(bf.true, bool))
-	print(bf.false == False)
-	```
+2. The easy way
 
-	b. The easy way
+```python
+from booleanfix import true, false
 
-	```python
-	from booleanfix import true, false
+print(isinstance(true, bool))
+print(false == False)
+```
 
-	print(isinstance(true, bool))
-	print(false == False)
-	```
+3. The all-in-one way
+
+```python
+from booleanfix import *
+
+print(isinstance(true, bool))
+print(false == False)
+```
 
 ## Example
 
 ```python
-from booleanfix import true, false, null, undefined
+from booleanfix import *
 
 array = [1, 2, 3, 4, 5]
 for i in range(len((array))):
 	if array[i] % 2 == 0:
 		array[i] = true
 	else:
 		array[i] = false
```

### Comparing `booleanfix-1.1.0/README.md` & `booleanfix-1.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,111 +1,122 @@
-# booleanfix
-
-The most useless pip package so far  
-[![PyPI version](https://badge.fury.io/py/booleanfix.svg)](https://pypi.org/project/booleanfix)
-  
-## The problem
-
-If you come from another programming language, you may have noticed that Python's boolean variables are a bit different. This module aims to fix that, by giving you boolean variables like you're used to.
-
-## The solution
-
-This very simple project gives you boolean variables like you're used to. It's as simple as that.  
-*Note* : Since v1.1.0, booleanfix also allows you to use `null` and `undefined` as `None`.
-
-#### Behind the scenes
-
-```python
-true = True
-false = False
-null = None
-undefined = None
-```
-
-## Usage
-
-1. Install the package in your repo
-
-```bash
-pip install booleanfix==1.1.0
-```
-
-**If you use a requirements file, add this line to it :**
-
-```bash
-booleanfix==1.1.0
-```
-
-1. Use it in your code
-
-	a. The classic way
-
-	```python
-	import booleanfix as bf
-
-	print(isinstance(bf.true, bool))
-	print(bf.false == False)
-	```
-
-	b. The easy way
-
-	```python
-	from booleanfix import true, false
-
-	print(isinstance(true, bool))
-	print(false == False)
-	```
-
-## Example
-
-```python
-from booleanfix import true, false, null, undefined
-
-array = [1, 2, 3, 4, 5]
-for i in range(len((array))):
-	if array[i] % 2 == 0:
-		array[i] = true
-	else:
-		array[i] = false
-
-print(array)
-
-for i in array:
-	print(type(i), isinstance(i, bool), i)
-
-if null == undefined:
-	print("null == undefined")
-
-if array[5] == null:
-	print("array[5] == null")
-```
-
-## Contributing
-
-Feel free to open an [issue](https://github.com/EDM115/booleanfix/issues) or a [pull request](https://github.com/EDM115/booleanfix/pulls) if you want to contribute to this project
-
-### How to build ?
-
-```bash
-py -m pip install --upgrade pip build twine setuptools wheel
-py -m build
-py -m twine check dist/*
-# Optional : publish to test.pypi.org
-py -m twine upload --repository testpypi dist/*
-# Or to pypi.org
-py -m twine upload dist/*
-```
-
-### How to test ?
-
-```bash
-py -m pip install --upgrade pytest
-py -m pytest
-```
-
-## License
-
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-## Authors
-
-* **EDM115** - *Initial work* - [EDM115](https://github.com/EDM115)
+# booleanfix
+
+The most useless pip package so far  
+![PyPI - Version](https://img.shields.io/pypi/v/booleanfix) ![PyPI - Downloads](https://img.shields.io/pypi/dm/booleanfix) ![Pepy Total Downlods](https://img.shields.io/pepy/dt/booleanfix)
+  
+## The problem
+
+If you come from another programming language, you may have noticed that Python's boolean variables are a bit different. This module aims to fix that, by giving you boolean variables like you're used to.
+
+## The solution
+
+This very simple project gives you boolean variables like you're used to. It's as simple as that.  
+
+> [!NOTE]
+> v1.1.0 added the ability to use `null` and `undefined` as `None`.
+> v1.2.0 added the ability to use `none` as `None`.
+
+#### Behind the scenes
+
+```python
+true = True
+false = False
+none = None
+null = None
+undefined = None
+```
+
+## Usage
+
+1. Install the package in your repo
+
+```bash
+pip install booleanfix
+```
+
+**If you use a requirements file, add this line to it :**
+
+```bash
+booleanfix==1.2.0
+```
+
+1. The classic way
+
+```python
+import booleanfix as bf
+
+print(isinstance(bf.true, bool))
+print(bf.false == False)
+```
+
+2. The easy way
+
+```python
+from booleanfix import true, false
+
+print(isinstance(true, bool))
+print(false == False)
+```
+
+3. The all-in-one way
+
+```python
+from booleanfix import *
+
+print(isinstance(true, bool))
+print(false == False)
+```
+
+## Example
+
+```python
+from booleanfix import *
+
+array = [1, 2, 3, 4, 5]
+for i in range(len((array))):
+	if array[i] % 2 == 0:
+		array[i] = true
+	else:
+		array[i] = false
+
+print(array)
+
+for i in array:
+	print(type(i), isinstance(i, bool), i)
+
+if null == undefined:
+	print("null == undefined")
+
+if array[5] == null:
+	print("array[5] == null")
+```
+
+## Contributing
+
+Feel free to open an [issue](https://github.com/EDM115/booleanfix/issues) or a [pull request](https://github.com/EDM115/booleanfix/pulls) if you want to contribute to this project
+
+### How to build ?
+
+```bash
+py -m pip install --upgrade pip build twine setuptools wheel
+py -m build
+py -m twine check dist/*
+# Optional : publish to test.pypi.org
+py -m twine upload --repository testpypi dist/*
+# Or to pypi.org
+py -m twine upload dist/*
+```
+
+### How to test ?
+
+```bash
+py -m pip install --upgrade pytest
+py -m pytest
+```
+
+## License
+
+This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
+
+## Authors
+
+* **EDM115** - *Initial work* - [EDM115](https://github.com/EDM115)
```

### Comparing `booleanfix-1.1.0/booleanfix.egg-info/PKG-INFO` & `booleanfix-1.2.0/booleanfix.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: booleanfix
-Version: 1.1.0
+Version: 1.2.0
 Summary: Fix for boolean variables in Python
 Home-page: https://github.com/EDM115/booleanfix
 Author: EDM115
 Author-email: EDM115 <dev@edm115.eu.org>
 License: MIT License
         
         Copyright (c) 2023 EDM115
@@ -39,72 +39,83 @@
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # booleanfix
 
 The most useless pip package so far  
-[![PyPI version](https://badge.fury.io/py/booleanfix.svg)](https://pypi.org/project/booleanfix)
+![PyPI - Version](https://img.shields.io/pypi/v/booleanfix) ![PyPI - Downloads](https://img.shields.io/pypi/dm/booleanfix) ![Pepy Total Downlods](https://img.shields.io/pepy/dt/booleanfix)
   
 ## The problem
 
 If you come from another programming language, you may have noticed that Python's boolean variables are a bit different. This module aims to fix that, by giving you boolean variables like you're used to.
 
 ## The solution
 
 This very simple project gives you boolean variables like you're used to. It's as simple as that.  
-*Note* : Since v1.1.0, booleanfix also allows you to use `null` and `undefined` as `None`.
+
+> [!NOTE]
+> v1.1.0 added the ability to use `null` and `undefined` as `None`.
+> v1.2.0 added the ability to use `none` as `None`.
 
 #### Behind the scenes
 
 ```python
 true = True
 false = False
+none = None
 null = None
 undefined = None
 ```
 
 ## Usage
 
 1. Install the package in your repo
 
 ```bash
-pip install booleanfix==1.1.0
+pip install booleanfix
 ```
 
 **If you use a requirements file, add this line to it :**
 
 ```bash
-booleanfix==1.1.0
+booleanfix==1.2.0
 ```
 
-1. Use it in your code
+1. The classic way
 
-	a. The classic way
+```python
+import booleanfix as bf
 
-	```python
-	import booleanfix as bf
+print(isinstance(bf.true, bool))
+print(bf.false == False)
+```
 
-	print(isinstance(bf.true, bool))
-	print(bf.false == False)
-	```
+2. The easy way
 
-	b. The easy way
+```python
+from booleanfix import true, false
 
-	```python
-	from booleanfix import true, false
+print(isinstance(true, bool))
+print(false == False)
+```
 
-	print(isinstance(true, bool))
-	print(false == False)
-	```
+3. The all-in-one way
+
+```python
+from booleanfix import *
+
+print(isinstance(true, bool))
+print(false == False)
+```
 
 ## Example
 
 ```python
-from booleanfix import true, false, null, undefined
+from booleanfix import *
 
 array = [1, 2, 3, 4, 5]
 for i in range(len((array))):
 	if array[i] % 2 == 0:
 		array[i] = true
 	else:
 		array[i] = false
```

### Comparing `booleanfix-1.1.0/pyproject.toml` & `booleanfix-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "booleanfix"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="EDM115", email="dev@edm115.eu.org" },
 ]
 description = "Fix for boolean variables in Python"
 readme = "README.md"
 license = {file = "LICENSE"}
 keywords = ["boolean", "fix", "python"]
```

### Comparing `booleanfix-1.1.0/setup.py` & `booleanfix-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="booleanfix",
-    version="1.1.0",
+    version="1.2.0",
     description="Fix for boolean variables in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EDM115/booleanfix",
     author="EDM115",
     license="MIT",
     classifiers=[
```

### Comparing `booleanfix-1.1.0/tests/test_booleanfix.py` & `booleanfix-1.2.0/tests/test_booleanfix.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from booleanfix import true, false, null, undefined
+from booleanfix import *
 
 def test_true():
     assert true
 
 
 def test_false():
     assert not false
@@ -82,30 +82,66 @@
     assert null is None
 
 
 def test_undefined():
     assert undefined is None
 
 
+def test_none():
+    assert None is null
+
+
 def test_null_undefined():
     assert null == undefined
 
 
 def test_null_is_undefined():
     assert null is undefined
 
 
+def test_null_none():
+    assert null == none
+
+
+def test_null_is_none():
+    assert null is none
+
+
 def test_undefined_null():
 	assert undefined == null
 
 
 def test_undefined_is_null():
 	assert undefined is null
 
 
+def test_undefined_none():
+    assert undefined == none
+
+
+def test_undefined_is_none():
+    assert undefined is none
+
+
+def test_none_null():
+    assert none == null
+
+
+def test_none_is_null():
+    assert none is null
+
+
+def test_none_undefined():
+    assert none == undefined
+
+
+def test_none_is_undefined():
+    assert none is undefined
+
+
 def test_null_true():
 	assert null != true
 
 
 def test_null_false():
 	assert null != false
 
@@ -114,14 +150,22 @@
 	assert undefined != true
 
 
 def test_undefined_false():
 	assert undefined != false
 
 
+def test_none_true():
+    assert none != true
+
+
+def test_none_false():
+    assert none != false
+
+
 def test_array_manipulation():
     array = [1, 2, 3, 4, 5]
     for i in range(len((array))):
         if array[i] % 2 == 0:
             array[i] = true
         else:
             array[i] = false
@@ -154,7 +198,23 @@
 
 def test_array_null_comparison():
     array = [1, 2, 3, 4, 5]
     array.append(null)
 
     assert array[5] == null
     assert array[5] is null
+
+
+def test_array_undefined_comparison():
+    array = [1, 2, 3, 4, 5]
+    array.append(undefined)
+
+    assert array[5] == undefined
+    assert array[5] is undefined
+
+
+def test_array_none_comparison():
+    array = [1, 2, 3, 4, 5]
+    array.append(none)
+
+    assert array[5] == none
+    assert array[5] is none
```

