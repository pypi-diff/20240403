# Comparing `tmp/directory_forms_api_client-7.4.0-py3-none-any.whl.zip` & `tmp/directory_forms_api_client-7.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8528 bytes, number of entries: 10
--rw-r--r--  2.0 unx       95 b- defN 24-Mar-18 12:28 directory_forms_api_client/__init__.py
--rw-r--r--  2.0 unx     4017 b- defN 24-Mar-18 12:28 directory_forms_api_client/actions.py
--rw-r--r--  2.0 unx     1694 b- defN 24-Mar-18 12:28 directory_forms_api_client/client.py
--rw-r--r--  2.0 unx     1888 b- defN 24-Mar-18 12:28 directory_forms_api_client/forms.py
--rw-r--r--  2.0 unx     1828 b- defN 24-Mar-18 12:28 directory_forms_api_client/helpers.py
--rw-r--r--  2.0 unx     1091 b- defN 24-Mar-18 12:28 directory_forms_api_client-7.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     9867 b- defN 24-Mar-18 12:28 directory_forms_api_client-7.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-18 12:28 directory_forms_api_client-7.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       27 b- defN 24-Mar-18 12:28 directory_forms_api_client-7.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      947 b- defN 24-Mar-18 12:28 directory_forms_api_client-7.4.0.dist-info/RECORD
-10 files, 21546 bytes uncompressed, 6872 bytes compressed:  68.1%
+Zip file size: 8523 bytes, number of entries: 10
+-rw-r--r--  2.0 unx       95 b- defN 24-Mar-26 13:51 directory_forms_api_client/__init__.py
+-rw-r--r--  2.0 unx     3951 b- defN 24-Mar-26 13:51 directory_forms_api_client/actions.py
+-rw-r--r--  2.0 unx     1694 b- defN 24-Mar-26 13:51 directory_forms_api_client/client.py
+-rw-r--r--  2.0 unx     1888 b- defN 24-Mar-26 13:51 directory_forms_api_client/forms.py
+-rw-r--r--  2.0 unx     1828 b- defN 24-Mar-26 13:51 directory_forms_api_client/helpers.py
+-rw-r--r--  2.0 unx     1091 b- defN 24-Mar-26 13:52 directory_forms_api_client-7.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9867 b- defN 24-Mar-26 13:52 directory_forms_api_client-7.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-26 13:52 directory_forms_api_client-7.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       27 b- defN 24-Mar-26 13:52 directory_forms_api_client-7.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      947 b- defN 24-Mar-26 13:52 directory_forms_api_client-7.4.1.dist-info/RECORD
+10 files, 21480 bytes uncompressed, 6867 bytes compressed:  68.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: directory_forms_api_client/forms.py
 Comment: 
 
 Filename: directory_forms_api_client/helpers.py
 Comment: 
 
-Filename: directory_forms_api_client-7.4.0.dist-info/LICENSE
+Filename: directory_forms_api_client-7.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: directory_forms_api_client-7.4.0.dist-info/METADATA
+Filename: directory_forms_api_client-7.4.1.dist-info/METADATA
 Comment: 
 
-Filename: directory_forms_api_client-7.4.0.dist-info/WHEEL
+Filename: directory_forms_api_client-7.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: directory_forms_api_client-7.4.0.dist-info/top_level.txt
+Filename: directory_forms_api_client-7.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: directory_forms_api_client-7.4.0.dist-info/RECORD
+Filename: directory_forms_api_client-7.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## directory_forms_api_client/actions.py

```diff
@@ -106,20 +106,19 @@
         super().__init__(*args, **kwargs)
 
 
 class GovNotifyBulkEmailAction(AbstractAction):
     name = 'gov-notify-bulk-email'
 
     def __init__(
-        self, template_id, email_addresses, email_reply_to_id=None,
+        self, template_id, email_reply_to_id=None,
         *args, **kwargs
     ):
         self.meta = {
-            'template_id': template_id,
-            'email_addresses': email_addresses,
+            'template_id': template_id
         }
         if email_reply_to_id:
             self.meta['email_reply_to_id'] = email_reply_to_id
         super().__init__(*args, **kwargs)
 
 
 class GovNotifyLetterAction(AbstractAction):
```

## Comparing `directory_forms_api_client-7.4.0.dist-info/LICENSE` & `directory_forms_api_client-7.4.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `directory_forms_api_client-7.4.0.dist-info/METADATA` & `directory_forms_api_client-7.4.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: directory-forms-api-client
-Version: 7.4.0
+Version: 7.4.1
 Summary: Python API client for Directory forms .
 Home-page: https://github.com/uktrade/directory-forms-api-client
 Author: Department for International Trade
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

## Comparing `directory_forms_api_client-7.4.0.dist-info/RECORD` & `directory_forms_api_client-7.4.1.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 directory_forms_api_client/__init__.py,sha256=KqAK9V-nuLVYF7EzyQNFVSIC7E2O_jWWb2CtCYNPOU8,95
-directory_forms_api_client/actions.py,sha256=pYOyCyf0jl8-M7gxha3y5a6Fq7fMt_6XHdtMjt9KFzA,4017
+directory_forms_api_client/actions.py,sha256=-zG7MywWxISGcO3axOieeTYX65slB4wBpE5hVeS16SU,3951
 directory_forms_api_client/client.py,sha256=5-vTUuGhc5lGSWgIoMeJK_ECzz3AG5drU4jIMh_BQUw,1694
 directory_forms_api_client/forms.py,sha256=Edz7Ot0PoelHwDmHZiPJIuQYGbfP4EScdBuxaa6RGQY,1888
 directory_forms_api_client/helpers.py,sha256=oz7N7YYW4FK5iwm5fWM7XwjOVndJbW3Ndr3FRMEdJNA,1828
-directory_forms_api_client-7.4.0.dist-info/LICENSE,sha256=q4QjlbTN37umB_xq3DRmS0qvT2tMO_5_-u0WWzYcDQE,1091
-directory_forms_api_client-7.4.0.dist-info/METADATA,sha256=KnTObi8zmP7UF5Kq9g9RzPdl2aahFot9dEgNKFU1Kss,9867
-directory_forms_api_client-7.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-directory_forms_api_client-7.4.0.dist-info/top_level.txt,sha256=gv9OO61BimYYZjW7FO0hQ0kM1IUPSYZz7e83_7QBx7c,27
-directory_forms_api_client-7.4.0.dist-info/RECORD,,
+directory_forms_api_client-7.4.1.dist-info/LICENSE,sha256=q4QjlbTN37umB_xq3DRmS0qvT2tMO_5_-u0WWzYcDQE,1091
+directory_forms_api_client-7.4.1.dist-info/METADATA,sha256=mo2LBQGIIxxtH8agjRTLgEJ_rqRncBl4uyyaVmY98ME,9867
+directory_forms_api_client-7.4.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+directory_forms_api_client-7.4.1.dist-info/top_level.txt,sha256=gv9OO61BimYYZjW7FO0hQ0kM1IUPSYZz7e83_7QBx7c,27
+directory_forms_api_client-7.4.1.dist-info/RECORD,,
```

