# Comparing `tmp/nodestream_plugin_akamai-0.9.0.tar.gz` & `tmp/nodestream_plugin_akamai-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nodestream_plugin_akamai-0.9.0.tar", max compression
+gzip compressed data, was "nodestream_plugin_akamai-0.9.1.tar", max compression
```

## Comparing `nodestream_plugin_akamai-0.9.0.tar` & `nodestream_plugin_akamai-0.9.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0    11357 2023-08-09 17:50:02.744276 nodestream_plugin_akamai-0.9.0/LICENSE
--rw-r--r--   0        0        0      853 2023-12-11 23:25:56.153522 nodestream_plugin_akamai-0.9.0/nodestream_akamai/__init__.py
--rw-r--r--   0        0        0      129 2023-12-11 23:25:56.154575 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/__init__.py
--rw-r--r--   0        0        0     1135 2023-12-11 23:25:56.155370 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/appsec_client.py
--rw-r--r--   0        0        0     4169 2023-12-11 23:25:56.156139 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/client.py
--rw-r--r--   0        0        0     6054 2023-12-11 23:25:56.156950 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/cloudlets_v2_client.py
--rw-r--r--   0        0        0      791 2023-12-11 23:25:56.157840 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/cps_client.py
--rw-r--r--   0        0        0      318 2023-12-11 23:25:56.158771 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/edgehostnames_client.py
--rw-r--r--   0        0        0      570 2023-12-11 23:25:56.159592 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/gtm_client.py
--rw-r--r--   0        0        0     1364 2023-12-11 23:25:56.160419 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/model.py
--rw-r--r--   0        0        0      402 2023-12-11 23:25:56.161301 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/netstorage_client.py
--rw-r--r--   0        0        0    11743 2023-12-11 23:25:56.162548 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/property_client.py
--rw-r--r--   0        0        0      327 2023-12-11 23:25:56.163586 nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/siteshield_client.py
--rw-r--r--   0        0        0      747 2023-12-11 23:25:56.164574 nodestream_plugin_akamai-0.9.0/nodestream_akamai/appsec-coverage.yaml
--rw-r--r--   0        0        0      105 2023-08-30 18:24:04.874605 nodestream_plugin_akamai-0.9.0/nodestream_akamai/appsec_coverage/__init__.py
--rw-r--r--   0        0        0     1995 2023-12-11 23:25:56.165399 nodestream_plugin_akamai-0.9.0/nodestream_akamai/appsec_coverage/appsec_coverage.py
--rw-r--r--   0        0        0       71 2023-08-30 18:24:04.876433 nodestream_plugin_akamai-0.9.0/nodestream_akamai/cps/__init__.py
--rw-r--r--   0        0        0     1191 2023-12-11 23:25:56.167266 nodestream_plugin_akamai-0.9.0/nodestream_akamai/cps/cps.py
--rw-r--r--   0        0        0      980 2023-12-11 23:25:56.166375 nodestream_plugin_akamai-0.9.0/nodestream_akamai/cps.yaml
--rw-r--r--   0        0        0       71 2023-08-30 18:24:04.878179 nodestream_plugin_akamai-0.9.0/nodestream_akamai/ehn/__init__.py
--rw-r--r--   0        0        0      785 2023-12-11 23:25:56.168825 nodestream_plugin_akamai-0.9.0/nodestream_akamai/ehn/ehn.py
--rw-r--r--   0        0        0      853 2023-12-11 23:25:56.168006 nodestream_plugin_akamai-0.9.0/nodestream_akamai/ehn.yaml
--rw-r--r--   0        0        0       71 2023-08-30 18:24:04.879848 nodestream_plugin_akamai-0.9.0/nodestream_akamai/gtm/__init__.py
--rw-r--r--   0        0        0     1155 2023-12-11 23:25:56.170311 nodestream_plugin_akamai-0.9.0/nodestream_akamai/gtm/gtm.py
--rw-r--r--   0        0        0     1038 2023-12-11 23:25:56.169561 nodestream_plugin_akamai-0.9.0/nodestream_akamai/gtm.yaml
--rw-r--r--   0        0        0      114 2023-12-11 20:02:21.488557 nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_account/__init__.py
--rw-r--r--   0        0        0     1398 2023-12-11 23:25:56.172457 nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_account/netstorage_account.py
--rw-r--r--   0        0        0     1712 2023-12-11 23:25:56.171466 nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_account.yaml
--rw-r--r--   0        0        0      108 2023-12-11 20:02:21.491092 nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_group/__init__.py
--rw-r--r--   0        0        0     1889 2023-12-11 23:25:56.174617 nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_group/netstorage_group.py
--rw-r--r--   0        0        0     2325 2023-12-11 23:25:56.173578 nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_group.yaml
--rw-r--r--   0        0        0      279 2023-12-11 23:25:56.175561 nodestream_plugin_akamai-0.9.0/nodestream_akamai/plugin.py
--rw-r--r--   0        0        0       86 2023-08-30 18:24:04.884161 nodestream_plugin_akamai-0.9.0/nodestream_akamai/property/__init__.py
--rw-r--r--   0        0        0     1212 2023-12-11 23:25:56.177323 nodestream_plugin_akamai-0.9.0/nodestream_akamai/property/property.py
--rw-r--r--   0        0        0     1118 2023-12-11 23:25:56.176284 nodestream_plugin_akamai-0.9.0/nodestream_akamai/property.yaml
--rw-r--r--   0        0        0       86 2023-08-30 18:24:04.885976 nodestream_plugin_akamai-0.9.0/nodestream_akamai/redirect/__init__.py
--rw-r--r--   0        0        0      771 2023-12-11 23:25:56.179415 nodestream_plugin_akamai-0.9.0/nodestream_akamai/redirect/redirect.py
--rw-r--r--   0        0        0      977 2023-12-11 23:25:56.178301 nodestream_plugin_akamai-0.9.0/nodestream_akamai/redirect.yaml
--rw-r--r--   0        0        0       92 2023-08-30 18:24:04.887824 nodestream_plugin_akamai-0.9.0/nodestream_akamai/siteshield/__init__.py
--rw-r--r--   0        0        0      655 2023-12-11 23:25:56.182041 nodestream_plugin_akamai-0.9.0/nodestream_akamai/siteshield/siteshield.py
--rw-r--r--   0        0        0      970 2023-12-11 23:25:56.180568 nodestream_plugin_akamai-0.9.0/nodestream_akamai/siteshield.yaml
--rw-r--r--   0        0        0       71 2023-08-30 18:24:04.889781 nodestream_plugin_akamai-0.9.0/nodestream_akamai/waf/__init__.py
--rw-r--r--   0        0        0     3045 2023-12-11 23:25:56.184190 nodestream_plugin_akamai-0.9.0/nodestream_akamai/waf/waf.py
--rw-r--r--   0        0        0     1050 2023-12-11 23:25:56.182875 nodestream_plugin_akamai-0.9.0/nodestream_akamai/waf.yaml
--rw-r--r--   0        0        0     1105 2023-12-12 21:57:58.644144 nodestream_plugin_akamai-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      626 1970-01-01 00:00:00.000000 nodestream_plugin_akamai-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-09 17:50:02.744276 nodestream_plugin_akamai-0.9.1/LICENSE
+-rw-r--r--   0        0        0      853 2023-12-11 23:25:56.153522 nodestream_plugin_akamai-0.9.1/nodestream_akamai/__init__.py
+-rw-r--r--   0        0        0      129 2023-12-11 23:25:56.154575 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/__init__.py
+-rw-r--r--   0        0        0     1135 2023-12-11 23:25:56.155370 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/appsec_client.py
+-rw-r--r--   0        0        0     4169 2023-12-11 23:25:56.156139 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/client.py
+-rw-r--r--   0        0        0     6054 2023-12-11 23:25:56.156950 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/cloudlets_v2_client.py
+-rw-r--r--   0        0        0      791 2023-12-11 23:25:56.157840 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/cps_client.py
+-rw-r--r--   0        0        0      318 2023-12-11 23:25:56.158771 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/edgehostnames_client.py
+-rw-r--r--   0        0        0      570 2023-12-11 23:25:56.159592 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/gtm_client.py
+-rw-r--r--   0        0        0     1364 2023-12-11 23:25:56.160419 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/model.py
+-rw-r--r--   0        0        0      402 2023-12-11 23:25:56.161301 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/netstorage_client.py
+-rw-r--r--   0        0        0    11743 2023-12-11 23:25:56.162548 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/property_client.py
+-rw-r--r--   0        0        0      327 2023-12-11 23:25:56.163586 nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/siteshield_client.py
+-rw-r--r--   0        0        0      747 2023-12-11 23:25:56.164574 nodestream_plugin_akamai-0.9.1/nodestream_akamai/appsec-coverage.yaml
+-rw-r--r--   0        0        0      105 2023-08-30 18:24:04.874605 nodestream_plugin_akamai-0.9.1/nodestream_akamai/appsec_coverage/__init__.py
+-rw-r--r--   0        0        0     1995 2023-12-11 23:25:56.165399 nodestream_plugin_akamai-0.9.1/nodestream_akamai/appsec_coverage/appsec_coverage.py
+-rw-r--r--   0        0        0       71 2023-08-30 18:24:04.876433 nodestream_plugin_akamai-0.9.1/nodestream_akamai/cps/__init__.py
+-rw-r--r--   0        0        0     1191 2023-12-11 23:25:56.167266 nodestream_plugin_akamai-0.9.1/nodestream_akamai/cps/cps.py
+-rw-r--r--   0        0        0      980 2023-12-11 23:25:56.166375 nodestream_plugin_akamai-0.9.1/nodestream_akamai/cps.yaml
+-rw-r--r--   0        0        0       71 2023-08-30 18:24:04.878179 nodestream_plugin_akamai-0.9.1/nodestream_akamai/ehn/__init__.py
+-rw-r--r--   0        0        0      785 2023-12-11 23:25:56.168825 nodestream_plugin_akamai-0.9.1/nodestream_akamai/ehn/ehn.py
+-rw-r--r--   0        0        0      853 2023-12-11 23:25:56.168006 nodestream_plugin_akamai-0.9.1/nodestream_akamai/ehn.yaml
+-rw-r--r--   0        0        0       71 2023-08-30 18:24:04.879848 nodestream_plugin_akamai-0.9.1/nodestream_akamai/gtm/__init__.py
+-rw-r--r--   0        0        0     1155 2023-12-11 23:25:56.170311 nodestream_plugin_akamai-0.9.1/nodestream_akamai/gtm/gtm.py
+-rw-r--r--   0        0        0     1038 2023-12-11 23:25:56.169561 nodestream_plugin_akamai-0.9.1/nodestream_akamai/gtm.yaml
+-rw-r--r--   0        0        0      114 2023-12-11 20:02:21.488557 nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_account/__init__.py
+-rw-r--r--   0        0        0     1398 2023-12-11 23:25:56.172457 nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_account/netstorage_account.py
+-rw-r--r--   0        0        0     1712 2023-12-11 23:25:56.171466 nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_account.yaml
+-rw-r--r--   0        0        0      108 2023-12-11 20:02:21.491092 nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_group/__init__.py
+-rw-r--r--   0        0        0     1889 2023-12-11 23:25:56.174617 nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_group/netstorage_group.py
+-rw-r--r--   0        0        0     2325 2023-12-11 23:25:56.173578 nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_group.yaml
+-rw-r--r--   0        0        0      279 2023-12-11 23:25:56.175561 nodestream_plugin_akamai-0.9.1/nodestream_akamai/plugin.py
+-rw-r--r--   0        0        0       86 2023-08-30 18:24:04.884161 nodestream_plugin_akamai-0.9.1/nodestream_akamai/property/__init__.py
+-rw-r--r--   0        0        0     1212 2023-12-11 23:25:56.177323 nodestream_plugin_akamai-0.9.1/nodestream_akamai/property/property.py
+-rw-r--r--   0        0        0     1118 2023-12-11 23:25:56.176284 nodestream_plugin_akamai-0.9.1/nodestream_akamai/property.yaml
+-rw-r--r--   0        0        0       86 2023-08-30 18:24:04.885976 nodestream_plugin_akamai-0.9.1/nodestream_akamai/redirect/__init__.py
+-rw-r--r--   0        0        0      771 2023-12-11 23:25:56.179415 nodestream_plugin_akamai-0.9.1/nodestream_akamai/redirect/redirect.py
+-rw-r--r--   0        0        0      977 2023-12-11 23:25:56.178301 nodestream_plugin_akamai-0.9.1/nodestream_akamai/redirect.yaml
+-rw-r--r--   0        0        0       92 2023-08-30 18:24:04.887824 nodestream_plugin_akamai-0.9.1/nodestream_akamai/siteshield/__init__.py
+-rw-r--r--   0        0        0      655 2023-12-11 23:25:56.182041 nodestream_plugin_akamai-0.9.1/nodestream_akamai/siteshield/siteshield.py
+-rw-r--r--   0        0        0      970 2023-12-11 23:25:56.180568 nodestream_plugin_akamai-0.9.1/nodestream_akamai/siteshield.yaml
+-rw-r--r--   0        0        0       71 2023-08-30 18:24:04.889781 nodestream_plugin_akamai-0.9.1/nodestream_akamai/waf/__init__.py
+-rw-r--r--   0        0        0     3045 2023-12-11 23:25:56.184190 nodestream_plugin_akamai-0.9.1/nodestream_akamai/waf/waf.py
+-rw-r--r--   0        0        0     1050 2023-12-11 23:25:56.182875 nodestream_plugin_akamai-0.9.1/nodestream_akamai/waf.yaml
+-rw-r--r--   0        0        0     1110 2023-12-12 22:34:59.061909 nodestream_plugin_akamai-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      570 1970-01-01 00:00:00.000000 nodestream_plugin_akamai-0.9.1/PKG-INFO
```

### Comparing `nodestream_plugin_akamai-0.9.0/LICENSE` & `nodestream_plugin_akamai-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/__init__.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/__init__.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/appsec_client.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/appsec_client.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/client.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/client.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/cloudlets_v2_client.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/cloudlets_v2_client.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/cps_client.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/cps_client.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/gtm_client.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/gtm_client.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/model.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/model.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/akamai_utils/property_client.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/akamai_utils/property_client.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/appsec-coverage.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/appsec-coverage.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/appsec_coverage/appsec_coverage.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/appsec_coverage/appsec_coverage.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/cps/cps.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/cps/cps.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/cps.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/cps.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/ehn/ehn.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/ehn/ehn.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/ehn.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/ehn.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/gtm/gtm.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/gtm/gtm.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/gtm.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/gtm.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_account/netstorage_account.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_account/netstorage_account.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_account.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_account.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_group/netstorage_group.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_group/netstorage_group.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/netstorage_group.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/netstorage_group.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/property/property.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/property/property.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/property.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/property.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/redirect/redirect.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/redirect/redirect.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/redirect.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/redirect.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/siteshield/siteshield.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/siteshield/siteshield.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/siteshield.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/siteshield.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/waf/waf.py` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/waf/waf.py`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/nodestream_akamai/waf.yaml` & `nodestream_plugin_akamai-0.9.1/nodestream_akamai/waf.yaml`

 * *Files identical despite different names*

### Comparing `nodestream_plugin_akamai-0.9.0/pyproject.toml` & `nodestream_plugin_akamai-0.9.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "nodestream-plugin-akamai"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = [
     "Zach Probst <Zach_Probst@intuit.com>",
     "Chad Cloes <Chad_Cloes@intuit.com>",
     "Bryan Norman <Bryan_Norman@intuit.com>",
     "Gabe Gallagher <Gabe_Gallagher@intuit.com>",
     "Grant Hoffman <Grant_Hoffman@intuit.com>"
 ]
 packages = [
     { include = "nodestream_akamai" }
 ]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.11"
 edgegrid-python = "^1.2.1"
 python-json-logger = "^2.0.2"
-python-dotenv = "^0.20.0"
+python-dotenv = ">=0.21.0,< 2"
 click = "^8.1.3"
 boto3 = "^1.26.3"
-nodestream = "^0.9.1"
+nodestream = "^0.9.3"
 jsonpath-ng = "^1.5.3"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.6.1"
```

### Comparing `nodestream_plugin_akamai-0.9.0/PKG-INFO` & `nodestream_plugin_akamai-0.9.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: nodestream-plugin-akamai
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: Zach Probst
 Author-email: Zach_Probst@intuit.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.26.3,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: edgegrid-python (>=1.2.1,<2.0.0)
 Requires-Dist: jsonpath-ng (>=1.5.3,<2.0.0)
-Requires-Dist: nodestream (>=0.9.1,<0.10.0)
-Requires-Dist: python-dotenv (>=0.20.0,<0.21.0)
+Requires-Dist: nodestream (>=0.9.3,<0.10.0)
+Requires-Dist: python-dotenv (>=0.21.0,<2)
 Requires-Dist: python-json-logger (>=2.0.2,<3.0.0)
```

