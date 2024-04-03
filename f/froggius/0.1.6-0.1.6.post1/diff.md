# Comparing `tmp/froggius-0.1.6.tar.gz` & `tmp/froggius-0.1.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froggius-0.1.6.tar", last modified: Wed Apr  3 14:22:36 2024, max compression
+gzip compressed data, was "froggius-0.1.6.post1.tar", last modified: Wed Apr  3 14:32:24 2024, max compression
```

## Comparing `froggius-0.1.6.tar` & `froggius-0.1.6.post1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:22:36.026121 froggius-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-03 14:22:27.000000 froggius-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-03 14:22:36.026121 froggius-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-03 14:22:27.000000 froggius-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:22:36.022121 froggius-0.1.6/froggius/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 14:22:33.000000 froggius-0.1.6/froggius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8759 2024-04-03 14:22:33.000000 froggius-0.1.6/froggius/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:22:36.026121 froggius-0.1.6/froggius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-03 14:22:36.000000 froggius-0.1.6/froggius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 14:22:36.000000 froggius-0.1.6/froggius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:22:36.000000 froggius-0.1.6/froggius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 14:22:36.000000 froggius-0.1.6/froggius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:22:36.026121 froggius-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 14:22:33.000000 froggius-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:32:24.136570 froggius-0.1.6.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-03 14:32:17.000000 froggius-0.1.6.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-03 14:32:24.136570 froggius-0.1.6.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-04-03 14:32:17.000000 froggius-0.1.6.post1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:32:24.132570 froggius-0.1.6.post1/froggius/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 14:32:21.000000 froggius-0.1.6.post1/froggius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-04-03 14:32:21.000000 froggius-0.1.6.post1/froggius/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:32:24.136570 froggius-0.1.6.post1/froggius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-04-03 14:32:24.000000 froggius-0.1.6.post1/froggius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 14:32:24.000000 froggius-0.1.6.post1/froggius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:32:24.000000 froggius-0.1.6.post1/froggius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 14:32:24.000000 froggius-0.1.6.post1/froggius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:32:24.136570 froggius-0.1.6.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-03 14:32:21.000000 froggius-0.1.6.post1/setup.py
```

### Comparing `froggius-0.1.6/LICENSE` & `froggius-0.1.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `froggius-0.1.6/PKG-INFO` & `froggius-0.1.6.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.6
+Version: 0.1.6.post1
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
```

### Comparing `froggius-0.1.6/README.md` & `froggius-0.1.6.post1/README.md`

 * *Files identical despite different names*

### Comparing `froggius-0.1.6/froggius/logger.py` & `froggius-0.1.6.post1/froggius/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                 print(log_string, file=sys.stderr)
         if print_out and not self.glob_print_out:
             print(log_string, file=sys.stderr)
         if self.glob_print_out is None and print_out is None:
             print(log_string, file=sys.stderr)
 
     @staticmethod
-    def catch(self, file_path=None, continue_onexpception=True):
+    def catch(file_path=None, continue_onexpception=True):
         """
         A decorator that catches exceptions and logs them with LogMx.error
 
         Parameters
         ----------
         file_path : str, optional
         contiune_onexpception : bool, optional
@@ -133,15 +133,16 @@
                 except Exception as e:
                     _, _, tb = sys.exc_info()
                     traceback_info = traceback.extract_tb(tb)
                     line = traceback_info[-1][1]
                     file = traceback_info[-1][0]
                     function_name = traceback_info[-1][2]
 
-                    self.error(
+                    errorinstance = Froggius()
+                    errorinstance.error(
                         log_msg=str(e),
                         highlighting=True,
                         print_out=True,
                         line=[line, file, function_name],
                         file_path=file_path,
                     )
```

### Comparing `froggius-0.1.6/froggius.egg-info/PKG-INFO` & `froggius-0.1.6.post1/froggius.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.6
+Version: 0.1.6.post1
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
```

### Comparing `froggius-0.1.6/setup.py` & `froggius-0.1.6.post1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="froggius",
     packages=find_packages(include=["froggius"]),
     description="Froggius is a dumb easy logging tool for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MPL-2.0",
-    version="0.1.6",
+    version="0.1.6-1",
     author="zlElo",
     author_email="mail@zlelo.de",
     url="https://github.com/zlElo/Froggius",
     keywords=["logging", "logger", "easy-to-use", "log"],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

