# Comparing `tmp/cbrkit-0.9.0.tar.gz` & `tmp/cbrkit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbrkit-0.9.0.tar", max compression
+gzip compressed data, was "cbrkit-0.9.1.tar", max compression
```

## Comparing `cbrkit-0.9.0.tar` & `cbrkit-0.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1067 2024-04-02 07:43:48.623737 cbrkit-0.9.0/LICENSE
--rw-r--r--   0        0        0    10939 2024-04-02 07:43:48.623737 cbrkit-0.9.0/README.md
--rw-r--r--   0        0        0      246 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/__init__.py
--rw-r--r--   0        0        0       34 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/__main__.py
--rw-r--r--   0        0        0     1680 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/api.py
--rw-r--r--   0        0        0      813 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/cli.py
--rw-r--r--   0        0        0     4383 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/helpers.py
--rw-r--r--   0        0        0    10126 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/loaders.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/py.typed
--rw-r--r--   0        0        0     7551 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/retrieval.py
--rw-r--r--   0        0        0      814 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/__init__.py
--rw-r--r--   0        0        0     2997 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/_aggregator.py
--rw-r--r--   0        0        0     4805 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/_attribute_value.py
--rw-r--r--   0        0        0     2434 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/collections.py
--rw-r--r--   0        0        0     1559 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/generic.py
--rw-r--r--   0        0        0      386 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/graph/__init__.py
--rw-r--r--   0        0        0     9987 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/graph/_astar.py
--rw-r--r--   0        0        0      685 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/graph/_model.py
--rw-r--r--   0        0        0     2511 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/numbers.py
--rw-r--r--   0        0        0     9225 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/strings/__init__.py
--rw-r--r--   0        0        0    10258 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/sim/strings/taxonomy.py
--rw-r--r--   0        0        0     1856 2024-04-02 07:43:48.627737 cbrkit-0.9.0/cbrkit/typing.py
--rw-r--r--   0        0        0     2998 2024-04-02 07:44:58.315766 cbrkit-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    13503 1970-01-01 00:00:00.000000 cbrkit-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-03 07:53:46.919378 cbrkit-0.9.1/LICENSE
+-rw-r--r--   0        0        0    10939 2024-04-03 07:53:46.919378 cbrkit-0.9.1/README.md
+-rw-r--r--   0        0        0      246 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/__init__.py
+-rw-r--r--   0        0        0       34 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/__main__.py
+-rw-r--r--   0        0        0     1680 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/api.py
+-rw-r--r--   0        0        0      813 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/cli.py
+-rw-r--r--   0        0        0     4383 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/helpers.py
+-rw-r--r--   0        0        0    10126 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/loaders.py
+-rw-r--r--   0        0        0        0 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/py.typed
+-rw-r--r--   0        0        0     7551 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/retrieval.py
+-rw-r--r--   0        0        0      814 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/__init__.py
+-rw-r--r--   0        0        0     2997 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/_aggregator.py
+-rw-r--r--   0        0        0     4805 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/_attribute_value.py
+-rw-r--r--   0        0        0     2434 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/collections.py
+-rw-r--r--   0        0        0     1559 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/generic.py
+-rw-r--r--   0        0        0      386 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/graph/__init__.py
+-rw-r--r--   0        0        0     9987 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/graph/_astar.py
+-rw-r--r--   0        0        0      685 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/graph/_model.py
+-rw-r--r--   0        0        0     2511 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/numbers.py
+-rw-r--r--   0        0        0     9225 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/strings/__init__.py
+-rw-r--r--   0        0        0    10258 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/sim/strings/taxonomy.py
+-rw-r--r--   0        0        0     1856 2024-04-03 07:53:46.923378 cbrkit-0.9.1/cbrkit/typing.py
+-rw-r--r--   0        0        0     2998 2024-04-03 07:54:51.275618 cbrkit-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    13503 1970-01-01 00:00:00.000000 cbrkit-0.9.1/PKG-INFO
```

### Comparing `cbrkit-0.9.0/LICENSE` & `cbrkit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/README.md` & `cbrkit-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/api.py` & `cbrkit-0.9.1/cbrkit/api.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/cli.py` & `cbrkit-0.9.1/cbrkit/cli.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/helpers.py` & `cbrkit-0.9.1/cbrkit/helpers.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/loaders.py` & `cbrkit-0.9.1/cbrkit/loaders.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/retrieval.py` & `cbrkit-0.9.1/cbrkit/retrieval.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/__init__.py` & `cbrkit-0.9.1/cbrkit/sim/__init__.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/_aggregator.py` & `cbrkit-0.9.1/cbrkit/sim/_aggregator.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/_attribute_value.py` & `cbrkit-0.9.1/cbrkit/sim/_attribute_value.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/collections.py` & `cbrkit-0.9.1/cbrkit/sim/collections.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/generic.py` & `cbrkit-0.9.1/cbrkit/sim/generic.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/graph/_astar.py` & `cbrkit-0.9.1/cbrkit/sim/graph/_astar.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/graph/_model.py` & `cbrkit-0.9.1/cbrkit/sim/graph/_model.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/numbers.py` & `cbrkit-0.9.1/cbrkit/sim/numbers.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/strings/__init__.py` & `cbrkit-0.9.1/cbrkit/sim/strings/__init__.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/sim/strings/taxonomy.py` & `cbrkit-0.9.1/cbrkit/sim/strings/taxonomy.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/cbrkit/typing.py` & `cbrkit-0.9.1/cbrkit/typing.py`

 * *Files identical despite different names*

### Comparing `cbrkit-0.9.0/pyproject.toml` & `cbrkit-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cbrkit"
-version = "0.9.0"
+version = "0.9.1"
 description = "Customizable Case-Based Reasoning (CBR) toolkit for Python with a built-in API and CLI."
 authors = ["Mirko Lenz <mirko@mirkolenz.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "cbrkit" }]
 repository = "https://github.com/wi2trier/cbrkit"
 homepage = "https://wi2trier.github.io/cbrkit/"
```

### Comparing `cbrkit-0.9.0/PKG-INFO` & `cbrkit-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbrkit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Customizable Case-Based Reasoning (CBR) toolkit for Python with a built-in API and CLI.
 Home-page: https://wi2trier.github.io/cbrkit/
 License: MIT
 Keywords: cbr,case-based reasoning,api,similarity,nlp,retrieval,cli,tool,library
 Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com
 Requires-Python: >=3.11,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cbrkit Version: 0.9.0 Summary: Customizable Case-
+Metadata-Version: 2.1 Name: cbrkit Version: 0.9.1 Summary: Customizable Case-
 Based Reasoning (CBR) toolkit for Python with a built-in API and CLI. Home-
 page: https://wi2trier.github.io/cbrkit/ License: MIT Keywords: cbr,case-based
 reasoning,api,similarity,nlp,retrieval,cli,tool,library Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com Requires-Python: >=3.11,<3.13 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
 Framework :: Pytest Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
```

