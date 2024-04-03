# Comparing `tmp/cdk-certbot-dns-route53-2.4.93.tar.gz` & `tmp/cdk-certbot-dns-route53-2.4.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-certbot-dns-route53-2.4.93.tar", last modified: Mon Apr  1 00:29:32 2024, max compression
+gzip compressed data, was "cdk-certbot-dns-route53-2.4.94.tar", last modified: Tue Apr  2 00:26:59 2024, max compression
```

## Comparing `cdk-certbot-dns-route53-2.4.93.tar` & `cdk-certbot-dns-route53-2.4.94.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:29:32.693089 cdk-certbot-dns-route53-2.4.93/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-01 00:29:32.693089 cdk-certbot-dns-route53-2.4.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 00:29:32.693089 cdk-certbot-dns-route53-2.4.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:29:32.693089 cdk-certbot-dns-route53-2.4.93/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:29:32.693089 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53/
--rw-r--r--   0 runner    (1001) docker     (127)    36178 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:29:32.693089 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33225 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53/_jsii/cdk-certbot-dns-route53@2.4.93.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:29:21.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 00:29:32.693089 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-01 00:29:32.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-01 00:29:32.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 00:29:32.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-01 00:29:32.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 00:29:32.000000 cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:26:59.785668 cdk-certbot-dns-route53-2.4.94/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-02 00:26:59.785668 cdk-certbot-dns-route53-2.4.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 00:26:59.785668 cdk-certbot-dns-route53-2.4.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:26:59.781669 cdk-certbot-dns-route53-2.4.94/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:26:59.785668 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53/
+-rw-r--r--   0 runner    (1001) docker     (127)    36178 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:26:59.785668 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33227 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53/_jsii/cdk-certbot-dns-route53@2.4.94.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:26:47.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 00:26:59.785668 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-02 00:26:59.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-02 00:26:59.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 00:26:59.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 00:26:59.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-02 00:26:59.000000 cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53.egg-info/top_level.txt
```

### Comparing `cdk-certbot-dns-route53-2.4.93/LICENSE` & `cdk-certbot-dns-route53-2.4.94/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.93/PKG-INFO` & `cdk-certbot-dns-route53-2.4.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-certbot-dns-route53
-Version: 2.4.93
+Version: 2.4.94
 Summary: Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.
 Home-page: https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-certbot-dns-route53-2.4.93/README.md` & `cdk-certbot-dns-route53-2.4.94/README.md`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.93/setup.py` & `cdk-certbot-dns-route53-2.4.94/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-certbot-dns-route53",
-    "version": "2.4.93",
+    "version": "2.4.94",
     "description": "Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.",
     "license": "Apache-2.0",
     "url": "https://github.com/neilkuan/cdk-certbot-dns-route53.git",
     "long_description_content_type": "text/markdown",
     "author": "Neil Kuan<guan840912@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_certbot_dns_route53",
         "cdk_certbot_dns_route53._jsii"
     ],
     "package_data": {
         "cdk_certbot_dns_route53._jsii": [
-            "cdk-certbot-dns-route53@2.4.93.jsii.tgz"
+            "cdk-certbot-dns-route53@2.4.94.jsii.tgz"
         ],
         "cdk_certbot_dns_route53": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53/__init__.py` & `cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53/_jsii/__init__.py` & `cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53/_jsii/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 
 import aws_cdk._jsii
 import aws_cdk.aws_lambda_python_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "cdk-certbot-dns-route53",
-    "2.4.93",
+    "2.4.94",
     __name__[0:-6],
-    "cdk-certbot-dns-route53@2.4.93.jsii.tgz",
+    "cdk-certbot-dns-route53@2.4.94.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `cdk-certbot-dns-route53-2.4.93/src/cdk_certbot_dns_route53.egg-info/PKG-INFO` & `cdk-certbot-dns-route53-2.4.94/src/cdk_certbot_dns_route53.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-certbot-dns-route53
-Version: 2.4.93
+Version: 2.4.94
 Summary: Create Cron Job Via Lambda, to update certificate and put it to S3 Bucket.
 Home-page: https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Author: Neil Kuan<guan840912@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/neilkuan/cdk-certbot-dns-route53.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

