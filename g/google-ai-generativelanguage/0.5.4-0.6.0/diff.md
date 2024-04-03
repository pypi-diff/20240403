# Comparing `tmp/google-ai-generativelanguage-0.5.4.tar.gz` & `tmp/google-ai-generativelanguage-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ai-generativelanguage-0.5.4.tar", last modified: Tue Mar  5 18:48:59 2024, max compression
+gzip compressed data, was "google-ai-generativelanguage-0.6.0.tar", last modified: Fri Mar 22 12:18:24 2024, max compression
```

## Comparing `google-ai-generativelanguage-0.5.4.tar` & `google-ai-generativelanguage-0.6.0.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.559261 google-ai-generativelanguage-0.5.4/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5188 2024-03-05 18:48:59.559261 google-ai-generativelanguage-0.5.4/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3800 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.487232 google-ai-generativelanguage-0.5.4/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.491233 google-ai-generativelanguage-0.5.4/google/ai/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.495235 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage/
--rw-rw-r--   0 root         (0)     1003     8988 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.499237 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/
--rw-rw-r--   0 root         (0)     1003     2229 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     3669 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.499237 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.499237 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    45932 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    61250 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.499237 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10725 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19633 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    19938 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    46100 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.503238 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    27020 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    43332 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003     5747 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.503238 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7270 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15410 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15664 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    26746 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.503238 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/
--rw-rw-r--   0 root         (0)     1003     1759 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2895 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/citation.py
--rw-rw-r--   0 root         (0)     1003     3720 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/content.py
--rw-rw-r--   0 root         (0)     1003    20134 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/generative_service.py
--rw-rw-r--   0 root         (0)     1003     4665 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/model.py
--rw-rw-r--   0 root         (0)     1003     3143 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     6161 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/safety.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.503238 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/
--rw-rw-r--   0 root         (0)     1003     7693 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003    19350 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.507240 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.507240 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24748 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40660 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.507240 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7451 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13414 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13641 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18401 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.507240 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    46928 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62242 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.511242 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10886 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18398 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18725 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    40935 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.511242 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    47264 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62596 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003    10950 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.511242 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    11616 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19686 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20146 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41543 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.511242 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    41727 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    57530 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/client.py
--rw-rw-r--   0 root         (0)     1003     6013 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.515243 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    10464 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18156 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18520 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41155 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.515243 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/
--rw-rw-r--   0 root         (0)     1003      777 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    97421 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   112654 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/client.py
--rw-rw-r--   0 root         (0)     1003    16011 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.515243 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/
--rw-rw-r--   0 root         (0)     1003     1428 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20205 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    33226 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    33948 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   105077 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.519245 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    35868 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51394 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.519245 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9013 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15599 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15899 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    28406 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.523246 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     6553 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2903 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/citation.py
--rw-rw-r--   0 root         (0)     1003    14001 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/content.py
--rw-rw-r--   0 root         (0)     1003    11601 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003    36351 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/generative_service.py
--rw-rw-r--   0 root         (0)     1003     4669 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/model.py
--rw-rw-r--   0 root         (0)     1003     9676 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     4530 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/permission.py
--rw-rw-r--   0 root         (0)     1003     6362 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/permission_service.py
--rw-rw-r--   0 root         (0)     1003    13703 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/retriever.py
--rw-rw-r--   0 root         (0)     1003    24469 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/retriever_service.py
--rw-rw-r--   0 root         (0)     1003     8594 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/safety.py
--rw-rw-r--   0 root         (0)     1003    14378 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/text_service.py
--rw-rw-r--   0 root         (0)     1003    12826 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/tuned_model.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.523246 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/
--rw-rw-r--   0 root         (0)     1003     2426 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003     3627 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.523246 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.527248 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24701 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40613 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.527248 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7391 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13355 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13582 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18341 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.527248 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    21080 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    36905 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003     5792 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.527248 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7203 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    12847 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13101 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    16216 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.531250 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    25037 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40877 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.531250 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7273 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13103 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13341 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    17420 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.531250 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/
--rw-rw-r--   0 root         (0)     1003     1847 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2905 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/citation.py
--rw-rw-r--   0 root         (0)     1003    11613 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     4670 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/model.py
--rw-rw-r--   0 root         (0)     1003     3158 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     7878 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/safety.py
--rw-rw-r--   0 root         (0)     1003    10981 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.535251 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/
--rw-rw-r--   0 root         (0)     1003     4188 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003     8993 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       89 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.535251 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.535251 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/
--rw-rw-r--   0 root         (0)     1003      769 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    24142 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    40676 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.535251 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/
--rw-rw-r--   0 root         (0)     1003     1400 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6769 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13417 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13644 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    18404 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.539253 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/
--rw-rw-r--   0 root         (0)     1003      761 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    45130 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    62639 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/client.py
--rw-rw-r--   0 root         (0)     1003    10967 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.539253 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     9226 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    19696 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    20156 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    41554 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.539253 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/
--rw-rw-r--   0 root         (0)     1003      781 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    40149 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    57825 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/client.py
--rw-rw-r--   0 root         (0)     1003     6022 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.543254 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/
--rw-rw-r--   0 root         (0)     1003     1442 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8758 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    18165 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    18529 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    40318 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.543254 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/
--rw-rw-r--   0 root         (0)     1003      757 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    34750 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    51520 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.543254 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/
--rw-rw-r--   0 root         (0)     1003     1358 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7647 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15604 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    15904 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003    28412 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.547256 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/
--rw-rw-r--   0 root         (0)     1003     3416 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     2905 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/citation.py
--rw-rw-r--   0 root         (0)     1003    11613 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/discuss_service.py
--rw-rw-r--   0 root         (0)     1003     4670 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/model.py
--rw-rw-r--   0 root         (0)     1003     8924 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/model_service.py
--rw-rw-r--   0 root         (0)     1003     4460 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/permission.py
--rw-rw-r--   0 root         (0)     1003     6197 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/permission_service.py
--rw-rw-r--   0 root         (0)     1003     7974 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/safety.py
--rw-rw-r--   0 root         (0)     1003    13777 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/text_service.py
--rw-rw-r--   0 root         (0)     1003    12841 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/tuned_model.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.547256 google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/
--rw-r--r--   0 root         (0)     1003     5188 2024-03-05 18:48:59.000000 google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003    14880 2024-03-05 18:48:59.000000 google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:48:59.000000 google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-05 18:48:59.000000 google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      305 2024-03-05 18:48:59.000000 google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-05 18:48:59.000000 google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-05 18:48:59.559261 google-ai-generativelanguage-0.5.4/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3201 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.547256 google-ai-generativelanguage-0.5.4/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.547256 google-ai-generativelanguage-0.5.4/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.551258 google-ai-generativelanguage-0.5.4/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.551258 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   189722 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1/test_generative_service.py
--rw-rw-r--   0 root         (0)     1003   131822 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1/test_model_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.555259 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   109193 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   189343 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py
--rw-rw-r--   0 root         (0)     1003   218874 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   196027 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py
--rw-rw-r--   0 root         (0)     1003   442055 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py
--rw-rw-r--   0 root         (0)     1003   143187 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.555259 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/__init__.py
--rw-rw-r--   0 root         (0)     1003   109139 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   109768 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   106284 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-05 18:48:59.555259 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/__init__.py
--rw-rw-r--   0 root         (0)     1003   109201 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py
--rw-rw-r--   0 root         (0)     1003   218889 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py
--rw-rw-r--   0 root         (0)     1003   196597 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py
--rw-rw-r--   0 root         (0)     1003   143734 2024-03-05 18:46:00.000000 google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.899938 google-ai-generativelanguage-0.6.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5188 2024-03-22 12:18:24.899938 google-ai-generativelanguage-0.6.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3800 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.827933 google-ai-generativelanguage-0.6.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.835933 google-ai-generativelanguage-0.6.0/google/ai/
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.839934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage/
+-rw-rw-r--   0 root         (0)     1003     8988 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.839934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/
+-rw-rw-r--   0 root         (0)     1003     2229 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3669 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.839934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.839934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    45932 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    61250 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.843934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10725 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19633 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    19938 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    46100 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.843934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    27020 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    43332 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5747 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.843934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7270 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15410 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15664 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    26746 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.847934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/
+-rw-rw-r--   0 root         (0)     1003     1759 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2895 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/citation.py
+-rw-rw-r--   0 root         (0)     1003     3720 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/content.py
+-rw-rw-r--   0 root         (0)     1003    20134 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/generative_service.py
+-rw-rw-r--   0 root         (0)     1003     4665 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/model.py
+-rw-rw-r--   0 root         (0)     1003     3143 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     6161 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/safety.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.847934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/
+-rw-rw-r--   0 root         (0)     1003     7693 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003    19350 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.847934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.847934 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24748 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40660 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.851935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7451 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13414 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13641 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18401 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.851935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47141 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62455 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.851935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10886 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18398 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18725 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41119 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.851935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    47264 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62596 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10950 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.855935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    11616 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19686 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20146 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41543 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.855935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    41727 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    57530 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6013 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.855935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10464 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18156 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18520 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41155 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.859935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/
+-rw-rw-r--   0 root         (0)     1003      777 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    97421 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   112654 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/client.py
+-rw-rw-r--   0 root         (0)     1003    16011 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.859935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1428 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20205 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    33226 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    33948 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   105077 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.859935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    35868 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51394 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.863935 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9013 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15599 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15899 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    28406 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.867936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     6553 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2903 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    14001 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/content.py
+-rw-rw-r--   0 root         (0)     1003    11601 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003    36393 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/generative_service.py
+-rw-rw-r--   0 root         (0)     1003     4669 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/model.py
+-rw-rw-r--   0 root         (0)     1003     9676 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     4530 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/permission.py
+-rw-rw-r--   0 root         (0)     1003     6362 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/permission_service.py
+-rw-rw-r--   0 root         (0)     1003    13703 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/retriever.py
+-rw-rw-r--   0 root         (0)     1003    24469 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/retriever_service.py
+-rw-rw-r--   0 root         (0)     1003     8594 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    14378 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/text_service.py
+-rw-rw-r--   0 root         (0)     1003    13772 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/tuned_model.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.867936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003     2426 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003     3627 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.867936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.867936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24701 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40613 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.867936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7391 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13355 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13582 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18341 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.871936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21080 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    36905 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5792 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.871936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7203 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    12847 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13101 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    16216 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.871936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    25037 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40877 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.875936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7273 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13103 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13341 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    17420 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.875936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/
+-rw-rw-r--   0 root         (0)     1003     1847 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2905 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    11613 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     4670 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/model.py
+-rw-rw-r--   0 root         (0)     1003     3158 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     7878 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    10981 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.875936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/
+-rw-rw-r--   0 root         (0)     1003     4188 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8993 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       89 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.875936 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.879937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/
+-rw-rw-r--   0 root         (0)     1003      769 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    24142 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    40676 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.879937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1400 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6769 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13417 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13644 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    18404 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.879937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/
+-rw-rw-r--   0 root         (0)     1003      761 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    45130 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    62639 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/client.py
+-rw-rw-r--   0 root         (0)     1003    10967 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.879937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9226 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    19696 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    20156 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    41554 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.883937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/
+-rw-rw-r--   0 root         (0)     1003      781 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    40149 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    57825 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/client.py
+-rw-rw-r--   0 root         (0)     1003     6022 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.883937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1442 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8758 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    18165 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    18529 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    40318 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.883937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/
+-rw-rw-r--   0 root         (0)     1003      757 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    34750 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    51520 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.887937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1358 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7647 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15604 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    15904 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003    28412 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.887937 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/
+-rw-rw-r--   0 root         (0)     1003     3416 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     2905 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/citation.py
+-rw-rw-r--   0 root         (0)     1003    11613 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/discuss_service.py
+-rw-rw-r--   0 root         (0)     1003     4670 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/model.py
+-rw-rw-r--   0 root         (0)     1003     8924 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/model_service.py
+-rw-rw-r--   0 root         (0)     1003     4460 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/permission.py
+-rw-rw-r--   0 root         (0)     1003     6197 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/permission_service.py
+-rw-rw-r--   0 root         (0)     1003     7974 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/safety.py
+-rw-rw-r--   0 root         (0)     1003    13777 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/text_service.py
+-rw-rw-r--   0 root         (0)     1003    12841 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/tuned_model.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.891938 google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/
+-rw-r--r--   0 root         (0)     1003     5188 2024-03-22 12:18:24.000000 google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003    14880 2024-03-22 12:18:24.000000 google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-03-22 12:18:24.000000 google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-03-22 12:18:24.000000 google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      305 2024-03-22 12:18:24.000000 google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-03-22 12:18:24.000000 google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-03-22 12:18:24.899938 google-ai-generativelanguage-0.6.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3201 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.891938 google-ai-generativelanguage-0.6.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.891938 google-ai-generativelanguage-0.6.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.891938 google-ai-generativelanguage-0.6.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.891938 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   189722 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1/test_generative_service.py
+-rw-rw-r--   0 root         (0)     1003   131822 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1/test_model_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.895938 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   109193 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   189343 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py
+-rw-rw-r--   0 root         (0)     1003   218978 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   196027 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py
+-rw-rw-r--   0 root         (0)     1003   442055 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py
+-rw-rw-r--   0 root         (0)     1003   143187 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.895938 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/__init__.py
+-rw-rw-r--   0 root         (0)     1003   109139 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   109768 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   106284 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:18:24.899938 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/
+-rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/__init__.py
+-rw-rw-r--   0 root         (0)     1003   109201 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py
+-rw-rw-r--   0 root         (0)     1003   218889 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py
+-rw-rw-r--   0 root         (0)     1003   196597 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py
+-rw-rw-r--   0 root         (0)     1003   143734 2024-03-22 12:15:14.000000 google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py
```

### Comparing `google-ai-generativelanguage-0.5.4/LICENSE` & `google-ai-generativelanguage-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.5.4/MANIFEST.in` & `google-ai-generativelanguage-0.6.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.5.4/PKG-INFO` & `google-ai-generativelanguage-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-generativelanguage
-Version: 0.5.4
+Version: 0.6.0
 Summary: Google Ai Generativelanguage API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ai-generativelanguage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-ai-generativelanguage-0.5.4/README.rst` & `google-ai-generativelanguage-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage/gapic_version.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.4"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/gapic_metadata.json` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/gapic_version.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.4"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/generative_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/services/model_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/citation.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/citation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/content.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/generative_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/generative_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/model.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/model_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/model_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1/types/safety.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1/types/safety.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/gapic_metadata.json` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/gapic_version.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.4"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/discuss_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -483,15 +483,19 @@
                 be more than one setting for each ``SafetyCategory``
                 type. The API will block any contents and responses that
                 fail to meet the thresholds set by these settings. This
                 list overrides the default settings for each
                 ``SafetyCategory`` specified in the safety_settings. If
                 there is no ``SafetySetting`` for a given
                 ``SafetyCategory`` provided in the list, the API will
-                use the default safety setting for that category.
+                use the default safety setting for that category. Harm
+                categories HARM_CATEGORY_HATE_SPEECH,
+                HARM_CATEGORY_SEXUALLY_EXPLICIT,
+                HARM_CATEGORY_DANGEROUS_CONTENT,
+                HARM_CATEGORY_HARASSMENT are supported.
 
                 This corresponds to the ``safety_settings`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             answer_style (:class:`google.ai.generativelanguage_v1beta.types.GenerateAnswerRequest.AnswerStyle`):
                 Required. Style in which answers
                 should be returned.
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -879,15 +879,19 @@
                 be more than one setting for each ``SafetyCategory``
                 type. The API will block any contents and responses that
                 fail to meet the thresholds set by these settings. This
                 list overrides the default settings for each
                 ``SafetyCategory`` specified in the safety_settings. If
                 there is no ``SafetySetting`` for a given
                 ``SafetyCategory`` provided in the list, the API will
-                use the default safety setting for that category.
+                use the default safety setting for that category. Harm
+                categories HARM_CATEGORY_HATE_SPEECH,
+                HARM_CATEGORY_SEXUALLY_EXPLICIT,
+                HARM_CATEGORY_DANGEROUS_CONTENT,
+                HARM_CATEGORY_HARASSMENT are supported.
 
                 This corresponds to the ``safety_settings`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             answer_style (google.ai.generativelanguage_v1beta.types.GenerateAnswerRequest.AnswerStyle):
                 Required. Style in which answers
                 should be returned.
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/generative_service/transports/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -794,14 +794,19 @@
 
             http_options: List[Dict[str, str]] = [
                 {
                     "method": "post",
                     "uri": "/v1beta/{model=models/*}:generateContent",
                     "body": "*",
                 },
+                {
+                    "method": "post",
+                    "uri": "/v1beta/{model=tunedModels/*}:generateContent",
+                    "body": "*",
+                },
             ]
             request, metadata = self._interceptor.pre_generate_content(
                 request, metadata
             )
             pb_request = generative_service.GenerateContentRequest.pb(request)
             transcoded_request = path_template.transcode(http_options, pb_request)
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/model_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/permission_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/retriever_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/services/text_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/citation.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/citation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/content.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/discuss_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/discuss_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/generative_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/generative_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -177,28 +177,27 @@
             specified, the API will stop at the first
             appearance of a stop sequence. The stop sequence
             will not be included as part of the response.
         max_output_tokens (int):
             Optional. The maximum number of tokens to include in a
             candidate.
 
-            If unset, this will default to output_token_limit specified
-            in the ``Model`` specification.
+            Note: The default value varies by model, see the
+            ``Model.output_token_limit`` attribute of the ``Model``
+            returned from the ``getModel`` function.
 
             This field is a member of `oneof`_ ``_max_output_tokens``.
         temperature (float):
-            Optional. Controls the randomness of the output. Note: The
-            default value varies by model, see the ``Model.temperature``
-            attribute of the ``Model`` returned the ``getModel``
-            function.
+            Optional. Controls the randomness of the output.
 
-            Values can range from [0.0,1.0], inclusive. A value closer
-            to 1.0 will produce responses that are more varied and
-            creative, while a value closer to 0.0 will typically result
-            in more straightforward responses from the model.
+            Note: The default value varies by model, see the
+            ``Model.temperature`` attribute of the ``Model`` returned
+            from the ``getModel`` function.
+
+            Values can range from [0.0, infinity).
 
             This field is a member of `oneof`_ ``_temperature``.
         top_p (float):
             Optional. The maximum cumulative probability of tokens to
             consider when sampling.
 
             The model uses combined Top-k and nucleus sampling.
@@ -206,29 +205,29 @@
             Tokens are sorted based on their assigned probabilities so
             that only the most likely tokens are considered. Top-k
             sampling directly limits the maximum number of tokens to
             consider, while Nucleus sampling limits number of tokens
             based on the cumulative probability.
 
             Note: The default value varies by model, see the
-            ``Model.top_p`` attribute of the ``Model`` returned the
+            ``Model.top_p`` attribute of the ``Model`` returned from the
             ``getModel`` function.
 
             This field is a member of `oneof`_ ``_top_p``.
         top_k (int):
             Optional. The maximum number of tokens to consider when
             sampling.
 
             The model uses combined Top-k and nucleus sampling.
 
             Top-k sampling considers the set of ``top_k`` most probable
-            tokens. Defaults to 40.
+            tokens.
 
             Note: The default value varies by model, see the
-            ``Model.top_k`` attribute of the ``Model`` returned the
+            ``Model.top_k`` attribute of the ``Model`` returned from the
             ``getModel`` function.
 
             This field is a member of `oneof`_ ``_top_k``.
     """
 
     candidate_count: int = proto.Field(
         proto.INT32,
@@ -651,15 +650,19 @@
             ``GenerateAnswerResponse.candidate``. There should not be
             more than one setting for each ``SafetyCategory`` type. The
             API will block any contents and responses that fail to meet
             the thresholds set by these settings. This list overrides
             the default settings for each ``SafetyCategory`` specified
             in the safety_settings. If there is no ``SafetySetting`` for
             a given ``SafetyCategory`` provided in the list, the API
-            will use the default safety setting for that category.
+            will use the default safety setting for that category. Harm
+            categories HARM_CATEGORY_HATE_SPEECH,
+            HARM_CATEGORY_SEXUALLY_EXPLICIT,
+            HARM_CATEGORY_DANGEROUS_CONTENT, HARM_CATEGORY_HARASSMENT
+            are supported.
         temperature (float):
             Optional. Controls the randomness of the output.
 
             Values can range from [0.0,1.0], inclusive. A value closer
             to 1.0 will produce responses that are more varied and
             creative, while a value closer to 0.0 will typically result
             in more straightforward responses from the model. A low
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/model.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1beta",
+    package="google.ai.generativelanguage.v1beta2",
     manifest={
         "Model",
     },
 )
 
 
 class Model(proto.Message):
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/model_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/model_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/permission.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/permission_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/permission_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/retriever.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/retriever.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/retriever_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/retriever_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/safety.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/safety.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -40,20 +40,20 @@
     Values:
         HARM_CATEGORY_UNSPECIFIED (0):
             Category is unspecified.
         HARM_CATEGORY_DEROGATORY (1):
             Negative or harmful comments targeting
             identity and/or protected attribute.
         HARM_CATEGORY_TOXICITY (2):
-            Content that is rude, disrepspectful, or
+            Content that is rude, disrespectful, or
             profane.
         HARM_CATEGORY_VIOLENCE (3):
-            Describes scenarios depictng violence against
-            an individual or group, or general descriptions
-            of gore.
+            Describes scenarios depicting violence
+            against an individual or group, or general
+            descriptions of gore.
         HARM_CATEGORY_SEXUAL (4):
             Contains references to sexual acts or other
             lewd content.
         HARM_CATEGORY_MEDICAL (5):
             Promotes unchecked medical advice.
         HARM_CATEGORY_DANGEROUS (6):
             Dangerous content that promotes, facilitates,
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/text_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/text_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta/types/tuned_model.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/tuned_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,15 +17,15 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1beta",
+    package="google.ai.generativelanguage.v1beta3",
     manifest={
         "TunedModel",
         "TunedModelSource",
         "TuningTask",
         "Hyperparameters",
         "Dataset",
         "TuningExamples",
@@ -43,15 +43,15 @@
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        tuned_model_source (google.ai.generativelanguage_v1beta.types.TunedModelSource):
+        tuned_model_source (google.ai.generativelanguage_v1beta3.types.TunedModelSource):
             Optional. TunedModel to use as the starting
             point for training the new model.
 
             This field is a member of `oneof`_ ``source_model``.
         base_model (str):
             Immutable. The name of the ``Model`` to tune. Example:
             ``models/text-bison-001``
@@ -100,23 +100,23 @@
             tokens. This value specifies default to be used by the
             backend while making the call to the model.
 
             This value specifies default to be the one used by the base
             model while creating the model.
 
             This field is a member of `oneof`_ ``_top_k``.
-        state (google.ai.generativelanguage_v1beta.types.TunedModel.State):
+        state (google.ai.generativelanguage_v1beta3.types.TunedModel.State):
             Output only. The state of the tuned model.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when this model
             was created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when this model
             was updated.
-        tuning_task (google.ai.generativelanguage_v1beta.types.TuningTask):
+        tuning_task (google.ai.generativelanguage_v1beta3.types.TuningTask):
             Required. The tuning task that creates the
             tuned model.
     """
 
     class State(proto.Enum):
         r"""The state of the tuned model.
 
@@ -225,20 +225,20 @@
     Attributes:
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when tuning this
             model started.
         complete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when tuning this
             model completed.
-        snapshots (MutableSequence[google.ai.generativelanguage_v1beta.types.TuningSnapshot]):
+        snapshots (MutableSequence[google.ai.generativelanguage_v1beta3.types.TuningSnapshot]):
             Output only. Metrics collected during tuning.
-        training_data (google.ai.generativelanguage_v1beta.types.Dataset):
+        training_data (google.ai.generativelanguage_v1beta3.types.Dataset):
             Required. Input only. Immutable. The model
             training data.
-        hyperparameters (google.ai.generativelanguage_v1beta.types.Hyperparameters):
+        hyperparameters (google.ai.generativelanguage_v1beta3.types.Hyperparameters):
             Immutable. Hyperparameters controlling the
             tuning process. If not provided, default values
             will be used.
     """
 
     start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
@@ -314,33 +314,34 @@
 
 class Dataset(proto.Message):
     r"""Dataset for training or validation.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        examples (google.ai.generativelanguage_v1beta.types.TuningExamples):
+        examples (google.ai.generativelanguage_v1beta3.types.TuningExamples):
             Optional. Inline examples.
 
             This field is a member of `oneof`_ ``dataset``.
     """
 
     examples: "TuningExamples" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="dataset",
         message="TuningExamples",
     )
 
 
 class TuningExamples(proto.Message):
-    r"""A set of tuning examples. Can be training or validation data.
+    r"""A set of tuning examples. Can be training or validatation
+    data.
 
     Attributes:
-        examples (MutableSequence[google.ai.generativelanguage_v1beta.types.TuningExample]):
+        examples (MutableSequence[google.ai.generativelanguage_v1beta3.types.TuningExample]):
             Required. The examples. Example input can be
             for text or discuss, but all examples in a set
             must be of the same type.
     """
 
     examples: MutableSequence["TuningExample"] = proto.RepeatedField(
         proto.MESSAGE,
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/gapic_metadata.json` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/gapic_version.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.4"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/discuss_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/model_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/services/text_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/citation.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/citation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/discuss_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/discuss_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/model.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1beta2",
+    package="google.ai.generativelanguage.v1beta3",
     manifest={
         "Model",
     },
 )
 
 
 class Model(proto.Message):
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/model_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/model_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/safety.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/safety.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta2/types/text_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta2/types/text_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/gapic_metadata.json` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/gapic_version.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.5.4"  # {x-release-please-version}
+__version__ = "0.6.0"  # {x-release-please-version}
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/discuss_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/pagers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/model_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/pagers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/grpc_asyncio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/permission_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/client.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/services/text_service/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/__init__.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/citation.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/citation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/discuss_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/discuss_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/model.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 from __future__ import annotations
 
 from typing import MutableMapping, MutableSequence
 
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1beta3",
+    package="google.ai.generativelanguage.v1beta",
     manifest={
         "Model",
     },
 )
 
 
 class Model(proto.Message):
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/model_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/model_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/permission.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/permission.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/permission_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/permission_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/safety.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/safety.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/text_service.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta3/types/text_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/google/ai/generativelanguage_v1beta3/types/tuned_model.py` & `google-ai-generativelanguage-0.6.0/google/ai/generativelanguage_v1beta/types/tuned_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,15 +17,15 @@
 
 from typing import MutableMapping, MutableSequence
 
 from google.protobuf import timestamp_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.ai.generativelanguage.v1beta3",
+    package="google.ai.generativelanguage.v1beta",
     manifest={
         "TunedModel",
         "TunedModelSource",
         "TuningTask",
         "Hyperparameters",
         "Dataset",
         "TuningExamples",
@@ -43,15 +43,15 @@
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        tuned_model_source (google.ai.generativelanguage_v1beta3.types.TunedModelSource):
+        tuned_model_source (google.ai.generativelanguage_v1beta.types.TunedModelSource):
             Optional. TunedModel to use as the starting
             point for training the new model.
 
             This field is a member of `oneof`_ ``source_model``.
         base_model (str):
             Immutable. The name of the ``Model`` to tune. Example:
             ``models/text-bison-001``
@@ -100,23 +100,23 @@
             tokens. This value specifies default to be used by the
             backend while making the call to the model.
 
             This value specifies default to be the one used by the base
             model while creating the model.
 
             This field is a member of `oneof`_ ``_top_k``.
-        state (google.ai.generativelanguage_v1beta3.types.TunedModel.State):
+        state (google.ai.generativelanguage_v1beta.types.TunedModel.State):
             Output only. The state of the tuned model.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when this model
             was created.
         update_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when this model
             was updated.
-        tuning_task (google.ai.generativelanguage_v1beta3.types.TuningTask):
+        tuning_task (google.ai.generativelanguage_v1beta.types.TuningTask):
             Required. The tuning task that creates the
             tuned model.
     """
 
     class State(proto.Enum):
         r"""The state of the tuned model.
 
@@ -225,20 +225,20 @@
     Attributes:
         start_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when tuning this
             model started.
         complete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when tuning this
             model completed.
-        snapshots (MutableSequence[google.ai.generativelanguage_v1beta3.types.TuningSnapshot]):
+        snapshots (MutableSequence[google.ai.generativelanguage_v1beta.types.TuningSnapshot]):
             Output only. Metrics collected during tuning.
-        training_data (google.ai.generativelanguage_v1beta3.types.Dataset):
+        training_data (google.ai.generativelanguage_v1beta.types.Dataset):
             Required. Input only. Immutable. The model
             training data.
-        hyperparameters (google.ai.generativelanguage_v1beta3.types.Hyperparameters):
+        hyperparameters (google.ai.generativelanguage_v1beta.types.Hyperparameters):
             Immutable. Hyperparameters controlling the
             tuning process. If not provided, default values
             will be used.
     """
 
     start_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
@@ -264,84 +264,102 @@
         proto.MESSAGE,
         number=5,
         message="Hyperparameters",
     )
 
 
 class Hyperparameters(proto.Message):
-    r"""Hyperparameters controlling the tuning process.
+    r"""Hyperparameters controlling the tuning process. Read more at
+    https://ai.google.dev/docs/model_tuning_guidance
+
+    This message has `oneof`_ fields (mutually exclusive fields).
+    For each oneof, at most one member field can be set at the same time.
+    Setting any member of the oneof automatically clears all other
+    members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
+        learning_rate (float):
+            Optional. Immutable. The learning rate
+            hyperparameter for tuning. If not set, a default
+            of 0.001 or 0.0002 will be calculated based on
+            the number of training examples.
+
+            This field is a member of `oneof`_ ``learning_rate_option``.
+        learning_rate_multiplier (float):
+            Optional. Immutable. The learning rate multiplier is used to
+            calculate a final learning_rate based on the default
+            (recommended) value. Actual learning rate :=
+            learning_rate_multiplier \* default learning rate Default
+            learning rate is dependent on base model and dataset size.
+            If not set, a default of 1.0 will be used.
+
+            This field is a member of `oneof`_ ``learning_rate_option``.
         epoch_count (int):
             Immutable. The number of training epochs. An
             epoch is one pass through the training data. If
-            not set, a default of 10 will be used.
+            not set, a default of 5 will be used.
 
             This field is a member of `oneof`_ ``_epoch_count``.
         batch_size (int):
             Immutable. The batch size hyperparameter for
-            tuning. If not set, a default of 16 or 64 will
-            be used based on the number of training
-            examples.
+            tuning. If not set, a default of 4 or 16 will be
+            used based on the number of training examples.
 
             This field is a member of `oneof`_ ``_batch_size``.
-        learning_rate (float):
-            Immutable. The learning rate hyperparameter
-            for tuning. If not set, a default of 0.0002 or
-            0.002 will be calculated based on the number of
-            training examples.
-
-            This field is a member of `oneof`_ ``_learning_rate``.
     """
 
+    learning_rate: float = proto.Field(
+        proto.FLOAT,
+        number=16,
+        oneof="learning_rate_option",
+    )
+    learning_rate_multiplier: float = proto.Field(
+        proto.FLOAT,
+        number=17,
+        oneof="learning_rate_option",
+    )
     epoch_count: int = proto.Field(
         proto.INT32,
         number=14,
         optional=True,
     )
     batch_size: int = proto.Field(
         proto.INT32,
         number=15,
         optional=True,
     )
-    learning_rate: float = proto.Field(
-        proto.FLOAT,
-        number=16,
-        optional=True,
-    )
 
 
 class Dataset(proto.Message):
     r"""Dataset for training or validation.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        examples (google.ai.generativelanguage_v1beta3.types.TuningExamples):
+        examples (google.ai.generativelanguage_v1beta.types.TuningExamples):
             Optional. Inline examples.
 
             This field is a member of `oneof`_ ``dataset``.
     """
 
     examples: "TuningExamples" = proto.Field(
         proto.MESSAGE,
         number=1,
         oneof="dataset",
         message="TuningExamples",
     )
 
 
 class TuningExamples(proto.Message):
-    r"""A set of tuning examples. Can be training or validatation
-    data.
+    r"""A set of tuning examples. Can be training or validation data.
 
     Attributes:
-        examples (MutableSequence[google.ai.generativelanguage_v1beta3.types.TuningExample]):
+        examples (MutableSequence[google.ai.generativelanguage_v1beta.types.TuningExample]):
             Required. The examples. Example input can be
             for text or discuss, but all examples in a set
             must be of the same type.
     """
 
     examples: MutableSequence["TuningExample"] = proto.RepeatedField(
         proto.MESSAGE,
```

### Comparing `google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/PKG-INFO` & `google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-ai-generativelanguage
-Version: 0.5.4
+Version: 0.6.0
 Summary: Google Ai Generativelanguage API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-ai-generativelanguage
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-ai-generativelanguage-0.5.4/google_ai_generativelanguage.egg-info/SOURCES.txt` & `google-ai-generativelanguage-0.6.0/google_ai_generativelanguage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-ai-generativelanguage-0.5.4/setup.py` & `google-ai-generativelanguage-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/__init__.py` & `google-ai-generativelanguage-0.6.0/tests/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/__init__.py` & `google-ai-generativelanguage-0.6.0/tests/unit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/__init__.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1/__init__.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1/test_generative_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1/test_generative_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1/test_model_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1/test_model_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/__init__.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_discuss_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_generative_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_model_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -4217,17 +4217,18 @@
                 "examples": {
                     "examples": [
                         {"text_input": "text_input_value", "output": "output_value"}
                     ]
                 }
             },
             "hyperparameters": {
+                "learning_rate": 0.1371,
+                "learning_rate_multiplier": 0.2561,
                 "epoch_count": 1175,
                 "batch_size": 1052,
-                "learning_rate": 0.1371,
             },
         },
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
@@ -4584,17 +4585,18 @@
                 "examples": {
                     "examples": [
                         {"text_input": "text_input_value", "output": "output_value"}
                     ]
                 }
             },
             "hyperparameters": {
+                "learning_rate": 0.1371,
+                "learning_rate_multiplier": 0.2561,
                 "epoch_count": 1175,
                 "batch_size": 1052,
-                "learning_rate": 0.1371,
             },
         },
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_permission_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_retriever_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta/test_text_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/__init__.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/test_discuss_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/test_model_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta2/test_text_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/__init__.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/test_discuss_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/test_model_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/test_permission_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `google-ai-generativelanguage-0.5.4/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py` & `google-ai-generativelanguage-0.6.0/tests/unit/gapic/generativelanguage_v1beta3/test_text_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-# Copyright 2023 Google LLC
+# Copyright 2024 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

