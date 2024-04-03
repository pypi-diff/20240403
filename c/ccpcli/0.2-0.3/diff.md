# Comparing `tmp/ccpcli-0.2.tar.gz` & `tmp/ccpcli-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccpcli-0.2.tar", last modified: Tue Apr  2 11:18:27 2024, max compression
+gzip compressed data, was "ccpcli-0.3.tar", last modified: Wed Apr  3 06:32:36 2024, max compression
```

## Comparing `ccpcli-0.2.tar` & `ccpcli-0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.234756 ccpcli-0.2/
--rw-r--r--   0 shubham    (501) staff       (20)      181 2024-04-02 11:18:27.234556 ccpcli-0.2/PKG-INFO
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.234242 ccpcli-0.2/ccpcli.egg-info/
--rw-r--r--   0 shubham    (501) staff       (20)      181 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/PKG-INFO
--rw-r--r--   0 shubham    (501) staff       (20)      675 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/SOURCES.txt
--rw-r--r--   0 shubham    (501) staff       (20)        1 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/dependency_links.txt
--rw-r--r--   0 shubham    (501) staff       (20)       39 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/entry_points.txt
--rw-r--r--   0 shubham    (501) staff       (20)       20 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/requires.txt
--rw-r--r--   0 shubham    (501) staff       (20)       14 2024-04-02 11:18:27.000000 ccpcli-0.2/ccpcli.egg-info/top_level.txt
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.229021 ccpcli-0.2/resources/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/resources/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)       38 2024-04-02 11:18:27.234803 ccpcli-0.2/setup.cfg
--rw-r--r--   0 shubham    (501) staff       (20)      863 2024-04-02 10:52:45.000000 ccpcli-0.2/setup.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.229744 ccpcli-0.2/src/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     5552 2024-04-02 09:53:33.000000 ccpcli-0.2/src/cli.py
--rw-r--r--   0 shubham    (501) staff       (20)     5546 2024-04-02 09:53:33.000000 ccpcli-0.2/src/project.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.231651 ccpcli-0.2/src/resource_schemas/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/resource_schemas/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     2864 2024-04-02 09:53:33.000000 ccpcli-0.2/src/resource_schemas/network.py
--rw-r--r--   0 shubham    (501) staff       (20)     1223 2024-04-02 09:53:33.000000 ccpcli-0.2/src/resource_schemas/project.py
--rw-r--r--   0 shubham    (501) staff       (20)     1124 2024-04-02 09:53:33.000000 ccpcli-0.2/src/resource_schemas/volume.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.232427 ccpcli-0.2/src/service/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/__init__.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.232806 ccpcli-0.2/src/service/network/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/network/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     2860 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/network/network.py
--rw-r--r--   0 shubham    (501) staff       (20)     1669 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/network/security_group.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.233085 ccpcli-0.2/src/service/volume/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/volume/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     2703 2024-04-02 09:53:33.000000 ccpcli-0.2/src/service/volume/volume.py
-drwxr-xr-x   0 shubham    (501) staff       (20)        0 2024-04-02 11:18:27.233946 ccpcli-0.2/src/util/
--rw-r--r--   0 shubham    (501) staff       (20)        0 2024-04-02 09:53:33.000000 ccpcli-0.2/src/util/__init__.py
--rw-r--r--   0 shubham    (501) staff       (20)     4814 2024-04-02 10:50:35.000000 ccpcli-0.2/src/util/constants.py
--rw-r--r--   0 shubham    (501) staff       (20)     1593 2024-04-02 09:53:33.000000 ccpcli-0.2/src/util/file_utils.py
--rw-r--r--   0 shubham    (501) staff       (20)     3219 2024-04-02 09:53:33.000000 ccpcli-0.2/src/util/http_helper.py
--rw-r--r--   0 shubham    (501) staff       (20)     4697 2024-04-02 09:53:33.000000 ccpcli-0.2/src/util/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.940156 ccpcli-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 06:32:36.940156 ccpcli-0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.940156 ccpcli-0.3/ccpcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 06:32:36.000000 ccpcli-0.3/ccpcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-03 06:32:36.000000 ccpcli-0.3/ccpcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:32:36.000000 ccpcli-0.3/ccpcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 06:32:36.000000 ccpcli-0.3/ccpcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 06:32:36.000000 ccpcli-0.3/ccpcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 06:32:36.000000 ccpcli-0.3/ccpcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.936156 ccpcli-0.3/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:18.000000 ccpcli-0.3/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:32:36.940156 ccpcli-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-03 06:32:18.000000 ccpcli-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.936156 ccpcli-0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:18.000000 ccpcli-0.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-03 06:32:18.000000 ccpcli-0.3/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5546 2024-04-03 06:32:18.000000 ccpcli-0.3/src/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.936156 ccpcli-0.3/src/resource_schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:18.000000 ccpcli-0.3/src/resource_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-03 06:32:18.000000 ccpcli-0.3/src/resource_schemas/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-03 06:32:18.000000 ccpcli-0.3/src/resource_schemas/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-03 06:32:18.000000 ccpcli-0.3/src/resource_schemas/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.936156 ccpcli-0.3/src/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:18.000000 ccpcli-0.3/src/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.940156 ccpcli-0.3/src/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:18.000000 ccpcli-0.3/src/service/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-03 06:32:18.000000 ccpcli-0.3/src/service/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-03 06:32:18.000000 ccpcli-0.3/src/service/network/security_group.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.940156 ccpcli-0.3/src/service/volume/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:18.000000 ccpcli-0.3/src/service/volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-04-03 06:32:18.000000 ccpcli-0.3/src/service/volume/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:36.940156 ccpcli-0.3/src/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:32:18.000000 ccpcli-0.3/src/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4828 2024-04-03 06:32:18.000000 ccpcli-0.3/src/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-04-03 06:32:18.000000 ccpcli-0.3/src/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-03 06:32:18.000000 ccpcli-0.3/src/util/http_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-03 06:32:18.000000 ccpcli-0.3/src/util/utils.py
```

### Comparing `ccpcli-0.2/ccpcli.egg-info/SOURCES.txt` & `ccpcli-0.3/ccpcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/setup.py` & `ccpcli-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Written by Mani Keshari <mani@coredge.io>, March 2024                       #
 ###############################################################################
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name='ccpcli',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     author='Mani Keshari',
     author_email='mani@coredge.io',
     description='CCP cli',
     install_requires=['click', 'halo', 'tabulate'],
     entry_points={
         'console_scripts': [
```

### Comparing `ccpcli-0.2/src/cli.py` & `ccpcli-0.3/src/cli.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/project.py` & `ccpcli-0.3/src/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/resource_schemas/network.py` & `ccpcli-0.3/src/resource_schemas/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/resource_schemas/project.py` & `ccpcli-0.3/src/resource_schemas/project.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/resource_schemas/volume.py` & `ccpcli-0.3/src/resource_schemas/volume.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/service/network/network.py` & `ccpcli-0.3/src/service/network/network.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/service/network/security_group.py` & `ccpcli-0.3/src/service/network/security_group.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/service/volume/volume.py` & `ccpcli-0.3/src/service/volume/volume.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/util/constants.py` & `ccpcli-0.3/src/util/constants.py`

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
-    os.sep, 'resources', f'env-{profile}')
+    os.getcwd() + os.sep, 'resources', f'env-{profile}')
 
 
 def read_properties(property_file_path):
     ''' read properties of environment property_file_path and returning dict '''
     try:
         with open(property_file_path, 'r') as f:
             data = f.read()
```

### Comparing `ccpcli-0.2/src/util/file_utils.py` & `ccpcli-0.3/src/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/util/http_helper.py` & `ccpcli-0.3/src/util/http_helper.py`

 * *Files identical despite different names*

### Comparing `ccpcli-0.2/src/util/utils.py` & `ccpcli-0.3/src/util/utils.py`

 * *Files identical despite different names*

