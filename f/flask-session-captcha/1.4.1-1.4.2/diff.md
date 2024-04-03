# Comparing `tmp/flask_session_captcha-1.4.1.tar.gz` & `tmp/flask_session_captcha-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_session_captcha-1.4.1.tar", last modified: Mon Mar 18 20:26:46 2024, max compression
+gzip compressed data, was "flask_session_captcha-1.4.2.tar", last modified: Wed Apr  3 17:30:41 2024, max compression
```

## Comparing `flask_session_captcha-1.4.1.tar` & `flask_session_captcha-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:26:46.725859 flask_session_captcha-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-18 20:26:42.000000 flask_session_captcha-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-03-18 20:26:46.725859 flask_session_captcha-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-03-18 20:26:42.000000 flask_session_captcha-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:26:46.721859 flask_session_captcha-1.4.1/flask_session_captcha/
--rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-03-18 20:26:42.000000 flask_session_captcha-1.4.1/flask_session_captcha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:26:46.725859 flask_session_captcha-1.4.1/flask_session_captcha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-03-18 20:26:46.000000 flask_session_captcha-1.4.1/flask_session_captcha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-18 20:26:46.000000 flask_session_captcha-1.4.1/flask_session_captcha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 20:26:46.000000 flask_session_captcha-1.4.1/flask_session_captcha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-18 20:26:46.000000 flask_session_captcha-1.4.1/flask_session_captcha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-18 20:26:46.000000 flask_session_captcha-1.4.1/flask_session_captcha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-18 20:26:46.725859 flask_session_captcha-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-18 20:26:42.000000 flask_session_captcha-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 20:26:46.721859 flask_session_captcha-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-03-18 20:26:42.000000 flask_session_captcha-1.4.1/tests/test_charsets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-03-18 20:26:42.000000 flask_session_captcha-1.4.1/tests/test_flask_session_captcha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:41.849575 flask_session_captcha-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-03 17:30:37.000000 flask_session_captcha-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-03 17:30:41.849575 flask_session_captcha-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-04-03 17:30:37.000000 flask_session_captcha-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:41.845575 flask_session_captcha-1.4.2/flask_session_captcha/
+-rw-r--r--   0 runner    (1001) docker     (127)     7298 2024-04-03 17:30:37.000000 flask_session_captcha-1.4.2/flask_session_captcha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:41.849575 flask_session_captcha-1.4.2/flask_session_captcha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4602 2024-04-03 17:30:41.000000 flask_session_captcha-1.4.2/flask_session_captcha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-03 17:30:41.000000 flask_session_captcha-1.4.2/flask_session_captcha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:30:41.000000 flask_session_captcha-1.4.2/flask_session_captcha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 17:30:41.000000 flask_session_captcha-1.4.2/flask_session_captcha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:30:41.000000 flask_session_captcha-1.4.2/flask_session_captcha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 17:30:41.849575 flask_session_captcha-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-04-03 17:30:37.000000 flask_session_captcha-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:30:41.849575 flask_session_captcha-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-03 17:30:37.000000 flask_session_captcha-1.4.2/tests/test_charsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-03 17:30:37.000000 flask_session_captcha-1.4.2/tests/test_flask_session_captcha.py
```

### Comparing `flask_session_captcha-1.4.1/LICENSE` & `flask_session_captcha-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_session_captcha-1.4.1/PKG-INFO` & `flask_session_captcha-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_session_captcha
-Version: 1.4.1
+Version: 1.4.2
 Summary: Captcha implementation for flask and flask-session.
 Home-page: https://github.com/Tethik/flask-session-captcha
 Author: Joakim Uddholm
 Author-email: tethik@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `flask_session_captcha-1.4.1/README.md` & `flask_session_captcha-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `flask_session_captcha-1.4.1/flask_session_captcha/__init__.py` & `flask_session_captcha-1.4.2/flask_session_captcha/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_session_captcha-1.4.1/flask_session_captcha.egg-info/PKG-INFO` & `flask_session_captcha-1.4.2/flask_session_captcha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_session_captcha
-Version: 1.4.1
+Version: 1.4.2
 Summary: Captcha implementation for flask and flask-session.
 Home-page: https://github.com/Tethik/flask-session-captcha
 Author: Joakim Uddholm
 Author-email: tethik@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `flask_session_captcha-1.4.1/setup.py` & `flask_session_captcha-1.4.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "1.4.1"
+VERSION = "1.4.2"
 with open("README.md") as f:
     README = f.read()
 
 setup(
     name='flask_session_captcha',
     version=VERSION,
     author='Joakim Uddholm',
```

### Comparing `flask_session_captcha-1.4.1/tests/test_charsets.py` & `flask_session_captcha-1.4.2/tests/test_charsets.py`

 * *Files identical despite different names*

### Comparing `flask_session_captcha-1.4.1/tests/test_flask_session_captcha.py` & `flask_session_captcha-1.4.2/tests/test_flask_session_captcha.py`

 * *Files identical despite different names*

