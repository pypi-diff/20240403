# Comparing `tmp/inverters-0.0.4.tar.gz` & `tmp/inverters-0.0.5.tar.gz`

## Comparing `inverters-0.0.4.tar` & `inverters-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 inverters-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 inverters-0.0.4/src/inverters/__about__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 inverters-0.0.4/src/inverters/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 inverters-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 inverters-0.0.4/tests/init_test.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 inverters-0.0.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 inverters-0.0.4/LICENSE
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 inverters-0.0.4/README.md
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 inverters-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 inverters-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 inverters-0.0.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 inverters-0.0.5/src/inverters/__about__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 inverters-0.0.5/src/inverters/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 inverters-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 inverters-0.0.5/tests/init_test.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 inverters-0.0.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 inverters-0.0.5/LICENSE
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 inverters-0.0.5/README.md
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 inverters-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 inverters-0.0.5/PKG-INFO
```

### Comparing `inverters-0.0.4/.github/workflows/publish.yml` & `inverters-0.0.5/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `inverters-0.0.4/LICENSE` & `inverters-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `inverters-0.0.4/pyproject.toml` & `inverters-0.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 description = ''
 readme = "README.md"
 requires-python = ">=3.8"
 license = "apache-2.0"
 keywords = []
 authors = [
   { name = "Arturas Aleksandraus", email = "arturas@aleksandraus.se" },
+  { name = "Nithesh Chandher Karthikeyan", email = "nithesh.chandher.karthikeyan@liu.se" },
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
```

### Comparing `inverters-0.0.4/PKG-INFO` & `inverters-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.3
 Name: inverters
-Version: 0.0.4
+Version: 0.0.5
 Project-URL: Documentation, https://github.com/Arty-Facts/inverters#readme
 Project-URL: Issues, https://github.com/Arty-Facts/inverters/issues
 Project-URL: Source, https://github.com/Arty-Facts/inverters
-Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>
+Author-email: Arturas Aleksandraus <arturas@aleksandraus.se>, Nithesh Chandher Karthikeyan <nithesh.chandher.karthikeyan@liu.se>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

