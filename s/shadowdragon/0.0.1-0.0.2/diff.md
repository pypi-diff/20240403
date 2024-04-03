# Comparing `tmp/shadowdragon-0.0.1.tar.gz` & `tmp/shadowdragon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shadowdragon-0.0.1.tar", last modified: Wed Apr  3 19:39:07 2024, max compression
+gzip compressed data, was "shadowdragon-0.0.2.tar", last modified: Wed Apr  3 19:47:50 2024, max compression
```

## Comparing `shadowdragon-0.0.1.tar` & `shadowdragon-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:39:07.892866 shadowdragon-0.0.1/
--rw-r--r--   0 kojinglick   (501) staff       (20)     1067 2024-04-03 19:25:27.000000 shadowdragon-0.0.1/LICENSE
--rw-r--r--   0 kojinglick   (501) staff       (20)      586 2024-04-03 19:39:07.892062 shadowdragon-0.0.1/PKG-INFO
--rw-r--r--   0 kojinglick   (501) staff       (20)       49 2024-03-28 16:44:23.000000 shadowdragon-0.0.1/README.md
--rw-r--r--   0 kojinglick   (501) staff       (20)      518 2024-04-03 19:37:52.000000 shadowdragon-0.0.1/pyproject.toml
--rw-r--r--   0 kojinglick   (501) staff       (20)       38 2024-04-03 19:39:07.893047 shadowdragon-0.0.1/setup.cfg
-drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:39:07.884673 shadowdragon-0.0.1/src/
-drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:39:07.888373 shadowdragon-0.0.1/src/shadowdragon/
--rw-r--r--   0 kojinglick   (501) staff       (20)       40 2024-04-03 19:18:10.000000 shadowdragon-0.0.1/src/shadowdragon/__init__.py
--rw-r--r--   0 kojinglick   (501) staff       (20)     4328 2024-03-21 18:56:17.000000 shadowdragon-0.0.1/src/shadowdragon/archive.py
--rw-r--r--   0 kojinglick   (501) staff       (20)    20927 2024-04-02 21:42:55.000000 shadowdragon-0.0.1/src/shadowdragon/shadowdragon.py
-drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:39:07.891406 shadowdragon-0.0.1/src/shadowdragon.egg-info/
--rw-r--r--   0 kojinglick   (501) staff       (20)      586 2024-04-03 19:39:07.000000 shadowdragon-0.0.1/src/shadowdragon.egg-info/PKG-INFO
--rw-r--r--   0 kojinglick   (501) staff       (20)      282 2024-04-03 19:39:07.000000 shadowdragon-0.0.1/src/shadowdragon.egg-info/SOURCES.txt
--rw-r--r--   0 kojinglick   (501) staff       (20)        1 2024-04-03 19:39:07.000000 shadowdragon-0.0.1/src/shadowdragon.egg-info/dependency_links.txt
--rw-r--r--   0 kojinglick   (501) staff       (20)       13 2024-04-03 19:39:07.000000 shadowdragon-0.0.1/src/shadowdragon.egg-info/top_level.txt
+drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:47:50.442108 shadowdragon-0.0.2/
+-rw-r--r--   0 kojinglick   (501) staff       (20)     1067 2024-04-03 19:25:27.000000 shadowdragon-0.0.2/LICENSE
+-rw-r--r--   0 kojinglick   (501) staff       (20)      586 2024-04-03 19:47:50.441505 shadowdragon-0.0.2/PKG-INFO
+-rw-r--r--   0 kojinglick   (501) staff       (20)       49 2024-03-28 16:44:23.000000 shadowdragon-0.0.2/README.md
+-rw-r--r--   0 kojinglick   (501) staff       (20)      518 2024-04-03 19:47:45.000000 shadowdragon-0.0.2/pyproject.toml
+-rw-r--r--   0 kojinglick   (501) staff       (20)       38 2024-04-03 19:47:50.442232 shadowdragon-0.0.2/setup.cfg
+drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:47:50.435011 shadowdragon-0.0.2/src/
+drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:47:50.438082 shadowdragon-0.0.2/src/shadowdragon/
+-rw-r--r--   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:46:14.000000 shadowdragon-0.0.2/src/shadowdragon/__init__.py
+-rw-r--r--   0 kojinglick   (501) staff       (20)     4328 2024-03-21 18:56:17.000000 shadowdragon-0.0.2/src/shadowdragon/archive.py
+-rw-r--r--   0 kojinglick   (501) staff       (20)    20927 2024-04-02 21:42:55.000000 shadowdragon-0.0.2/src/shadowdragon/shadowdragon.py
+drwxr-xr-x   0 kojinglick   (501) staff       (20)        0 2024-04-03 19:47:50.440892 shadowdragon-0.0.2/src/shadowdragon.egg-info/
+-rw-r--r--   0 kojinglick   (501) staff       (20)      586 2024-04-03 19:47:50.000000 shadowdragon-0.0.2/src/shadowdragon.egg-info/PKG-INFO
+-rw-r--r--   0 kojinglick   (501) staff       (20)      282 2024-04-03 19:47:50.000000 shadowdragon-0.0.2/src/shadowdragon.egg-info/SOURCES.txt
+-rw-r--r--   0 kojinglick   (501) staff       (20)        1 2024-04-03 19:47:50.000000 shadowdragon-0.0.2/src/shadowdragon.egg-info/dependency_links.txt
+-rw-r--r--   0 kojinglick   (501) staff       (20)       13 2024-04-03 19:47:50.000000 shadowdragon-0.0.2/src/shadowdragon.egg-info/top_level.txt
```

### Comparing `shadowdragon-0.0.1/LICENSE` & `shadowdragon-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shadowdragon-0.0.1/PKG-INFO` & `shadowdragon-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowdragon
-Version: 0.0.1
+Version: 0.0.2
 Summary: An async wrapper for the ShadowDragon API
 Author-email: Kojin Glick <kglick@middlebury.edu>
 Project-URL: Homepage, https://github.com/kojinglick-ctec/shadowdragon/
 Project-URL: Issues, https://github.com/kojinglick-ctec/shadowdragon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `shadowdragon-0.0.1/pyproject.toml` & `shadowdragon-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shadowdragon"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Kojin Glick", email="kglick@middlebury.edu" },
 ]
 description = "An async wrapper for the ShadowDragon API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `shadowdragon-0.0.1/src/shadowdragon/archive.py` & `shadowdragon-0.0.2/src/shadowdragon/archive.py`

 * *Files identical despite different names*

### Comparing `shadowdragon-0.0.1/src/shadowdragon/shadowdragon.py` & `shadowdragon-0.0.2/src/shadowdragon/shadowdragon.py`

 * *Files identical despite different names*

### Comparing `shadowdragon-0.0.1/src/shadowdragon.egg-info/PKG-INFO` & `shadowdragon-0.0.2/src/shadowdragon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shadowdragon
-Version: 0.0.1
+Version: 0.0.2
 Summary: An async wrapper for the ShadowDragon API
 Author-email: Kojin Glick <kglick@middlebury.edu>
 Project-URL: Homepage, https://github.com/kojinglick-ctec/shadowdragon/
 Project-URL: Issues, https://github.com/kojinglick-ctec/shadowdragon/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

