# Comparing `tmp/certbot_dns_ispconfig_ddns-1.0.7.tar.gz` & `tmp/certbot_dns_ispconfig_ddns-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot_dns_ispconfig_ddns-1.0.7.tar", max compression
+gzip compressed data, was "certbot_dns_ispconfig_ddns-1.0.8.tar", max compression
```

## Comparing `certbot_dns_ispconfig_ddns-1.0.7.tar` & `certbot_dns_ispconfig_ddns-1.0.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11357 2024-03-25 09:02:48.030253 certbot_dns_ispconfig_ddns-1.0.7/LICENSE
--rw-r--r--   0        0        0     3569 2024-03-25 09:02:48.030253 certbot_dns_ispconfig_ddns-1.0.7/README.md
--rw-r--r--   0        0        0        0 2024-03-25 09:02:48.030253 certbot_dns_ispconfig_ddns-1.0.7/certbot_dns_ispconfig_ddns/__init__.py
--rw-r--r--   0        0        0     4353 2024-03-25 09:02:48.030253 certbot_dns_ispconfig_ddns-1.0.7/certbot_dns_ispconfig_ddns/authenticator.py
--rw-r--r--   0        0        0     3152 2024-03-25 09:02:48.030253 certbot_dns_ispconfig_ddns-1.0.7/certbot_dns_ispconfig_ddns/ispconfig_client.py
--rw-r--r--   0        0        0     1397 2024-03-25 09:03:10.006022 certbot_dns_ispconfig_ddns-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     4646 1970-01-01 00:00:00.000000 certbot_dns_ispconfig_ddns-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 17:13:05.928370 certbot_dns_ispconfig_ddns-1.0.8/LICENSE
+-rw-r--r--   0        0        0     3569 2024-04-03 17:13:05.928370 certbot_dns_ispconfig_ddns-1.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 17:13:05.928370 certbot_dns_ispconfig_ddns-1.0.8/certbot_dns_ispconfig_ddns/__init__.py
+-rw-r--r--   0        0        0     4353 2024-04-03 17:13:05.928370 certbot_dns_ispconfig_ddns-1.0.8/certbot_dns_ispconfig_ddns/authenticator.py
+-rw-r--r--   0        0        0     3152 2024-04-03 17:13:05.928370 certbot_dns_ispconfig_ddns-1.0.8/certbot_dns_ispconfig_ddns/ispconfig_client.py
+-rw-r--r--   0        0        0     1397 2024-04-03 17:13:32.460416 certbot_dns_ispconfig_ddns-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4646 1970-01-01 00:00:00.000000 certbot_dns_ispconfig_ddns-1.0.8/PKG-INFO
```

### Comparing `certbot_dns_ispconfig_ddns-1.0.7/LICENSE` & `certbot_dns_ispconfig_ddns-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `certbot_dns_ispconfig_ddns-1.0.7/README.md` & `certbot_dns_ispconfig_ddns-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `certbot_dns_ispconfig_ddns-1.0.7/certbot_dns_ispconfig_ddns/authenticator.py` & `certbot_dns_ispconfig_ddns-1.0.8/certbot_dns_ispconfig_ddns/authenticator.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_ispconfig_ddns-1.0.7/certbot_dns_ispconfig_ddns/ispconfig_client.py` & `certbot_dns_ispconfig_ddns-1.0.8/certbot_dns_ispconfig_ddns/ispconfig_client.py`

 * *Files identical despite different names*

### Comparing `certbot_dns_ispconfig_ddns-1.0.7/pyproject.toml` & `certbot_dns_ispconfig_ddns-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "certbot-dns-ispconfig-ddns"
-version = "1.0.7"
+version = "1.0.8"
 description = "Obtain certificates using a DNS TXT record for ISPConfig domains with DDNS module tokens"
 authors = ["Marcel Hofer <m.hofer117@gmail.com>"]
 readme = "README.md"
 homepage  = "https://github.com/mhofer117/certbot-dns-ispconfig-ddns"
 repository = "https://github.com/mhofer117/certbot-dns-ispconfig-ddns"
 license = "Apache-2.0"
 classifiers = [
```

### Comparing `certbot_dns_ispconfig_ddns-1.0.7/PKG-INFO` & `certbot_dns_ispconfig_ddns-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-dns-ispconfig-ddns
-Version: 1.0.7
+Version: 1.0.8
 Summary: Obtain certificates using a DNS TXT record for ISPConfig domains with DDNS module tokens
 Home-page: https://github.com/mhofer117/certbot-dns-ispconfig-ddns
 License: Apache-2.0
 Author: Marcel Hofer
 Author-email: m.hofer117@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

