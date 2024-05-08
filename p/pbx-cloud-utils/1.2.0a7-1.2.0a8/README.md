# Comparing `tmp/pbx_cloud_utils-1.2.0a7-py3-none-any.whl.zip` & `tmp/pbx_cloud_utils-1.2.0a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,13 @@
-Zip file size: 7163 bytes, number of entries: 10
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-09 15:28 cloud_utils/__init__.py
--rw-r--r--  2.0 unx    12017 b- defN 24-Apr-09 15:25 cloud_utils/aio_storage.py
+Zip file size: 7562 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-22 11:19 cloud_utils/__init__.py
+-rw-r--r--  2.0 unx    12261 b- defN 24-Apr-22 11:06 cloud_utils/aio_storage.py
+-rw-r--r--  2.0 unx       57 b- defN 24-Apr-22 11:06 cloud_utils/const.py
 -rw-r--r--  2.0 unx      284 b- defN 24-Apr-02 10:50 cloud_utils/exceptions.py
--rw-r--r--  2.0 unx     9825 b- defN 24-Apr-08 11:05 cloud_utils/storage.py
--rw-r--r--  2.0 unx     1258 b- defN 24-Apr-08 11:05 cloud_utils/types.py
+-rw-r--r--  2.0 unx     9960 b- defN 24-Apr-22 11:06 cloud_utils/storage.py
+-rw-r--r--  2.0 unx     1345 b- defN 24-Apr-18 13:35 cloud_utils/types.py
 -rw-r--r--  2.0 unx      346 b- defN 24-Apr-02 10:50 cloud_utils/utils.py
--rw-r--r--  2.0 unx      324 b- defN 24-Apr-09 15:28 pbx_cloud_utils-1.2.0a7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-09 15:28 pbx_cloud_utils-1.2.0a7.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Apr-09 15:28 pbx_cloud_utils-1.2.0a7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      811 b- defN 24-Apr-09 15:28 pbx_cloud_utils-1.2.0a7.dist-info/RECORD
-10 files, 24969 bytes uncompressed, 5773 bytes compressed:  76.9%
+-rw-r--r--  2.0 unx      324 b- defN 24-Apr-22 11:19 pbx_cloud_utils-1.2.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-22 11:19 pbx_cloud_utils-1.2.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Apr-22 11:19 pbx_cloud_utils-1.2.0a8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      886 b- defN 24-Apr-22 11:19 pbx_cloud_utils-1.2.0a8.dist-info/RECORD
+11 files, 25567 bytes uncompressed, 6056 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -1,31 +1,34 @@
 Filename: cloud_utils/__init__.py
 Comment: 
 
 Filename: cloud_utils/aio_storage.py
 Comment: 
 
+Filename: cloud_utils/const.py
+Comment: 
+
 Filename: cloud_utils/exceptions.py
 Comment: 
 
 Filename: cloud_utils/storage.py
 Comment: 
 
 Filename: cloud_utils/types.py
 Comment: 
 
 Filename: cloud_utils/utils.py
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a7.dist-info/METADATA
+Filename: pbx_cloud_utils-1.2.0a8.dist-info/METADATA
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a7.dist-info/WHEEL
+Filename: pbx_cloud_utils-1.2.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a7.dist-info/top_level.txt
+Filename: pbx_cloud_utils-1.2.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: pbx_cloud_utils-1.2.0a7.dist-info/RECORD
+Filename: pbx_cloud_utils-1.2.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloud_utils/aio_storage.py

```diff
@@ -5,18 +5,20 @@
 from typing import Any, Tuple
 
 from aiobotocore import config as s3_config
 from azure.storage.blob import BlobSasPermissions, generate_blob_sas
 from azure.storage.blob.aio import BlobClient, ContainerClient
 from google.cloud import storage as gcs_storage
 
+from cloud_utils.const import GOOGLE_BUCKET_API_URL
 from cloud_utils.types import (
     PbxACL,
     PbxStorageClass,
     S3AddressingStyles,
+    UploadObjectData,
     azure_acl_map,
     azure_storage_class_map,
     gcs_acl_map,
     gcs_storage_class_map,
     s3_acl_map,
     s3_storage_class_map,
 )
@@ -37,51 +39,51 @@
     def __init__(self, bucket_name: str, region_name: str, **kwargs: Any):
         self.region_name: str = region_name
         self.bucket_name: str = bucket_name
         self.extra_kwargs: Any = kwargs
 
     @abstractmethod
     async def delete_object(self, key: str) -> None:
-        pass  # pragma: no cover
+        pass
 
     @abstractmethod
     async def generate_presigned_url(
         self, key: str, size: str, content_md5: str, **kwargs: Any
     ) -> Tuple[str, dict]:
-        pass  # pragma: no cover
+        pass
 
     @abstractmethod
     async def change_storage_class(
         self,
         key: str,
         target_storage_class: PbxStorageClass,
         acl: PbxACL = PbxACL.PUBLIC_READ,
     ) -> None:
-        pass  # pragma: no cover
+        pass
 
     @abstractmethod
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
     ) -> None:
-        pass  # pragma: no cover
+        pass
 
     @abstractmethod
     async def download(self, key: str) -> tuple[BytesIO, dict[str, str]]:
-        pass  # pragma: no cover
+        pass
 
     @abstractmethod
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
-    ):
-        pass  # pragma: no cover
+    ) -> UploadObjectData:
+        pass
 
 
 class AsyncAmazonS3Storage(AsyncStorage):
     provider_storage_class_map: dict[str, str] = s3_storage_class_map
     provider_acl_map: dict[str, str] = s3_acl_map
 
     def __new__(cls, *args, **kwargs):
@@ -124,15 +126,15 @@
             return url, headers
 
     async def change_storage_class(
         self,
         key: str,
         target_storage_class: PbxStorageClass,
         acl: PbxACL = PbxACL.PUBLIC_READ,
-    ):
+    ) -> None:
         session = aiobotocore.session.get_session()
         async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
             await client.copy_object(
                 ACL=self.provider_acl_map[acl.name],
                 Bucket=self.bucket_name,
                 Key=key,
                 CopySource={"Bucket": self.bucket_name, "Key": key},
@@ -167,25 +169,26 @@
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
-    ):
+    ) -> UploadObjectData:
         session = aiobotocore.session.get_session()
         async with session.create_client("s3", self.region_name, **self.extra_kwargs) as client:
-            return await client.put_object(
+            response = await client.put_object(
                 ACL=self.provider_acl_map[acl.name],
                 Body=content.getvalue(),
                 Bucket=self.bucket_name,
                 Key=key,
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
                 ContentType=mimetype,
             )
+            return UploadObjectData(md5sum=response["ETag"].replace('"', ""))
 
 
 class AsyncAzureBlobStorage(AsyncStorage):
     provider_storage_class_map: dict[str, str] = azure_storage_class_map
     provider_acl_map: dict[str, str] = azure_acl_map
 
     def __init__(self, container_name: str, **kwargs: Any) -> None:
@@ -238,51 +241,51 @@
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
-    ):
+    ) -> UploadObjectData:
         raise NotImplementedError()
 
 
 class HybridAsyncGoogleCloudStorage(AsyncStorage):
     provider_storage_class_map: dict[str, str] = gcs_storage_class_map
     provider_acl_map: dict[str, str] = gcs_acl_map
     bucket_client: gcs_storage.Bucket
     endpoint_url: str
 
-    def __init__(self, endpoint_url: str, gcs_project_id: str = "", *args, **kwargs):
+    def __init__(self, endpoint_url: str = "", gcs_project_id: str = "", *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.gcs_project = gcs_project_id or os.environ.get("GCS_PROJECT_ID")
         gcs_storage_client_kwargs = {
             key.removeprefix("gcs_"): value
             for key, value in kwargs.items()
             if key.startswith("gcs_")
         }
         client = gcs_storage.Client(project=self.gcs_project, **gcs_storage_client_kwargs)
         bucket = client.bucket(self.bucket_name)
         self.bucket_client = bucket
-        self.endpoint_url = endpoint_url
+        self.endpoint_url = endpoint_url or GOOGLE_BUCKET_API_URL
 
     async def delete_object(self, key: str) -> None:
         raise NotImplementedError()
 
     async def generate_presigned_url(
         self, key: str, size: str, content_md5: str, **kwargs: Any
     ) -> Tuple[str, dict]:
         raise NotImplementedError()
 
     async def change_storage_class(
         self,
         key: str,
         target_storage_class: PbxStorageClass,
         acl: PbxACL = PbxACL.PUBLIC_READ,
-    ):
+    ) -> None:
         # TODO use async API
         self.bucket_client.blob(key).update_storage_class(
             self.provider_storage_class_map[target_storage_class.name]
         )
 
     async def copy(
         self, key: str, target_key: str, acl: PbxACL = PbxACL.AUTHENTICATED_READ
@@ -316,20 +319,21 @@
     async def upload(
         self,
         key: str,
         content: BytesIO,
         mimetype: str,
         acl: PbxACL = PbxACL.PUBLIC_READ,
         target_storage_class: PbxStorageClass = PbxStorageClass.STANDARD,
-    ):
+    ) -> UploadObjectData:
         session = aiobotocore.session.get_session()
         async with session.create_client(
             "s3", self.region_name, endpoint_url=self.endpoint_url
         ) as client:
-            return await client.put_object(
+            response = await client.put_object(
                 ACL=self.provider_acl_map[acl.name],
                 Body=content.getvalue(),
                 Bucket=self.bucket_name,
                 Key=key,
                 StorageClass=self.provider_storage_class_map[target_storage_class.name],
                 ContentType=mimetype,
             )
+            return UploadObjectData(md5sum=response["ETag"].replace('"', ""))
```

## cloud_utils/storage.py

```diff
@@ -7,14 +7,15 @@
 import boto3
 from azure.core.exceptions import AzureError
 from azure.storage.blob import BlobClient, ContainerClient, ContentSettings
 from botocore.exceptions import BotoCoreError, ClientError
 from google.cloud import storage as gcs_storage
 
 from cloud_utils import exceptions
+from cloud_utils.const import GOOGLE_BUCKET_API_URL
 from cloud_utils.types import (
     azure_storage_class_map,
     gcs_storage_class_map,
     s3_storage_class_map,
 )
 
 BotoError = (BotoCoreError, ClientError)
@@ -304,14 +305,15 @@
 
 class HybridGoogleCloudStorage(AmazonS3Storage):
     object_class = HybridGoogleCloudStorageObject
 
     def __init__(
         self, bucket_name: str, region_name: str, gcs_project: str = "", **kwargs: Any
     ) -> None:
+        kwargs["endpoint_url"] = kwargs.get("endpoint_url", GOOGLE_BUCKET_API_URL)
         super().__init__(bucket_name, region_name, **kwargs)
         self.gcs_project = gcs_project or os.environ.get("GCS_PROJECT_ID")
         gcs_storage_client_kwargs = {
             key.removeprefix("gcs_"): value
             for key, value in kwargs.items()
             if key.startswith("gcs_")
         }
```

## cloud_utils/types.py

```diff
@@ -1,7 +1,8 @@
+from dataclasses import dataclass
 from enum import IntEnum
 from typing import Literal
 
 S3AddressingStyles = Literal["path", "virtual", "auto"]
 
 
 class PbxStorageClass(IntEnum):
@@ -44,7 +45,12 @@
     PbxACL.AUTHENTICATED_READ.name: "authenticated-read",
 }
 
 gcs_acl_map: dict[str, str] = {
     PbxACL.PUBLIC_READ.name: "public-read",
     PbxACL.AUTHENTICATED_READ.name: "project-private",
 }
+
+
+@dataclass
+class UploadObjectData:
+    md5sum: str
```

