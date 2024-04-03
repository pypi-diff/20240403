# Comparing `tmp/ccpcli-0.1.tar.gz` & `tmp/ccpcli-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpcli-0.1.tar", last modified: Tue Apr  2 08:11:45 2024, max compression
+gzip compressed data, was "ccpcli-0.2.tar", last modified: Tue Apr  2 11:18:27 2024, max compression
```

## Comparing `ccpcli-0.1.tar` & `ccpcli-0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.457722 ccpcli-0.1/
--rw-r--r--   0 shubham    (501) staff       (20)      181 2024-04-02 08:11:45.457396 ccpcli-0.1/PKG-INFO
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.456930 ccpcli-0.1/ccpcli.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)      181 2024-04-02 08:11:45.000000 ccpcli-0.1/ccpcli.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      675 2024-04-02 08:11:45.000000 ccpcli-0.1/ccpcli.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2024-04-02 08:11:45.000000 ccpcli-0.1/ccpcli.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       39 2024-04-02 08:11:45.000000 ccpcli-0.1/ccpcli.egg-info/entry_points.txt
--rw-r--r--   0 shubham    (501) staff       (20)       20 2024-04-02 08:11:45.000000 ccpcli-0.1/ccpcli.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       14 2024-04-02 08:11:45.000000 ccpcli-0.1/ccpcli.egg-info/top_level.txt
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.449387 ccpcli-0.1/resources/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 07:44:18.000000 ccpcli-0.1/resources/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)       38 2024-04-02 08:11:45.457812 ccpcli-0.1/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)      863 2024-04-02 07:44:18.000000 ccpcli-0.1/setup.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.450248 ccpcli-0.1/src/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 07:44:18.000000 ccpcli-0.1/src/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     5552 2024-04-02 07:44:18.000000 ccpcli-0.1/src/cli.py
--rw-r--r--   0 shubham    (501) staff       (20)     5546 2024-04-02 07:44:18.000000 ccpcli-0.1/src/project.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.451933 ccpcli-0.1/src/resource_schemas/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 07:44:18.000000 ccpcli-0.1/src/resource_schemas/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     2864 2024-04-02 07:44:18.000000 ccpcli-0.1/src/resource_schemas/network.py
--rw-r--r--   0 shubham    (501) staff       (20)     1223 2024-04-02 07:44:18.000000 ccpcli-0.1/src/resource_schemas/project.py
--rw-r--r--   0 shubham    (501) staff       (20)     1124 2024-04-02 07:44:18.000000 ccpcli-0.1/src/resource_schemas/volume.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.452364 ccpcli-0.1/src/service/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 07:44:18.000000 ccpcli-0.1/src/service/__init__.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.453127 ccpcli-0.1/src/service/network/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 07:44:18.000000 ccpcli-0.1/src/service/network/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     2860 2024-04-02 07:44:18.000000 ccpcli-0.1/src/service/network/network.py
--rw-r--r--   0 shubham    (501) staff       (20)     1669 2024-04-02 07:44:18.000000 ccpcli-0.1/src/service/network/security_group.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.453747 ccpcli-0.1/src/service/volume/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 07:44:18.000000 ccpcli-0.1/src/service/volume/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     2703 2024-04-02 07:44:18.000000 ccpcli-0.1/src/service/volume/volume.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 08:11:45.456266 ccpcli-0.1/src/util/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 07:44:18.000000 ccpcli-0.1/src/util/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     4828 2024-04-02 07:44:18.000000 ccpcli-0.1/src/util/constants.py
--rw-r--r--   0 shubham    (501) staff       (20)     1593 2024-04-02 07:44:18.000000 ccpcli-0.1/src/util/file_utils.py
--rw-r--r--   0 shubham    (501) staff       (20)     3219 2024-04-02 07:44:18.000000 ccpcli-0.1/src/util/http_helper.py
--rw-r--r--   0 shubham    (501) staff       (20)     4697 2024-04-02 07:44:18.000000 ccpcli-0.1/src/util/utils.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.234756 ccpcli-0.2/
+-rw-r--r--   0 shubham    (501) staff       (20)      181 2024-04-02 11:18:27.234556 ccpcli-0.2/PKG-INFO
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.234242 ccpcli-0.2/ccpcli.egg-info/
+-rw-r--r--   0 shubham    (501) staff       (20)      181 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/PKG-INFO
+-rw-r--r--   0 shubham    (501) staff       (20)      675 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/SOURCES.txt
+-rw-r--r--   0 shubham    (501) staff       (20)        1 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/dependency_links.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       39 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/entry_points.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       20 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/requires.txt
+-rw-r--r--   0 shubham    (501) staff       (20)       14 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/top_level.txt
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.229021 ccpcli-0.2/resources/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/resources/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)       38 2024-04-02 11:18:27.234803 ccpcli-0.2/setup.cfg
+-rw-r--r--   0 shubham    (501) staff       (20)      863 2024-04-02 10:52:45.000000 ccpcli-0.2/setup.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.229744 ccpcli-0.2/src/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5552 2024-04-02 09:53:33.000000 ccpcli-0.2/src/cli.py
+-rw-r--r--   0 shubham    (501) staff       (20)     5546 2024-04-02 09:53:33.000000 ccpcli-0.2/src/project.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.231651 ccpcli-0.2/src/resource_schemas/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/resource_schemas/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     2864 2024-04-02 09:53:33.000000 ccpcli-0.2/src/resource_schemas/network.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1223 2024-04-02 09:53:33.000000 ccpcli-0.2/src/resource_schemas/project.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1124 2024-04-02 09:53:33.000000 ccpcli-0.2/src/resource_schemas/volume.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.232427 ccpcli-0.2/src/service/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/__init__.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.232806 ccpcli-0.2/src/service/network/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/network/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     2860 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/network/network.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1669 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/network/security_group.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.233085 ccpcli-0.2/src/service/volume/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/volume/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     2703 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/volume/volume.py
+drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.233946 ccpcli-0.2/src/util/
+-rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/util/__init__.py
+-rw-r--r--   0 shubham    (501) staff       (20)     4814 2024-04-02 10:50:35.000000 ccpcli-0.2/src/util/constants.py
+-rw-r--r--   0 shubham    (501) staff       (20)     1593 2024-04-02 09:53:33.000000 ccpcli-0.2/src/util/file_utils.py
+-rw-r--r--   0 shubham    (501) staff       (20)     3219 2024-04-02 09:53:33.000000 ccpcli-0.2/src/util/http_helper.py
+-rw-r--r--   0 shubham    (501) staff       (20)     4697 2024-04-02 09:53:33.000000 ccpcli-0.2/src/util/utils.py
```

### Comparing `ccpcli-0.1/ccpcli.egg-info/SOURCES.txt` & `ccpcli-0.2/ccpcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/setup.py` & `ccpcli-0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Written by Mani Keshari <mani@coredge.io>, March 2024                       #
 ###############################################################################
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='ccpcli',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     author='Mani Keshari',
     author_email='mani@coredge.io',
     description='CCP cli',
     install_requires=['click', 'halo', 'tabulate'],
     entry_points={
         'console_scripts': [
```

### Comparing `ccpcli-0.1/src/cli.py` & `ccpcli-0.2/src/cli.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/project.py` & `ccpcli-0.2/src/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/resource_schemas/network.py` & `ccpcli-0.2/src/resource_schemas/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/resource_schemas/project.py` & `ccpcli-0.2/src/resource_schemas/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/resource_schemas/volume.py` & `ccpcli-0.2/src/resource_schemas/volume.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/service/network/network.py` & `ccpcli-0.2/src/service/network/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/service/network/security_group.py` & `ccpcli-0.2/src/service/network/security_group.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/service/volume/volume.py` & `ccpcli-0.2/src/service/volume/volume.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/util/constants.py` & `ccpcli-0.2/src/util/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Unauthorized copying of this file, via any medium is strictly prohibited    #
 # Proprietary and confidential                                                #
 # Written by Mani Keshari <mani@coredge.io>, March 2024                       #
 ###############################################################################
 import os
 profile = os.getenv('YNTRAA_CLI_PROFILE', 'dev')
 ENV_DEV_FILE_PATH = os.path.join(
-    os.getcwd() + os.sep, 'resources', f'env-{profile}')
+    os.sep, 'resources', f'env-{profile}')
 
 
 def read_properties(property_file_path):
     ''' read properties of environment property_file_path and returning dict '''
     try:
         with open(property_file_path, 'r') as f:
             data = f.read()
```

### Comparing `ccpcli-0.1/src/util/file_utils.py` & `ccpcli-0.2/src/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/util/http_helper.py` & `ccpcli-0.2/src/util/http_helper.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.1/src/util/utils.py` & `ccpcli-0.2/src/util/utils.py`

 * *Files identical despite different names*

