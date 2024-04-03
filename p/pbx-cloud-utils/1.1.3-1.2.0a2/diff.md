# Comparing `tmp/pbx_cloud_utils-1.1.3-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.2.0a2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5628 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-04 10:39 cloud_utils/__init__.py
--rw-r--r--  2.0 unx     3940 b- defN 23-Nov-30 12:01 cloud_utils/aio_storage.py
--rw-r--r--  2.0 unx      284 b- defN 23-Nov-30 12:01 cloud_utils/exceptions.py
--rw-r--r--  2.0 unx     8368 b- defN 23-Nov-30 15:33 cloud_utils/storage.py
--rw-r--r--  2.0 unx       84 b- defN 23-Nov-30 12:01 cloud_utils/types.py
--rw-r--r--  2.0 unx      346 b- defN 23-Nov-30 12:01 cloud_utils/utils.py
--rw-r--r--  2.0 unx      286 b- defN 23-Dec-04 10:39 pbx_cloud_utils-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Dec-04 10:39 pbx_cloud_utils-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Dec-04 10:39 pbx_cloud_utils-1.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      800 b- defN 23-Dec-04 10:39 pbx_cloud_utils-1.1.3.dist-info/RECORD
-10 files, 14212 bytes uncompressed, 4254 bytes compressed:  70.1%
+Zip file size: 7017 bytes, number of entries: 10
+-rw-r--r--  2.0 unx        0 b- defN 23-May-10 08:55 cloud_utils/__init__.py
+-rw-r--r--  2.0 unx    11325 b- defN 24-Apr-03 07:39 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx      284 b- defN 23-May-10 08:55 cloud_utils/exceptions.py
+-rw-r--r--  2.0 unx     9825 b- defN 24-Apr-02 13:37 cloud_utils/storage.py
+-rw-r--r--  2.0 unx     1261 b- defN 24-Apr-02 13:41 cloud_utils/types.py
+-rw-r--r--  2.0 unx      346 b- defN 23-May-10 08:55 cloud_utils/utils.py
+-rw-r--r--  2.0 unx      324 b- defN 24-Apr-03 08:49 pbx_cloud_utils-1.2.0a2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 08:49 pbx_cloud_utils-1.2.0a2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-03 08:49 pbx_cloud_utils-1.2.0a2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      811 b- defN 24-Apr-03 08:49 pbx_cloud_utils-1.2.0a2.dist-info/RECORD
+10 files, 24280 bytes uncompressed, 5627 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.1.3.dist-info/METADATA
+Filename: pbx_cloud_utils-1.2.0a2.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.1.3.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.2.0a2.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.1.3.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.2.0a2.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.1.3.dist-info/RECORD
+Filename: pbx_cloud_utils-1.2.0a2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/aio_storage.py

```diff
@@ -1,45 +1,93 @@
 import datetime
 import os
 from abc import ABC, abstractmethod
+from io import BytesIO
 from typing import Any, Tuple
 
 from aiobotocore import config as s3_config
 from azure.storage.blob import BlobSasPermissions, generate_blob_sas
 from azure.storage.blob.aio import BlobClient, ContainerClient
+from google.cloud import storage as gcs_storage
 
-from cloud_utils.types import S3AddressingStyles
+from cloud_utils.types import (
+    PbxACL,
+    PbxStorageClass,
+    S3AddressingStyles,
+    azure_acl_map,
+    azure_storage_class_map,
+    gcs_acl_map,
+    gcs_storage_class_map,
+    s3_acl_map,
+    s3_storage_class_map,
+)
 from cloud_utils.utils import get_account_key
 
 try:
     import aiobotocore  # type: ignore
 
     HAS_AIOBOTOCORE = True
 except ImportError:  # pragma: no cover
     HAS_AIOBOTOCORE = False
 
 
 class AsyncStorage(ABC):
+    provider_storage_class_map: dict[str, str]
+    provider_acl_map: dict[str, str]
+
     def __init__(self, bucket_name: str, region_name: str, **kwargs: Any):
         self.region_name: str = region_name
         self.bucket_name: str = bucket_name
         self.extra_kwargs: Any = kwargs
 
     @abstractmethod
-    async def delete_object(self, key: str):
+    async def delete_object(self, key: str) -> None:
         pass  # pragma: no cover
 
     @abstractmethod
     async def generate_presigned_url(
         self, key: str, size: str, content_md5: str, **kwargs: Any
     ) -> Tuple[str, dict]:
         pass  # pragma: no cover
 
+    @abstractmethod
+    async def change_storage_class(
+        self,
+        key: str,
+        target_storage_class: PbxStorageClass,
+        acl: PbxACL = PbxACL.PUBLIC_READ,
+    ) -> None:
+        pass  # pragma: no cover
+
+    @abstractmethod
+    async def copy(
+        self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
+    ) -> None:
+        pass
+
+    @abstractmethod
+    async def download(self, key: str) -> BytesIO:
+        pass
+
+    @abstractmethod
+    async def upload(
+        self,
+        key: str,
+        content: BytesIO,
+        mimetype: str,
+        acl: PbxACL = PbxACL.PUBLIC_READ,
+        target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
+    ):
+        pass
+
 
 class AsyncAmazonS3Storage(AsyncStorage):
+    provider_storage_class_map: dict[str, str] = s3_storage_class_map
+    provider_acl_map: dict[str, str] = s3_acl_map
+
     def __new__(cls, *args, **kwargs):
         if not HAS_AIOBOTOCORE:  # pragma: no cover
             raise ImportError("Required aiobotocore, please install aiobotocore>=1.4.0.")
         return super().__new__(cls)
 
     async def delete_object(self, key: str):
         session = aiobotocore.session.get_session()
@@ -71,16 +119,76 @@
                     "ContentLength": size,
                     "ContentMD5": content_md5,
                 },
             )
 
             return url, headers
 
+    async def change_storage_class(
+        self,
+        key: str,
+        target_storage_class: PbxStorageClass,
+        acl: PbxACL = PbxACL.PUBLIC_READ,
+    ):
+        session = aiobotocore.session.get_session()
+        async with session.create_client("s3", self.region_name) as client:
+            client.copy_object(
+                ACL=self.provider_acl_map[acl.name],
+                Bucket=self.bucket_name,
+                Key=key,
+                CopySource={"Bucket": self.bucket_name, "Key": key},
+                StorageClass=self.provider_storage_class_map[target_storage_class.name],
+                MetadataDirective="COPY",
+            )
+
+    async def copy(
+        self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
+    ) -> None:
+        session = aiobotocore.session.get_session()
+        async with session.create_client("s3", self.region_name) as client:
+            client.copy_object(
+                ACL=self.provider_acl_map[acl.name],
+                Bucket=self.bucket_name,
+                Key=target_key,
+                CopySource={"Bucket": self.bucket_name, "Key": key},
+                MetadataDirective="COPY",
+            )
+
+    async def download(self, key: str) -> BytesIO:
+        session = aiobotocore.session.get_session()
+        async with session.create_client("s3", self.region_name) as client:
+            obj = await client.get_object(Bucket=self.bucket_name, Key=key)
+            async with obj["Body"] as body_stream:
+                data = await body_stream.read()
+            return BytesIO(data)
+
+    async def upload(
+        self,
+        key: str,
+        content: BytesIO,
+        mimetype: str,
+        acl: PbxACL = PbxACL.PUBLIC_READ,
+        target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
+    ):
+        session = aiobotocore.session.get_session()
+        async with session.create_client("s3", self.region_name) as client:
+            return await client.put_object(
+                ACL=self.provider_acl_map[acl.name],
+                Body=content.getvalue(),
+                Bucket=self.bucket_name,
+                Key=key,
+                StorageClass=self.provider_storage_class_map[target_storage_class.name],
+                ContentType=mimetype,
+            )
+
 
 class AsyncAzureBlobStorage(AsyncStorage):
+    provider_storage_class_map: dict[str, str] = azure_storage_class_map
+    provider_acl_map: dict[str, str] = azure_acl_map
+
     def __init__(self, container_name: str, **kwargs: Any) -> None:
         connection_string = kwargs.get(
             "conn_str",
             os.environ.get("AZURE_STORAGE_CONNECTION_STRING"),
         )
         self.account_key: str = get_account_key(connection_string)
         self.container_name: str = container_name
@@ -106,7 +214,114 @@
             permission=BlobSasPermissions(create=True, write=True),
             expiry=datetime.datetime.now() + datetime.timedelta(hours=kwargs.get("expiry", 1)),
         )
         container_blob_url = self.client.get_blob_client(key).url
         blob_client = BlobClient.from_blob_url(container_blob_url, credential=sas_token)
 
         return blob_client.url, headers
+
+    async def change_storage_class(
+        self, key: str, target_storage_class: PbxStorageClass, acl: PbxACL = PbxACL.PUBLIC_READ
+    ) -> None:
+        raise NotImplementedError()
+
+    async def copy(
+        self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
+    ) -> None:
+        raise NotImplementedError()
+
+    async def download(self, key: str) -> BytesIO:
+        raise NotImplementedError()
+
+    async def upload(
+        self,
+        key: str,
+        content: BytesIO,
+        mimetype: str,
+        acl: PbxACL = PbxACL.PUBLIC_READ,
+        target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
+    ):
+        raise NotImplementedError()
+
+
+class AsyncGoogleCloudStorage(AsyncStorage):
+    provider_storage_class_map: dict[str, str] = gcs_storage_class_map
+    provider_acl_map: dict[str, str] = gcs_acl_map
+    bucket_client: gcs_storage.Bucket
+    endpoint_url: str
+
+    def __init__(self, gcs_project_id: str, endpoint_url: str, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        gcs_storage_client_kwargs = {
+            key.removeprefix("gcs_"): value
+            for key, value in kwargs.items()
+            if key.startswith("gcs_")
+        }
+        client = gcs_storage.Client(project=gcs_project_id, **gcs_storage_client_kwargs)
+        bucket = client.bucket(self.bucket_name)
+        self.bucket_client = bucket
+        self.endpoint_url = endpoint_url
+
+    async def delete_object(self, key: str) -> None:
+        raise NotImplementedError()
+
+    async def generate_presigned_url(
+        self, key: str, size: str, content_md5: str, **kwargs: Any
+    ) -> Tuple[str, dict]:
+        raise NotImplementedError()
+
+    async def change_storage_class(
+        self,
+        key: str,
+        target_storage_class: PbxStorageClass,
+        acl: PbxACL = PbxACL.PUBLIC_READ,
+    ):
+        # TODO use async API
+        self.bucket_client.blob(key).update_storage_class(
+            self.provider_storage_class_map[target_storage_class.name]
+        )
+
+    async def copy(
+        self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
+    ) -> None:
+        session = aiobotocore.session.get_session()
+        async with session.create_client(
+            "s3", self.region_name, endpoint_url=self.endpoint_url
+        ) as client:
+            client.copy_object(
+                ACL=self.provider_acl_map[acl.name],
+                Bucket=self.bucket_name,
+                Key=target_key,
+                CopySource={"Bucket": self.bucket_name, "Key": key},
+                MetadataDirective="COPY",
+            )
+
+    async def download(self, key: str) -> BytesIO:
+        session = aiobotocore.session.get_session()
+        async with session.create_client(
+            "s3", self.region_name, endpoint_url=self.endpoint_url
+        ) as client:
+            obj = await client.get_object(Bucket=self.bucket_name, Key=key)
+            async with obj["Body"] as body_stream:
+                data = await body_stream.read()
+            return BytesIO(data)
+
+    async def upload(
+        self,
+        key: str,
+        content: BytesIO,
+        mimetype: str,
+        acl: PbxACL = PbxACL.PUBLIC_READ,
+        target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
+    ):
+        session = aiobotocore.session.get_session()
+        async with session.create_client(
+            "s3", self.region_name, endpoint_url=self.endpoint_url
+        ) as client:
+            return await client.put_object(
+                ACL=self.provider_acl_map[acl.name],
+                Body=content.getvalue(),
+                Bucket=self.bucket_name,
+                Key=key,
+                StorageClass=self.provider_storage_class_map[target_storage_class.name],
+                ContentType=mimetype,
+            )
```

## cloud_utils/storage.py

```diff
@@ -1,30 +1,29 @@
 from __future__ import annotations
 
 import os
 from abc import ABC, abstractmethod
-from enum import IntEnum
 from typing import IO, Any, Callable, Iterable
 
 import boto3
 from azure.core.exceptions import AzureError
 from azure.storage.blob import BlobClient, ContainerClient, ContentSettings
 from botocore.exceptions import BotoCoreError, ClientError
+from google.cloud import storage as gcs_storage
 
 from cloud_utils import exceptions
+from cloud_utils.types import (
+    azure_storage_class_map,
+    gcs_storage_class_map,
+    s3_storage_class_map,
+)
 
 BotoError = (BotoCoreError, ClientError)
 
 
-class PbxStorageClass(IntEnum):
-    STANDARD = 0
-    INFREQUENT_ACCESS = 1
-    ARCHIVE = 2
-
-
 class StorageObject(ABC):
     provider_storage_class_map: dict[str, str]
     pbx_storage_class_map: dict[str, str]
 
     def __new__(cls, *args):
         new = super().__new__(cls)
         new.pbx_storage_class_map = {v: k for k, v in cls.provider_storage_class_map.items()}
@@ -81,19 +80,15 @@
     @property
     @abstractmethod
     def _provider_storage_class(self) -> str:
         pass
 
 
 class AmazonS3Object(StorageObject):
-    provider_storage_class_map: dict[str, str] = {
-        PbxStorageClass.STANDARD.name: "STANDARD",
-        PbxStorageClass.INFREQUENT_ACCESS.name: "ONEZONE_IA",
-        PbxStorageClass.ARCHIVE.name: "GLACIER",
-    }
+    provider_storage_class_map: dict[str, str] = s3_storage_class_map
 
     @property
     def path(self):
         return self.client.key
 
     @property
     def bucket_name(self) -> str:
@@ -151,19 +146,15 @@
 
     @property
     def _provider_storage_class(self) -> str:
         return self.client.storage_class or "STANDARD"
 
 
 class AzureBlobObject(StorageObject):
-    provider_storage_class_map: dict[str, str] = {
-        PbxStorageClass.STANDARD.name: "Hot",
-        PbxStorageClass.INFREQUENT_ACCESS.name: "Cool",
-        PbxStorageClass.ARCHIVE.name: "Archive",
-    }
+    provider_storage_class_map: dict[str, str] = azure_storage_class_map
 
     @property
     def path(self):
         return self.client.blob_name
 
     @property
     def bucket_name(self) -> str:
@@ -208,14 +199,33 @@
         self.client.set_standard_blob_tier(self.provider_storage_class_map[storage_class])
 
     @property
     def _provider_storage_class(self) -> str:
         return self.client.get_blob_properties()["blob_tier"]
 
 
+class HybridGoogleCloudStorageObject(AmazonS3Object):
+    provider_storage_class_map: dict[str, str] = gcs_storage_class_map
+
+    def __init__(self, client, gcs_client: gcs_storage.Bucket) -> None:
+        super().__init__(client)
+        self.gcs_client = gcs_client
+
+    def set_storage_class(self, storage_class: str) -> None:
+        destination_storage_class = self.provider_storage_class_map[storage_class]
+
+        blob = self.gcs_client.blob(self.path)
+        blob.update_storage_class(destination_storage_class)
+
+    @property
+    def _provider_storage_class(self) -> str:
+        blob = self.gcs_client.get_blob(self.path)
+        return blob.storage_class
+
+
 class Storage(ABC):
     object_class: type[StorageObject]
 
     def get_object(self, path: str) -> StorageObject:
         object_client = self.object_client_class(path)
         return self.object_class(object_client)
 
@@ -286,7 +296,31 @@
     def object_client_class(
         self,
     ) -> Callable[..., BlobClient]:
         return self.client.get_blob_client
 
     def find_object_names(self, prefix: str) -> Iterable[str]:
         return (item.name for item in self.client.list_blobs(name_starts_with=prefix))
+
+
+class HybridGoogleCloudStorage(AmazonS3Storage):
+    object_class = HybridGoogleCloudStorageObject
+
+    def __init__(
+        self, bucket_name: str, region_name: str, gcs_project: str = "", **kwargs: Any
+    ) -> None:
+        super().__init__(bucket_name, region_name, **kwargs)
+        self.gcs_project = gcs_project or os.environ.get("GCS_PROJECT_ID")
+        gcs_storage_client_kwargs = {
+            key.removeprefix("gcs_"): value
+            for key, value in kwargs.items()
+            if key.startswith("gcs_")
+        }
+        self.gcs_client = self.get_gcs_bucket_client(**gcs_storage_client_kwargs)
+
+    def get_gcs_bucket_client(self, **kwargs: Any) -> gcs_storage.Bucket:
+        gcs_storage_client = gcs_storage.Client(project=self.gcs_project, **kwargs)
+        return gcs_storage_client.bucket(self.bucket_name)
+
+    def get_object(self, path: str) -> HybridGoogleCloudStorageObject:
+        object_client = self.object_client_class(path)
+        return self.object_class(object_client, self.gcs_client)
```

## cloud_utils/types.py

```diff
@@ -1,3 +1,50 @@
+from enum import IntEnum
 from typing import Literal
 
 S3AddressingStyles = Literal["path", "virtual", "auto"]
+
+
+class PbxStorageClass(IntEnum):
+    STANDARD = 0
+    INFREQUENT_ACCESS = 1
+    ARCHIVE = 2
+
+
+s3_storage_class_map: dict[str, str] = {
+    PbxStorageClass.STANDARD.name: "STANDARD",
+    PbxStorageClass.INFREQUENT_ACCESS.name: "ONEZONE_IA",
+    PbxStorageClass.ARCHIVE.name: "GLACIER",
+}
+
+azure_storage_class_map: dict[str, str] = {
+    PbxStorageClass.STANDARD.name: "Hot",
+    PbxStorageClass.INFREQUENT_ACCESS.name: "Cool",
+    PbxStorageClass.ARCHIVE.name: "Archive",
+}
+
+gcs_storage_class_map: dict[str, str] = {
+    PbxStorageClass.STANDARD.name: "STANDARD",
+    PbxStorageClass.INFREQUENT_ACCESS.name: "NEARLINE",
+    PbxStorageClass.ARCHIVE.name: "ARCHIVE",
+}
+
+
+class PbxACL(IntEnum):
+    PUBLIC_READ = 0
+    AUTHENTICATED_READ = 1
+
+
+s3_acl_map: dict[str, str] = {
+    PbxACL.PUBLIC_READ.name: "public-read",
+    PbxACL.AUTHENTICATED_READ.name: "authenticated-read",
+}
+
+azure_acl_map: dict[str, str] = {
+    PbxACL.PUBLIC_READ.name: "public-read",
+    PbxACL.AUTHENTICATED_READ.name: "authenticated-read",
+}
+
+gcs_acl_map: dict[str, str] = {
+    PbxACL.PUBLIC_READ.name: "public-read",
+    PbxACL.AUTHENTICATED_READ.name: "authenticated-read",
+}
```

