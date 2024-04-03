# Comparing `tmp/amazon-textract-caller-0.2.2.tar.gz` & `tmp/amazon-textract-caller-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon-textract-caller-0.2.2.tar", last modified: Wed Feb 14 10:44:15 2024, max compression
+gzip compressed data, was "amazon-textract-caller-0.2.3.tar", last modified: Wed Apr  3 00:33:58 2024, max compression
```

## Comparing `amazon-textract-caller-0.2.2.tar` & `amazon-textract-caller-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2024-02-14 10:44:15.619207 amazon-textract-caller-0.2.2/
--rw-r--r--   0 schadem    (504) staff       (20)    10142 2022-09-08 17:40:40.000000 amazon-textract-caller-0.2.2/LICENSE
--rw-r--r--   0 schadem    (504) staff       (20)      161 2022-09-08 17:40:40.000000 amazon-textract-caller-0.2.2/MANIFEST.in
--rw-r--r--   0 schadem    (504) staff       (20)     8294 2024-02-14 10:44:15.619359 amazon-textract-caller-0.2.2/PKG-INFO
--rw-r--r--   0 schadem    (504) staff       (20)     6067 2023-11-02 13:51:56.000000 amazon-textract-caller-0.2.2/README.md
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2024-02-14 10:44:15.618654 amazon-textract-caller-0.2.2/amazon_textract_caller.egg-info/
--rw-r--r--   0 schadem    (504) staff       (20)     8294 2024-02-14 10:44:15.000000 amazon-textract-caller-0.2.2/amazon_textract_caller.egg-info/PKG-INFO
--rw-r--r--   0 schadem    (504) staff       (20)      356 2024-02-14 10:44:15.000000 amazon-textract-caller-0.2.2/amazon_textract_caller.egg-info/SOURCES.txt
--rw-r--r--   0 schadem    (504) staff       (20)        1 2024-02-14 10:44:15.000000 amazon-textract-caller-0.2.2/amazon_textract_caller.egg-info/dependency_links.txt
--rw-r--r--   0 schadem    (504) staff       (20)      114 2024-02-14 10:44:15.000000 amazon-textract-caller-0.2.2/amazon_textract_caller.egg-info/requires.txt
--rw-r--r--   0 schadem    (504) staff       (20)       15 2024-02-14 10:44:15.000000 amazon-textract-caller-0.2.2/amazon_textract_caller.egg-info/top_level.txt
--rw-r--r--   0 schadem    (504) staff       (20)      399 2024-02-14 10:44:15.619650 amazon-textract-caller-0.2.2/setup.cfg
--rw-r--r--   0 schadem    (504) staff       (20)     2075 2024-02-14 10:43:58.000000 amazon-textract-caller-0.2.2/setup.py
-drwxr-xr-x   0 schadem    (504) staff       (20)        0 2024-02-14 10:44:15.619053 amazon-textract-caller-0.2.2/textractcaller/
--rw-r--r--   0 schadem    (504) staff       (20)      594 2023-11-02 13:51:56.000000 amazon-textract-caller-0.2.2/textractcaller/__init__.py
--rw-r--r--   0 schadem    (504) staff       (20)       23 2024-02-14 10:43:58.000000 amazon-textract-caller-0.2.2/textractcaller/_version.py
--rw-r--r--   0 schadem    (504) staff       (20)    32213 2024-02-14 10:43:58.000000 amazon-textract-caller-0.2.2/textractcaller/t_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:33:58.032602 amazon-textract-caller-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-04-03 00:33:48.000000 amazon-textract-caller-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-03 00:33:58.032602 amazon-textract-caller-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-03 00:33:48.000000 amazon-textract-caller-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:33:58.032602 amazon-textract-caller-0.2.3/amazon_textract_caller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-03 00:33:58.000000 amazon-textract-caller-0.2.3/amazon_textract_caller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-03 00:33:58.000000 amazon-textract-caller-0.2.3/amazon_textract_caller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:33:58.000000 amazon-textract-caller-0.2.3/amazon_textract_caller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 00:33:58.000000 amazon-textract-caller-0.2.3/amazon_textract_caller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 00:33:58.000000 amazon-textract-caller-0.2.3/amazon_textract_caller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-03 00:33:58.032602 amazon-textract-caller-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-03 00:33:48.000000 amazon-textract-caller-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:33:58.032602 amazon-textract-caller-0.2.3/textractcaller/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 00:33:48.000000 amazon-textract-caller-0.2.3/textractcaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 00:33:48.000000 amazon-textract-caller-0.2.3/textractcaller/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33003 2024-04-03 00:33:48.000000 amazon-textract-caller-0.2.3/textractcaller/t_call.py
```

### Comparing `amazon-textract-caller-0.2.2/LICENSE` & `amazon-textract-caller-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon-textract-caller-0.2.2/PKG-INFO` & `amazon-textract-caller-0.2.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,196 @@
 Metadata-Version: 2.1
 Name: amazon-textract-caller
-Version: 0.2.2
+Version: 0.2.3
 Summary: Amazon Textract Caller tools
 Home-page: https://github.com/aws-samples/amazon-textract-textractor/tree/master/caller
 Author: Amazon Rekognition Textract Demoes
 Author-email: rekognition-textract-demos@amazon.com
 License: Apache License Version 2.0
-Description: # Textract-Caller
-        
-        amazon-textract-caller provides a collection of ready to use functions and sample implementations to speed up the evaluation and development for any project using Amazon Textract.
-        
-        Making it easy to call Amazon Textract regardless of file type and location.
-        
-        ## Install
-        
-        ```bash
-        > python -m pip install amazon-textract-caller
-        ```
-        
-        ## Functions
-        
-        ```python
-        from textractcaller import call_textract
-        def call_textract(input_document: Union[str, bytes],
-                          features: Optional[List[Textract_Features]] = None,
-                          queries_config: Optional[QueriesConfig] = None,
-                          output_config: Optional[OutputConfig] = None,
-                          adapters_config: Optional[AdaptersConfig] = None,
-                          kms_key_id: str = "",
-                          job_tag: str = "",
-                          notification_channel: Optional[NotificationChannel] = None,
-                          client_request_token: str = "",
-                          return_job_id: bool = False,
-                          force_async_api: bool = False,
-                          call_mode: Textract_Call_Mode = Textract_Call_Mode.DEFAULT,
-                          boto3_textract_client=None,
-                          job_done_polling_interval=1) -> dict:
-        ```
-        
-        Also useful when receiving the JSON response from an asynchronous job (start_document_text_detection or start_document_analysis)
-        
-        ```python
-        from textractcaller import get_full_json
-        def get_full_json(job_id: str = None,
-                          textract_api: Textract_API = Textract_API.DETECT,
-                          boto3_textract_client=None)->dict:
-        ```
-        
-        And when receiving the JSON from the OutputConfig location, this method is useful as well.
-        
-        ```python
-        from textractcaller import get_full_json_from_output_config
-        def get_full_json_from_output_config(output_config: OutputConfig = None,
-                                             job_id: str = None,
-                                             s3_client = None)->dict:
-        ```
-        
-        ## Samples
-        
-        ### Calling with file from local filesystem only with detect_text
-        
-        ```python
-        textract_json = call_textract(input_document="/folder/local-filesystem-file.png")
-        ```
-        
-        ### Calling with file from local filesystem only detect_text and using in Textract Response Parser
-        
-        (needs trp dependency through ```python -m pip install amazon-textract-response-parser```)
-        
-        ```python
-        import json
-        from trp import Document
-        from textractcaller import call_textract
-        
-        textract_json = call_textract(input_document="/folder/local-filesystem-file.png")
-        d = Document(textract_json)
-        ```
-        
-        ### Calling with Queries for a multi-page document and extract the Answers
-        
-        sample also uses the amazon-textract-response-parser
-        
-        ```
-        python -m pip install amazon-textract-caller amazon-textract-response-parser
-        ```
-        
-        ```python
-        import textractcaller as tc
-        import trp.trp2 as t2
-        import boto3
-        
-        textract = boto3.client('textract', region_name="us-east-2")
-        q1 = tc.Query(text="What is the employee SSN?", alias="SSN", pages=["1"])
-        q2 = tc.Query(text="What is YTD gross pay?", alias="GROSS_PAY", pages=["2"])
-        textract_json = tc.call_textract(
-            input_document="s3://amazon-textract-public-content/blogs/2-pager.pdf",
-            queries_config=tc.QueriesConfig(queries=[q1, q2]),
-            features=[tc.Textract_Features.QUERIES],
-            force_async_api=True,
-            boto3_textract_client=textract)
-        t_doc: t2.TDocument = t2.TDocumentSchema().load(textract_json)  # type: ignore
-        for page in t_doc.pages:
-            query_answers = t_doc.get_query_answers(page=page)
-            for x in query_answers:
-                print(f"{x[1]},{x[2]}")
-        ```
-        
-        ### Calling with Custom Queries for a multi-page document using an adapter
-        
-        sample also uses the amazon-textract-response-parser
-        
-        ```
-        python -m pip install amazon-textract-caller amazon-textract-response-parser
-        ```
-        
-        ```python
-        import textractcaller as tc
-        import trp.trp2 as t2
-        import boto3
-        
-        textract = boto3.client('textract', region_name="us-east-2")
-        q1 = tc.Query(text="What is the employee SSN?", alias="SSN", pages=["1"])
-        q2 = tc.Query(text="What is YTD gross pay?", alias="GROSS_PAY", pages=["2"])
-        adapter1 = tc.Adapter(adapter_id="2e9bf1c4aa31", version="1", pages=["1"])
-        textract_json = tc.call_textract(
-            input_document="s3://amazon-textract-public-content/blogs/2-pager.pdf",
-            queries_config=tc.QueriesConfig(queries=[q1, q2]),
-            adapters_config=tc.AdaptersConfig(adapters=[adapter1])
-            features=[tc.Textract_Features.QUERIES],
-            force_async_api=True,
-            boto3_textract_client=textract)
-        t_doc: t2.TDocument = t2.TDocumentSchema().load(textract_json)  # type: ignore
-        for page in t_doc.pages:
-            query_answers = t_doc.get_query_answers(page=page)
-            for x in query_answers:
-                print(f"{x[1]},{x[2]}")
-        ```
-        
-        
-        ### Calling with file from local filesystem with TABLES features
-        
-        ```python
-        from textractcaller import call_textract, Textract_Features
-        features = [Textract_Features.TABLES]
-        response = call_textract(
-            input_document="/folder/local-filesystem-file.png", features=features)
-        ```
-        
-        ### Call with images located on S3 but force asynchronous API
-        
-        ```python
-        from textractcaller import call_textract
-        response = call_textract(input_document="s3://some-bucket/w2-example.png", force_async_api=True)
-        ```
-        
-        ### Call with OutputConfig, Customer-Managed-Key
-        
-        ```python
-        from textractcaller import call_textract
-        from textractcaller import OutputConfig, Textract_Features
-        output_config = OutputConfig(s3_bucket="somebucket-encrypted", s3_prefix="output/")
-        response = call_textract(input_document="s3://someprefix/somefile.png",
-                                  force_async_api=True,
-                                  output_config=output_config,
-                                  kms_key_id="arn:aws:kms:us-east-1:12345678901:key/some-key-id-ref-erence",
-                                  return_job_id=False,
-                                  job_tag="sometag",
-                                  client_request_token="sometoken")
-        
-        ```
-        
-        ### Call with PDF located on S3 and force return of JobId instead of JSON response
-        
-        ```python
-        from textractcaller import call_textract
-        response = call_textract(input_document="s3://some-bucket/some-document.pdf", return_job_id=True)
-        job_id = response['JobId']
-        ```
-        
 Keywords: amazon-textract-textractor amazon textract textractor helper caller
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+# Textract-Caller
+
+amazon-textract-caller provides a collection of ready to use functions and sample implementations to speed up the evaluation and development for any project using Amazon Textract.
+
+Making it easy to call Amazon Textract regardless of file type and location.
+
+## Install
+
+```bash
+> python -m pip install amazon-textract-caller
+```
+
+## Functions
+
+```python
+from textractcaller import call_textract
+def call_textract(input_document: Union[str, bytes],
+                  features: Optional[List[Textract_Features]] = None,
+                  queries_config: Optional[QueriesConfig] = None,
+                  output_config: Optional[OutputConfig] = None,
+                  adapters_config: Optional[AdaptersConfig] = None,
+                  kms_key_id: str = "",
+                  job_tag: str = "",
+                  notification_channel: Optional[NotificationChannel] = None,
+                  client_request_token: str = "",
+                  return_job_id: bool = False,
+                  force_async_api: bool = False,
+                  call_mode: Textract_Call_Mode = Textract_Call_Mode.DEFAULT,
+                  boto3_textract_client=None,
+                  job_done_polling_interval=1) -> dict:
+```
+
+Also useful when receiving the JSON response from an asynchronous job (start_document_text_detection or start_document_analysis)
+
+```python
+from textractcaller import get_full_json
+def get_full_json(job_id: str = None,
+                  textract_api: Textract_API = Textract_API.DETECT,
+                  boto3_textract_client=None)->dict:
+```
+
+And when receiving the JSON from the OutputConfig location, this method is useful as well.
+
+```python
+from textractcaller import get_full_json_from_output_config
+def get_full_json_from_output_config(output_config: OutputConfig = None,
+                                     job_id: str = None,
+                                     s3_client = None)->dict:
+```
+
+## Samples
+
+### Calling with file from local filesystem only with detect_text
+
+```python
+textract_json = call_textract(input_document="/folder/local-filesystem-file.png")
+```
+
+### Calling with file from local filesystem only detect_text and using in Textract Response Parser
+
+(needs trp dependency through ```python -m pip install amazon-textract-response-parser```)
+
+```python
+import json
+from trp import Document
+from textractcaller import call_textract
+
+textract_json = call_textract(input_document="/folder/local-filesystem-file.png")
+d = Document(textract_json)
+```
+
+### Calling with Queries for a multi-page document and extract the Answers
+
+sample also uses the amazon-textract-response-parser
+
+```
+python -m pip install amazon-textract-caller amazon-textract-response-parser
+```
+
+```python
+import textractcaller as tc
+import trp.trp2 as t2
+import boto3
+
+textract = boto3.client('textract', region_name="us-east-2")
+q1 = tc.Query(text="What is the employee SSN?", alias="SSN", pages=["1"])
+q2 = tc.Query(text="What is YTD gross pay?", alias="GROSS_PAY", pages=["2"])
+textract_json = tc.call_textract(
+    input_document="s3://amazon-textract-public-content/blogs/2-pager.pdf",
+    queries_config=tc.QueriesConfig(queries=[q1, q2]),
+    features=[tc.Textract_Features.QUERIES],
+    force_async_api=True,
+    boto3_textract_client=textract)
+t_doc: t2.TDocument = t2.TDocumentSchema().load(textract_json)  # type: ignore
+for page in t_doc.pages:
+    query_answers = t_doc.get_query_answers(page=page)
+    for x in query_answers:
+        print(f"{x[1]},{x[2]}")
+```
+
+### Calling with Custom Queries for a multi-page document using an adapter
+
+sample also uses the amazon-textract-response-parser
+
+```
+python -m pip install amazon-textract-caller amazon-textract-response-parser
+```
+
+```python
+import textractcaller as tc
+import trp.trp2 as t2
+import boto3
+
+textract = boto3.client('textract', region_name="us-east-2")
+q1 = tc.Query(text="What is the employee SSN?", alias="SSN", pages=["1"])
+q2 = tc.Query(text="What is YTD gross pay?", alias="GROSS_PAY", pages=["2"])
+adapter1 = tc.Adapter(adapter_id="2e9bf1c4aa31", version="1", pages=["1"])
+textract_json = tc.call_textract(
+    input_document="s3://amazon-textract-public-content/blogs/2-pager.pdf",
+    queries_config=tc.QueriesConfig(queries=[q1, q2]),
+    adapters_config=tc.AdaptersConfig(adapters=[adapter1])
+    features=[tc.Textract_Features.QUERIES],
+    force_async_api=True,
+    boto3_textract_client=textract)
+t_doc: t2.TDocument = t2.TDocumentSchema().load(textract_json)  # type: ignore
+for page in t_doc.pages:
+    query_answers = t_doc.get_query_answers(page=page)
+    for x in query_answers:
+        print(f"{x[1]},{x[2]}")
+```
+
+
+### Calling with file from local filesystem with TABLES features
+
+```python
+from textractcaller import call_textract, Textract_Features
+features = [Textract_Features.TABLES]
+response = call_textract(
+    input_document="/folder/local-filesystem-file.png", features=features)
+```
+
+### Call with images located on S3 but force asynchronous API
+
+```python
+from textractcaller import call_textract
+response = call_textract(input_document="s3://some-bucket/w2-example.png", force_async_api=True)
+```
+
+### Call with OutputConfig, Customer-Managed-Key
+
+```python
+from textractcaller import call_textract
+from textractcaller import OutputConfig, Textract_Features
+output_config = OutputConfig(s3_bucket="somebucket-encrypted", s3_prefix="output/")
+response = call_textract(input_document="s3://someprefix/somefile.png",
+                          force_async_api=True,
+                          output_config=output_config,
+                          kms_key_id="arn:aws:kms:us-east-1:12345678901:key/some-key-id-ref-erence",
+                          return_job_id=False,
+                          job_tag="sometag",
+                          client_request_token="sometoken")
+
+```
+
+### Call with PDF located on S3 and force return of JobId instead of JSON response
+
+```python
+from textractcaller import call_textract
+response = call_textract(input_document="s3://some-bucket/some-document.pdf", return_job_id=True)
+job_id = response['JobId']
+```
+
+
```

### Comparing `amazon-textract-caller-0.2.2/README.md` & `amazon-textract-caller-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `amazon-textract-caller-0.2.2/amazon_textract_caller.egg-info/PKG-INFO` & `amazon-textract-caller-0.2.3/amazon_textract_caller.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,192 +1,196 @@
 Metadata-Version: 2.1
 Name: amazon-textract-caller
-Version: 0.2.2
+Version: 0.2.3
 Summary: Amazon Textract Caller tools
 Home-page: https://github.com/aws-samples/amazon-textract-textractor/tree/master/caller
 Author: Amazon Rekognition Textract Demoes
 Author-email: rekognition-textract-demos@amazon.com
 License: Apache License Version 2.0
-Description: # Textract-Caller
-        
-        amazon-textract-caller provides a collection of ready to use functions and sample implementations to speed up the evaluation and development for any project using Amazon Textract.
-        
-        Making it easy to call Amazon Textract regardless of file type and location.
-        
-        ## Install
-        
-        ```bash
-        > python -m pip install amazon-textract-caller
-        ```
-        
-        ## Functions
-        
-        ```python
-        from textractcaller import call_textract
-        def call_textract(input_document: Union[str, bytes],
-                          features: Optional[List[Textract_Features]] = None,
-                          queries_config: Optional[QueriesConfig] = None,
-                          output_config: Optional[OutputConfig] = None,
-                          adapters_config: Optional[AdaptersConfig] = None,
-                          kms_key_id: str = "",
-                          job_tag: str = "",
-                          notification_channel: Optional[NotificationChannel] = None,
-                          client_request_token: str = "",
-                          return_job_id: bool = False,
-                          force_async_api: bool = False,
-                          call_mode: Textract_Call_Mode = Textract_Call_Mode.DEFAULT,
-                          boto3_textract_client=None,
-                          job_done_polling_interval=1) -> dict:
-        ```
-        
-        Also useful when receiving the JSON response from an asynchronous job (start_document_text_detection or start_document_analysis)
-        
-        ```python
-        from textractcaller import get_full_json
-        def get_full_json(job_id: str = None,
-                          textract_api: Textract_API = Textract_API.DETECT,
-                          boto3_textract_client=None)->dict:
-        ```
-        
-        And when receiving the JSON from the OutputConfig location, this method is useful as well.
-        
-        ```python
-        from textractcaller import get_full_json_from_output_config
-        def get_full_json_from_output_config(output_config: OutputConfig = None,
-                                             job_id: str = None,
-                                             s3_client = None)->dict:
-        ```
-        
-        ## Samples
-        
-        ### Calling with file from local filesystem only with detect_text
-        
-        ```python
-        textract_json = call_textract(input_document="/folder/local-filesystem-file.png")
-        ```
-        
-        ### Calling with file from local filesystem only detect_text and using in Textract Response Parser
-        
-        (needs trp dependency through ```python -m pip install amazon-textract-response-parser```)
-        
-        ```python
-        import json
-        from trp import Document
-        from textractcaller import call_textract
-        
-        textract_json = call_textract(input_document="/folder/local-filesystem-file.png")
-        d = Document(textract_json)
-        ```
-        
-        ### Calling with Queries for a multi-page document and extract the Answers
-        
-        sample also uses the amazon-textract-response-parser
-        
-        ```
-        python -m pip install amazon-textract-caller amazon-textract-response-parser
-        ```
-        
-        ```python
-        import textractcaller as tc
-        import trp.trp2 as t2
-        import boto3
-        
-        textract = boto3.client('textract', region_name="us-east-2")
-        q1 = tc.Query(text="What is the employee SSN?", alias="SSN", pages=["1"])
-        q2 = tc.Query(text="What is YTD gross pay?", alias="GROSS_PAY", pages=["2"])
-        textract_json = tc.call_textract(
-            input_document="s3://amazon-textract-public-content/blogs/2-pager.pdf",
-            queries_config=tc.QueriesConfig(queries=[q1, q2]),
-            features=[tc.Textract_Features.QUERIES],
-            force_async_api=True,
-            boto3_textract_client=textract)
-        t_doc: t2.TDocument = t2.TDocumentSchema().load(textract_json)  # type: ignore
-        for page in t_doc.pages:
-            query_answers = t_doc.get_query_answers(page=page)
-            for x in query_answers:
-                print(f"{x[1]},{x[2]}")
-        ```
-        
-        ### Calling with Custom Queries for a multi-page document using an adapter
-        
-        sample also uses the amazon-textract-response-parser
-        
-        ```
-        python -m pip install amazon-textract-caller amazon-textract-response-parser
-        ```
-        
-        ```python
-        import textractcaller as tc
-        import trp.trp2 as t2
-        import boto3
-        
-        textract = boto3.client('textract', region_name="us-east-2")
-        q1 = tc.Query(text="What is the employee SSN?", alias="SSN", pages=["1"])
-        q2 = tc.Query(text="What is YTD gross pay?", alias="GROSS_PAY", pages=["2"])
-        adapter1 = tc.Adapter(adapter_id="2e9bf1c4aa31", version="1", pages=["1"])
-        textract_json = tc.call_textract(
-            input_document="s3://amazon-textract-public-content/blogs/2-pager.pdf",
-            queries_config=tc.QueriesConfig(queries=[q1, q2]),
-            adapters_config=tc.AdaptersConfig(adapters=[adapter1])
-            features=[tc.Textract_Features.QUERIES],
-            force_async_api=True,
-            boto3_textract_client=textract)
-        t_doc: t2.TDocument = t2.TDocumentSchema().load(textract_json)  # type: ignore
-        for page in t_doc.pages:
-            query_answers = t_doc.get_query_answers(page=page)
-            for x in query_answers:
-                print(f"{x[1]},{x[2]}")
-        ```
-        
-        
-        ### Calling with file from local filesystem with TABLES features
-        
-        ```python
-        from textractcaller import call_textract, Textract_Features
-        features = [Textract_Features.TABLES]
-        response = call_textract(
-            input_document="/folder/local-filesystem-file.png", features=features)
-        ```
-        
-        ### Call with images located on S3 but force asynchronous API
-        
-        ```python
-        from textractcaller import call_textract
-        response = call_textract(input_document="s3://some-bucket/w2-example.png", force_async_api=True)
-        ```
-        
-        ### Call with OutputConfig, Customer-Managed-Key
-        
-        ```python
-        from textractcaller import call_textract
-        from textractcaller import OutputConfig, Textract_Features
-        output_config = OutputConfig(s3_bucket="somebucket-encrypted", s3_prefix="output/")
-        response = call_textract(input_document="s3://someprefix/somefile.png",
-                                  force_async_api=True,
-                                  output_config=output_config,
-                                  kms_key_id="arn:aws:kms:us-east-1:12345678901:key/some-key-id-ref-erence",
-                                  return_job_id=False,
-                                  job_tag="sometag",
-                                  client_request_token="sometoken")
-        
-        ```
-        
-        ### Call with PDF located on S3 and force return of JobId instead of JSON response
-        
-        ```python
-        from textractcaller import call_textract
-        response = call_textract(input_document="s3://some-bucket/some-document.pdf", return_job_id=True)
-        job_id = response['JobId']
-        ```
-        
 Keywords: amazon-textract-textractor amazon textract textractor helper caller
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: testing
+License-File: LICENSE
+
+# Textract-Caller
+
+amazon-textract-caller provides a collection of ready to use functions and sample implementations to speed up the evaluation and development for any project using Amazon Textract.
+
+Making it easy to call Amazon Textract regardless of file type and location.
+
+## Install
+
+```bash
+> python -m pip install amazon-textract-caller
+```
+
+## Functions
+
+```python
+from textractcaller import call_textract
+def call_textract(input_document: Union[str, bytes],
+                  features: Optional[List[Textract_Features]] = None,
+                  queries_config: Optional[QueriesConfig] = None,
+                  output_config: Optional[OutputConfig] = None,
+                  adapters_config: Optional[AdaptersConfig] = None,
+                  kms_key_id: str = "",
+                  job_tag: str = "",
+                  notification_channel: Optional[NotificationChannel] = None,
+                  client_request_token: str = "",
+                  return_job_id: bool = False,
+                  force_async_api: bool = False,
+                  call_mode: Textract_Call_Mode = Textract_Call_Mode.DEFAULT,
+                  boto3_textract_client=None,
+                  job_done_polling_interval=1) -> dict:
+```
+
+Also useful when receiving the JSON response from an asynchronous job (start_document_text_detection or start_document_analysis)
+
+```python
+from textractcaller import get_full_json
+def get_full_json(job_id: str = None,
+                  textract_api: Textract_API = Textract_API.DETECT,
+                  boto3_textract_client=None)->dict:
+```
+
+And when receiving the JSON from the OutputConfig location, this method is useful as well.
+
+```python
+from textractcaller import get_full_json_from_output_config
+def get_full_json_from_output_config(output_config: OutputConfig = None,
+                                     job_id: str = None,
+                                     s3_client = None)->dict:
+```
+
+## Samples
+
+### Calling with file from local filesystem only with detect_text
+
+```python
+textract_json = call_textract(input_document="/folder/local-filesystem-file.png")
+```
+
+### Calling with file from local filesystem only detect_text and using in Textract Response Parser
+
+(needs trp dependency through ```python -m pip install amazon-textract-response-parser```)
+
+```python
+import json
+from trp import Document
+from textractcaller import call_textract
+
+textract_json = call_textract(input_document="/folder/local-filesystem-file.png")
+d = Document(textract_json)
+```
+
+### Calling with Queries for a multi-page document and extract the Answers
+
+sample also uses the amazon-textract-response-parser
+
+```
+python -m pip install amazon-textract-caller amazon-textract-response-parser
+```
+
+```python
+import textractcaller as tc
+import trp.trp2 as t2
+import boto3
+
+textract = boto3.client('textract', region_name="us-east-2")
+q1 = tc.Query(text="What is the employee SSN?", alias="SSN", pages=["1"])
+q2 = tc.Query(text="What is YTD gross pay?", alias="GROSS_PAY", pages=["2"])
+textract_json = tc.call_textract(
+    input_document="s3://amazon-textract-public-content/blogs/2-pager.pdf",
+    queries_config=tc.QueriesConfig(queries=[q1, q2]),
+    features=[tc.Textract_Features.QUERIES],
+    force_async_api=True,
+    boto3_textract_client=textract)
+t_doc: t2.TDocument = t2.TDocumentSchema().load(textract_json)  # type: ignore
+for page in t_doc.pages:
+    query_answers = t_doc.get_query_answers(page=page)
+    for x in query_answers:
+        print(f"{x[1]},{x[2]}")
+```
+
+### Calling with Custom Queries for a multi-page document using an adapter
+
+sample also uses the amazon-textract-response-parser
+
+```
+python -m pip install amazon-textract-caller amazon-textract-response-parser
+```
+
+```python
+import textractcaller as tc
+import trp.trp2 as t2
+import boto3
+
+textract = boto3.client('textract', region_name="us-east-2")
+q1 = tc.Query(text="What is the employee SSN?", alias="SSN", pages=["1"])
+q2 = tc.Query(text="What is YTD gross pay?", alias="GROSS_PAY", pages=["2"])
+adapter1 = tc.Adapter(adapter_id="2e9bf1c4aa31", version="1", pages=["1"])
+textract_json = tc.call_textract(
+    input_document="s3://amazon-textract-public-content/blogs/2-pager.pdf",
+    queries_config=tc.QueriesConfig(queries=[q1, q2]),
+    adapters_config=tc.AdaptersConfig(adapters=[adapter1])
+    features=[tc.Textract_Features.QUERIES],
+    force_async_api=True,
+    boto3_textract_client=textract)
+t_doc: t2.TDocument = t2.TDocumentSchema().load(textract_json)  # type: ignore
+for page in t_doc.pages:
+    query_answers = t_doc.get_query_answers(page=page)
+    for x in query_answers:
+        print(f"{x[1]},{x[2]}")
+```
+
+
+### Calling with file from local filesystem with TABLES features
+
+```python
+from textractcaller import call_textract, Textract_Features
+features = [Textract_Features.TABLES]
+response = call_textract(
+    input_document="/folder/local-filesystem-file.png", features=features)
+```
+
+### Call with images located on S3 but force asynchronous API
+
+```python
+from textractcaller import call_textract
+response = call_textract(input_document="s3://some-bucket/w2-example.png", force_async_api=True)
+```
+
+### Call with OutputConfig, Customer-Managed-Key
+
+```python
+from textractcaller import call_textract
+from textractcaller import OutputConfig, Textract_Features
+output_config = OutputConfig(s3_bucket="somebucket-encrypted", s3_prefix="output/")
+response = call_textract(input_document="s3://someprefix/somefile.png",
+                          force_async_api=True,
+                          output_config=output_config,
+                          kms_key_id="arn:aws:kms:us-east-1:12345678901:key/some-key-id-ref-erence",
+                          return_job_id=False,
+                          job_tag="sometag",
+                          client_request_token="sometoken")
+
+```
+
+### Call with PDF located on S3 and force return of JobId instead of JSON response
+
+```python
+from textractcaller import call_textract
+response = call_textract(input_document="s3://some-bucket/some-document.pdf", return_job_id=True)
+job_id = response['JobId']
+```
+
+
```

### Comparing `amazon-textract-caller-0.2.2/setup.py` & `amazon-textract-caller-0.2.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     os.system('twine upload --repository pypi dist/*')
     sys.exit()
 
 setup(name='amazon-textract-caller',
       packages=find_packages(exclude=['tests']),
       include_package_data=True,
       exclude_package_data={"": ["test_*.py", "__pycache__"]},
-      version='0.2.2',
+      version='0.2.3',
       description='Amazon Textract Caller tools',
       install_requires=requirements,
       extras_require={'testing': ['amazon-textract-response-parser', 'pytest']},
       long_description_content_type='text/markdown',
       long_description=read('README.md'),
       author='Amazon Rekognition Textract Demoes',
       author_email='rekognition-textract-demos@amazon.com',
@@ -44,9 +44,10 @@
           "Development Status :: 4 - Beta",
           "Topic :: Utilities",
           'License :: OSI Approved :: Apache Software License',
           'Programming Language :: Python :: 3.8',
           'Programming Language :: Python :: 3.9',
           'Programming Language :: Python :: 3.10',
           'Programming Language :: Python :: 3.11',
+          'Programming Language :: Python :: 3.12',
       ],
       python_requires='>=3.6')
```

### Comparing `amazon-textract-caller-0.2.2/textractcaller/__init__.py` & `amazon-textract-caller-0.2.3/textractcaller/__init__.py`

 * *Files identical despite different names*

### Comparing `amazon-textract-caller-0.2.2/textractcaller/t_call.py` & `amazon-textract-caller-0.2.3/textractcaller/t_call.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Union, List, Optional
+from typing import Union, List, Optional, Tuple
 from enum import Enum
 import os
 from dataclasses import dataclass, field
 import boto3
 import time
 import logging
 import json
@@ -170,14 +170,24 @@
 
 def is_tiff(filename: str) -> bool:
     _, suffix = os.path.splitext(filename)
     if suffix in tiff_suffixes:
         return True
     return False
 
+def parse_s3_url(url: str) -> Tuple[str, str]:
+    if url.lower().startswith("s3://"):
+        url_parts = url[5:].split("/", 1)
+        bucket = url_parts[0]
+        key = url_parts[1] if len(url_parts) > 1 else None
+        if not key:
+            raise ValueError(f"Missing object key in S3 path {url}")    
+        return bucket, key
+    else:
+        raise ValueError("URL must be in s3://bucket/path/to/file format")
 
 def generate_request_params(
     document_location: Optional[DocumentLocation] = None,
     document: Optional[Document] = None,
     features: Optional[List[Textract_Features]] = None,
     queries_config: Optional[QueriesConfig] = None,
     adapters_config: Optional[AdaptersConfig] = None,
@@ -485,15 +495,17 @@
     output_config: Optional[OutputConfig] = None,
     kms_key_id: str = "",
     return_job_id: bool = False,
     job_done_polling_interval=1,
     boto3_textract_client=None,
 ):
     if len(input_document) > 7 and input_document.lower().startswith("s3://"):
-        s3_bucket, s3_key = input_document.replace("s3://", "").split("/", 1)
+        # Fix #345
+        # s3_bucket, s3_key = input_document.replace("s3://", "").split("/", 1)
+        s3_bucket, s3_key = parse_s3_url(url=input_document)
     else:
         raise Exception("input_document needs to be an S3 URL.")
 
     if not boto3_textract_client:
         textract = boto3.client("textract")
     else:
         textract = boto3_textract_client
@@ -572,15 +584,17 @@
     elif call_mode == Textract_Call_Mode.FORCE_ASYNC:
         force_async_api = True
     if force_async_api and force_sync_api:
         raise ValueError("can not force both, async and sync")
     if isinstance(input_document, str):
         if len(input_document) > 7 and input_document.lower().startswith("s3://"):
             is_s3_document = True
-            s3_bucket, s3_key = input_document.replace("s3://", "").split("/", 1)
+            # Fix #345
+            # s3_bucket, s3_key = input_document.replace("s3://", "").split("/", 1)
+            s3_bucket, s3_key = parse_s3_url(url=input_document)
         ext: str = ""
         _, ext = os.path.splitext(input_document)
         ext = ext.lower()
         is_pdf: bool = (ext is not None and ext.lower() in only_async_suffixes) or (mime_type == 'application/pdf')
 
         if is_pdf and not is_s3_document:
             raise ValueError("PDF only supported when located on S3")
@@ -743,15 +757,17 @@
         textract = boto3_textract_client
 
     document_pages_param: List[DocumentPage] = list()
     for input_document in document_pages:
         if isinstance(input_document, str):
             if len(input_document) > 7 and input_document.lower().startswith("s3://"):
                 logger.debug("processing s3")
-                s3_bucket, s3_key = input_document.replace("s3://", "").split("/", 1)
+                # Fix #345
+                # s3_bucket, s3_key = input_document.replace("s3://", "").split("/", 1)
+                s3_bucket, s3_key = parse_s3_url(url=input_document)
                 document_pages_param.append(
                     DocumentPage(
                         s3_object=DocumentLocation(
                             s3_bucket=s3_bucket, s3_prefix=s3_key
                         )
                     )
                 )
@@ -789,15 +805,17 @@
     is_s3_document: bool = False
     s3_bucket = ""
     s3_key = ""
     result_value = {}
     if isinstance(input_document, str):
         if len(input_document) > 7 and input_document.lower().startswith("s3://"):
             is_s3_document = True
-            s3_bucket, s3_key = input_document.replace("s3://", "").split("/", 1)
+            # Fix #345
+            # s3_bucket, s3_key = input_document.replace("s3://", "").split("/", 1)
+            s3_bucket, s3_key = parse_s3_url(url=input_document)
         ext: str = ""
         _, ext = os.path.splitext(input_document)
         ext = ext.lower()
 
         is_pdf: bool = ext != None and ext.lower() in only_async_suffixes
         if is_pdf and not is_s3_document:
             raise ValueError("PDF only supported when located on S3")
```

