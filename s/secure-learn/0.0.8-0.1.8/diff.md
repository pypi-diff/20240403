# Comparing `tmp/secure-learn-0.0.8.tar.gz` & `tmp/secure-learn-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure-learn-0.0.8.tar", last modified: Wed Apr  3 16:03:09 2024, max compression
+gzip compressed data, was "secure-learn-0.1.8.tar", last modified: Wed Apr  3 16:15:13 2024, max compression
```

## Comparing `secure-learn-0.0.8.tar` & `secure-learn-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:03:09.787295 secure-learn-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 16:02:50.000000 secure-learn-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-03 16:03:09.787295 secure-learn-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-03 16:02:50.000000 secure-learn-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 16:02:50.000000 secure-learn-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 16:03:09.787295 secure-learn-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-03 16:02:50.000000 secure-learn-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:03:09.783295 secure-learn-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:03:09.783295 secure-learn-0.0.8/src/SecuPy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:02:50.000000 secure-learn-0.0.8/src/SecuPy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 16:02:50.000000 secure-learn-0.0.8/src/SecuPy/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-03 16:02:50.000000 secure-learn-0.0.8/src/SecuPy/auditing.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 16:02:50.000000 secure-learn-0.0.8/src/SecuPy/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 16:02:50.000000 secure-learn-0.0.8/src/SecuPy/data_privacy_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 16:02:50.000000 secure-learn-0.0.8/src/SecuPy/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:03:09.787295 secure-learn-0.0.8/src/secure_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-03 16:03:09.000000 secure-learn-0.0.8/src/secure_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 16:03:09.000000 secure-learn-0.0.8/src/secure_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:03:09.000000 secure-learn-0.0.8/src/secure_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 16:03:09.000000 secure-learn-0.0.8/src/secure_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 16:03:09.000000 secure-learn-0.0.8/src/secure_learn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:13.298158 secure-learn-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 16:14:53.000000 secure-learn-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-03 16:15:13.298158 secure-learn-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-03 16:14:53.000000 secure-learn-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 16:14:53.000000 secure-learn-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 16:15:13.298158 secure-learn-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-03 16:14:53.000000 secure-learn-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:13.294158 secure-learn-0.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:13.294158 secure-learn-0.1.8/src/SecuPy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/auditing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/data_privacy_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:13.294158 secure-learn-0.1.8/src/secure_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/top_level.txt
```

### Comparing `secure-learn-0.0.8/LICENSE` & `secure-learn-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `secure-learn-0.0.8/PKG-INFO` & `secure-learn-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: secure-learn
-Version: 0.0.8
-Summary: Protect sensitive data with SheildPy, a Python package offering encryption, anonymization, and compliance tools for data scientists.
+Version: 0.1.8
+Summary: Protect sensitive data with secure-learn, a Python package offering encryption, anonymization, and compliance tools for data scientists.
 Home-page: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
 Author: DeependraVerma
 Author-email: deependra.verma00@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `secure-learn-0.0.8/README.md` & `secure-learn-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `secure-learn-0.0.8/setup.cfg` & `secure-learn-0.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `secure-learn-0.0.8/setup.py` & `secure-learn-0.1.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,26 @@
         requirements = file_obj.readlines()
         requirements = [req.replace("\n","") for req in requirements]
 
         if HYPEN_E_DOT in requirements:
             requirements.remove(HYPEN_E_DOT)
     return requirements
 
-__version__ = "0.0.8"
+__version__ = "0.1.8"
 REPO_NAME = "SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists"
 PKG_NAME= "secure-learn"
 AUTHOR_USER_NAME = "DeependraVerma"
 AUTHOR_EMAIL = "deependra.verma00@gmail.com"
 
 setup(
     name=PKG_NAME,
     version=__version__,
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
-    description="Protect sensitive data with SheildPy, a Python package offering encryption, anonymization, and compliance tools for data scientists.",
+    description="Protect sensitive data with secure-learn, a Python package offering encryption, anonymization, and compliance tools for data scientists.",
     long_description=long_description,
     long_description_content="text/x-rst",
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     package_dir={"": "src"},
```

### Comparing `secure-learn-0.0.8/src/SecuPy/data_privacy_framework.py` & `secure-learn-0.1.8/src/SecuPy/data_privacy_framework.py`

 * *Files identical despite different names*

### Comparing `secure-learn-0.0.8/src/secure_learn.egg-info/PKG-INFO` & `secure-learn-0.1.8/src/secure_learn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: secure-learn
-Version: 0.0.8
-Summary: Protect sensitive data with SheildPy, a Python package offering encryption, anonymization, and compliance tools for data scientists.
+Version: 0.1.8
+Summary: Protect sensitive data with secure-learn, a Python package offering encryption, anonymization, and compliance tools for data scientists.
 Home-page: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
 Author: DeependraVerma
 Author-email: deependra.verma00@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

