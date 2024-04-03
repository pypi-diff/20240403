# Comparing `tmp/google-cloud-storage-control-0.1.0.tar.gz` & `tmp/google-cloud-storage-control-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-storage-control-0.1.0.tar", last modified: Mon Mar 25 19:56:53 2024, max compression
+gzip compressed data, was "google-cloud-storage-control-0.1.1.tar", last modified: Wed Apr  3 01:22:09 2024, max compression
```

## Comparing `google-cloud-storage-control-0.1.0.tar` & `google-cloud-storage-control-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.437289 google-cloud-storage-control-0.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5200 2024-03-25 19:56:53.437289 google-cloud-storage-control-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3812 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.425289 google-cloud-storage-control-0.1.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.425289 google-cloud-storage-control-0.1.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.429289 google-cloud-storage-control-0.1.0/google/cloud/storage_control/
--rw-rw-r--   0 root         (0)     1003     1702 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.429289 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/
--rw-rw-r--   0 root         (0)     1003     1537 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003     1997 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.429289 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.433289 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/
--rw-rw-r--   0 root         (0)     1003      769 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/__init__.py
--rw-rw-r--   0 root         (0)     1003    39516 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/async_client.py
--rw-rw-r--   0 root         (0)     1003    57850 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/client.py
--rw-rw-r--   0 root         (0)     1003     5814 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.433289 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/
--rw-rw-r--   0 root         (0)     1003     1193 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11151 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18214 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18634 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.433289 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/types/
--rw-rw-r--   0 root         (0)     1003     1262 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    19110 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/types/storage_control.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.433289 google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/
--rw-r--r--   0 root         (0)     1003     5200 2024-03-25 19:56:53.000000 google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1590 2024-03-25 19:56:53.000000 google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-25 19:56:53.000000 google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-25 19:56:53.000000 google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-25 19:56:53.000000 google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-25 19:56:53.000000 google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-25 19:56:53.437289 google-cloud-storage-control-0.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3201 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.433289 google-cloud-storage-control-0.1.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.433289 google-cloud-storage-control-0.1.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.437289 google-cloud-storage-control-0.1.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-25 19:56:53.437289 google-cloud-storage-control-0.1.0/tests/unit/gapic/storage_control_v2/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/tests/unit/gapic/storage_control_v2/__init__.py
--rw-rw-r--   0 root         (0)     1003   141583 2024-03-25 19:53:27.000000 google-cloud-storage-control-0.1.0/tests/unit/gapic/storage_control_v2/test_storage_control.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5200 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3812 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.262756 google-cloud-storage-control-0.1.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.262756 google-cloud-storage-control-0.1.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.266756 google-cloud-storage-control-0.1.1/google/cloud/storage_control/
+-rw-rw-r--   0 root         (0)     1003     2064 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/
+-rw-rw-r--   0 root         (0)     1003     1899 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3061 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/
+-rw-rw-r--   0 root         (0)     1003      769 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/__init__.py
+-rw-rw-r--   0 root         (0)     1003    58574 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/async_client.py
+-rw-rw-r--   0 root         (0)     1003    78950 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/client.py
+-rw-rw-r--   0 root         (0)     1003    11060 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/
+-rw-rw-r--   0 root         (0)     1003     1193 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14186 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    22977 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    23517 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.270757 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/
+-rw-rw-r--   0 root         (0)     1003     1624 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27732 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/storage_control.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/
+-rw-r--r--   0 root         (0)     1003     5200 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1590 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-03 01:22:09.000000 google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3201 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 01:22:09.274757 google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   194411 2024-04-03 01:18:25.000000 google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/test_storage_control.py
```

### Comparing `google-cloud-storage-control-0.1.0/LICENSE` & `google-cloud-storage-control-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/MANIFEST.in` & `google-cloud-storage-control-0.1.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/PKG-INFO` & `google-cloud-storage-control-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-control
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Storage Control API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-storage-control-0.1.0/README.rst` & `google-cloud-storage-control-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control/__init__.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,35 +23,47 @@
 )
 from google.cloud.storage_control_v2.services.storage_control.client import (
     StorageControlClient,
 )
 from google.cloud.storage_control_v2.types.storage_control import (
     CommonLongRunningOperationMetadata,
     CreateFolderRequest,
+    CreateManagedFolderRequest,
     DeleteFolderRequest,
+    DeleteManagedFolderRequest,
     Folder,
     GetFolderRequest,
+    GetManagedFolderRequest,
     GetStorageLayoutRequest,
     ListFoldersRequest,
     ListFoldersResponse,
+    ListManagedFoldersRequest,
+    ListManagedFoldersResponse,
+    ManagedFolder,
     PendingRenameInfo,
     RenameFolderMetadata,
     RenameFolderRequest,
     StorageLayout,
 )
 
 __all__ = (
     "StorageControlClient",
     "StorageControlAsyncClient",
     "CommonLongRunningOperationMetadata",
     "CreateFolderRequest",
+    "CreateManagedFolderRequest",
     "DeleteFolderRequest",
+    "DeleteManagedFolderRequest",
     "Folder",
     "GetFolderRequest",
+    "GetManagedFolderRequest",
     "GetStorageLayoutRequest",
     "ListFoldersRequest",
     "ListFoldersResponse",
+    "ListManagedFoldersRequest",
+    "ListManagedFoldersResponse",
+    "ManagedFolder",
     "PendingRenameInfo",
     "RenameFolderMetadata",
     "RenameFolderRequest",
     "StorageLayout",
 )
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control/gapic_version.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/__init__.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,35 +18,47 @@
 __version__ = package_version.__version__
 
 
 from .services.storage_control import StorageControlAsyncClient, StorageControlClient
 from .types.storage_control import (
     CommonLongRunningOperationMetadata,
     CreateFolderRequest,
+    CreateManagedFolderRequest,
     DeleteFolderRequest,
+    DeleteManagedFolderRequest,
     Folder,
     GetFolderRequest,
+    GetManagedFolderRequest,
     GetStorageLayoutRequest,
     ListFoldersRequest,
     ListFoldersResponse,
+    ListManagedFoldersRequest,
+    ListManagedFoldersResponse,
+    ManagedFolder,
     PendingRenameInfo,
     RenameFolderMetadata,
     RenameFolderRequest,
     StorageLayout,
 )
 
 __all__ = (
     "StorageControlAsyncClient",
     "CommonLongRunningOperationMetadata",
     "CreateFolderRequest",
+    "CreateManagedFolderRequest",
     "DeleteFolderRequest",
+    "DeleteManagedFolderRequest",
     "Folder",
     "GetFolderRequest",
+    "GetManagedFolderRequest",
     "GetStorageLayoutRequest",
     "ListFoldersRequest",
     "ListFoldersResponse",
+    "ListManagedFoldersRequest",
+    "ListManagedFoldersResponse",
+    "ManagedFolder",
     "PendingRenameInfo",
     "RenameFolderMetadata",
     "RenameFolderRequest",
     "StorageControlClient",
     "StorageLayout",
 )
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/gapic_metadata.json` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/gapic_metadata.json`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9989583333333334%*

 * *Differences: {"'services'": "{'StorageControl': {'clients': {'grpc': {'rpcs': {'CreateManagedFolder': "*

 * *               "OrderedDict([('methods', ['create_managed_folder'])]), 'DeleteManagedFolder': "*

 * *               "OrderedDict([('methods', ['delete_managed_folder'])]), 'GetManagedFolder': "*

 * *               "OrderedDict([('methods', ['get_managed_folder'])]), 'ListManagedFolders': "*

 * *               "OrderedDict([('methods', ['list_managed_folders'])])}}, 'grpc-async': {'rpcs': "*

 * *               "{'CreateManagedFolder': Ord […]*

```diff
@@ -11,34 +11,54 @@
                     "libraryClient": "StorageControlClient",
                     "rpcs": {
                         "CreateFolder": {
                             "methods": [
                                 "create_folder"
                             ]
                         },
+                        "CreateManagedFolder": {
+                            "methods": [
+                                "create_managed_folder"
+                            ]
+                        },
                         "DeleteFolder": {
                             "methods": [
                                 "delete_folder"
                             ]
                         },
+                        "DeleteManagedFolder": {
+                            "methods": [
+                                "delete_managed_folder"
+                            ]
+                        },
                         "GetFolder": {
                             "methods": [
                                 "get_folder"
                             ]
                         },
+                        "GetManagedFolder": {
+                            "methods": [
+                                "get_managed_folder"
+                            ]
+                        },
                         "GetStorageLayout": {
                             "methods": [
                                 "get_storage_layout"
                             ]
                         },
                         "ListFolders": {
                             "methods": [
                                 "list_folders"
                             ]
                         },
+                        "ListManagedFolders": {
+                            "methods": [
+                                "list_managed_folders"
+                            ]
+                        },
                         "RenameFolder": {
                             "methods": [
                                 "rename_folder"
                             ]
                         }
                     }
                 },
@@ -46,34 +66,54 @@
                     "libraryClient": "StorageControlAsyncClient",
                     "rpcs": {
                         "CreateFolder": {
                             "methods": [
                                 "create_folder"
                             ]
                         },
+                        "CreateManagedFolder": {
+                            "methods": [
+                                "create_managed_folder"
+                            ]
+                        },
                         "DeleteFolder": {
                             "methods": [
                                 "delete_folder"
                             ]
                         },
+                        "DeleteManagedFolder": {
+                            "methods": [
+                                "delete_managed_folder"
+                            ]
+                        },
                         "GetFolder": {
                             "methods": [
                                 "get_folder"
                             ]
                         },
+                        "GetManagedFolder": {
+                            "methods": [
+                                "get_managed_folder"
+                            ]
+                        },
                         "GetStorageLayout": {
                             "methods": [
                                 "get_storage_layout"
                             ]
                         },
                         "ListFolders": {
                             "methods": [
                                 "list_folders"
                             ]
                         },
+                        "ListManagedFolders": {
+                            "methods": [
+                                "list_managed_folders"
+                            ]
+                        },
                         "RenameFolder": {
                             "methods": [
                                 "rename_folder"
                             ]
                         }
                     }
                 }
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/gapic_version.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/gapic_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.0"  # {x-release-please-version}
+__version__ = "0.1.1"  # {x-release-please-version}
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/__init__.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/__init__.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/async_client.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/async_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -68,14 +68,18 @@
     DEFAULT_ENDPOINT = StorageControlClient.DEFAULT_ENDPOINT
     DEFAULT_MTLS_ENDPOINT = StorageControlClient.DEFAULT_MTLS_ENDPOINT
     _DEFAULT_ENDPOINT_TEMPLATE = StorageControlClient._DEFAULT_ENDPOINT_TEMPLATE
     _DEFAULT_UNIVERSE = StorageControlClient._DEFAULT_UNIVERSE
 
     folder_path = staticmethod(StorageControlClient.folder_path)
     parse_folder_path = staticmethod(StorageControlClient.parse_folder_path)
+    managed_folder_path = staticmethod(StorageControlClient.managed_folder_path)
+    parse_managed_folder_path = staticmethod(
+        StorageControlClient.parse_managed_folder_path
+    )
     storage_layout_path = staticmethod(StorageControlClient.storage_layout_path)
     parse_storage_layout_path = staticmethod(
         StorageControlClient.parse_storage_layout_path
     )
     common_billing_account_path = staticmethod(
         StorageControlClient.common_billing_account_path
     )
@@ -320,16 +324,20 @@
                 parent and folder_id fields, respectively. Populating
                 those fields in ``folder`` will result in an error.
 
                 This corresponds to the ``folder`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             folder_id (:class:`str`):
-                Required. The absolute path of the folder, using a
-                single ``/`` as delimiter.
+                Required. The full name of a folder, including all its
+                parent folders. Folders use single '/' characters as a
+                delimiter. The folder_id must end with a slash. For
+                example, the folder_id of "books/biographies/" would
+                create a new "biographies/" folder under the "books/"
+                folder.
 
                 This corresponds to the ``folder_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -964,14 +972,476 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    async def create_managed_folder(
+        self,
+        request: Optional[
+            Union[storage_control.CreateManagedFolderRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        managed_folder: Optional[storage_control.ManagedFolder] = None,
+        managed_folder_id: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> storage_control.ManagedFolder:
+        r"""Creates a new managed folder.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import storage_control_v2
+
+            async def sample_create_managed_folder():
+                # Create a client
+                client = storage_control_v2.StorageControlAsyncClient()
+
+                # Initialize request argument(s)
+                request = storage_control_v2.CreateManagedFolderRequest(
+                    parent="parent_value",
+                    managed_folder_id="managed_folder_id_value",
+                )
+
+                # Make the request
+                response = await client.create_managed_folder(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.storage_control_v2.types.CreateManagedFolderRequest, dict]]):
+                The request object. Request message for
+                CreateManagedFolder.
+            parent (:class:`str`):
+                Required. Name of the bucket this
+                managed folder belongs to.
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            managed_folder (:class:`google.cloud.storage_control_v2.types.ManagedFolder`):
+                Required. Properties of the managed folder being
+                created. The bucket and managed folder names are
+                specified in the ``parent`` and ``managed_folder_id``
+                fields. Populating these fields in ``managed_folder``
+                will result in an error.
+
+                This corresponds to the ``managed_folder`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            managed_folder_id (:class:`str`):
+                Required. The name of the managed folder. It uses a
+                single ``/`` as delimiter and leading and trailing ``/``
+                are allowed.
+
+                This corresponds to the ``managed_folder_id`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.storage_control_v2.types.ManagedFolder:
+                A managed folder.
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent, managed_folder, managed_folder_id])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = storage_control.CreateManagedFolderRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
+        if managed_folder is not None:
+            request.managed_folder = managed_folder
+        if managed_folder_id is not None:
+            request.managed_folder_id = managed_folder_id
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.create_managed_folder,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        if not request.request_id:
+            request.request_id = str(uuid.uuid4())
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def delete_managed_folder(
+        self,
+        request: Optional[
+            Union[storage_control.DeleteManagedFolderRequest, dict]
+        ] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Permanently deletes an empty managed folder.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import storage_control_v2
+
+            async def sample_delete_managed_folder():
+                # Create a client
+                client = storage_control_v2.StorageControlAsyncClient()
+
+                # Initialize request argument(s)
+                request = storage_control_v2.DeleteManagedFolderRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                await client.delete_managed_folder(request=request)
+
+        Args:
+            request (Optional[Union[google.cloud.storage_control_v2.types.DeleteManagedFolderRequest, dict]]):
+                The request object. DeleteManagedFolder RPC request
+                message.
+            name (:class:`str`):
+                Required. Name of the managed folder. Format:
+                ``projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = storage_control.DeleteManagedFolderRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.delete_managed_folder,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        if not request.request_id:
+            request.request_id = str(uuid.uuid4())
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+    async def get_managed_folder(
+        self,
+        request: Optional[Union[storage_control.GetManagedFolderRequest, dict]] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> storage_control.ManagedFolder:
+        r"""Returns metadata for the specified managed folder.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import storage_control_v2
+
+            async def sample_get_managed_folder():
+                # Create a client
+                client = storage_control_v2.StorageControlAsyncClient()
+
+                # Initialize request argument(s)
+                request = storage_control_v2.GetManagedFolderRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = await client.get_managed_folder(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.storage_control_v2.types.GetManagedFolderRequest, dict]]):
+                The request object. Request message for GetManagedFolder.
+            name (:class:`str`):
+                Required. Name of the managed folder. Format:
+                ``projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.storage_control_v2.types.ManagedFolder:
+                A managed folder.
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = storage_control.GetManagedFolderRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if name is not None:
+            request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.get_managed_folder,
+            default_retry=retries.AsyncRetry(
+                initial=1.0,
+                maximum=60.0,
+                multiplier=2,
+                predicate=retries.if_exception_type(
+                    core_exceptions.DeadlineExceeded,
+                    core_exceptions.InternalServerError,
+                    core_exceptions.ResourceExhausted,
+                    core_exceptions.ServiceUnavailable,
+                    core_exceptions.Unknown,
+                ),
+                deadline=60.0,
+            ),
+            default_timeout=60.0,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        if not request.request_id:
+            request.request_id = str(uuid.uuid4())
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_managed_folders(
+        self,
+        request: Optional[
+            Union[storage_control.ListManagedFoldersRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListManagedFoldersAsyncPager:
+        r"""Retrieves a list of managed folders for a given
+        bucket.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import storage_control_v2
+
+            async def sample_list_managed_folders():
+                # Create a client
+                client = storage_control_v2.StorageControlAsyncClient()
+
+                # Initialize request argument(s)
+                request = storage_control_v2.ListManagedFoldersRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_managed_folders(request=request)
+
+                # Handle the response
+                async for response in page_result:
+                    print(response)
+
+        Args:
+            request (Optional[Union[google.cloud.storage_control_v2.types.ListManagedFoldersRequest, dict]]):
+                The request object. Request message for
+                ListManagedFolders.
+            parent (:class:`str`):
+                Required. Name of the bucket this
+                managed folder belongs to.
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry_async.AsyncRetry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.storage_control_v2.services.storage_control.pagers.ListManagedFoldersAsyncPager:
+                Response message for
+                ListManagedFolders.
+                Iterating over this object will yield
+                results and resolve additional pages
+                automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        request = storage_control.ListManagedFoldersRequest(request)
+
+        # If we have keyword arguments corresponding to fields on the
+        # request, apply these.
+        if parent is not None:
+            request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method_async.wrap_method(
+            self._client._transport.list_managed_folders,
+            default_retry=retries.AsyncRetry(
+                initial=1.0,
+                maximum=60.0,
+                multiplier=2,
+                predicate=retries.if_exception_type(
+                    core_exceptions.DeadlineExceeded,
+                    core_exceptions.InternalServerError,
+                    core_exceptions.ResourceExhausted,
+                    core_exceptions.ServiceUnavailable,
+                    core_exceptions.Unknown,
+                ),
+                deadline=60.0,
+            ),
+            default_timeout=60.0,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        if not request.request_id:
+            request.request_id = str(uuid.uuid4())
+
+        # Validate the universe domain.
+        self._client._validate_universe_domain()
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__aiter__` convenience method.
+        response = pagers.ListManagedFoldersAsyncPager(
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     async def __aenter__(self) -> "StorageControlAsyncClient":
         return self
 
     async def __aexit__(self, exc_type, exc, tb):
         await self.transport.close()
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/client.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -207,14 +207,38 @@
         m = re.match(
             r"^projects/(?P<project>.+?)/buckets/(?P<bucket>.+?)/folders/(?P<folder>.+?)$",
             path,
         )
         return m.groupdict() if m else {}
 
     @staticmethod
+    def managed_folder_path(
+        project: str,
+        bucket: str,
+        managedFolder: str,
+    ) -> str:
+        """Returns a fully-qualified managed_folder string."""
+        return (
+            "projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}".format(
+                project=project,
+                bucket=bucket,
+                managedFolder=managedFolder,
+            )
+        )
+
+    @staticmethod
+    def parse_managed_folder_path(path: str) -> Dict[str, str]:
+        """Parses a managed_folder path into its component segments."""
+        m = re.match(
+            r"^projects/(?P<project>.+?)/buckets/(?P<bucket>.+?)/managedFolders/(?P<managedFolder>.+?)$",
+            path,
+        )
+        return m.groupdict() if m else {}
+
+    @staticmethod
     def storage_layout_path(
         project: str,
         bucket: str,
     ) -> str:
         """Returns a fully-qualified storage_layout string."""
         return "projects/{project}/buckets/{bucket}/storageLayout".format(
             project=project,
@@ -746,16 +770,20 @@
                 parent and folder_id fields, respectively. Populating
                 those fields in ``folder`` will result in an error.
 
                 This corresponds to the ``folder`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             folder_id (str):
-                Required. The absolute path of the folder, using a
-                single ``/`` as delimiter.
+                Required. The full name of a folder, including all its
+                parent folders. Folders use single '/' characters as a
+                delimiter. The folder_id must end with a slash. For
+                example, the folder_id of "books/biographies/" would
+                create a new "biographies/" folder under the "books/"
+                folder.
 
                 This corresponds to the ``folder_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1418,14 +1446,502 @@
             timeout=timeout,
             metadata=metadata,
         )
 
         # Done; return the response.
         return response
 
+    def create_managed_folder(
+        self,
+        request: Optional[
+            Union[storage_control.CreateManagedFolderRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        managed_folder: Optional[storage_control.ManagedFolder] = None,
+        managed_folder_id: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> storage_control.ManagedFolder:
+        r"""Creates a new managed folder.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import storage_control_v2
+
+            def sample_create_managed_folder():
+                # Create a client
+                client = storage_control_v2.StorageControlClient()
+
+                # Initialize request argument(s)
+                request = storage_control_v2.CreateManagedFolderRequest(
+                    parent="parent_value",
+                    managed_folder_id="managed_folder_id_value",
+                )
+
+                # Make the request
+                response = client.create_managed_folder(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.storage_control_v2.types.CreateManagedFolderRequest, dict]):
+                The request object. Request message for
+                CreateManagedFolder.
+            parent (str):
+                Required. Name of the bucket this
+                managed folder belongs to.
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            managed_folder (google.cloud.storage_control_v2.types.ManagedFolder):
+                Required. Properties of the managed folder being
+                created. The bucket and managed folder names are
+                specified in the ``parent`` and ``managed_folder_id``
+                fields. Populating these fields in ``managed_folder``
+                will result in an error.
+
+                This corresponds to the ``managed_folder`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            managed_folder_id (str):
+                Required. The name of the managed folder. It uses a
+                single ``/`` as delimiter and leading and trailing ``/``
+                are allowed.
+
+                This corresponds to the ``managed_folder_id`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.storage_control_v2.types.ManagedFolder:
+                A managed folder.
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent, managed_folder, managed_folder_id])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a storage_control.CreateManagedFolderRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, storage_control.CreateManagedFolderRequest):
+            request = storage_control.CreateManagedFolderRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+            if managed_folder is not None:
+                request.managed_folder = managed_folder
+            if managed_folder_id is not None:
+                request.managed_folder_id = managed_folder_id
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.create_managed_folder]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<bucket>.*)$")
+        regex_match = routing_param_regex.match(request.parent)
+        if regex_match and regex_match.group("bucket"):
+            header_params["bucket"] = regex_match.group("bucket")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
+
+        if not request.request_id:
+            request.request_id = str(uuid.uuid4())
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def delete_managed_folder(
+        self,
+        request: Optional[
+            Union[storage_control.DeleteManagedFolderRequest, dict]
+        ] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Permanently deletes an empty managed folder.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import storage_control_v2
+
+            def sample_delete_managed_folder():
+                # Create a client
+                client = storage_control_v2.StorageControlClient()
+
+                # Initialize request argument(s)
+                request = storage_control_v2.DeleteManagedFolderRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                client.delete_managed_folder(request=request)
+
+        Args:
+            request (Union[google.cloud.storage_control_v2.types.DeleteManagedFolderRequest, dict]):
+                The request object. DeleteManagedFolder RPC request
+                message.
+            name (str):
+                Required. Name of the managed folder. Format:
+                ``projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a storage_control.DeleteManagedFolderRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, storage_control.DeleteManagedFolderRequest):
+            request = storage_control.DeleteManagedFolderRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.delete_managed_folder]
+
+        header_params = {}
+
+        routing_param_regex = re.compile(
+            "^(?P<bucket>projects/[^/]+/buckets/[^/]+)(?:/.*)?$"
+        )
+        regex_match = routing_param_regex.match(request.name)
+        if regex_match and regex_match.group("bucket"):
+            header_params["bucket"] = regex_match.group("bucket")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
+
+        if not request.request_id:
+            request.request_id = str(uuid.uuid4())
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+    def get_managed_folder(
+        self,
+        request: Optional[Union[storage_control.GetManagedFolderRequest, dict]] = None,
+        *,
+        name: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> storage_control.ManagedFolder:
+        r"""Returns metadata for the specified managed folder.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import storage_control_v2
+
+            def sample_get_managed_folder():
+                # Create a client
+                client = storage_control_v2.StorageControlClient()
+
+                # Initialize request argument(s)
+                request = storage_control_v2.GetManagedFolderRequest(
+                    name="name_value",
+                )
+
+                # Make the request
+                response = client.get_managed_folder(request=request)
+
+                # Handle the response
+                print(response)
+
+        Args:
+            request (Union[google.cloud.storage_control_v2.types.GetManagedFolderRequest, dict]):
+                The request object. Request message for GetManagedFolder.
+            name (str):
+                Required. Name of the managed folder. Format:
+                ``projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}``
+
+                This corresponds to the ``name`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.storage_control_v2.types.ManagedFolder:
+                A managed folder.
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([name])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a storage_control.GetManagedFolderRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, storage_control.GetManagedFolderRequest):
+            request = storage_control.GetManagedFolderRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if name is not None:
+                request.name = name
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.get_managed_folder]
+
+        header_params = {}
+
+        routing_param_regex = re.compile(
+            "^(?P<bucket>projects/[^/]+/buckets/[^/]+)(?:/.*)?$"
+        )
+        regex_match = routing_param_regex.match(request.name)
+        if regex_match and regex_match.group("bucket"):
+            header_params["bucket"] = regex_match.group("bucket")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
+
+        if not request.request_id:
+            request.request_id = str(uuid.uuid4())
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_managed_folders(
+        self,
+        request: Optional[
+            Union[storage_control.ListManagedFoldersRequest, dict]
+        ] = None,
+        *,
+        parent: Optional[str] = None,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> pagers.ListManagedFoldersPager:
+        r"""Retrieves a list of managed folders for a given
+        bucket.
+
+        .. code-block:: python
+
+            # This snippet has been automatically generated and should be regarded as a
+            # code template only.
+            # It will require modifications to work:
+            # - It may require correct/in-range values for request initialization.
+            # - It may require specifying regional endpoints when creating the service
+            #   client as shown in:
+            #   https://googleapis.dev/python/google-api-core/latest/client_options.html
+            from google.cloud import storage_control_v2
+
+            def sample_list_managed_folders():
+                # Create a client
+                client = storage_control_v2.StorageControlClient()
+
+                # Initialize request argument(s)
+                request = storage_control_v2.ListManagedFoldersRequest(
+                    parent="parent_value",
+                )
+
+                # Make the request
+                page_result = client.list_managed_folders(request=request)
+
+                # Handle the response
+                for response in page_result:
+                    print(response)
+
+        Args:
+            request (Union[google.cloud.storage_control_v2.types.ListManagedFoldersRequest, dict]):
+                The request object. Request message for
+                ListManagedFolders.
+            parent (str):
+                Required. Name of the bucket this
+                managed folder belongs to.
+
+                This corresponds to the ``parent`` field
+                on the ``request`` instance; if ``request`` is provided, this
+                should not be set.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+
+        Returns:
+            google.cloud.storage_control_v2.services.storage_control.pagers.ListManagedFoldersPager:
+                Response message for
+                ListManagedFolders.
+                Iterating over this object will yield
+                results and resolve additional pages
+                automatically.
+
+        """
+        # Create or coerce a protobuf request object.
+        # Quick check: If we got a request object, we should *not* have
+        # gotten any keyword arguments that map to the request.
+        has_flattened_params = any([parent])
+        if request is not None and has_flattened_params:
+            raise ValueError(
+                "If the `request` argument is set, then none of "
+                "the individual field arguments should be set."
+            )
+
+        # Minor optimization to avoid making a copy if the user passes
+        # in a storage_control.ListManagedFoldersRequest.
+        # There's no risk of modifying the input as we've already verified
+        # there are no flattened fields.
+        if not isinstance(request, storage_control.ListManagedFoldersRequest):
+            request = storage_control.ListManagedFoldersRequest(request)
+            # If we have keyword arguments corresponding to fields on the
+            # request, apply these.
+            if parent is not None:
+                request.parent = parent
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = self._transport._wrapped_methods[self._transport.list_managed_folders]
+
+        header_params = {}
+
+        routing_param_regex = re.compile("^(?P<bucket>.*)$")
+        regex_match = routing_param_regex.match(request.parent)
+        if regex_match and regex_match.group("bucket"):
+            header_params["bucket"] = regex_match.group("bucket")
+
+        if header_params:
+            metadata = tuple(metadata) + (
+                gapic_v1.routing_header.to_grpc_metadata(header_params),
+            )
+
+        if not request.request_id:
+            request.request_id = str(uuid.uuid4())
+
+        # Validate the universe domain.
+        self._validate_universe_domain()
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # This method is paged; wrap the response in a pager, which provides
+        # an `__iter__` convenience method.
+        response = pagers.ListManagedFoldersPager(
+            method=rpc,
+            request=request,
+            response=response,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
     def __enter__(self) -> "StorageControlClient":
         return self
 
     def __exit__(self, type, value, traceback):
         """Releases underlying transport's resources.
 
         .. warning::
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/base.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -212,14 +212,60 @@
                         core_exceptions.Unknown,
                     ),
                     deadline=60.0,
                 ),
                 default_timeout=60.0,
                 client_info=client_info,
             ),
+            self.create_managed_folder: gapic_v1.method.wrap_method(
+                self.create_managed_folder,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.delete_managed_folder: gapic_v1.method.wrap_method(
+                self.delete_managed_folder,
+                default_timeout=None,
+                client_info=client_info,
+            ),
+            self.get_managed_folder: gapic_v1.method.wrap_method(
+                self.get_managed_folder,
+                default_retry=retries.Retry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=2,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.InternalServerError,
+                        core_exceptions.ResourceExhausted,
+                        core_exceptions.ServiceUnavailable,
+                        core_exceptions.Unknown,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
+            self.list_managed_folders: gapic_v1.method.wrap_method(
+                self.list_managed_folders,
+                default_retry=retries.Retry(
+                    initial=1.0,
+                    maximum=60.0,
+                    multiplier=2,
+                    predicate=retries.if_exception_type(
+                        core_exceptions.DeadlineExceeded,
+                        core_exceptions.InternalServerError,
+                        core_exceptions.ResourceExhausted,
+                        core_exceptions.ServiceUnavailable,
+                        core_exceptions.Unknown,
+                    ),
+                    deadline=60.0,
+                ),
+                default_timeout=60.0,
+                client_info=client_info,
+            ),
         }
 
     def close(self):
         """Closes resources associated with the transport.
 
         .. warning::
              Only call this method if the transport is NOT shared
@@ -286,12 +332,51 @@
     ) -> Callable[
         [storage_control.GetStorageLayoutRequest],
         Union[storage_control.StorageLayout, Awaitable[storage_control.StorageLayout]],
     ]:
         raise NotImplementedError()
 
     @property
+    def create_managed_folder(
+        self,
+    ) -> Callable[
+        [storage_control.CreateManagedFolderRequest],
+        Union[storage_control.ManagedFolder, Awaitable[storage_control.ManagedFolder]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def delete_managed_folder(
+        self,
+    ) -> Callable[
+        [storage_control.DeleteManagedFolderRequest],
+        Union[empty_pb2.Empty, Awaitable[empty_pb2.Empty]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def get_managed_folder(
+        self,
+    ) -> Callable[
+        [storage_control.GetManagedFolderRequest],
+        Union[storage_control.ManagedFolder, Awaitable[storage_control.ManagedFolder]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_managed_folders(
+        self,
+    ) -> Callable[
+        [storage_control.ListManagedFoldersRequest],
+        Union[
+            storage_control.ListManagedFoldersResponse,
+            Awaitable[storage_control.ListManagedFoldersResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("StorageControlTransport",)
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/grpc.py`

 * *Files 10% similar despite different names*

```diff
@@ -405,14 +405,126 @@
             self._stubs["get_storage_layout"] = self.grpc_channel.unary_unary(
                 "/google.storage.control.v2.StorageControl/GetStorageLayout",
                 request_serializer=storage_control.GetStorageLayoutRequest.serialize,
                 response_deserializer=storage_control.StorageLayout.deserialize,
             )
         return self._stubs["get_storage_layout"]
 
+    @property
+    def create_managed_folder(
+        self,
+    ) -> Callable[
+        [storage_control.CreateManagedFolderRequest], storage_control.ManagedFolder
+    ]:
+        r"""Return a callable for the create managed folder method over gRPC.
+
+        Creates a new managed folder.
+
+        Returns:
+            Callable[[~.CreateManagedFolderRequest],
+                    ~.ManagedFolder]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "create_managed_folder" not in self._stubs:
+            self._stubs["create_managed_folder"] = self.grpc_channel.unary_unary(
+                "/google.storage.control.v2.StorageControl/CreateManagedFolder",
+                request_serializer=storage_control.CreateManagedFolderRequest.serialize,
+                response_deserializer=storage_control.ManagedFolder.deserialize,
+            )
+        return self._stubs["create_managed_folder"]
+
+    @property
+    def delete_managed_folder(
+        self,
+    ) -> Callable[[storage_control.DeleteManagedFolderRequest], empty_pb2.Empty]:
+        r"""Return a callable for the delete managed folder method over gRPC.
+
+        Permanently deletes an empty managed folder.
+
+        Returns:
+            Callable[[~.DeleteManagedFolderRequest],
+                    ~.Empty]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "delete_managed_folder" not in self._stubs:
+            self._stubs["delete_managed_folder"] = self.grpc_channel.unary_unary(
+                "/google.storage.control.v2.StorageControl/DeleteManagedFolder",
+                request_serializer=storage_control.DeleteManagedFolderRequest.serialize,
+                response_deserializer=empty_pb2.Empty.FromString,
+            )
+        return self._stubs["delete_managed_folder"]
+
+    @property
+    def get_managed_folder(
+        self,
+    ) -> Callable[
+        [storage_control.GetManagedFolderRequest], storage_control.ManagedFolder
+    ]:
+        r"""Return a callable for the get managed folder method over gRPC.
+
+        Returns metadata for the specified managed folder.
+
+        Returns:
+            Callable[[~.GetManagedFolderRequest],
+                    ~.ManagedFolder]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_managed_folder" not in self._stubs:
+            self._stubs["get_managed_folder"] = self.grpc_channel.unary_unary(
+                "/google.storage.control.v2.StorageControl/GetManagedFolder",
+                request_serializer=storage_control.GetManagedFolderRequest.serialize,
+                response_deserializer=storage_control.ManagedFolder.deserialize,
+            )
+        return self._stubs["get_managed_folder"]
+
+    @property
+    def list_managed_folders(
+        self,
+    ) -> Callable[
+        [storage_control.ListManagedFoldersRequest],
+        storage_control.ListManagedFoldersResponse,
+    ]:
+        r"""Return a callable for the list managed folders method over gRPC.
+
+        Retrieves a list of managed folders for a given
+        bucket.
+
+        Returns:
+            Callable[[~.ListManagedFoldersRequest],
+                    ~.ListManagedFoldersResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_managed_folders" not in self._stubs:
+            self._stubs["list_managed_folders"] = self.grpc_channel.unary_unary(
+                "/google.storage.control.v2.StorageControl/ListManagedFolders",
+                request_serializer=storage_control.ListManagedFoldersRequest.serialize,
+                response_deserializer=storage_control.ListManagedFoldersResponse.deserialize,
+            )
+        return self._stubs["list_managed_folders"]
+
     def close(self):
         self.grpc_channel.close()
 
     @property
     def kind(self) -> str:
         return "grpc"
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/services/storage_control/transports/grpc_asyncio.py`

 * *Files 16% similar despite different names*

```diff
@@ -418,12 +418,128 @@
             self._stubs["get_storage_layout"] = self.grpc_channel.unary_unary(
                 "/google.storage.control.v2.StorageControl/GetStorageLayout",
                 request_serializer=storage_control.GetStorageLayoutRequest.serialize,
                 response_deserializer=storage_control.StorageLayout.deserialize,
             )
         return self._stubs["get_storage_layout"]
 
+    @property
+    def create_managed_folder(
+        self,
+    ) -> Callable[
+        [storage_control.CreateManagedFolderRequest],
+        Awaitable[storage_control.ManagedFolder],
+    ]:
+        r"""Return a callable for the create managed folder method over gRPC.
+
+        Creates a new managed folder.
+
+        Returns:
+            Callable[[~.CreateManagedFolderRequest],
+                    Awaitable[~.ManagedFolder]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "create_managed_folder" not in self._stubs:
+            self._stubs["create_managed_folder"] = self.grpc_channel.unary_unary(
+                "/google.storage.control.v2.StorageControl/CreateManagedFolder",
+                request_serializer=storage_control.CreateManagedFolderRequest.serialize,
+                response_deserializer=storage_control.ManagedFolder.deserialize,
+            )
+        return self._stubs["create_managed_folder"]
+
+    @property
+    def delete_managed_folder(
+        self,
+    ) -> Callable[
+        [storage_control.DeleteManagedFolderRequest], Awaitable[empty_pb2.Empty]
+    ]:
+        r"""Return a callable for the delete managed folder method over gRPC.
+
+        Permanently deletes an empty managed folder.
+
+        Returns:
+            Callable[[~.DeleteManagedFolderRequest],
+                    Awaitable[~.Empty]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "delete_managed_folder" not in self._stubs:
+            self._stubs["delete_managed_folder"] = self.grpc_channel.unary_unary(
+                "/google.storage.control.v2.StorageControl/DeleteManagedFolder",
+                request_serializer=storage_control.DeleteManagedFolderRequest.serialize,
+                response_deserializer=empty_pb2.Empty.FromString,
+            )
+        return self._stubs["delete_managed_folder"]
+
+    @property
+    def get_managed_folder(
+        self,
+    ) -> Callable[
+        [storage_control.GetManagedFolderRequest],
+        Awaitable[storage_control.ManagedFolder],
+    ]:
+        r"""Return a callable for the get managed folder method over gRPC.
+
+        Returns metadata for the specified managed folder.
+
+        Returns:
+            Callable[[~.GetManagedFolderRequest],
+                    Awaitable[~.ManagedFolder]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_managed_folder" not in self._stubs:
+            self._stubs["get_managed_folder"] = self.grpc_channel.unary_unary(
+                "/google.storage.control.v2.StorageControl/GetManagedFolder",
+                request_serializer=storage_control.GetManagedFolderRequest.serialize,
+                response_deserializer=storage_control.ManagedFolder.deserialize,
+            )
+        return self._stubs["get_managed_folder"]
+
+    @property
+    def list_managed_folders(
+        self,
+    ) -> Callable[
+        [storage_control.ListManagedFoldersRequest],
+        Awaitable[storage_control.ListManagedFoldersResponse],
+    ]:
+        r"""Return a callable for the list managed folders method over gRPC.
+
+        Retrieves a list of managed folders for a given
+        bucket.
+
+        Returns:
+            Callable[[~.ListManagedFoldersRequest],
+                    Awaitable[~.ListManagedFoldersResponse]]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_managed_folders" not in self._stubs:
+            self._stubs["list_managed_folders"] = self.grpc_channel.unary_unary(
+                "/google.storage.control.v2.StorageControl/ListManagedFolders",
+                request_serializer=storage_control.ListManagedFoldersRequest.serialize,
+                response_deserializer=storage_control.ListManagedFoldersResponse.deserialize,
+            )
+        return self._stubs["list_managed_folders"]
+
     def close(self):
         return self.grpc_channel.close()
 
 
 __all__ = ("StorageControlGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-storage-control-0.1.0/google/cloud/storage_control_v2/types/storage_control.py` & `google-cloud-storage-control-0.1.1/google/cloud/storage_control_v2/types/storage_control.py`

 * *Files 21% similar despite different names*

```diff
@@ -31,14 +31,20 @@
         "ListFoldersRequest",
         "ListFoldersResponse",
         "RenameFolderRequest",
         "CommonLongRunningOperationMetadata",
         "RenameFolderMetadata",
         "StorageLayout",
         "GetStorageLayoutRequest",
+        "ManagedFolder",
+        "GetManagedFolderRequest",
+        "CreateManagedFolderRequest",
+        "DeleteManagedFolderRequest",
+        "ListManagedFoldersRequest",
+        "ListManagedFoldersResponse",
     },
 )
 
 
 class PendingRenameInfo(proto.Message):
     r"""Contains information about a pending rename operation.
 
@@ -161,16 +167,19 @@
             folder will reside.
         folder (google.cloud.storage_control_v2.types.Folder):
             Required. Properties of the new folder being created. The
             bucket and name of the folder are specified in the parent
             and folder_id fields, respectively. Populating those fields
             in ``folder`` will result in an error.
         folder_id (str):
-            Required. The absolute path of the folder, using a single
-            ``/`` as delimiter.
+            Required. The full name of a folder, including all its
+            parent folders. Folders use single '/' characters as a
+            delimiter. The folder_id must end with a slash. For example,
+            the folder_id of "books/biographies/" would create a new
+            "biographies/" folder under the "books/" folder.
         recursive (bool):
             Optional. If true, parent folder doesn't have
             to be present and all missing ancestor folders
             will be created atomically.
         request_id (str):
             Optional. A unique identifier for this request. UUID is the
             recommended format, but other formats are still accepted.
@@ -598,8 +607,269 @@
     )
     request_id: str = proto.Field(
         proto.STRING,
         number=3,
     )
 
 
+class ManagedFolder(proto.Message):
+    r"""A managed folder.
+
+    Attributes:
+        name (str):
+            Identifier. The name of this managed folder. Format:
+            ``projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}``
+        metageneration (int):
+            Output only. The metadata version of this
+            managed folder. It increases whenever the
+            metadata is updated. Used for preconditions and
+            for detecting changes in metadata. Managed
+            folders don't have a generation number.
+        create_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The creation time of the managed
+            folder.
+        update_time (google.protobuf.timestamp_pb2.Timestamp):
+            Output only. The modification time of the
+            managed folder.
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    metageneration: int = proto.Field(
+        proto.INT64,
+        number=3,
+    )
+    create_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=4,
+        message=timestamp_pb2.Timestamp,
+    )
+    update_time: timestamp_pb2.Timestamp = proto.Field(
+        proto.MESSAGE,
+        number=5,
+        message=timestamp_pb2.Timestamp,
+    )
+
+
+class GetManagedFolderRequest(proto.Message):
+    r"""Request message for GetManagedFolder.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        name (str):
+            Required. Name of the managed folder. Format:
+            ``projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}``
+        if_metageneration_match (int):
+            The operation succeeds conditional on the
+            managed folder's current metageneration matching
+            the value here specified.
+
+            This field is a member of `oneof`_ ``_if_metageneration_match``.
+        if_metageneration_not_match (int):
+            The operation succeeds conditional on the
+            managed folder's current metageneration NOT
+            matching the value here specified.
+
+            This field is a member of `oneof`_ ``_if_metageneration_not_match``.
+        request_id (str):
+            Optional. A unique identifier for this
+            request. UUID is the recommended format, but
+            other formats are still accepted.
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+    if_metageneration_match: int = proto.Field(
+        proto.INT64,
+        number=3,
+        optional=True,
+    )
+    if_metageneration_not_match: int = proto.Field(
+        proto.INT64,
+        number=4,
+        optional=True,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+
+
+class CreateManagedFolderRequest(proto.Message):
+    r"""Request message for CreateManagedFolder.
+
+    Attributes:
+        parent (str):
+            Required. Name of the bucket this managed
+            folder belongs to.
+        managed_folder (google.cloud.storage_control_v2.types.ManagedFolder):
+            Required. Properties of the managed folder being created.
+            The bucket and managed folder names are specified in the
+            ``parent`` and ``managed_folder_id`` fields. Populating
+            these fields in ``managed_folder`` will result in an error.
+        managed_folder_id (str):
+            Required. The name of the managed folder. It uses a single
+            ``/`` as delimiter and leading and trailing ``/`` are
+            allowed.
+        request_id (str):
+            Optional. A unique identifier for this
+            request. UUID is the recommended format, but
+            other formats are still accepted.
+    """
+
+    parent: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    managed_folder: "ManagedFolder" = proto.Field(
+        proto.MESSAGE,
+        number=2,
+        message="ManagedFolder",
+    )
+    managed_folder_id: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+
+
+class DeleteManagedFolderRequest(proto.Message):
+    r"""DeleteManagedFolder RPC request message.
+
+    .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
+
+    Attributes:
+        name (str):
+            Required. Name of the managed folder. Format:
+            ``projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}``
+        if_metageneration_match (int):
+            The operation succeeds conditional on the
+            managed folder's current metageneration matching
+            the value here specified.
+
+            This field is a member of `oneof`_ ``_if_metageneration_match``.
+        if_metageneration_not_match (int):
+            The operation succeeds conditional on the
+            managed folder's current metageneration NOT
+            matching the value here specified.
+
+            This field is a member of `oneof`_ ``_if_metageneration_not_match``.
+        allow_non_empty (bool):
+            Allows deletion of a managed folder even if
+            it is not empty. A managed folder is empty if it
+            manages no child managed folders or objects.
+            Caller must have permission for
+            storage.managedFolders.setIamPolicy.
+        request_id (str):
+            Optional. A unique identifier for this
+            request. UUID is the recommended format, but
+            other formats are still accepted.
+    """
+
+    name: str = proto.Field(
+        proto.STRING,
+        number=7,
+    )
+    if_metageneration_match: int = proto.Field(
+        proto.INT64,
+        number=3,
+        optional=True,
+    )
+    if_metageneration_not_match: int = proto.Field(
+        proto.INT64,
+        number=4,
+        optional=True,
+    )
+    allow_non_empty: bool = proto.Field(
+        proto.BOOL,
+        number=5,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=6,
+    )
+
+
+class ListManagedFoldersRequest(proto.Message):
+    r"""Request message for ListManagedFolders.
+
+    Attributes:
+        parent (str):
+            Required. Name of the bucket this managed
+            folder belongs to.
+        page_size (int):
+            Optional. Maximum number of managed folders
+            to return in a single response. The service will
+            use this parameter or 1,000 items, whichever is
+            smaller.
+        page_token (str):
+            Optional. A previously-returned page token
+            representing part of the larger set of results
+            to view.
+        prefix (str):
+            Optional. Filter results to match managed
+            folders with name starting with this prefix.
+        request_id (str):
+            Optional. A unique identifier for this
+            request. UUID is the recommended format, but
+            other formats are still accepted.
+    """
+
+    parent: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
+    page_size: int = proto.Field(
+        proto.INT32,
+        number=2,
+    )
+    page_token: str = proto.Field(
+        proto.STRING,
+        number=3,
+    )
+    prefix: str = proto.Field(
+        proto.STRING,
+        number=4,
+    )
+    request_id: str = proto.Field(
+        proto.STRING,
+        number=5,
+    )
+
+
+class ListManagedFoldersResponse(proto.Message):
+    r"""Response message for ListManagedFolders.
+
+    Attributes:
+        managed_folders (MutableSequence[google.cloud.storage_control_v2.types.ManagedFolder]):
+            The list of matching managed folders
+        next_page_token (str):
+            The continuation token, used to page through
+            large result sets. Provide this value in a
+            subsequent request to return the next page of
+            results.
+    """
+
+    @property
+    def raw_page(self):
+        return self
+
+    managed_folders: MutableSequence["ManagedFolder"] = proto.RepeatedField(
+        proto.MESSAGE,
+        number=1,
+        message="ManagedFolder",
+    )
+    next_page_token: str = proto.Field(
+        proto.STRING,
+        number=2,
+    )
+
+
 __all__ = tuple(sorted(__protobuf__.manifest))
```

### Comparing `google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/PKG-INFO` & `google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-storage-control
-Version: 0.1.0
+Version: 0.1.1
 Summary: Google Cloud Storage Control API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-storage-control
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-storage-control-0.1.0/google_cloud_storage_control.egg-info/SOURCES.txt` & `google-cloud-storage-control-0.1.1/google_cloud_storage_control.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/setup.py` & `google-cloud-storage-control-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/tests/__init__.py` & `google-cloud-storage-control-0.1.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/tests/unit/__init__.py` & `google-cloud-storage-control-0.1.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/tests/unit/gapic/__init__.py` & `google-cloud-storage-control-0.1.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/tests/unit/gapic/storage_control_v2/__init__.py` & `google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-storage-control-0.1.0/tests/unit/gapic/storage_control_v2/test_storage_control.py` & `google-cloud-storage-control-0.1.1/tests/unit/gapic/storage_control_v2/test_storage_control.py`

 * *Files 23% similar despite different names*

```diff
@@ -2988,14 +2988,1407 @@
     with pytest.raises(ValueError):
         await client.get_storage_layout(
             storage_control.GetStorageLayoutRequest(),
             name="name_value",
         )
 
 
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        storage_control.CreateManagedFolderRequest,
+        dict,
+    ],
+)
+def test_create_managed_folder(request_type, transport: str = "grpc"):
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+    if isinstance(request, dict):
+        request["request_id"] = "explicit value for autopopulate-able field"
+    else:
+        request.request_id = "explicit value for autopopulate-able field"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ManagedFolder(
+            name="name_value",
+            metageneration=1491,
+        )
+        response = client.create_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = storage_control.CreateManagedFolderRequest()
+        request.request_id = "explicit value for autopopulate-able field"
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, storage_control.ManagedFolder)
+    assert response.name == "name_value"
+    assert response.metageneration == 1491
+
+
+def test_create_managed_folder_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_managed_folder), "__call__"
+    ) as call:
+        client.create_managed_folder()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.CreateManagedFolderRequest()
+
+
+def test_create_managed_folder_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = storage_control.CreateManagedFolderRequest(
+        parent="parent_value",
+        managed_folder_id="managed_folder_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_managed_folder), "__call__"
+    ) as call:
+        client.create_managed_folder(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.CreateManagedFolderRequest(
+            parent="parent_value",
+            managed_folder_id="managed_folder_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_managed_folder_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ManagedFolder(
+                name="name_value",
+                metageneration=1491,
+            )
+        )
+        response = await client.create_managed_folder()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.CreateManagedFolderRequest()
+
+
+@pytest.mark.asyncio
+async def test_create_managed_folder_async(
+    transport: str = "grpc_asyncio",
+    request_type=storage_control.CreateManagedFolderRequest,
+):
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+    if isinstance(request, dict):
+        request["request_id"] = "explicit value for autopopulate-able field"
+    else:
+        request.request_id = "explicit value for autopopulate-able field"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ManagedFolder(
+                name="name_value",
+                metageneration=1491,
+            )
+        )
+        response = await client.create_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = storage_control.CreateManagedFolderRequest()
+        request.request_id = "explicit value for autopopulate-able field"
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, storage_control.ManagedFolder)
+    assert response.name == "name_value"
+    assert response.metageneration == 1491
+
+
+@pytest.mark.asyncio
+async def test_create_managed_folder_async_from_dict():
+    await test_create_managed_folder_async(request_type=dict)
+
+
+def test_create_managed_folder_routing_parameters():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = storage_control.CreateManagedFolderRequest(**{"parent": "sample1"})
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_managed_folder), "__call__"
+    ) as call:
+        call.return_value = storage_control.ManagedFolder()
+        client.create_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    _, _, kw = call.mock_calls[0]
+    # This test doesn't assert anything useful.
+    assert kw["metadata"]
+
+
+def test_create_managed_folder_flattened():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ManagedFolder()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.create_managed_folder(
+            parent="parent_value",
+            managed_folder=storage_control.ManagedFolder(name="name_value"),
+            managed_folder_id="managed_folder_id_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].managed_folder
+        mock_val = storage_control.ManagedFolder(name="name_value")
+        assert arg == mock_val
+        arg = args[0].managed_folder_id
+        mock_val = "managed_folder_id_value"
+        assert arg == mock_val
+
+
+def test_create_managed_folder_flattened_error():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.create_managed_folder(
+            storage_control.CreateManagedFolderRequest(),
+            parent="parent_value",
+            managed_folder=storage_control.ManagedFolder(name="name_value"),
+            managed_folder_id="managed_folder_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_managed_folder_flattened_async():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ManagedFolder()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ManagedFolder()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.create_managed_folder(
+            parent="parent_value",
+            managed_folder=storage_control.ManagedFolder(name="name_value"),
+            managed_folder_id="managed_folder_id_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+        arg = args[0].managed_folder
+        mock_val = storage_control.ManagedFolder(name="name_value")
+        assert arg == mock_val
+        arg = args[0].managed_folder_id
+        mock_val = "managed_folder_id_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_create_managed_folder_flattened_error_async():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.create_managed_folder(
+            storage_control.CreateManagedFolderRequest(),
+            parent="parent_value",
+            managed_folder=storage_control.ManagedFolder(name="name_value"),
+            managed_folder_id="managed_folder_id_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        storage_control.DeleteManagedFolderRequest,
+        dict,
+    ],
+)
+def test_delete_managed_folder(request_type, transport: str = "grpc"):
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+    if isinstance(request, dict):
+        request["request_id"] = "explicit value for autopopulate-able field"
+    else:
+        request.request_id = "explicit value for autopopulate-able field"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+        response = client.delete_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = storage_control.DeleteManagedFolderRequest()
+        request.request_id = "explicit value for autopopulate-able field"
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+def test_delete_managed_folder_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_managed_folder), "__call__"
+    ) as call:
+        client.delete_managed_folder()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.DeleteManagedFolderRequest()
+
+
+def test_delete_managed_folder_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = storage_control.DeleteManagedFolderRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_managed_folder), "__call__"
+    ) as call:
+        client.delete_managed_folder(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.DeleteManagedFolderRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_managed_folder_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_managed_folder()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.DeleteManagedFolderRequest()
+
+
+@pytest.mark.asyncio
+async def test_delete_managed_folder_async(
+    transport: str = "grpc_asyncio",
+    request_type=storage_control.DeleteManagedFolderRequest,
+):
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+    if isinstance(request, dict):
+        request["request_id"] = "explicit value for autopopulate-able field"
+    else:
+        request.request_id = "explicit value for autopopulate-able field"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = storage_control.DeleteManagedFolderRequest()
+        request.request_id = "explicit value for autopopulate-able field"
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+@pytest.mark.asyncio
+async def test_delete_managed_folder_async_from_dict():
+    await test_delete_managed_folder_async(request_type=dict)
+
+
+def test_delete_managed_folder_routing_parameters():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = storage_control.DeleteManagedFolderRequest(
+        **{"name": "projects/sample1/buckets/sample2/sample3"}
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_managed_folder), "__call__"
+    ) as call:
+        call.return_value = None
+        client.delete_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    _, _, kw = call.mock_calls[0]
+    # This test doesn't assert anything useful.
+    assert kw["metadata"]
+
+
+def test_delete_managed_folder_flattened():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.delete_managed_folder(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+def test_delete_managed_folder_flattened_error():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.delete_managed_folder(
+            storage_control.DeleteManagedFolderRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_managed_folder_flattened_async():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.delete_managed_folder(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_delete_managed_folder_flattened_error_async():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.delete_managed_folder(
+            storage_control.DeleteManagedFolderRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        storage_control.GetManagedFolderRequest,
+        dict,
+    ],
+)
+def test_get_managed_folder(request_type, transport: str = "grpc"):
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+    if isinstance(request, dict):
+        request["request_id"] = "explicit value for autopopulate-able field"
+    else:
+        request.request_id = "explicit value for autopopulate-able field"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ManagedFolder(
+            name="name_value",
+            metageneration=1491,
+        )
+        response = client.get_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = storage_control.GetManagedFolderRequest()
+        request.request_id = "explicit value for autopopulate-able field"
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, storage_control.ManagedFolder)
+    assert response.name == "name_value"
+    assert response.metageneration == 1491
+
+
+def test_get_managed_folder_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_managed_folder), "__call__"
+    ) as call:
+        client.get_managed_folder()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.GetManagedFolderRequest()
+
+
+def test_get_managed_folder_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = storage_control.GetManagedFolderRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_managed_folder), "__call__"
+    ) as call:
+        client.get_managed_folder(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.GetManagedFolderRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_managed_folder_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ManagedFolder(
+                name="name_value",
+                metageneration=1491,
+            )
+        )
+        response = await client.get_managed_folder()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.GetManagedFolderRequest()
+
+
+@pytest.mark.asyncio
+async def test_get_managed_folder_async(
+    transport: str = "grpc_asyncio",
+    request_type=storage_control.GetManagedFolderRequest,
+):
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+    if isinstance(request, dict):
+        request["request_id"] = "explicit value for autopopulate-able field"
+    else:
+        request.request_id = "explicit value for autopopulate-able field"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ManagedFolder(
+                name="name_value",
+                metageneration=1491,
+            )
+        )
+        response = await client.get_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = storage_control.GetManagedFolderRequest()
+        request.request_id = "explicit value for autopopulate-able field"
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, storage_control.ManagedFolder)
+    assert response.name == "name_value"
+    assert response.metageneration == 1491
+
+
+@pytest.mark.asyncio
+async def test_get_managed_folder_async_from_dict():
+    await test_get_managed_folder_async(request_type=dict)
+
+
+def test_get_managed_folder_routing_parameters():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = storage_control.GetManagedFolderRequest(
+        **{"name": "projects/sample1/buckets/sample2/sample3"}
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_managed_folder), "__call__"
+    ) as call:
+        call.return_value = storage_control.ManagedFolder()
+        client.get_managed_folder(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    _, _, kw = call.mock_calls[0]
+    # This test doesn't assert anything useful.
+    assert kw["metadata"]
+
+
+def test_get_managed_folder_flattened():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ManagedFolder()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.get_managed_folder(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+def test_get_managed_folder_flattened_error():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.get_managed_folder(
+            storage_control.GetManagedFolderRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_managed_folder_flattened_async():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_managed_folder), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ManagedFolder()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ManagedFolder()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.get_managed_folder(
+            name="name_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].name
+        mock_val = "name_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_get_managed_folder_flattened_error_async():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.get_managed_folder(
+            storage_control.GetManagedFolderRequest(),
+            name="name_value",
+        )
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        storage_control.ListManagedFoldersRequest,
+        dict,
+    ],
+)
+def test_list_managed_folders(request_type, transport: str = "grpc"):
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+    if isinstance(request, dict):
+        request["request_id"] = "explicit value for autopopulate-able field"
+    else:
+        request.request_id = "explicit value for autopopulate-able field"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ListManagedFoldersResponse(
+            next_page_token="next_page_token_value",
+        )
+        response = client.list_managed_folders(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        request = storage_control.ListManagedFoldersRequest()
+        request.request_id = "explicit value for autopopulate-able field"
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListManagedFoldersPager)
+    assert response.next_page_token == "next_page_token_value"
+
+
+def test_list_managed_folders_empty_call():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        client.list_managed_folders()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.ListManagedFoldersRequest()
+
+
+def test_list_managed_folders_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = storage_control.ListManagedFoldersRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        prefix="prefix_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        client.list_managed_folders(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.ListManagedFoldersRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            prefix="prefix_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_managed_folders_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ListManagedFoldersResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_managed_folders()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        # Ensure that the uuid4 field is set according to AIP 4235
+        assert re.match(
+            r"[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}",
+            args[0].request_id,
+        )
+        # clear UUID field so that the check below succeeds
+        args[0].request_id = None
+        assert args[0] == storage_control.ListManagedFoldersRequest()
+
+
+@pytest.mark.asyncio
+async def test_list_managed_folders_async(
+    transport: str = "grpc_asyncio",
+    request_type=storage_control.ListManagedFoldersRequest,
+):
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = request_type()
+    if isinstance(request, dict):
+        request["request_id"] = "explicit value for autopopulate-able field"
+    else:
+        request.request_id = "explicit value for autopopulate-able field"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ListManagedFoldersResponse(
+                next_page_token="next_page_token_value",
+            )
+        )
+        response = await client.list_managed_folders(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        request = storage_control.ListManagedFoldersRequest()
+        request.request_id = "explicit value for autopopulate-able field"
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, pagers.ListManagedFoldersAsyncPager)
+    assert response.next_page_token == "next_page_token_value"
+
+
+@pytest.mark.asyncio
+async def test_list_managed_folders_async_from_dict():
+    await test_list_managed_folders_async(request_type=dict)
+
+
+def test_list_managed_folders_routing_parameters():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = storage_control.ListManagedFoldersRequest(**{"parent": "sample1"})
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        call.return_value = storage_control.ListManagedFoldersResponse()
+        client.list_managed_folders(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    _, _, kw = call.mock_calls[0]
+    # This test doesn't assert anything useful.
+    assert kw["metadata"]
+
+
+def test_list_managed_folders_flattened():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ListManagedFoldersResponse()
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        client.list_managed_folders(
+            parent="parent_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+
+
+def test_list_managed_folders_flattened_error():
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        client.list_managed_folders(
+            storage_control.ListManagedFoldersRequest(),
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_managed_folders_flattened_async():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = storage_control.ListManagedFoldersResponse()
+
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            storage_control.ListManagedFoldersResponse()
+        )
+        # Call the method with a truthy value for each flattened field,
+        # using the keyword arguments to the method.
+        response = await client.list_managed_folders(
+            parent="parent_value",
+        )
+
+        # Establish that the underlying call was made with the expected
+        # request object values.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        arg = args[0].parent
+        mock_val = "parent_value"
+        assert arg == mock_val
+
+
+@pytest.mark.asyncio
+async def test_list_managed_folders_flattened_error_async():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Attempting to call a method with both a request object and flattened
+    # fields is an error.
+    with pytest.raises(ValueError):
+        await client.list_managed_folders(
+            storage_control.ListManagedFoldersRequest(),
+            parent="parent_value",
+        )
+
+
+def test_list_managed_folders_pager(transport_name: str = "grpc"):
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport_name,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                ],
+                next_page_token="abc",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[],
+                next_page_token="def",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                ],
+                next_page_token="ghi",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                ],
+            ),
+            RuntimeError,
+        )
+
+        metadata = ()
+        pager = client.list_managed_folders(request={})
+
+        assert pager._metadata == metadata
+
+        results = list(pager)
+        assert len(results) == 6
+        assert all(isinstance(i, storage_control.ManagedFolder) for i in results)
+
+
+def test_list_managed_folders_pages(transport_name: str = "grpc"):
+    client = StorageControlClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport_name,
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders), "__call__"
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                ],
+                next_page_token="abc",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[],
+                next_page_token="def",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                ],
+                next_page_token="ghi",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                ],
+            ),
+            RuntimeError,
+        )
+        pages = list(client.list_managed_folders(request={}).pages)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
+@pytest.mark.asyncio
+async def test_list_managed_folders_async_pager():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders),
+        "__call__",
+        new_callable=mock.AsyncMock,
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                ],
+                next_page_token="abc",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[],
+                next_page_token="def",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                ],
+                next_page_token="ghi",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                ],
+            ),
+            RuntimeError,
+        )
+        async_pager = await client.list_managed_folders(
+            request={},
+        )
+        assert async_pager.next_page_token == "abc"
+        responses = []
+        async for response in async_pager:  # pragma: no branch
+            responses.append(response)
+
+        assert len(responses) == 6
+        assert all(isinstance(i, storage_control.ManagedFolder) for i in responses)
+
+
+@pytest.mark.asyncio
+async def test_list_managed_folders_async_pages():
+    client = StorageControlAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_managed_folders),
+        "__call__",
+        new_callable=mock.AsyncMock,
+    ) as call:
+        # Set the response to a series of pages.
+        call.side_effect = (
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                ],
+                next_page_token="abc",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[],
+                next_page_token="def",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                ],
+                next_page_token="ghi",
+            ),
+            storage_control.ListManagedFoldersResponse(
+                managed_folders=[
+                    storage_control.ManagedFolder(),
+                    storage_control.ManagedFolder(),
+                ],
+            ),
+            RuntimeError,
+        )
+        pages = []
+        # Workaround issue in python 3.9 related to code coverage by adding `# pragma: no branch`
+        # See https://github.com/googleapis/gapic-generator-python/pull/1174#issuecomment-1025132372
+        async for page_ in (  # pragma: no branch
+            await client.list_managed_folders(request={})
+        ).pages:
+            pages.append(page_)
+        for page_, token in zip(pages, ["abc", "def", "ghi", ""]):
+            assert page_.raw_page.next_page_token == token
+
+
 def test_credentials_transport_error():
     # It is an error to provide credentials and a transport instance.
     transport = transports.StorageControlGrpcTransport(
         credentials=ga_credentials.AnonymousCredentials(),
     )
     with pytest.raises(ValueError):
         client = StorageControlClient(
@@ -3131,14 +4524,18 @@
     methods = (
         "create_folder",
         "delete_folder",
         "get_folder",
         "list_folders",
         "rename_folder",
         "get_storage_layout",
+        "create_managed_folder",
+        "delete_managed_folder",
+        "get_managed_folder",
+        "list_managed_folders",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -3565,132 +4962,160 @@
     path = StorageControlClient.folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = StorageControlClient.parse_folder_path(path)
     assert expected == actual
 
 
-def test_storage_layout_path():
+def test_managed_folder_path():
     project = "cuttlefish"
     bucket = "mussel"
+    managedFolder = "winkle"
+    expected = (
+        "projects/{project}/buckets/{bucket}/managedFolders/{managedFolder}".format(
+            project=project,
+            bucket=bucket,
+            managedFolder=managedFolder,
+        )
+    )
+    actual = StorageControlClient.managed_folder_path(project, bucket, managedFolder)
+    assert expected == actual
+
+
+def test_parse_managed_folder_path():
+    expected = {
+        "project": "nautilus",
+        "bucket": "scallop",
+        "managedFolder": "abalone",
+    }
+    path = StorageControlClient.managed_folder_path(**expected)
+
+    # Check that the path construction is reversible.
+    actual = StorageControlClient.parse_managed_folder_path(path)
+    assert expected == actual
+
+
+def test_storage_layout_path():
+    project = "squid"
+    bucket = "clam"
     expected = "projects/{project}/buckets/{bucket}/storageLayout".format(
         project=project,
         bucket=bucket,
     )
     actual = StorageControlClient.storage_layout_path(project, bucket)
     assert expected == actual
 
 
 def test_parse_storage_layout_path():
     expected = {
-        "project": "winkle",
-        "bucket": "nautilus",
+        "project": "whelk",
+        "bucket": "octopus",
     }
     path = StorageControlClient.storage_layout_path(**expected)
 
     # Check that the path construction is reversible.
     actual = StorageControlClient.parse_storage_layout_path(path)
     assert expected == actual
 
 
 def test_common_billing_account_path():
-    billing_account = "scallop"
+    billing_account = "oyster"
     expected = "billingAccounts/{billing_account}".format(
         billing_account=billing_account,
     )
     actual = StorageControlClient.common_billing_account_path(billing_account)
     assert expected == actual
 
 
 def test_parse_common_billing_account_path():
     expected = {
-        "billing_account": "abalone",
+        "billing_account": "nudibranch",
     }
     path = StorageControlClient.common_billing_account_path(**expected)
 
     # Check that the path construction is reversible.
     actual = StorageControlClient.parse_common_billing_account_path(path)
     assert expected == actual
 
 
 def test_common_folder_path():
-    folder = "squid"
+    folder = "cuttlefish"
     expected = "folders/{folder}".format(
         folder=folder,
     )
     actual = StorageControlClient.common_folder_path(folder)
     assert expected == actual
 
 
 def test_parse_common_folder_path():
     expected = {
-        "folder": "clam",
+        "folder": "mussel",
     }
     path = StorageControlClient.common_folder_path(**expected)
 
     # Check that the path construction is reversible.
     actual = StorageControlClient.parse_common_folder_path(path)
     assert expected == actual
 
 
 def test_common_organization_path():
-    organization = "whelk"
+    organization = "winkle"
     expected = "organizations/{organization}".format(
         organization=organization,
     )
     actual = StorageControlClient.common_organization_path(organization)
     assert expected == actual
 
 
 def test_parse_common_organization_path():
     expected = {
-        "organization": "octopus",
+        "organization": "nautilus",
     }
     path = StorageControlClient.common_organization_path(**expected)
 
     # Check that the path construction is reversible.
     actual = StorageControlClient.parse_common_organization_path(path)
     assert expected == actual
 
 
 def test_common_project_path():
-    project = "oyster"
+    project = "scallop"
     expected = "projects/{project}".format(
         project=project,
     )
     actual = StorageControlClient.common_project_path(project)
     assert expected == actual
 
 
 def test_parse_common_project_path():
     expected = {
-        "project": "nudibranch",
+        "project": "abalone",
     }
     path = StorageControlClient.common_project_path(**expected)
 
     # Check that the path construction is reversible.
     actual = StorageControlClient.parse_common_project_path(path)
     assert expected == actual
 
 
 def test_common_location_path():
-    project = "cuttlefish"
-    location = "mussel"
+    project = "squid"
+    location = "clam"
     expected = "projects/{project}/locations/{location}".format(
         project=project,
         location=location,
     )
     actual = StorageControlClient.common_location_path(project, location)
     assert expected == actual
 
 
 def test_parse_common_location_path():
     expected = {
-        "project": "winkle",
-        "location": "nautilus",
+        "project": "whelk",
+        "location": "octopus",
     }
     path = StorageControlClient.common_location_path(**expected)
 
     # Check that the path construction is reversible.
     actual = StorageControlClient.parse_common_location_path(path)
     assert expected == actual
```

