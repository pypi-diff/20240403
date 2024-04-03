# Comparing `tmp/alibabacloud_ocr-api20210707_py2-2.0.6.tar.gz` & `tmp/alibabacloud_ocr-api20210707_py2-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_ocr-api20210707_py2-2.0.6.tar", last modified: Tue Mar 19 17:11:36 2024, max compression
+gzip compressed data, was "dist/alibabacloud_ocr-api20210707_py2-2.0.7.tar", last modified: Wed Apr  3 03:11:16 2024, max compression
```

## Comparing `alibabacloud_ocr-api20210707_py2-2.0.6.tar` & `alibabacloud_ocr-api20210707_py2-2.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/
--rw-r--r--   0 root         (0) root         (0)     1130 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      588 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       28 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2496 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1045 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1128 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707/
--rw-r--r--   0 root         (0) root         (0)       21 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92480 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707/client.py
--rw-r--r--   0 root         (0) root         (0)   362785 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2496 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      472 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      172 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707_py2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2925 2024-03-19 17:11:36.000000 alibabacloud_ocr-api20210707_py2-2.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/
+-rw-r--r--   0 root         (0) root         (0)     1209 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      588 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       28 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92602 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707/client.py
+-rw-r--r--   0 root         (0) root         (0)   363077 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2496 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      472 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      172 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707_py2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-03 03:11:16.000000 alibabacloud_ocr-api20210707_py2-2.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2925 2024-04-03 03:11:15.000000 alibabacloud_ocr-api20210707_py2-2.0.7/setup.py
```

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/ChangeLog.md` & `alibabacloud_ocr-api20210707_py2-2.0.7/ChangeLog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-03-19 Version: 2.0.6
+- Update API RecognizeBasic: add param NeedRotate.
+
+
 2024-03-15 Version: 2.0.5
 - Update API VerifyVATInvoice: add param InvoiceKind.
 
 
 2024-01-23 Version: 2.0.4
 - Generated python2 2021-07-07 for ocr-api.
```

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/LICENSE` & `alibabacloud_ocr-api20210707_py2-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/PKG-INFO` & `alibabacloud_ocr-api20210707_py2-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_ocr-api20210707_py2
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud ocr-api (20210707) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/README-CN.md` & `alibabacloud_ocr-api20210707_py2-2.0.7/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/README.md` & `alibabacloud_ocr-api20210707_py2-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707/client.py` & `alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1589,14 +1589,16 @@
     def recognize_medical_device_produce_license(self, request):
         runtime = util_models.RuntimeOptions()
         return self.recognize_medical_device_produce_license_with_options(request, runtime)
 
     def recognize_mixed_invoices_with_options(self, request, runtime):
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

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707/models.py` & `alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -7623,38 +7623,43 @@
         if m.get('body') is not None:
             temp_model = RecognizeMedicalDeviceProduceLicenseResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
 class RecognizeMixedInvoicesRequest(TeaModel):
-    def __init__(self, page_no=None, url=None, body=None):
+    def __init__(self, merge_pdf_pages=None, page_no=None, url=None, body=None):
+        self.merge_pdf_pages = merge_pdf_pages  # type: bool
         self.page_no = page_no  # type: int
         self.url = url  # type: str
         self.body = body  # type: READABLE
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super(RecognizeMixedInvoicesRequest, self).to_map()
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
 
     def from_map(self, m=None):
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

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/alibabacloud_ocr_api20210707_py2.egg-info/PKG-INFO` & `alibabacloud_ocr-api20210707_py2-2.0.7/alibabacloud_ocr_api20210707_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-ocr-api20210707-py2
-Version: 2.0.6
+Version: 2.0.7
 Summary: Alibaba Cloud ocr-api (20210707) SDK Library for Python2
 Home-page: https://github.com/aliyun/alibabacloud-python2-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_ocr-api20210707_py2-2.0.6/setup.py` & `alibabacloud_ocr-api20210707_py2-2.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import os
 import sys
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_ocr-api20210707_py2.
 
-Created on 19/03/2024
+Created on 03/04/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_ocr_api20210707"
 NAME = "alibabacloud_ocr-api20210707_py2" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud ocr-api (20210707) SDK Library for Python2"
```

