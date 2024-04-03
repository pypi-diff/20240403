# Comparing `tmp/st_common_data-0.2.9.7.tar.gz` & `tmp/st_common_data-0.2.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_common_data-0.2.9.7.tar", last modified: Mon Mar 18 12:38:04 2024, max compression
+gzip compressed data, was "st_common_data-0.2.9.8.tar", last modified: Wed Apr  3 14:34:36 2024, max compression
```

## Comparing `st_common_data-0.2.9.7.tar` & `st_common_data-0.2.9.8.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-03-18 12:38:04.925288 st_common_data-0.2.9.7/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.9.7/LICENCE
--rw-r--r--   0 bayraktar  (1000) bayraktar  (1000)     1224 2024-03-18 12:38:04.925288 st_common_data-0.2.9.7/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      648 2024-01-03 16:21:08.000000 st_common_data-0.2.9.7/README.md
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.9.7/pyproject.toml
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2024-03-18 12:38:04.925288 st_common_data-0.2.9.7/setup.cfg
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-03-18 12:38:04.917288 st_common_data-0.2.9.7/st_common_data/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2024-03-18 11:52:18.000000 st_common_data-0.2.9.7/st_common_data/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-03-18 12:38:04.921288 st_common_data-0.2.9.7/st_common_data/auth/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.9.7/st_common_data/auth/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.9.7/st_common_data/auth/apps.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10938 2024-03-18 12:37:09.000000 st_common_data-0.2.9.7/st_common_data/auth/django_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.9.7/st_common_data/auth/fastapi_auth.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.9.7/st_common_data/auth/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.9.7/st_common_data/auth/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4086 2024-01-11 11:51:04.000000 st_common_data-0.2.9.7/st_common_data/auth/views.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    33901 2024-01-03 12:58:10.000000 st_common_data-0.2.9.7/st_common_data/datum.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.9.7/st_common_data/pagination.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-03-18 12:38:04.921288 st_common_data-0.2.9.7/st_common_data/trading_accounts/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/__init__.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-03-18 12:38:04.921288 st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0001_initial.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      539 2023-11-20 18:32:49.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      541 2024-03-12 13:41:45.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3625 2024-03-12 13:41:45.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/models.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/serializers.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/urls.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.9.7/st_common_data/trading_accounts/views.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-03-18 12:38:04.925288 st_common_data-0.2.9.7/st_common_data/utils/
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.9.7/st_common_data/utils/__init__.py
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4885 2024-01-03 17:13:10.000000 st_common_data-0.2.9.7/st_common_data/utils/common.py
-drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-03-18 12:38:04.925288 st_common_data-0.2.9.7/st_common_data.egg-info/
--rw-r--r--   0 bayraktar  (1000) bayraktar  (1000)     1224 2024-03-18 12:38:04.000000 st_common_data-0.2.9.7/st_common_data.egg-info/PKG-INFO
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1197 2024-03-18 12:38:04.000000 st_common_data-0.2.9.7/st_common_data.egg-info/SOURCES.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2024-03-18 12:38:04.000000 st_common_data-0.2.9.7/st_common_data.egg-info/dependency_links.txt
--rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2024-03-18 12:38:04.000000 st_common_data-0.2.9.7/st_common_data.egg-info/top_level.txt
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1073 2022-04-19 17:26:26.000000 st_common_data-0.2.9.8/LICENCE
+-rw-r--r--   0 bayraktar  (1000) bayraktar  (1000)     1224 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      648 2024-01-03 16:21:08.000000 st_common_data-0.2.9.8/README.md
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      103 2022-04-19 17:26:26.000000 st_common_data-0.2.9.8/pyproject.toml
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      669 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/setup.cfg
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.215991 st_common_data-0.2.9.8/st_common_data/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      143 2024-04-03 14:34:31.000000 st_common_data-0.2.9.8/st_common_data/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.215991 st_common_data-0.2.9.8/st_common_data/auth/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      443 2023-04-11 10:31:33.000000 st_common_data-0.2.9.8/st_common_data/auth/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      118 2022-12-07 11:03:09.000000 st_common_data-0.2.9.8/st_common_data/auth/apps.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10938 2024-03-18 12:37:09.000000 st_common_data-0.2.9.8/st_common_data/auth/django_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    10009 2023-04-18 06:48:02.000000 st_common_data-0.2.9.8/st_common_data/auth/fastapi_auth.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      386 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/auth/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      278 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/auth/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4086 2024-01-11 11:51:04.000000 st_common_data-0.2.9.8/st_common_data/auth/views.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)    34092 2024-04-03 14:26:00.000000 st_common_data-0.2.9.8/st_common_data/datum.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      398 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/pagination.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.215991 st_common_data-0.2.9.8/st_common_data/trading_accounts/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/__init__.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4299 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0001_initial.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      652 2023-02-24 09:24:45.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      456 2023-03-22 00:17:46.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0003_tradingaccount_personal_status.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      539 2023-11-20 18:32:49.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      541 2024-03-12 13:41:45.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     3625 2024-03-12 13:41:45.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/models.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      214 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/serializers.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)      200 2022-08-23 10:22:22.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/urls.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4193 2022-12-07 11:03:09.000000 st_common_data-0.2.9.8/st_common_data/trading_accounts/views.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/st_common_data/utils/
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        0 2022-07-21 20:22:31.000000 st_common_data-0.2.9.8/st_common_data/utils/__init__.py
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     4885 2024-01-03 17:13:10.000000 st_common_data-0.2.9.8/st_common_data/utils/common.py
+drwxrwxr-x   0 bayraktar  (1000) bayraktar  (1000)        0 2024-04-03 14:34:36.219991 st_common_data-0.2.9.8/st_common_data.egg-info/
+-rw-r--r--   0 bayraktar  (1000) bayraktar  (1000)     1224 2024-04-03 14:34:36.000000 st_common_data-0.2.9.8/st_common_data.egg-info/PKG-INFO
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)     1197 2024-04-03 14:34:36.000000 st_common_data-0.2.9.8/st_common_data.egg-info/SOURCES.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)        1 2024-04-03 14:34:36.000000 st_common_data-0.2.9.8/st_common_data.egg-info/dependency_links.txt
+-rw-rw-r--   0 bayraktar  (1000) bayraktar  (1000)       15 2024-04-03 14:34:36.000000 st_common_data-0.2.9.8/st_common_data.egg-info/top_level.txt
```

### Comparing `st_common_data-0.2.9.7/LICENCE` & `st_common_data-0.2.9.8/LICENCE`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/PKG-INFO` & `st_common_data-0.2.9.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_common_data
-Version: 0.2.9.7
+Version: 0.2.9.8
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.9.7/README.md` & `st_common_data-0.2.9.8/README.md`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/setup.cfg` & `st_common_data-0.2.9.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/auth/django_auth.py` & `st_common_data-0.2.9.8/st_common_data/auth/django_auth.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/auth/fastapi_auth.py` & `st_common_data-0.2.9.8/st_common_data/auth/fastapi_auth.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/auth/views.py` & `st_common_data-0.2.9.8/st_common_data/auth/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/datum.py` & `st_common_data-0.2.9.8/st_common_data/datum.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,19 +456,23 @@
         )
 
         date_from = intermediate_date + datetime.timedelta(days=1)
 
     return result
 
 
-def api_get_ptp_tickers(datum_api_url: str, service_auth0_token: str):
-    return datum_api_get_request(
-        url=f'{datum_api_url}/tickers/sorters/ptp',
+def api_get_ptp_tickers(datum_api_url: str, service_auth0_token: str) -> Dict[str, list]:
+    datum_response = datum_api_get_request(
+        url=f'{datum_api_url}/tickers/all_ptps',
         service_auth0_token=service_auth0_token
     )
+    tickers_by_sorter = defaultdict(list)
+    for row in datum_response:
+        tickers_by_sorter[row['sorter']].append(row['ticker'])
+    return tickers_by_sorter
 
 
 def api_get_tickers_changes(datum_api_url: str,
                             service_auth0_token: str,
                             start_eff_date: str,
                             end_eff_date: str,
                             ):
```

### Comparing `st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0001_initial.py` & `st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py` & `st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0002_tradingaccount_first_user.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py` & `st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0004_tradingaccount_platform.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py` & `st_common_data-0.2.9.8/st_common_data/trading_accounts/migrations/0005_tradingaccount_routing.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/trading_accounts/models.py` & `st_common_data-0.2.9.8/st_common_data/trading_accounts/models.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/trading_accounts/views.py` & `st_common_data-0.2.9.8/st_common_data/trading_accounts/views.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data/utils/common.py` & `st_common_data-0.2.9.8/st_common_data/utils/common.py`

 * *Files identical despite different names*

### Comparing `st_common_data-0.2.9.7/st_common_data.egg-info/PKG-INFO` & `st_common_data-0.2.9.8/st_common_data.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st_common_data
-Version: 0.2.9.7
+Version: 0.2.9.8
 Summary: Data that is used in different ST projects
 Home-page: https://github.com/ivanovds/st_common_data
 Author: Daniil Ivanov
 Author-email: danil.98and@gmail.com
 Project-URL: Bug Tracker, https://github.com/ivanovds/st_common_data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Web Environment
```

### Comparing `st_common_data-0.2.9.7/st_common_data.egg-info/SOURCES.txt` & `st_common_data-0.2.9.8/st_common_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

