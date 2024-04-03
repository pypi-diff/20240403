# Comparing `tmp/localstack-extension-aws-replicator-0.1.8.tar.gz` & `tmp/localstack-extension-aws-replicator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-extension-aws-replicator-0.1.8.tar", last modified: Fri Feb  9 14:24:10 2024, max compression
+gzip compressed data, was "localstack-extension-aws-replicator-0.1.9.tar", last modified: Fri Feb  9 14:51:13 2024, max compression
```

## Comparing `localstack-extension-aws-replicator-0.1.8.tar` & `localstack-extension-aws-replicator-0.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:24:10.400351 localstack-extension-aws-replicator-0.1.8/
--rw-r--r--   0 whummer    (501) staff       (20)      117 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/MANIFEST.in
--rw-r--r--   0 whummer    (501) staff       (20)     7855 2024-02-09 14:24:10.400276 localstack-extension-aws-replicator-0.1.8/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)     6859 2024-02-09 14:14:37.000000 localstack-extension-aws-replicator-0.1.8/README.md
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:24:10.393197 localstack-extension-aws-replicator-0.1.8/aws_replicator/
--rw-r--r--   0 whummer    (501) staff       (20)       24 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/__init__.py
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:24:10.394994 localstack-extension-aws-replicator-0.1.8/aws_replicator/client/
--rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/client/__init__.py
--rw-r--r--   0 whummer    (501) staff       (20)    16045 2024-02-09 14:17:36.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/client/auth_proxy.py
--rw-r--r--   0 whummer    (501) staff       (20)     3279 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/client/cli.py
--rw-r--r--   0 whummer    (501) staff       (20)    10042 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/client/replicate.py
--rw-r--r--   0 whummer    (501) staff       (20)     4594 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/client/service_states.py
--rw-r--r--   0 whummer    (501) staff       (20)      916 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/client/utils.py
--rw-r--r--   0 whummer    (501) staff       (20)      414 2024-02-09 14:12:45.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/config.py
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:24:10.396014 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/
--rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/__init__.py
--rw-r--r--   0 whummer    (501) staff       (20)     8791 2023-12-10 18:13:38.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/aws_request_forwarder.py
--rw-r--r--   0 whummer    (501) staff       (20)      861 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/extension.py
--rw-r--r--   0 whummer    (501) staff       (20)     6099 2024-02-09 14:23:31.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/request_handler.py
--rw-r--r--   0 whummer    (501) staff       (20)     4087 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/resource_replicator.py
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:24:10.396990 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/ui/
--rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/ui/__init__.py
--rw-r--r--   0 whummer    (501) staff       (20)     5489 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/ui/app.js
--rw-r--r--   0 whummer    (501) staff       (20)     7206 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/ui/favicon.png
--rw-r--r--   0 whummer    (501) staff       (20)     1584 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/server/ui/index.html
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:24:10.397539 localstack-extension-aws-replicator-0.1.8/aws_replicator/shared/
--rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/shared/__init__.py
--rw-r--r--   0 whummer    (501) staff       (20)     3547 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/shared/models.py
--rw-r--r--   0 whummer    (501) staff       (20)      951 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/aws_replicator/shared/utils.py
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:24:10.399769 localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/
--rw-r--r--   0 whummer    (501) staff       (20)     7855 2024-02-09 14:24:10.000000 localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/PKG-INFO
--rw-r--r--   0 whummer    (501) staff       (20)     1248 2024-02-09 14:24:10.000000 localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/SOURCES.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2024-02-09 14:24:10.000000 localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/dependency_links.txt
--rw-r--r--   0 whummer    (501) staff       (20)      185 2024-02-09 14:24:10.000000 localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/entry_points.txt
--rw-r--r--   0 whummer    (501) staff       (20)        1 2024-02-09 14:23:54.000000 localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/not-zip-safe
--rw-r--r--   0 whummer    (501) staff       (20)      237 2024-02-09 14:24:10.000000 localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/requires.txt
--rw-r--r--   0 whummer    (501) staff       (20)       21 2024-02-09 14:24:10.000000 localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/top_level.txt
--rw-r--r--   0 whummer    (501) staff       (20)      226 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/pyproject.toml
--rw-r--r--   0 whummer    (501) staff       (20)     1098 2024-02-09 14:24:10.400633 localstack-extension-aws-replicator-0.1.8/setup.cfg
--rw-r--r--   0 whummer    (501) staff       (20)       60 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/setup.py
-drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:24:10.399217 localstack-extension-aws-replicator-0.1.8/tests/
--rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/tests/__init__.py
--rw-r--r--   0 whummer    (501) staff       (20)      538 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/tests/conftest.py
--rw-r--r--   0 whummer    (501) staff       (20)      578 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/tests/test_config.py
--rw-r--r--   0 whummer    (501) staff       (20)     6537 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.8/tests/test_extension.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:51:13.310151 localstack-extension-aws-replicator-0.1.9/
+-rw-r--r--   0 whummer    (501) staff       (20)      117 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/MANIFEST.in
+-rw-r--r--   0 whummer    (501) staff       (20)     7855 2024-02-09 14:51:13.310061 localstack-extension-aws-replicator-0.1.9/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)     6859 2024-02-09 14:14:37.000000 localstack-extension-aws-replicator-0.1.9/README.md
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:51:13.302459 localstack-extension-aws-replicator-0.1.9/aws_replicator/
+-rw-r--r--   0 whummer    (501) staff       (20)       24 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/__init__.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:51:13.304260 localstack-extension-aws-replicator-0.1.9/aws_replicator/client/
+-rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/client/__init__.py
+-rw-r--r--   0 whummer    (501) staff       (20)    16202 2024-02-09 14:50:16.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/client/auth_proxy.py
+-rw-r--r--   0 whummer    (501) staff       (20)     3279 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/client/cli.py
+-rw-r--r--   0 whummer    (501) staff       (20)    10042 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/client/replicate.py
+-rw-r--r--   0 whummer    (501) staff       (20)     4594 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/client/service_states.py
+-rw-r--r--   0 whummer    (501) staff       (20)      916 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/client/utils.py
+-rw-r--r--   0 whummer    (501) staff       (20)      733 2024-02-09 14:45:45.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/config.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:51:13.305336 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/
+-rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/__init__.py
+-rw-r--r--   0 whummer    (501) staff       (20)     8791 2023-12-10 18:13:38.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/aws_request_forwarder.py
+-rw-r--r--   0 whummer    (501) staff       (20)      861 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/extension.py
+-rw-r--r--   0 whummer    (501) staff       (20)     6099 2024-02-09 14:23:31.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/request_handler.py
+-rw-r--r--   0 whummer    (501) staff       (20)     4087 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/resource_replicator.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:51:13.306244 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/ui/
+-rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/ui/__init__.py
+-rw-r--r--   0 whummer    (501) staff       (20)     5489 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/ui/app.js
+-rw-r--r--   0 whummer    (501) staff       (20)     7206 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/ui/favicon.png
+-rw-r--r--   0 whummer    (501) staff       (20)     1584 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/server/ui/index.html
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:51:13.306908 localstack-extension-aws-replicator-0.1.9/aws_replicator/shared/
+-rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/shared/__init__.py
+-rw-r--r--   0 whummer    (501) staff       (20)     3547 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/shared/models.py
+-rw-r--r--   0 whummer    (501) staff       (20)      951 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/aws_replicator/shared/utils.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:51:13.309511 localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/
+-rw-r--r--   0 whummer    (501) staff       (20)     7855 2024-02-09 14:51:13.000000 localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/PKG-INFO
+-rw-r--r--   0 whummer    (501) staff       (20)     1248 2024-02-09 14:51:13.000000 localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/SOURCES.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2024-02-09 14:51:13.000000 localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/dependency_links.txt
+-rw-r--r--   0 whummer    (501) staff       (20)      185 2024-02-09 14:51:13.000000 localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/entry_points.txt
+-rw-r--r--   0 whummer    (501) staff       (20)        1 2024-02-09 14:51:00.000000 localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/not-zip-safe
+-rw-r--r--   0 whummer    (501) staff       (20)      237 2024-02-09 14:51:13.000000 localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/requires.txt
+-rw-r--r--   0 whummer    (501) staff       (20)       21 2024-02-09 14:51:13.000000 localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/top_level.txt
+-rw-r--r--   0 whummer    (501) staff       (20)      226 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/pyproject.toml
+-rw-r--r--   0 whummer    (501) staff       (20)     1098 2024-02-09 14:51:13.310524 localstack-extension-aws-replicator-0.1.9/setup.cfg
+-rw-r--r--   0 whummer    (501) staff       (20)       60 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/setup.py
+drwxr-xr-x   0 whummer    (501) staff       (20)        0 2024-02-09 14:51:13.308910 localstack-extension-aws-replicator-0.1.9/tests/
+-rw-r--r--   0 whummer    (501) staff       (20)        0 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/tests/__init__.py
+-rw-r--r--   0 whummer    (501) staff       (20)      538 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/tests/conftest.py
+-rw-r--r--   0 whummer    (501) staff       (20)      578 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/tests/test_config.py
+-rw-r--r--   0 whummer    (501) staff       (20)     6537 2023-12-08 15:45:24.000000 localstack-extension-aws-replicator-0.1.9/tests/test_extension.py
```

### Comparing `localstack-extension-aws-replicator-0.1.8/PKG-INFO` & `localstack-extension-aws-replicator-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-extension-aws-replicator
-Version: 0.1.8
+Version: 0.1.9
 Summary: LocalStack Extension: AWS replicator
 Home-page: https://github.com/localstack/localstack-extensions/tree/main/aws-replicator
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 Description-Content-Type: text/markdown; charset=UTF-8
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
```

### Comparing `localstack-extension-aws-replicator-0.1.8/README.md` & `localstack-extension-aws-replicator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/client/auth_proxy.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/client/auth_proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,14 +139,15 @@
 
     def register_in_instance(self):
         port = getattr(self, "port", None)
         if not port:
             raise Exception("Proxy currently not running")
         url = f"{external_service_url()}{HANDLER_PATH_PROXIES}"
         data = AddProxyRequest(port=port, config=self.config)
+        LOG.debug("Registering new proxy in main container via: %s", url)
         try:
             response = requests.post(url, json=data)
             assert response.ok
             return response
         except Exception:
             LOG.warning(
                 "Unable to register auth proxy - is LocalStack running with the extension enabled?"
@@ -343,15 +344,17 @@
         "AWS_SESSION_TOKEN",
         "AWS_DEFAULT_REGION",
         ENV_LOCALSTACK_API_KEY,
         ENV_LOCALSTACK_AUTH_TOKEN,
     ]
     env_vars = env_vars or os.environ
     env_vars = select_attributes(dict(env_vars), env_var_names)
-    env_vars["LOCALSTACK_HOST"] = "host.docker.internal"
+    # note: ...
+    target_host = repl_config.PROXY_LOCALSTACK_HOST or "host.docker.internal"
+    env_vars["LOCALSTACK_HOST"] = target_host
 
     try:
         print("Proxy container is ready.")
         command = f"{venv_activate}; localstack aws proxy -c {CONTAINER_CONFIG_FILE} -p {port} --host 0.0.0.0 > {CONTAINER_LOG_FILE} 2>&1"
         if quiet:
             DOCKER_CLIENT.exec_in_container(
                 container_name, command=["bash", "-c", command], env_vars=env_vars, interactive=True
```

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/client/cli.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/client/cli.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/client/replicate.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/client/replicate.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/client/service_states.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/client/service_states.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/client/utils.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/client/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/server/aws_request_forwarder.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/server/aws_request_forwarder.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/server/extension.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/server/extension.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/server/request_handler.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/server/request_handler.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/server/resource_replicator.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/server/resource_replicator.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/server/ui/app.js` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/server/ui/app.js`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/server/ui/favicon.png` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/server/ui/favicon.png`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/server/ui/index.html` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/server/ui/index.html`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/shared/models.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/shared/models.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/aws_replicator/shared/utils.py` & `localstack-extension-aws-replicator-0.1.9/aws_replicator/shared/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/PKG-INFO` & `localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack-extension-aws-replicator
-Version: 0.1.8
+Version: 0.1.9
 Summary: LocalStack Extension: AWS replicator
 Home-page: https://github.com/localstack/localstack-extensions/tree/main/aws-replicator
 Author: LocalStack Team
 Author-email: info@localstack.cloud
 Description-Content-Type: text/markdown; charset=UTF-8
 Requires-Dist: boto3>=1.26.151
 Requires-Dist: botocore>=1.29.151
```

### Comparing `localstack-extension-aws-replicator-0.1.8/localstack_extension_aws_replicator.egg-info/SOURCES.txt` & `localstack-extension-aws-replicator-0.1.9/localstack_extension_aws_replicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/setup.cfg` & `localstack-extension-aws-replicator-0.1.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = localstack-extension-aws-replicator
-version = 0.1.8
+version = 0.1.9
 summary = LocalStack Extension: AWS replicator
 description = Replicate AWS resources into your LocalStack instance
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/localstack/localstack-extensions/tree/main/aws-replicator
 author = LocalStack Team
 author_email = info@localstack.cloud
```

### Comparing `localstack-extension-aws-replicator-0.1.8/tests/conftest.py` & `localstack-extension-aws-replicator-0.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/tests/test_config.py` & `localstack-extension-aws-replicator-0.1.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `localstack-extension-aws-replicator-0.1.8/tests/test_extension.py` & `localstack-extension-aws-replicator-0.1.9/tests/test_extension.py`

 * *Files identical despite different names*

