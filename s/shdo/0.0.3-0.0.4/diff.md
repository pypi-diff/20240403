# Comparing `tmp/shdo-0.0.3.tar.gz` & `tmp/shdo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shdo-0.0.3.tar", last modified: Tue Apr  2 12:11:44 2024, max compression
+gzip compressed data, was "shdo-0.0.4.tar", last modified: Tue Apr  2 12:16:44 2024, max compression
```

## Comparing `shdo-0.0.3.tar` & `shdo-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:11:44.779994 shdo-0.0.3/
--rw-rw-rw-   0        0        0      329 2024-04-02 12:11:44.778647 shdo-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-02 12:11:44.780592 shdo-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      580 2024-04-02 12:10:17.000000 shdo-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:11:44.776865 shdo-0.0.3/shdo.egg-info/
--rw-rw-rw-   0        0        0      329 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      169 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 12:11:44.000000 shdo-0.0.3/shdo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    12848 2024-04-02 12:05:54.000000 shdo-0.0.3/shdo.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:44.953054 shdo-0.0.4/
+-rw-rw-rw-   0        0        0      329 2024-04-02 12:16:44.949956 shdo-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 12:16:44.953966 shdo-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      580 2024-04-02 12:16:38.000000 shdo-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 12:16:44.945988 shdo-0.0.4/shdo.egg-info/
+-rw-rw-rw-   0        0        0      329 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      169 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-02 12:16:44.000000 shdo-0.0.4/shdo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13138 2024-04-02 12:16:19.000000 shdo-0.0.4/shdo.py
```

### Comparing `shdo-0.0.3/setup.py` & `shdo-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup
 
 setup(
     name='shdo',
-    version='0.0.3',
+    version='0.0.4',
     packages=['shdo'],
     package_dir={'shdo': '.'},
     py_modules=['shdo'],
     entry_points={
         'console_scripts': [
             'shdo = shdo:main'
         ]
     },
     author='Zen',
     description='A tool to escalate privileges in Android',
-    long_description='shdo is a tool that helps you run elevated commands in Android (similar to sudo) without requiring root access. It utilizes debug privileges instead of root privileges.',
+    long_description='Shdo is a tool that helps you run elevated commands in Android (similar to sudo) without requiring root access. It utilizes debug privileges instead of root privileges.',
     url='https://github.com/42zen/shdo',
 )
```

### Comparing `shdo-0.0.3/shdo.py` & `shdo-0.0.4/shdo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # import the command line variable
 from sys import argv as sys_argv
+from os import environ
 
 # import the file functions
 from os.path import exists as file_exists
 from shutil import copy as file_copy, SameFileError
 
 # import the path function
 from os.path import expanduser as path_get_user_directory
@@ -40,14 +41,19 @@
     argv = sys_argv
 
     # check usage
     if argc <= 1:
         print("Usage: shdo <command> [parameters]")
         return 1
     
+    # check if we're running the tool with termux
+    if 'TERMUX_VERSION' not in environ:
+        print("Error: You need to run this tool from Termux. If you want to run this tool anyway create the environment variable 'TERMUX_VERSION'.")
+        return 1
+    
     # build the command
     parameters = ""
     if argc >= 3:
         for parameter in argv[2:]:
             parameters += f" '{parameter}'"
 
     # run the command
```

