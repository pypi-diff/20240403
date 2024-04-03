# Comparing `tmp/lpb_lib-0.0.8.tar.gz` & `tmp/lpb_lib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpb_lib-0.0.8.tar", last modified: Wed Apr  3 14:21:49 2024, max compression
+gzip compressed data, was "lpb_lib-0.0.9.tar", last modified: Wed Apr  3 15:08:16 2024, max compression
```

## Comparing `lpb_lib-0.0.8.tar` & `lpb_lib-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:21:49.470280 lpb_lib-0.0.8/
--rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      755 2024-04-03 14:21:49.469282 lpb_lib-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      260 2024-04-03 14:07:09.000000 lpb_lib-0.0.8/README.md
--rw-rw-rw-   0        0        0     1207 2024-04-03 13:20:54.000000 lpb_lib-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      626 2024-04-03 14:21:49.472278 lpb_lib-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 14:21:49.436004 lpb_lib-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 14:21:49.455558 lpb_lib-0.0.8/src/lpb_lib/
--rw-rw-rw-   0        0        0        0 2024-04-03 14:08:10.000000 lpb_lib-0.0.8/src/lpb_lib/__init__.py
--rw-rw-rw-   0        0        0     1530 2024-04-03 13:21:41.000000 lpb_lib-0.0.8/src/lpb_lib/big_query.py
--rw-rw-rw-   0        0        0      367 2024-04-03 13:13:33.000000 lpb_lib-0.0.8/src/lpb_lib/compute_log.py
--rw-rw-rw-   0        0        0      574 2024-04-03 14:21:06.000000 lpb_lib-0.0.8/src/lpb_lib/get_env.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:21:49.468282 lpb_lib-0.0.8/src/lpb_lib.egg-info/
--rw-rw-rw-   0        0        0      755 2024-04-03 14:21:48.000000 lpb_lib-0.0.8/src/lpb_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      281 2024-04-03 14:21:48.000000 lpb_lib-0.0.8/src/lpb_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:21:48.000000 lpb_lib-0.0.8/src/lpb_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-03 14:21:48.000000 lpb_lib-0.0.8/src/lpb_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 15:08:16.126795 lpb_lib-0.0.9/
+-rw-rw-rw-   0        0        0        0 2024-04-03 09:50:17.000000 lpb_lib-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      823 2024-04-03 15:08:16.125796 lpb_lib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      328 2024-04-03 15:01:26.000000 lpb_lib-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1342 2024-04-03 15:06:28.000000 lpb_lib-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      626 2024-04-03 15:08:16.141810 lpb_lib-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 15:08:16.034797 lpb_lib-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 15:08:16.100892 lpb_lib-0.0.9/src/lpb_lib/
+-rw-rw-rw-   0        0        0        0 2024-04-03 14:08:10.000000 lpb_lib-0.0.9/src/lpb_lib/__init__.py
+-rw-rw-rw-   0        0        0     1530 2024-04-03 13:21:41.000000 lpb_lib-0.0.9/src/lpb_lib/big_query.py
+-rw-rw-rw-   0        0        0      367 2024-04-03 13:13:33.000000 lpb_lib-0.0.9/src/lpb_lib/compute_log.py
+-rw-rw-rw-   0        0        0      614 2024-04-03 14:58:12.000000 lpb_lib-0.0.9/src/lpb_lib/get_env.py
+-rw-rw-rw-   0        0        0     6844 2024-04-03 15:00:54.000000 lpb_lib-0.0.9/src/lpb_lib/gmail.py
+-rw-rw-rw-   0        0        0     4206 2024-04-03 15:05:14.000000 lpb_lib-0.0.9/src/lpb_lib/gsheet.py
+-rw-rw-rw-   0        0        0        0 2024-04-03 14:31:22.000000 lpb_lib-0.0.9/src/lpb_lib/main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:08:16.121799 lpb_lib-0.0.9/src/lpb_lib.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-04-03 15:08:15.000000 lpb_lib-0.0.9/src/lpb_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2024-04-03 15:08:15.000000 lpb_lib-0.0.9/src/lpb_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:08:15.000000 lpb_lib-0.0.9/src/lpb_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 15:08:15.000000 lpb_lib-0.0.9/src/lpb_lib.egg-info/top_level.txt
```

### Comparing `lpb_lib-0.0.8/PKG-INFO` & `lpb_lib-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpb_lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package contains tools that will help me to develop my projects
 Home-page: https://github.com/Fajitas08090/lpb_lib
 Author: Maxime Renac
 Author-email: maxime.renac@lepetitballon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,8 @@
 
 # lpb_lib
 This repo allows me to deploy the tools I need for my projects at LPB.
 
 # Main features
 *  big_query : This function allows me to query the data from BigQuery.
 *  get_env : This function allows me to get the environment variables from .env file.
+*  gmail : This function allows me to send emails using Gmail API.
```

### Comparing `lpb_lib-0.0.8/pyproject.toml` & `lpb_lib-0.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 "build==1.2.1",
 "cachetools==5.3.3",
 "certifi==2024.2.2",
 "charset-normalizer==3.3.2",
 "colorama==0.4.6",
 "docutils==0.20.1",
 "google-api-core==2.18.0",
+"google-api-python-client==2.125.0",
 "google-auth==2.29.0",
+"google-auth-httplib2==0.2.0",
 "google-cloud-bigquery==3.20.1",
 "google-cloud-core==2.4.1",
 "google-crc32c==1.5.0",
 "google-resumable-media==2.7.0",
 "googleapis-common-protos==1.63.0",
 "grpcio==1.62.1",
 "grpcio-status==1.62.1",
+"httplib2==0.22.0",
 "idna==3.6",
 "importlib_metadata==7.1.0",
 "jaraco.classes==3.4.0",
 "jaraco.context==4.3.0",
 "jaraco.functools==4.0.0",
 "keyring==25.1.0",
 "markdown-it-py==3.0.0",
@@ -31,23 +34,25 @@
 "pandas==2.2.1",
 "pkginfo==1.10.0",
 "proto-plus==1.23.0",
 "protobuf==4.25.3",
 "pyasn1==0.6.0",
 "pyasn1_modules==0.4.0",
 "Pygments==2.17.2",
+"pyparsing==3.1.2",
 "pyproject_hooks==1.0.0",
 "python-dateutil==2.9.0.post0",
 "pytz==2024.1",
 "pywin32-ctypes==0.2.2",
 "readme_renderer==43.0",
 "requests==2.31.0",
 "requests-toolbelt==1.0.0",
 "rfc3986==2.0.0",
 "rich==13.7.1",
 "rsa==4.9",
 "six==1.16.0",
 "twine==5.0.0",
 "tzdata==2024.1",
+"uritemplate==4.1.1",
 "urllib3==2.2.1",
 "zipp==3.18.1"]
 build-backend = "setuptools.build_meta"
```

### Comparing `lpb_lib-0.0.8/setup.cfg` & `lpb_lib-0.0.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206c 7062 5f6c 6962 0d0a 7665 7273   = lpb_lib..vers
-00000020: 696f 6e20 3d20 302e 302e 380d 0a61 7574  ion = 0.0.8..aut
+00000020: 696f 6e20 3d20 302e 302e 390d 0a61 7574  ion = 0.0.9..aut
 00000030: 686f 7220 3d20 4d61 7869 6d65 2052 656e  hor = Maxime Ren
 00000040: 6163 0d0a 6175 7468 6f72 5f65 6d61 696c  ac..author_email
 00000050: 203d 206d 6178 696d 652e 7265 6e61 6340   = maxime.renac@
 00000060: 6c65 7065 7469 7462 616c 6c6f 6e2e 636f  lepetitballon.co
 00000070: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000080: 2054 6869 7320 7061 636b 6167 6520 636f   This package co
 00000090: 6e74 6169 6e73 2074 6f6f 6c73 2074 6861  ntains tools tha
```

### Comparing `lpb_lib-0.0.8/src/lpb_lib/big_query.py` & `lpb_lib-0.0.9/src/lpb_lib/big_query.py`

 * *Files identical despite different names*

### Comparing `lpb_lib-0.0.8/src/lpb_lib/get_env.py` & `lpb_lib-0.0.9/src/lpb_lib/get_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 import lpb_lib
 
-def find_code_in_env_file(path, code_to_find):    
+def find_code_in_env_file(path_w, code_to_find):    
     """
     Find a code in the .env file and return its value.
     Args:
     :path: The path to the .env file.
     :code_to_find: The code to find in the .env file.
     Returns:
         :value: The value of the code in the .env file.
     """
-    if os.path.exists(".env"):
-        with open(".env", 'r') as file:
+    if os.path.exists(f"{path_w}/.env"):
+        with open(f"{path_w}/.env", 'r') as file:
             for line in file:
                 if code_to_find in line:
-                    value = line.split("=")[1]
-                    return value
+                    value = line.split("= ")[1]
+                    return value.replace('"', "")
     return None
```

### Comparing `lpb_lib-0.0.8/src/lpb_lib.egg-info/PKG-INFO` & `lpb_lib-0.0.9/src/lpb_lib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpb_lib
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package contains tools that will help me to develop my projects
 Home-page: https://github.com/Fajitas08090/lpb_lib
 Author: Maxime Renac
 Author-email: maxime.renac@lepetitballon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,7 +14,8 @@
 
 # lpb_lib
 This repo allows me to deploy the tools I need for my projects at LPB.
 
 # Main features
 *  big_query : This function allows me to query the data from BigQuery.
 *  get_env : This function allows me to get the environment variables from .env file.
+*  gmail : This function allows me to send emails using Gmail API.
```

