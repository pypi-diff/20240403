# Comparing `tmp/codec_sdk-0.2.4.tar.gz` & `tmp/codec_sdk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codec_sdk-0.2.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "codec_sdk-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `codec_sdk-0.2.4.tar` & `codec_sdk-0.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2757 2024-03-25 13:32:56.805766 codec_sdk-0.2.4/.gitignore
--rw-r--r--   0        0        0      148 2024-03-27 16:29:36.840236 codec_sdk-0.2.4/.pypirc
--rw-r--r--   0        0        0      501 2024-04-02 18:53:10.455880 codec_sdk-0.2.4/CHANGELOG.md
--rw-r--r--   0        0        0     1072 2024-03-25 11:46:44.142211 codec_sdk-0.2.4/LICENSE
--rw-r--r--   0        0        0      211 2024-03-25 20:13:09.134215 codec_sdk-0.2.4/Pipfile
--rw-r--r--   0        0        0     1405 2024-03-31 16:16:48.725034 codec_sdk-0.2.4/README.md
--rw-r--r--   0        0        0       95 2024-04-02 18:50:33.798622 codec_sdk-0.2.4/codec/__init__.py
--rw-r--r--   0        0        0      389 2024-03-25 15:11:00.385160 codec_sdk-0.2.4/codec/auth.py
--rw-r--r--   0        0        0     1060 2024-04-02 18:41:51.102977 codec_sdk-0.2.4/codec/client.py
--rw-r--r--   0        0        0     1318 2024-04-02 10:46:02.079632 codec_sdk-0.2.4/codec/constants.py
--rw-r--r--   0        0        0     1154 2024-03-31 16:38:04.420397 codec_sdk-0.2.4/codec/exceptions.py
--rw-r--r--   0        0        0      157 2024-04-02 18:49:59.803952 codec_sdk-0.2.4/codec/resources/__init__.py
--rw-r--r--   0        0        0        0 2024-03-31 14:49:40.788907 codec_sdk-0.2.4/codec/resources/collections/__init__.py
--rw-r--r--   0        0        0     1076 2024-04-02 18:32:08.559513 codec_sdk-0.2.4/codec/resources/collections/collections.py
--rw-r--r--   0        0        0      476 2024-03-31 15:55:20.630364 codec_sdk-0.2.4/codec/resources/collections/format.py
--rw-r--r--   0        0        0      246 2024-03-31 16:21:39.938800 codec_sdk-0.2.4/codec/resources/collections/types.py
--rw-r--r--   0        0        0       98 2024-03-31 16:53:09.176751 codec_sdk-0.2.4/codec/resources/logger.py
--rw-r--r--   0        0        0     2819 2024-03-31 14:50:06.360715 codec_sdk-0.2.4/codec/resources/request.py
--rw-r--r--   0        0        0        0 2024-03-31 14:50:01.919681 codec_sdk-0.2.4/codec/resources/search/__init__.py
--rw-r--r--   0        0        0      604 2024-03-31 16:40:39.439653 codec_sdk-0.2.4/codec/resources/search/search.py
--rw-r--r--   0        0        0      273 2024-03-31 16:52:38.800607 codec_sdk-0.2.4/codec/resources/search/types.py
--rw-r--r--   0        0        0        0 2024-03-31 14:49:13.206374 codec_sdk-0.2.4/codec/resources/videos/__init__.py
--rw-r--r--   0        0        0      371 2024-03-31 15:54:29.778454 codec_sdk-0.2.4/codec/resources/videos/format.py
--rw-r--r--   0        0        0      486 2024-03-31 16:04:41.602700 codec_sdk-0.2.4/codec/resources/videos/types.py
--rw-r--r--   0        0        0     2882 2024-03-31 16:39:01.854587 codec_sdk-0.2.4/codec/resources/videos/videos.py
--rw-r--r--   0        0        0       51 2024-04-02 18:34:36.254380 codec_sdk-0.2.4/codec/resources/webhook/__init__.py
--rw-r--r--   0        0        0     1092 2024-04-02 18:49:57.471447 codec_sdk-0.2.4/codec/resources/webhook/webhook.py
--rw-r--r--   0        0        0        0 2024-03-25 20:03:51.340117 codec_sdk-0.2.4/codec/utils/__init__.py
--rw-r--r--   0        0        0      633 2024-03-26 12:38:41.420078 codec_sdk-0.2.4/codec/utils/file_utils.py
--rw-r--r--   0        0        0      114 2024-03-31 15:35:42.827701 codec_sdk-0.2.4/codec/utils/type_utils.py
--rw-r--r--   0        0        0      606 2024-03-31 16:16:51.826816 codec_sdk-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 codec_sdk-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2757 2024-03-25 13:32:56.805766 codec_sdk-0.2.5/.gitignore
+-rw-r--r--   0        0        0      148 2024-03-27 16:29:36.840236 codec_sdk-0.2.5/.pypirc
+-rw-r--r--   0        0        0      599 2024-04-03 12:27:52.830347 codec_sdk-0.2.5/CHANGELOG.md
+-rw-r--r--   0        0        0     1072 2024-03-25 11:46:44.142211 codec_sdk-0.2.5/LICENSE
+-rw-r--r--   0        0        0      211 2024-03-25 20:13:09.134215 codec_sdk-0.2.5/Pipfile
+-rw-r--r--   0        0        0     1339 2024-04-03 12:24:08.966117 codec_sdk-0.2.5/README.md
+-rw-r--r--   0        0        0       95 2024-04-03 12:27:55.901262 codec_sdk-0.2.5/codec/__init__.py
+-rw-r--r--   0        0        0      389 2024-03-25 15:11:00.385160 codec_sdk-0.2.5/codec/auth.py
+-rw-r--r--   0        0        0     1060 2024-04-03 12:28:04.791143 codec_sdk-0.2.5/codec/client.py
+-rw-r--r--   0        0        0     1318 2024-04-02 10:46:02.079632 codec_sdk-0.2.5/codec/constants.py
+-rw-r--r--   0        0        0     1154 2024-03-31 16:38:04.420397 codec_sdk-0.2.5/codec/exceptions.py
+-rw-r--r--   0        0        0      157 2024-04-02 18:49:59.803952 codec_sdk-0.2.5/codec/resources/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:49:40.788907 codec_sdk-0.2.5/codec/resources/collections/__init__.py
+-rw-r--r--   0        0        0     1076 2024-04-02 18:32:08.559513 codec_sdk-0.2.5/codec/resources/collections/collections.py
+-rw-r--r--   0        0        0      452 2024-04-03 12:26:14.996441 codec_sdk-0.2.5/codec/resources/collections/format.py
+-rw-r--r--   0        0        0      240 2024-04-03 12:28:08.755135 codec_sdk-0.2.5/codec/resources/collections/types.py
+-rw-r--r--   0        0        0       98 2024-03-31 16:53:09.176751 codec_sdk-0.2.5/codec/resources/logger.py
+-rw-r--r--   0        0        0     2819 2024-03-31 14:50:06.360715 codec_sdk-0.2.5/codec/resources/request.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:50:01.919681 codec_sdk-0.2.5/codec/resources/search/__init__.py
+-rw-r--r--   0        0        0      604 2024-03-31 16:40:39.439653 codec_sdk-0.2.5/codec/resources/search/search.py
+-rw-r--r--   0        0        0      273 2024-04-03 12:30:00.980022 codec_sdk-0.2.5/codec/resources/search/types.py
+-rw-r--r--   0        0        0        0 2024-03-31 14:49:13.206374 codec_sdk-0.2.5/codec/resources/videos/__init__.py
+-rw-r--r--   0        0        0      347 2024-04-03 12:26:46.601634 codec_sdk-0.2.5/codec/resources/videos/format.py
+-rw-r--r--   0        0        0      468 2024-04-03 12:29:19.052679 codec_sdk-0.2.5/codec/resources/videos/types.py
+-rw-r--r--   0        0        0     2852 2024-04-03 12:29:48.049822 codec_sdk-0.2.5/codec/resources/videos/videos.py
+-rw-r--r--   0        0        0       51 2024-04-02 18:34:36.254380 codec_sdk-0.2.5/codec/resources/webhook/__init__.py
+-rw-r--r--   0        0        0     1092 2024-04-02 18:49:57.471447 codec_sdk-0.2.5/codec/resources/webhook/webhook.py
+-rw-r--r--   0        0        0        0 2024-03-25 20:03:51.340117 codec_sdk-0.2.5/codec/utils/__init__.py
+-rw-r--r--   0        0        0      633 2024-03-26 12:38:41.420078 codec_sdk-0.2.5/codec/utils/file_utils.py
+-rw-r--r--   0        0        0      114 2024-03-31 15:35:42.827701 codec_sdk-0.2.5/codec/utils/type_utils.py
+-rw-r--r--   0        0        0      606 2024-03-31 16:16:51.826816 codec_sdk-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 codec_sdk-0.2.5/PKG-INFO
```

### Comparing `codec_sdk-0.2.4/.gitignore` & `codec_sdk-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/LICENSE` & `codec_sdk-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/README.md` & `codec_sdk-0.2.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,14 @@
 
 You don't need this source code unless you want to modify the package. If you just want to use the package, just run:
 
 ```python
 pip install --upgrade codec-sdk
 ```
 
-Install from source with:
-
-```python
-python setup.py install
-```
-
 ### Requirements
 Python 3.8+
 
 
 ## Usage
 
 The library needs to be configured with your team's API key which is available in the [Codec Dashboard](https://codec.io/dashboard). Instantiate the Codec client with it:
```

### Comparing `codec_sdk-0.2.4/codec/client.py` & `codec_sdk-0.2.5/codec/client.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/codec/constants.py` & `codec_sdk-0.2.5/codec/constants.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/codec/exceptions.py` & `codec_sdk-0.2.5/codec/exceptions.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/codec/resources/collections/collections.py` & `codec_sdk-0.2.5/codec/resources/collections/collections.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/codec/resources/request.py` & `codec_sdk-0.2.5/codec/resources/request.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/codec/resources/search/search.py` & `codec_sdk-0.2.5/codec/resources/search/search.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/codec/resources/videos/videos.py` & `codec_sdk-0.2.5/codec/resources/videos/videos.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from codec.resources.videos.types import (
-    VideoStatusObject,
-    PreUploadedVideoObject
+    VideoStatus,
+    PreUploadedVideo
 )
 from codec.constants import SUPABASE_URL, SUPABASE_PUBLIC_KEY, POLLING_INTERVAL
 from codec.utils.file_utils import validate_path_and_get_filename
 from codec.resources.videos.format import format_video_object
 from codec.resources.request import Request
 from supabase import create_client
 import time
@@ -26,15 +26,15 @@
     pre_upload_response = Request(auth).post(
         pre_upload_endpoint,
         body={
             "original_filename": filename,
             "collection": collection
         }
     )
-    pre_upload_response = PreUploadedVideoObject(**pre_upload_response)
+    pre_upload_response = PreUploadedVideo(**pre_upload_response)
 
     with open(path, "rb") as f:
         supabase.storage.from_("codec-multi").upload_to_signed_url(
             path=pre_upload_response.path,
             token=pre_upload_response.token,
             file=f,
             file_options={
@@ -57,15 +57,15 @@
             response = Request(auth).get(endpoint)
 
             if response.get("status") == "indexed":
                 keep_polling = False
             
             time.sleep(POLLING_INTERVAL)
 
-    response = VideoStatusObject(**response)
+    response = VideoStatus(**response)
 
     return response
 
 
 class Videos:
     def __init__(self, auth):
         self.auth = auth
@@ -85,15 +85,15 @@
 
     def delete(
         self,
         uid: str
     ):
         endpoint = f"/video/{uid}"
         response = Request(self.auth).delete(endpoint)
-        response = VideoStatusObject(**response)
+        response = VideoStatus(**response)
 
         return response
     
     def upload(
         self,
         path: str,
         collection: str
```

### Comparing `codec_sdk-0.2.4/codec/resources/webhook/webhook.py` & `codec_sdk-0.2.5/codec/resources/webhook/webhook.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/codec/utils/file_utils.py` & `codec_sdk-0.2.5/codec/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/pyproject.toml` & `codec_sdk-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `codec_sdk-0.2.4/PKG-INFO` & `codec_sdk-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codec-sdk
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python Library for the Codec API
 Author-email: Armada Labs Inc <contact@codec.io>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests >=2.31.0
 Requires-Dist: supabase >=1.0.3
@@ -25,20 +25,14 @@
 
 You don't need this source code unless you want to modify the package. If you just want to use the package, just run:
 
 ```python
 pip install --upgrade codec-sdk
 ```
 
-Install from source with:
-
-```python
-python setup.py install
-```
-
 ### Requirements
 Python 3.8+
 
 
 ## Usage
 
 The library needs to be configured with your team's API key which is available in the [Codec Dashboard](https://codec.io/dashboard). Instantiate the Codec client with it:
```

