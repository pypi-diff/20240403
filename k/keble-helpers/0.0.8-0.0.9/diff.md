# Comparing `tmp/keble_helpers-0.0.8.tar.gz` & `tmp/keble_helpers-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keble_helpers-0.0.8.tar", max compression
+gzip compressed data, was "keble_helpers-0.0.9.tar", max compression
```

## Comparing `keble_helpers-0.0.8.tar` & `keble_helpers-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1067 2024-03-05 11:10:37.691742 keble_helpers-0.0.8/LICENSE
--rw-r--r--   0        0        0        0 2024-03-05 11:10:37.692790 keble_helpers-0.0.8/README.md
--rw-r--r--   0        0        0      336 2024-03-08 10:26:06.008246 keble_helpers-0.0.8/keble_helpers/__init__.py
--rw-r--r--   0        0        0       78 2024-03-08 10:10:15.151580 keble_helpers-0.0.8/keble_helpers/aliyun/__init__.py
--rw-r--r--   0        0        0      284 2024-03-08 09:24:25.533371 keble_helpers-0.0.8/keble_helpers/aliyun/base.py
--rw-r--r--   0        0        0     3842 2024-03-08 10:26:58.233634 keble_helpers-0.0.8/keble_helpers/aliyun/oss.py
--rw-r--r--   0        0        0     1476 2024-03-08 10:27:40.754964 keble_helpers-0.0.8/keble_helpers/aliyun/sts.py
--rw-r--r--   0        0        0     3229 2024-03-08 10:23:17.599247 keble_helpers-0.0.8/keble_helpers/common.py
--rw-r--r--   0        0        0      132 2024-03-05 11:10:37.691567 keble_helpers-0.0.8/keble_helpers/enum.py
--rw-r--r--   0        0        0      125 2024-03-08 11:59:44.470150 keble_helpers-0.0.8/keble_helpers/pydantic/__init__.py
--rw-r--r--   0        0        0      869 2024-03-08 12:00:01.979940 keble_helpers-0.0.8/keble_helpers/pydantic/cloud_storage.py
--rw-r--r--   0        0        0      372 2024-03-08 10:26:58.235388 keble_helpers-0.0.8/keble_helpers/pydantic/config.py
--rw-r--r--   0        0        0      662 2024-03-08 12:00:13.230945 keble_helpers-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 keble_helpers-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-03-05 11:10:37.691742 keble_helpers-0.0.9/LICENSE
+-rw-r--r--   0        0        0        0 2024-03-05 11:10:37.692790 keble_helpers-0.0.9/README.md
+-rw-r--r--   0        0        0      336 2024-03-08 10:26:06.008246 keble_helpers-0.0.9/keble_helpers/__init__.py
+-rw-r--r--   0        0        0       78 2024-03-08 10:10:15.151580 keble_helpers-0.0.9/keble_helpers/aliyun/__init__.py
+-rw-r--r--   0        0        0      284 2024-03-08 09:24:25.533371 keble_helpers-0.0.9/keble_helpers/aliyun/base.py
+-rw-r--r--   0        0        0     4025 2024-03-09 03:14:50.298490 keble_helpers-0.0.9/keble_helpers/aliyun/oss.py
+-rw-r--r--   0        0        0     1476 2024-03-08 10:27:40.754964 keble_helpers-0.0.9/keble_helpers/aliyun/sts.py
+-rw-r--r--   0        0        0     3229 2024-03-08 10:23:17.599247 keble_helpers-0.0.9/keble_helpers/common.py
+-rw-r--r--   0        0        0      132 2024-03-05 11:10:37.691567 keble_helpers-0.0.9/keble_helpers/enum.py
+-rw-r--r--   0        0        0      125 2024-03-08 11:59:44.470150 keble_helpers-0.0.9/keble_helpers/pydantic/__init__.py
+-rw-r--r--   0        0        0      960 2024-03-09 07:25:55.488426 keble_helpers-0.0.9/keble_helpers/pydantic/cloud_storage.py
+-rw-r--r--   0        0        0      372 2024-03-08 10:26:58.235388 keble_helpers-0.0.9/keble_helpers/pydantic/config.py
+-rw-r--r--   0        0        0      662 2024-03-09 07:26:07.549677 keble_helpers-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 keble_helpers-0.0.9/PKG-INFO
```

### Comparing `keble_helpers-0.0.8/LICENSE` & `keble_helpers-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `keble_helpers-0.0.8/keble_helpers/aliyun/oss.py` & `keble_helpers-0.0.9/keble_helpers/aliyun/oss.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     content_length: Optional[int] = Field(None, description='File size in bytes', serialization_alias="contentLength")
     last_modified: Optional[int] = Field(None, description='File size in bytes', serialization_alias="lastModified")
     content_type: Optional[str] = Field(None, description='MIME type of the file, e.g. img/jpeg', serialization_alias="contentType")
 
 
 class AliyunOss(Aliyun):
 
+    # Aliyun OSS upload requires STS+RAM user authentication
+    # see: https://help.aliyun.com/zh/oss/developer-reference/use-the-accesskey-pair-of-a-ram-user-to-initiate-a-request
+
     def __init__(self, oss_endpoint: AnyHttpUrl, bucket: str, **kwargs):
         super().__init__(**kwargs)
         self.__oss_endpoint: str = str(oss_endpoint).strip("/ ")
         self.__bucket_name: str = bucket.strip("/ ")
 
     def get_bucket(self) -> oss2.Bucket:
         auth = oss2.Auth(self.access_key, self.secret)
```

### Comparing `keble_helpers-0.0.8/keble_helpers/aliyun/sts.py` & `keble_helpers-0.0.9/keble_helpers/aliyun/sts.py`

 * *Files identical despite different names*

### Comparing `keble_helpers-0.0.8/keble_helpers/common.py` & `keble_helpers-0.0.9/keble_helpers/common.py`

 * *Files identical despite different names*

### Comparing `keble_helpers-0.0.8/keble_helpers/pydantic/cloud_storage.py` & `keble_helpers-0.0.9/keble_helpers/pydantic/cloud_storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pydantic import BaseModel, AnyHttpUrl
 from .config import PydanticModelConfig
 from enum import Enum
-
+from typing import Optional
 
 class CloudStorageType(str, Enum):
     AWS_S3 = "AWS_S3"
     ALIYUN_OSS = "ALIYUN_OSS"
 
 
 class CloudStorageObjectType(str, Enum):
@@ -31,7 +31,10 @@
     base_url: AnyHttpUrl
 
     # type of cloud service
     type: CloudStorageType
 
     # type of file
     object_type: CloudStorageObjectType
+
+    # original file name
+    original_file_name: Optional[str]
```

### Comparing `keble_helpers-0.0.8/pyproject.toml` & `keble_helpers-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # poetry tutorial see: https://www.digitalocean.com/community/tutorials/how-to-publish-python-packages-to-pypi-using-poetry-on-ubuntu-22-04
 # also see: https://www.freecodecamp.org/news/how-to-build-and-publish-python-packages-with-poetry/
 
 [tool.poetry]
 name = "keble-helpers"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 authors = ["zhenhao-ma <bob0103779@gmail.com>"]
 readme = "README.md"
 packages = [{include = "keble_helpers"}]
 
 
 [tool.poetry.dependencies]
```

### Comparing `keble_helpers-0.0.8/PKG-INFO` & `keble_helpers-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keble-helpers
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Author: zhenhao-ma
 Author-email: bob0103779@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

