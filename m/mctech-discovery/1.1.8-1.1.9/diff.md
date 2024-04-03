# Comparing `tmp/mctech_discovery-1.1.8.tar.gz` & `tmp/mctech_discovery-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mctech_discovery-1.1.8.tar", last modified: Wed Dec  6 02:02:11 2023, max compression
+gzip compressed data, was "mctech_discovery-1.1.9.tar", last modified: Mon Dec 11 02:29:28 2023, max compression
```

## Comparing `mctech_discovery-1.1.8.tar` & `mctech_discovery-1.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.718689 mctech_discovery-1.1.8/
--rw-rw-rw-   0        0        0      151 2023-12-06 02:02:11.717707 mctech_discovery-1.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      497 2023-07-19 12:16:29.000000 mctech_discovery-1.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.614093 mctech_discovery-1.1.8/mctech_discovery/
--rw-rw-rw-   0        0        0       72 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.637093 mctech_discovery-1.1.8/mctech_discovery/config/
--rw-rw-rw-   0        0        0      977 2022-10-08 03:15:48.000000 mctech_discovery-1.1.8/mctech_discovery/config/__init__.py
--rw-rw-rw-   0        0        0     8300 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/config/_configure.py
--rw-rw-rw-   0        0        0     8384 2023-08-26 09:57:47.000000 mctech_discovery-1.1.8/mctech_discovery/config/config_merger.py
--rw-rw-rw-   0        0        0     1922 2022-10-08 03:15:48.000000 mctech_discovery-1.1.8/mctech_discovery/config/config_value.py
--rw-rw-rw-   0        0        0     1464 2023-05-12 06:58:39.000000 mctech_discovery-1.1.8/mctech_discovery/config/yaml_loader.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.647093 mctech_discovery-1.1.8/mctech_discovery/discovery/
--rw-rw-rw-   0        0        0     1420 2022-10-08 03:15:48.000000 mctech_discovery-1.1.8/mctech_discovery/discovery/__init__.py
--rw-rw-rw-   0        0        0     8996 2023-12-05 09:34:59.000000 mctech_discovery-1.1.8/mctech_discovery/discovery/eureka_discovery_client.py
--rw-rw-rw-   0        0        0      830 2022-10-08 03:15:48.000000 mctech_discovery-1.1.8/mctech_discovery/discovery/local_discovery_client.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.651095 mctech_discovery-1.1.8/mctech_discovery/lifecycle/
--rw-rw-rw-   0        0        0        0 2023-05-12 06:58:39.000000 mctech_discovery-1.1.8/mctech_discovery/lifecycle/__init__.py
--rw-rw-rw-   0        0        0     1167 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/lifecycle/lifecycle.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.659095 mctech_discovery-1.1.8/mctech_discovery/rpc/
--rw-rw-rw-   0        0        0       68 2023-12-05 09:44:25.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.671157 mctech_discovery-1.1.8/mctech_discovery/rpc/ep/
--rw-rw-rw-   0        0        0        0 2020-06-01 03:25:27.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/ep/__init__.py
--rw-rw-rw-   0        0        0      640 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/ep/ep_request.py
--rw-rw-rw-   0        0        0     4158 2023-12-06 02:00:38.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/ep/internal_rpc.py
--rw-rw-rw-   0        0        0      719 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/ep/simple_ep_request.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.688693 mctech_discovery-1.1.8/mctech_discovery/rpc/lb/
--rw-rw-rw-   0        0        0     3253 2023-11-02 11:17:36.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/lb/__init__.py
--rw-rw-rw-   0        0        0     1555 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/lb/direct_loadbalancer.py
--rw-rw-rw-   0        0        0     1903 2023-12-05 09:50:47.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/lb/discovery_service_loadbalancer.py
--rw-rw-rw-   0        0        0     1299 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/lb/loadbalancer.py
--rw-rw-rw-   0        0        0     1180 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/lb/local_service_loadabalancer.py
--rw-rw-rw-   0        0        0     1070 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/lb/retry_loadbalancer.py
--rw-rw-rw-   0        0        0     8120 2023-12-06 01:53:20.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/request_context.py
--rw-rw-rw-   0        0        0     4777 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/rpc_client.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.698692 mctech_discovery-1.1.8/mctech_discovery/rpc/rule/
--rw-rw-rw-   0        0        0        0 2023-05-12 06:58:39.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/rule/__init__.py
--rw-rw-rw-   0        0        0     1041 2023-12-05 09:49:38.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/rule/abstarct_rule.py
--rw-rw-rw-   0        0        0      477 2023-05-12 06:58:39.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/rule/simple_rule.py
--rw-rw-rw-   0        0        0      785 2023-09-20 02:30:17.000000 mctech_discovery-1.1.8/mctech_discovery/rpc/web_error.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.714702 mctech_discovery-1.1.8/mctech_discovery/test/
--rw-rw-rw-   0        0        0        0 2020-06-01 05:42:33.000000 mctech_discovery-1.1.8/mctech_discovery/test/__init__.py
--rw-rw-rw-   0        0        0      196 2022-10-08 03:15:48.000000 mctech_discovery-1.1.8/mctech_discovery/test/config_test.py
--rw-rw-rw-   0        0        0      491 2022-10-08 03:15:48.000000 mctech_discovery-1.1.8/mctech_discovery/test/crypto_text.py
--rw-rw-rw-   0        0        0     1859 2023-12-06 02:01:53.000000 mctech_discovery-1.1.8/mctech_discovery/test/eureka_test.py
--rw-rw-rw-   0        0        0      650 2023-05-12 06:58:39.000000 mctech_discovery-1.1.8/mctech_discovery/test/pkg_test.py
-drwxrwxrwx   0        0        0        0 2023-12-06 02:02:11.628098 mctech_discovery-1.1.8/mctech_discovery.egg-info/
--rw-rw-rw-   0        0        0      151 2023-12-06 02:02:11.000000 mctech_discovery-1.1.8/mctech_discovery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1566 2023-12-06 02:02:11.000000 mctech_discovery-1.1.8/mctech_discovery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-06 02:02:11.000000 mctech_discovery-1.1.8/mctech_discovery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       86 2023-12-06 02:02:11.000000 mctech_discovery-1.1.8/mctech_discovery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-12-06 02:02:11.000000 mctech_discovery-1.1.8/mctech_discovery.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      395 2023-12-06 02:02:04.000000 mctech_discovery-1.1.8/mctech_discovery_setup.py
--rw-rw-rw-   0        0        0       42 2023-12-06 02:02:11.719698 mctech_discovery-1.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.255380 mctech_discovery-1.1.9/
+-rw-rw-rw-   0        0        0      151 2023-12-11 02:29:28.254380 mctech_discovery-1.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      497 2023-07-19 12:16:29.000000 mctech_discovery-1.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.126785 mctech_discovery-1.1.9/mctech_discovery/
+-rw-rw-rw-   0        0        0       72 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.153794 mctech_discovery-1.1.9/mctech_discovery/config/
+-rw-rw-rw-   0        0        0      977 2022-10-08 03:15:48.000000 mctech_discovery-1.1.9/mctech_discovery/config/__init__.py
+-rw-rw-rw-   0        0        0     8300 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/config/_configure.py
+-rw-rw-rw-   0        0        0     8384 2023-08-26 09:57:47.000000 mctech_discovery-1.1.9/mctech_discovery/config/config_merger.py
+-rw-rw-rw-   0        0        0     1922 2022-10-08 03:15:48.000000 mctech_discovery-1.1.9/mctech_discovery/config/config_value.py
+-rw-rw-rw-   0        0        0     1464 2023-05-12 06:58:39.000000 mctech_discovery-1.1.9/mctech_discovery/config/yaml_loader.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.171782 mctech_discovery-1.1.9/mctech_discovery/discovery/
+-rw-rw-rw-   0        0        0     1420 2022-10-08 03:15:48.000000 mctech_discovery-1.1.9/mctech_discovery/discovery/__init__.py
+-rw-rw-rw-   0        0        0     8996 2023-12-05 09:34:59.000000 mctech_discovery-1.1.9/mctech_discovery/discovery/eureka_discovery_client.py
+-rw-rw-rw-   0        0        0      830 2022-10-08 03:15:48.000000 mctech_discovery-1.1.9/mctech_discovery/discovery/local_discovery_client.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.177783 mctech_discovery-1.1.9/mctech_discovery/lifecycle/
+-rw-rw-rw-   0        0        0        0 2023-05-12 06:58:39.000000 mctech_discovery-1.1.9/mctech_discovery/lifecycle/__init__.py
+-rw-rw-rw-   0        0        0     1167 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/lifecycle/lifecycle.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.188784 mctech_discovery-1.1.9/mctech_discovery/rpc/
+-rw-rw-rw-   0        0        0       68 2023-12-05 09:44:25.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.202848 mctech_discovery-1.1.9/mctech_discovery/rpc/ep/
+-rw-rw-rw-   0        0        0        0 2020-06-01 03:25:27.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/ep/__init__.py
+-rw-rw-rw-   0        0        0      640 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/ep/ep_request.py
+-rw-rw-rw-   0        0        0     4220 2023-12-11 02:26:05.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/ep/internal_rpc.py
+-rw-rw-rw-   0        0        0      719 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/ep/simple_ep_request.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.223390 mctech_discovery-1.1.9/mctech_discovery/rpc/lb/
+-rw-rw-rw-   0        0        0     3253 2023-11-02 11:17:36.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/lb/__init__.py
+-rw-rw-rw-   0        0        0     1555 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/lb/direct_loadbalancer.py
+-rw-rw-rw-   0        0        0     1903 2023-12-05 09:50:47.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/lb/discovery_service_loadbalancer.py
+-rw-rw-rw-   0        0        0     1299 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/lb/loadbalancer.py
+-rw-rw-rw-   0        0        0     1180 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/lb/local_service_loadabalancer.py
+-rw-rw-rw-   0        0        0     1070 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/lb/retry_loadbalancer.py
+-rw-rw-rw-   0        0        0    10261 2023-12-11 02:01:56.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/request_context.py
+-rw-rw-rw-   0        0        0     4777 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/rpc_client.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.230392 mctech_discovery-1.1.9/mctech_discovery/rpc/rule/
+-rw-rw-rw-   0        0        0        0 2023-05-12 06:58:39.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/rule/__init__.py
+-rw-rw-rw-   0        0        0     1041 2023-12-05 09:49:38.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/rule/abstarct_rule.py
+-rw-rw-rw-   0        0        0      477 2023-05-12 06:58:39.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/rule/simple_rule.py
+-rw-rw-rw-   0        0        0      785 2023-09-20 02:30:17.000000 mctech_discovery-1.1.9/mctech_discovery/rpc/web_error.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.249381 mctech_discovery-1.1.9/mctech_discovery/test/
+-rw-rw-rw-   0        0        0        0 2020-06-01 05:42:33.000000 mctech_discovery-1.1.9/mctech_discovery/test/__init__.py
+-rw-rw-rw-   0        0        0      196 2022-10-08 03:15:48.000000 mctech_discovery-1.1.9/mctech_discovery/test/config_test.py
+-rw-rw-rw-   0        0        0      491 2022-10-08 03:15:48.000000 mctech_discovery-1.1.9/mctech_discovery/test/crypto_text.py
+-rw-rw-rw-   0        0        0     1859 2023-12-06 02:01:53.000000 mctech_discovery-1.1.9/mctech_discovery/test/eureka_test.py
+-rw-rw-rw-   0        0        0      650 2023-05-12 06:58:39.000000 mctech_discovery-1.1.9/mctech_discovery/test/pkg_test.py
+drwxrwxrwx   0        0        0        0 2023-12-11 02:29:28.137796 mctech_discovery-1.1.9/mctech_discovery.egg-info/
+-rw-rw-rw-   0        0        0      151 2023-12-11 02:29:28.000000 mctech_discovery-1.1.9/mctech_discovery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1566 2023-12-11 02:29:28.000000 mctech_discovery-1.1.9/mctech_discovery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-11 02:29:28.000000 mctech_discovery-1.1.9/mctech_discovery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       86 2023-12-11 02:29:28.000000 mctech_discovery-1.1.9/mctech_discovery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-12-11 02:29:28.000000 mctech_discovery-1.1.9/mctech_discovery.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      395 2023-12-11 02:27:17.000000 mctech_discovery-1.1.9/mctech_discovery_setup.py
+-rw-rw-rw-   0        0        0       42 2023-12-11 02:29:28.256385 mctech_discovery-1.1.9/setup.cfg
```

### Comparing `mctech_discovery-1.1.8/mctech_discovery/config/__init__.py` & `mctech_discovery-1.1.9/mctech_discovery/config/__init__.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/config/_configure.py` & `mctech_discovery-1.1.9/mctech_discovery/config/_configure.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/config/config_merger.py` & `mctech_discovery-1.1.9/mctech_discovery/config/config_merger.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/config/config_value.py` & `mctech_discovery-1.1.9/mctech_discovery/config/config_value.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/config/yaml_loader.py` & `mctech_discovery-1.1.9/mctech_discovery/config/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/discovery/__init__.py` & `mctech_discovery-1.1.9/mctech_discovery/discovery/__init__.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/discovery/eureka_discovery_client.py` & `mctech_discovery-1.1.9/mctech_discovery/discovery/eureka_discovery_client.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/discovery/local_discovery_client.py` & `mctech_discovery-1.1.9/mctech_discovery/discovery/local_discovery_client.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/lifecycle/lifecycle.py` & `mctech_discovery-1.1.9/mctech_discovery/lifecycle/lifecycle.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/ep/ep_request.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/ep/ep_request.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/ep/internal_rpc.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/ep/internal_rpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     option['headers'].update(context.headers)
     context.process_request_option(option)
     return option
 
 
 async def _walk_using_urllib(context: RequestContext, url: str) -> httpx.Response:  # noqa
     option = _create_request_option(context, url)
-    async with httpx.AsyncClient() as client:
+    timeout = httpx.Timeout(10.0, connect=5.0)
+    async with httpx.AsyncClient(timeout=timeout) as client:
         content_type = option['headers'].get('content-type') or ''
         kwargs = {}
         body = option["body"]
         if isinstance(body, (str, bytes)):
             kwargs['content'] = body
         # elif isinstance(body, io.IOBase):
         #     pass
```

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/ep/simple_ep_request.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/ep/simple_ep_request.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/lb/__init__.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/lb/__init__.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/lb/direct_loadbalancer.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/lb/direct_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/lb/discovery_service_loadbalancer.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/lb/discovery_service_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/lb/loadbalancer.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/lb/loadbalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/lb/local_service_loadabalancer.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/lb/local_service_loadabalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/lb/retry_loadbalancer.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/lb/retry_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/rpc_client.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/rpc_client.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/rule/abstarct_rule.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/rule/abstarct_rule.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/rpc/web_error.py` & `mctech_discovery-1.1.9/mctech_discovery/rpc/web_error.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/test/eureka_test.py` & `mctech_discovery-1.1.9/mctech_discovery/test/eureka_test.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery/test/pkg_test.py` & `mctech_discovery-1.1.9/mctech_discovery/test/pkg_test.py`

 * *Files identical despite different names*

### Comparing `mctech_discovery-1.1.8/mctech_discovery.egg-info/SOURCES.txt` & `mctech_discovery-1.1.9/mctech_discovery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

