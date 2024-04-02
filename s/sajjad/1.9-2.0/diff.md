# Comparing `tmp/sajjad-1.9.tar.gz` & `tmp/sajjad-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sajjad-1.9.tar", last modified: Tue Apr  2 14:16:08 2024, max compression
+gzip compressed data, was "sajjad-2.0.tar", last modified: Tue Apr  2 14:36:57 2024, max compression
```

## Comparing `sajjad-1.9.tar` & `sajjad-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 14:16:08.698794 sajjad-1.9/
--rw-rw-rw-   0        0        0      490 2024-04-02 14:16:08.697795 sajjad-1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-02 14:16:08.684175 sajjad-1.9/sajjad/
--rw-rw-rw-   0        0        0       21 2024-04-01 20:31:53.000000 sajjad-1.9/sajjad/__init__.py
--rw-rw-rw-   0        0        0      248 2024-04-01 23:15:53.000000 sajjad-1.9/sajjad/sajjad.py
-drwxrwxrwx   0        0        0        0 2024-04-02 14:16:08.696795 sajjad-1.9/sajjad.egg-info/
--rw-rw-rw-   0        0        0      490 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      193 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 14:16:08.000000 sajjad-1.9/sajjad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 14:16:08.698794 sajjad-1.9/setup.cfg
--rw-rw-rw-   0        0        0      639 2024-04-02 14:15:56.000000 sajjad-1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:36:57.571980 sajjad-2.0/
+-rw-rw-rw-   0        0        0      490 2024-04-02 14:36:57.570976 sajjad-2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-02 14:36:57.555771 sajjad-2.0/sajjad/
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:36:38.000000 sajjad-2.0/sajjad/__init__.py
+-rw-rw-rw-   0        0        0      248 2024-04-01 23:15:53.000000 sajjad-2.0/sajjad/sajjad.py
+drwxrwxrwx   0        0        0        0 2024-04-02 14:36:57.570004 sajjad-2.0/sajjad.egg-info/
+-rw-rw-rw-   0        0        0      490 2024-04-02 14:36:57.000000 sajjad-2.0/sajjad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      193 2024-04-02 14:36:57.000000 sajjad-2.0/sajjad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 14:36:57.000000 sajjad-2.0/sajjad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-02 14:36:57.000000 sajjad-2.0/sajjad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 14:36:57.000000 sajjad-2.0/sajjad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 14:36:57.571980 sajjad-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      639 2024-04-02 14:36:20.000000 sajjad-2.0/setup.py
```

### Comparing `sajjad-1.9/setup.py` & `sajjad-2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sajjad',
-    version='1.9',
+    version='2.0',
     packages=find_packages(),
     description='Sajjad developer creatd this library',
     author='sajjad seyedi',
     author_email='sajjad.seyedi.88@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

