# Comparing `tmp/bbwebservice-1.0.4.tar.gz` & `tmp/bbwebservice-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbwebservice-1.0.4.tar", last modified: Wed Apr  3 16:37:38 2024, max compression
+gzip compressed data, was "bbwebservice-1.0.5.tar", last modified: Wed Apr  3 16:49:50 2024, max compression
```

## Comparing `bbwebservice-1.0.4.tar` & `bbwebservice-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 16:37:38.806518 bbwebservice-1.0.4/
--rw-rw-rw-   0        0        0     1092 2022-11-21 21:52:54.000000 bbwebservice-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     5184 2024-04-03 16:37:38.672978 bbwebservice-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4799 2024-03-30 23:50:09.000000 bbwebservice-1.0.4/README.md
--rw-rw-rw-   0        0        0      108 2022-11-21 16:45:12.000000 bbwebservice-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      523 2024-04-03 16:37:38.810520 bbwebservice-1.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 16:37:37.999989 bbwebservice-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 16:37:38.656804 bbwebservice-1.0.4/src/bbwebservice.egg-info/
--rw-rw-rw-   0        0        0     5184 2024-04-03 16:37:37.000000 bbwebservice-1.0.4/src/bbwebservice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2024-04-03 16:37:37.000000 bbwebservice-1.0.4/src/bbwebservice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 16:37:37.000000 bbwebservice-1.0.4/src/bbwebservice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 16:37:37.000000 bbwebservice-1.0.4/src/bbwebservice.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 16:49:50.671970 bbwebservice-1.0.5/
+-rw-rw-rw-   0        0        0     1092 2022-11-21 21:52:54.000000 bbwebservice-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5184 2024-04-03 16:49:50.539900 bbwebservice-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4799 2024-03-30 23:50:09.000000 bbwebservice-1.0.5/README.md
+-rw-rw-rw-   0        0        0      108 2022-11-21 16:45:12.000000 bbwebservice-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      523 2024-04-03 16:49:50.683479 bbwebservice-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 16:49:48.459437 bbwebservice-1.0.5/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 16:49:49.709118 bbwebservice-1.0.5/src/bbwebservice/
+-rw-rw-rw-   0        0        0     1892 2024-03-21 01:05:32.000000 bbwebservice-1.0.5/src/bbwebservice/__init__.py
+-rw-rw-rw-   0        0        0      796 2024-03-29 16:07:29.000000 bbwebservice-1.0.5/src/bbwebservice/app_utils.py
+-rw-rw-rw-   0        0        0     1949 2022-11-22 10:00:46.000000 bbwebservice-1.0.5/src/bbwebservice/config_loader.py
+-rw-rw-rw-   0        0        0     4970 2024-03-29 19:35:56.000000 bbwebservice-1.0.5/src/bbwebservice/core.py
+-rw-rw-rw-   0        0        0    30166 2024-03-31 21:57:37.000000 bbwebservice-1.0.5/src/bbwebservice/http_parser.py
+-rw-rw-rw-   0        0        0     1009 2023-09-09 12:34:49.000000 bbwebservice-1.0.5/src/bbwebservice/special_media_type.py
+-rw-rw-rw-   0        0        0     3326 2024-03-30 23:40:38.000000 bbwebservice-1.0.5/src/bbwebservice/url_utils.py
+-rw-rw-rw-   0        0        0     9736 2024-03-29 19:45:30.000000 bbwebservice-1.0.5/src/bbwebservice/webserver.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:49:50.525359 bbwebservice-1.0.5/src/bbwebservice.egg-info/
+-rw-rw-rw-   0        0        0     5184 2024-04-03 16:49:48.000000 bbwebservice-1.0.5/src/bbwebservice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2024-04-03 16:49:48.000000 bbwebservice-1.0.5/src/bbwebservice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 16:49:48.000000 bbwebservice-1.0.5/src/bbwebservice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-04-03 16:49:48.000000 bbwebservice-1.0.5/src/bbwebservice.egg-info/top_level.txt
```

### Comparing `bbwebservice-1.0.4/LICENSE` & `bbwebservice-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.4/PKG-INFO` & `bbwebservice-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbwebservice
-Version: 1.0.4
+Version: 1.0.5
 Summary: A bare bone webserver
 Author: Lukas
 Author-email: lukasogwalker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `bbwebservice-1.0.4/README.md` & `bbwebservice-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bbwebservice-1.0.4/setup.cfg` & `bbwebservice-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 6277 6562 7365 7276 6963 650d   = bbwebservice.
-00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e34  .version = 1.0.4
+00000020: 0a76 6572 7369 6f6e 203d 2031 2e30 2e35  .version = 1.0.5
 00000030: 0d0a 6175 7468 6f72 203d 204c 756b 6173  ..author = Lukas
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 206c 756b 6173 6f67 7761 6c6b 6572 4067   lukasogwalker@g
 00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000070: 7074 696f 6e20 3d20 4120 6261 7265 2062  ption = A bare b
 00000080: 6f6e 6520 7765 6273 6572 7665 720d 0a6c  one webserver..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description
```

### Comparing `bbwebservice-1.0.4/src/bbwebservice.egg-info/PKG-INFO` & `bbwebservice-1.0.5/src/bbwebservice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbwebservice
-Version: 1.0.4
+Version: 1.0.5
 Summary: A bare bone webserver
 Author: Lukas
 Author-email: lukasogwalker@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

