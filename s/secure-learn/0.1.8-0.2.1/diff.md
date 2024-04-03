# Comparing `tmp/secure-learn-0.1.8.tar.gz` & `tmp/secure-learn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secure-learn-0.1.8.tar", last modified: Wed Apr  3 16:15:13 2024, max compression
+gzip compressed data, was "secure-learn-0.2.1.tar", last modified: Wed Apr  3 16:30:30 2024, max compression
```

## Comparing `secure-learn-0.1.8.tar` & `secure-learn-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:13.298158 secure-learn-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 16:14:53.000000 secure-learn-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-03 16:15:13.298158 secure-learn-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-03 16:14:53.000000 secure-learn-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 16:14:53.000000 secure-learn-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 16:15:13.298158 secure-learn-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-03 16:14:53.000000 secure-learn-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:13.294158 secure-learn-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:13.294158 secure-learn-0.1.8/src/SecuPy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/auditing.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/data_privacy_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 16:14:53.000000 secure-learn-0.1.8/src/SecuPy/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:15:13.294158 secure-learn-0.1.8/src/secure_learn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5701 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 16:15:13.000000 secure-learn-0.1.8/src/secure_learn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:30.140937 secure-learn-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 16:30:11.000000 secure-learn-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-03 16:30:30.140937 secure-learn-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-03 16:30:11.000000 secure-learn-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 16:30:11.000000 secure-learn-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 16:30:30.140937 secure-learn-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-04-03 16:30:11.000000 secure-learn-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:30.136937 secure-learn-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:30.140937 secure-learn-0.2.1/src/SecuPy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/auditing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/data_privacy_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 16:30:11.000000 secure-learn-0.2.1/src/SecuPy/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:30:30.140937 secure-learn-0.2.1/src/secure_learn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 16:30:30.000000 secure-learn-0.2.1/src/secure_learn.egg-info/top_level.txt
```

### Comparing `secure-learn-0.1.8/LICENSE` & `secure-learn-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secure-learn-0.1.8/PKG-INFO` & `secure-learn-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-learn
-Version: 0.1.8
+Version: 0.2.1
 Summary: Protect sensitive data with secure-learn, a Python package offering encryption, anonymization, and compliance tools for data scientists.
 Home-page: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
 Author: DeependraVerma
 Author-email: deependra.verma00@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/issues
 Classifier: Programming Language :: Python :: 3.7
@@ -115,9 +115,10 @@
 We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our [Contributing Guidelines](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki) to get started.
 
 ## License
 
 secure-learn is licensed under the [MIT License](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE). See the [LICENSE](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE) file for details.
 
 ## About the Author
-
+```
 [Email](mailto:deependra.verma00@gmail.com) | [LinkedIn](https://www.linkedin.com/in/deependra-verma-data-science/) | [GitHub](https://github.com/DeependraVerma) | [Portfolio](https://deependradatascience-productportfolio.netlify.app/)
+```
```

### Comparing `secure-learn-0.1.8/README.md` & `secure-learn-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,9 +91,10 @@
 We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our [Contributing Guidelines](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki) to get started.
 
 ## License
 
 secure-learn is licensed under the [MIT License](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE). See the [LICENSE](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE) file for details.
 
 ## About the Author
-
-[Email](mailto:deependra.verma00@gmail.com) | [LinkedIn](https://www.linkedin.com/in/deependra-verma-data-science/) | [GitHub](https://github.com/DeependraVerma) | [Portfolio](https://deependradatascience-productportfolio.netlify.app/)
+```
+[Email](mailto:deependra.verma00@gmail.com) | [LinkedIn](https://www.linkedin.com/in/deependra-verma-data-science/) | [GitHub](https://github.com/DeependraVerma) | [Portfolio](https://deependradatascience-productportfolio.netlify.app/)
+```
```

### Comparing `secure-learn-0.1.8/setup.cfg` & `secure-learn-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `secure-learn-0.1.8/setup.py` & `secure-learn-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         requirements = file_obj.readlines()
         requirements = [req.replace("\n","") for req in requirements]
 
         if HYPEN_E_DOT in requirements:
             requirements.remove(HYPEN_E_DOT)
     return requirements
 
-__version__ = "0.1.8"
+__version__ = "0.2.1"
 REPO_NAME = "SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists"
 PKG_NAME= "secure-learn"
 AUTHOR_USER_NAME = "DeependraVerma"
 AUTHOR_EMAIL = "deependra.verma00@gmail.com"
 
 setup(
     name=PKG_NAME,
```

### Comparing `secure-learn-0.1.8/src/SecuPy/data_privacy_framework.py` & `secure-learn-0.2.1/src/SecuPy/data_privacy_framework.py`

 * *Files identical despite different names*

### Comparing `secure-learn-0.1.8/src/secure_learn.egg-info/PKG-INFO` & `secure-learn-0.2.1/src/secure_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secure-learn
-Version: 0.1.8
+Version: 0.2.1
 Summary: Protect sensitive data with secure-learn, a Python package offering encryption, anonymization, and compliance tools for data scientists.
 Home-page: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
 Author: DeependraVerma
 Author-email: deependra.verma00@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/issues
 Classifier: Programming Language :: Python :: 3.7
@@ -115,9 +115,10 @@
 We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our [Contributing Guidelines](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki) to get started.
 
 ## License
 
 secure-learn is licensed under the [MIT License](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE). See the [LICENSE](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE) file for details.
 
 ## About the Author
-
+```
 [Email](mailto:deependra.verma00@gmail.com) | [LinkedIn](https://www.linkedin.com/in/deependra-verma-data-science/) | [GitHub](https://github.com/DeependraVerma) | [Portfolio](https://deependradatascience-productportfolio.netlify.app/)
+```
```

