# Comparing `tmp/pbx_cloud_utils-1.2.0a2-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.2.0a3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7017 bytes, number of entries: 10
+Zip file size: 7065 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-May-10 08:55 cloud_utils/__init__.py
--rw-r--r--  2.0 unx    11325 b- defN 24-Apr-03 07:39 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx    11695 b- defN 24-Apr-03 12:59 cloud_utils/aio_storage.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-10 08:55 cloud_utils/exceptions.py
 -rw-r--r--  2.0 unx     9825 b- defN 24-Apr-02 13:37 cloud_utils/storage.py
 -rw-r--r--  2.0 unx     1261 b- defN 24-Apr-02 13:41 cloud_utils/types.py
 -rw-r--r--  2.0 unx      346 b- defN 23-May-10 08:55 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-03 08:49 pbx_cloud_utils-1.2.0a2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 08:49 pbx_cloud_utils-1.2.0a2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-03 08:49 pbx_cloud_utils-1.2.0a2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      811 b- defN 24-Apr-03 08:49 pbx_cloud_utils-1.2.0a2.dist-info/RECORD
-10 files, 24280 bytes uncompressed, 5627 bytes compressed:  76.8%
+-rw-r--r--  2.0 unx      324 b- defN 24-Apr-03 13:04 pbx_cloud_utils-1.2.0a3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 13:04 pbx_cloud_utils-1.2.0a3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-03 13:04 pbx_cloud_utils-1.2.0a3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      811 b- defN 24-Apr-03 13:04 pbx_cloud_utils-1.2.0a3.dist-info/RECORD
+10 files, 24650 bytes uncompressed, 5675 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a2.dist-info/METADATA
+Filename: pbx_cloud_utils-1.2.0a3.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a2.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.2.0a3.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a2.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.2.0a3.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a2.dist-info/RECORD
+Filename: pbx_cloud_utils-1.2.0a3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/aio_storage.py

```diff
@@ -61,15 +61,15 @@
     @abstractmethod
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
         pass
 
     @abstractmethod
-    async def download(self, key: str) -> BytesIO:
+    async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
         pass
 
     @abstractmethod
     async def upload(
         self,
         key: str,
         content: BytesIO,
@@ -149,21 +149,24 @@
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=target_key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 MetadataDirective="COPY",
             )
 
-    async def download(self, key: str) -> BytesIO:
+    async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
         session = aiobotocore.session.get_session()
         async with session.create_client("s3", self.region_name) as client:
             obj = await client.get_object(Bucket=self.bucket_name, Key=key)
             async with obj["Body"] as body_stream:
                 data = await body_stream.read()
-            return BytesIO(data)
+            return BytesIO(data), {
+                "mimetype": obj.get("ContentType"),
+                "storage_class": obj.get("StorageClass", "STANDARD"),
+            }
 
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
@@ -225,15 +228,15 @@
         raise NotImplementedError()
 
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
         raise NotImplementedError()
 
-    async def download(self, key: str) -> BytesIO:
+    async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
         raise NotImplementedError()
 
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
@@ -291,23 +294,26 @@
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=target_key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
                 MetadataDirective="COPY",
             )
 
-    async def download(self, key: str) -> BytesIO:
+    async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
         session = aiobotocore.session.get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
             obj = await client.get_object(Bucket=self.bucket_name, Key=key)
             async with obj["Body"] as body_stream:
                 data = await body_stream.read()
-            return BytesIO(data)
+            return BytesIO(data), {
+                "mimetype": obj.get("ContentType"),
+                "storage_class": obj.get("StorageClass", "STANDARD"),
+            }
 
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
```

