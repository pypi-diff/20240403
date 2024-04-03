# Comparing `tmp/python-bridge-0.0.2.tar.gz` & `tmp/python-bridge-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bridge-0.0.2.tar", last modified: Wed Apr  3 01:09:02 2024, max compression
+gzip compressed data, was "python-bridge-0.0.3.tar", last modified: Wed Apr  3 01:14:51 2024, max compression
```

## Comparing `python-bridge-0.0.2.tar` & `python-bridge-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.203678 python-bridge-0.0.2/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.2/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1307 2024-04-03 01:09:02.203445 python-bridge-0.0.2/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.2/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.199541 python-bridge-0.0.2/bridge/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.2/bridge/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.199933 python-bridge-0.0.2/bridge/cli/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.2/bridge/cli/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3108 2024-04-02 22:25:52.000000 python-bridge-0.0.2/bridge/cli/bridge.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.200556 python-bridge-0.0.2/bridge/cli/deploy/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.2/bridge/cli/deploy/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2221 2024-04-02 22:47:43.000000 python-bridge-0.0.2/bridge/cli/deploy/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.2/bridge/cli/deploy/django.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      843 2024-04-02 22:55:44.000000 python-bridge-0.0.2/bridge/console.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.201326 python-bridge-0.0.2/bridge/framework/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.2/bridge/framework/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.2/bridge/framework/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1157 2024-04-03 00:33:01.000000 python-bridge-0.0.2/bridge/framework/django.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.202035 python-bridge-0.0.2/bridge/service/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.2/bridge/service/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2552 2024-04-02 22:52:20.000000 python-bridge-0.0.2/bridge/service/docker.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1893 2024-04-02 22:52:42.000000 python-bridge-0.0.2/bridge/service/postgres.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1486 2024-04-03 01:08:54.000000 python-bridge-0.0.2/pyproject.toml
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.203164 python-bridge-0.0.2/python_bridge.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1307 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/entry_points.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       95 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 01:09:02.203728 python-bridge-0.0.2/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.281896 python-bridge-0.0.3/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.3/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 01:14:51.281658 python-bridge-0.0.3/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.3/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.276930 python-bridge-0.0.3/bridge/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.3/bridge/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.277287 python-bridge-0.0.3/bridge/cli/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.3/bridge/cli/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3108 2024-04-02 22:25:52.000000 python-bridge-0.0.3/bridge/cli/bridge.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.277962 python-bridge-0.0.3/bridge/cli/deploy/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.3/bridge/cli/deploy/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2221 2024-04-02 22:47:43.000000 python-bridge-0.0.3/bridge/cli/deploy/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.3/bridge/cli/deploy/django.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      843 2024-04-02 22:55:44.000000 python-bridge-0.0.3/bridge/console.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.278982 python-bridge-0.0.3/bridge/framework/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.3/bridge/framework/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.3/bridge/framework/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1157 2024-04-03 00:33:01.000000 python-bridge-0.0.3/bridge/framework/django.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.280092 python-bridge-0.0.3/bridge/service/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.3/bridge/service/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2552 2024-04-02 22:52:20.000000 python-bridge-0.0.3/bridge/service/docker.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1893 2024-04-02 22:52:42.000000 python-bridge-0.0.3/bridge/service/postgres.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 01:14:41.000000 python-bridge-0.0.3/pyproject.toml
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:14:51.281371 python-bridge-0.0.3/python_bridge.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 01:14:51.000000 python-bridge-0.0.3/python_bridge.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 01:14:51.281955 python-bridge-0.0.3/setup.cfg
```

### Comparing `python-bridge-0.0.2/LICENSE` & `python-bridge-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/PKG-INFO` & `python-bridge-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,13 +18,13 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docker==7.0.0
-Requires-Dist: psycopg-binary==3.1.18
+Requires-Dist: psycopg[binary]==3.1.18
 Requires-Dist: rich==13.7.1
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: google-cloud-storage==2.16.0
 
 # bridge
```

### Comparing `python-bridge-0.0.2/bridge/cli/bridge.py` & `python-bridge-0.0.3/bridge/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/bridge/cli/deploy/base.py` & `python-bridge-0.0.3/bridge/cli/deploy/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/bridge/cli/deploy/django.py` & `python-bridge-0.0.3/bridge/cli/deploy/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/bridge/console.py` & `python-bridge-0.0.3/bridge/console.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/bridge/framework/base.py` & `python-bridge-0.0.3/bridge/framework/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/bridge/framework/django.py` & `python-bridge-0.0.3/bridge/framework/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/bridge/service/docker.py` & `python-bridge-0.0.3/bridge/service/docker.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/bridge/service/postgres.py` & `python-bridge-0.0.3/bridge/service/postgres.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.2/pyproject.toml` & `python-bridge-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-bridge"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to abstract your Django infrastructure."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -21,15 +21,15 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3 :: Only",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 keywords = ['python', 'deployment', 'local', 'infrastructure', 'postgres', 'django', 'architecture']
 dependencies = [
     "docker==7.0.0",
-    "psycopg-binary==3.1.18",
+    "psycopg[binary]==3.1.18",
     "rich==13.7.1",
     "pydantic==2.6.4",
     "google-cloud-storage==2.16.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/never-over/bridge"
```

### Comparing `python-bridge-0.0.2/python_bridge.egg-info/PKG-INFO` & `python-bridge-0.0.3/python_bridge.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -18,13 +18,13 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: docker==7.0.0
-Requires-Dist: psycopg-binary==3.1.18
+Requires-Dist: psycopg[binary]==3.1.18
 Requires-Dist: rich==13.7.1
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: google-cloud-storage==2.16.0
 
 # bridge
```

### Comparing `python-bridge-0.0.2/python_bridge.egg-info/SOURCES.txt` & `python-bridge-0.0.3/python_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

