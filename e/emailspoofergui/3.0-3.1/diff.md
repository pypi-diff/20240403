# Comparing `tmp/emailspoofergui-3.0.tar.gz` & `tmp/emailspoofergui-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailspoofergui-3.0.tar", last modified: Sun Mar 17 10:08:49 2024, max compression
+gzip compressed data, was "emailspoofergui-3.1.tar", last modified: Wed Apr  3 08:34:51 2024, max compression
```

## Comparing `emailspoofergui-3.0.tar` & `emailspoofergui-3.1.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-03-17 10:08:49.597643 emailspoofergui-3.0/
--rw-r--r--   0 kali      (1000) kali      (1000)     1076 2024-03-17 10:08:36.000000 emailspoofergui-3.0/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)     1755 2024-03-17 10:08:49.597643 emailspoofergui-3.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1160 2024-03-17 10:08:36.000000 emailspoofergui-3.0/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-03-17 10:08:49.597643 emailspoofergui-3.0/emailspoofergui/
--rw-r--r--   0 kali      (1000) kali      (1000)      143 2024-03-17 10:08:36.000000 emailspoofergui-3.0/emailspoofergui/__init__.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-03-17 10:08:49.597643 emailspoofergui-3.0/emailspoofergui/data/
--rw-r--r--   0 kali      (1000) kali      (1000)      112 2024-03-17 10:08:36.000000 emailspoofergui-3.0/emailspoofergui/data/config.json
--rw-r--r--   0 kali      (1000) kali      (1000)     5428 2024-03-17 10:08:36.000000 emailspoofergui-3.0/emailspoofergui/emailspoofergui.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-03-17 10:08:49.597643 emailspoofergui-3.0/emailspoofergui.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)     1755 2024-03-17 10:08:49.000000 emailspoofergui-3.0/emailspoofergui.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      320 2024-03-17 10:08:49.000000 emailspoofergui-3.0/emailspoofergui.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-03-17 10:08:49.000000 emailspoofergui-3.0/emailspoofergui.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       79 2024-03-17 10:08:49.000000 emailspoofergui-3.0/emailspoofergui.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       16 2024-03-17 10:08:49.000000 emailspoofergui-3.0/emailspoofergui.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-03-17 10:08:49.597643 emailspoofergui-3.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     1021 2024-03-17 10:08:36.000000 emailspoofergui-3.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:34:51.661453 emailspoofergui-3.1/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1076 2024-04-03 08:34:32.000000 emailspoofergui-3.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)     1755 2024-04-03 08:34:51.661453 emailspoofergui-3.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1160 2024-04-03 08:34:32.000000 emailspoofergui-3.1/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:34:51.657453 emailspoofergui-3.1/emailspoofergui/
+-rw-r--r--   0 kali      (1000) kali      (1000)      143 2024-04-03 08:34:32.000000 emailspoofergui-3.1/emailspoofergui/__init__.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:34:51.661453 emailspoofergui-3.1/emailspoofergui/data/
+-rw-r--r--   0 kali      (1000) kali      (1000)      112 2024-04-03 08:34:32.000000 emailspoofergui-3.1/emailspoofergui/data/config.json
+-rw-r--r--   0 kali      (1000) kali      (1000)     5428 2024-04-03 08:34:32.000000 emailspoofergui-3.1/emailspoofergui/emailspoofergui.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:34:51.661453 emailspoofergui-3.1/emailspoofergui.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1755 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      358 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       79 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       28 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       16 2024-04-03 08:34:51.000000 emailspoofergui-3.1/emailspoofergui.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-04-03 08:34:51.661453 emailspoofergui-3.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1145 2024-04-03 08:34:32.000000 emailspoofergui-3.1/setup.py
```

### Comparing `emailspoofergui-3.0/LICENSE` & `emailspoofergui-3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emailspoofergui-3.0/PKG-INFO` & `emailspoofergui-3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailspoofergui
-Version: 3.0
+Version: 3.1
 Summary: A graphical email spoofing tool
 Home-page: https://github.com/IMApurbo/emailspoofergui
 Author: AKM Korishee Apurbo
 Author-email: bandinvisible8@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emailspoofergui-3.0/README.md` & `emailspoofergui-3.1/README.md`

 * *Files identical despite different names*

### Comparing `emailspoofergui-3.0/emailspoofergui/emailspoofergui.py` & `emailspoofergui-3.1/emailspoofergui/emailspoofergui.py`

 * *Files identical despite different names*

### Comparing `emailspoofergui-3.0/emailspoofergui.egg-info/PKG-INFO` & `emailspoofergui-3.1/emailspoofergui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailspoofergui
-Version: 3.0
+Version: 3.1
 Summary: A graphical email spoofing tool
 Home-page: https://github.com/IMApurbo/emailspoofergui
 Author: AKM Korishee Apurbo
 Author-email: bandinvisible8@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emailspoofergui-3.0/setup.py` & `emailspoofergui-3.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='emailspoofergui',
-    version='3.0',
+    version='3.1',
     packages=find_packages(),
     package_data={'emailspoofergui': ['data/config.json']},
     install_requires=[
-        # List your dependencies here
+        'customtkinter',  # Example of a required package with a minimum version
+        'CTkMessagebox',  # Example of a required package with an exact version 
     ],
     entry_points={
         'console_scripts': [
             'emailspoofergui = emailspoofergui.emailspoofergui:send_email',
         ],
     },
     author='AKM Korishee Apurbo',
```

