# Comparing `tmp/Andreani_QA_Scanner-0.0.8.tar.gz` & `tmp/Andreani_QA_Scanner-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Andreani_QA_Scanner-0.0.8.tar", last modified: Mon Mar 18 17:26:26 2024, max compression
+gzip compressed data, was "Andreani_QA_Scanner-0.0.9.tar", last modified: Mon Mar 18 17:40:48 2024, max compression
```

## Comparing `Andreani_QA_Scanner-0.0.8.tar` & `Andreani_QA_Scanner-0.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.492698 Andreani_QA_Scanner-0.0.8/
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.467764 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/
--rw-rw-rw-   0        0        0       30 2024-03-18 13:04:01.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.483722 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/
--rw-rw-rw-   0        0        0    20444 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/Scanner.py
--rw-rw-rw-   0        0        0     2414 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/ScreenManagement.py
--rw-rw-rw-   0        0        0    10724 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/ScriptToFile.py
--rw-rw-rw-   0        0        0     6627 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/UserManagement.py
--rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/__init__.py
--rw-rw-rw-   0        0        0      776 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/main.py
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.484718 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/services/
--rw-rw-rw-   0        0        0     1406 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/services/Listener.py
--rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/services/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.485717 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/src/
--rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.486714 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/src/js/
--rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/src/js/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.486714 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/src/style/
--rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/src/style/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.488710 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/src/templates/
--rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/src/templates/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.491701 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/views/
--rw-rw-rw-   0        0        0    18146 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/views/Landing.py
--rw-rw-rw-   0        0        0     6877 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/views/Reporter.py
--rw-rw-rw-   0        0        0     8383 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/views/User.py
--rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/views/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-18 17:26:26.478736 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner.egg-info/
--rw-rw-rw-   0        0        0      309 2024-03-18 17:26:26.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      893 2024-03-18 17:26:26.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-18 17:26:26.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      785 2024-03-18 17:26:26.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-18 17:26:26.000000 Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       43 2024-03-18 14:04:09.000000 Andreani_QA_Scanner-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      309 2024-03-18 17:26:26.491701 Andreani_QA_Scanner-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       59 2024-03-18 12:07:28.000000 Andreani_QA_Scanner-0.0.8/README.md
--rw-rw-rw-   0        0        0       42 2024-03-18 17:26:26.492698 Andreani_QA_Scanner-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     2457 2024-03-18 17:26:14.000000 Andreani_QA_Scanner-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.700101 Andreani_QA_Scanner-0.0.9/
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.672479 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/
+-rw-rw-rw-   0        0        0       30 2024-03-18 13:04:01.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.689128 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/
+-rw-rw-rw-   0        0        0    20444 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/Scanner.py
+-rw-rw-rw-   0        0        0     2414 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/ScreenManagement.py
+-rw-rw-rw-   0        0        0    10724 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/ScriptToFile.py
+-rw-rw-rw-   0        0        0     6627 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/UserManagement.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/__init__.py
+-rw-rw-rw-   0        0        0      776 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/main.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.691123 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/services/
+-rw-rw-rw-   0        0        0     1406 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/services/Listener.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/services/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.692120 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/src/
+-rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.692120 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/src/js/
+-rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/src/js/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.693117 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/src/style/
+-rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/src/style/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.694115 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/src/templates/
+-rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/src/templates/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.698104 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/views/
+-rw-rw-rw-   0        0        0    18146 2024-03-18 13:35:11.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/views/Landing.py
+-rw-rw-rw-   0        0        0     6877 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/views/Reporter.py
+-rw-rw-rw-   0        0        0     8383 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/views/User.py
+-rw-rw-rw-   0        0        0        0 2024-03-18 13:00:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/views/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-18 17:40:48.684141 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner.egg-info/
+-rw-rw-rw-   0        0        0      309 2024-03-18 17:40:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      893 2024-03-18 17:40:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-18 17:40:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      785 2024-03-18 17:40:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-03-18 17:40:48.000000 Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       43 2024-03-18 14:04:09.000000 Andreani_QA_Scanner-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      309 2024-03-18 17:40:48.699101 Andreani_QA_Scanner-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       59 2024-03-18 12:07:28.000000 Andreani_QA_Scanner-0.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-18 17:40:48.700101 Andreani_QA_Scanner-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2472 2024-03-18 17:37:33.000000 Andreani_QA_Scanner-0.0.9/setup.py
```

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/Scanner.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/Scanner.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/ScreenManagement.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/ScreenManagement.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/ScriptToFile.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/ScriptToFile.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/app/UserManagement.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/app/UserManagement.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/main.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/main.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/services/Listener.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/services/Listener.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/views/Landing.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/views/Landing.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/views/Reporter.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/views/Reporter.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner/views/User.py` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner/views/User.py`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner.egg-info/SOURCES.txt` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/Andreani_QA_Scanner.egg-info/requires.txt` & `Andreani_QA_Scanner-0.0.9/Andreani_QA_Scanner.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `Andreani_QA_Scanner-0.0.8/setup.py` & `Andreani_QA_Scanner-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 PACKAGE_NAME = 'Andreani_QA_Scanner'  # Debe coincidir con el nombre de la carpeta
 AUTHOR = 'AndreaniTesting'
 AUTHOR_EMAIL = 'user_appglatest@andreani.com'
 URL = ''
 LICENSE = 'MIT'  # Tipo de licencia
 DESCRIPTION = 'SeleniumFramework para ejecución de casos automatizados'  # Descripción corta
 LONG_DESCRIPTION = ""
@@ -37,11 +37,11 @@
     url=URL,
     install_requires=INSTALL_REQUIRES,
     license=LICENSE,
     packages=find_packages(),
     package_data={
         'Andreani_QA_Scanner': ['app/*.js', 'app/extension/*.css', 'app/extension/*.png', 'app/extension/*.js',
                                 'app/extension/*.html', 'app/extension/*.svg', 'app/extension/*.json',
-                                'app/src/*.json', 'src/*.js', 'src/js/*.json', 'src/style/*.css',
+                                'app/src/*.json', 'src/*.js', 'src/js/*.json', 'src/js/*.js', 'src/style/*.css',
                                 'src/templates/*.html']},
     include_package_data=True
 )
```

