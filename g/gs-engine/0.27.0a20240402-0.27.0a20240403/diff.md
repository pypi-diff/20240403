# Comparing `tmp/gs_engine-0.27.0a20240402-py2.py3-none-any.whl.zip` & `tmp/gs_engine-0.27.0a20240403-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12625 bytes, number of entries: 9
--rw-r--r--  2.0 unx      398 b- defN 24-Apr-02 19:01 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      593 b- defN 24-Apr-02 19:01 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx     1573 b- defN 24-Apr-02 19:01 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      204 b- defN 24-Apr-02 19:01 graphscope.runtime/conf/log4rs.yml
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-02 19:01 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx    23179 b- defN 24-Apr-02 20:04 gs_engine-0.27.0a20240402.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 24-Apr-02 20:04 gs_engine-0.27.0a20240402.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 24-Apr-02 20:04 gs_engine-0.27.0a20240402.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      831 b- defN 24-Apr-02 20:04 gs_engine-0.27.0a20240402.dist-info/RECORD
-9 files, 27601 bytes uncompressed, 11163 bytes compressed:  59.6%
+Zip file size: 12624 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 24-Apr-03 19:01 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      593 b- defN 24-Apr-03 19:01 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 24-Apr-03 19:01 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 24-Apr-03 19:01 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-03 19:01 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    23179 b- defN 24-Apr-03 20:02 gs_engine-0.27.0a20240403.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 24-Apr-03 20:02 gs_engine-0.27.0a20240403.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Apr-03 20:02 gs_engine-0.27.0a20240403.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 24-Apr-03 20:02 gs_engine-0.27.0a20240403.dist-info/RECORD
+9 files, 27601 bytes uncompressed, 11162 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: gs_engine-0.27.0a20240402.dist-info/METADATA
+Filename: gs_engine-0.27.0a20240403.dist-info/METADATA
 Comment: 
 
-Filename: gs_engine-0.27.0a20240402.dist-info/WHEEL
+Filename: gs_engine-0.27.0a20240403.dist-info/WHEEL
 Comment: 
 
-Filename: gs_engine-0.27.0a20240402.dist-info/top_level.txt
+Filename: gs_engine-0.27.0a20240403.dist-info/top_level.txt
 Comment: 
 
-Filename: gs_engine-0.27.0a20240402.dist-info/RECORD
+Filename: gs_engine-0.27.0a20240403.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.27.0a20240402.dist-info/METADATA` & `gs_engine-0.27.0a20240403.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.27.0a20240402
+Version: 0.27.0a20240403
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

## Comparing `gs_engine-0.27.0a20240402.dist-info/RECORD` & `gs_engine-0.27.0a20240403.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 graphscope.runtime/conf/executor.vineyard.properties,sha256=FX6Og8G2x4VrMvdtT-XGjTsDGkY0iTWrLlNUg2aFX6o,398
 graphscope.runtime/conf/frontend.vineyard.properties,sha256=A99pIMZorNr0hWMbPF2cX58Y1_LhfCICzgQlMcL1Xg0,593
 graphscope.runtime/conf/log4j2.xml,sha256=JiMUDFQ779aE33kOkah4-VlGQqMVW1_xlzWVZsvhHWQ,1573
 graphscope.runtime/conf/log4rs.yml,sha256=jFXF2AwsTarQhUr2vH4qD9-TJGdY2vVbvBtGYm-fotM,204
 graphscope_runtime/__init__.py,sha256=w_Me0NHI5zy8GitMCD7mzOi0Qz7ZfeE2zUI5wGfZIyM,694
-gs_engine-0.27.0a20240402.dist-info/METADATA,sha256=ukaulbSJH2vMZI5CT1B4a_4fIGum-UbpAKP7QXquyIc,23179
-gs_engine-0.27.0a20240402.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
-gs_engine-0.27.0a20240402.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
-gs_engine-0.27.0a20240402.dist-info/RECORD,,
+gs_engine-0.27.0a20240403.dist-info/METADATA,sha256=deEpIbTU50ipZtHxWdMiRNATzdB20Ty6tD9YanBQnOs,23179
+gs_engine-0.27.0a20240403.dist-info/WHEEL,sha256=-G_t0oGuE7UD0DrSpVZnq1hHMBV9DD2XkS5v7XpmTnk,110
+gs_engine-0.27.0a20240403.dist-info/top_level.txt,sha256=8OYX8275H-myeSCvZ0ZHMFaQrPlxRlQfm6Z2pK0SbFw,19
+gs_engine-0.27.0a20240403.dist-info/RECORD,,
```

