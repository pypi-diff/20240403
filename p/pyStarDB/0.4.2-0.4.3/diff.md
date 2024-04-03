# Comparing `tmp/pyStarDB-0.4.2.tar.gz` & `tmp/pyStarDB-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyStarDB-0.4.2.tar", last modified: Wed Apr 26 07:38:35 2023, max compression
+gzip compressed data, was "pyStarDB-0.4.3.tar", last modified: Wed Apr  3 09:14:43 2024, max compression
```

## Comparing `pyStarDB-0.4.2.tar` & `pyStarDB-0.4.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/
--rw-r--r--   0 twagner  (22293) domain users (32000)     1101 2020-09-15 10:59:24.000000 pyStarDB-0.4.2/LICENSE
--rw-r--r--   0 twagner  (22293) domain users (32000)      234 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)      986 2022-03-25 10:05:17.000000 pyStarDB-0.4.2/README.md
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/pyStarDB/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2020-09-15 10:59:24.000000 pyStarDB-0.4.2/pyStarDB/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    29159 2023-04-26 07:30:04.000000 pyStarDB-0.4.2/pyStarDB/sp_pystardb.py
--rwxr-xr-x   0 twagner  (22293) domain users (32000)     9354 2021-11-03 15:20:34.000000 pyStarDB-0.4.2/pyStarDB/star_viewer.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/pyStarDB.egg-info/
--rw-r--r--   0 twagner  (22293) domain users (32000)      234 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/PKG-INFO
--rw-r--r--   0 twagner  (22293) domain users (32000)      295 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/SOURCES.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)        1 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/dependency_links.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       28 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/requires.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       15 2023-04-26 07:38:35.000000 pyStarDB-0.4.2/pyStarDB.egg-info/top_level.txt
--rw-r--r--   0 twagner  (22293) domain users (32000)       38 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/setup.cfg
--rw-r--r--   0 twagner  (22293) domain users (32000)      466 2023-04-26 07:35:48.000000 pyStarDB-0.4.2/setup.py
-drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2023-04-26 07:38:35.480863 pyStarDB-0.4.2/tests/
--rw-r--r--   0 twagner  (22293) domain users (32000)        0 2020-09-15 11:49:36.000000 pyStarDB-0.4.2/tests/__init__.py
--rw-r--r--   0 twagner  (22293) domain users (32000)    10527 2023-04-26 07:33:37.000000 pyStarDB-0.4.2/tests/test_pystardb.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 09:14:43.017186 pyStarDB-0.4.3/
+-rw-r--r--   0 twagner  (22293) domain users (32000)     1101 2020-09-15 10:59:24.000000 pyStarDB-0.4.3/LICENSE
+-rw-r--r--   0 twagner  (22293) domain users (32000)      251 2024-04-03 09:14:43.017186 pyStarDB-0.4.3/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)      986 2022-03-25 10:05:17.000000 pyStarDB-0.4.3/README.md
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 09:14:43.017186 pyStarDB-0.4.3/pyStarDB/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2020-09-15 10:59:24.000000 pyStarDB-0.4.3/pyStarDB/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    29252 2024-04-03 09:14:26.000000 pyStarDB-0.4.3/pyStarDB/sp_pystardb.py
+-rwxr-xr-x   0 twagner  (22293) domain users (32000)     9354 2021-11-03 15:20:34.000000 pyStarDB-0.4.3/pyStarDB/star_viewer.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 09:14:43.017186 pyStarDB-0.4.3/pyStarDB.egg-info/
+-rw-r--r--   0 twagner  (22293) domain users (32000)      251 2024-04-03 09:14:43.000000 pyStarDB-0.4.3/pyStarDB.egg-info/PKG-INFO
+-rw-r--r--   0 twagner  (22293) domain users (32000)      295 2024-04-03 09:14:43.000000 pyStarDB-0.4.3/pyStarDB.egg-info/SOURCES.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)        1 2024-04-03 09:14:43.000000 pyStarDB-0.4.3/pyStarDB.egg-info/dependency_links.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       28 2024-04-03 09:14:43.000000 pyStarDB-0.4.3/pyStarDB.egg-info/requires.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       15 2024-04-03 09:14:43.000000 pyStarDB-0.4.3/pyStarDB.egg-info/top_level.txt
+-rw-r--r--   0 twagner  (22293) domain users (32000)       38 2024-04-03 09:14:43.017186 pyStarDB-0.4.3/setup.cfg
+-rw-r--r--   0 twagner  (22293) domain users (32000)      483 2024-04-03 09:12:27.000000 pyStarDB-0.4.3/setup.py
+drwxr-xr-x   0 twagner  (22293) domain users (32000)        0 2024-04-03 09:14:43.017186 pyStarDB-0.4.3/tests/
+-rw-r--r--   0 twagner  (22293) domain users (32000)        0 2020-09-15 11:49:36.000000 pyStarDB-0.4.3/tests/__init__.py
+-rw-r--r--   0 twagner  (22293) domain users (32000)    10527 2023-04-26 07:33:37.000000 pyStarDB-0.4.3/tests/test_pystardb.py
```

### Comparing `pyStarDB-0.4.2/LICENSE` & `pyStarDB-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyStarDB-0.4.2/README.md` & `pyStarDB-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pyStarDB-0.4.2/pyStarDB/sp_pystardb.py` & `pyStarDB-0.4.3/pyStarDB/sp_pystardb.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,28 +241,30 @@
         header_names = pandas.read_csv(
             self.star_content,
             usecols=[0],
             skiprows=line_dict['header'][0] - 1,
             nrows=line_dict['header'][1] - line_dict['header'][0] + 1,
             skip_blank_lines=False,
             header=None,
-            delim_whitespace=True,
+            sep='\s+',
+            #delim_whitespace=True,
         )
         header_names = header_names.squeeze("columns")
 
         self.star_content.seek(0)
         return pandas.read_csv(
             self.star_content,
             index_col=None,
             names=header_names,
             skiprows=line_dict['content'][0] - 1,
             nrows=line_dict['content'][1] - line_dict['content'][0] + 1,
             skip_blank_lines=False,
             header=None,
-            delim_whitespace=True,
+            sep='\s+',
+            #delim_whitespace=True,
         )
 
     def read_without_loop(self, line_dict:dict):
         """
         Reads data when block doesn't start with 'loop_'.
         :param line_dict:
         :return:
@@ -274,15 +276,16 @@
             self.star_content,
             index_col=0,
             names=['', '0'],
             skiprows=line_dict['content'][0] - 1,
             nrows=line_dict['content'][1] - line_dict['content'][0] + 1,
             skip_blank_lines=False,
             header=None,
-            delim_whitespace=True,
+            sep='\s+',
+            #delim_whitespace=True,
         ).transpose()
 
     # Never forget the concept of Recursion otherwise you will be doomed
     # This will haunt you forever
     # def __getitem__(self, tag):
     #     return self.__getitem__(tag)
     #
@@ -519,15 +522,16 @@
         :param text_file: Input text file
         :param header: List, column headers -- If None, headers will be column index
         :param is_loop: Boolean, if False, all data will be printed on the same line as the '_rln' parameter name
         :return: None
         """
         self[tag]= pandas.read_csv(
           text_file,
-          delim_whitespace=True, 
+          sep='\s+',
+          #delim_whitespace=True,
           skiprows=1, 
           header=None
           )
           # skiprows: If not specified, leading comment line will be used to define columns
 
         # If None, headers will be column index (which might be easier than '_rlnMicrographShiftX'.)
         if header : self[tag].columns= header
```

### Comparing `pyStarDB-0.4.2/pyStarDB/star_viewer.py` & `pyStarDB-0.4.3/pyStarDB/star_viewer.py`

 * *Files identical despite different names*

### Comparing `pyStarDB-0.4.2/tests/test_pystardb.py` & `pyStarDB-0.4.3/tests/test_pystardb.py`

 * *Files identical despite different names*

