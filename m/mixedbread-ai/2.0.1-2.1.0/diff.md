# Comparing `tmp/mixedbread_ai-2.0.1.tar.gz` & `tmp/mixedbread_ai-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixedbread_ai-2.0.1.tar", max compression
+gzip compressed data, was "mixedbread_ai-2.1.0.tar", max compression
```

## Comparing `mixedbread_ai-2.0.1.tar` & `mixedbread_ai-2.1.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    11348 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/LICENSE.md
--rw-r--r--   0        0        0     3841 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/README.md
--rw-r--r--   0        0        0     1981 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/__init__.py
--rw-r--r--   0        0        0    24344 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/client.py
--rw-r--r--   0        0        0      790 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/api_error.py
--rw-r--r--   0        0        0     1081 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/file.py
--rw-r--r--   0        0        0     4882 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/core/request_options.py
--rw-r--r--   0        0        0      163 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/environment.py
--rw-r--r--   0        0        0      620 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/errors/__init__.py
--rw-r--r--   0        0        0      305 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/errors/bad_request_error.py
--rw-r--r--   0        0        0      300 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/errors/forbidden_error.py
--rw-r--r--   0        0        0      289 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/errors/internal_server_error.py
--rw-r--r--   0        0        0      297 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/errors/not_found_error.py
--rw-r--r--   0        0        0      326 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      312 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/errors/unauthorized_error.py
--rw-r--r--   0        0        0      300 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     2337 2024-04-02 19:55:21.845388 mixedbread_ai-2.0.1/mixedbread_ai/types/__init__.py
--rw-r--r--   0        0        0     1163 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/bad_request_error_body.py
--rw-r--r--   0        0        0      268 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/data.py
--rw-r--r--   0        0        0     1202 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/embedding.py
--rw-r--r--   0        0        0      152 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/embedding_item.py
--rw-r--r--   0        0        0      217 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/embeddings_request_encoding_format.py
--rw-r--r--   0        0        0     1612 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/embeddings_response.py
--rw-r--r--   0        0        0      218 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/embeddings_response_encoding_format.py
--rw-r--r--   0        0        0     1052 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/encoding_format.py
--rw-r--r--   0        0        0     1160 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/forbidden_error_body.py
--rw-r--r--   0        0        0      206 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/input.py
--rw-r--r--   0        0        0     1152 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/internal_error.py
--rw-r--r--   0        0        0     1194 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py
--rw-r--r--   0        0        0     1184 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/invalid_matryoshka_model_error.py
--rw-r--r--   0        0        0     1166 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/model_not_found_error.py
--rw-r--r--   0        0        0     1411 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/multiple_encodings_embedding.py
--rw-r--r--   0        0        0     1293 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/multiple_encodings_embedding_item.py
--rw-r--r--   0        0        0     1125 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/mxbai_web_error.py
--rw-r--r--   0        0        0      171 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/mxbai_web_error_details.py
--rw-r--r--   0        0        0     1159 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/not_found_error_body.py
--rw-r--r--   0        0        0      837 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/object_type.py
--rw-r--r--   0        0        0     1223 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/ranked_document.py
--rw-r--r--   0        0        0     1558 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/reranking_response.py
--rw-r--r--   0        0        0      970 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/text_document.py
--rw-r--r--   0        0        0     1174 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/too_many_requests_error_body.py
--rw-r--r--   0        0        0      689 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/truncation_strategy.py
--rw-r--r--   0        0        0     1166 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/unauthorized_error_body.py
--rw-r--r--   0        0        0     1133 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/usage.py
--rw-r--r--   0        0        0      141 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/validation_error.py
--rw-r--r--   0        0        0     1161 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/mixedbread_ai/types/web_truncation_error.py
--rw-r--r--   0        0        0      543 2024-04-02 19:55:21.849388 mixedbread_ai-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 mixedbread_ai-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11348 2024-04-03 13:00:22.152145 mixedbread_ai-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0     3841 2024-04-03 13:00:22.152145 mixedbread_ai-2.1.0/README.md
+-rw-r--r--   0        0        0     1981 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/__init__.py
+-rw-r--r--   0        0        0    24344 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/client.py
+-rw-r--r--   0        0        0      790 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/api_error.py
+-rw-r--r--   0        0        0     1081 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/file.py
+-rw-r--r--   0        0        0     4882 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/http_client.py
+-rw-r--r--   0        0        0     3799 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/core/request_options.py
+-rw-r--r--   0        0        0      163 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/environment.py
+-rw-r--r--   0        0        0      620 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/bad_request_error.py
+-rw-r--r--   0        0        0      300 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/forbidden_error.py
+-rw-r--r--   0        0        0      289 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/internal_server_error.py
+-rw-r--r--   0        0        0      297 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/not_found_error.py
+-rw-r--r--   0        0        0      326 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      312 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      300 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     2337 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/__init__.py
+-rw-r--r--   0        0        0     1163 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/bad_request_error_body.py
+-rw-r--r--   0        0        0      268 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/data.py
+-rw-r--r--   0        0        0     1202 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embedding.py
+-rw-r--r--   0        0        0      152 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embedding_item.py
+-rw-r--r--   0        0        0      217 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embeddings_request_encoding_format.py
+-rw-r--r--   0        0        0     1612 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embeddings_response.py
+-rw-r--r--   0        0        0      218 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/embeddings_response_encoding_format.py
+-rw-r--r--   0        0        0     1052 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/encoding_format.py
+-rw-r--r--   0        0        0     1160 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/forbidden_error_body.py
+-rw-r--r--   0        0        0      206 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/input.py
+-rw-r--r--   0        0        0     1152 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/internal_error.py
+-rw-r--r--   0        0        0     1194 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py
+-rw-r--r--   0        0        0     1184 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/invalid_matryoshka_model_error.py
+-rw-r--r--   0        0        0     1166 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/model_not_found_error.py
+-rw-r--r--   0        0        0     1411 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/multiple_encodings_embedding.py
+-rw-r--r--   0        0        0     1293 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/multiple_encodings_embedding_item.py
+-rw-r--r--   0        0        0     1125 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/mxbai_api_error.py
+-rw-r--r--   0        0        0      171 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/mxbai_api_error_details.py
+-rw-r--r--   0        0        0     1159 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/not_found_error_body.py
+-rw-r--r--   0        0        0      837 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/object_type.py
+-rw-r--r--   0        0        0     1223 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/ranked_document.py
+-rw-r--r--   0        0        0     1558 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/reranking_response.py
+-rw-r--r--   0        0        0      970 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/text_document.py
+-rw-r--r--   0        0        0     1174 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0      689 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/truncation_strategy.py
+-rw-r--r--   0        0        0     1166 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/unauthorized_error_body.py
+-rw-r--r--   0        0        0     1133 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/usage.py
+-rw-r--r--   0        0        0      141 2024-04-03 13:00:22.156145 mixedbread_ai-2.1.0/mixedbread_ai/types/validation_error.py
+-rw-r--r--   0        0        0     1161 2024-04-03 13:00:22.160145 mixedbread_ai-2.1.0/mixedbread_ai/types/web_truncation_error.py
+-rw-r--r--   0        0        0      544 2024-04-03 13:00:22.160145 mixedbread_ai-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 mixedbread_ai-2.1.0/PKG-INFO
```

### Comparing `mixedbread_ai-2.0.1/LICENSE.md` & `mixedbread_ai-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/README.md` & `mixedbread_ai-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/__init__.py` & `mixedbread_ai-2.1.0/mixedbread_ai/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     Input,
     InternalError,
     InvalidMatryoshkaDimensionsError,
     InvalidMatryoshkaModelError,
     ModelNotFoundError,
     MultipleEncodingsEmbedding,
     MultipleEncodingsEmbeddingItem,
-    MxbaiWebError,
-    MxbaiWebErrorDetails,
+    MxbaiApiError,
+    MxbaiApiErrorDetails,
     NotFoundErrorBody,
     ObjectType,
     RankedDocument,
     RerankingResponse,
     TextDocument,
     TooManyRequestsErrorBody,
     TruncationStrategy,
@@ -59,16 +59,16 @@
     "InternalServerError",
     "InvalidMatryoshkaDimensionsError",
     "InvalidMatryoshkaModelError",
     "MixedbreadAIEnvironment",
     "ModelNotFoundError",
     "MultipleEncodingsEmbedding",
     "MultipleEncodingsEmbeddingItem",
-    "MxbaiWebError",
-    "MxbaiWebErrorDetails",
+    "MxbaiApiError",
+    "MxbaiApiErrorDetails",
     "NotFoundError",
     "NotFoundErrorBody",
     "ObjectType",
     "RankedDocument",
     "RerankingResponse",
     "TextDocument",
     "TooManyRequestsError",
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/client.py` & `mixedbread_ai-2.1.0/mixedbread_ai/client.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/core/__init__.py` & `mixedbread_ai-2.1.0/mixedbread_ai/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/core/client_wrapper.py` & `mixedbread_ai-2.1.0/mixedbread_ai/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/core/datetime_utils.py` & `mixedbread_ai-2.1.0/mixedbread_ai/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/core/file.py` & `mixedbread_ai-2.1.0/mixedbread_ai/core/file.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/core/http_client.py` & `mixedbread_ai-2.1.0/mixedbread_ai/core/http_client.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/core/jsonable_encoder.py` & `mixedbread_ai-2.1.0/mixedbread_ai/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/core/request_options.py` & `mixedbread_ai-2.1.0/mixedbread_ai/core/request_options.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/errors/__init__.py` & `mixedbread_ai-2.1.0/mixedbread_ai/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/__init__.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from .input import Input
 from .internal_error import InternalError
 from .invalid_matryoshka_dimensions_error import InvalidMatryoshkaDimensionsError
 from .invalid_matryoshka_model_error import InvalidMatryoshkaModelError
 from .model_not_found_error import ModelNotFoundError
 from .multiple_encodings_embedding import MultipleEncodingsEmbedding
 from .multiple_encodings_embedding_item import MultipleEncodingsEmbeddingItem
-from .mxbai_web_error import MxbaiWebError
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error import MxbaiApiError
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 from .not_found_error_body import NotFoundErrorBody
 from .object_type import ObjectType
 from .ranked_document import RankedDocument
 from .reranking_response import RerankingResponse
 from .text_document import TextDocument
 from .too_many_requests_error_body import TooManyRequestsErrorBody
 from .truncation_strategy import TruncationStrategy
@@ -43,16 +43,16 @@
     "Input",
     "InternalError",
     "InvalidMatryoshkaDimensionsError",
     "InvalidMatryoshkaModelError",
     "ModelNotFoundError",
     "MultipleEncodingsEmbedding",
     "MultipleEncodingsEmbeddingItem",
-    "MxbaiWebError",
-    "MxbaiWebErrorDetails",
+    "MxbaiApiError",
+    "MxbaiApiErrorDetails",
     "NotFoundErrorBody",
     "ObjectType",
     "RankedDocument",
     "RerankingResponse",
     "TextDocument",
     "TooManyRequestsErrorBody",
     "TruncationStrategy",
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/bad_request_error_body.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/internal_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class BadRequestErrorBody(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["bad_request_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class InternalError(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["server_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/embedding.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/embedding.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/embeddings_response.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/embeddings_response.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/encoding_format.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/encoding_format.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/forbidden_error_body.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/not_found_error_body.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ForbiddenErrorBody(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["forbidden_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class NotFoundErrorBody(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["not_found_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/internal_error.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/invalid_matryoshka_model_error.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class InternalError(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["server_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class InvalidMatryoshkaModelError(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["invalid_matryoshka_model_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/model_not_found_error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class InvalidMatryoshkaDimensionsError(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["invalid_matryoshka_dimensions_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class ModelNotFoundError(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["model_not_found_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/invalid_matryoshka_model_error.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/invalid_matryoshka_dimensions_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class InvalidMatryoshkaModelError(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["invalid_matryoshka_model_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class InvalidMatryoshkaDimensionsError(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["invalid_matryoshka_dimensions_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/model_not_found_error.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/too_many_requests_error_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class ModelNotFoundError(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["model_not_found_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class TooManyRequestsErrorBody(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["too_many_requests_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/multiple_encodings_embedding.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/multiple_encodings_embedding.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/multiple_encodings_embedding_item.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/multiple_encodings_embedding_item.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/mxbai_web_error.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/web_truncation_error.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class MxbaiWebError(pydantic.BaseModel):
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class WebTruncationError(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["truncation_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
-    type: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/not_found_error_body.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/mxbai_api_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class NotFoundErrorBody(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["not_found_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class MxbaiApiError(pydantic.BaseModel):
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
+    type: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/object_type.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/object_type.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/ranked_document.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/ranked_document.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/reranking_response.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/reranking_response.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/text_document.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/text_document.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/too_many_requests_error_body.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/bad_request_error_body.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class TooManyRequestsErrorBody(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["too_many_requests_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class BadRequestErrorBody(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["bad_request_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/truncation_strategy.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/truncation_strategy.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/unauthorized_error_body.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/unauthorized_error_body.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class UnauthorizedErrorBody(pydantic.BaseModel):
     type: typing.Optional[typing.Literal["unauthorized_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/usage.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/usage.py`

 * *Files identical despite different names*

### Comparing `mixedbread_ai-2.0.1/mixedbread_ai/types/web_truncation_error.py` & `mixedbread_ai-2.1.0/mixedbread_ai/types/forbidden_error_body.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .mxbai_web_error_details import MxbaiWebErrorDetails
+from .mxbai_api_error_details import MxbaiApiErrorDetails
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class WebTruncationError(pydantic.BaseModel):
-    type: typing.Optional[typing.Literal["truncation_error"]] = None
-    details: typing.Optional[MxbaiWebErrorDetails] = None
+class ForbiddenErrorBody(pydantic.BaseModel):
+    type: typing.Optional[typing.Literal["forbidden_error"]] = None
+    details: typing.Optional[MxbaiApiErrorDetails] = None
     message: typing.Optional[str] = None
     url: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
```

### Comparing `mixedbread_ai-2.0.1/pyproject.toml` & `mixedbread_ai-2.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mixedbread-ai"
-version = "2.0.1"
+version = "2.1.0"
 description = "mixedbread ai (https://www.mixedbread.ai)"
 authors = ["mixedbread.ai <support@mixedbread.ai>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/mixedbread-ai/python-sdk.git"
 keywords = ["Embeddings", "NLP", "mixedbread.ai"]
 packages = [
@@ -13,8 +13,8 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 httpx = ">=0.21.2"
 pydantic = ">= 1.9.2"
 requests = "^2.31.0"
 types-requests = "^2.31.0.20240311"
-typing_extensions = ">= 4.0.0"
+typing_extensions = ">= 4.0.0"
```

### Comparing `mixedbread_ai-2.0.1/PKG-INFO` & `mixedbread_ai-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixedbread-ai
-Version: 2.0.1
+Version: 2.1.0
 Summary: mixedbread ai (https://www.mixedbread.ai)
 Home-page: https://github.com/mixedbread-ai/python-sdk.git
 License: Apache-2.0
 Keywords: Embeddings,NLP,mixedbread.ai
 Author: mixedbread.ai
 Author-email: support@mixedbread.ai
 Requires-Python: >=3.8,<4.0
```

