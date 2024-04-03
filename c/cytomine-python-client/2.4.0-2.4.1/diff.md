# Comparing `tmp/cytomine-python-client-2.4.0.tar.gz` & `tmp/cytomine-python-client-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cytomine-python-client-2.4.0.tar", last modified: Thu Jan 18 14:53:30 2024, max compression
+gzip compressed data, was "cytomine-python-client-2.4.1.tar", last modified: Wed Apr  3 08:03:29 2024, max compression
```

## Comparing `cytomine-python-client-2.4.0.tar` & `cytomine-python-client-2.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 14:53:30.547042 cytomine-python-client-2.4.0/
--rw-rw-rw-   0 root         (0) root         (0)    11358 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2296 2024-01-18 14:53:30.543042 cytomine-python-client-2.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1684 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 14:53:30.539042 cytomine-python-client-2.4.0/cytomine/
--rwxrwxrwx   0 root         (0) root         (0)     1016 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    53965 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/cytomine.py
--rw-rw-rw-   0 root         (0) root         (0)    13962 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/cytomine_job.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 14:53:30.543042 cytomine-python-client-2.4.0/cytomine/models/
--rwxrwxrwx   0 root         (0) root         (0)     2739 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 14:53:30.543042 cytomine-python-client-2.4.0/cytomine/models/_utilities/
--rw-rw-rw-   0 root         (0) root         (0)      167 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/_utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/_utilities/dump.py
--rw-rw-rw-   0 root         (0) root         (0)     4425 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/_utilities/parallel.py
--rw-rw-rw-   0 root         (0) root         (0)     1527 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/_utilities/pattern_matching.py
--rw-rw-rw-   0 root         (0) root         (0)    16521 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/annotation.py
--rw-rw-rw-   0 root         (0) root         (0)    11155 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/collection.py
--rwxrwxrwx   0 root         (0) root         (0)    23887 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/image.py
--rwxrwxrwx   0 root         (0) root         (0)     4644 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/model.py
--rwxrwxrwx   0 root         (0) root         (0)     3624 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/ontology.py
--rwxrwxrwx   0 root         (0) root         (0)     3502 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/project.py
--rw-rw-rw-   0 root         (0) root         (0)     7958 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/property.py
--rw-rw-rw-   0 root         (0) root         (0)     7116 2024-01-15 08:47:49.000000 cytomine-python-client-2.4.0/cytomine/models/social.py
--rwxrwxrwx   0 root         (0) root         (0)    12863 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/software.py
--rw-rw-rw-   0 root         (0) root         (0)     3300 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/storage.py
--rw-rw-rw-   0 root         (0) root         (0)     2994 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/track.py
--rwxrwxrwx   0 root         (0) root         (0)     8394 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/models/user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 14:53:30.543042 cytomine-python-client-2.4.0/cytomine/utilities/
--rw-rw-rw-   0 root         (0) root         (0)      972 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/utilities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/utilities/annotations.py
--rw-rw-rw-   0 root         (0) root         (0)     5646 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/utilities/descriptor_reader.py
--rw-rw-rw-   0 root         (0) root         (0)     3527 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/utilities/geometry.py
--rwxrwxrwx   0 root         (0) root         (0)    11203 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/utilities/reader.py
--rw-rw-rw-   0 root         (0) root         (0)     4621 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/utilities/software.py
--rwxrwxrwx   0 root         (0) root         (0)     4412 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/cytomine/utilities/wholeslide.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-18 14:53:30.543042 cytomine-python-client-2.4.0/cytomine_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2296 2024-01-18 14:53:30.000000 cytomine-python-client-2.4.0/cytomine_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1102 2024-01-18 14:53:30.000000 cytomine-python-client-2.4.0/cytomine_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-18 14:53:30.000000 cytomine-python-client-2.4.0/cytomine_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      180 2024-01-18 14:53:30.000000 cytomine-python-client-2.4.0/cytomine_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-01-18 14:53:30.000000 cytomine-python-client-2.4.0/cytomine_python_client.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      973 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/requirements-py2.7.txt
--rw-rw-rw-   0 root         (0) root         (0)     1003 2024-01-12 15:12:20.000000 cytomine-python-client-2.4.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-18 14:53:30.547042 cytomine-python-client-2.4.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2299 2024-01-18 14:53:29.000000 cytomine-python-client-2.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/
+-rw-rw-rw-   0 root         (0) root         (0)    11358 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1684 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.869130 cytomine-python-client-2.4.1/cytomine/
+-rwxrwxrwx   0 root         (0) root         (0)     1016 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    53983 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/cytomine.py
+-rw-rw-rw-   0 root         (0) root         (0)    13962 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/cytomine_job.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.869130 cytomine-python-client-2.4.1/cytomine/models/
+-rwxrwxrwx   0 root         (0) root         (0)     2739 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/cytomine/models/_utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      167 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/_utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/_utilities/dump.py
+-rw-rw-rw-   0 root         (0) root         (0)     4425 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/_utilities/parallel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1527 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/_utilities/pattern_matching.py
+-rw-rw-rw-   0 root         (0) root         (0)    16521 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/annotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    11155 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/collection.py
+-rwxrwxrwx   0 root         (0) root         (0)    23887 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/image.py
+-rwxrwxrwx   0 root         (0) root         (0)     4644 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/model.py
+-rwxrwxrwx   0 root         (0) root         (0)     3624 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/ontology.py
+-rwxrwxrwx   0 root         (0) root         (0)     3502 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/project.py
+-rw-rw-rw-   0 root         (0) root         (0)     7958 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/property.py
+-rw-rw-rw-   0 root         (0) root         (0)     7116 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/social.py
+-rwxrwxrwx   0 root         (0) root         (0)    12863 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/software.py
+-rw-rw-rw-   0 root         (0) root         (0)     3300 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     2994 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/track.py
+-rwxrwxrwx   0 root         (0) root         (0)     8394 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/models/user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/cytomine/utilities/
+-rw-rw-rw-   0 root         (0) root         (0)      972 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2533 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/annotations.py
+-rw-rw-rw-   0 root         (0) root         (0)     5646 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/descriptor_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     3527 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/geometry.py
+-rwxrwxrwx   0 root         (0) root         (0)    11203 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     4621 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/software.py
+-rwxrwxrwx   0 root         (0) root         (0)     4412 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/cytomine/utilities/wholeslide.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1102 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      180 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/cytomine_python_client.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      973 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/requirements-py2.7.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1003 2024-04-03 08:01:55.000000 cytomine-python-client-2.4.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:03:29.873130 cytomine-python-client-2.4.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2299 2024-04-03 08:03:29.000000 cytomine-python-client-2.4.1/setup.py
```

### Comparing `cytomine-python-client-2.4.0/LICENSE` & `cytomine-python-client-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/PKG-INFO` & `cytomine-python-client-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytomine-python-client
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python client to interact with Cytomine.
 Home-page: https://www.cytomine.org
 License: LICENSE
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `cytomine-python-client-2.4.0/README.md` & `cytomine-python-client-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/__init__.py` & `cytomine-python-client-2.4.1/cytomine/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/cytomine.py` & `cytomine-python-client-2.4.1/cytomine/cytomine.py`

 * *Files 0% similar despite different names*

```diff
@@ -443,20 +443,20 @@
         if not response.status_code == requests.codes.ok:
             return False
 
         return response.json()
 
     def get_model(self, model, query_parameters=None):
         response = self._get(model.uri(), query_parameters)
-        
+
         if response.status_code == requests.codes.ok:
             response_json = response.json()
             model = model.populate(response_json)
             self._log_response(response, model)
-            
+
         if not response.status_code == requests.codes.ok:
             self._log_response(response, model.uri())
             model = False
 
         return model
 
     def get_collection(self, collection, query_parameters=None, append_mode=False):
@@ -675,16 +675,17 @@
             query_parameters["idProject"] = id_project  # backwards compatibility
             query_parameters["projects"] = id_project
 
         if properties:
             query_parameters["keys"] = ','.join(list(properties.keys()))
             query_parameters["values"] = ','.join(list(properties.values()))
 
-        m = MultipartEncoder(fields={"files[]": (filename, open(filename, 'rb'))})
-        response = self._session.post("{}/upload".format(upload_host),
+        basename = os.path.basename(filename)
+        m = MultipartEncoder(fields={"files[]": (basename, open(filename, 'rb'))})
+        response = self._session.post(f"{upload_host}/upload",
                                       auth=CytomineAuth(
                                           self._public_key, self._private_key,
                                           upload_host, ""),
                                       headers=self._headers(content_type=m.content_type),
                                       params=query_parameters,
                                       data=m)
```

### Comparing `cytomine-python-client-2.4.0/cytomine/cytomine_job.py` & `cytomine-python-client-2.4.1/cytomine/cytomine_job.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/__init__.py` & `cytomine-python-client-2.4.1/cytomine/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/_utilities/dump.py` & `cytomine-python-client-2.4.1/cytomine/models/_utilities/dump.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/_utilities/parallel.py` & `cytomine-python-client-2.4.1/cytomine/models/_utilities/parallel.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/_utilities/pattern_matching.py` & `cytomine-python-client-2.4.1/cytomine/models/_utilities/pattern_matching.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/annotation.py` & `cytomine-python-client-2.4.1/cytomine/models/annotation.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/collection.py` & `cytomine-python-client-2.4.1/cytomine/models/collection.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/image.py` & `cytomine-python-client-2.4.1/cytomine/models/image.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/model.py` & `cytomine-python-client-2.4.1/cytomine/models/model.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/ontology.py` & `cytomine-python-client-2.4.1/cytomine/models/ontology.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/project.py` & `cytomine-python-client-2.4.1/cytomine/models/project.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/property.py` & `cytomine-python-client-2.4.1/cytomine/models/property.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/social.py` & `cytomine-python-client-2.4.1/cytomine/models/social.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/software.py` & `cytomine-python-client-2.4.1/cytomine/models/software.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/storage.py` & `cytomine-python-client-2.4.1/cytomine/models/storage.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/track.py` & `cytomine-python-client-2.4.1/cytomine/models/track.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/models/user.py` & `cytomine-python-client-2.4.1/cytomine/models/user.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/utilities/__init__.py` & `cytomine-python-client-2.4.1/cytomine/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/utilities/annotations.py` & `cytomine-python-client-2.4.1/cytomine/utilities/annotations.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/utilities/descriptor_reader.py` & `cytomine-python-client-2.4.1/cytomine/utilities/descriptor_reader.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/utilities/geometry.py` & `cytomine-python-client-2.4.1/cytomine/utilities/geometry.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/utilities/reader.py` & `cytomine-python-client-2.4.1/cytomine/utilities/reader.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/utilities/software.py` & `cytomine-python-client-2.4.1/cytomine/utilities/software.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine/utilities/wholeslide.py` & `cytomine-python-client-2.4.1/cytomine/utilities/wholeslide.py`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/cytomine_python_client.egg-info/PKG-INFO` & `cytomine-python-client-2.4.1/cytomine_python_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cytomine-python-client
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python client to interact with Cytomine.
 Home-page: https://www.cytomine.org
 License: LICENSE
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `cytomine-python-client-2.4.0/cytomine_python_client.egg-info/SOURCES.txt` & `cytomine-python-client-2.4.1/cytomine_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/requirements-py2.7.txt` & `cytomine-python-client-2.4.1/requirements-py2.7.txt`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/requirements.txt` & `cytomine-python-client-2.4.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `cytomine-python-client-2.4.0/setup.py` & `cytomine-python-client-2.4.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 with open("README.md", "r", encoding="utf8") as fh:
     long_description = fh.read()
 
 pillow_version_constraint = ',<7.0.0' if sys.version_info.major < 3 else ''
 
 setup(
     name='cytomine-python-client',
-    version='2.4.0',
+    version='2.4.1',
     description='Python client to interact with Cytomine.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['cytomine', 'cytomine.models', 'cytomine.models._utilities', 'cytomine.utilities'],
     url='https://www.cytomine.org',
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
```

