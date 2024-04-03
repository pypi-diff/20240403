# Comparing `tmp/HandyLLM-0.6.1.tar.gz` & `tmp/HandyLLM-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HandyLLM-0.6.1.tar", last modified: Wed Apr  3 15:45:13 2024, max compression
+gzip compressed data, was "HandyLLM-0.6.2.tar", last modified: Wed Apr  3 15:46:14 2024, max compression
```

## Comparing `HandyLLM-0.6.1.tar` & `HandyLLM-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:13.699469 HandyLLM-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-03 15:45:13.695469 HandyLLM-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 15:45:10.000000 HandyLLM-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:45:13.699469 HandyLLM-0.6.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:13.691470 HandyLLM-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:13.695469 HandyLLM-0.6.1/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-03 15:45:13.000000 HandyLLM-0.6.1/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 15:45:13.000000 HandyLLM-0.6.1/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:45:13.000000 HandyLLM-0.6.1/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 15:45:13.000000 HandyLLM-0.6.1/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 15:45:13.000000 HandyLLM-0.6.1/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:13.695469 HandyLLM-0.6.1/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:13.695469 HandyLLM-0.6.1/src/handyllm/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/deprecated/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/deprecated/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/src/handyllm/requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2191 2024-04-03 15:45:10.000000 HandyLLM-0.6.1/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:45:13.695469 HandyLLM-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/tests/test_client_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 15:45:09.000000 HandyLLM-0.6.1/tests/test_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.497467 HandyLLM-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 15:46:14.000000 HandyLLM-0.6.2/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/src/handyllm/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/deprecated/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/deprecated/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11014 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:46:14.501467 HandyLLM-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/tests/test_client_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 15:46:07.000000 HandyLLM-0.6.2/tests/test_prompt.py
```

### Comparing `HandyLLM-0.6.1/PKG-INFO` & `HandyLLM-0.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.6.1
+Version: 0.6.2
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.6.1/README.md` & `HandyLLM-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/pyproject.toml` & `HandyLLM-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.6.1"
+version = "0.6.2"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HandyLLM-0.6.1/src/HandyLLM.egg-info/PKG-INFO` & `HandyLLM-0.6.2/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.6.1
+Version: 0.6.2
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `HandyLLM-0.6.1/src/HandyLLM.egg-info/SOURCES.txt` & `HandyLLM-0.6.2/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/_utils.py` & `HandyLLM-0.6.2/src/handyllm/_utils.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/deprecated/api_request.py` & `HandyLLM-0.6.2/src/handyllm/deprecated/api_request.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/deprecated/openai_api.py` & `HandyLLM-0.6.2/src/handyllm/deprecated/openai_api.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/endpoint_manager.py` & `HandyLLM-0.6.2/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/openai_api.py` & `HandyLLM-0.6.2/src/handyllm/openai_api.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/openai_client.py` & `HandyLLM-0.6.2/src/handyllm/openai_client.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/prompt_converter.py` & `HandyLLM-0.6.2/src/handyllm/prompt_converter.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/requestor.py` & `HandyLLM-0.6.2/src/handyllm/requestor.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/src/handyllm/utils.py` & `HandyLLM-0.6.2/src/handyllm/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-import requests
 from urllib.parse import urlparse
 import os
 import time
 
 
 def get_filename_from_url(download_url):
     # Parse the URL.
     parsed_url = urlparse(download_url)
     # The last part of the path is usually the filename.
     filename = os.path.basename(parsed_url.path)
     return filename
 
 def download_binary(download_url, file_path=None, dir='.'):
+    import requests
     response = requests.get(download_url, allow_redirects=True)
     if file_path == None:
         filename = get_filename_from_url(download_url)
         if filename == '' or filename == None:
             filename = 'download_' + time.strftime("%Y%m%d_%H%M%S")
         file_path = os.path.abspath(os.path.join(dir, filename))
     # Open the file in binary mode and write to it.
```

### Comparing `HandyLLM-0.6.1/tests/test_azure.py` & `HandyLLM-0.6.2/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/tests/test_client_async_sync.py` & `HandyLLM-0.6.2/tests/test_client_async_sync.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/tests/test_endpoint.py` & `HandyLLM-0.6.2/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `HandyLLM-0.6.1/tests/test_prompt.py` & `HandyLLM-0.6.2/tests/test_prompt.py`

 * *Files identical despite different names*

