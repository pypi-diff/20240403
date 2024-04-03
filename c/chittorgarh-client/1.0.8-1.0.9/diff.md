# Comparing `tmp/chittorgarh_client-1.0.8.tar.gz` & `tmp/chittorgarh_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chittorgarh_client-1.0.8.tar", last modified: Mon Oct 30 08:48:00 2023, max compression
+gzip compressed data, was "chittorgarh_client-1.0.9.tar", last modified: Mon Oct 30 11:46:00 2023, max compression
```

## Comparing `chittorgarh_client-1.0.8.tar` & `chittorgarh_client-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:48:00.684471 chittorgarh_client-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-10-30 08:48:00.684471 chittorgarh_client-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-30 08:47:37.000000 chittorgarh_client-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:48:00.684471 chittorgarh_client-1.0.8/chittorgarh_client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 08:47:37.000000 chittorgarh_client-1.0.8/chittorgarh_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7282 2023-10-30 08:47:37.000000 chittorgarh_client-1.0.8/chittorgarh_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-10-30 08:47:37.000000 chittorgarh_client-1.0.8/chittorgarh_client/mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2023-10-30 08:47:37.000000 chittorgarh_client-1.0.8/chittorgarh_client/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2023-10-30 08:47:37.000000 chittorgarh_client-1.0.8/chittorgarh_client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:48:00.684471 chittorgarh_client-1.0.8/chittorgarh_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2023-10-30 08:48:00.000000 chittorgarh_client-1.0.8/chittorgarh_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-30 08:48:00.000000 chittorgarh_client-1.0.8/chittorgarh_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 08:48:00.000000 chittorgarh_client-1.0.8/chittorgarh_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-30 08:48:00.000000 chittorgarh_client-1.0.8/chittorgarh_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-30 08:48:00.000000 chittorgarh_client-1.0.8/chittorgarh_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 08:48:00.684471 chittorgarh_client-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      458 2023-10-30 08:47:37.000000 chittorgarh_client-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 08:48:00.684471 chittorgarh_client-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 08:47:37.000000 chittorgarh_client-1.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:46:00.852972 chittorgarh_client-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-10-30 11:46:00.852972 chittorgarh_client-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-30 11:45:48.000000 chittorgarh_client-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:46:00.852972 chittorgarh_client-1.0.9/chittorgarh_client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:45:48.000000 chittorgarh_client-1.0.9/chittorgarh_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7337 2023-10-30 11:45:48.000000 chittorgarh_client-1.0.9/chittorgarh_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2023-10-30 11:45:48.000000 chittorgarh_client-1.0.9/chittorgarh_client/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2023-10-30 11:45:48.000000 chittorgarh_client-1.0.9/chittorgarh_client/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2023-10-30 11:45:48.000000 chittorgarh_client-1.0.9/chittorgarh_client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:46:00.852972 chittorgarh_client-1.0.9/chittorgarh_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2023-10-30 11:46:00.000000 chittorgarh_client-1.0.9/chittorgarh_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2023-10-30 11:46:00.000000 chittorgarh_client-1.0.9/chittorgarh_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-30 11:46:00.000000 chittorgarh_client-1.0.9/chittorgarh_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-10-30 11:46:00.000000 chittorgarh_client-1.0.9/chittorgarh_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2023-10-30 11:46:00.000000 chittorgarh_client-1.0.9/chittorgarh_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-30 11:46:00.852972 chittorgarh_client-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-10-30 11:45:48.000000 chittorgarh_client-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-30 11:46:00.852972 chittorgarh_client-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-30 11:45:48.000000 chittorgarh_client-1.0.9/tests/__init__.py
```

### Comparing `chittorgarh_client-1.0.8/chittorgarh_client/client.py` & `chittorgarh_client-1.0.9/chittorgarh_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
     live_subscription_category_mapping = {
         'Qualified Institutions': IPOSubscriptionCategory.QIB,
         'Non-Institutional Buyers': IPOSubscriptionCategory.NII,
         'bNII (bids above 10L)': IPOSubscriptionCategory.BHNI,
         'sNII (bids below 10L)': IPOSubscriptionCategory.SHNI,
         'Retail Investors': IPOSubscriptionCategory.Retail,
+        'Employees': IPOSubscriptionCategory.Employee,
         'Total **': IPOSubscriptionCategory.Total,
     }
 
     def get_live_subscription(self, ipo_id: Union[str, int]) -> Dict[str, Subscription]:
         table = parse_table_from_url(self.SUBSCRIPTION_URL.format(ipo_id=ipo_id), self.SUBSCRIPTION_XPATH)
         subscription_data = {}
```

### Comparing `chittorgarh_client-1.0.8/chittorgarh_client/mapper.py` & `chittorgarh_client-1.0.9/chittorgarh_client/mapper.py`

 * *Files identical despite different names*

### Comparing `chittorgarh_client-1.0.8/chittorgarh_client/models.py` & `chittorgarh_client-1.0.9/chittorgarh_client/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,8 +63,9 @@
 
 class IPOSubscriptionCategory:
     QIB = 'QIB'
     NII = 'NII'
     BHNI = 'BHNI'
     SHNI = 'SHNI'
     Retail = 'Retail'
+    Employee = 'Employee'
     Total = 'Total'
```

### Comparing `chittorgarh_client-1.0.8/chittorgarh_client/utils.py` & `chittorgarh_client-1.0.9/chittorgarh_client/utils.py`

 * *Files identical despite different names*

