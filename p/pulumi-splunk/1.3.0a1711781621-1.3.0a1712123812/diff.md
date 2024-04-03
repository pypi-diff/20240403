# Comparing `tmp/pulumi_splunk-1.3.0a1711781621.tar.gz` & `tmp/pulumi_splunk-1.3.0a1712123812.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_splunk-1.3.0a1711781621.tar", last modified: Sat Mar 30 06:55:58 2024, max compression
+gzip compressed data, was "pulumi_splunk-1.3.0a1712123812.tar", last modified: Wed Apr  3 05:58:43 2024, max compression
```

## Comparing `pulumi_splunk-1.3.0a1711781621.tar` & `pulumi_splunk-1.3.0a1712123812.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:55:58.664319 pulumi_splunk-1.3.0a1711781621/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-30 06:55:58.664319 pulumi_splunk-1.3.0a1711781621/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:55:58.660319 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/
--rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/admin_saml_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    38756 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/apps_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    22001 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/authentication_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/authorization_roles.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:55:58.664319 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/configs_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/data_ui_views.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/generic_acl.py
--rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/global_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)   154940 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_http_event_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)    42158 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_tcp_cooked.py
--rw-r--r--   0 runner    (1001) docker     (127)    36720 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_tcp_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_tcp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_udp.py
--rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    44131 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs_tcp_default.py
--rw-r--r--   0 runner    (1001) docker     (127)    43577 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs_tcp_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    32027 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    27963 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs_tcp_syslog.py
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   515197 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/saved_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk/sh_indexes_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 06:55:58.664319 pulumi_splunk-1.3.0a1711781621/pulumi_splunk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-03-30 06:55:58.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-30 06:55:58.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 06:55:58.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-30 06:55:58.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 06:55:58.000000 pulumi_splunk-1.3.0a1711781621/pulumi_splunk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-30 06:55:52.000000 pulumi_splunk-1.3.0a1711781621/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-30 06:55:58.664319 pulumi_splunk-1.3.0a1711781621/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:43.114420 pulumi_splunk-1.3.0a1712123812/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-03 05:58:43.114420 pulumi_splunk-1.3.0a1712123812/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:43.110420 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/
+-rw-r--r--   0 runner    (1001) docker     (127)     5441 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148655 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/admin_saml_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38756 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/apps_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22001 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/authentication_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45908 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/authorization_roles.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:43.110420 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/configs_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14457 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/data_ui_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/generic_acl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25146 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/global_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)   154940 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23872 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_http_event_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42158 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29999 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19019 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_cooked.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36720 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10637 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_splunk_tcp_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14095 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34349 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)   127784 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44131 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43577 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32027 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27963 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_syslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   515197 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/saved_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17106 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk/sh_indexes_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:58:43.114420 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3454 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 05:58:43.000000 pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-03 05:58:36.000000 pulumi_splunk-1.3.0a1712123812/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:58:43.114420 pulumi_splunk-1.3.0a1712123812/setup.cfg
```

### Comparing `pulumi_splunk-1.3.0a1711781621/PKG-INFO` & `pulumi_splunk-1.3.0a1712123812/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1711781621
+Version: 1.3.0a1712123812
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1711781621/README.md` & `pulumi_splunk-1.3.0a1712123812/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/__init__.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/_inputs.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/_utilities.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/admin_saml_groups.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/admin_saml_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/apps_local.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/apps_local.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/authentication_users.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/authentication_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/authorization_roles.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/authorization_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/config/__init__.pyi` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/config/vars.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/configs_conf.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/configs_conf.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/data_ui_views.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/data_ui_views.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/generic_acl.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/generic_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/global_http_event_collector.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/global_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/indexes.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/indexes.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_http_event_collector.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_http_event_collector.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_monitor.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_monitor.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_script.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_tcp_cooked.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_cooked.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_tcp_raw.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_raw.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_tcp_splunk_tcp_token.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_splunk_tcp_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_tcp_ssl.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_tcp_ssl.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/inputs_udp.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/inputs_udp.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs_tcp_default.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs_tcp_group.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs_tcp_server.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_server.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/outputs_tcp_syslog.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/outputs_tcp_syslog.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/provider.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/saved_searches.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/saved_searches.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk/sh_indexes_manager.py` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk/sh_indexes_manager.py`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk.egg-info/PKG-INFO` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_splunk
-Version: 1.3.0a1711781621
+Version: 1.3.0a1712123812
 Summary: A Pulumi package for creating and managing splunk cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-splunk
 Keywords: pulumi,splunk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_splunk-1.3.0a1711781621/pulumi_splunk.egg-info/SOURCES.txt` & `pulumi_splunk-1.3.0a1712123812/pulumi_splunk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_splunk-1.3.0a1711781621/pyproject.toml` & `pulumi_splunk-1.3.0a1712123812/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_splunk"
   description = "A Pulumi package for creating and managing splunk cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0a1,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "splunk"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.3.0a1711781621"
+  version = "1.3.0a1712123812"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-splunk"
 
 [build-system]
```

