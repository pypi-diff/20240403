# Comparing `tmp/segy-0.0.8.tar.gz` & `tmp/segy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segy-0.0.8.tar", max compression
+gzip compressed data, was "segy-0.0.9.tar", max compression
```

## Comparing `segy-0.0.8.tar` & `segy-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    11357 2024-03-05 23:32:25.031489 segy-0.0.8/LICENSE
--rw-r--r--   0        0        0     4826 2024-03-05 23:32:25.031489 segy-0.0.8/README.md
--rw-r--r--   0        0        0     3855 2024-03-05 23:32:37.635642 segy-0.0.8/pyproject.toml
--rw-r--r--   0        0        0       91 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/__init__.py
--rw-r--r--   0        0        0       41 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/cli/__init__.py
--rw-r--r--   0        0        0     1253 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/cli/common.py
--rw-r--r--   0        0        0     4092 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/cli/dump.py
--rw-r--r--   0        0        0      183 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/cli/segy.py
--rw-r--r--   0        0        0      559 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/compat.py
--rw-r--r--   0        0        0     1923 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/config.py
--rw-r--r--   0        0        0     4874 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/ebcdic.py
--rw-r--r--   0        0        0     7961 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/file.py
--rw-r--r--   0        0        0     4572 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/ibm.py
--rw-r--r--   0        0        0    11393 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/indexing.py
--rw-r--r--   0        0        0        0 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/py.typed
--rw-r--r--   0        0        0      826 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/schema/__init__.py
--rw-r--r--   0        0        0     1674 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/schema/base.py
--rw-r--r--   0        0        0     6431 2024-03-05 23:32:25.039489 segy-0.0.8/src/segy/schema/data_type.py
--rw-r--r--   0        0        0     2776 2024-03-05 23:32:25.043490 segy-0.0.8/src/segy/schema/header.py
--rw-r--r--   0        0        0     3871 2024-03-05 23:32:25.043490 segy-0.0.8/src/segy/schema/segy.py
--rw-r--r--   0        0        0     2039 2024-03-05 23:32:25.043490 segy-0.0.8/src/segy/schema/trace.py
--rw-r--r--   0        0        0      358 2024-03-05 23:32:25.043490 segy-0.0.8/src/segy/standards/__init__.py
--rw-r--r--   0        0        0     1088 2024-03-05 23:32:25.043490 segy-0.0.8/src/segy/standards/registry.py
--rw-r--r--   0        0        0    21423 2024-03-05 23:32:25.043490 segy-0.0.8/src/segy/standards/rev0.py
--rw-r--r--   0        0        0     6673 2024-03-05 23:32:25.043490 segy-0.0.8/src/segy/standards/rev1.py
--rw-r--r--   0        0        0      186 2024-03-05 23:32:25.043490 segy-0.0.8/src/segy/typing.py
--rw-r--r--   0        0        0     6286 1970-01-01 00:00:00.000000 segy-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-05 23:41:21.290005 segy-0.0.9/LICENSE
+-rw-r--r--   0        0        0     4833 2024-03-05 23:41:32.993965 segy-0.0.9/README.md
+-rw-r--r--   0        0        0     3855 2024-03-05 23:41:32.993965 segy-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0       91 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/__init__.py
+-rw-r--r--   0        0        0       41 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/cli/__init__.py
+-rw-r--r--   0        0        0     1253 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/cli/common.py
+-rw-r--r--   0        0        0     4092 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/cli/dump.py
+-rw-r--r--   0        0        0      183 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/cli/segy.py
+-rw-r--r--   0        0        0      559 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/compat.py
+-rw-r--r--   0        0        0     1923 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/config.py
+-rw-r--r--   0        0        0     4874 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/ebcdic.py
+-rw-r--r--   0        0        0     7961 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/file.py
+-rw-r--r--   0        0        0     4572 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/ibm.py
+-rw-r--r--   0        0        0    11393 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/indexing.py
+-rw-r--r--   0        0        0        0 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/py.typed
+-rw-r--r--   0        0        0      826 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/schema/__init__.py
+-rw-r--r--   0        0        0     1674 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/schema/base.py
+-rw-r--r--   0        0        0     6431 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/schema/data_type.py
+-rw-r--r--   0        0        0     2776 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/schema/header.py
+-rw-r--r--   0        0        0     3871 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/schema/segy.py
+-rw-r--r--   0        0        0     2039 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/schema/trace.py
+-rw-r--r--   0        0        0      358 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/standards/__init__.py
+-rw-r--r--   0        0        0     1088 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/standards/registry.py
+-rw-r--r--   0        0        0    21423 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/standards/rev0.py
+-rw-r--r--   0        0        0     6673 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/standards/rev1.py
+-rw-r--r--   0        0        0      186 2024-03-05 23:41:21.302004 segy-0.0.9/src/segy/typing.py
+-rw-r--r--   0        0        0     6293 1970-01-01 00:00:00.000000 segy-0.0.9/PKG-INFO
```

### Comparing `segy-0.0.8/LICENSE` & `segy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/README.md` & `segy-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -117,21 +117,21 @@
 ## Credits
 
 This project was established at [TGS](https://www.tgs.com/). Current
 maintainer is [Altay Sansal](https://github.com/tasansal) with the support
 of many more great colleagues.
 
 The CI/CD tooling is loosely based on [Hypermodern Python Cookiecutter]
-with more modern tooling applied elsewhere!.
+with more modern tooling applied elsewhere.
 
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [pypi]: https://pypi.org/
 [file an issue]: https://github.com/TGSAI/segy/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
 [apache 2.0 license]: https://github.com/TGSAI/segy/blob/main/LICENSE
 [contributor guide]: https://github.com/TGSAI/segy/blob/main/CONTRIBUTING.md
-[command-line usage]: https://segy.readthedocs.io/en/stable/usage.html
-[api reference]: https://segy.readthedocs.io/en/stable/reference.html
+[command-line usage]: https://segy.readthedocs.io/en/stable/cli_usage.html
+[api reference]: https://segy.readthedocs.io/en/stable/api_reference.html
 [installation instructions]: https://segy.readthedocs.io/en/stable/installation.html
```

### Comparing `segy-0.0.8/pyproject.toml` & `segy-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "segy"
-version = "0.0.8"
+version = "0.0.9"
 description = "The Ultimate Python SEG-Y I/O with Cloud Support and Schemas"
 authors = ["TGS <sys-opensource@tgs.com>"]
 maintainers = [
     "Altay Sansal <altay.sansal@tgs.com>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
```

### Comparing `segy-0.0.8/src/segy/cli/common.py` & `segy-0.0.9/src/segy/cli/common.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/cli/dump.py` & `segy-0.0.9/src/segy/cli/dump.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/compat.py` & `segy-0.0.9/src/segy/compat.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/config.py` & `segy-0.0.9/src/segy/config.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/ebcdic.py` & `segy-0.0.9/src/segy/ebcdic.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/file.py` & `segy-0.0.9/src/segy/file.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/ibm.py` & `segy-0.0.9/src/segy/ibm.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/indexing.py` & `segy-0.0.9/src/segy/indexing.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/schema/__init__.py` & `segy-0.0.9/src/segy/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/schema/base.py` & `segy-0.0.9/src/segy/schema/base.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/schema/data_type.py` & `segy-0.0.9/src/segy/schema/data_type.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/schema/header.py` & `segy-0.0.9/src/segy/schema/header.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/schema/segy.py` & `segy-0.0.9/src/segy/schema/segy.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/schema/trace.py` & `segy-0.0.9/src/segy/schema/trace.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/standards/registry.py` & `segy-0.0.9/src/segy/standards/registry.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/standards/rev0.py` & `segy-0.0.9/src/segy/standards/rev0.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/src/segy/standards/rev1.py` & `segy-0.0.9/src/segy/standards/rev1.py`

 * *Files identical despite different names*

### Comparing `segy-0.0.8/PKG-INFO` & `segy-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segy
-Version: 0.0.8
+Version: 0.0.9
 Summary: The Ultimate Python SEG-Y I/O with Cloud Support and Schemas
 Home-page: https://github.com/TGSAI/segy
 License: Apache-2.0
 Keywords: segy,seismic,data,geophysics
 Author: TGS
 Author-email: sys-opensource@tgs.com
 Maintainer: Altay Sansal
@@ -153,22 +153,22 @@
 ## Credits
 
 This project was established at [TGS](https://www.tgs.com/). Current
 maintainer is [Altay Sansal](https://github.com/tasansal) with the support
 of many more great colleagues.
 
 The CI/CD tooling is loosely based on [Hypermodern Python Cookiecutter]
-with more modern tooling applied elsewhere!.
+with more modern tooling applied elsewhere.
 
 [hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
 [pypi]: https://pypi.org/
 [file an issue]: https://github.com/TGSAI/segy/issues
 [pip]: https://pip.pypa.io/
 
 <!-- github-only -->
 
 [apache 2.0 license]: https://github.com/TGSAI/segy/blob/main/LICENSE
 [contributor guide]: https://github.com/TGSAI/segy/blob/main/CONTRIBUTING.md
-[command-line usage]: https://segy.readthedocs.io/en/stable/usage.html
-[api reference]: https://segy.readthedocs.io/en/stable/reference.html
+[command-line usage]: https://segy.readthedocs.io/en/stable/cli_usage.html
+[api reference]: https://segy.readthedocs.io/en/stable/api_reference.html
 [installation instructions]: https://segy.readthedocs.io/en/stable/installation.html
```

