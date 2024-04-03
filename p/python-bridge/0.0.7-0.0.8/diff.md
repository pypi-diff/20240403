# Comparing `tmp/python-bridge-0.0.7.tar.gz` & `tmp/python-bridge-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bridge-0.0.7.tar", last modified: Wed Apr  3 07:29:30 2024, max compression
+gzip compressed data, was "python-bridge-0.0.8.tar", last modified: Wed Apr  3 16:30:13 2024, max compression
```

## Comparing `python-bridge-0.0.7.tar` & `python-bridge-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 07:29:30.006170 python-bridge-0.0.7/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.7/LICENSE
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 07:29:30.005945 python-bridge-0.0.7/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.7/README.md
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 07:29:30.001533 python-bridge-0.0.7/bridge/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.7/bridge/__init__.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 07:29:30.002076 python-bridge-0.0.7/bridge/cli/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.7/bridge/cli/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3055 2024-04-03 01:58:27.000000 python-bridge-0.0.7/bridge/cli/bridge.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 07:29:30.002881 python-bridge-0.0.7/bridge/cli/deploy/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.7/bridge/cli/deploy/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4342 2024-04-03 07:27:17.000000 python-bridge-0.0.7/bridge/cli/deploy/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1086 2024-04-03 05:37:16.000000 python-bridge-0.0.7/bridge/cli/deploy/django.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.7/bridge/console.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 07:29:30.003713 python-bridge-0.0.7/bridge/framework/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.7/bridge/framework/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.7/bridge/framework/base.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1228 2024-04-03 01:58:36.000000 python-bridge-0.0.7/bridge/framework/django.py
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 07:29:30.004383 python-bridge-0.0.7/bridge/service/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.7/bridge/service/__init__.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2572 2024-04-03 01:59:22.000000 python-bridge-0.0.7/bridge/service/docker.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2126 2024-04-03 04:37:20.000000 python-bridge-0.0.7/bridge/service/postgres.py
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 07:29:02.000000 python-bridge-0.0.7/pyproject.toml
-drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 07:29:30.005678 python-bridge-0.0.7/python_bridge.egg-info/
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 07:29:29.000000 python-bridge-0.0.7/python_bridge.egg-info/PKG-INFO
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 07:29:29.000000 python-bridge-0.0.7/python_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 07:29:29.000000 python-bridge-0.0.7/python_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 07:29:29.000000 python-bridge-0.0.7/python_bridge.egg-info/entry_points.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 07:29:29.000000 python-bridge-0.0.7/python_bridge.egg-info/requires.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 07:29:29.000000 python-bridge-0.0.7/python_bridge.egg-info/top_level.txt
--rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 07:29:30.006211 python-bridge-0.0.7/setup.cfg
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.662610 python-bridge-0.0.8/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)    35149 2024-03-26 19:19:35.000000 python-bridge-0.0.8/LICENSE
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 16:30:13.662357 python-bridge-0.0.8/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        8 2024-03-26 19:19:35.000000 python-bridge-0.0.8/README.md
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.657979 python-bridge-0.0.8/bridge/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 00:45:56.000000 python-bridge-0.0.8/bridge/__init__.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.658705 python-bridge-0.0.8/bridge/cli/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-27 22:30:18.000000 python-bridge-0.0.8/bridge/cli/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     3055 2024-04-03 01:58:27.000000 python-bridge-0.0.8/bridge/cli/bridge.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.659525 python-bridge-0.0.8/bridge/cli/deploy/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-04-01 20:56:09.000000 python-bridge-0.0.8/bridge/cli/deploy/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     4342 2024-04-03 07:27:17.000000 python-bridge-0.0.8/bridge/cli/deploy/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1086 2024-04-03 05:37:16.000000 python-bridge-0.0.8/bridge/cli/deploy/django.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      960 2024-04-03 01:27:55.000000 python-bridge-0.0.8/bridge/console.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.660400 python-bridge-0.0.8/bridge/framework/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:48:24.000000 python-bridge-0.0.8/bridge/framework/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1900 2024-04-03 01:07:39.000000 python-bridge-0.0.8/bridge/framework/base.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1362 2024-04-03 16:23:57.000000 python-bridge-0.0.8/bridge/framework/django.py
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.661015 python-bridge-0.0.8/bridge/service/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        0 2024-03-26 19:52:25.000000 python-bridge-0.0.8/bridge/service/__init__.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2572 2024-04-03 01:59:22.000000 python-bridge-0.0.8/bridge/service/docker.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     2126 2024-04-03 04:37:20.000000 python-bridge-0.0.8/bridge/service/postgres.py
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1487 2024-04-03 16:29:43.000000 python-bridge-0.0.8/pyproject.toml
+drwxr-xr-x   0 caeleanbarnes   (501) staff       (20)        0 2024-04-03 16:30:13.662058 python-bridge-0.0.8/python_bridge.egg-info/
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)     1308 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)      581 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        1 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       50 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/entry_points.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       96 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/requires.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)        7 2024-04-03 16:30:13.000000 python-bridge-0.0.8/python_bridge.egg-info/top_level.txt
+-rw-r--r--   0 caeleanbarnes   (501) staff       (20)       38 2024-04-03 16:30:13.662661 python-bridge-0.0.8/setup.cfg
```

### Comparing `python-bridge-0.0.7/LICENSE` & `python-bridge-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.7/PKG-INFO` & `python-bridge-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.7/bridge/cli/bridge.py` & `python-bridge-0.0.8/bridge/cli/bridge.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.7/bridge/cli/deploy/base.py` & `python-bridge-0.0.8/bridge/cli/deploy/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.7/bridge/cli/deploy/django.py` & `python-bridge-0.0.8/bridge/cli/deploy/django.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.7/bridge/console.py` & `python-bridge-0.0.8/bridge/console.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.7/bridge/framework/base.py` & `python-bridge-0.0.8/bridge/framework/base.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.7/bridge/framework/django.py` & `python-bridge-0.0.8/bridge/framework/django.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,16 @@
                 "NAME": environment.POSTGRES_DB,
                 "USER": environment.POSTGRES_USER,
                 "PASSWORD": environment.POSTGRES_PASSWORD,
                 "HOST": environment.POSTGRES_HOST,
                 "PORT": environment.POSTGRES_PORT,
             }
         }
+        if os.environ.get("IS_BRIDGE_PLATFORM"):
+            self.framework_locals["ALLOWED_HOSTS"].append(os.environ["BRIDGE_HOST"])
 
 
 def configure(settings_locals: dict, enable_postgres=True) -> None:
     project_name = os.path.basename(settings_locals["BASE_DIR"])
 
     handler = DjangoHandler(
         project_name=project_name,
```

### Comparing `python-bridge-0.0.7/bridge/service/docker.py` & `python-bridge-0.0.8/bridge/service/docker.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.7/bridge/service/postgres.py` & `python-bridge-0.0.8/bridge/service/postgres.py`

 * *Files identical despite different names*

### Comparing `python-bridge-0.0.7/pyproject.toml` & `python-bridge-0.0.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "python-bridge"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to abstract your Django infrastructure."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `python-bridge-0.0.7/python_bridge.egg-info/PKG-INFO` & `python-bridge-0.0.8/python_bridge.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-bridge
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python tool to abstract your Django infrastructure.
 Author-email: Caelean Barnes <caeleanb@gmail.com>, Evan Doyle <evanmdoyle@gmail.com>
 Project-URL: Homepage, https://github.com/never-over/bridge
 Project-URL: Issues, https://github.com/never-over/bridge/issues
 Keywords: python,deployment,local,infrastructure,postgres,django,architecture
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `python-bridge-0.0.7/python_bridge.egg-info/SOURCES.txt` & `python-bridge-0.0.8/python_bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

