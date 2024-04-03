# Comparing `tmp/specnn4pde-0.0.1.tar.gz` & `tmp/specnn4pde-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specnn4pde-0.0.1.tar", last modified: Wed Apr  3 07:35:44 2024, max compression
+gzip compressed data, was "specnn4pde-0.0.2.tar", last modified: Wed Apr  3 06:54:01 2024, max compression
```

## Comparing `specnn4pde-0.0.1.tar` & `specnn4pde-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 07:35:44.735372 specnn4pde-0.0.1/
--rw-rw-rw-   0        0        0     1091 2024-04-03 06:49:12.000000 specnn4pde-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2716 2024-04-03 07:35:44.734370 specnn4pde-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1654 2024-04-03 06:39:13.000000 specnn4pde-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 07:35:44.735372 specnn4pde-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1709 2024-04-03 07:35:36.000000 specnn4pde-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:35:44.717918 specnn4pde-0.0.1/specnn4pde/
--rw-rw-rw-   0        0        0        0 2023-11-10 02:06:30.000000 specnn4pde-0.0.1/specnn4pde/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-03-15 09:39:53.000000 specnn4pde-0.0.1/specnn4pde/linalg.py
--rw-rw-rw-   0        0        0    12133 2024-04-03 03:41:58.000000 specnn4pde-0.0.1/specnn4pde/npde.py
--rw-rw-rw-   0        0        0    16254 2024-04-03 05:24:24.000000 specnn4pde-0.0.1/specnn4pde/spectral.py
--rw-rw-rw-   0        0        0     6621 2024-03-20 02:37:42.000000 specnn4pde-0.0.1/specnn4pde/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-03 07:35:44.733381 specnn4pde-0.0.1/specnn4pde.egg-info/
--rw-rw-rw-   0        0        0     2716 2024-04-03 07:35:44.000000 specnn4pde-0.0.1/specnn4pde.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      301 2024-04-03 07:35:44.000000 specnn4pde-0.0.1/specnn4pde.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 07:35:44.000000 specnn4pde-0.0.1/specnn4pde.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-04-03 07:35:44.000000 specnn4pde-0.0.1/specnn4pde.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-03 07:35:44.000000 specnn4pde-0.0.1/specnn4pde.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 06:54:01.909791 specnn4pde-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 06:49:12.000000 specnn4pde-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2716 2024-04-03 06:54:01.908790 specnn4pde-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1654 2024-04-03 06:39:13.000000 specnn4pde-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 06:54:01.900791 specnn4pde-0.0.2/mxwpy/
+-rw-rw-rw-   0        0        0        0 2023-11-10 02:06:30.000000 specnn4pde-0.0.2/mxwpy/__init__.py
+-rw-rw-rw-   0        0        0     1755 2024-03-15 09:39:53.000000 specnn4pde-0.0.2/mxwpy/linalg.py
+-rw-rw-rw-   0        0        0    12133 2024-04-03 03:41:58.000000 specnn4pde-0.0.2/mxwpy/npde.py
+-rw-rw-rw-   0        0        0    16254 2024-04-03 05:24:24.000000 specnn4pde-0.0.2/mxwpy/spectral.py
+-rw-rw-rw-   0        0        0     6621 2024-03-20 02:37:42.000000 specnn4pde-0.0.2/mxwpy/tools.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 06:54:01.909791 specnn4pde-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1709 2024-04-03 06:53:53.000000 specnn4pde-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:54:01.907791 specnn4pde-0.0.2/specnn4pde.egg-info/
+-rw-rw-rw-   0        0        0     2716 2024-04-03 06:54:01.000000 specnn4pde-0.0.2/specnn4pde.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-04-03 06:54:01.000000 specnn4pde-0.0.2/specnn4pde.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 06:54:01.000000 specnn4pde-0.0.2/specnn4pde.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-03 06:54:01.000000 specnn4pde-0.0.2/specnn4pde.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-03 06:54:01.000000 specnn4pde-0.0.2/specnn4pde.egg-info/top_level.txt
```

### Comparing `specnn4pde-0.0.1/LICENSE` & `specnn4pde-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.1/PKG-INFO` & `specnn4pde-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specnn4pde
-Version: 0.0.1
+Version: 0.0.2
 Summary: Solving partial differential equations using spectral methods and neural networks.
 Home-page: https://github.com/mxweng/specnn4pde
 Author: MXWeng
 Author-email: 2431141461@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `specnn4pde-0.0.1/README.md` & `specnn4pde-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.1/setup.py` & `specnn4pde-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.command import install_data
 from setuptools import setup, find_packages
 
 setup(
     name='specnn4pde',  # package name
-    version='0.0.1',  # version
+    version='0.0.2',  # version
     author='MXWeng',  # author name
     author_email='2431141461@qq.com',  # author email
     description='Solving partial differential equations using spectral methods and neural networks.',  # short description
     long_description=open('README.md').read(),  # long description, usually your README
     long_description_content_type='text/markdown',  # format of the long description, 'text/markdown' if it's Markdown
     url='https://github.com/mxweng/specnn4pde',  # project homepage
     packages=find_packages(),  # automatically discover all packages
```

### Comparing `specnn4pde-0.0.1/specnn4pde/linalg.py` & `specnn4pde-0.0.2/mxwpy/linalg.py`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.1/specnn4pde/npde.py` & `specnn4pde-0.0.2/mxwpy/npde.py`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.1/specnn4pde/spectral.py` & `specnn4pde-0.0.2/mxwpy/spectral.py`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.1/specnn4pde/tools.py` & `specnn4pde-0.0.2/mxwpy/tools.py`

 * *Files identical despite different names*

### Comparing `specnn4pde-0.0.1/specnn4pde.egg-info/PKG-INFO` & `specnn4pde-0.0.2/specnn4pde.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specnn4pde
-Version: 0.0.1
+Version: 0.0.2
 Summary: Solving partial differential equations using spectral methods and neural networks.
 Home-page: https://github.com/mxweng/specnn4pde
 Author: MXWeng
 Author-email: 2431141461@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

