# Comparing `tmp/heaserver-buckets-1.0.4.tar.gz` & `tmp/heaserver-buckets-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-buckets-1.0.4.tar", last modified: Wed Mar 27 00:34:11 2024, max compression
+gzip compressed data, was "heaserver-buckets-1.1.0.tar", last modified: Wed Apr  3 03:35:36 2024, max compression
```

## Comparing `heaserver-buckets-1.0.4.tar` & `heaserver-buckets-1.1.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.161363 heaserver-buckets-1.0.4/
--rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/.gitignore
--rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4873 2024-03-27 00:34:11.160363 heaserver-buckets-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3532 2024-03-27 00:21:18.000000 heaserver-buckets-1.0.4/README.md
--rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/RELEASING.md
--rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.042176 heaserver-buckets-1.0.4/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.042176 heaserver-buckets-1.0.4/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.111290 heaserver-buckets-1.0.4/integrationtests/heaserver/bucketintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/integrationtests/heaserver/bucketintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/integrationtests/heaserver/bucketintegrationtest/test_all.py
--rw-rw-rw-   0        0        0    10477 2024-03-27 00:16:45.000000 heaserver-buckets-1.0.4/integrationtests/heaserver/bucketintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/pytest.ini
--rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/requirements_dev.txt
--rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-03-27 00:34:11.161363 heaserver-buckets-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1838 2024-03-27 00:33:22.000000 heaserver-buckets-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.044146 heaserver-buckets-1.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.043146 heaserver-buckets-1.0.4/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.113290 heaserver-buckets-1.0.4/src/heaserver/bucket/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/src/heaserver/bucket/__init__.py
--rw-rw-rw-   0        0        0    73277 2024-03-27 00:13:26.000000 heaserver-buckets-1.0.4/src/heaserver/bucket/service.py
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.114292 heaserver-buckets-1.0.4/src/heaserver/bucket/wstl/
--rw-rw-rw-   0        0        0    13825 2024-03-27 00:15:05.000000 heaserver-buckets-1.0.4/src/heaserver/bucket/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.159362 heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/
--rw-rw-rw-   0        0        0     4873 2024-03-27 00:34:11.000000 heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2024-03-27 00:34:11.000000 heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 00:34:11.000000 heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-03-27 00:34:11.000000 heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-03-27 00:34:11.000000 heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-27 00:34:11.000000 heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.045146 heaserver-buckets-1.0.4/tests/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.045146 heaserver-buckets-1.0.4/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-03-27 00:34:11.157362 heaserver-buckets-1.0.4/tests/heaserver/buckettest/
--rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/tests/heaserver/buckettest/__init__.py
--rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver-buckets-1.0.4/tests/heaserver/buckettest/test_all.py
--rw-rw-rw-   0        0        0     8727 2024-03-27 00:16:14.000000 heaserver-buckets-1.0.4/tests/heaserver/buckettest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.464555 heaserver-buckets-1.1.0/
+-rw-rw-rw-   0        0        0      261 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/.gitignore
+-rw-rw-rw-   0        0        0     1515 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4989 2024-04-03 03:35:36.463556 heaserver-buckets-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3648 2024-04-03 03:21:21.000000 heaserver-buckets-1.1.0/README.md
+-rw-rw-rw-   0        0        0     1737 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/RELEASING.md
+-rw-rw-rw-   0        0        0      470 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.312638 heaserver-buckets-1.1.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.313661 heaserver-buckets-1.1.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.392383 heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4817 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0    10825 2024-04-02 02:10:02.000000 heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/pytest.ini
+-rw-rw-rw-   0        0        0      262 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     5310 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-04-03 03:35:36.464555 heaserver-buckets-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1838 2024-04-03 03:34:21.000000 heaserver-buckets-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.315726 heaserver-buckets-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.314699 heaserver-buckets-1.1.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.406295 heaserver-buckets-1.1.0/src/heaserver/bucket/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/src/heaserver/bucket/__init__.py
+-rw-rw-rw-   0        0        0    73544 2024-04-02 02:09:27.000000 heaserver-buckets-1.1.0/src/heaserver/bucket/service.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.413519 heaserver-buckets-1.1.0/src/heaserver/bucket/wstl/
+-rw-rw-rw-   0        0        0    14512 2024-04-02 22:57:58.000000 heaserver-buckets-1.1.0/src/heaserver/bucket/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.461589 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/
+-rw-rw-rw-   0        0        0     4989 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-03 03:35:36.000000 heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.315726 heaserver-buckets-1.1.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.316753 heaserver-buckets-1.1.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-03 03:35:36.459556 heaserver-buckets-1.1.0/tests/heaserver/buckettest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/tests/heaserver/buckettest/__init__.py
+-rw-rw-rw-   0        0        0     1623 2023-12-18 18:48:15.000000 heaserver-buckets-1.1.0/tests/heaserver/buckettest/test_all.py
+-rw-rw-rw-   0        0        0     9075 2024-04-02 00:28:40.000000 heaserver-buckets-1.1.0/tests/heaserver/buckettest/testcase.py
```

### Comparing `heaserver-buckets-1.0.4/Dockerfile` & `heaserver-buckets-1.1.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.4/LICENSE` & `heaserver-buckets-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.4/PKG-INFO` & `heaserver-buckets-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.0.4
+Version: 1.1.0
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.1
+Requires-Dist: heaserver~=1.1.2
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.0
+* Fixed support for uploading to a bucket.
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.4
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
 
 ## Version 1.0.3
 * Improved performance getting all buckets.
```

### Comparing `heaserver-buckets-1.0.4/README.md` & `heaserver-buckets-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.0
+* Fixed support for uploading to a bucket.
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.4
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
 
 ## Version 1.0.3
 * Improved performance getting all buckets.
```

### Comparing `heaserver-buckets-1.0.4/RELEASING.md` & `heaserver-buckets-1.1.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.4/integrationtests/heaserver/bucketintegrationtest/test_all.py` & `heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.4/integrationtests/heaserver/bucketintegrationtest/testcase.py` & `heaserver-buckets-1.1.0/integrationtests/heaserver/bucketintegrationtest/testcase.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,20 @@
         'object_count': None,
         'size': None,
         'display_name': 'hci-foundation-1',
         'invites': [],
         'modified': None,
         'name': 'hci-foundation-1',
         'owner': AWS_USER,
-        'shares': [],
+        'shares': [{
+            'invite': None,
+            'permissions': ['EDITOR'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.bucket.AWSBucket',
         'arn': 'arn:aws:s3::hci-foundation-1',
         'versioned': True,
         'encrypted': False,
         'region': 'us-west-1',
@@ -52,15 +57,20 @@
             'object_count': None,
             'size': None,
             'display_name': 'hci-foundation-2',
             'invites': [],
             'modified': None,
             'name': 'hci-foundation-2',
             'owner': AWS_USER,
-            'shares': [],
+            'shares': [{
+                'invite': None,
+                'permissions': ['EDITOR'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': 'system|all'
+            }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.bucket.AWSBucket',
             'arn': 'arn:aws:s3::hci-foundation-2',
             'versioned': True,
             'encrypted': False,
             'region': 'us-west-1',
```

### Comparing `heaserver-buckets-1.0.4/run-swaggerui.py` & `heaserver-buckets-1.1.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.4/setup.py` & `heaserver-buckets-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-buckets',
-    version='1.0.4',
+    version='1.1.0',
     description="a service for managing buckets and their data within the cloud",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.bucket'],
     package_data={'heaserver.bucket': ['wstl/*.json']},
-    install_requires=['heaserver~=1.1.1'],
+    install_requires=['heaserver~=1.1.2'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-buckets-1.0.4/src/heaserver/bucket/service.py` & `heaserver-buckets-1.1.0/src/heaserver/bucket/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from heaserver.service.db import awsservicelib, aws
 from heaserver.service.wstl import builder_factory, action
 from heaobject.folder import AWSS3BucketItem, Folder, AWSS3Folder
 from heaobject.project import AWSS3Project
 from heaobject.volume import AWSFileSystem
 from heaobject.bucket import AWSBucket
 from heaobject.error import DeserializeException
-from heaobject.root import Tag
+from heaobject.root import Tag, ShareImpl, Permission
 from heaobject.activity import Status
-from heaobject.user import NONE_USER, AWS_USER
+from heaobject.user import NONE_USER, AWS_USER, ALL_USERS
 from heaserver.service.appproperty import HEA_CACHE
 from heaserver.service.oidcclaimhdrs import SUB
 from heaserver.service.heaobjectsupport import new_heaobject_from_type, type_to_resource_url
 from heaserver.service.sources import AWS_S3
 from heaserver.service.messagebroker import publish_desktop_object, publisher_cleanup_context_factory
 from heaserver.service.activity import DesktopObjectActionLifecycle
 from botocore.exceptions import ClientError as BotoClientError
@@ -669,15 +669,15 @@
                     return awsservicelib.handle_client_error(e)
                 else:
                     bucket_dict_list = [buck.to_dict() for buck in buck_list if buck is not None]
                     request.app[HEA_CACHE][cache_key] = bucket_dict_list
                     for buck in bucket_dict_list:
                         request.app[HEA_CACHE][(sub, volume_id, buck['id'], 'head')] = buck['id']
                         request.app[HEA_CACHE][(sub, volume_id, buck['id'], 'actual')] = buck
-    return await response.get_all(request, bucket_dict_list)
+    return await response.get_all(request, bucket_dict_list, permissions=[buck.get_permissions(sub) for buck in buck_list])
 
 
 @routes.get('/volumes/{volume_id}/bucketitems')
 @routes.get('/volumes/{volume_id}/bucketitems/')
 @action(name='heaserver-buckets-item-get-actual', rel='hea-actual', path='{+actual_object_uri}')
 @action(name='heaserver-buckets-item-get-volume', rel='hea-volume', path='volumes/{volume_id}')
 async def get_all_bucketitems(request: web.Request) -> web.Response:
@@ -1427,15 +1427,15 @@
                     if type(bucket_result) is AWSBucket:
                         activity.new_object_id = bucket_name
                         activity.new_object_uri = f'volumes/{volume_id}/buckets/{bucket_name}'
                         activity.new_object_type_name = AWSBucket.get_type_name()
                         activity.new_volume_id = volume_id
                         bucket_dict = bucket_result.to_dict()
                         request.app[HEA_CACHE][(sub, volume_id, bucket_dict['id'], 'actual')] = bucket_dict
-                        return await response.get(request=request, data=bucket_dict)
+                        return await response.get(request=request, data=bucket_dict, permissions=bucket_result.get_permissions(sub))
                     activity.status = Status.FAILED
                     return await response.get(request, data=None)
                 except BotoClientError as e:
                     activity.status = Status.FAILED
                     return awsservicelib.handle_client_error(e)
 
 
@@ -1465,14 +1465,18 @@
         b.display_name = bucket_name
     async_bucket_methods = []
     b.bucket_id = b.name
     b.source = AWS_S3
     b.source_detail = AWS_S3
     b.arn = f'arn:aws:s3::{b.id}'
     b.owner = AWS_USER
+    share = ShareImpl()
+    share.user = ALL_USERS
+    share.permissions = [Permission.EDITOR]
+    b.shares = [share]
 
     if creation_date:
         b.created = creation_date
     elif cached_value := cache.get((sub, volume_id, None, 'items')):
         b.created = next((bucket_['created'] for bucket_ in cached_value if bucket_['name'] == b.name), None)
     else:
         async def _get_creation_date(b: AWSBucket):
```

### Comparing `heaserver-buckets-1.0.4/src/heaserver/bucket/wstl/all.json` & `heaserver-buckets-1.1.0/src/heaserver/bucket/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998249299719888%*

 * *Differences: {"'wstl'": "{'actions': {11: {'inputs': {insert: [(2, OrderedDict([('name', 'storage_class'), "*

 * *           "('prompt', 'Storage'), ('type', 'select'), ('required', True), ('suggest', "*

 * *           "[OrderedDict([('value', 'STANDARD'), ('text', 'Standard')]), OrderedDict([('value', "*

 * *           "'DEEP_ARCHIVE'), ('text', 'Glacier Deep Archive')]), OrderedDict([('value', "*

 * *           "'GLACIER'), ('text', 'Glacier Flexible Retrieval')]), OrderedDict([('value', "*

 * *           "'GLACIER_IR'), ('text', 'Glacier Ins […]*

```diff
@@ -102,14 +102,39 @@
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
+                        "value": "STANDARD"
                     }
                 ],
                 "name": "heaserver-buckets-bucket-get-upload-form",
                 "prompt": "Get target folder",
                 "target": "item cj-template",
                 "type": "safe"
             },
```

### Comparing `heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/PKG-INFO` & `heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-buckets
-Version: 1.0.4
+Version: 1.1.0
 Summary: a service for managing buckets and their data within the cloud
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-buckets,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,26 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.1.1
+Requires-Dist: heaserver~=1.1.2
 
 # HEA Server Buckets Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Server Buckets Microservice is a service for managing buckets and their data within the cloud.
 
+## Version 1.1.0
+* Fixed support for uploading to a bucket.
+* Pass desktop object permissions back to clients.
+
 ## Version 1.0.4
 * Changed presented bucket owner to system|aws.
 * Omitted shares from the properties template.
 
 ## Version 1.0.3
 * Improved performance getting all buckets.
```

### Comparing `heaserver-buckets-1.0.4/src/heaserver_buckets.egg-info/SOURCES.txt` & `heaserver-buckets-1.1.0/src/heaserver_buckets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.4/tests/heaserver/buckettest/test_all.py` & `heaserver-buckets-1.1.0/tests/heaserver/buckettest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-buckets-1.0.4/tests/heaserver/buckettest/testcase.py` & `heaserver-buckets-1.1.0/tests/heaserver/buckettest/testcase.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,20 @@
         'object_count': None,
         'size': None,
         'display_name': 'hci-foundation-1',
         'invites': [],
         'modified': None,
         'name': 'hci-foundation-1',
         'owner': AWS_USER,
-        'shares': [],
+        'shares': [{
+            'invite': None,
+            'permissions': ['EDITOR'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': 'system|all'
+        }],
         'source': 'AWS S3',
         'source_detail': 'AWS S3',
         'type': 'heaobject.bucket.AWSBucket',
         'arn': 'arn:aws:s3::hci-foundation-1',
         'versioned': True,
         'encrypted': False,
         'region': 'us-west-1',
@@ -46,15 +51,20 @@
             'object_count': None,
             'size': None,
             'display_name': 'hci-foundation-2',
             'invites': [],
             'modified': None,
             'name': 'hci-foundation-2',
             'owner': AWS_USER,
-            'shares': [],
+            'shares': [{
+                'invite': None,
+                'permissions': ['EDITOR'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': 'system|all'
+            }],
             'source': 'AWS S3',
             'source_detail': 'AWS S3',
             'type': 'heaobject.bucket.AWSBucket',
             'arn': 'arn:aws:s3::hci-foundation-2',
             'versioned': True,
             'encrypted': False,
             'region': 'us-west-1',
```

