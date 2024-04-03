# Comparing `tmp/froggius-0.1.4.post2.tar.gz` & `tmp/froggius-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "froggius-0.1.4.post2.tar", last modified: Tue Apr  2 14:07:42 2024, max compression
+gzip compressed data, was "froggius-0.1.5.tar", last modified: Wed Apr  3 07:09:48 2024, max compression
```

## Comparing `froggius-0.1.4.post2.tar` & `froggius-0.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/
--rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-02 14:07:30.000000 froggius-0.1.4.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-02 14:07:30.000000 froggius-0.1.4.post2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/froggius/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-02 14:07:39.000000 froggius-0.1.4.post2/froggius/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6760 2024-04-02 14:07:39.000000 froggius-0.1.4.post2/froggius/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/froggius.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4977 2024-04-02 14:07:42.000000 froggius-0.1.4.post2/froggius.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 14:07:42.000000 froggius-0.1.4.post2/froggius.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 14:07:42.000000 froggius-0.1.4.post2/froggius.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 14:07:42.000000 froggius-0.1.4.post2/froggius.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 14:07:42.458803 froggius-0.1.4.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-02 14:07:39.000000 froggius-0.1.4.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:09:48.753090 froggius-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    16726 2024-04-03 07:09:43.000000 froggius-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-03 07:09:48.753090 froggius-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-03 07:09:43.000000 froggius-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:09:48.753090 froggius-0.1.5/froggius/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 07:09:46.000000 froggius-0.1.5/froggius/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8099 2024-04-03 07:09:46.000000 froggius-0.1.5/froggius/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:09:48.753090 froggius-0.1.5/froggius.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-03 07:09:48.000000 froggius-0.1.5/froggius.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 07:09:48.000000 froggius-0.1.5/froggius.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:09:48.000000 froggius-0.1.5/froggius.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 07:09:48.000000 froggius-0.1.5/froggius.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:09:48.753090 froggius-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-03 07:09:46.000000 froggius-0.1.5/setup.py
```

### Comparing `froggius-0.1.4.post2/LICENSE` & `froggius-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `froggius-0.1.4.post2/PKG-INFO` & `froggius-0.1.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,20 @@
-Metadata-Version: 2.1
-Name: froggius
-Version: 0.1.4.post2
-Summary: Froggius is a dumb easy logging tool for python
-Home-page: https://github.com/zlElo/Froggius
-Author: zlElo
-Author-email: mail@zlelo.de
-License: MPL-2.0
-Keywords: logging,logger,easy-to-use,log
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <img src="https://github.com/zlElo/Froggius/blob/main/res/froggius-cropped.png?raw=true" style="width: 200px">
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
 </p>
 
 # Froggius
-Froggius is a dumb easy logging tool for python
+Froggius is a lightweight and dumb easy logging tool for python
 
 ---------
 
 ## Introduction
 Froggius is a lightweight python libary, which is designed for easy to use logging for all your programs. It makes it easy for everybody, but also brings a lot of options to configure it like you need it. An very interesting feature for example is the error catching for functions, which makes it easy to log unexpected errors, warnings etc.
 
 ## Installation
@@ -132,7 +115,30 @@
 example_function()
 ```
 
 Output in log file:
 `
 [ERR] [01/04/2024 09:15:00] division by zero | Occured on line: 28 in /Users/username/path/examples.py, example_function()
 `
+
+### Using global configuration
+If you want to configure the file_path and the print_out for everything, you can do that with following line before all other Froggius statements:
+
+```py
+# configure print_out and file_path for everything
+Froggius(print_out=False, file_path='tests/example.log')
+
+Froggius.debug('Test normal')
+Froggius.error('Test error')
+Froggius.information('Test information')
+```
+
+It's also possible to say, that you want that all is not printed, but this `Froggius.debug('Test normal')` or `Froggius.information('Test information')`. Just work with the available parameters:
+
+```py
+# configure print_out and file_path for everything
+Froggius(print_out=False, file_path='tests/example.log')
+
+Froggius.debug('Test normal', print_out=True) # everything is not printed, but this line is printed
+Froggius.error('Test error')
+Froggius.information('Test information')
+```
```

### Comparing `froggius-0.1.4.post2/README.md` & `froggius-0.1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,37 @@
+Metadata-Version: 2.1
+Name: froggius
+Version: 0.1.5
+Summary: Froggius is a dumb easy logging tool for python
+Home-page: https://github.com/zlElo/Froggius
+Author: zlElo
+Author-email: mail@zlelo.de
+License: MPL-2.0
+Keywords: logging,logger,easy-to-use,log
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <p align="center">
   <img src="https://github.com/zlElo/Froggius/blob/main/res/froggius-cropped.png?raw=true" style="width: 200px">
 </p>
 
 <p align="center">
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
 </p>
 
 # Froggius
-Froggius is a dumb easy logging tool for python
+Froggius is a lightweight and dumb easy logging tool for python
 
 ---------
 
 ## Introduction
 Froggius is a lightweight python libary, which is designed for easy to use logging for all your programs. It makes it easy for everybody, but also brings a lot of options to configure it like you need it. An very interesting feature for example is the error catching for functions, which makes it easy to log unexpected errors, warnings etc.
 
 ## Installation
@@ -115,7 +132,30 @@
 example_function()
 ```
 
 Output in log file:
 `
 [ERR] [01/04/2024 09:15:00] division by zero | Occured on line: 28 in /Users/username/path/examples.py, example_function()
 `
+
+### Using global configuration
+If you want to configure the file_path and the print_out for everything, you can do that with following line before all other Froggius statements:
+
+```py
+# configure print_out and file_path for everything
+Froggius(print_out=False, file_path='tests/example.log')
+
+Froggius.debug('Test normal')
+Froggius.error('Test error')
+Froggius.information('Test information')
+```
+
+It's also possible to say, that you want that all is not printed, but this `Froggius.debug('Test normal')` or `Froggius.information('Test information')`. Just work with the available parameters:
+
+```py
+# configure print_out and file_path for everything
+Froggius(print_out=False, file_path='tests/example.log')
+
+Froggius.debug('Test normal', print_out=True) # everything is not printed, but this line is printed
+Froggius.error('Test error')
+Froggius.information('Test information')
+```
```

### Comparing `froggius-0.1.4.post2/froggius/logger.py` & `froggius-0.1.5/froggius/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,26 @@
 
 class Froggius:
     """
     Main class of Froggius
     Includes logging methods
     """
 
-    def debug(log_msg, file_path=None, print_out=True):
+    def __init__(self, file_path=None, print_out=None) -> None:
+        global glob_file_path, glob_print_out
+        if file_path is not None:
+            glob_file_path = file_path
+        else:
+            glob_file_path = None
+        if print_out is not None:
+            glob_print_out = print_out
+        else:
+            glob_print_out = None
+
+    def debug(log_msg, file_path=None, print_out=None):
         """
         Writes logs, optionally to a file.
 
         Parameters
         ----------
         log_msg : str
             The message to be logged.
@@ -27,25 +38,32 @@
             Whether the DEBUG tag should be highlighted with ANSI escape sequences, by default True
         print_out : bool, optional
             Whether the log should be printed to the stdout, by default True
         """
         current_date = datetime.datetime.now()
         log_string = f'[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
 
-        # check for filepath
+        # check for vars for filepath
+        if glob_file_path is not None:
+            file_path = glob_file_path
+
         if file_path is not None:
             with open(file_path, "a") as log:
                 log.write(
                     f'\n[DBG] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
                 )
 
-        if print_out:
+        if glob_print_out:
+            print(log_string, file=sys.stdout)
+        elif print_out:
+            print(log_string, file=sys.stdout)
+        elif glob_print_out is None and print_out is None:
             print(log_string, file=sys.stdout)
 
-    def error(log_msg, file_path=None, highlighting=True, print_out=True, line=None):
+    def error(log_msg, file_path=None, highlighting=True, print_out=None, line=None):
         """
         Writes errors, optionally to a file.
 
         Parameters
         ----------
         log_msg : str
             The message to be logged.
@@ -60,27 +78,34 @@
             A list containing information about the line where the error occurred,
             by default None. The list should contain [line number, file name,
             function name].
         """
 
         # get datetime
         current_date = datetime.datetime.now()
-        if highlighting == True:
+        if highlighting:
             log_string = f'[\033[91mERR\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
         else:
             log_string = f'[ERR] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
 
         # check for filepath
+        if glob_file_path is not None:
+            file_path = glob_file_path
+
         if file_path is not None:
             with open(file_path, "a") as log:
                 log.write(
                     f'\n[ERR] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg} {f"| Occured on line: {line[0]} in {line[1]}, {line[2]}()" if line is not None else ""}'
                 )
 
-        if print_out == True:
+        if glob_print_out:
+            print(log_string, file=sys.stderr)
+        elif print_out:
+            print(log_string, file=sys.stderr)
+        elif glob_print_out is None and print_out is None:
             print(log_string, file=sys.stderr)
 
     @staticmethod
     def catch(file_path=None, continue_onexpception=True):
         """
         A decorator that catches exceptions and logs them with LogMx.error
 
@@ -116,15 +141,15 @@
                     if not continue_onexpception:
                         raise e
 
             return wrapper
 
         return decorator
 
-    def information(log_msg, file_path=None, highlighting=True, print_out=True):
+    def information(log_msg, file_path=None, highlighting=True, print_out=None):
         """
         A function to log information with optional file output and highlighting.
 
         Parameters:
             log_msg (str): The message to be logged.
             file_path (str, optional): The file path to log to. Defaults to None.
             highlighting (bool, optional): Whether to highlight the log message. Defaults to True.
@@ -137,47 +162,58 @@
             log_string = f'[\033[32mINF\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
         else:
             log_string = (
                 f'[INF] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
             )
 
         # check for filepath
+        if glob_file_path is not None:
+            file_path = glob_file_path
+
         if file_path is not None:
             with open(file_path, "a") as log:
                 log.write(
                     f'\n[INF] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
                 )
 
-        if print_out == True:
+        if glob_print_out:
+            print(log_string, file=sys.stdout)
+        elif print_out:
+            print(log_string, file=sys.stdout)
+        elif glob_print_out is None and print_out is None:
             print(log_string, file=sys.stdout)
 
-    def warning(log_msg, file_path=None, highlighting=True, print_out=True):
+    def warning(log_msg, file_path=None, highlighting=True, print_out=None):
         """
         Logs a warning message with an optional file path, highlighting, and print out.
 
         Parameters:
             log_msg (str): The warning message to be logged.
             file_path (str, optional): The file path to write the log message to. Defaults to None.
             highlighting (bool, optional): Whether to highlight the log message. Defaults to True.
             print_out (bool, optional): Whether to print the log message to the console. Defaults to True.
-
-        Returns:
-            None
         """
         current_date = datetime.datetime.now()
 
         if highlighting:
             log_string = f'[\033[93mWRN\033[0m] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
         else:
             log_string = (
                 f'[WRN] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
             )
 
         # check for filepath
+        if glob_file_path is not None:
+            file_path = glob_file_path
+
         if file_path is not None:
             with open(file_path, "a") as log:
                 log.write(
                     f'\n[WRN] [{current_date.strftime("%d/%m/%Y %H:%M:%S")}] {log_msg}'
                 )
 
-        if print_out == True:
+        if glob_print_out:
+            print(log_string, file=sys.stdout)
+        elif print_out:
+            print(log_string, file=sys.stdout)
+        elif glob_print_out is None and print_out is None:
             print(log_string, file=sys.stdout)
```

### Comparing `froggius-0.1.4.post2/froggius.egg-info/PKG-INFO` & `froggius-0.1.5/froggius.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: froggius
-Version: 0.1.4.post2
+Version: 0.1.5
 Summary: Froggius is a dumb easy logging tool for python
 Home-page: https://github.com/zlElo/Froggius
 Author: zlElo
 Author-email: mail@zlelo.de
 License: MPL-2.0
 Keywords: logging,logger,easy-to-use,log
 Classifier: Intended Audience :: Developers
@@ -23,15 +23,15 @@
   <img src="https://img.shields.io/github/languages/code-size/zlElo/Froggius" alt="GitHub code size in bytes" />
   <img src="https://img.shields.io/github/last-commit/zlElo/Froggius" alt="GitHub last commit" />
   <img src="https://img.shields.io/github/commit-activity/m/zlElo/Froggius" alt="GitHub commit activity month" />
   <img src="https://img.shields.io/github/license/zlElo/Froggius" alt="GitHub license" />
 </p>
 
 # Froggius
-Froggius is a dumb easy logging tool for python
+Froggius is a lightweight and dumb easy logging tool for python
 
 ---------
 
 ## Introduction
 Froggius is a lightweight python libary, which is designed for easy to use logging for all your programs. It makes it easy for everybody, but also brings a lot of options to configure it like you need it. An very interesting feature for example is the error catching for functions, which makes it easy to log unexpected errors, warnings etc.
 
 ## Installation
@@ -132,7 +132,30 @@
 example_function()
 ```
 
 Output in log file:
 `
 [ERR] [01/04/2024 09:15:00] division by zero | Occured on line: 28 in /Users/username/path/examples.py, example_function()
 `
+
+### Using global configuration
+If you want to configure the file_path and the print_out for everything, you can do that with following line before all other Froggius statements:
+
+```py
+# configure print_out and file_path for everything
+Froggius(print_out=False, file_path='tests/example.log')
+
+Froggius.debug('Test normal')
+Froggius.error('Test error')
+Froggius.information('Test information')
+```
+
+It's also possible to say, that you want that all is not printed, but this `Froggius.debug('Test normal')` or `Froggius.information('Test information')`. Just work with the available parameters:
+
+```py
+# configure print_out and file_path for everything
+Froggius(print_out=False, file_path='tests/example.log')
+
+Froggius.debug('Test normal', print_out=True) # everything is not printed, but this line is printed
+Froggius.error('Test error')
+Froggius.information('Test information')
+```
```

### Comparing `froggius-0.1.4.post2/setup.py` & `froggius-0.1.5/setup.py`

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
-    version="0.1.4-2",
+    version="0.1.5",
     author="zlElo",
     author_email="mail@zlelo.de",
     url="https://github.com/zlElo/Froggius",
     keywords=["logging", "logger", "easy-to-use", "log"],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```

