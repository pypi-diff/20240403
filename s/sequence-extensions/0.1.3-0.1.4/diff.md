# Comparing `tmp/sequence-extensions-0.1.3.tar.gz` & `tmp/sequence-extensions-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sequence-extensions-0.1.3.tar", last modified: Wed Mar 13 10:56:16 2024, max compression
+gzip compressed data, was "sequence-extensions-0.1.4.tar", last modified: Wed Apr  3 08:30:53 2024, max compression
```

## Comparing `sequence-extensions-0.1.3.tar` & `sequence-extensions-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-03-13 10:56:16.384486 sequence-extensions-0.1.3/
--rw-rw-r--   0 eriro     (1010) eriro     (1010)     1065 2024-03-11 07:41:19.000000 sequence-extensions-0.1.3/LICENSE
--rw-r--r--   0 eriro     (1010) eriro     (1010)      878 2024-03-13 10:56:16.384486 sequence-extensions-0.1.3/PKG-INFO
--rw-rw-r--   0 eriro     (1010) eriro     (1010)      377 2024-03-12 07:55:51.000000 sequence-extensions-0.1.3/README.md
--rw-rw-r--   0 eriro     (1010) eriro     (1010)      479 2024-03-13 10:49:22.000000 sequence-extensions-0.1.3/pyproject.toml
--rw-rw-r--   0 eriro     (1010) eriro     (1010)       38 2024-03-13 10:56:16.384486 sequence-extensions-0.1.3/setup.cfg
-drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-03-13 10:56:16.376486 sequence-extensions-0.1.3/src/
-drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-03-13 10:56:16.380486 sequence-extensions-0.1.3/src/sequence_extensions/
--rw-rw-r--   0 eriro     (1010) eriro     (1010)        0 2024-03-11 08:24:13.000000 sequence-extensions-0.1.3/src/sequence_extensions/__init__.py
--rw-rw-r--   0 eriro     (1010) eriro     (1010)     5222 2024-03-13 10:52:25.000000 sequence-extensions-0.1.3/src/sequence_extensions/ext_list.py
-drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-03-13 10:56:16.384486 sequence-extensions-0.1.3/src/sequence_extensions.egg-info/
--rw-r--r--   0 eriro     (1010) eriro     (1010)      878 2024-03-13 10:56:16.000000 sequence-extensions-0.1.3/src/sequence_extensions.egg-info/PKG-INFO
--rw-rw-r--   0 eriro     (1010) eriro     (1010)      315 2024-03-13 10:56:16.000000 sequence-extensions-0.1.3/src/sequence_extensions.egg-info/SOURCES.txt
--rw-rw-r--   0 eriro     (1010) eriro     (1010)        1 2024-03-13 10:56:16.000000 sequence-extensions-0.1.3/src/sequence_extensions.egg-info/dependency_links.txt
--rw-rw-r--   0 eriro     (1010) eriro     (1010)       20 2024-03-13 10:56:16.000000 sequence-extensions-0.1.3/src/sequence_extensions.egg-info/top_level.txt
-drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-03-13 10:56:16.384486 sequence-extensions-0.1.3/tests/
--rw-rw-r--   0 eriro     (1010) eriro     (1010)     3446 2024-03-13 10:53:01.000000 sequence-extensions-0.1.3/tests/test_list_ext.py
+drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-04-03 08:30:53.247401 sequence-extensions-0.1.4/
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)     1065 2024-03-11 07:41:19.000000 sequence-extensions-0.1.4/LICENSE
+-rw-r--r--   0 eriro     (1010) eriro     (1010)      999 2024-04-03 08:30:53.243401 sequence-extensions-0.1.4/PKG-INFO
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)      499 2024-04-02 06:09:44.000000 sequence-extensions-0.1.4/README.md
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)      479 2024-03-24 13:39:43.000000 sequence-extensions-0.1.4/pyproject.toml
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)       38 2024-04-03 08:30:53.247401 sequence-extensions-0.1.4/setup.cfg
+drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-04-03 08:30:53.235401 sequence-extensions-0.1.4/src/
+drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-04-03 08:30:53.239401 sequence-extensions-0.1.4/src/sequence_extensions/
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)       99 2024-03-20 09:01:43.000000 sequence-extensions-0.1.4/src/sequence_extensions/__init__.py
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)     3794 2024-04-02 06:09:44.000000 sequence-extensions-0.1.4/src/sequence_extensions/dict_ext.py
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)      437 2024-03-26 08:25:35.000000 sequence-extensions-0.1.4/src/sequence_extensions/gen_ext.py
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)     6880 2024-04-02 12:28:45.000000 sequence-extensions-0.1.4/src/sequence_extensions/list_ext.py
+drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-04-03 08:30:53.243401 sequence-extensions-0.1.4/src/sequence_extensions.egg-info/
+-rw-r--r--   0 eriro     (1010) eriro     (1010)      999 2024-04-03 08:30:53.000000 sequence-extensions-0.1.4/src/sequence_extensions.egg-info/PKG-INFO
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)      431 2024-04-03 08:30:53.000000 sequence-extensions-0.1.4/src/sequence_extensions.egg-info/SOURCES.txt
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)        1 2024-04-03 08:30:53.000000 sequence-extensions-0.1.4/src/sequence_extensions.egg-info/dependency_links.txt
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)       20 2024-04-03 08:30:53.000000 sequence-extensions-0.1.4/src/sequence_extensions.egg-info/top_level.txt
+drwxrwxr-x   0 eriro     (1010) eriro     (1010)        0 2024-04-03 08:30:53.243401 sequence-extensions-0.1.4/tests/
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)     3153 2024-04-02 06:09:44.000000 sequence-extensions-0.1.4/tests/test_dict_ext.py
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)     1041 2024-03-26 08:25:46.000000 sequence-extensions-0.1.4/tests/test_gen_ext.py
+-rw-rw-r--   0 eriro     (1010) eriro     (1010)     4458 2024-04-02 12:29:45.000000 sequence-extensions-0.1.4/tests/test_list_ext.py
```

### Comparing `sequence-extensions-0.1.3/LICENSE` & `sequence-extensions-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sequence-extensions-0.1.3/PKG-INFO` & `sequence-extensions-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequence-extensions
-Version: 0.1.3
+Version: 0.1.4
 Summary: Higher order functions extension functins
 Author: jkCXf9X4
 Project-URL: Homepage, https://github.com/jkCXf9X4/sequence_extensions
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 # sequence_extensions
 
 provides high order functions as extesions for the custom list class in python
 
 ```python 
-l = ext_list([1, 2, 3, 4])
+l = list_ext([1, 2, 3, 4])
 
 l.map(lambda x: x*2)
 [2, 4, 6, 8]
 
 l.filter(lambda x: x%2==0)
 [2, 4]
 
@@ -40,7 +40,18 @@
 l.to_strings()
 ["1", "2", "3", "4"]
 
 l.to_string()
 "1, 2, 3, 4"
 
 ```
+
+
+for develompment install 
+pip install -e .
+
+to run tests
+pytest
+
+To generate coverage
+pytest --cov  --cov-report html
+
```

### Comparing `sequence-extensions-0.1.3/src/sequence_extensions/ext_list.py` & `sequence-extensions-0.1.4/src/sequence_extensions/list_ext.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # this code is free to use, copy, change and do anything that c
 
+from collections import ChainMap
 from functools import reduce
+from statistics import mean
 
 
-class ext_list(list):
+class list_ext(list):
+    """
+    Extend the normal list class
+    """
 
     def map(self, func):
         """
         Map function over the list
         func(x) -> y
 
-        ext_list(map(func, list))
+        list_ext(map(func, list))
         """
         return type(self)(map(func, self))
 
     def filter(self, func):
         """
         Filter the list using func
         func(x) -> bool
 
-        ext_list(filter(func, list))
+        list_ext(filter(func, list))
         """
         return type(self)(filter(func, self))
 
     def reduce(self, func):
         """
         Reduce the list
         func(a, b) -> c
@@ -32,24 +37,43 @@
         """
         return reduce(func, self)
 
     def zip(self, *iterables):
         """
         Zip list together with iterables
 
-        ext_list(zip(self, *iterables))
+        list_ext(zip(self, *iterables))
         """
         return type(self)(zip(self, *iterables))
 
-    def for_each(self, func):
+    def for_each(self, func) -> None:
         """
         Execute function on each item in list
         [func(i) for i in list]
         """
-        [func(i) for i in self]
+        self.map(func)
+
+    def rolling(self, n=2):
+        """
+        [[a1, a2], [a2, a3],...]
+        """
+        return type(self)([self[i : i + n] for i in range(len(self) - n + 1)])
+
+    def rolling_map(self, func=None, n=2):
+        """
+        Apply func to a sliding/rolling window of size n
+        [a1, a2, a3, a4, ...]
+
+        for n=2
+        [func(a1, a2), func(a2, a3),...]
+        n=3
+        [func(a1, a2, a3), func(a2, a3, a4),...]
+
+        """
+        return type(self)(self.rolling(n=n).map(lambda x: func(*x)))
 
     @staticmethod
     def execute_or_default(func, default=None, exception=Exception):
         """
         Try to execute function, return default if exception is raised
         """
         try:
@@ -102,15 +126,15 @@
         """
         l = self.filter(func) if func != None else self
 
         return l.get_item_or_default(index=-1, default=default)
 
     def to_type(self, t):
         """
-        ext_list([t(x) for x in list])
+        list_ext([t(x) for x in list])
         """
         return type(self)([t(i) for i in self])
 
     def to_strings(self):
         """
         Convert all items to their string equvalent
         """
@@ -139,33 +163,57 @@
 
     def to_tuple(self):
         """
         Convert to tuple
         """
         return tuple(self)
 
-    def to_dict(self, keys):
+    def to_dict_key(self, keys):
+        """
+        Convert to dict
+        """
+        from sequence_extensions import dict_ext
+
+        return dict_ext((j, i) for i, j in self.zip(keys))
+
+    def to_dict_value(self, values):
         """
         Convert to dict
         """
-        return {j: i for i, j in self.zip(keys)}
+        from sequence_extensions import dict_ext
 
-    def all(self, func) -> bool:
+        return dict_ext((i, j) for i, j in self.zip(values))
+
+    def to_dict_fn(self, key_func=None, value_func=None):
+        """
+        Convert to dict using a
+        {func(i): i for i in self}
+        """
+        from sequence_extensions import dict_ext
+
+        def f(i):
+            k = key_func(i) if key_func else i
+            v = value_func(i) if value_func else i
+            return (k, v)
+
+        return dict_ext(f(i) for i in self)
+
+    def all(self, func=None) -> bool:
         """
         Check if all items fullfill the condition
         """
-        l = self.map(func)
+        l = self.map(func) if func != None else self
         return all(l)
 
-    def any(self, func) -> bool:
+    def any(self, func=None) -> bool:
         """
         Check if at least one item fullfill the condition
 
         """
-        l = self.map(func)
+        l = self.map(func) if func != None else self
         return any(l)
 
     def contains(self, x) -> bool:
         """
         Check if x is an item in the list
         """
         return x in self
@@ -201,7 +249,24 @@
         return type(self)(set(self) & set(l))
 
     def union(self, l):
         """
         Return a list of the set containing all the items
         """
         return type(self)(set(self) | set(l))
+
+    def chainmap(self: list[dict]):
+        """
+        Chain multiple dicts together
+        """
+        from sequence_extensions import dict_ext
+
+        return dict_ext(ChainMap(*self))
+
+    def average(self):
+        return mean(self)
+
+    def max(self):
+        return max(self)
+
+    def min(self):
+        return min(self)
```

### Comparing `sequence-extensions-0.1.3/src/sequence_extensions.egg-info/PKG-INFO` & `sequence-extensions-0.1.4/src/sequence_extensions.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sequence-extensions
-Version: 0.1.3
+Version: 0.1.4
 Summary: Higher order functions extension functins
 Author: jkCXf9X4
 Project-URL: Homepage, https://github.com/jkCXf9X4/sequence_extensions
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -13,15 +13,15 @@
 License-File: LICENSE
 
 # sequence_extensions
 
 provides high order functions as extesions for the custom list class in python
 
 ```python 
-l = ext_list([1, 2, 3, 4])
+l = list_ext([1, 2, 3, 4])
 
 l.map(lambda x: x*2)
 [2, 4, 6, 8]
 
 l.filter(lambda x: x%2==0)
 [2, 4]
 
@@ -40,7 +40,18 @@
 l.to_strings()
 ["1", "2", "3", "4"]
 
 l.to_string()
 "1, 2, 3, 4"
 
 ```
+
+
+for develompment install 
+pip install -e .
+
+to run tests
+pytest
+
+To generate coverage
+pytest --cov  --cov-report html
+
```

### Comparing `sequence-extensions-0.1.3/tests/test_list_ext.py` & `sequence-extensions-0.1.4/tests/test_list_ext.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import pytest
-from sequence_extensions.ext_list import ext_list
+from sequence_extensions import list_ext
 
 
 @pytest.fixture
 def simple_int_list():
-    return ext_list([1, 2, 3, 4])
+    return list_ext([1, 2, 3, 4])
 
 
 @pytest.fixture
 def empty_list():
-    return ext_list([])
+    return list_ext([])
 
 
 def test_init_1():
-    l1 = ext_list([1, 2, 3, 4])
+    l1 = list_ext([1, 2, 3, 4])
     assert l1[0] == 1
 
-    l2 = ext_list()
+    l2 = list_ext()
     l2.append(1)
     assert l2[0] == 1
 
 
 def test_map(simple_int_list):
     b = simple_int_list.map(lambda x: x * 2)
 
@@ -39,15 +39,15 @@
 
     b = simple_int_list.reduce(_max)
 
     assert b == 4
 
 
 def test_zip():
-    a = ext_list([1, 2])
+    a = list_ext([1, 2])
 
     b = [1, 2]
 
     c = a.zip(b)
 
     assert c == [(1, 1), (2, 2)]
 
@@ -115,47 +115,66 @@
 def test_to_string_pre(simple_int_list):
 
     s = simple_int_list.to_string(pre=True)
     assert s == ", 1, 2, 3, 4"
 
 
 def test_of_type():
-    l = ext_list([1, "2"])
+    l = list_ext([1, "2"])
     assert l.of_type(str) == ["2"]
 
 
 def test_to_set(simple_int_list):
     assert {1, 2, 3, 4} == simple_int_list.to_set()
 
 
 def test_to_tuple(simple_int_list):
     assert (1, 2, 3, 4) == simple_int_list.to_tuple()
 
 
 def test_to_dict(simple_int_list):
-    d = simple_int_list.to_dict(["a", "b", "c", "d"])
+    d = simple_int_list.to_dict_key(["a", "b", "c", "d"])
 
     assert d == {"a": 1, "b": 2, "c": 3, "d": 4}
 
+    assert d.inverse() == simple_int_list.to_dict_value(["a", "b", "c", "d"])
+
+
+
+def test_to_dict_fn(simple_int_list):
+    d = simple_int_list.to_dict_fn(value_func=lambda x: x * 2)
+
+    assert d == {1: 2, 2: 4, 3: 6, 4: 8}
+
 
 def test_all(simple_int_list):
     results = simple_int_list.all(lambda x: True)
     assert results == True
 
     results = simple_int_list.all(lambda x: False)
     assert results == False
 
+    l1 = list_ext([True, True])
+    assert l1.all() == True
+    l2 = list_ext([True, False])
+    assert l2.all() == False
+
 
 def test_any(simple_int_list):
     results = simple_int_list.any(lambda x: x == 1)
     assert results == True
 
     results = simple_int_list.any(lambda x: x == 6)
     assert results == False
 
+    l1 = list_ext([True, True])
+    assert l1.any() == True
+    l2 = list_ext([True, False])
+    assert l2.any() == True
+
 
 def test_contains(simple_int_list):
     assert simple_int_list.contains(4)
     assert not simple_int_list.contains(5)
 
 
 def test_is_empty(simple_int_list, empty_list):
@@ -165,11 +184,40 @@
 
 def test_single(simple_int_list):
     assert not simple_int_list.is_single()
 
     l = simple_int_list.single(lambda x: x == 2)
     assert l == 2
 
-    assert ext_list([2]).single() == 2
+    assert list_ext([2]).single() == 2
 
     with pytest.raises(Exception):
         l = simple_int_list.single(lambda x: x % 2 == 0)
+
+
+def test_chainmap():
+
+    l = list_ext([{"a": 1}, {"b": 2}, {"c": 3}])
+
+    d = l.chainmap()
+
+    assert d == {"a": 1, "b": 2, "c": 3}
+
+
+def test_rolling_map(simple_int_list):
+    def f(a, b):
+        return a + b
+
+    assert simple_int_list.rolling_map(f) == [3, 5, 7]
+
+    def f(a, b, c):
+        return a + b + c
+
+    assert simple_int_list.rolling_map(f, n=3) == [6, 9]
+
+
+def test_rolling(simple_int_list):
+
+
+    assert simple_int_list.rolling() == [[1, 2], [2, 3], [3, 4]]
+
+    assert simple_int_list.rolling(n=3) == [[1, 2, 3], [2, 3, 4]]
```

