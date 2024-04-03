# Comparing `tmp/alibabacloud_ocr-api20210707-2.0.6.tar.gz` & `tmp/alibabacloud_ocr-api20210707-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ocr-api20210707-2.0.6.tar", last modified: Tue Mar 19 17:17:11 2024, max compression
+gzip compressed data, was "dist/alibabacloud_ocr-api20210707-2.0.7.tar", last modified: Wed Apr  3 03:11:40 2024, max compression
```

## Comparing `alibabacloud_ocr-api20210707-2.0.6.tar` & `alibabacloud_ocr-api20210707-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/
--rw-r--r--   0 root         (0) root         (0)     1411 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2429 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1111 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1196 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707/__init__.py
--rw-r--r--   0 root         (0) root         (0)   233305 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707/client.py
--rw-r--r--   0 root         (0) root         (0)   358900 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2429 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      452 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2633 2024-03-19 17:17:11.000000 alibabacloud_ocr-api20210707-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1111 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1196 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   233549 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707/client.py
+-rw-r--r--   0 root         (0) root         (0)   359194 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      452 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2633 2024-04-03 03:11:40.000000 alibabacloud_ocr-api20210707-2.0.7/setup.py
```

### Comparing `alibabacloud_ocr-api20210707-2.0.6/ChangeLog.md` & `alibabacloud_ocr-api20210707-2.0.7/ChangeLog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-03-19 Version: 2.0.6
+- Update API RecognizeBasic: add param NeedRotate.
+
+
 2024-03-15 Version: 2.0.5
 - Update API VerifyVATInvoice: add param InvoiceKind.
 
 
 2024-01-23 Version: 2.0.4
 - Generated python 2021-07-07 for ocr-api.
```

### Comparing `alibabacloud_ocr-api20210707-2.0.6/LICENSE` & `alibabacloud_ocr-api20210707-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707-2.0.6/PKG-INFO` & `alibabacloud_ocr-api20210707-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ocr-api20210707
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud ocr-api (20210707) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr-api20210707-2.0.6/README-CN.md` & `alibabacloud_ocr-api20210707-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707-2.0.6/README.md` & `alibabacloud_ocr-api20210707-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707/client.py` & `alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3822,14 +3822,16 @@
     def recognize_mixed_invoices_with_options(
         self,
         request: ocr_api_20210707_models.RecognizeMixedInvoicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_api_20210707_models.RecognizeMixedInvoicesResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.merge_pdf_pages):
+            query['MergePdfPages'] = request.merge_pdf_pages
         if not UtilClient.is_unset(request.page_no):
             query['PageNo'] = request.page_no
         if not UtilClient.is_unset(request.url):
             query['Url'] = request.url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=request.body,
@@ -3854,14 +3856,16 @@
     async def recognize_mixed_invoices_with_options_async(
         self,
         request: ocr_api_20210707_models.RecognizeMixedInvoicesRequest,
         runtime: util_models.RuntimeOptions,
     ) -> ocr_api_20210707_models.RecognizeMixedInvoicesResponse:
         UtilClient.validate_model(request)
         query = {}
+        if not UtilClient.is_unset(request.merge_pdf_pages):
+            query['MergePdfPages'] = request.merge_pdf_pages
         if not UtilClient.is_unset(request.page_no):
             query['PageNo'] = request.page_no
         if not UtilClient.is_unset(request.url):
             query['Url'] = request.url
         req = open_api_models.OpenApiRequest(
             query=OpenApiUtilClient.query(query),
             body=request.body,
```

### Comparing `alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707/models.py` & `alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -8703,41 +8703,47 @@
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeMixedInvoicesRequest(TeaModel):
     def __init__(
         self,
+        merge_pdf_pages: bool = None,
         page_no: int = None,
         url: str = None,
         body: BinaryIO = None,
     ):
+        self.merge_pdf_pages = merge_pdf_pages
         self.page_no = page_no
         self.url = url
         self.body = body
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
+        if self.merge_pdf_pages is not None:
+            result['MergePdfPages'] = self.merge_pdf_pages
         if self.page_no is not None:
             result['PageNo'] = self.page_no
         if self.url is not None:
             result['Url'] = self.url
         if self.body is not None:
             result['body'] = self.body
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
+        if m.get('MergePdfPages') is not None:
+            self.merge_pdf_pages = m.get('MergePdfPages')
         if m.get('PageNo') is not None:
             self.page_no = m.get('PageNo')
         if m.get('Url') is not None:
             self.url = m.get('Url')
         if m.get('body') is not None:
             self.body = m.get('body')
         return self
```

### Comparing `alibabacloud_ocr-api20210707-2.0.6/alibabacloud_ocr_api20210707.egg-info/PKG-INFO` & `alibabacloud_ocr-api20210707-2.0.7/alibabacloud_ocr_api20210707.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ocr-api20210707
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud ocr-api (20210707) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr-api20210707-2.0.6/setup.py` & `alibabacloud_ocr-api20210707-2.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ocr-api20210707.
 
-Created on 19/03/2024
+Created on 03/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ocr_api20210707"
 NAME = "alibabacloud_ocr-api20210707" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ocr-api (20210707) SDK Library for Python"
```

