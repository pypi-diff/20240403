# Comparing `tmp/heaserver-folders-aws-s3-1.0.9.tar.gz` & `tmp/heaserver-folders-aws-s3-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-folders-aws-s3-1.0.9.tar", last modified: Wed Feb  7 00:06:17 2024, max compression
+gzip compressed data, was "heaserver-folders-aws-s3-1.1.0.tar", last modified: Tue Apr  2 22:02:48 2024, max compression
```

## Comparing `heaserver-folders-aws-s3-1.0.9.tar` & `heaserver-folders-aws-s3-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.176981 heaserver-folders-aws-s3-1.0.9/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.9/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/.gitignore
--rw-rw-rw-   0        0        0     1664 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     6010 2024-02-07 00:06:17.175321 heaserver-folders-aws-s3-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4768 2024-02-07 00:04:52.000000 heaserver-folders-aws-s3-1.0.9/README.md
--rw-rw-rw-   0        0        0     1777 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/RELEASING.md
--rw-rw-rw-   0        0        0      658 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.117519 heaserver-folders-aws-s3-1.0.9/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.117519 heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.149232 heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/folderawss3integrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/folderawss3integrationtest/__init__.py
--rw-rw-rw-   0        0        0    37313 2024-02-06 02:51:18.000000 heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
--rw-rw-rw-   0        0        0    39341 2024-02-06 02:51:18.000000 heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
--rw-rw-rw-   0        0        0    29518 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/folderawss3integrationtest/test_all.py
--rw-rw-rw-   0        0        0      111 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/pytest.ini
--rw-rw-rw-   0        0        0      261 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/requirements_dev.txt
--rw-rw-rw-   0        0        0    14464 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-02-07 00:06:17.176981 heaserver-folders-aws-s3-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0     2473 2024-02-07 00:05:36.000000 heaserver-folders-aws-s3-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.119054 heaserver-folders-aws-s3-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.118547 heaserver-folders-aws-s3-1.0.9/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.158199 heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/__init__.py
--rw-rw-rw-   0        0        0   152432 2024-02-06 02:51:18.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/projectservice.py
--rw-rw-rw-   0        0        0   154860 2024-02-06 02:51:18.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/service.py
--rw-rw-rw-   0        0        0     8330 2024-01-21 23:25:35.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/util.py
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.159203 heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/wstl/
--rw-rw-rw-   0        0        0    34338 2024-02-06 21:01:41.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.174320 heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/
--rw-rw-rw-   0        0        0     6010 2024-02-07 00:06:17.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1196 2024-02-07 00:06:17.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-07 00:06:17.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-02-07 00:06:17.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-02-07 00:06:17.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-02-07 00:06:17.000000 heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.120084 heaserver-folders-aws-s3-1.0.9/tests/
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.120084 heaserver-folders-aws-s3-1.0.9/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.172287 heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/__init__.py
--rw-rw-rw-   0        0        0    36619 2024-02-06 02:51:18.000000 heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/folderawss3testcase.py
--rw-rw-rw-   0        0        0    37972 2024-02-06 02:51:18.000000 heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/projectawss3testcase.py
--rw-rw-rw-   0        0        0     2608 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/test_all.py
-drwxrwxrwx   0        0        0        0 2024-02-07 00:06:17.173320 heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/wstl/
--rw-rw-rw-   0        0        0    14496 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.749316 heaserver-folders-aws-s3-1.1.0/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1664 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     6441 2024-04-02 22:02:48.748291 heaserver-folders-aws-s3-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5199 2024-04-02 22:01:09.000000 heaserver-folders-aws-s3-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1777 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/RELEASING.md
+-rw-rw-rw-   0        0        0      658 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.696441 heaserver-folders-aws-s3-1.1.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.697472 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.721588 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/__init__.py
+-rw-rw-rw-   0        0        0    38029 2024-04-02 02:35:42.000000 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    40017 2024-04-02 02:36:47.000000 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py
+-rw-rw-rw-   0        0        0    30361 2024-04-02 04:31:30.000000 heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/test_all.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/pytest.ini
+-rw-rw-rw-   0        0        0      261 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0    14460 2024-03-22 02:50:09.000000 heaserver-folders-aws-s3-1.1.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-02 22:02:48.749316 heaserver-folders-aws-s3-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     2473 2024-04-02 21:57:36.000000 heaserver-folders-aws-s3-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.698503 heaserver-folders-aws-s3-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.698475 heaserver-folders-aws-s3-1.1.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.727736 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/__init__.py
+-rw-rw-rw-   0        0        0   153693 2024-04-02 21:01:46.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/projectservice.py
+-rw-rw-rw-   0        0        0   156242 2024-04-02 21:01:52.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/service.py
+-rw-rw-rw-   0        0        0     8385 2024-03-22 02:50:09.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/util.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.729783 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/wstl/
+-rw-rw-rw-   0        0        0    32616 2024-03-27 20:38:49.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.747225 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/
+-rw-rw-rw-   0        0        0     6441 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1196 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-02 22:02:48.000000 heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.699532 heaserver-folders-aws-s3-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.699532 heaserver-folders-aws-s3-1.1.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.744158 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:25.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/__init__.py
+-rw-rw-rw-   0        0        0    37295 2024-04-02 02:35:59.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/folderawss3testcase.py
+-rw-rw-rw-   0        0        0    38648 2024-04-02 02:36:18.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/projectawss3testcase.py
+-rw-rw-rw-   0        0        0     2608 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/test_all.py
+drwxrwxrwx   0        0        0        0 2024-04-02 22:02:48.745181 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/wstl/
+-rw-rw-rw-   0        0        0    14496 2023-12-18 20:10:59.000000 heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/wstl/all.json
```

### Comparing `heaserver-folders-aws-s3-1.0.9/Dockerfile` & `heaserver-folders-aws-s3-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.9/LICENSE` & `heaserver-folders-aws-s3-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.9/PKG-INFO` & `heaserver-folders-aws-s3-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.0.9
+Version: 1.1.0
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,22 +20,38 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.7
+Requires-Dist: heaserver~=1.1.2
 
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.0
+* Pass folder and project permissions back to clients.
+
+## Version 1.0.13
+* Changed presented bucket owner to system|aws.
+* Omitted shares from the properties template.
+
+## Version 1.0.12
+* Improved upload desktop object action message.
+
+## Version 1.0.11
+* Improved performance.
+
+## Version 1.0.10
+* Support getting the content of a folder as a zip file when the folder has files > 2GiB in size.
+
 ## Version 1.0.9
 * Prevent zip file corruption when getting the content of a folder.
 
 ## Version 1.0.8
 * Addressed issue where downloads start failing for all users if one user interrupts their download.
 
 ## Version 1.0.7
```

### Comparing `heaserver-folders-aws-s3-1.0.9/README.md` & `heaserver-folders-aws-s3-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,29 @@
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.0
+* Pass folder and project permissions back to clients.
+
+## Version 1.0.13
+* Changed presented bucket owner to system|aws.
+* Omitted shares from the properties template.
+
+## Version 1.0.12
+* Improved upload desktop object action message.
+
+## Version 1.0.11
+* Improved performance.
+
+## Version 1.0.10
+* Support getting the content of a folder as a zip file when the folder has files > 2GiB in size.
+
 ## Version 1.0.9
 * Prevent zip file corruption when getting the content of a folder.
 
 ## Version 1.0.8
 * Addressed issue where downloads start failing for all users if one user interrupts their download.
 
 ## Version 1.0.7
```

### Comparing `heaserver-folders-aws-s3-1.0.9/RELEASING.md` & `heaserver-folders-aws-s3-1.1.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.9/docker-entrypoint.sh` & `heaserver-folders-aws-s3-1.1.0/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py` & `heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/folderawss3testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,21 @@
             'description': None,
             'display_name': 'TestFolder',
             'id': 'VGVzdEZvbGRlci8=',
             'invites': [],
             'modified': None,
             'mime_type': 'application/x.item',
             'name': 'VGVzdEZvbGRlci8=',
-            'owner': user.NONE_USER,
-            'shares': [],
+            'owner': user.AWS_USER,
+            'shares': [{
+                'invite': None,
+                'permissions': ['COOWNER'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': 'system|all'
+            }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.folder.AWSS3ItemInFolder',
             'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
             'actual_object_id': 'VGVzdEZvbGRlci8=',
             'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlci8=',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
@@ -54,16 +59,21 @@
             'derived_from': [],
             'description': None,
             'display_name': 'TestFolder2',
             'id': 'VGVzdEZvbGRlcjIv',
             'invites': [],
             'modified': None,
             'name': 'VGVzdEZvbGRlcjIv',
-            'owner': user.NONE_USER,
-            'shares': [],
+            'owner': user.AWS_USER,
+            'shares': [{
+                'invite': None,
+                'permissions': ['COOWNER'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': 'system|all'
+            }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.folder.AWSS3ItemInFolder',
             'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
             'actual_object_id': 'VGVzdEZvbGRlcjIv',
             'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlcjIv',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
@@ -186,16 +196,21 @@
         'derived_from': [],
         'description': None,
         'display_name': 'TestFolder',
         'id': 'VGVzdEZvbGRlci8=',
         'invites': [],
         'modified': None,
         'name': 'VGVzdEZvbGRlci8=',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3Folder',
         'mime_type': 'application/x.folder',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder/',
@@ -207,16 +222,21 @@
             'derived_from': [],
             'description': None,
             'display_name': 'TestFolder2',
             'id': 'VGVzdEZvbGRlcjIv',
             'invites': [],
             'modified': None,
             'name': 'VGVzdEZvbGRlcjIv',
-            'owner': user.NONE_USER,
-            'shares': [],
+            'owner': user.AWS_USER,
+            'shares': [{
+                'invite': None,
+                'permissions': ['COOWNER'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': 'system|all'
+            }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.folder.AWSS3Folder',
             'mime_type': 'application/x.folder',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'TestFolder2/',
```

### Comparing `heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py` & `heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/projectawss3testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,21 @@
         'description': None,
         'display_name': 'TestProject',
         'id': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdC8=',
         'invites': [],
         'modified': None,
         'mime_type': 'application/x.item',
         'name': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdC8=',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3ItemInFolder',
         'actual_object_type_name': 'heaobject.project.AWSS3Project',
         'actual_object_id': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdC8=',
         'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3projects/VGVzdEZvbGRlci9UZXN0UHJvamVjdC8=',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestProject/',
@@ -87,16 +92,21 @@
         'derived_from': [],
         'description': None,
         'display_name': 'TestProject2',
         'id': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdDIv',
         'invites': [],
         'modified': None,
         'name': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdDIv',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3ItemInFolder',
         'actual_object_type_name': 'heaobject.project.AWSS3Project',
         'actual_object_id': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdDIv',
         'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3projects/VGVzdEZvbGRlci9UZXN0UHJvamVjdDIv',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject2/',
@@ -269,16 +279,21 @@
         'derived_from': [],
         'description': None,
         'display_name': 'TestProject',
         'id': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdC8=',
         'invites': [],
         'modified': None,
         'name': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdC8=',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.project.AWSS3Project',
         'mime_type': 'application/x.project',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject/',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder/TestProject/'
@@ -289,16 +304,21 @@
             'derived_from': [],
             'description': None,
             'display_name': 'TestProject2',
             'id': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdDIv',
             'invites': [],
             'modified': None,
             'name': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdDIv',
-            'owner': user.NONE_USER,
-            'shares': [],
+            'owner': user.AWS_USER,
+            'shares': [{
+                'invite': None,
+                'permissions': ['COOWNER'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': 'system|all'
+            }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.project.AWSS3Project',
             'mime_type': 'application/x.project',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject2/',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'TestFolder/TestProject2/'
```

### Comparing `heaserver-folders-aws-s3-1.0.9/integrationtests/heaserver/folderawss3integrationtest/test_all.py` & `heaserver-folders-aws-s3-1.1.0/integrationtests/heaserver/folderawss3integrationtest/test_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,20 +143,26 @@
         href2 = f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/{encode_key("TestFolder2/TestFolder/")}'
         async with self.client.get(href2, headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             expected = [{'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11', 'created': None,
                          'derived_by': None, 'derived_from': [], 'description': None, 'display_name': 'TestFolder',
                          'id': 'VGVzdEZvbGRlcjIvVGVzdEZvbGRlci8=', 'invites': [],
                          'key': 'TestFolder2/TestFolder/', 'mime_type': 'application/x.folder',
                          'modified': None, 'name': 'VGVzdEZvbGRlcjIvVGVzdEZvbGRlci8=',
-                         'owner': 'system|none',
+                         'owner': 'system|aws',
                          'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder2/TestFolder/',
-                         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/TestFolder/', 'shares': [],
+                         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/TestFolder/',
                          'source': 'AWS S3',
                          'source_detail': 'AWS S3',
-                         'type': 'heaobject.folder.AWSS3Folder'}]
+                         'type': 'heaobject.folder.AWSS3Folder',
+                         'shares': [{
+                            'invite': None,
+                            'permissions': ['COOWNER'],
+                            'type': 'heaobject.root.ShareImpl',
+                            'user': 'system|all'
+                         }]}]
             self._assert_equal_ordered(expected, await resp.json())
 
     async def test_copy_async(self):
         href = f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/{encode_key("TestFolder/")}/duplicatorasync'
         body = {'template':
             {'data': [
                 {'name': 'target',
@@ -173,20 +179,27 @@
         href2 = f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/{encode_key("TestFolder2/TestFolder/")}'
         async with self.client.get(href2, headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             expected = [{'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11', 'created': None,
                          'derived_by': None, 'derived_from': [], 'description': None, 'display_name': 'TestFolder',
                          'id': 'VGVzdEZvbGRlcjIvVGVzdEZvbGRlci8=', 'invites': [],
                          'key': 'TestFolder2/TestFolder/', 'mime_type': 'application/x.folder',
                          'modified': None, 'name': 'VGVzdEZvbGRlcjIvVGVzdEZvbGRlci8=',
-                         'owner': 'system|none',
+                         'owner': 'system|aws',
                          'path': '/arp-scale-2-cloud-bucket-with-tags11/TestFolder2/TestFolder/',
-                         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/TestFolder/', 'shares': [],
+                         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/TestFolder/',
                          'source': 'AWS S3',
                          'source_detail': 'AWS S3',
-                         'type': 'heaobject.folder.AWSS3Folder'}]
+                         'type': 'heaobject.folder.AWSS3Folder',
+                         'shares': [{
+                             'invite': None,
+                             'permissions': ['COOWNER'],
+                             'type': 'heaobject.root.ShareImpl',
+                             'user': 'system|all'
+                         }]
+                         }]
             self._assert_equal_ordered(expected, await resp.json())
 
 
 class TestDeleteItem(AWSS3ItemTestCase, DeleteMixin):
     pass
 
 
@@ -426,17 +439,23 @@
         href2 = f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3projects/{encode_key("TestFolder/TestProject2/")}'
         async with self.client.get(href2, headers={hdrs.ACCEPT: nvpjson.MIME_TYPE}) as resp:
             expected = [{'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11', 'created': None,
                          'derived_by': None, 'derived_from': [], 'description': None, 'display_name': 'TestProject2',
                          'id': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdDIv', 'invites': [],
                          'key': 'TestFolder/TestProject2/', 'mime_type': 'application/x.project',
                          'modified': None, 'name': 'VGVzdEZvbGRlci9UZXN0UHJvamVjdDIv',
-                         'owner': 'system|none',
-                         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject2/', 'shares': [],
-                         'source': 'AWS S3', 'source_detail': 'AWS S3', 'type': 'heaobject.project.AWSS3Project'}]
+                         'owner': 'system|aws',
+                         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/TestProject2/',
+                         'source': 'AWS S3', 'source_detail': 'AWS S3', 'type': 'heaobject.project.AWSS3Project',
+                         'shares': [{
+                            'invite': None,
+                            'permissions': ['COOWNER'],
+                            'type': 'heaobject.root.ShareImpl',
+                            'user': 'system|all'
+                        }]}]
             self._assert_equal_ordered(expected, await resp.json())
 
     async def test_not_folder(self):
         href = f'/volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/{encode_key("TestFolder/TestProject/")}'
         async with self.client.get(href) as resp:
             if resp.status != 404:
                 self.fail('The folder API returned a project')
```

### Comparing `heaserver-folders-aws-s3-1.0.9/run-swaggerui.py` & `heaserver-folders-aws-s3-1.1.0/run-swaggerui.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
                           (post, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/{folder_id}/items',
                            service.projectservice.post_item_in_project),
                           (delete, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/{folder_id}/items/{id}',
                            service.projectservice.delete_item),
                           (get, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/{id}', service.projectservice.get_project),
                           (options, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/{id}',
                            service.projectservice.get_project_options),
-                          (get, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/', service.projectservice.get_all_projects),
+                          (get, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/', service.projectservice.get_projects),
                           (get, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/byname/{name}',
                            service.projectservice.get_project_by_name),
                           (get, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/{id}/presignedurl', service.projectservice.get_presigned_url_form),
                           (post, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/{id}/presignedurl', service.projectservice.post_presigned_url_form),
                           (post, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/', service.projectservice.post_project),
                           (view, '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/{id}/opener',
                            service.projectservice.get_project_opener),
```

### Comparing `heaserver-folders-aws-s3-1.0.9/setup.py` & `heaserver-folders-aws-s3-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaserver-folders-aws-s3',
-                 version='1.0.9',
+                 version='1.1.0',
                  description='The HEA AWS S3 bucket folder service.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
                  package_dir={'': 'src'},
                  packages=['heaserver.folderawss3'],
                  package_data={'heaserver.folderawss3': ['wstl/*.json']},
                  install_requires=[
-                     'heaserver~=1.0.7'
+                     'heaserver~=1.1.2'
                  ],
                  classifiers=[
                      'Development Status :: 5 - Production/Stable',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: Apache Software License',
                      'Framework :: AsyncIO',
```

### Comparing `heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/projectservice.py` & `heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/projectservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import asyncio
 from functools import partial
+from itertools import chain
 import logging
 from heaserver.service.runner import routes
 from heaserver.service import response
 from aiohttp import web, hdrs
 from heaserver.service.wstl import action
 from heaserver.service.db import awsservicelib, mongo, aws
 from heaserver.service.activity import DesktopObjectActionLifecycle
@@ -16,18 +17,18 @@
 from heaserver.service.util import queued_processing
 from heaobject.root import DesktopObjectDict
 from heaobject.awss3key import encode_key, split, KeyDecodeException, join, decode_key, is_object_in_folder, parent
 from heaobject.activity import Status, Activity
 from heaobject.folder import AWSS3ItemInFolder, AWSS3Folder
 from heaobject.project import AWSS3Project
 from heaobject.data import AWSS3FileObject, ClipboardData
-from heaobject.user import NONE_USER
+from heaobject.user import NONE_USER, AWS_USER, ALL_USERS
 from heaobject.error import DeserializeException
 from heaobject.aws import S3StorageClass
-from heaobject.root import DesktopObject
+from heaobject.root import DesktopObject, ShareImpl, Permission
 from botocore.exceptions import ClientError as BotoClientError, ParamValidationError
 from mypy_boto3_s3 import S3Client
 from typing import Any
 from datetime import datetime
 from json import JSONDecodeError
 from yarl import URL
 from io import BytesIO
@@ -110,33 +111,34 @@
             if folder_key is None:
                 # We couldn't decode the folder_id, and we need to check if the user can access the bucket in order to
                 # decide which HTTP status code to respond with (Forbidden vs Not Found).
                 async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3:
                     return await awsservicelib.return_bucket_status_or_not_found(bucket_name, loop, s3)
             logger.debug('Getting all items in project %s in bucket %s', folder_key, bucket_name)
             actual_object_uri_base = URL('volumes') / volume_id / 'buckets' / bucket_name
-            owner = request.headers.get(SUB, NONE_USER)
+            owner = AWS_USER
             file_type_name = AWSS3FileObject.get_type_name()
         except BotoClientError as e:
             return awsservicelib.handle_client_error(e)
         except ParamValidationError as e:
             return response.status_bad_request(str(e))
         async with DesktopObjectActionLifecycle(request,
                                                 code='hea-get',
                                                 description=f'Listing all items in {awsservicelib._activity_object_display_name(bucket_name, folder_key)}',
                                                 activity_cb=publish_desktop_object) as activity:
             cache_key = (sub, volume_id, bucket_name, folder_id_, None, 'items')
             cached_value = request.app[HEA_CACHE].get(cache_key)
-            if False:  #cached_value:
+            if cached_value:
                 logger.debug('Getting cached value for %s: %s', cache_key, cached_value)
-                return await response.get_all(request, cached_value)
+                return await response.get_all(request, cached_value[0], permissions=cached_value[1])
             else:
                 async with mongo.MongoContext(request=request) as mongo_client:
                     try:
-                        folders: list[AWSS3ItemInFolder] = []
+                        folders: list[DesktopObjectDict] = []
+                        permissions: list[list[Permission]] = []
                         folders_actual_object_uri_base = actual_object_uri_base / 'awss3folders'
                         projects_actual_object_uri_base = actual_object_uri_base / 'awss3projects'
                         files_actual_object_uri_base = actual_object_uri_base / 'awss3files'
                         new_object_uri_prefix = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/'
                         item = AWSS3ItemInFolder()
                         async def get_metadata() -> dict[str, DesktopObjectDict]:
                             metadata = {}
@@ -189,22 +191,27 @@
                                     else:
                                         item.actual_object_type_name = None
                                         item.actual_object_uri = None
                                     item.size = None
                                     item.storage_class = None
                                     item.source = AWS_S3
                                     item.source_detail = AWS_S3
+                                share = ShareImpl()
+                                share.user = ALL_USERS
+                                share.permissions = [Permission.COOWNER]
+                                item.shares = [share]
+                                permissions.append(item.get_permissions(sub))
                                 folders.append(item.to_dict())
                         await metadata_task
                         activity.new_object_uri = new_object_uri_prefix
                         activity.new_object_type_name = AWSS3Project.get_type_name()
                         activity.new_volume_id = volume_id
-                        request.app[HEA_CACHE][cache_key] = folders
-                        for folder_item_dict in folders:
-                            request.app[HEA_CACHE][(sub, volume_id, bucket_name, folder_id_, folder_item_dict['id'], 'items')] = folder_item_dict
+                        request.app[HEA_CACHE][cache_key] = (folders, permissions)
+                        for folder_item_dict, perms in zip(folders, permissions):
+                            request.app[HEA_CACHE][(sub, volume_id, bucket_name, folder_id_, folder_item_dict['id'], 'items')] = (folder_item_dict, perms)
                         return await response.get_all(request, folders)
                     except BotoClientError as e:
                         activity.status = Status.FAILED
                         return awsservicelib.handle_client_error(e)
                     except ParamValidationError as e:
                         activity.status = Status.FAILED
                         return response.status_bad_request(str(e))
@@ -287,45 +294,49 @@
 
     async with DesktopObjectActionLifecycle(request=request,
                                             code='hea-get',
                                             description=f'Getting item {awsservicelib._activity_object_display_name(bucket_name, decoded_key)}',
                                             activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, volume_id, bucket_name, id_, 'items')
         if cached_value := request.app[HEA_CACHE].get(cache_key):
-            return await response.get(request, cached_value)
+            return await response.get(request, cached_value[0], permissions=cached_value[1])
         else:
             async with mongo.MongoContext(request=request) as mongo_client:
                 async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3:
                     try:
                         loop = asyncio.get_running_loop()
 
                         if folder_or_item_not_found:
                             activity.status = Status.FAILED
                             return await awsservicelib.return_bucket_status_or_not_found(bucket_name, loop, s3)
 
                         logger.debug('Getting item %s in folder %s in bucket %s', decoded_key, decoded_folder_key, bucket_name)
                         response_ = await loop.run_in_executor(None, partial(s3.list_objects_v2, Bucket=bucket_name, Prefix=decoded_key,
                                                                             MaxKeys=1, Delimiter='/', OptionalObjectAttributes=['RestoreStatus']))
-                        from itertools import chain
+
                         for obj in chain(response_.get('CommonPrefixes', []), response_.get('Contents', [])):
                             id_ = obj['Key'] if 'Key' in obj else obj['Prefix']
                             is_folder_ = awsservicelib.is_folder(id_)
                             id_encoded = encode_key(id_)
                             logger.debug('Found item %s in bucket %s', id_, bucket_name)
 
                             item = AWSS3ItemInFolder()
                             item.id = id_encoded
                             if not is_folder_:
                                 item.modified = obj.get('LastModified')
                                 item.created = obj.get('LastModified')
-                            item.owner = request.headers.get(SUB, NONE_USER)
+                            item.owner = AWS_USER
                             item.folder_id = folder_id_
                             item.actual_object_id = id_encoded
                             item.bucket_id = bucket_name
                             item.volume_id = volume_id
+                            share = ShareImpl()
+                            share.user = ALL_USERS
+                            share.permissions = [Permission.COOWNER]
+                            item.shares = [share]
                             if is_folder_:
                                 metadata_dict = await mongo_client.get_admin(MONGODB_AWS_S3_FOLDER_METADATA_COLLECTION, {'bucket_id': bucket_name, 'encoded_key': id_encoded})
                                 if not metadata_dict or metadata_dict['actual_object_type_name'] == AWSS3Folder.get_type_name():
                                     item.actual_object_uri = str(actual_object_uri_base / 'awss3folders' / id_encoded)
                                     item.actual_object_type_name = AWSS3Folder.get_type_name()
                                 elif metadata_dict['actual_object_type_name'] == AWSS3Project.get_type_name():
                                     item.actual_object_type_name = AWSS3Project.get_type_name()
@@ -339,16 +350,17 @@
                                 item.storage_class = S3StorageClass[obj['StorageClass']]
                                 set_file_source(obj, item)
                             activity.new_object_id = id_
                             activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/{folder_id_}/items/{id_}'
                             activity.new_object_type_name = AWSS3ItemInFolder.get_type_name()
                             activity.new_volume_id = volume_id
                             item_dict = item.to_dict()
-                            request.app[HEA_CACHE][cache_key] = item_dict
-                            return await response.get(request, item_dict)
+                            perms = item.get_permissions(sub)
+                            request.app[HEA_CACHE][cache_key] = (item_dict, perms)
+                            return await response.get(request, item_dict, permissions=perms)
                         return await response.get(request, None)
                     except BotoClientError as e:
                         activity.status = Status.FAILED
                         return awsservicelib.handle_client_error(e)
 
 @routes.route('OPTIONS', '/volumes/{volume_id}/buckets/{bucket_id}/awss3projects/{folder_id}/items/{id}')
 async def get_item_options(request: web.Request) -> web.Response:
@@ -2631,44 +2643,46 @@
     async with mongo.MongoContext(request) as mongo_client:
         async with DesktopObjectActionLifecycle(request=request,
                                                 code='hea-get',
                                                 description=f'Listing all projects in bucket {bucket_name}',
                                                 activity_cb=publish_desktop_object) as activity:
             cache_key = (sub, volume_id, bucket_name, None, 'actual')
             if cached_value := request.app[HEA_CACHE].get(cache_key):
-                return await response.get_all(request, cached_value)
+                return await response.get_all(request, cached_value[0], permissions=cached_value[1])
             else:
                 async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3:
                     try:
                         loop = asyncio.get_running_loop()
                         logger.debug('Getting all projects from bucket %s', bucket_name)
-                        folder_dicts = []
+                        folders: list[DesktopObject] = []
                         async for obj in awsservicelib.list_objects(s3, bucket_name, loop=loop):
                             logger.debug('Checking possible project %s in bucket %s', obj, bucket_name)
                             key = obj['Key']
                             if awsservicelib.is_folder(key):
                                 encoded_key = encode_key(key)
                                 logger.debug('Project %s in bucket %s is a folder', key, bucket_name)
                                 description = await _get_description(s3, bucket_name, key)
-                                folder_dict = _new_project(bucket_name, obj, encoded_key, request, description=description)
-                                folder_dicts.append(folder_dict.to_dict())
+                                folder_ = _new_project(bucket_name, obj, encoded_key, request, description=description)
+                                folders.append(folder_)
                         folder_metadata = {}
                         async for metadata_dict in mongo_client.get_all_admin(MONGODB_AWS_S3_FOLDER_METADATA_COLLECTION, {'bucket_id': bucket_name}):
                             folder_metadata[metadata_dict['encoded_key']] = metadata_dict
-                        real_folder_dicts = []
-                        for folder_dict in folder_dicts:
-                            if (obj_metadata_ := folder_metadata.get(folder_dict['id'])) is None or obj_metadata_['actual_object_type_name'] == AWSS3Project.get_type_name():
-                                real_folder_dicts.append(folder_dict)
+                        real_folder_dicts: list[DesktopObjectDict] = []
+                        permissions: list[list[Permission]] = []
+                        for folder_ in folders:
+                            if (obj_metadata_ := folder_metadata.get(folder_.id)) is None or obj_metadata_['actual_object_type_name'] == AWSS3Project.get_type_name():
+                                real_folder_dicts.append(folder_.to_dict())
+                                permissions.append(folder_.get_permissions(sub))
                         activity.new_volume_id = volume_id
                         activity.new_object_type_name = AWSS3Project.get_type_name()
                         activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/'
-                        request.app[HEA_CACHE][cache_key] = real_folder_dicts
+                        request.app[HEA_CACHE][cache_key] = (real_folder_dicts, permissions)
                         for fd in real_folder_dicts:
                             request.app[HEA_CACHE][(sub, volume_id, bucket_name, fd['id'], 'actual')] = fd
-                        return await response.get_all(request, real_folder_dicts)
+                        return await response.get_all(request, real_folder_dicts, permissions=permissions)
                     except BotoClientError as e:
                         activity.status = Status.FAILED
                         return awsservicelib.handle_client_error(e)
                     except ParamValidationError as e:
                         activity.status = Status.FAILED
                         return response.status_not_found()
 
@@ -3040,14 +3054,15 @@
         - $ref: '#/components/parameters/id'
     responses:
       '300':
         $ref: '#/components/responses/300'
       '404':
         $ref: '#/components/responses/404'
     """
+    sub = request.headers.get(SUB, NONE_USER)
     volume_id = request.match_info['volume_id']
     bucket_name = request.match_info['bucket_id']
     folder_name = request.match_info['id']
     try:
         folder_key = awsservicelib.decode_folder(folder_name)
     except KeyDecodeException as e:
         return response.status_not_found()
@@ -3131,15 +3146,15 @@
                                             code='hea-get',
                                             description=f'Accessing {awsservicelib._activity_object_display_name(bucket_name, folder_key)}',
                                             activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, volume_id, bucket_name, folder_name, 'actual')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value:
             logger.debug('Getting cached value for %s: %s', cache_key, cached_value)
-            return await response.get_all(request, cached_value)
+            return await response.get_multiple_choices(request)
         else:
             async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3_client:
                 try:
                     folder, is_folder = await asyncio.gather(_has_project_helper(s3_client, request),
                                                             _is_project(request, volume_id, bucket_name, folder_name))
                     if not folder or not is_folder:
                         return response.status_not_found()
@@ -3218,30 +3233,31 @@
 
     async with DesktopObjectActionLifecycle(request=request,
                                             code='hea-get',
                                             description=f'Accessing {awsservicelib._activity_object_display_name(bucket_name, project_key)}',
                                             activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, volume_id, bucket_name, project_id, 'actual')
         if cached_value := request.app[HEA_CACHE].get(cache_key):
-            return await response.get(request, cached_value)
+            return await response.get(request, cached_value[0], permissions=cached_value[1])
         else:
             async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3_client:
                 try:
-                    is_project, project  = await asyncio.gather(_is_project(request, volume_id, bucket_name, project_id),
+                    is_project, project = await asyncio.gather(_is_project(request, volume_id, bucket_name, project_id),
                                                                 _get_project_helper(s3_client, request))
                     if not is_project or not project:
                         activity.status = Status.FAILED
                         return await response.get(request, None)
                     activity.new_object_id = project_id
                     activity.new_object_type_name = AWSS3Project.get_type_name()
                     activity.new_volume_id = volume_id
                     activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/{project_id}'
                     project_dict = project.to_dict()
-                    request.app[HEA_CACHE][cache_key] = project_dict
-                    return await response.get(request, project_dict)
+                    perms = project.get_permissions(sub)
+                    request.app[HEA_CACHE][cache_key] = (project_dict, perms)
+                    return await response.get(request, project_dict, permissions=perms)
                 except BotoClientError as e:
                     activity.status = Status.FAILED
                     return awsservicelib.handle_client_error(e)
                 except web.HTTPClientError as e:
                     activity.status = Status.FAILED
                     return e
 
@@ -3329,19 +3345,23 @@
             return False
     return True
 
 def _new_project(bucket_name: str, contents: dict[str, Any], encoded_key: str,
                 request: web.Request, description: str | None = None) -> AWSS3Project:
     project = AWSS3Project()
     project.id = encoded_key
-    project.owner = request.headers.get(SUB, NONE_USER)
+    project.owner = AWS_USER
     project.bucket_id = bucket_name
     project.source = AWS_S3
     project.source_detail = AWS_S3
     project.description = description
+    share = ShareImpl()
+    share.user = ALL_USERS
+    share.permissions = [Permission.COOWNER]
+    project.shares = [share]
     return project
 
 async def _get_project_move_template(request: web.Request) -> web.Response:
     logger = logging.getLogger(__name__)
     try:
         return await _get_project(request)
     except KeyDecodeException as e:
```

### Comparing `heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/service.py` & `heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 from heaserver.service.sources import AWS_S3
 from heaserver.service.activity import DesktopObjectActionLifecycle
 from heaserver.service.util import queued_processing
 from heaobject.awss3key import KeyDecodeException, decode_key, encode_key, join, is_object_in_folder
 from heaobject.folder import AWSS3ItemInFolder, AWSS3Folder
 from heaobject.project import AWSS3Project
 from heaobject.data import AWSS3FileObject, ClipboardData
-from heaobject.user import NONE_USER
+from heaobject.user import NONE_USER, AWS_USER, ALL_USERS
 from heaobject.aws import S3StorageClass
 from heaobject.awss3key import parent
 from heaobject.error import DeserializeException
-from heaobject.root import DesktopObjectDict, DesktopObject
+from heaobject.root import DesktopObjectDict, DesktopObject, ShareImpl, Permission
 from heaobject.activity import Activity
 from aiohttp import web
 from typing import Any
 from aiohttp.client_exceptions import ClientError
 from aiohttp import hdrs
 from botocore.exceptions import ParamValidationError, ClientError as BotoClientError
 from yarl import URL
@@ -134,34 +134,35 @@
             if folder_key is None:
                 # We couldn't decode the folder_id, and we need to check if the user can access the bucket in order to
                 # decide which HTTP status code to respond with (Forbidden vs Not Found).
                 async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3:
                     return await awsservicelib.return_bucket_status_or_not_found(bucket_name, loop, s3)
             logger.debug('Getting all items in folder %s in bucket %s', folder_key, bucket_name)
             actual_object_uri_base = URL('volumes') / volume_id / 'buckets' / bucket_name
-            owner = request.headers.get(SUB, NONE_USER)
+            owner = AWS_USER
             file_type_name = AWSS3FileObject.get_type_name()
         except BotoClientError as e:
             return awsservicelib.handle_client_error(e)
         except ParamValidationError as e:
             return response.status_bad_request(str(e))
 
         async with DesktopObjectActionLifecycle(request,
                                                 code='hea-get',
                                                 description=f'Listing all items in {awsservicelib._activity_object_display_name(bucket_name, folder_key)}',
                                                 activity_cb=publish_desktop_object) as activity:
             cache_key = (sub, volume_id, bucket_name, folder_id_, None, 'items')
             cached_value = request.app[HEA_CACHE].get(cache_key)
-            if False:  # cached_value:
+            if cached_value:
                 logger.debug('Getting cached value for %s: %s', cache_key, cached_value)
-                return await response.get_all(request, cached_value)
+                return await response.get_all(request, cached_value[0], permissions=cached_value[1])
             else:
                 async with mongo.MongoContext(request=request) as mongo_client:
                     try:
-                        folders: list[AWSS3ItemInFolder] = []
+                        folders: list[DesktopObjectDict] = []
+                        permissions: list[list[Permission]] = []
                         folders_actual_object_uri_base = actual_object_uri_base / 'awss3folders'
                         projects_actual_object_uri_base = actual_object_uri_base / 'awss3projects'
                         files_actual_object_uri_base = actual_object_uri_base / 'awss3files'
                         new_object_uri_prefix = f'volumes/{volume_id}/buckets/{bucket_name}/awss3folders/'
                         folder_type_name = AWSS3Folder.get_type_name()
                         project_type_name = AWSS3Project.get_type_name()
                         item = AWSS3ItemInFolder()
@@ -200,14 +201,18 @@
                                     item.modified = None
                                     item.created = None
                                 item.owner = owner
                                 item.actual_object_id = actual_id
                                 item.folder_id = folder_id_
                                 item.bucket_id = bucket_name
                                 item.volume_id = volume_id
+                                share = ShareImpl()
+                                share.user = ALL_USERS
+                                share.permissions = [Permission.COOWNER]
+                                item.shares = [share]
                                 if not is_folder_:
                                     item.actual_object_uri = str(files_actual_object_uri_base / item.actual_object_id)
                                     item.actual_object_type_name = file_type_name
                                     item.size = obj['Size']
                                     item.storage_class = S3StorageClass[obj['StorageClass']]
                                     set_file_source(obj, item)
                                 else:
@@ -227,24 +232,25 @@
                                     else:
                                         item.actual_object_type_name = None
                                         item.actual_object_uri = None
                                     item.size = None
                                     item.storage_class = None
                                     item.source = AWS_S3
                                     item.source_detail = AWS_S3
+                                permissions.append(item.get_permissions(sub))
                                 folders.append(item.to_dict())
                         await metadata_task
                         activity.new_object_uri = new_object_uri_prefix
                         activity.new_object_type_name = folder_type_name
                         activity.new_volume_id = volume_id
-                        request.app[HEA_CACHE][cache_key] = folders
-                        for folder_item_dict in folders:
+                        request.app[HEA_CACHE][cache_key] = (folders, permissions)
+                        for folder_item_dict, perms in zip(folders, permissions):
                             request.app[HEA_CACHE][(sub, volume_id, bucket_name, folder_id_, folder_item_dict['id'],
-                                                    'items')] = folder_item_dict
-                        return await response.get_all(request, folders)
+                                                    'items')] = (folder_item_dict, perms)
+                        return await response.get_all(request, folders, permissions=permissions)
                     except BotoClientError as e:
                         activity.status = Status.FAILED
                         return awsservicelib.handle_client_error(e)
                     except ParamValidationError as e:
                         activity.status = Status.FAILED
                         return response.status_bad_request(str(e))
 
@@ -489,15 +495,15 @@
 
     async with DesktopObjectActionLifecycle(request=request,
                                             code='hea-get',
                                             description=f'Getting item {awsservicelib._activity_object_display_name(bucket_name, decoded_key)}',
                                             activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, volume_id, bucket_name, id_, 'items')
         if cached_value := request.app[HEA_CACHE].get(cache_key):
-            return await response.get(request, cached_value)
+            return await response.get(request, cached_value[0], permissions=cached_value[1])
         else:
             async with mongo.MongoContext(request=request) as mongo_client:
                 async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3:
                     try:
                         loop = asyncio.get_running_loop()
 
                         if folder_or_item_not_found:
@@ -519,19 +525,23 @@
                             logger.debug('Found item %s in bucket %s', id_, bucket_name)
 
                             item = AWSS3ItemInFolder()
                             item.id = id_encoded
                             if not is_folder_:
                                 item.modified = obj.get('LastModified')
                                 item.created = obj.get('LastModified')
-                            item.owner = request.headers.get(SUB, NONE_USER)
+                            item.owner = AWS_USER
                             item.folder_id = folder_id_
                             item.actual_object_id = id_encoded
                             item.bucket_id = bucket_name
                             item.volume_id = volume_id
+                            share = ShareImpl()
+                            share.user = ALL_USERS
+                            share.permissions = [Permission.COOWNER]
+                            item.shares = [share]
                             if is_folder_:
                                 metadata_dict = await mongo_client.get_admin(MONGODB_AWS_S3_FOLDER_METADATA_COLLECTION,
                                                                              {'bucket_id': bucket_name,
                                                                               'encoded_key': id_encoded})
                                 if not metadata_dict or metadata_dict[
                                     'actual_object_type_name'] == AWSS3Folder.get_type_name():
                                     item.actual_object_uri = str(actual_object_uri_base / 'awss3folders' / id_encoded)
@@ -548,16 +558,17 @@
                                 item.storage_class = S3StorageClass[obj['StorageClass']]
                                 set_file_source(obj, item)
                             activity.new_object_id = id_
                             activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3projects/{folder_id_}/items/{id_}'
                             activity.new_object_type_name = AWSS3ItemInFolder.get_type_name()
                             activity.new_volume_id = volume_id
                             item_dict = item.to_dict()
-                            request.app[HEA_CACHE][cache_key] = item_dict
-                            return await response.get(request, item_dict)
+                            perms = item.get_permissions(sub)
+                            request.app[HEA_CACHE][cache_key] = (item_dict, perms)
+                            return await response.get(request, item_dict, permissions=perms)
                         return await response.get(request, None)
                     except BotoClientError as e:
                         activity.status = Status.FAILED
                         return awsservicelib.handle_client_error(e)
 
 
 @routes.get('/volumes/{volume_id}/buckets/{bucket_id}/awss3folders/{id}/duplicator')
@@ -1729,15 +1740,15 @@
     except KeyDecodeException:
         decoded_folder_id = None
     if not await _is_folder(request, volume_id, bucket_id, folder_id):
         return response.status_not_found()
 
     async with DesktopObjectActionLifecycle(request=request,
                                             code='hea-create',
-                                            description=f'Creating item {obj.display_name} in bucket {bucket_id}',
+                                            description=f'Uploading {obj.display_name} into bucket {bucket_id}',
                                             activity_cb=publish_desktop_object) as activity:
         async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3_client:
             loop = asyncio.get_running_loop()
             try:
                 if decoded_folder_id is None:
                     await loop.run_in_executor(None, partial(s3_client.head_bucket, Bucket=bucket_id))
                     return response.status_not_found()
@@ -1746,15 +1757,16 @@
                 content_id = f"{encode_key(obj_name)}/content"
                 # check if item exists, if not throws an exception
                 await loop.run_in_executor(None, partial(s3_client.head_object, Bucket=bucket_id, Key=obj_name))
                 return response.status_ok(headers={hdrs.LOCATION: f"/{url}/{content_id}"})
             except BotoClientError as e:
                 error_code = e.response['Error']['Code']
                 if error_code == awsservicelib.CLIENT_ERROR_404:  # file metadata doesn't exist
-                    await loop.run_in_executor(None, partial(s3_client.put_object, Bucket=bucket_id, Key=obj_name))
+                    await loop.run_in_executor(None, partial(s3_client.put_object, Bucket=bucket_id,
+                                                             Key=obj_name, StorageClass=obj.storage_class.name))
                     request.app[HEA_CACHE].pop((sub, volume_id, bucket_id, folder_id, None, 'items'), None)
                     request.app[HEA_CACHE].pop((sub, volume_id, bucket_id, folder_id, obj.name, 'items'), None)
                     request.app[HEA_CACHE].pop((sub, volume_id, bucket_id, None, 'actual'), None)
                     request.app[HEA_CACHE].pop((sub, volume_id, bucket_id, obj.name, 'actual'), None)
                     return await response.post(request, f"{encode_key(obj_name)}/content", url)
                 elif error_code == awsservicelib.CLIENT_ERROR_NO_SUCH_BUCKET:
                     activity.status = Status.FAILED
@@ -2790,38 +2802,42 @@
             if cached_value := request.app[HEA_CACHE].get(cache_key):
                 return await response.get_all(request, cached_value)
             else:
                 async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3:
                     try:
                         loop = asyncio.get_running_loop()
                         logger.debug('Getting all folders from bucket %s', bucket_name)
-                        folder_dicts = []
+
+                        folders: list[DesktopObject] = []
                         async for obj in awsservicelib.list_objects(s3, bucket_name, loop=loop):
                             key = obj['Key']
                             if awsservicelib.is_folder(key):
                                 encoded_key = encode_key(key)
                                 if logger.getEffectiveLevel() == logging.DEBUG:
                                     logger.debug('Found possible folder %s in bucket %s', key[:-1], bucket_name)
-                                folder_dicts.append(_new_folder(bucket_name, obj, encoded_key, request).to_dict())
+                                folder = _new_folder(bucket_name, obj, encoded_key, request)
+                                folders.append(folder)
                         folder_metadata = {}
                         async for metadata_dict in mongo_client.get_all_admin(MONGODB_AWS_S3_FOLDER_METADATA_COLLECTION,
                                                                               {'bucket_id': bucket_name}):
                             folder_metadata[metadata_dict['encoded_key']] = metadata_dict
-                        real_folder_dicts = []
-                        for folder_dict in folder_dicts:
-                            if (obj_metadata_ := folder_metadata.get(folder_dict['id'])) is None or obj_metadata_[
-                                'actual_object_type_name'] == AWSS3Folder.get_type_name():
-                                real_folder_dicts.append(folder_dict)
+                        permissions: list[list[Permission]] = []
+                        real_folder_dicts: list[DesktopObjectDict] = []
+                        for folder in folders:
+                            if (obj_metadata_ := folder_metadata.get(folder.id)) is None or \
+                                obj_metadata_['actual_object_type_name'] == AWSS3Folder.get_type_name():
+                                real_folder_dicts.append(folder.to_dict())
+                                permissions.append(folder.get_permissions(sub))
                         activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3folders/'
                         activity.new_volume_id = volume_id
                         activity.new_object_type_name = AWSS3Folder.get_type_name()
                         request.app[HEA_CACHE][cache_key] = real_folder_dicts
                         for fd in real_folder_dicts:
                             request.app[HEA_CACHE][(sub, volume_id, bucket_name, fd['id'], 'actual')] = fd
-                        return await response.get_all(request, real_folder_dicts)
+                        return await response.get_all(request, real_folder_dicts, permissions=permissions)
                     except BotoClientError as e:
                         activity.status = Status.FAILED
                         return awsservicelib.handle_client_error(e)
                     except ParamValidationError as e:
                         activity.status = Status.FAILED
                         return response.status_not_found()
 
@@ -3298,15 +3314,15 @@
                                             code='hea-get',
                                             description=f'Accessing {awsservicelib._activity_object_display_name(bucket_name, folder_key)}',
                                             activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, volume_id, bucket_name, folder_name, 'actual')
         cached_value = request.app[HEA_CACHE].get(cache_key)
         if cached_value:
             logger.debug('Getting cached value for %s: %s', cache_key, cached_value)
-            return await response.get_all(request, cached_value)
+            return await response.get_multiple_choices(request)
         else:
             logger.debug('Going to S3 for %s', cache_key)
             async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3_client:
                 try:
                     folder, is_folder = await asyncio.gather(_has_folder_helper(s3_client, request),
                                                              _is_folder(request, volume_id, bucket_name, folder_name))
                     if not folder or not is_folder:
@@ -3358,48 +3374,53 @@
     async with DesktopObjectActionLifecycle(request=request,
                                             code='hea-get',
                                             description=f'Accessing {awsservicelib._activity_object_display_name(bucket_name, folder_key)}',
                                             activity_cb=publish_desktop_object) as activity:
         cache_key = (sub, volume_id, bucket_name, folder_name, 'actual')
         if cached_value := request.app[HEA_CACHE].get(cache_key):
             logger.debug('Getting cached value for %s', cache_key)
-            return await response.get(request, cached_value)
+            return await response.get(request, cached_value[0], permissions=cached_value[1])
         else:
             async with aws.S3ClientContext(request=request, volume_id=volume_id) as s3_client:
                 try:
                     folder, is_folder = await asyncio.gather(_get_folder_helper(s3_client, request),
                                                              _is_folder(request, volume_id, bucket_name, folder_name))
                     if not is_folder:
                         logger.debug('No folder with id or name %s', folder_name)
                         activity.status = Status.FAILED
                         return await response.get(request, None)
                     activity.new_volume_id = volume_id
                     activity.new_object_id = folder_name
                     activity.new_object_type_name = AWSS3Folder.get_type_name()
                     activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}/awss3folders/{folder_name}'
                     folder_dict = folder.to_dict()
+                    perms = folder.get_permissions(sub)
                     logger.debug('Setting cache for %s', cache_key)
-                    request.app[HEA_CACHE][cache_key] = folder_dict
-                    return await response.get(request, folder_dict)
+                    request.app[HEA_CACHE][cache_key] = (folder_dict, perms)
+                    return await response.get(request, folder_dict, permissions=perms)
                 except BotoClientError as e:
                     activity.status = Status.FAILED
                     return awsservicelib.handle_client_error(e)
                 except web.HTTPClientError as e:
                     activity.status = Status.FAILED
                     return e
 
 
 def _new_folder(bucket_name: str, obj: dict[str, Any], encoded_key: str,
-                request: web.Request) -> AWSS3Folder:
+                request: web.Request, sub = NONE_USER) -> AWSS3Folder:
     folder = AWSS3Folder()
     folder.id = encoded_key
-    folder.owner = request.headers.get(SUB, NONE_USER)
+    folder.owner = AWS_USER
     folder.bucket_id = bucket_name
     folder.source = AWS_S3
     folder.source_detail = AWS_S3
+    share = ShareImpl()
+    share.user = ALL_USERS
+    share.permissions = [Permission.COOWNER]
+    folder.shares = [share]
     return folder
 
 
 async def _get_folder_helper(s3_client: S3Client, request: web.Request) -> AWSS3Folder:
     logger = logging.getLogger(__name__)
     try:
         bucket_name = request.match_info['bucket_id']
```

### Comparing `heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/util.py` & `heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
                     folder = obj['Key'].removeprefix(folder_key)
                     if not folder:
                         continue
                     if obj['StorageClass'] in (S3StorageClass.STANDARD.name, S3StorageClass.GLACIER_IR.name)\
                         or ((restore:= obj.get('RestoreStatus')) and restore.get('RestoreExpiryDate')):
                         filename = _fill_in_folders_with_no_name(folder)
                         zinfo = ZipInfo(filename=filename, date_time=obj['LastModified'].timetuple()[:6])
+                        zinfo.file_size = obj['Size']
                         #zinfo.compress_type = ZIP_DEFLATED  # Causes downloads to hang, possibly because something gets confused about file size.
                         if zinfo.is_dir():  # Zip also denotes a folders as names ending with a slash.
                             await loop.run_in_executor(None, zf.writestr, zinfo, '')
                         else:
                             with zf.open(zinfo, mode='w') as dest:
                                 await loop.run_in_executor(None, s3_client.download_fileobj, bucket_name, obj['Key'], dest)
                 except BotoClientError as e:
```

### Comparing `heaserver-folders-aws-s3-1.0.9/src/heaserver/folderawss3/wstl/all.json` & `heaserver-folders-aws-s3-1.1.0/src/heaserver/folderawss3/wstl/all.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998279696493982%*

 * *Differences: {"'wstl'": "{'actions': {20: {'inputs': {delete: [12, 11]}}, 21: {'inputs': {delete: [13, 12]}}, "*

 * *           "42: {'inputs': {insert: [(2, OrderedDict([('name', 'storage_class'), ('prompt', "*

 * *           "'Storage'), ('type', 'select'), ('required', True), ('suggest', "*

 * *           "[OrderedDict([('value', 'STANDARD'), ('text', 'Standard')]), OrderedDict([('value', "*

 * *           "'DEEP_ARCHIVE'), ('text', 'Glacier Deep Archive')]), OrderedDict([('value', "*

 * *           "'GLACIER'), ('text', 'Glacier Flexible Re […]*

```diff
@@ -291,66 +291,14 @@
                         "prompt": "Source",
                         "readOnly": true
                     },
                     {
                         "name": "source_detail",
                         "prompt": "Source detail",
                         "readOnly": true
-                    },
-                    {
-                        "hea": {
-                            "optionsFromUrl": {
-                                "path": "people/",
-                                "text": "display_name",
-                                "value": "id"
-                            },
-                            "section": "shares",
-                            "sectionPrompt": "Shares"
-                        },
-                        "name": "user",
-                        "prompt": "User",
-                        "readOnly": true,
-                        "required": true,
-                        "type": "select"
-                    },
-                    {
-                        "hea": {
-                            "cardinality": "multiple",
-                            "section": "shares"
-                        },
-                        "name": "permissions",
-                        "prompt": "Permissions",
-                        "readOnly": true,
-                        "suggest": [
-                            {
-                                "text": "Co-owner",
-                                "value": "COOWNER"
-                            },
-                            {
-                                "text": "Creator",
-                                "value": "CREATOR"
-                            },
-                            {
-                                "text": "Deleter",
-                                "value": "DELETER"
-                            },
-                            {
-                                "text": "Editor",
-                                "value": "EDITOR"
-                            },
-                            {
-                                "text": "Sharer",
-                                "value": "SHARER"
-                            },
-                            {
-                                "text": "Viewer",
-                                "value": "VIEWER"
-                            }
-                        ],
-                        "type": "select"
                     }
                 ],
                 "name": "heaserver-awss3folders-folder-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
@@ -441,66 +389,14 @@
                         "prompt": "Source",
                         "readOnly": true
                     },
                     {
                         "name": "source_detail",
                         "prompt": "Source detail",
                         "readOnly": true
-                    },
-                    {
-                        "hea": {
-                            "optionsFromUrl": {
-                                "path": "people/",
-                                "text": "display_name",
-                                "value": "id"
-                            },
-                            "section": "shares",
-                            "sectionPrompt": "Shares"
-                        },
-                        "name": "user",
-                        "prompt": "User",
-                        "readOnly": true,
-                        "required": true,
-                        "type": "select"
-                    },
-                    {
-                        "hea": {
-                            "cardinality": "multiple",
-                            "section": "shares"
-                        },
-                        "name": "permissions",
-                        "prompt": "Permissions",
-                        "readOnly": true,
-                        "suggest": [
-                            {
-                                "text": "Co-owner",
-                                "value": "COOWNER"
-                            },
-                            {
-                                "text": "Creator",
-                                "value": "CREATOR"
-                            },
-                            {
-                                "text": "Deleter",
-                                "value": "DELETER"
-                            },
-                            {
-                                "text": "Editor",
-                                "value": "EDITOR"
-                            },
-                            {
-                                "text": "Sharer",
-                                "value": "SHARER"
-                            },
-                            {
-                                "text": "Viewer",
-                                "value": "VIEWER"
-                            }
-                        ],
-                        "type": "select"
                     }
                 ],
                 "name": "heaserver-awss3folders-project-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
@@ -802,14 +698,39 @@
                         "hea": {
                             "display": false
                         },
                         "name": "target_type",
                         "prompt": "Type",
                         "readOnly": true,
                         "value": "heaobject.data.AWSS3FileObject"
+                    },
+                    {
+                        "name": "storage_class",
+                        "prompt": "Storage",
+                        "required": true,
+                        "suggest": [
+                            {
+                                "text": "Standard",
+                                "value": "STANDARD"
+                            },
+                            {
+                                "text": "Glacier Deep Archive",
+                                "value": "DEEP_ARCHIVE"
+                            },
+                            {
+                                "text": "Glacier Flexible Retrieval",
+                                "value": "GLACIER"
+                            },
+                            {
+                                "text": "Glacier Instant Retrieval",
+                                "value": "GLACIER_IR"
+                            }
+                        ],
+                        "type": "select",
+                        "value": "DEEP_ARCHIVE"
                     }
                 ],
                 "name": "heaserver-awss3folders-folder-upload-form",
                 "prompt": "Get target folder",
                 "target": "item cj-template",
                 "type": "safe"
             },
@@ -828,14 +749,39 @@
                         "hea": {
                             "display": false
                         },
                         "name": "target_type",
                         "prompt": "Type",
                         "readOnly": true,
                         "value": "heaobject.data.AWSS3FileObject"
+                    },
+                    {
+                        "name": "storage_class",
+                        "prompt": "Storage",
+                        "required": true,
+                        "suggest": [
+                            {
+                                "text": "Standard",
+                                "value": "STANDARD"
+                            },
+                            {
+                                "text": "Glacier Deep Archive",
+                                "value": "DEEP_ARCHIVE"
+                            },
+                            {
+                                "text": "Glacier Flexible Retrieval",
+                                "value": "GLACIER"
+                            },
+                            {
+                                "text": "Glacier Instant Retrieval",
+                                "value": "GLACIER_IR"
+                            }
+                        ],
+                        "type": "select",
+                        "value": "DEEP_ARCHIVE"
                     }
                 ],
                 "name": "heaserver-awss3folders-project-upload-form",
                 "prompt": "Get target project",
                 "target": "item cj-template",
                 "type": "safe"
             },
```

### Comparing `heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/PKG-INFO` & `heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-folders-aws-s3
-Version: 1.0.9
+Version: 1.1.0
 Summary: The HEA AWS S3 bucket folder service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,22 +20,38 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.0.7
+Requires-Dist: heaserver~=1.1.2
 
 # HEA Server AWS S3 Bucket Folders Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server AWS S3 Bucket Folders Microservice manages folders in AWS S3 buckets.
 
+## Version 1.1.0
+* Pass folder and project permissions back to clients.
+
+## Version 1.0.13
+* Changed presented bucket owner to system|aws.
+* Omitted shares from the properties template.
+
+## Version 1.0.12
+* Improved upload desktop object action message.
+
+## Version 1.0.11
+* Improved performance.
+
+## Version 1.0.10
+* Support getting the content of a folder as a zip file when the folder has files > 2GiB in size.
+
 ## Version 1.0.9
 * Prevent zip file corruption when getting the content of a folder.
 
 ## Version 1.0.8
 * Addressed issue where downloads start failing for all users if one user interrupts their download.
 
 ## Version 1.0.7
```

### Comparing `heaserver-folders-aws-s3-1.0.9/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt` & `heaserver-folders-aws-s3-1.1.0/src/heaserver_folders_aws_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/folderawss3testcase.py` & `heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/folderawss3testcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,16 +18,21 @@
         'description': None,
         'display_name': 'TestFolder',
         'id': 'VGVzdEZvbGRlci8=',
         'invites': [],
         'modified': None,
         'mime_type': 'application/x.item',
         'name': 'VGVzdEZvbGRlci8=',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3ItemInFolder',
         'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
         'actual_object_id': 'VGVzdEZvbGRlci8=',
         'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlci8=',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
@@ -47,16 +52,21 @@
         'derived_from': [],
         'description': None,
         'display_name': 'TestFolder2',
         'id': 'VGVzdEZvbGRlcjIv',
         'invites': [],
         'modified': None,
         'name': 'VGVzdEZvbGRlcjIv',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3ItemInFolder',
         'actual_object_type_name': 'heaobject.folder.AWSS3Folder',
         'actual_object_id': 'VGVzdEZvbGRlcjIv',
         'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3folders/VGVzdEZvbGRlcjIv',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
@@ -187,16 +197,21 @@
         'derived_from': [],
         'description': None,
         'display_name': 'TestFolder',
         'id': 'VGVzdEZvbGRlci8=',
         'invites': [],
         'modified': None,
         'name': 'VGVzdEZvbGRlci8=',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3Folder',
         'mime_type': 'application/x.folder',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder/',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestFolder/',
@@ -208,16 +223,21 @@
             'derived_from': [],
             'description': None,
             'display_name': 'TestFolder2',
             'id': 'VGVzdEZvbGRlcjIv',
             'invites': [],
             'modified': None,
             'name': 'VGVzdEZvbGRlcjIv',
-            'owner': user.NONE_USER,
-            'shares': [],
+            'owner': user.AWS_USER,
+            'shares': [{
+                'invite': None,
+                'permissions': ['COOWNER'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': 'system|all'
+            }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.folder.AWSS3Folder',
             'mime_type': 'application/x.folder',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestFolder2/',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'TestFolder2/',
```

### Comparing `heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/projectawss3testcase.py` & `heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/projectawss3testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,21 @@
         'description': None,
         'display_name': 'TestProject',
         'id': 'VGVzdFByb2plY3Qv',
         'invites': [],
         'modified': None,
         'mime_type': 'application/x.item',
         'name': 'VGVzdFByb2plY3Qv',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3ItemInFolder',
         'actual_object_type_name': 'heaobject.project.AWSS3Project',
         'actual_object_id': 'VGVzdFByb2plY3Qv',
         'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3projects/VGVzdFByb2plY3Qv',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestProject/',
@@ -68,16 +73,21 @@
         'derived_from': [],
         'description': None,
         'display_name': 'TestProject2',
         'id': 'VGVzdFByb2plY3QyLw==',
         'invites': [],
         'modified': None,
         'name': 'VGVzdFByb2plY3QyLw==',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.folder.AWSS3ItemInFolder',
         'actual_object_type_name': 'heaobject.project.AWSS3Project',
         'actual_object_id': 'VGVzdFByb2plY3QyLw==',
         'actual_object_uri': 'volumes/666f6f2d6261722d71757578/buckets/arp-scale-2-cloud-bucket-with-tags11/awss3projects/VGVzdFByb2plY3QyLw==',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestProject2/',
@@ -252,16 +262,21 @@
         'derived_from': [],
         'description': None,
         'display_name': 'TestProject',
         'id': 'VGVzdFByb2plY3Qv',
         'invites': [],
         'modified': None,
         'name': 'VGVzdFByb2plY3Qv',
-        'owner': user.NONE_USER,
-        'shares': [],
+        'owner': user.AWS_USER,
+        'shares': [{
+            'invite': None,
+            'permissions': ['COOWNER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.project.AWSS3Project',
         'mime_type': 'application/x.project',
         's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestProject/',
         'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
         'key': 'TestProject/'
@@ -272,16 +287,21 @@
             'derived_from': [],
             'description': None,
             'display_name': 'TestProject2',
             'id': 'VGVzdFByb2plY3QyLw==',
             'invites': [],
             'modified': None,
             'name': 'VGVzdFByb2plY3QyLw==',
-            'owner': user.NONE_USER,
-            'shares': [],
+            'owner': user.AWS_USER,
+            'shares': [{
+                'invite': None,
+                'permissions': ['COOWNER'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': 'system|all'
+            }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.project.AWSS3Project',
             'mime_type': 'application/x.project',
             's3_uri': 's3://arp-scale-2-cloud-bucket-with-tags11/TestProject2/',
             'bucket_id': 'arp-scale-2-cloud-bucket-with-tags11',
             'key': 'TestProject2/'
```

### Comparing `heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/test_all.py` & `heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-folders-aws-s3-1.0.9/tests/heaserver/folderawss3test/wstl/all.json` & `heaserver-folders-aws-s3-1.1.0/tests/heaserver/folderawss3test/wstl/all.json`

 * *Files identical despite different names*

