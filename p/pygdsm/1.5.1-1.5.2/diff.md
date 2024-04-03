# Comparing `tmp/pygdsm-1.5.1.tar.gz` & `tmp/pygdsm-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygdsm-1.5.1.tar", last modified: Fri Mar 29 01:45:16 2024, max compression
+gzip compressed data, was "pygdsm-1.5.2.tar", last modified: Wed Apr  3 07:41:31 2024, max compression
```

## Comparing `pygdsm-1.5.1.tar` & `pygdsm-1.5.2.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:45:16.714763 pygdsm-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 01:44:57.000000 pygdsm-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-03-29 01:45:16.714763 pygdsm-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-03-29 01:44:57.000000 pygdsm-1.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:45:16.710763 pygdsm-1.5.1/pygdsm/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/base_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/base_skymodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/component_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/gsm08.py
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/gsm16.py
--rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/haslam.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/lfsm.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-29 01:44:57.000000 pygdsm-1.5.1/pygdsm/plot_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:45:16.714763 pygdsm-1.5.1/pygdsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-03-29 01:45:16.000000 pygdsm-1.5.1/pygdsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-29 01:45:16.000000 pygdsm-1.5.1/pygdsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 01:45:16.000000 pygdsm-1.5.1/pygdsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 01:45:16.000000 pygdsm-1.5.1/pygdsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 01:45:16.000000 pygdsm-1.5.1/pygdsm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-29 01:45:16.714763 pygdsm-1.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-03-29 01:44:57.000000 pygdsm-1.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 01:45:16.714763 pygdsm-1.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-03-29 01:44:57.000000 pygdsm-1.5.1/tests/test_gsm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-03-29 01:44:57.000000 pygdsm-1.5.1/tests/test_gsm2016.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-03-29 01:44:57.000000 pygdsm-1.5.1/tests/test_gsm_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-29 01:44:57.000000 pygdsm-1.5.1/tests/test_haslam.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-29 01:44:57.000000 pygdsm-1.5.1/tests/test_lfsm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:41:31.550586 pygdsm-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-03 07:41:11.000000 pygdsm-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 07:41:11.000000 pygdsm-1.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-03 07:41:31.550586 pygdsm-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-04-03 07:41:11.000000 pygdsm-1.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:41:31.546585 pygdsm-1.5.2/pygdsm/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/base_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4198 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/base_skymodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/component_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7530 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/gsm08.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/gsm16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/haslam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/lfsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 07:41:11.000000 pygdsm-1.5.2/pygdsm/plot_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:41:31.550586 pygdsm-1.5.2/pygdsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8251 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 07:41:31.000000 pygdsm-1.5.2/pygdsm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-03 07:41:11.000000 pygdsm-1.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 07:41:11.000000 pygdsm-1.5.2/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 07:41:31.550586 pygdsm-1.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-03 07:41:11.000000 pygdsm-1.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:41:31.550586 pygdsm-1.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_gsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_gsm2016.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_gsm_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_haslam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-03 07:41:11.000000 pygdsm-1.5.2/tests/test_lfsm.py
```

### Comparing `pygdsm-1.5.1/LICENSE` & `pygdsm-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/PKG-INFO` & `pygdsm-1.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pygdsm
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python Global Sky Model of diffuse Galactic radio emission
 Home-page: https://github.com/telegraphic/pygdsm
-Author: Danny Price
-Author-email: dancpr@berkeley.edu
+Author: Danny C. Price
+Author-email: daniel.price@skao.int
 License: MIT
 Keywords: radio astronomy sky model galactic diffuse emission
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygdsm-1.5.1/README.md` & `pygdsm-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/pygdsm/base_observer.py` & `pygdsm-1.5.2/pygdsm/base_observer.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/pygdsm/base_skymodel.py` & `pygdsm-1.5.2/pygdsm/base_skymodel.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/pygdsm/component_data.py` & `pygdsm-1.5.2/pygdsm/component_data.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/pygdsm/gsm08.py` & `pygdsm-1.5.2/pygdsm/gsm08.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/pygdsm/gsm16.py` & `pygdsm-1.5.2/pygdsm/gsm16.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/pygdsm/haslam.py` & `pygdsm-1.5.2/pygdsm/haslam.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/pygdsm/lfsm.py` & `pygdsm-1.5.2/pygdsm/lfsm.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/pygdsm.egg-info/PKG-INFO` & `pygdsm-1.5.2/pygdsm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pygdsm
-Version: 1.5.1
+Version: 1.5.2
 Summary: Python Global Sky Model of diffuse Galactic radio emission
 Home-page: https://github.com/telegraphic/pygdsm
-Author: Danny Price
-Author-email: dancpr@berkeley.edu
+Author: Danny C. Price
+Author-email: daniel.price@skao.int
 License: MIT
 Keywords: radio astronomy sky model galactic diffuse emission
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pygdsm-1.5.1/setup.py` & `pygdsm-1.5.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 setup(
     name='pygdsm',
 
     # Versions should comply with PEP440.  For a discussion on single-sourcing
     # the version across setup.py and the project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.5.1',
+    version='1.5.2',
 
     description='Python Global Sky Model of diffuse Galactic radio emission',
     long_description=long_description,
     long_description_content_type='text/markdown',
 
     # The project's main homepage.
     url='https://github.com/telegraphic/pygdsm',
 
     # Author details
-    author='Danny Price',
-    author_email='dancpr@berkeley.edu',
+    author='Danny C. Price',
+    author_email='daniel.price@skao.int',
 
     # Choose your license
     license='MIT',
 
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         # How mature is this project? Common values are
```

### Comparing `pygdsm-1.5.1/tests/test_gsm.py` & `pygdsm-1.5.2/tests/test_gsm.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/tests/test_gsm2016.py` & `pygdsm-1.5.2/tests/test_gsm2016.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/tests/test_gsm_observer.py` & `pygdsm-1.5.2/tests/test_gsm_observer.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/tests/test_haslam.py` & `pygdsm-1.5.2/tests/test_haslam.py`

 * *Files identical despite different names*

### Comparing `pygdsm-1.5.1/tests/test_lfsm.py` & `pygdsm-1.5.2/tests/test_lfsm.py`

 * *Files identical despite different names*

