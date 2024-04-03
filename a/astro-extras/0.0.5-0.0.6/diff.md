# Comparing `tmp/astro_extras-0.0.5.tar.gz` & `tmp/astro_extras-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro_extras-0.0.5.tar", last modified: Tue Apr  2 08:24:42 2024, max compression
+gzip compressed data, was "astro_extras-0.0.6.tar", last modified: Wed Apr  3 12:26:13 2024, max compression
```

## Comparing `astro_extras-0.0.5.tar` & `astro_extras-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.248114 astro_extras-0.0.5/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.5/LICENSE
--rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.5/MANIFEST.in
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-02 08:24:42.248114 astro_extras-0.0.5/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.5/README.md
--rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.5/pyproject.toml
--rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.5/requirements.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-04-02 08:24:42.248114 astro_extras-0.0.5/setup.cfg
--rw-rw-r--   0 kol       (1000) kol       (1000)     1085 2024-04-02 07:11:17.000000 astro_extras-0.0.5/setup.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.236114 astro_extras-0.0.5/src/
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.236114 astro_extras-0.0.5/src/astro_extras/
--rw-rw-r--   0 kol       (1000) kol       (1000)     1000 2024-04-02 07:23:04.000000 astro_extras-0.0.5/src/astro_extras/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.244114 astro_extras-0.0.5/src/astro_extras/hooks/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.5/src/astro_extras/hooks/__init__.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.244114 astro_extras-0.0.5/src/astro_extras/operators/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.5/src/astro_extras/operators/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     3880 2023-10-26 14:10:20.000000 astro_extras-0.0.5/src/astro_extras/operators/direct.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    18057 2023-11-20 09:48:16.000000 astro_extras-0.0.5/src/astro_extras/operators/session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    22741 2024-03-11 14:32:23.000000 astro_extras-0.0.5/src/astro_extras/operators/table.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.248114 astro_extras-0.0.5/src/astro_extras/utils/
--rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.5/src/astro_extras/utils/__init__.py
--rw-rw-r--   0 kol       (1000) kol       (1000)    10549 2023-11-17 15:24:02.000000 astro_extras-0.0.5/src/astro_extras/utils/data_compare.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.5/src/astro_extras/utils/datetime_local.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.5/src/astro_extras/utils/template.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1952 2024-03-28 14:14:29.000000 astro_extras-0.0.5/src/astro_extras/utils/utils.py
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.248114 astro_extras-0.0.5/src/astro_extras.egg-info/
--rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/PKG-INFO
--rw-rw-r--   0 kol       (1000) kol       (1000)      751 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/SOURCES.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/dependency_links.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/requires.txt
--rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-04-02 08:24:42.000000 astro_extras-0.0.5/src/astro_extras.egg-info/top_level.txt
-drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-02 08:24:42.248114 astro_extras-0.0.5/tests/
--rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.5/tests/test_session.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.5/tests/test_table.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.5/tests/test_templates.py
--rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.5/tests/test_utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.623833 astro_extras-0.0.6/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1074 2023-11-17 10:43:31.000000 astro_extras-0.0.6/LICENSE
+-rw-rw-r--   0 kol       (1000) kol       (1000)       24 2023-10-26 14:10:20.000000 astro_extras-0.0.6/MANIFEST.in
+-rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-03 12:26:13.623833 astro_extras-0.0.6/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)     7444 2023-11-20 09:59:52.000000 astro_extras-0.0.6/README.md
+-rw-rw-r--   0 kol       (1000) kol       (1000)      352 2023-10-26 14:10:20.000000 astro_extras-0.0.6/pyproject.toml
+-rw-rw-r--   0 kol       (1000) kol       (1000)      260 2024-03-11 13:15:33.000000 astro_extras-0.0.6/requirements.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       38 2024-04-03 12:26:13.623833 astro_extras-0.0.6/setup.cfg
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1109 2024-04-03 12:25:48.000000 astro_extras-0.0.6/setup.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.611833 astro_extras-0.0.6/src/
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.611833 astro_extras-0.0.6/src/astro_extras/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1000 2024-04-03 12:25:54.000000 astro_extras-0.0.6/src/astro_extras/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.619833 astro_extras-0.0.6/src/astro_extras/hooks/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.6/src/astro_extras/hooks/__init__.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.623833 astro_extras-0.0.6/src/astro_extras/operators/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.6/src/astro_extras/operators/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     3880 2023-10-26 14:10:20.000000 astro_extras-0.0.6/src/astro_extras/operators/direct.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    18057 2023-11-20 09:48:16.000000 astro_extras-0.0.6/src/astro_extras/operators/session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    22741 2024-03-11 14:32:23.000000 astro_extras-0.0.6/src/astro_extras/operators/table.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.623833 astro_extras-0.0.6/src/astro_extras/sensors/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2024-04-02 07:09:42.000000 astro_extras-0.0.6/src/astro_extras/sensors/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5530 2024-04-02 07:34:37.000000 astro_extras-0.0.6/src/astro_extras/sensors/file.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.623833 astro_extras-0.0.6/src/astro_extras/utils/
+-rw-rw-r--   0 kol       (1000) kol       (1000)       45 2023-10-26 14:10:20.000000 astro_extras-0.0.6/src/astro_extras/utils/__init__.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)    10549 2023-11-17 15:24:02.000000 astro_extras-0.0.6/src/astro_extras/utils/data_compare.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1675 2024-03-11 13:15:59.000000 astro_extras-0.0.6/src/astro_extras/utils/datetime_local.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5378 2024-03-11 14:28:15.000000 astro_extras-0.0.6/src/astro_extras/utils/template.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1952 2024-03-28 14:14:29.000000 astro_extras-0.0.6/src/astro_extras/utils/utils.py
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.623833 astro_extras-0.0.6/src/astro_extras.egg-info/
+-rw-r--r--   0 kol       (1000) kol       (1000)     7878 2024-04-03 12:26:13.000000 astro_extras-0.0.6/src/astro_extras.egg-info/PKG-INFO
+-rw-rw-r--   0 kol       (1000) kol       (1000)      821 2024-04-03 12:26:13.000000 astro_extras-0.0.6/src/astro_extras.egg-info/SOURCES.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)        1 2024-04-03 12:26:13.000000 astro_extras-0.0.6/src/astro_extras.egg-info/dependency_links.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)      112 2024-04-03 12:26:13.000000 astro_extras-0.0.6/src/astro_extras.egg-info/requires.txt
+-rw-rw-r--   0 kol       (1000) kol       (1000)       13 2024-04-03 12:26:13.000000 astro_extras-0.0.6/src/astro_extras.egg-info/top_level.txt
+drwxrwxr-x   0 kol       (1000) kol       (1000)        0 2024-04-03 12:26:13.623833 astro_extras-0.0.6/tests/
+-rw-rw-r--   0 kol       (1000) kol       (1000)     4172 2023-11-17 09:41:29.000000 astro_extras-0.0.6/tests/test_session.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     6158 2023-11-17 10:36:18.000000 astro_extras-0.0.6/tests/test_table.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     1295 2023-11-17 09:42:18.000000 astro_extras-0.0.6/tests/test_templates.py
+-rw-rw-r--   0 kol       (1000) kol       (1000)     5772 2024-03-11 14:20:58.000000 astro_extras-0.0.6/tests/test_utils.py
```

### Comparing `astro_extras-0.0.5/LICENSE` & `astro_extras-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/PKG-INFO` & `astro_extras-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.5
+Version: 0.0.6
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.0.5/README.md` & `astro_extras-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/setup.py` & `astro_extras-0.0.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.readlines()
 
 setuptools.setup(
     name="astro_extras",
-    version="0.0.5",
+    version="0.0.6",
     author="Kol",
     author_email="skolchin@gmail.com",
     description="Additional Astro SDK operators",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/skolchin/astro-extras",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Framework :: Apache Airflow",
         "Framework :: Apache Airflow :: Provider",
     ],
     package_dir={"": "src"},
-    packages=['astro_extras', 'astro_extras.hooks', 'astro_extras.operators', 'astro_extras.utils'],
+    packages=['astro_extras', 'astro_extras.hooks', 'astro_extras.operators', 'astro_extras.sensors', 'astro_extras.utils'],
     python_requires=">=3.10",
     install_requires=requirements,
     setup_requires=['setuptools', 'wheel'],
 )
```

### Comparing `astro_extras-0.0.5/src/astro_extras/__init__.py` & `astro_extras-0.0.6/src/astro_extras/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Astro SDK Extras project
 # (c) kol, 2023-2024
 
-__version__ = '0.0.5'
+__version__ = '0.0.6'
 
 from .operators.session import (
     open_session, 
     close_session,
     ETLSession,
     get_current_session,
     get_session_period,
```

### Comparing `astro_extras-0.0.5/src/astro_extras/operators/direct.py` & `astro_extras-0.0.6/src/astro_extras/operators/direct.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/src/astro_extras/operators/session.py` & `astro_extras-0.0.6/src/astro_extras/operators/session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/src/astro_extras/operators/table.py` & `astro_extras-0.0.6/src/astro_extras/operators/table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/src/astro_extras/utils/data_compare.py` & `astro_extras-0.0.6/src/astro_extras/utils/data_compare.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/src/astro_extras/utils/datetime_local.py` & `astro_extras-0.0.6/src/astro_extras/utils/datetime_local.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/src/astro_extras/utils/template.py` & `astro_extras-0.0.6/src/astro_extras/utils/template.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/src/astro_extras/utils/utils.py` & `astro_extras-0.0.6/src/astro_extras/utils/utils.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/src/astro_extras.egg-info/PKG-INFO` & `astro_extras-0.0.6/src/astro_extras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro_extras
-Version: 0.0.5
+Version: 0.0.6
 Summary: Additional Astro SDK operators
 Home-page: https://github.com/skolchin/astro-extras
 Author: Kol
 Author-email: skolchin@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Apache Airflow
```

### Comparing `astro_extras-0.0.5/src/astro_extras.egg-info/SOURCES.txt` & `astro_extras-0.0.6/src/astro_extras.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 src/astro_extras.egg-info/requires.txt
 src/astro_extras.egg-info/top_level.txt
 src/astro_extras/hooks/__init__.py
 src/astro_extras/operators/__init__.py
 src/astro_extras/operators/direct.py
 src/astro_extras/operators/session.py
 src/astro_extras/operators/table.py
+src/astro_extras/sensors/__init__.py
+src/astro_extras/sensors/file.py
 src/astro_extras/utils/__init__.py
 src/astro_extras/utils/data_compare.py
 src/astro_extras/utils/datetime_local.py
 src/astro_extras/utils/template.py
 src/astro_extras/utils/utils.py
 tests/test_session.py
 tests/test_table.py
```

### Comparing `astro_extras-0.0.5/tests/test_session.py` & `astro_extras-0.0.6/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/tests/test_table.py` & `astro_extras-0.0.6/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/tests/test_templates.py` & `astro_extras-0.0.6/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `astro_extras-0.0.5/tests/test_utils.py` & `astro_extras-0.0.6/tests/test_utils.py`

 * *Files identical despite different names*

