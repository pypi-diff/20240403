# Comparing `tmp/microsoftgraph-python-1.1.5.tar.gz` & `tmp/microsoftgraph_python-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoftgraph-python-1.1.5.tar", last modified: Thu Nov 17 23:06:52 2022, max compression
+gzip compressed data, was "microsoftgraph_python-1.1.6.tar", max compression
```

## Comparing `microsoftgraph-python-1.1.5.tar` & `microsoftgraph_python-1.1.6.tar`

### file list

```diff
@@ -1,29 +1,18 @@
-drwxr-xr-x   0 ingmferrer  (1000) ingmferrer  (1000)        0 2022-11-17 23:06:52.772945 microsoftgraph-python-1.1.5/
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1065 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/LICENSE
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)       18 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/MANIFEST.in
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     9651 2022-11-17 23:06:52.772945 microsoftgraph-python-1.1.5/PKG-INFO
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     9280 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/README.md
-drwxr-xr-x   0 ingmferrer  (1000) ingmferrer  (1000)        0 2022-11-17 23:06:52.772945 microsoftgraph-python-1.1.5/microsoftgraph/
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)        0 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/__init__.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     5603 2022-07-01 15:10:16.000000 microsoftgraph-python-1.1.5/microsoftgraph/calendar.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)    13081 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/client.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     4452 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/contacts.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      632 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/decorators.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1073 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/exceptions.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     8022 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/files.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     6602 2022-11-17 23:06:30.000000 microsoftgraph-python-1.1.5/microsoftgraph/mail.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     3103 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/notes.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      871 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/response.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     1174 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/users.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      220 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/utils.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     3321 2022-07-01 15:10:16.000000 microsoftgraph-python-1.1.5/microsoftgraph/webhooks.py
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)    12372 2022-07-01 14:50:34.000000 microsoftgraph-python-1.1.5/microsoftgraph/workbooks.py
-drwxr-xr-x   0 ingmferrer  (1000) ingmferrer  (1000)        0 2022-11-17 23:06:52.772945 microsoftgraph-python-1.1.5/microsoftgraph_python.egg-info/
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)     9651 2022-11-17 23:06:52.000000 microsoftgraph-python-1.1.5/microsoftgraph_python.egg-info/PKG-INFO
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      671 2022-11-17 23:06:52.000000 microsoftgraph-python-1.1.5/microsoftgraph_python.egg-info/SOURCES.txt
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)        1 2022-11-17 23:06:52.000000 microsoftgraph-python-1.1.5/microsoftgraph_python.egg-info/dependency_links.txt
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)        1 2022-07-01 15:09:51.000000 microsoftgraph-python-1.1.5/microsoftgraph_python.egg-info/not-zip-safe
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)        9 2022-11-17 23:06:52.000000 microsoftgraph-python-1.1.5/microsoftgraph_python.egg-info/requires.txt
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)       15 2022-11-17 23:06:52.000000 microsoftgraph-python-1.1.5/microsoftgraph_python.egg-info/top_level.txt
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)       38 2022-11-17 23:06:52.772945 microsoftgraph-python-1.1.5/setup.cfg
--rw-r--r--   0 ingmferrer  (1000) ingmferrer  (1000)      640 2022-11-17 23:06:46.000000 microsoftgraph-python-1.1.5/setup.py
+-rw-r--r--   0        0        0     1065 2023-03-27 20:32:33.898149 microsoftgraph_python-1.1.6/LICENSE
+-rw-r--r--   0        0        0     9280 2023-03-27 20:32:33.898418 microsoftgraph_python-1.1.6/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 20:32:33.898512 microsoftgraph_python-1.1.6/microsoftgraph/__init__.py
+-rw-r--r--   0        0        0     5603 2023-03-27 20:32:33.898642 microsoftgraph_python-1.1.6/microsoftgraph/calendar.py
+-rw-r--r--   0        0        0    13081 2023-03-27 20:32:33.898806 microsoftgraph_python-1.1.6/microsoftgraph/client.py
+-rw-r--r--   0        0        0     4452 2023-03-27 20:32:33.898907 microsoftgraph_python-1.1.6/microsoftgraph/contacts.py
+-rw-r--r--   0        0        0      632 2023-03-27 20:32:33.898994 microsoftgraph_python-1.1.6/microsoftgraph/decorators.py
+-rw-r--r--   0        0        0     1073 2023-03-27 20:32:33.899233 microsoftgraph_python-1.1.6/microsoftgraph/exceptions.py
+-rw-r--r--   0        0        0     8022 2023-03-27 20:32:33.899377 microsoftgraph_python-1.1.6/microsoftgraph/files.py
+-rw-r--r--   0        0        0     6602 2023-03-27 20:32:33.899479 microsoftgraph_python-1.1.6/microsoftgraph/mail.py
+-rw-r--r--   0        0        0     3103 2023-03-27 20:32:33.899592 microsoftgraph_python-1.1.6/microsoftgraph/notes.py
+-rw-r--r--   0        0        0      871 2023-03-27 20:32:33.899686 microsoftgraph_python-1.1.6/microsoftgraph/response.py
+-rw-r--r--   0        0        0     1174 2023-03-27 20:32:33.899797 microsoftgraph_python-1.1.6/microsoftgraph/users.py
+-rw-r--r--   0        0        0      220 2023-03-27 20:32:33.899884 microsoftgraph_python-1.1.6/microsoftgraph/utils.py
+-rw-r--r--   0        0        0     3321 2023-03-27 20:32:33.899980 microsoftgraph_python-1.1.6/microsoftgraph/webhooks.py
+-rw-r--r--   0        0        0    12372 2023-03-27 20:32:33.900065 microsoftgraph_python-1.1.6/microsoftgraph/workbooks.py
+-rw-r--r--   0        0        0      416 2023-03-27 20:35:00.604777 microsoftgraph_python-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0     9942 1970-01-01 00:00:00.000000 microsoftgraph_python-1.1.6/PKG-INFO
```

### Comparing `microsoftgraph-python-1.1.5/LICENSE` & `microsoftgraph_python-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/PKG-INFO` & `microsoftgraph_python-1.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: microsoftgraph-python
-Version: 1.1.5
-Summary: API wrapper for Microsoft Graph written in Python
-Home-page: https://github.com/GearPlug/microsoftgraph-python
-Author: Miguel Ferrer, Nerio Rincon, Yordy Gelvez
-Author-email: ingferrermiguel@gmail.com
-License: MIT
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # microsoftgraph-python
 Microsoft graph API wrapper for Microsoft Graph written in Python.
 
 ## Before start
 To use Microsoft Graph to read and write resources on behalf of a user, your app must get an access token from
 the Microsoft identity platform and attach the token to requests that it sends to Microsoft Graph. The exact
 authentication flow that you will use to get access tokens will depend on the kind of app you are developing and
@@ -380,9 +368,7 @@
 ## Requirements
 - requests
 
 ## Tests
 ```
 test/test.py
 ```
-
-
```

### Comparing `microsoftgraph-python-1.1.5/README.md` & `microsoftgraph_python-1.1.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: microsoftgraph-python
+Version: 1.1.6
+Summary: API wrapper for Microsoft Graph written in Python
+License: MIT
+Author: Miguel Ferrer
+Author-email: ingferrermiguel@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.26.0,<3.0.0)
+Description-Content-Type: text/markdown
+
 # microsoftgraph-python
 Microsoft graph API wrapper for Microsoft Graph written in Python.
 
 ## Before start
 To use Microsoft Graph to read and write resources on behalf of a user, your app must get an access token from
 the Microsoft identity platform and attach the token to requests that it sends to Microsoft Graph. The exact
 authentication flow that you will use to get access tokens will depend on the kind of app you are developing and
@@ -368,7 +386,8 @@
 ## Requirements
 - requests
 
 ## Tests
 ```
 test/test.py
 ```
+
```

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/calendar.py` & `microsoftgraph_python-1.1.6/microsoftgraph/calendar.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/client.py` & `microsoftgraph_python-1.1.6/microsoftgraph/client.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/contacts.py` & `microsoftgraph_python-1.1.6/microsoftgraph/contacts.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/decorators.py` & `microsoftgraph_python-1.1.6/microsoftgraph/decorators.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/exceptions.py` & `microsoftgraph_python-1.1.6/microsoftgraph/exceptions.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/files.py` & `microsoftgraph_python-1.1.6/microsoftgraph/files.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/mail.py` & `microsoftgraph_python-1.1.6/microsoftgraph/mail.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/notes.py` & `microsoftgraph_python-1.1.6/microsoftgraph/notes.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/response.py` & `microsoftgraph_python-1.1.6/microsoftgraph/response.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/users.py` & `microsoftgraph_python-1.1.6/microsoftgraph/users.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/webhooks.py` & `microsoftgraph_python-1.1.6/microsoftgraph/webhooks.py`

 * *Files identical despite different names*

### Comparing `microsoftgraph-python-1.1.5/microsoftgraph/workbooks.py` & `microsoftgraph_python-1.1.6/microsoftgraph/workbooks.py`

 * *Files identical despite different names*

