# Comparing `tmp/python-bridge-0.0.1.tar.gz` & `tmp/python-bridge-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bridge-0.0.1.tar", last modified: Wed Apr  3 01:05:18 2024, max compression
+gzip compressed data, was "python-bridge-0.0.2.tar", last modified: Wed Apr  3 01:09:02 2024, max compression
```

## Comparing `python-bridge-0.0.1.tar` & `python-bridge-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:05:18.690782 python-bridge-0.0.1/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.1/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1307 2024-04-03 01:05:18.690519 python-bridge-0.0.1/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.1/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:05:18.686628 python-bridge-0.0.1/bridge/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.1/bridge/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:05:18.687080 python-bridge-0.0.1/bridge/cli/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.1/bridge/cli/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3108 2024-04-02 22:25:52.000000 python-bridge-0.0.1/bridge/cli/bridge.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:05:18.687761 python-bridge-0.0.1/bridge/cli/deploy/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.1/bridge/cli/deploy/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2221 2024-04-02 22:47:43.000000 python-bridge-0.0.1/bridge/cli/deploy/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.1/bridge/cli/deploy/django.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      843 2024-04-02 22:55:44.000000 python-bridge-0.0.1/bridge/console.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:05:18.688447 python-bridge-0.0.1/bridge/framework/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.1/bridge/framework/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1875 2024-04-03 00:38:00.000000 python-bridge-0.0.1/bridge/framework/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1157 2024-04-03 00:33:01.000000 python-bridge-0.0.1/bridge/framework/django.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:05:18.689004 python-bridge-0.0.1/bridge/service/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.1/bridge/service/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2552 2024-04-02 22:52:20.000000 python-bridge-0.0.1/bridge/service/docker.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1893 2024-04-02 22:52:42.000000 python-bridge-0.0.1/bridge/service/postgres.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1486 2024-04-03 00:55:30.000000 python-bridge-0.0.1/pyproject.toml
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:05:18.690207 python-bridge-0.0.1/python_bridge.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1307 2024-04-03 01:05:18.000000 python-bridge-0.0.1/python_bridge.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 01:05:18.000000 python-bridge-0.0.1/python_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 01:05:18.000000 python-bridge-0.0.1/python_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 01:05:18.000000 python-bridge-0.0.1/python_bridge.egg-info/entry_points.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       95 2024-04-03 01:05:18.000000 python-bridge-0.0.1/python_bridge.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 01:05:18.000000 python-bridge-0.0.1/python_bridge.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 01:05:18.690830 python-bridge-0.0.1/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.203678 python-bridge-0.0.2/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.2/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1307 2024-04-03 01:09:02.203445 python-bridge-0.0.2/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.2/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.199541 python-bridge-0.0.2/bridge/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.2/bridge/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.199933 python-bridge-0.0.2/bridge/cli/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.2/bridge/cli/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3108 2024-04-02 22:25:52.000000 python-bridge-0.0.2/bridge/cli/bridge.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.200556 python-bridge-0.0.2/bridge/cli/deploy/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.2/bridge/cli/deploy/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2221 2024-04-02 22:47:43.000000 python-bridge-0.0.2/bridge/cli/deploy/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1107 2024-04-02 22:57:15.000000 python-bridge-0.0.2/bridge/cli/deploy/django.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      843 2024-04-02 22:55:44.000000 python-bridge-0.0.2/bridge/console.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.201326 python-bridge-0.0.2/bridge/framework/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.2/bridge/framework/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.2/bridge/framework/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1157 2024-04-03 00:33:01.000000 python-bridge-0.0.2/bridge/framework/django.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.202035 python-bridge-0.0.2/bridge/service/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.2/bridge/service/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2552 2024-04-02 22:52:20.000000 python-bridge-0.0.2/bridge/service/docker.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1893 2024-04-02 22:52:42.000000 python-bridge-0.0.2/bridge/service/postgres.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1486 2024-04-03 01:08:54.000000 python-bridge-0.0.2/pyproject.toml
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 01:09:02.203164 python-bridge-0.0.2/python_bridge.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1307 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       95 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 01:09:02.000000 python-bridge-0.0.2/python_bridge.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 01:09:02.203728 python-bridge-0.0.2/setup.cfg
```

### Comparing `python-bridge-0.0.1/LICENSE` & `python-bridge-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.1/PKG-INFO` & `python-bridge-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.1/bridge/cli/bridge.py` & `python-bridge-0.0.2/bridge/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.1/bridge/cli/deploy/base.py` & `python-bridge-0.0.2/bridge/cli/deploy/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.1/bridge/cli/deploy/django.py` & `python-bridge-0.0.2/bridge/cli/deploy/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.1/bridge/console.py` & `python-bridge-0.0.2/bridge/console.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.1/bridge/framework/base.py` & `python-bridge-0.0.2/bridge/framework/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.project_name = project_name
         self.framework_locals = framework_locals
         self.enable_postgres = enable_postgres
 
     def run(self) -> None:
         """Start services."""
         if os.environ.get("IS_BRIDGE_PLATFORM"):
-
+            self.remote()
         else:
             client = docker.from_env()
             if self.enable_postgres:
                 self.start_postgres(client)
 
     def remote(self) -> None:
         """Connect to remote services."""
```

### Comparing `python-bridge-0.0.1/bridge/framework/django.py` & `python-bridge-0.0.2/bridge/framework/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.1/bridge/service/docker.py` & `python-bridge-0.0.2/bridge/service/docker.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.1/bridge/service/postgres.py` & `python-bridge-0.0.2/bridge/service/postgres.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.1/pyproject.toml` & `python-bridge-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-bridge"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to abstract your Django infrastructure."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python-bridge-0.0.1/python_bridge.egg-info/PKG-INFO` & `python-bridge-0.0.2/python_bridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.1/python_bridge.egg-info/SOURCES.txt` & `python-bridge-0.0.2/python_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

