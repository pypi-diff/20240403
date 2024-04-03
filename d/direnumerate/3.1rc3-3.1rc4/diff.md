# Comparing `tmp/direnumerate-3.1rc3.tar.gz` & `tmp/direnumerate-3.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-3.1rc3.tar", last modified: Wed Apr  3 12:49:51 2024, max compression
+gzip compressed data, was "direnumerate-3.1rc4.tar", last modified: Wed Apr  3 13:04:27 2024, max compression
```

## Comparing `direnumerate-3.1rc3.tar` & `direnumerate-3.1rc4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 12:49:51.912997 direnumerate-3.1rc3/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3858 2024-04-03 12:49:51.912997 direnumerate-3.1rc3/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2432 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 12:49:51.908997 direnumerate-3.1rc3/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16424 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3403 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-04-03 12:43:11.000000 direnumerate-3.1rc3/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/direnumerate/getinfo.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/direnumerate/ipcalculator.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-03 12:22:29.000000 direnumerate-3.1rc3/direnumerate/list_urls_accounts.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-03 12:48:05.000000 direnumerate-3.1rc3/direnumerate/version.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 12:49:51.912997 direnumerate-3.1rc3/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3858 2024-04-03 12:49:51.000000 direnumerate-3.1rc3/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-03 12:49:51.000000 direnumerate-3.1rc3/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-03 12:49:51.000000 direnumerate-3.1rc3/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-03 12:49:51.000000 direnumerate-3.1rc3/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-03 12:49:51.000000 direnumerate-3.1rc3/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-03 12:49:51.000000 direnumerate-3.1rc3/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-03 12:47:46.000000 direnumerate-3.1rc3/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-03 12:49:51.912997 direnumerate-3.1rc3/setup.cfg
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 13:04:27.615702 direnumerate-3.1rc4/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/LICENSE
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3858 2024-04-03 13:04:27.615702 direnumerate-3.1rc4/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2432 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/README.md
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 13:04:27.615702 direnumerate-3.1rc4/direnumerate/
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/direnumerate/__init__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    16424 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/direnumerate/__main__.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/direnumerate/banner.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     3403 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/direnumerate/cli.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/direnumerate/colors.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-04-03 12:43:11.000000 direnumerate-3.1rc4/direnumerate/createlist.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/direnumerate/getinfo.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/direnumerate/ipcalculator.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       47 2024-04-03 12:22:29.000000 direnumerate-3.1rc4/direnumerate/list_urls_accounts.py
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-04-03 13:01:43.000000 direnumerate-3.1rc4/direnumerate/version.py
+drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-04-03 13:04:27.615702 direnumerate-3.1rc4/direnumerate.egg-info/
+-rw-r--r--   0 estoque   (1000) estoque   (1000)     3858 2024-04-03 13:04:27.000000 direnumerate-3.1rc4/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)      505 2024-04-03 13:04:27.000000 direnumerate-3.1rc4/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-04-03 13:04:27.000000 direnumerate-3.1rc4/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-04-03 13:04:27.000000 direnumerate-3.1rc4/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-04-03 13:04:27.000000 direnumerate-3.1rc4/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-04-03 13:04:27.000000 direnumerate-3.1rc4/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-04-03 13:01:06.000000 direnumerate-3.1rc4/pyproject.toml
+-rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-04-03 13:04:27.615702 direnumerate-3.1rc4/setup.cfg
```

### Comparing `direnumerate-3.1rc3/LICENSE` & `direnumerate-3.1rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-3.1rc3/PKG-INFO` & `direnumerate-3.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.1rc3
+Version: 3.1rc4
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.1rc3 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.1rc4 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.1rc3/README.md` & `direnumerate-3.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `direnumerate-3.1rc3/direnumerate/__init__.py` & `direnumerate-3.1rc4/direnumerate/__init__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.1rc3/direnumerate/__main__.py` & `direnumerate-3.1rc4/direnumerate/__main__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.1rc3/direnumerate/cli.py` & `direnumerate-3.1rc4/direnumerate/cli.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.1rc3/direnumerate/createlist.py` & `direnumerate-3.1rc4/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.1rc3/direnumerate/ipcalculator.py` & `direnumerate-3.1rc4/direnumerate/ipcalculator.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.1rc3/direnumerate.egg-info/PKG-INFO` & `direnumerate-3.1rc4/direnumerate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.1rc3
+Version: 3.1rc4
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.1rc3 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 3.1rc4 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.1rc3/pyproject.toml` & `direnumerate-3.1rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "3.1-rc3"
+version = "3.1-rc4"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

