# Comparing `tmp/froggius-0.1.4.post1.tar.gz` & `tmp/froggius-0.1.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froggius-0.1.4.post1.tar", last modified: Mon Apr  1 15:15:42 2024, max compression
+gzip compressed data, was "froggius-0.1.4.post2.tar", last modified: Tue Apr  2 14:07:42 2024, max compression
```

## Comparing `froggius-0.1.4.post1.tar` & `froggius-0.1.4.post2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-01 15:15:36.000000 froggius-0.1.4.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4430 2024-04-01 15:15:36.000000 froggius-0.1.4.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/froggius/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 15:15:36.000000 froggius-0.1.4.post1/froggius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-01 15:15:39.000000 froggius-0.1.4.post1/froggius/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/froggius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-01 15:15:42.000000 froggius-0.1.4.post1/froggius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-01 15:15:42.000000 froggius-0.1.4.post1/froggius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 15:15:42.000000 froggius-0.1.4.post1/froggius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-01 15:15:42.000000 froggius-0.1.4.post1/froggius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 15:15:42.198522 froggius-0.1.4.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-01 15:15:39.000000 froggius-0.1.4.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-02 14:07:30.000000 froggius-0.1.4.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-02 14:07:30.000000 froggius-0.1.4.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/froggius/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 14:07:39.000000 froggius-0.1.4.post2/froggius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-02 14:07:39.000000 froggius-0.1.4.post2/froggius/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/froggius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-02 14:07:42.000000 froggius-0.1.4.post2/froggius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 14:07:42.000000 froggius-0.1.4.post2/froggius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:07:42.000000 froggius-0.1.4.post2/froggius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 14:07:42.000000 froggius-0.1.4.post2/froggius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 14:07:39.000000 froggius-0.1.4.post2/setup.py
```

### Comparing `froggius-0.1.4.post1/LICENSE` & `froggius-0.1.4.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `froggius-0.1.4.post1/PKG-INFO` & `froggius-0.1.4.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.4.post1
+Version: 0.1.4.post2
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
@@ -47,15 +47,15 @@
 pip install .
 ```
 
 ## Usage
 Here are examples for the usage of Froggius. Import statement is following:
 
 ```py
-from froggius.logger import Froggius
+from froggius import Froggius
 ```
 
 ### Using debugger/logger
 Use it as debugger/logger with following possible arguments:
 - log_msg (log message)
 - file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
 - print_out (True by default, used to setup printing to console and stdout)
```

### Comparing `froggius-0.1.4.post1/README.md` & `froggius-0.1.4.post2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 pip install .
 ```
 
 ## Usage
 Here are examples for the usage of Froggius. Import statement is following:
 
 ```py
-from froggius.logger import Froggius
+from froggius import Froggius
 ```
 
 ### Using debugger/logger
 Use it as debugger/logger with following possible arguments:
 - log_msg (log message)
 - file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
 - print_out (True by default, used to setup printing to console and stdout)
```

### Comparing `froggius-0.1.4.post1/froggius/logger.py` & `froggius-0.1.4.post2/froggius/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,14 +147,26 @@
                     f'\n[INF] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
                 )
 
         if print_out == True:
             print(log_string, file=sys.stdout)
 
     def warning(log_msg, file_path=None, highlighting=True, print_out=True):
+        """
+        Logs a warning message with an optional file path, highlighting, and print out.
+
+        Parameters:
+            log_msg (str): The warning message to be logged.
+            file_path (str, optional): The file path to write the log message to. Defaults to None.
+            highlighting (bool, optional): Whether to highlight the log message. Defaults to True.
+            print_out (bool, optional): Whether to print the log message to the console. Defaults to True.
+
+        Returns:
+            None
+        """
         current_date = datetime.datetime.now()
 
         if highlighting:
             log_string = f'[\033[93mWRN\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
         else:
             log_string = (
                 f'[WRN] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
```

### Comparing `froggius-0.1.4.post1/froggius.egg-info/PKG-INFO` & `froggius-0.1.4.post2/froggius.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.4.post1
+Version: 0.1.4.post2
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
@@ -47,15 +47,15 @@
 pip install .
 ```
 
 ## Usage
 Here are examples for the usage of Froggius. Import statement is following:
 
 ```py
-from froggius.logger import Froggius
+from froggius import Froggius
 ```
 
 ### Using debugger/logger
 Use it as debugger/logger with following possible arguments:
 - log_msg (log message)
 - file_path (None by default, used to set up a log file [...] to append to this file. The file does not have to already exist, if it does not exist, it will be created)
 - print_out (True by default, used to setup printing to console and stdout)
```

### Comparing `froggius-0.1.4.post1/setup.py` & `froggius-0.1.4.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 setup(
     name="froggius",
     packages=find_packages(include=["froggius"]),
     description="Froggius is a dumb easy logging tool for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MPL-2.0",
-    version="0.1.4-1",
+    version="0.1.4-2",
     author="zlElo",
     author_email="mail@zlelo.de",
     url="https://github.com/zlElo/Froggius",
     keywords=["logging", "logger", "easy-to-use", "log"],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

