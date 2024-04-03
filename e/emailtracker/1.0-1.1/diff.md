# Comparing `tmp/emailtracker-1.0.tar.gz` & `tmp/emailtracker-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailtracker-1.0.tar", last modified: Sun Mar 17 08:04:56 2024, max compression
+gzip compressed data, was "emailtracker-1.1.tar", last modified: Wed Apr  3 08:32:40 2024, max compression
```

## Comparing `emailtracker-1.0.tar` & `emailtracker-1.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-03-17 08:04:56.721723 emailtracker-1.0/
--rw-r--r--   0 kali      (1000) kali      (1000)     1076 2024-03-17 08:01:40.000000 emailtracker-1.0/LICENSE
--rw-r--r--   0 kali      (1000) kali      (1000)      604 2024-03-17 08:04:56.721723 emailtracker-1.0/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)       14 2024-03-17 08:01:40.000000 emailtracker-1.0/README.md
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-03-17 08:04:56.721723 emailtracker-1.0/emailtracker/
--rw-r--r--   0 kali      (1000) kali      (1000)      106 2024-03-17 08:01:40.000000 emailtracker-1.0/emailtracker/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3521 2024-03-17 08:01:40.000000 emailtracker-1.0/emailtracker/emailtracker.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-03-17 08:04:56.721723 emailtracker-1.0/emailtracker.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)      604 2024-03-17 08:04:56.000000 emailtracker-1.0/emailtracker.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)      263 2024-03-17 08:04:56.000000 emailtracker-1.0/emailtracker.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-03-17 08:04:56.000000 emailtracker-1.0/emailtracker.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       67 2024-03-17 08:04:56.000000 emailtracker-1.0/emailtracker.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-03-17 08:04:56.000000 emailtracker-1.0/emailtracker.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-03-17 08:04:56.721723 emailtracker-1.0/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)      943 2024-03-17 08:01:40.000000 emailtracker-1.0/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:32:40.705212 emailtracker-1.1/
+-rw-r--r--   0 kali      (1000) kali      (1000)     1076 2024-04-03 08:32:27.000000 emailtracker-1.1/LICENSE
+-rw-r--r--   0 kali      (1000) kali      (1000)      604 2024-04-03 08:32:40.705212 emailtracker-1.1/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)       14 2024-04-03 08:32:27.000000 emailtracker-1.1/README.md
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:32:40.701212 emailtracker-1.1/emailtracker/
+-rw-r--r--   0 kali      (1000) kali      (1000)      106 2024-04-03 08:32:27.000000 emailtracker-1.1/emailtracker/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3521 2024-04-03 08:32:27.000000 emailtracker-1.1/emailtracker/emailtracker.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2024-04-03 08:32:40.705212 emailtracker-1.1/emailtracker.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)      604 2024-04-03 08:32:40.000000 emailtracker-1.1/emailtracker.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)      298 2024-04-03 08:32:40.000000 emailtracker-1.1/emailtracker.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2024-04-03 08:32:40.000000 emailtracker-1.1/emailtracker.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       67 2024-04-03 08:32:40.000000 emailtracker-1.1/emailtracker.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       37 2024-04-03 08:32:40.000000 emailtracker-1.1/emailtracker.egg-info/requires.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       13 2024-04-03 08:32:40.000000 emailtracker-1.1/emailtracker.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2024-04-03 08:32:40.705212 emailtracker-1.1/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     1091 2024-04-03 08:32:27.000000 emailtracker-1.1/setup.py
```

### Comparing `emailtracker-1.0/LICENSE` & `emailtracker-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `emailtracker-1.0/PKG-INFO` & `emailtracker-1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailtracker
-Version: 1.0
+Version: 1.1
 Summary: A graphical email tracking tool
 Home-page: https://github.com/IMApurbo/emailtracker
 Author: AKM Korishee Apurbo
 Author-email: bandinvisible8@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `emailtracker-1.0/emailtracker/emailtracker.py` & `emailtracker-1.1/emailtracker/emailtracker.py`

 * *Files identical despite different names*

### Comparing `emailtracker-1.0/emailtracker.egg-info/PKG-INFO` & `emailtracker-1.1/emailtracker.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailtracker
-Version: 1.0
+Version: 1.1
 Summary: A graphical email tracking tool
 Home-page: https://github.com/IMApurbo/emailtracker
 Author: AKM Korishee Apurbo
 Author-email: bandinvisible8@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

