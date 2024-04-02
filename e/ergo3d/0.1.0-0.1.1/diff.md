# Comparing `tmp/ergo3d-0.1.0.tar.gz` & `tmp/ergo3d-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ergo3d-0.1.0.tar", last modified: Thu Mar 28 19:26:25 2024, max compression
+gzip compressed data, was "ergo3d-0.1.1.tar", last modified: Tue Apr  2 22:57:38 2024, max compression
```

## Comparing `ergo3d-0.1.0.tar` & `ergo3d-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-03-28 19:26:25.096556 ergo3d-0.1.0/
--rw-rw-rw-   0        0        0     1088 2024-02-02 20:31:08.000000 ergo3d-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      467 2024-03-28 19:26:25.096556 ergo3d-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      818 2024-02-02 21:21:07.000000 ergo3d-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-28 19:26:25.089558 ergo3d-0.1.0/ergo3d/
--rw-rw-rw-   0        0        0     5807 2024-03-28 18:13:13.000000 ergo3d-0.1.0/ergo3d/CoordinateSystem3D.py
--rw-rw-rw-   0        0        0    16718 2024-03-28 18:13:13.000000 ergo3d-0.1.0/ergo3d/JointAngles.py
--rw-rw-rw-   0        0        0     3175 2024-03-28 18:13:13.000000 ergo3d-0.1.0/ergo3d/Plane.py
--rw-rw-rw-   0        0        0    10358 2024-03-28 18:13:13.000000 ergo3d-0.1.0/ergo3d/Point.py
--rw-rw-rw-   0        0        0      157 2024-03-28 18:13:13.000000 ergo3d-0.1.0/ergo3d/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-28 19:26:25.095557 ergo3d-0.1.0/ergo3d.egg-info/
--rw-rw-rw-   0        0        0      467 2024-03-28 19:26:24.000000 ergo3d-0.1.0/ergo3d.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-03-28 19:26:25.000000 ergo3d-0.1.0/ergo3d.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-28 19:26:24.000000 ergo3d-0.1.0/ergo3d.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-03-28 19:26:24.000000 ergo3d-0.1.0/ergo3d.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-28 19:26:24.000000 ergo3d-0.1.0/ergo3d.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-28 19:26:25.097556 ergo3d-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1012 2024-02-02 20:57:54.000000 ergo3d-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.392226 ergo3d-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2024-02-02 20:31:08.000000 ergo3d-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      467 2024-04-02 22:57:38.392226 ergo3d-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      993 2024-04-02 22:57:36.000000 ergo3d-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.372224 ergo3d-0.1.1/ergo3d/
+-rw-rw-rw-   0        0        0       44 2024-04-02 22:51:33.000000 ergo3d-0.1.1/ergo3d/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.382236 ergo3d-0.1.1/ergo3d/camera/
+-rw-rw-rw-   0        0        0     4249 2024-04-02 22:55:21.000000 ergo3d-0.1.1/ergo3d/camera/Camera.py
+-rw-rw-rw-   0        0        0    13438 2024-04-02 22:55:21.000000 ergo3d-0.1.1/ergo3d/camera/FLIR_camera.py
+-rw-rw-rw-   0        0        0       24 2024-04-02 22:55:21.000000 ergo3d-0.1.1/ergo3d/camera/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.392226 ergo3d-0.1.1/ergo3d/geometry/
+-rw-rw-rw-   0        0        0     5807 2024-03-28 18:13:13.000000 ergo3d-0.1.1/ergo3d/geometry/CoordinateSystem3D.py
+-rw-rw-rw-   0        0        0    16718 2024-03-28 18:13:13.000000 ergo3d-0.1.1/ergo3d/geometry/JointAngles.py
+-rw-rw-rw-   0        0        0     3175 2024-03-28 18:13:13.000000 ergo3d-0.1.1/ergo3d/geometry/Plane.py
+-rw-rw-rw-   0        0        0    10358 2024-03-28 18:13:13.000000 ergo3d-0.1.1/ergo3d/geometry/Point.py
+-rw-rw-rw-   0        0        0      101 2024-04-02 22:50:46.000000 ergo3d-0.1.1/ergo3d/geometry/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:57:38.372224 ergo3d-0.1.1/ergo3d.egg-info/
+-rw-rw-rw-   0        0        0      467 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 22:57:38.000000 ergo3d-0.1.1/ergo3d.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 22:57:38.392226 ergo3d-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2024-04-02 22:57:08.000000 ergo3d-0.1.1/setup.py
```

### Comparing `ergo3d-0.1.0/LICENSE` & `ergo3d-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.0/README.md` & `ergo3d-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -15,12 +15,25 @@
 
 - `CoordinateSystem3D`: Provides a class for defining 3D coordinate systems.
 
 - `JointAngles`: Provides a class easy ergonomic angle calculations.
 
 ## Installation
 
+### build from source
 ```bash
 git clone https://github.com/LeyangWen/ergo3d.git
+
+
+```
+
+### install from PyPI
+```bash
+pip install ergo3d
 ```
 
+### Steps to update the package on PyPI
+```bash
+python setup.py sdist bdist_wheel
+
+
```

### Comparing `ergo3d-0.1.0/ergo3d/CoordinateSystem3D.py` & `ergo3d-0.1.1/ergo3d/geometry/CoordinateSystem3D.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.0/ergo3d/JointAngles.py` & `ergo3d-0.1.1/ergo3d/geometry/JointAngles.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.0/ergo3d/Plane.py` & `ergo3d-0.1.1/ergo3d/geometry/Plane.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.0/ergo3d/Point.py` & `ergo3d-0.1.1/ergo3d/geometry/Point.py`

 * *Files identical despite different names*

### Comparing `ergo3d-0.1.0/setup.py` & `ergo3d-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ergo3d',  # Name of your package
-    version='0.1.0',  # Version number
+    version='0.1.1',  # Version number
     description='A Python package for 3D ergonomic calculations.',  # Short description of your package
     url='https://github.com/LeyangWen/ergo3d',  # URL for your package's homepage
     author='Leyang Wen',  # Your name
     author_email='wenleyan@umich.edu',  # Your email
     license='MIT',  # License type for your package
     packages=find_packages(),  # Automatically find all packages and subpackages
     install_requires=[  # List of dependencies
```

