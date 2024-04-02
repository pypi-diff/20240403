# Comparing `tmp/apitoolkit-pyramid-0.0.2.tar.gz` & `tmp/apitoolkit-pyramid-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apitoolkit-pyramid-0.0.2.tar", last modified: Tue Apr  2 21:39:23 2024, max compression
+gzip compressed data, was "apitoolkit-pyramid-0.1.2.tar", last modified: Tue Apr  2 21:48:26 2024, max compression
```

## Comparing `apitoolkit-pyramid-0.0.2.tar` & `apitoolkit-pyramid-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 21:39:23.944646 apitoolkit-pyramid-0.0.2/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     1067 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.0.2/LICENSE
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      275 2024-04-02 21:39:23.944646 apitoolkit-pyramid-0.0.2/PKG-INFO
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       40 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.0.2/README.md
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 21:39:23.940645 apitoolkit-pyramid-0.0.2/apitoolkit_pyramid/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     6488 2024-04-02 21:28:57.000000 apitoolkit-pyramid-0.0.2/apitoolkit_pyramid/__init__.py
-drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 21:39:23.944646 apitoolkit-pyramid-0.0.2/apitoolkit_pyramid.egg-info/
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      275 2024-04-02 21:39:23.000000 apitoolkit-pyramid-0.0.2/apitoolkit_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      266 2024-04-02 21:39:23.000000 apitoolkit-pyramid-0.0.2/apitoolkit_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)        1 2024-04-02 21:39:23.000000 apitoolkit-pyramid-0.0.2/apitoolkit_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       84 2024-04-02 21:39:23.000000 apitoolkit-pyramid-0.0.2/apitoolkit_pyramid.egg-info/requires.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       19 2024-04-02 21:39:23.000000 apitoolkit-pyramid-0.0.2/apitoolkit_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       38 2024-04-02 21:39:23.944646 apitoolkit-pyramid-0.0.2/setup.cfg
--rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      634 2024-04-02 21:39:13.000000 apitoolkit-pyramid-0.0.2/setup.py
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 21:48:26.723083 apitoolkit-pyramid-0.1.2/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     1067 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.1.2/LICENSE
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      275 2024-04-02 21:48:26.723083 apitoolkit-pyramid-0.1.2/PKG-INFO
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       40 2024-04-01 20:32:31.000000 apitoolkit-pyramid-0.1.2/README.md
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 21:48:26.719083 apitoolkit-pyramid-0.1.2/apitoolkit_pyramid/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)     6489 2024-04-02 21:47:35.000000 apitoolkit-pyramid-0.1.2/apitoolkit_pyramid/__init__.py
+drwxrwxr-x   0 dawkaka   (1000) dawkaka   (1000)        0 2024-04-02 21:48:26.723083 apitoolkit-pyramid-0.1.2/apitoolkit_pyramid.egg-info/
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      275 2024-04-02 21:48:26.000000 apitoolkit-pyramid-0.1.2/apitoolkit_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      266 2024-04-02 21:48:26.000000 apitoolkit-pyramid-0.1.2/apitoolkit_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)        1 2024-04-02 21:48:26.000000 apitoolkit-pyramid-0.1.2/apitoolkit_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       84 2024-04-02 21:48:26.000000 apitoolkit-pyramid-0.1.2/apitoolkit_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       19 2024-04-02 21:48:26.000000 apitoolkit-pyramid-0.1.2/apitoolkit_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)       38 2024-04-02 21:48:26.723083 apitoolkit-pyramid-0.1.2/setup.cfg
+-rw-rw-r--   0 dawkaka   (1000) dawkaka   (1000)      634 2024-04-02 21:47:47.000000 apitoolkit-pyramid-0.1.2/setup.py
```

### Comparing `apitoolkit-pyramid-0.0.2/LICENSE` & `apitoolkit-pyramid-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `apitoolkit-pyramid-0.0.2/apitoolkit_pyramid/__init__.py` & `apitoolkit-pyramid-0.1.2/apitoolkit_pyramid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
                 "method": request_method,
                 "url_path": url_path,
                 "raw_url": url_path_with_query ,
                 "request_body": base64.b64encode(request_body).decode("utf-8"),
                 "response_body": base64.b64encode(response_body).decode("utf-8"),
                 "host": request.headers.get('HOST',""),
                 "referer": request.headers.get('Referer', ""),
-                "sdk_type": "PythonDjango",
+                "sdk_type": "PythonPyramid",
                 "project_id": self.meta["project_id"],
                 "status_code": status_code,
                 "errors": errors,
                 "msg_id": message_id,
                 "parent_id": None,
                 "duration": duration,
                 "service_version": self.service_version,
```

### Comparing `apitoolkit-pyramid-0.0.2/setup.py` & `apitoolkit-pyramid-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="apitoolkit-pyramid",
-    version="0.0.2",
+    version="0.1.2",
     packages=find_packages(),
     description='A Python Pyramid SDK for Apitoolkit integration',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author_email='hello@apitoolkit.io',
     author='APIToolkit',
     install_requires=[
```

