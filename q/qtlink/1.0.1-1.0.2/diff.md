# Comparing `tmp/qtlink-1.0.1.tar.gz` & `tmp/qtlink-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtlink-1.0.1.tar", last modified: Wed Apr  3 12:30:36 2024, max compression
+gzip compressed data, was "qtlink-1.0.2.tar", last modified: Wed Apr  3 12:54:21 2024, max compression
```

## Comparing `qtlink-1.0.1.tar` & `qtlink-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 12:30:36.684238 qtlink-1.0.1/
--rw-rw-rw-   0        0        0      492 2024-04-03 12:30:36.684238 qtlink-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       41 2024-03-17 08:35:49.000000 qtlink-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 12:30:36.670665 qtlink-1.0.1/qtlink/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:53:11.000000 qtlink-1.0.1/qtlink/__init__.py
--rw-rw-rw-   0        0        0      182 2024-04-03 06:56:46.000000 qtlink-1.0.1/qtlink/util.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:30:36.684238 qtlink-1.0.1/qtlink.egg-info/
--rw-rw-rw-   0        0        0      492 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 12:30:36.000000 qtlink-1.0.1/qtlink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-03 12:30:36.684238 qtlink-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      614 2024-04-03 12:20:03.000000 qtlink-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:54:21.019686 qtlink-1.0.2/
+-rw-rw-rw-   0        0        0     7816 2024-04-03 12:33:35.000000 qtlink-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      515 2024-04-03 12:54:21.014987 qtlink-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-04-03 12:35:06.000000 qtlink-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 12:54:20.992961 qtlink-1.0.2/qtlink/
+-rw-rw-rw-   0        0        0       92 2024-04-03 12:51:18.000000 qtlink-1.0.2/qtlink/__init__.py
+-rw-rw-rw-   0        0        0      182 2024-04-03 06:56:46.000000 qtlink-1.0.2/qtlink/util.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:54:21.014987 qtlink-1.0.2/qtlink.egg-info/
+-rw-rw-rw-   0        0        0      515 2024-04-03 12:54:20.000000 qtlink-1.0.2/qtlink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      209 2024-04-03 12:54:20.000000 qtlink-1.0.2/qtlink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:54:20.000000 qtlink-1.0.2/qtlink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-04-03 12:54:20.000000 qtlink-1.0.2/qtlink.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 12:54:20.000000 qtlink-1.0.2/qtlink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 12:54:21.019686 qtlink-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      614 2024-04-03 12:51:18.000000 qtlink-1.0.2/setup.py
```

### Comparing `qtlink-1.0.1/setup.py` & `qtlink-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="qtlink",
-    version="1.0.1",
+    version="1.0.2",
     author="NanHaiLoong",
     author_email="nanhai@163.com",
     description="a ui framework based on pyside6",
     long_description='a ui framework based on pyside6',
     long_description_content_type="text/markdown",
     url="https://gitee.com/darlingxyz/qtlink",
     install_requires=['PySide6', 'matplotlib', 'numpy'],
```

