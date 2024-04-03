# Comparing `tmp/loggingpython-1.3.1.tar.gz` & `tmp/loggingpython-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggingpython-1.3.1.tar", last modified: Sun Mar 31 20:10:24 2024, max compression
+gzip compressed data, was "loggingpython-1.3.2.tar", last modified: Wed Apr  3 16:30:17 2024, max compression
```

## Comparing `loggingpython-1.3.1.tar` & `loggingpython-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-03-31 20:10:24.135865 loggingpython-1.3.1/
--rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     3915 2024-03-31 20:10:24.134364 loggingpython-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     2947 2024-03-30 16:13:58.000000 loggingpython-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-03-31 20:10:24.135865 loggingpython-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1324 2024-03-31 20:10:19.000000 loggingpython-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-31 20:10:24.100364 loggingpython-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-31 20:10:24.106865 loggingpython-1.3.1/src/loggingpython/
--rw-rw-rw-   0        0        0     2967 2024-03-30 14:30:52.000000 loggingpython-1.3.1/src/loggingpython/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-31 20:10:24.130364 loggingpython-1.3.1/src/loggingpython/handler/
--rw-rw-rw-   0        0        0      779 2024-03-21 14:56:59.000000 loggingpython-1.3.1/src/loggingpython/handler/__init__.py
--rw-rw-rw-   0        0        0     4599 2024-03-20 16:50:39.000000 loggingpython-1.3.1/src/loggingpython/handler/consolehandler.py
--rw-rw-rw-   0        0        0     3969 2024-03-20 16:50:02.000000 loggingpython-1.3.1/src/loggingpython/handler/csvhandler.py
--rw-rw-rw-   0        0        0     3840 2024-03-20 16:50:27.000000 loggingpython-1.3.1/src/loggingpython/handler/filehandler.py
--rw-rw-rw-   0        0        0     1002 2024-03-30 14:31:02.000000 loggingpython-1.3.1/src/loggingpython/handler/handler.py
--rw-rw-rw-   0        0        0     5010 2024-03-20 16:50:13.000000 loggingpython-1.3.1/src/loggingpython/handler/jsonhandler.py
--rw-rw-rw-   0        0        0     5044 2024-03-20 16:50:07.000000 loggingpython-1.3.1/src/loggingpython/handler/sqlhandler.py
--rw-rw-rw-   0        0        0     1474 2024-03-30 14:31:08.000000 loggingpython-1.3.1/src/loggingpython/handler/syshandler.py
--rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.3.1/src/loggingpython/log_levels.py
--rw-rw-rw-   0        0        0     6961 2024-03-21 14:52:36.000000 loggingpython-1.3.1/src/loggingpython/logger.py
-drwxrwxrwx   0        0        0        0 2024-03-31 20:10:24.132865 loggingpython-1.3.1/src/loggingpython.egg-info/
--rw-rw-rw-   0        0        0     3915 2024-03-31 20:10:24.000000 loggingpython-1.3.1/src/loggingpython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      689 2024-03-31 20:10:24.000000 loggingpython-1.3.1/src/loggingpython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-31 20:10:24.000000 loggingpython-1.3.1/src/loggingpython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-03-31 20:10:24.000000 loggingpython-1.3.1/src/loggingpython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-31 20:10:24.000000 loggingpython-1.3.1/src/loggingpython.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-31 20:10:24.131864 loggingpython-1.3.1/test/
--rw-rw-rw-   0        0        0     1477 2024-03-20 16:50:32.000000 loggingpython-1.3.1/test/test_consolehandler.py
--rw-rw-rw-   0        0        0     1082 2024-03-20 16:50:17.000000 loggingpython-1.3.1/test/test_logger.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:30:17.286197 loggingpython-1.3.2/
+-rw-rw-rw-   0        0        0     1087 2024-03-04 14:25:44.000000 loggingpython-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3859 2024-04-03 16:30:17.285197 loggingpython-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2947 2024-03-30 16:13:58.000000 loggingpython-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 16:30:17.286197 loggingpython-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1269 2024-04-03 16:30:09.000000 loggingpython-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:30:17.247698 loggingpython-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 16:30:17.256196 loggingpython-1.3.2/src/loggingpython/
+-rw-rw-rw-   0        0        0     2967 2024-04-03 16:30:14.000000 loggingpython-1.3.2/src/loggingpython/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:30:17.281696 loggingpython-1.3.2/src/loggingpython/handler/
+-rw-rw-rw-   0        0        0      779 2024-03-21 14:56:59.000000 loggingpython-1.3.2/src/loggingpython/handler/__init__.py
+-rw-rw-rw-   0        0        0     4599 2024-03-20 16:50:39.000000 loggingpython-1.3.2/src/loggingpython/handler/consolehandler.py
+-rw-rw-rw-   0        0        0     3969 2024-03-20 16:50:02.000000 loggingpython-1.3.2/src/loggingpython/handler/csvhandler.py
+-rw-rw-rw-   0        0        0     3840 2024-03-20 16:50:27.000000 loggingpython-1.3.2/src/loggingpython/handler/filehandler.py
+-rw-rw-rw-   0        0        0     1002 2024-03-30 14:31:02.000000 loggingpython-1.3.2/src/loggingpython/handler/handler.py
+-rw-rw-rw-   0        0        0     5010 2024-03-20 16:50:13.000000 loggingpython-1.3.2/src/loggingpython/handler/jsonhandler.py
+-rw-rw-rw-   0        0        0     5044 2024-03-20 16:50:07.000000 loggingpython-1.3.2/src/loggingpython/handler/sqlhandler.py
+-rw-rw-rw-   0        0        0     4709 2024-04-03 16:28:06.000000 loggingpython-1.3.2/src/loggingpython/handler/syshandler.py
+-rw-rw-rw-   0        0        0      163 2024-03-04 14:56:48.000000 loggingpython-1.3.2/src/loggingpython/log_levels.py
+-rw-rw-rw-   0        0        0     7444 2024-04-03 14:00:41.000000 loggingpython-1.3.2/src/loggingpython/logger.py
+-rw-rw-rw-   0        0        0      129 2024-04-03 16:16:15.000000 loggingpython-1.3.2/src/loggingpython/sys_procolls.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:30:17.284197 loggingpython-1.3.2/src/loggingpython.egg-info/
+-rw-rw-rw-   0        0        0     3859 2024-04-03 16:30:17.000000 loggingpython-1.3.2/src/loggingpython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2024-04-03 16:30:17.000000 loggingpython-1.3.2/src/loggingpython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 16:30:17.000000 loggingpython-1.3.2/src/loggingpython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-03 16:30:17.000000 loggingpython-1.3.2/src/loggingpython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-03 16:30:17.000000 loggingpython-1.3.2/src/loggingpython.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 16:30:17.283197 loggingpython-1.3.2/test/
+-rw-rw-rw-   0        0        0     1477 2024-03-20 16:50:32.000000 loggingpython-1.3.2/test/test_consolehandler.py
+-rw-rw-rw-   0        0        0     1082 2024-03-20 16:50:17.000000 loggingpython-1.3.2/test/test_logger.py
```

### Comparing `loggingpython-1.3.1/LICENSE` & `loggingpython-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/PKG-INFO` & `loggingpython-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.3.1
+Version: 1.3.2
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
```

### Comparing `loggingpython-1.3.1/README.md` & `loggingpython-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/setup.py` & `loggingpython-1.3.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='loggingpython',
-    version='1.3.1',
+    version='1.3.2',
     description='Loggingpython is a Python package that provides a simple and\
  extensible way to integrate logging into your applications. The package\
  starts with a simple logger and can be extended with additional functions to\
  meet the requirements of your application.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='mrmajor.programmer',
@@ -18,15 +18,14 @@
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=['colorama', 'pandas'],
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
-        'Topic :: Software Development :: Libraries',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: System :: Logging',
     ],
     include_package_data=True,
     package_data={
```

### Comparing `loggingpython-1.3.1/src/loggingpython/__init__.py` & `loggingpython-1.3.2/src/loggingpython/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from .handler import Handler
 from .log_levels import LogLevel
 
 
 import importlib
 
 
-__version__ = "1.1.2"
+__version__ = "1.3.2"
 __all__ = ["Logger",
            # Hander
            "Handler",
            "FileHandler",
            "ConsoleHandler",
            "JSONHandler",
            "SQLHandler",
```

### Comparing `loggingpython-1.3.1/src/loggingpython/handler/__init__.py` & `loggingpython-1.3.2/src/loggingpython/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/src/loggingpython/handler/consolehandler.py` & `loggingpython-1.3.2/src/loggingpython/handler/consolehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/src/loggingpython/handler/csvhandler.py` & `loggingpython-1.3.2/src/loggingpython/handler/csvhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/src/loggingpython/handler/filehandler.py` & `loggingpython-1.3.2/src/loggingpython/handler/filehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/src/loggingpython/handler/handler.py` & `loggingpython-1.3.2/src/loggingpython/handler/handler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/src/loggingpython/handler/jsonhandler.py` & `loggingpython-1.3.2/src/loggingpython/handler/jsonhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/src/loggingpython/handler/sqlhandler.py` & `loggingpython-1.3.2/src/loggingpython/handler/sqlhandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/src/loggingpython/logger.py` & `loggingpython-1.3.2/src/loggingpython/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -217,7 +217,19 @@
         Args:
             message (str): The message to log.
 
         Raises:
             ValueError: If the level is not supported.
         """
         self._log(message, loglevel=LogLevel.CRITICAL)
+
+    def catch_debug(self, func):
+        def wrapper(*args, **kwargs):
+            try:
+                self.debug(f"func '{func.__name__}' with {args}, {kwargs}")
+                result = func(*args, **kwargs)
+                self.debug(f"func '{func.__name__}' completed successfully, \
+with '{result}'")
+                return result
+            except Exception as e:
+                self.error(f"{func.__name__} failed with error: {str(e)}")
+        return wrapper
```

### Comparing `loggingpython-1.3.1/src/loggingpython.egg-info/PKG-INFO` & `loggingpython-1.3.2/src/loggingpython.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: loggingpython
-Version: 1.3.1
+Version: 1.3.2
 Summary: Loggingpython is a Python package that provides a simple and extensible way to integrate logging into your applications. The package starts with a simple logger and can be extended with additional functions to meet the requirements of your application.
 Home-page: https://github.com/loggingpython-Community/loggingpython
 Author: mrmajor.programmer
 Author-email: mrmajork.programmer@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Logging
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: colorama
```

### Comparing `loggingpython-1.3.1/src/loggingpython.egg-info/SOURCES.txt` & `loggingpython-1.3.2/src/loggingpython.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 setup.py
 src/loggingpython/__init__.py
 src/loggingpython/log_levels.py
 src/loggingpython/logger.py
+src/loggingpython/sys_procolls.py
 src/loggingpython.egg-info/PKG-INFO
 src/loggingpython.egg-info/SOURCES.txt
 src/loggingpython.egg-info/dependency_links.txt
 src/loggingpython.egg-info/requires.txt
 src/loggingpython.egg-info/top_level.txt
 src/loggingpython/handler/__init__.py
 src/loggingpython/handler/consolehandler.py
```

### Comparing `loggingpython-1.3.1/test/test_consolehandler.py` & `loggingpython-1.3.2/test/test_consolehandler.py`

 * *Files identical despite different names*

### Comparing `loggingpython-1.3.1/test/test_logger.py` & `loggingpython-1.3.2/test/test_logger.py`

 * *Files identical despite different names*

