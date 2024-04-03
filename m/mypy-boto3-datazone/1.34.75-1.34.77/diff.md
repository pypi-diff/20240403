# Comparing `tmp/mypy-boto3-datazone-1.34.75.tar.gz` & `tmp/mypy-boto3-datazone-1.34.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-datazone-1.34.75.tar", last modified: Mon Apr  1 20:08:26 2024, max compression
+gzip compressed data, was "mypy-boto3-datazone-1.34.77.tar", last modified: Wed Apr  3 19:32:38 2024, max compression
```

## Comparing `mypy-boto3-datazone-1.34.75.tar` & `mypy-boto3-datazone-1.34.77.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.585728 mypy-boto3-datazone-1.34.75/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-01 20:08:26.585728 mypy-boto3-datazone-1.34.75/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.581728 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5320 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    82303 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    82300 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18591 2024-04-01 20:07:59.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    18591 2024-04-01 20:07:59.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29487 2024-04-01 20:07:59.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    29464 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   123413 2024-04-01 20:08:01.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   123413 2024-04-01 20:08:01.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 20:08:26.585728 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15889 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-01 20:08:26.000000 mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 20:08:26.585728 mypy-boto3-datazone-1.34.75/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-01 20:07:58.000000 mypy-boto3-datazone-1.34.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.852162 mypy-boto3-datazone-1.34.77/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-03 19:32:38.852162 mypy-boto3-datazone-1.34.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.852162 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85890 2024-04-03 19:32:05.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85887 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-03 19:32:06.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18871 2024-04-03 19:32:06.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    30969 2024-04-03 19:32:05.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30945 2024-04-03 19:32:05.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   128604 2024-04-03 19:32:08.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   128604 2024-04-03 19:32:07.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:32:38.852162 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16063 2024-04-03 19:32:38.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-03 19:32:38.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:38.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:32:38.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 19:32:38.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 19:32:38.000000 mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:32:38.852162 mypy-boto3-datazone-1.34.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-04-03 19:32:04.000000 mypy-boto3-datazone-1.34.77/setup.py
```

### Comparing `mypy-boto3-datazone-1.34.75/LICENSE` & `mypy-boto3-datazone-1.34.77/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datazone-1.34.75/PKG-INFO` & `mypy-boto3-datazone-1.34.77/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datazone
-Version: 1.34.75
-Summary: Type annotations for boto3.DataZone 1.34.75 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.DataZone 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datazone.svg?color=blue)](https://pypi.org/project/mypy-boto3-datazone)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datazone)](https://pepy.tech/project/mypy-boto3-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataZone 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[boto3.DataZone 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -297,14 +297,15 @@
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionTargetsPaginator,
     ListSubscriptionsPaginator,
+    ListTimeSeriesDataPointsPaginator,
     SearchPaginator,
     SearchGroupProfilesPaginator,
     SearchListingsPaginator,
     SearchTypesPaginator,
     SearchUserProfilesPaginator,
 )
 
@@ -351,14 +352,17 @@
 )
 list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator(
     "list_subscription_targets"
 )
 list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator(
     "list_subscriptions"
 )
+list_time_series_data_points_paginator: ListTimeSeriesDataPointsPaginator = client.get_paginator(
+    "list_time_series_data_points"
+)
 search_paginator: SearchPaginator = client.get_paginator("search")
 search_group_profiles_paginator: SearchGroupProfilesPaginator = client.get_paginator(
     "search_group_profiles"
 )
 search_listings_paginator: SearchListingsPaginator = client.get_paginator("search_listings")
 search_types_paginator: SearchTypesPaginator = client.get_paginator("search_types")
 search_user_profiles_paginator: SearchUserProfilesPaginator = client.get_paginator(
```

### Comparing `mypy-boto3-datazone-1.34.75/README.md` & `mypy-boto3-datazone-1.34.77/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datazone.svg?color=blue)](https://pypi.org/project/mypy-boto3-datazone)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datazone)](https://pepy.tech/project/mypy-boto3-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataZone 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[boto3.DataZone 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -264,14 +264,15 @@
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionTargetsPaginator,
     ListSubscriptionsPaginator,
+    ListTimeSeriesDataPointsPaginator,
     SearchPaginator,
     SearchGroupProfilesPaginator,
     SearchListingsPaginator,
     SearchTypesPaginator,
     SearchUserProfilesPaginator,
 )
 
@@ -318,14 +319,17 @@
 )
 list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator(
     "list_subscription_targets"
 )
 list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator(
     "list_subscriptions"
 )
+list_time_series_data_points_paginator: ListTimeSeriesDataPointsPaginator = client.get_paginator(
+    "list_time_series_data_points"
+)
 search_paginator: SearchPaginator = client.get_paginator("search")
 search_group_profiles_paginator: SearchGroupProfilesPaginator = client.get_paginator(
     "search_group_profiles"
 )
 search_listings_paginator: SearchListingsPaginator = client.get_paginator("search_listings")
 search_types_paginator: SearchTypesPaginator = client.get_paginator("search_types")
 search_user_profiles_paginator: SearchUserProfilesPaginator = client.get_paginator(
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__init__.py` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         ListNotificationsPaginator,
         ListProjectMembershipsPaginator,
         ListProjectsPaginator,
         ListSubscriptionGrantsPaginator,
         ListSubscriptionRequestsPaginator,
         ListSubscriptionTargetsPaginator,
         ListSubscriptionsPaginator,
+        ListTimeSeriesDataPointsPaginator,
         SearchGroupProfilesPaginator,
         SearchListingsPaginator,
         SearchPaginator,
         SearchTypesPaginator,
         SearchUserProfilesPaginator,
     )
 
@@ -48,14 +49,15 @@
     list_notifications_paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")
     list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_subscription_grants_paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")
     list_subscription_requests_paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")
     list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")
     list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
+    list_time_series_data_points_paginator: ListTimeSeriesDataPointsPaginator = client.get_paginator("list_time_series_data_points")
     search_paginator: SearchPaginator = client.get_paginator("search")
     search_group_profiles_paginator: SearchGroupProfilesPaginator = client.get_paginator("search_group_profiles")
     search_listings_paginator: SearchListingsPaginator = client.get_paginator("search_listings")
     search_types_paginator: SearchTypesPaginator = client.get_paginator("search_types")
     search_user_profiles_paginator: SearchUserProfilesPaginator = client.get_paginator("search_user_profiles")
     ```
 """
@@ -75,14 +77,15 @@
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionsPaginator,
     ListSubscriptionTargetsPaginator,
+    ListTimeSeriesDataPointsPaginator,
     SearchGroupProfilesPaginator,
     SearchListingsPaginator,
     SearchPaginator,
     SearchTypesPaginator,
     SearchUserProfilesPaginator,
 )
 
@@ -104,13 +107,14 @@
     "ListNotificationsPaginator",
     "ListProjectMembershipsPaginator",
     "ListProjectsPaginator",
     "ListSubscriptionGrantsPaginator",
     "ListSubscriptionRequestsPaginator",
     "ListSubscriptionTargetsPaginator",
     "ListSubscriptionsPaginator",
+    "ListTimeSeriesDataPointsPaginator",
     "SearchGroupProfilesPaginator",
     "SearchListingsPaginator",
     "SearchPaginator",
     "SearchTypesPaginator",
     "SearchUserProfilesPaginator",
 )
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__init__.pyi` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         ListNotificationsPaginator,
         ListProjectMembershipsPaginator,
         ListProjectsPaginator,
         ListSubscriptionGrantsPaginator,
         ListSubscriptionRequestsPaginator,
         ListSubscriptionTargetsPaginator,
         ListSubscriptionsPaginator,
+        ListTimeSeriesDataPointsPaginator,
         SearchGroupProfilesPaginator,
         SearchListingsPaginator,
         SearchPaginator,
         SearchTypesPaginator,
         SearchUserProfilesPaginator,
     )
 
@@ -48,14 +49,15 @@
     list_notifications_paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")
     list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_subscription_grants_paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")
     list_subscription_requests_paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")
     list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")
     list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
+    list_time_series_data_points_paginator: ListTimeSeriesDataPointsPaginator = client.get_paginator("list_time_series_data_points")
     search_paginator: SearchPaginator = client.get_paginator("search")
     search_group_profiles_paginator: SearchGroupProfilesPaginator = client.get_paginator("search_group_profiles")
     search_listings_paginator: SearchListingsPaginator = client.get_paginator("search_listings")
     search_types_paginator: SearchTypesPaginator = client.get_paginator("search_types")
     search_user_profiles_paginator: SearchUserProfilesPaginator = client.get_paginator("search_user_profiles")
     ```
 """
@@ -75,14 +77,15 @@
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionsPaginator,
     ListSubscriptionTargetsPaginator,
+    ListTimeSeriesDataPointsPaginator,
     SearchGroupProfilesPaginator,
     SearchListingsPaginator,
     SearchPaginator,
     SearchTypesPaginator,
     SearchUserProfilesPaginator,
 )
 
@@ -104,13 +107,14 @@
     "ListNotificationsPaginator",
     "ListProjectMembershipsPaginator",
     "ListProjectsPaginator",
     "ListSubscriptionGrantsPaginator",
     "ListSubscriptionRequestsPaginator",
     "ListSubscriptionTargetsPaginator",
     "ListSubscriptionsPaginator",
+    "ListTimeSeriesDataPointsPaginator",
     "SearchGroupProfilesPaginator",
     "SearchListingsPaginator",
     "SearchPaginator",
     "SearchTypesPaginator",
     "SearchUserProfilesPaginator",
 )
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/__main__.py` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.DataZone 1.34.75\n"
-        "Version:         1.34.75\n"
+        "Type annotations for boto3.DataZone 1.34.77\n"
+        "Version:         1.34.77\n"
         "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.75")
+    print("1.34.77")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/client.py` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     GlossaryStatusType,
     GlossaryTermStatusType,
     GroupProfileStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
     MetadataGenerationRunStatusType,
     NotificationTypeType,
+    SearchOutputAdditionalAttributeType,
     SortKeyType,
     SortOrderType,
     SubscriptionGrantStatusType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
+    TimeSeriesEntityTypeType,
     TypesSearchScopeType,
     UserDesignationType,
     UserProfileStatusType,
     UserProfileTypeType,
     UserSearchTypeType,
     UserTypeType,
 )
@@ -62,14 +64,15 @@
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionsPaginator,
     ListSubscriptionTargetsPaginator,
+    ListTimeSeriesDataPointsPaginator,
     SearchGroupProfilesPaginator,
     SearchListingsPaginator,
     SearchPaginator,
     SearchTypesPaginator,
     SearchUserProfilesPaginator,
 )
 from .type_defs import (
@@ -123,14 +126,15 @@
     GetListingOutputTypeDef,
     GetMetadataGenerationRunOutputTypeDef,
     GetProjectOutputTypeDef,
     GetSubscriptionGrantOutputTypeDef,
     GetSubscriptionOutputTypeDef,
     GetSubscriptionRequestDetailsOutputTypeDef,
     GetSubscriptionTargetOutputTypeDef,
+    GetTimeSeriesDataPointOutputTypeDef,
     GetUserProfileOutputTypeDef,
     GrantedEntityInputTypeDef,
     ListAssetRevisionsOutputTypeDef,
     ListDataSourceRunActivitiesOutputTypeDef,
     ListDataSourceRunsOutputTypeDef,
     ListDataSourcesOutputTypeDef,
     ListDomainsOutputTypeDef,
@@ -143,17 +147,19 @@
     ListProjectMembershipsOutputTypeDef,
     ListProjectsOutputTypeDef,
     ListSubscriptionGrantsOutputTypeDef,
     ListSubscriptionRequestsOutputTypeDef,
     ListSubscriptionsOutputTypeDef,
     ListSubscriptionTargetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListTimeSeriesDataPointsOutputTypeDef,
     MemberTypeDef,
     MetadataGenerationRunTargetTypeDef,
     ModelTypeDef,
+    PostTimeSeriesDataPointsOutputTypeDef,
     PredictionConfigurationTypeDef,
     PutEnvironmentBlueprintConfigurationOutputTypeDef,
     RecommendationConfigurationTypeDef,
     RejectChoiceTypeDef,
     RejectPredictionsOutputTypeDef,
     RejectRuleTypeDef,
     RejectSubscriptionRequestOutputTypeDef,
@@ -169,14 +175,15 @@
     SingleSignOnTypeDef,
     StartDataSourceRunOutputTypeDef,
     StartMetadataGenerationRunOutputTypeDef,
     SubscribedListingInputTypeDef,
     SubscribedPrincipalInputTypeDef,
     SubscriptionTargetFormTypeDef,
     TermRelationsTypeDef,
+    TimeSeriesDataPointFormInputTypeDef,
     TimestampTypeDef,
     UpdateDataSourceOutputTypeDef,
     UpdateDomainOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateEnvironmentProfileOutputTypeDef,
     UpdateGlossaryOutputTypeDef,
     UpdateGlossaryTermOutputTypeDef,
@@ -760,14 +767,30 @@
         """
         Deletes a subscription target in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_subscription_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#delete_subscription_target)
         """
 
+    def delete_time_series_data_points(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        formName: str,
+        clientToken: str = ...,
+    ) -> Dict[str, Any]:
+        """
+        Deletes the specified time series form for the specified asset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_time_series_data_points)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#delete_time_series_data_points)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -978,14 +1001,30 @@
         """
         Gets the subscription target in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_subscription_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_subscription_target)
         """
 
+    def get_time_series_data_point(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        formName: str,
+        identifier: str,
+    ) -> GetTimeSeriesDataPointOutputTypeDef:
+        """
+        Gets the existing data point for the asset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_time_series_data_point)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_time_series_data_point)
+        """
+
     def get_user_profile(
         self, *, domainIdentifier: str, userIdentifier: str, type: UserProfileTypeType = ...
     ) -> GetUserProfileOutputTypeDef:
         """
         Gets a user profile in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_user_profile)
@@ -1281,14 +1320,49 @@
         """
         Lists tags for the specified resource in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#list_tags_for_resource)
         """
 
+    def list_time_series_data_points(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        formName: str,
+        endedAt: TimestampTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        startedAt: TimestampTypeDef = ...,
+    ) -> ListTimeSeriesDataPointsOutputTypeDef:
+        """
+        Lists time series data points.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_time_series_data_points)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#list_time_series_data_points)
+        """
+
+    def post_time_series_data_points(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        forms: Sequence[TimeSeriesDataPointFormInputTypeDef],
+        clientToken: str = ...,
+    ) -> PostTimeSeriesDataPointsOutputTypeDef:
+        """
+        Posts time series data points to Amazon DataZone for the specified asset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.post_time_series_data_points)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#post_time_series_data_points)
+        """
+
     def put_environment_blueprint_configuration(
         self,
         *,
         domainIdentifier: str,
         enabledRegions: Sequence[str],
         environmentBlueprintIdentifier: str,
         manageAccessRoleArn: str = ...,
@@ -1343,15 +1417,15 @@
         """
 
     def search(
         self,
         *,
         domainIdentifier: str,
         searchScope: InventorySearchScopeType,
-        additionalAttributes: Sequence[Literal["FORMS"]] = ...,
+        additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         owningProjectIdentifier: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
@@ -1379,15 +1453,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#search_group_profiles)
         """
 
     def search_listings(
         self,
         *,
         domainIdentifier: str,
-        additionalAttributes: Sequence[Literal["FORMS"]] = ...,
+        additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
     ) -> SearchListingsOutputTypeDef:
@@ -1819,14 +1893,23 @@
     ) -> ListSubscriptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_time_series_data_points"]
+    ) -> ListTimeSeriesDataPointsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["search"]) -> SearchPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/client.pyi` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -31,20 +31,22 @@
     GlossaryStatusType,
     GlossaryTermStatusType,
     GroupProfileStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
     MetadataGenerationRunStatusType,
     NotificationTypeType,
+    SearchOutputAdditionalAttributeType,
     SortKeyType,
     SortOrderType,
     SubscriptionGrantStatusType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
+    TimeSeriesEntityTypeType,
     TypesSearchScopeType,
     UserDesignationType,
     UserProfileStatusType,
     UserProfileTypeType,
     UserSearchTypeType,
     UserTypeType,
 )
@@ -62,14 +64,15 @@
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionsPaginator,
     ListSubscriptionTargetsPaginator,
+    ListTimeSeriesDataPointsPaginator,
     SearchGroupProfilesPaginator,
     SearchListingsPaginator,
     SearchPaginator,
     SearchTypesPaginator,
     SearchUserProfilesPaginator,
 )
 from .type_defs import (
@@ -123,14 +126,15 @@
     GetListingOutputTypeDef,
     GetMetadataGenerationRunOutputTypeDef,
     GetProjectOutputTypeDef,
     GetSubscriptionGrantOutputTypeDef,
     GetSubscriptionOutputTypeDef,
     GetSubscriptionRequestDetailsOutputTypeDef,
     GetSubscriptionTargetOutputTypeDef,
+    GetTimeSeriesDataPointOutputTypeDef,
     GetUserProfileOutputTypeDef,
     GrantedEntityInputTypeDef,
     ListAssetRevisionsOutputTypeDef,
     ListDataSourceRunActivitiesOutputTypeDef,
     ListDataSourceRunsOutputTypeDef,
     ListDataSourcesOutputTypeDef,
     ListDomainsOutputTypeDef,
@@ -143,17 +147,19 @@
     ListProjectMembershipsOutputTypeDef,
     ListProjectsOutputTypeDef,
     ListSubscriptionGrantsOutputTypeDef,
     ListSubscriptionRequestsOutputTypeDef,
     ListSubscriptionsOutputTypeDef,
     ListSubscriptionTargetsOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ListTimeSeriesDataPointsOutputTypeDef,
     MemberTypeDef,
     MetadataGenerationRunTargetTypeDef,
     ModelTypeDef,
+    PostTimeSeriesDataPointsOutputTypeDef,
     PredictionConfigurationTypeDef,
     PutEnvironmentBlueprintConfigurationOutputTypeDef,
     RecommendationConfigurationTypeDef,
     RejectChoiceTypeDef,
     RejectPredictionsOutputTypeDef,
     RejectRuleTypeDef,
     RejectSubscriptionRequestOutputTypeDef,
@@ -169,14 +175,15 @@
     SingleSignOnTypeDef,
     StartDataSourceRunOutputTypeDef,
     StartMetadataGenerationRunOutputTypeDef,
     SubscribedListingInputTypeDef,
     SubscribedPrincipalInputTypeDef,
     SubscriptionTargetFormTypeDef,
     TermRelationsTypeDef,
+    TimeSeriesDataPointFormInputTypeDef,
     TimestampTypeDef,
     UpdateDataSourceOutputTypeDef,
     UpdateDomainOutputTypeDef,
     UpdateEnvironmentOutputTypeDef,
     UpdateEnvironmentProfileOutputTypeDef,
     UpdateGlossaryOutputTypeDef,
     UpdateGlossaryTermOutputTypeDef,
@@ -757,14 +764,30 @@
         """
         Deletes a subscription target in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_subscription_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#delete_subscription_target)
         """
 
+    def delete_time_series_data_points(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        formName: str,
+        clientToken: str = ...,
+    ) -> Dict[str, Any]:
+        """
+        Deletes the specified time series form for the specified asset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.delete_time_series_data_points)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#delete_time_series_data_points)
+        """
+
     def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
@@ -975,14 +998,30 @@
         """
         Gets the subscription target in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_subscription_target)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_subscription_target)
         """
 
+    def get_time_series_data_point(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        formName: str,
+        identifier: str,
+    ) -> GetTimeSeriesDataPointOutputTypeDef:
+        """
+        Gets the existing data point for the asset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_time_series_data_point)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_time_series_data_point)
+        """
+
     def get_user_profile(
         self, *, domainIdentifier: str, userIdentifier: str, type: UserProfileTypeType = ...
     ) -> GetUserProfileOutputTypeDef:
         """
         Gets a user profile in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_user_profile)
@@ -1278,14 +1317,49 @@
         """
         Lists tags for the specified resource in Amazon DataZone.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_tags_for_resource)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#list_tags_for_resource)
         """
 
+    def list_time_series_data_points(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        formName: str,
+        endedAt: TimestampTypeDef = ...,
+        maxResults: int = ...,
+        nextToken: str = ...,
+        startedAt: TimestampTypeDef = ...,
+    ) -> ListTimeSeriesDataPointsOutputTypeDef:
+        """
+        Lists time series data points.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.list_time_series_data_points)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#list_time_series_data_points)
+        """
+
+    def post_time_series_data_points(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        forms: Sequence[TimeSeriesDataPointFormInputTypeDef],
+        clientToken: str = ...,
+    ) -> PostTimeSeriesDataPointsOutputTypeDef:
+        """
+        Posts time series data points to Amazon DataZone for the specified asset.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.post_time_series_data_points)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#post_time_series_data_points)
+        """
+
     def put_environment_blueprint_configuration(
         self,
         *,
         domainIdentifier: str,
         enabledRegions: Sequence[str],
         environmentBlueprintIdentifier: str,
         manageAccessRoleArn: str = ...,
@@ -1340,15 +1414,15 @@
         """
 
     def search(
         self,
         *,
         domainIdentifier: str,
         searchScope: InventorySearchScopeType,
-        additionalAttributes: Sequence[Literal["FORMS"]] = ...,
+        additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         owningProjectIdentifier: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
@@ -1376,15 +1450,15 @@
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#search_group_profiles)
         """
 
     def search_listings(
         self,
         *,
         domainIdentifier: str,
-        additionalAttributes: Sequence[Literal["FORMS"]] = ...,
+        additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,
         filters: "FilterClauseTypeDef" = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
     ) -> SearchListingsOutputTypeDef:
@@ -1816,14 +1890,23 @@
     ) -> ListSubscriptionsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
         """
 
     @overload
+    def get_paginator(
+        self, operation_name: Literal["list_time_series_data_points"]
+    ) -> ListTimeSeriesDataPointsPaginator:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
+        """
+
+    @overload
     def get_paginator(self, operation_name: Literal["search"]) -> SearchPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Client.get_paginator)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/client/#get_paginator)
         """
 
     @overload
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/literals.py` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "ListNotificationsPaginatorName",
     "ListProjectMembershipsPaginatorName",
     "ListProjectsPaginatorName",
     "ListSubscriptionGrantsPaginatorName",
     "ListSubscriptionRequestsPaginatorName",
     "ListSubscriptionTargetsPaginatorName",
     "ListSubscriptionsPaginatorName",
+    "ListTimeSeriesDataPointsPaginatorName",
     "ListingStatusType",
     "MetadataGenerationRunStatusType",
     "MetadataGenerationRunTypeType",
     "MetadataGenerationTargetTypeType",
     "NotificationResourceTypeType",
     "NotificationRoleType",
     "NotificationTypeType",
@@ -78,14 +79,15 @@
     "SortKeyType",
     "SortOrderType",
     "SubscriptionGrantOverallStatusType",
     "SubscriptionGrantStatusType",
     "SubscriptionRequestStatusType",
     "SubscriptionStatusType",
     "TaskStatusType",
+    "TimeSeriesEntityTypeType",
     "TimezoneType",
     "TypesSearchScopeType",
     "UserAssignmentType",
     "UserDesignationType",
     "UserProfileStatusType",
     "UserProfileTypeType",
     "UserSearchTypeType",
@@ -178,14 +180,15 @@
 ListNotificationsPaginatorName = Literal["list_notifications"]
 ListProjectMembershipsPaginatorName = Literal["list_project_memberships"]
 ListProjectsPaginatorName = Literal["list_projects"]
 ListSubscriptionGrantsPaginatorName = Literal["list_subscription_grants"]
 ListSubscriptionRequestsPaginatorName = Literal["list_subscription_requests"]
 ListSubscriptionTargetsPaginatorName = Literal["list_subscription_targets"]
 ListSubscriptionsPaginatorName = Literal["list_subscriptions"]
+ListTimeSeriesDataPointsPaginatorName = Literal["list_time_series_data_points"]
 ListingStatusType = Literal["ACTIVE", "CREATING", "INACTIVE"]
 MetadataGenerationRunStatusType = Literal[
     "CANCELED", "FAILED", "IN_PROGRESS", "SUBMITTED", "SUCCEEDED"
 ]
 MetadataGenerationRunTypeType = Literal["BUSINESS_DESCRIPTIONS"]
 MetadataGenerationTargetTypeType = Literal["ASSET"]
 NotificationResourceTypeType = Literal["PROJECT"]
@@ -193,15 +196,15 @@
     "DOMAIN_OWNER", "PROJECT_CONTRIBUTOR", "PROJECT_OWNER", "PROJECT_SUBSCRIBER", "PROJECT_VIEWER"
 ]
 NotificationTypeType = Literal["EVENT", "TASK"]
 ProjectStatusType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 RejectRuleBehaviorType = Literal["ALL", "NONE"]
 SearchGroupProfilesPaginatorName = Literal["search_group_profiles"]
 SearchListingsPaginatorName = Literal["search_listings"]
-SearchOutputAdditionalAttributeType = Literal["FORMS"]
+SearchOutputAdditionalAttributeType = Literal["FORMS", "TIME_SERIES_DATA_POINT_FORMS"]
 SearchPaginatorName = Literal["search"]
 SearchTypesPaginatorName = Literal["search_types"]
 SearchUserProfilesPaginatorName = Literal["search_user_profiles"]
 SortFieldProjectType = Literal["NAME"]
 SortKeyType = Literal["CREATED_AT", "UPDATED_AT"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
 SubscriptionGrantOverallStatusType = Literal[
@@ -222,14 +225,15 @@
     "REVOKE_FAILED",
     "REVOKE_IN_PROGRESS",
     "REVOKE_PENDING",
 ]
 SubscriptionRequestStatusType = Literal["ACCEPTED", "PENDING", "REJECTED"]
 SubscriptionStatusType = Literal["APPROVED", "CANCELLED", "REVOKED"]
 TaskStatusType = Literal["ACTIVE", "INACTIVE"]
+TimeSeriesEntityTypeType = Literal["ASSET", "LISTING"]
 TimezoneType = Literal[
     "AFRICA_JOHANNESBURG",
     "AMERICA_MONTREAL",
     "AMERICA_SAO_PAULO",
     "ASIA_BAHRAIN",
     "ASIA_BANGKOK",
     "ASIA_CALCUTTA",
@@ -709,14 +713,15 @@
     "list_notifications",
     "list_project_memberships",
     "list_projects",
     "list_subscription_grants",
     "list_subscription_requests",
     "list_subscription_targets",
     "list_subscriptions",
+    "list_time_series_data_points",
     "search",
     "search_group_profiles",
     "search_listings",
     "search_types",
     "search_user_profiles",
 ]
 RegionName = Literal[
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/literals.pyi` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "ListNotificationsPaginatorName",
     "ListProjectMembershipsPaginatorName",
     "ListProjectsPaginatorName",
     "ListSubscriptionGrantsPaginatorName",
     "ListSubscriptionRequestsPaginatorName",
     "ListSubscriptionTargetsPaginatorName",
     "ListSubscriptionsPaginatorName",
+    "ListTimeSeriesDataPointsPaginatorName",
     "ListingStatusType",
     "MetadataGenerationRunStatusType",
     "MetadataGenerationRunTypeType",
     "MetadataGenerationTargetTypeType",
     "NotificationResourceTypeType",
     "NotificationRoleType",
     "NotificationTypeType",
@@ -78,14 +79,15 @@
     "SortKeyType",
     "SortOrderType",
     "SubscriptionGrantOverallStatusType",
     "SubscriptionGrantStatusType",
     "SubscriptionRequestStatusType",
     "SubscriptionStatusType",
     "TaskStatusType",
+    "TimeSeriesEntityTypeType",
     "TimezoneType",
     "TypesSearchScopeType",
     "UserAssignmentType",
     "UserDesignationType",
     "UserProfileStatusType",
     "UserProfileTypeType",
     "UserSearchTypeType",
@@ -178,14 +180,15 @@
 ListNotificationsPaginatorName = Literal["list_notifications"]
 ListProjectMembershipsPaginatorName = Literal["list_project_memberships"]
 ListProjectsPaginatorName = Literal["list_projects"]
 ListSubscriptionGrantsPaginatorName = Literal["list_subscription_grants"]
 ListSubscriptionRequestsPaginatorName = Literal["list_subscription_requests"]
 ListSubscriptionTargetsPaginatorName = Literal["list_subscription_targets"]
 ListSubscriptionsPaginatorName = Literal["list_subscriptions"]
+ListTimeSeriesDataPointsPaginatorName = Literal["list_time_series_data_points"]
 ListingStatusType = Literal["ACTIVE", "CREATING", "INACTIVE"]
 MetadataGenerationRunStatusType = Literal[
     "CANCELED", "FAILED", "IN_PROGRESS", "SUBMITTED", "SUCCEEDED"
 ]
 MetadataGenerationRunTypeType = Literal["BUSINESS_DESCRIPTIONS"]
 MetadataGenerationTargetTypeType = Literal["ASSET"]
 NotificationResourceTypeType = Literal["PROJECT"]
@@ -193,15 +196,15 @@
     "DOMAIN_OWNER", "PROJECT_CONTRIBUTOR", "PROJECT_OWNER", "PROJECT_SUBSCRIBER", "PROJECT_VIEWER"
 ]
 NotificationTypeType = Literal["EVENT", "TASK"]
 ProjectStatusType = Literal["ACTIVE", "DELETE_FAILED", "DELETING"]
 RejectRuleBehaviorType = Literal["ALL", "NONE"]
 SearchGroupProfilesPaginatorName = Literal["search_group_profiles"]
 SearchListingsPaginatorName = Literal["search_listings"]
-SearchOutputAdditionalAttributeType = Literal["FORMS"]
+SearchOutputAdditionalAttributeType = Literal["FORMS", "TIME_SERIES_DATA_POINT_FORMS"]
 SearchPaginatorName = Literal["search"]
 SearchTypesPaginatorName = Literal["search_types"]
 SearchUserProfilesPaginatorName = Literal["search_user_profiles"]
 SortFieldProjectType = Literal["NAME"]
 SortKeyType = Literal["CREATED_AT", "UPDATED_AT"]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
 SubscriptionGrantOverallStatusType = Literal[
@@ -222,14 +225,15 @@
     "REVOKE_FAILED",
     "REVOKE_IN_PROGRESS",
     "REVOKE_PENDING",
 ]
 SubscriptionRequestStatusType = Literal["ACCEPTED", "PENDING", "REJECTED"]
 SubscriptionStatusType = Literal["APPROVED", "CANCELLED", "REVOKED"]
 TaskStatusType = Literal["ACTIVE", "INACTIVE"]
+TimeSeriesEntityTypeType = Literal["ASSET", "LISTING"]
 TimezoneType = Literal[
     "AFRICA_JOHANNESBURG",
     "AMERICA_MONTREAL",
     "AMERICA_SAO_PAULO",
     "ASIA_BAHRAIN",
     "ASIA_BANGKOK",
     "ASIA_CALCUTTA",
@@ -709,14 +713,15 @@
     "list_notifications",
     "list_project_memberships",
     "list_projects",
     "list_subscription_grants",
     "list_subscription_requests",
     "list_subscription_targets",
     "list_subscriptions",
+    "list_time_series_data_points",
     "search",
     "search_group_profiles",
     "search_listings",
     "search_types",
     "search_user_profiles",
 ]
 RegionName = Literal[
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/paginator.py` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         ListNotificationsPaginator,
         ListProjectMembershipsPaginator,
         ListProjectsPaginator,
         ListSubscriptionGrantsPaginator,
         ListSubscriptionRequestsPaginator,
         ListSubscriptionTargetsPaginator,
         ListSubscriptionsPaginator,
+        ListTimeSeriesDataPointsPaginator,
         SearchPaginator,
         SearchGroupProfilesPaginator,
         SearchListingsPaginator,
         SearchTypesPaginator,
         SearchUserProfilesPaginator,
     )
 
@@ -50,14 +51,15 @@
     list_notifications_paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")
     list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_subscription_grants_paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")
     list_subscription_requests_paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")
     list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")
     list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
+    list_time_series_data_points_paginator: ListTimeSeriesDataPointsPaginator = client.get_paginator("list_time_series_data_points")
     search_paginator: SearchPaginator = client.get_paginator("search")
     search_group_profiles_paginator: SearchGroupProfilesPaginator = client.get_paginator("search_group_profiles")
     search_listings_paginator: SearchListingsPaginator = client.get_paginator("search_listings")
     search_types_paginator: SearchTypesPaginator = client.get_paginator("search_types")
     search_user_profiles_paginator: SearchUserProfilesPaginator = client.get_paginator("search_user_profiles")
     ```
 """
@@ -73,19 +75,21 @@
     DataSourceStatusType,
     DomainStatusType,
     EnvironmentStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
     MetadataGenerationRunStatusType,
     NotificationTypeType,
+    SearchOutputAdditionalAttributeType,
     SortKeyType,
     SortOrderType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
+    TimeSeriesEntityTypeType,
     TypesSearchScopeType,
     UserSearchTypeType,
 )
 from .type_defs import (
     FilterClauseTypeDef,
     ListAssetRevisionsOutputTypeDef,
     ListDataSourceRunActivitiesOutputTypeDef,
@@ -100,14 +104,15 @@
     ListNotificationsOutputTypeDef,
     ListProjectMembershipsOutputTypeDef,
     ListProjectsOutputTypeDef,
     ListSubscriptionGrantsOutputTypeDef,
     ListSubscriptionRequestsOutputTypeDef,
     ListSubscriptionsOutputTypeDef,
     ListSubscriptionTargetsOutputTypeDef,
+    ListTimeSeriesDataPointsOutputTypeDef,
     PaginatorConfigTypeDef,
     SearchGroupProfilesOutputTypeDef,
     SearchInItemTypeDef,
     SearchListingsOutputTypeDef,
     SearchOutputPaginatorTypeDef,
     SearchSortTypeDef,
     SearchTypesOutputTypeDef,
@@ -134,14 +139,15 @@
     "ListNotificationsPaginator",
     "ListProjectMembershipsPaginator",
     "ListProjectsPaginator",
     "ListSubscriptionGrantsPaginator",
     "ListSubscriptionRequestsPaginator",
     "ListSubscriptionTargetsPaginator",
     "ListSubscriptionsPaginator",
+    "ListTimeSeriesDataPointsPaginator",
     "SearchPaginator",
     "SearchGroupProfilesPaginator",
     "SearchListingsPaginator",
     "SearchTypesPaginator",
     "SearchUserProfilesPaginator",
 )
 
@@ -511,26 +517,49 @@
     ) -> _PageIterator[ListSubscriptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listsubscriptionspaginator)
         """
 
 
+class ListTimeSeriesDataPointsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListTimeSeriesDataPoints)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listtimeseriesdatapointspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        formName: str,
+        endedAt: TimestampTypeDef = ...,
+        startedAt: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListTimeSeriesDataPointsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListTimeSeriesDataPoints.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listtimeseriesdatapointspaginator)
+        """
+
+
 class SearchPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.Search)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#searchpaginator)
     """
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         searchScope: InventorySearchScopeType,
-        additionalAttributes: Sequence[Literal["FORMS"]] = ...,
+        additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,
         filters: FilterClauseTypeDef = ...,
         owningProjectIdentifier: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[SearchOutputPaginatorTypeDef]:
@@ -566,15 +595,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#searchlistingspaginator)
     """
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
-        additionalAttributes: Sequence[Literal["FORMS"]] = ...,
+        additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,
         filters: FilterClauseTypeDef = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[SearchListingsOutputTypeDef]:
         """
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/paginator.pyi` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         ListNotificationsPaginator,
         ListProjectMembershipsPaginator,
         ListProjectsPaginator,
         ListSubscriptionGrantsPaginator,
         ListSubscriptionRequestsPaginator,
         ListSubscriptionTargetsPaginator,
         ListSubscriptionsPaginator,
+        ListTimeSeriesDataPointsPaginator,
         SearchPaginator,
         SearchGroupProfilesPaginator,
         SearchListingsPaginator,
         SearchTypesPaginator,
         SearchUserProfilesPaginator,
     )
 
@@ -50,14 +51,15 @@
     list_notifications_paginator: ListNotificationsPaginator = client.get_paginator("list_notifications")
     list_project_memberships_paginator: ListProjectMembershipsPaginator = client.get_paginator("list_project_memberships")
     list_projects_paginator: ListProjectsPaginator = client.get_paginator("list_projects")
     list_subscription_grants_paginator: ListSubscriptionGrantsPaginator = client.get_paginator("list_subscription_grants")
     list_subscription_requests_paginator: ListSubscriptionRequestsPaginator = client.get_paginator("list_subscription_requests")
     list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator("list_subscription_targets")
     list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator("list_subscriptions")
+    list_time_series_data_points_paginator: ListTimeSeriesDataPointsPaginator = client.get_paginator("list_time_series_data_points")
     search_paginator: SearchPaginator = client.get_paginator("search")
     search_group_profiles_paginator: SearchGroupProfilesPaginator = client.get_paginator("search_group_profiles")
     search_listings_paginator: SearchListingsPaginator = client.get_paginator("search_listings")
     search_types_paginator: SearchTypesPaginator = client.get_paginator("search_types")
     search_user_profiles_paginator: SearchUserProfilesPaginator = client.get_paginator("search_user_profiles")
     ```
 """
@@ -73,19 +75,21 @@
     DataSourceStatusType,
     DomainStatusType,
     EnvironmentStatusType,
     GroupSearchTypeType,
     InventorySearchScopeType,
     MetadataGenerationRunStatusType,
     NotificationTypeType,
+    SearchOutputAdditionalAttributeType,
     SortKeyType,
     SortOrderType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
+    TimeSeriesEntityTypeType,
     TypesSearchScopeType,
     UserSearchTypeType,
 )
 from .type_defs import (
     FilterClauseTypeDef,
     ListAssetRevisionsOutputTypeDef,
     ListDataSourceRunActivitiesOutputTypeDef,
@@ -100,14 +104,15 @@
     ListNotificationsOutputTypeDef,
     ListProjectMembershipsOutputTypeDef,
     ListProjectsOutputTypeDef,
     ListSubscriptionGrantsOutputTypeDef,
     ListSubscriptionRequestsOutputTypeDef,
     ListSubscriptionsOutputTypeDef,
     ListSubscriptionTargetsOutputTypeDef,
+    ListTimeSeriesDataPointsOutputTypeDef,
     PaginatorConfigTypeDef,
     SearchGroupProfilesOutputTypeDef,
     SearchInItemTypeDef,
     SearchListingsOutputTypeDef,
     SearchOutputPaginatorTypeDef,
     SearchSortTypeDef,
     SearchTypesOutputTypeDef,
@@ -134,14 +139,15 @@
     "ListNotificationsPaginator",
     "ListProjectMembershipsPaginator",
     "ListProjectsPaginator",
     "ListSubscriptionGrantsPaginator",
     "ListSubscriptionRequestsPaginator",
     "ListSubscriptionTargetsPaginator",
     "ListSubscriptionsPaginator",
+    "ListTimeSeriesDataPointsPaginator",
     "SearchPaginator",
     "SearchGroupProfilesPaginator",
     "SearchListingsPaginator",
     "SearchTypesPaginator",
     "SearchUserProfilesPaginator",
 )
 
@@ -492,26 +498,48 @@
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[ListSubscriptionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListSubscriptions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listsubscriptionspaginator)
         """
 
+class ListTimeSeriesDataPointsPaginator(Paginator):
+    """
+    [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListTimeSeriesDataPoints)
+    [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listtimeseriesdatapointspaginator)
+    """
+
+    def paginate(
+        self,
+        *,
+        domainIdentifier: str,
+        entityIdentifier: str,
+        entityType: TimeSeriesEntityTypeType,
+        formName: str,
+        endedAt: TimestampTypeDef = ...,
+        startedAt: TimestampTypeDef = ...,
+        PaginationConfig: PaginatorConfigTypeDef = ...,
+    ) -> _PageIterator[ListTimeSeriesDataPointsOutputTypeDef]:
+        """
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.ListTimeSeriesDataPoints.paginate)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#listtimeseriesdatapointspaginator)
+        """
+
 class SearchPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone.Paginator.Search)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#searchpaginator)
     """
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
         searchScope: InventorySearchScopeType,
-        additionalAttributes: Sequence[Literal["FORMS"]] = ...,
+        additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,
         filters: FilterClauseTypeDef = ...,
         owningProjectIdentifier: str = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[SearchOutputPaginatorTypeDef]:
@@ -545,15 +573,15 @@
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/paginators/#searchlistingspaginator)
     """
 
     def paginate(
         self,
         *,
         domainIdentifier: str,
-        additionalAttributes: Sequence[Literal["FORMS"]] = ...,
+        additionalAttributes: Sequence[SearchOutputAdditionalAttributeType] = ...,
         filters: FilterClauseTypeDef = ...,
         searchIn: Sequence[SearchInItemTypeDef] = ...,
         searchText: str = ...,
         sort: SearchSortTypeDef = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
     ) -> _PageIterator[SearchListingsOutputTypeDef]:
         """
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/type_defs.py` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,23 @@
     InventorySearchScopeType,
     ListingStatusType,
     MetadataGenerationRunStatusType,
     NotificationRoleType,
     NotificationTypeType,
     ProjectStatusType,
     RejectRuleBehaviorType,
+    SearchOutputAdditionalAttributeType,
     SortKeyType,
     SortOrderType,
     SubscriptionGrantOverallStatusType,
     SubscriptionGrantStatusType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
+    TimeSeriesEntityTypeType,
     TimezoneType,
     TypesSearchScopeType,
     UserAssignmentType,
     UserDesignationType,
     UserProfileStatusType,
     UserProfileTypeType,
     UserSearchTypeType,
@@ -76,16 +78,16 @@
 
 __all__ = (
     "AcceptChoiceTypeDef",
     "AcceptRuleTypeDef",
     "ResponseMetadataTypeDef",
     "AcceptSubscriptionRequestInputRequestTypeDef",
     "FormOutputTypeDef",
+    "TimeSeriesDataPointSummaryFormOutputTypeDef",
     "AssetListingDetailsTypeDef",
-    "AssetListingItemAdditionalAttributesTypeDef",
     "DetailedGlossaryTermTypeDef",
     "AssetRevisionTypeDef",
     "AssetTargetNameMapTypeDef",
     "FormEntryOutputTypeDef",
     "BusinessNameGenerationConfigurationTypeDef",
     "CancelMetadataGenerationRunInputRequestTypeDef",
     "CancelSubscriptionInputRequestTypeDef",
@@ -125,14 +127,15 @@
     "DeleteGlossaryInputRequestTypeDef",
     "DeleteGlossaryTermInputRequestTypeDef",
     "DeleteListingInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteSubscriptionGrantInputRequestTypeDef",
     "DeleteSubscriptionRequestInputRequestTypeDef",
     "DeleteSubscriptionTargetInputRequestTypeDef",
+    "DeleteTimeSeriesDataPointsInputRequestTypeDef",
     "EnvironmentErrorTypeDef",
     "DomainSummaryTypeDef",
     "EnvironmentBlueprintConfigurationItemTypeDef",
     "EnvironmentProfileSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "FailureCauseTypeDef",
     "FilterTypeDef",
@@ -156,14 +159,16 @@
     "GetMetadataGenerationRunInputRequestTypeDef",
     "MetadataGenerationRunTargetTypeDef",
     "GetProjectInputRequestTypeDef",
     "GetSubscriptionGrantInputRequestTypeDef",
     "GetSubscriptionInputRequestTypeDef",
     "GetSubscriptionRequestDetailsInputRequestTypeDef",
     "GetSubscriptionTargetInputRequestTypeDef",
+    "GetTimeSeriesDataPointInputRequestTypeDef",
+    "TimeSeriesDataPointFormOutputTypeDef",
     "GetUserProfileInputRequestTypeDef",
     "GlossaryItemTypeDef",
     "TermRelationsPaginatorTypeDef",
     "ListingRevisionInputTypeDef",
     "ListingRevisionTypeDef",
     "GroupDetailsTypeDef",
     "GroupProfileSummaryTypeDef",
@@ -228,16 +233,17 @@
     "ListTagsForResourceResponseTypeDef",
     "PutEnvironmentBlueprintConfigurationOutputTypeDef",
     "RejectPredictionsOutputTypeDef",
     "StartMetadataGenerationRunOutputTypeDef",
     "UpdateGlossaryOutputTypeDef",
     "UpdateGroupProfileOutputTypeDef",
     "AssetItemAdditionalAttributesTypeDef",
+    "AssetListingItemAdditionalAttributesTypeDef",
+    "ListTimeSeriesDataPointsOutputTypeDef",
     "GetAssetOutputTypeDef",
-    "AssetListingItemTypeDef",
     "AssetListingTypeDef",
     "SubscribedAssetListingTypeDef",
     "ListAssetRevisionsOutputTypeDef",
     "AssetTypeItemTypeDef",
     "CreateAssetTypeOutputTypeDef",
     "GetAssetTypeOutputTypeDef",
     "PredictionConfigurationTypeDef",
@@ -290,14 +296,16 @@
     "FilterClauseTypeDef",
     "RelationalFilterConfigurationTypeDef",
     "FormTypeDataTypeDef",
     "GetFormTypeOutputTypeDef",
     "GetMetadataGenerationRunOutputTypeDef",
     "MetadataGenerationRunItemTypeDef",
     "StartMetadataGenerationRunInputRequestTypeDef",
+    "GetTimeSeriesDataPointOutputTypeDef",
+    "PostTimeSeriesDataPointsOutputTypeDef",
     "GlossaryTermItemPaginatorTypeDef",
     "GrantedEntityInputTypeDef",
     "GrantedEntityTypeDef",
     "SearchGroupProfilesOutputTypeDef",
     "ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef",
     "ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef",
     "ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef",
@@ -314,26 +322,29 @@
     "ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef",
     "ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef",
     "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef",
     "SearchUserProfilesInputSearchUserProfilesPaginateTypeDef",
     "ListNotificationsInputListNotificationsPaginateTypeDef",
     "ListNotificationsInputRequestTypeDef",
+    "ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef",
+    "ListTimeSeriesDataPointsInputRequestTypeDef",
+    "TimeSeriesDataPointFormInputTypeDef",
     "MemberDetailsTypeDef",
     "TopicTypeDef",
     "RedshiftStorageTypeDef",
     "RejectPredictionsInputRequestTypeDef",
     "SearchInputRequestTypeDef",
     "SearchListingsInputRequestTypeDef",
     "SearchTypesInputRequestTypeDef",
     "UserProfileDetailsTypeDef",
     "SubscribedPrincipalInputTypeDef",
     "SubscribedPrincipalTypeDef",
     "AssetItemTypeDef",
-    "SearchResultItemTypeDef",
+    "AssetListingItemTypeDef",
     "ListingItemTypeDef",
     "SubscribedListingItemTypeDef",
     "CreateAssetInputRequestTypeDef",
     "CreateAssetOutputTypeDef",
     "CreateAssetRevisionInputRequestTypeDef",
     "CreateAssetRevisionOutputTypeDef",
     "EnvironmentBlueprintSummaryTypeDef",
@@ -355,38 +366,40 @@
     "ListMetadataGenerationRunsOutputTypeDef",
     "CreateSubscriptionGrantInputRequestTypeDef",
     "CreateSubscriptionGrantOutputTypeDef",
     "DeleteSubscriptionGrantOutputTypeDef",
     "GetSubscriptionGrantOutputTypeDef",
     "SubscriptionGrantSummaryTypeDef",
     "UpdateSubscriptionGrantStatusOutputTypeDef",
+    "PostTimeSeriesDataPointsInputRequestTypeDef",
     "ProjectMemberTypeDef",
     "NotificationOutputTypeDef",
     "RedshiftRunConfigurationInputTypeDef",
     "RedshiftRunConfigurationOutputTypeDef",
     "CreateUserProfileOutputTypeDef",
     "GetUserProfileOutputTypeDef",
     "UpdateUserProfileOutputTypeDef",
     "UserProfileSummaryTypeDef",
     "CreateSubscriptionRequestInputRequestTypeDef",
     "SearchInventoryResultItemPaginatorTypeDef",
     "SearchInventoryResultItemTypeDef",
-    "SearchListingsOutputTypeDef",
+    "SearchResultItemTypeDef",
     "GetListingOutputTypeDef",
     "SubscribedListingTypeDef",
     "ListEnvironmentBlueprintsOutputTypeDef",
     "SearchTypesOutputTypeDef",
     "ListSubscriptionGrantsOutputTypeDef",
     "ListProjectMembershipsOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "DataSourceConfigurationInputTypeDef",
     "DataSourceConfigurationOutputTypeDef",
     "SearchUserProfilesOutputTypeDef",
     "SearchOutputPaginatorTypeDef",
     "SearchOutputTypeDef",
+    "SearchListingsOutputTypeDef",
     "AcceptSubscriptionRequestOutputTypeDef",
     "CancelSubscriptionOutputTypeDef",
     "CreateSubscriptionRequestOutputTypeDef",
     "GetSubscriptionOutputTypeDef",
     "GetSubscriptionRequestDetailsOutputTypeDef",
     "RejectSubscriptionRequestOutputTypeDef",
     "RevokeSubscriptionOutputTypeDef",
@@ -441,27 +454,32 @@
     {
         "formName": str,
         "content": NotRequired[str],
         "typeName": NotRequired[str],
         "typeRevision": NotRequired[str],
     },
 )
+TimeSeriesDataPointSummaryFormOutputTypeDef = TypedDict(
+    "TimeSeriesDataPointSummaryFormOutputTypeDef",
+    {
+        "formName": str,
+        "timestamp": datetime,
+        "typeIdentifier": str,
+        "contentSummary": NotRequired[str],
+        "id": NotRequired[str],
+        "typeRevision": NotRequired[str],
+    },
+)
 AssetListingDetailsTypeDef = TypedDict(
     "AssetListingDetailsTypeDef",
     {
         "listingId": str,
         "listingStatus": ListingStatusType,
     },
 )
-AssetListingItemAdditionalAttributesTypeDef = TypedDict(
-    "AssetListingItemAdditionalAttributesTypeDef",
-    {
-        "forms": NotRequired[str],
-    },
-)
 DetailedGlossaryTermTypeDef = TypedDict(
     "DetailedGlossaryTermTypeDef",
     {
         "name": NotRequired[str],
         "shortDescription": NotRequired[str],
     },
 )
@@ -811,14 +829,24 @@
     "DeleteSubscriptionTargetInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "environmentIdentifier": str,
         "identifier": str,
     },
 )
+DeleteTimeSeriesDataPointsInputRequestTypeDef = TypedDict(
+    "DeleteTimeSeriesDataPointsInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "formName": str,
+        "clientToken": NotRequired[str],
+    },
+)
 EnvironmentErrorTypeDef = TypedDict(
     "EnvironmentErrorTypeDef",
     {
         "message": str,
         "code": NotRequired[str],
     },
 )
@@ -1064,14 +1092,35 @@
     "GetSubscriptionTargetInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "environmentIdentifier": str,
         "identifier": str,
     },
 )
+GetTimeSeriesDataPointInputRequestTypeDef = TypedDict(
+    "GetTimeSeriesDataPointInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "formName": str,
+        "identifier": str,
+    },
+)
+TimeSeriesDataPointFormOutputTypeDef = TypedDict(
+    "TimeSeriesDataPointFormOutputTypeDef",
+    {
+        "formName": str,
+        "timestamp": datetime,
+        "typeIdentifier": str,
+        "content": NotRequired[str],
+        "id": NotRequired[str],
+        "typeRevision": NotRequired[str],
+    },
+)
 GetUserProfileInputRequestTypeDef = TypedDict(
     "GetUserProfileInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "userIdentifier": str,
         "type": NotRequired[UserProfileTypeType],
     },
@@ -1726,67 +1775,73 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 AssetItemAdditionalAttributesTypeDef = TypedDict(
     "AssetItemAdditionalAttributesTypeDef",
     {
         "formsOutput": NotRequired[List[FormOutputTypeDef]],
+        "latestTimeSeriesDataPointFormsOutput": NotRequired[
+            List[TimeSeriesDataPointSummaryFormOutputTypeDef]
+        ],
         "readOnlyFormsOutput": NotRequired[List[FormOutputTypeDef]],
     },
 )
+AssetListingItemAdditionalAttributesTypeDef = TypedDict(
+    "AssetListingItemAdditionalAttributesTypeDef",
+    {
+        "forms": NotRequired[str],
+        "latestTimeSeriesDataPointForms": NotRequired[
+            List[TimeSeriesDataPointSummaryFormOutputTypeDef]
+        ],
+    },
+)
+ListTimeSeriesDataPointsOutputTypeDef = TypedDict(
+    "ListTimeSeriesDataPointsOutputTypeDef",
+    {
+        "items": List[TimeSeriesDataPointSummaryFormOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetAssetOutputTypeDef = TypedDict(
     "GetAssetOutputTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
         "description": str,
         "domainId": str,
         "externalIdentifier": str,
         "firstRevisionCreatedAt": datetime,
         "firstRevisionCreatedBy": str,
         "formsOutput": List[FormOutputTypeDef],
         "glossaryTerms": List[str],
         "id": str,
+        "latestTimeSeriesDataPointFormsOutput": List[TimeSeriesDataPointSummaryFormOutputTypeDef],
         "listing": AssetListingDetailsTypeDef,
         "name": str,
         "owningProjectId": str,
         "readOnlyFormsOutput": List[FormOutputTypeDef],
         "revision": str,
         "typeIdentifier": str,
         "typeRevision": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-AssetListingItemTypeDef = TypedDict(
-    "AssetListingItemTypeDef",
-    {
-        "additionalAttributes": NotRequired[AssetListingItemAdditionalAttributesTypeDef],
-        "createdAt": NotRequired[datetime],
-        "description": NotRequired[str],
-        "entityId": NotRequired[str],
-        "entityRevision": NotRequired[str],
-        "entityType": NotRequired[str],
-        "glossaryTerms": NotRequired[List[DetailedGlossaryTermTypeDef]],
-        "listingCreatedBy": NotRequired[str],
-        "listingId": NotRequired[str],
-        "listingRevision": NotRequired[str],
-        "listingUpdatedBy": NotRequired[str],
-        "name": NotRequired[str],
-        "owningProjectId": NotRequired[str],
-    },
-)
 AssetListingTypeDef = TypedDict(
     "AssetListingTypeDef",
     {
         "assetId": NotRequired[str],
         "assetRevision": NotRequired[str],
         "assetType": NotRequired[str],
         "createdAt": NotRequired[datetime],
         "forms": NotRequired[str],
         "glossaryTerms": NotRequired[List[DetailedGlossaryTermTypeDef]],
+        "latestTimeSeriesDataPointForms": NotRequired[
+            List[TimeSeriesDataPointSummaryFormOutputTypeDef]
+        ],
         "owningProjectId": NotRequired[str],
     },
 )
 SubscribedAssetListingTypeDef = TypedDict(
     "SubscribedAssetListingTypeDef",
     {
         "entityId": NotRequired[str],
@@ -2592,14 +2647,35 @@
         "domainIdentifier": str,
         "owningProjectIdentifier": str,
         "target": MetadataGenerationRunTargetTypeDef,
         "type": Literal["BUSINESS_DESCRIPTIONS"],
         "clientToken": NotRequired[str],
     },
 )
+GetTimeSeriesDataPointOutputTypeDef = TypedDict(
+    "GetTimeSeriesDataPointOutputTypeDef",
+    {
+        "domainId": str,
+        "entityId": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "form": TimeSeriesDataPointFormOutputTypeDef,
+        "formName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+PostTimeSeriesDataPointsOutputTypeDef = TypedDict(
+    "PostTimeSeriesDataPointsOutputTypeDef",
+    {
+        "domainId": str,
+        "entityId": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "forms": List[TimeSeriesDataPointFormOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GlossaryTermItemPaginatorTypeDef = TypedDict(
     "GlossaryTermItemPaginatorTypeDef",
     {
         "domainId": str,
         "glossaryId": str,
         "id": str,
         "name": str,
@@ -2839,14 +2915,49 @@
         "beforeTimestamp": NotRequired[TimestampTypeDef],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "subjects": NotRequired[Sequence[str]],
         "taskStatus": NotRequired[TaskStatusType],
     },
 )
+ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef = TypedDict(
+    "ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "formName": str,
+        "endedAt": NotRequired[TimestampTypeDef],
+        "startedAt": NotRequired[TimestampTypeDef],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListTimeSeriesDataPointsInputRequestTypeDef = TypedDict(
+    "ListTimeSeriesDataPointsInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "formName": str,
+        "endedAt": NotRequired[TimestampTypeDef],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+        "startedAt": NotRequired[TimestampTypeDef],
+    },
+)
+TimeSeriesDataPointFormInputTypeDef = TypedDict(
+    "TimeSeriesDataPointFormInputTypeDef",
+    {
+        "formName": str,
+        "timestamp": TimestampTypeDef,
+        "typeIdentifier": str,
+        "content": NotRequired[str],
+        "typeRevision": NotRequired[str],
+    },
+)
 MemberDetailsTypeDef = TypedDict(
     "MemberDetailsTypeDef",
     {
         "group": NotRequired[GroupDetailsTypeDef],
         "user": NotRequired[UserDetailsTypeDef],
     },
 )
@@ -2877,29 +2988,29 @@
     },
 )
 SearchInputRequestTypeDef = TypedDict(
     "SearchInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "searchScope": InventorySearchScopeType,
-        "additionalAttributes": NotRequired[Sequence[Literal["FORMS"]]],
+        "additionalAttributes": NotRequired[Sequence[SearchOutputAdditionalAttributeType]],
         "filters": NotRequired["FilterClauseTypeDef"],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "owningProjectIdentifier": NotRequired[str],
         "searchIn": NotRequired[Sequence[SearchInItemTypeDef]],
         "searchText": NotRequired[str],
         "sort": NotRequired[SearchSortTypeDef],
     },
 )
 SearchListingsInputRequestTypeDef = TypedDict(
     "SearchListingsInputRequestTypeDef",
     {
         "domainIdentifier": str,
-        "additionalAttributes": NotRequired[Sequence[Literal["FORMS"]]],
+        "additionalAttributes": NotRequired[Sequence[SearchOutputAdditionalAttributeType]],
         "filters": NotRequired["FilterClauseTypeDef"],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "searchIn": NotRequired[Sequence[SearchInItemTypeDef]],
         "searchText": NotRequired[str],
         "sort": NotRequired[SearchSortTypeDef],
     },
@@ -2952,18 +3063,30 @@
         "description": NotRequired[str],
         "externalIdentifier": NotRequired[str],
         "firstRevisionCreatedAt": NotRequired[datetime],
         "firstRevisionCreatedBy": NotRequired[str],
         "glossaryTerms": NotRequired[List[str]],
     },
 )
-SearchResultItemTypeDef = TypedDict(
-    "SearchResultItemTypeDef",
+AssetListingItemTypeDef = TypedDict(
+    "AssetListingItemTypeDef",
     {
-        "assetListing": NotRequired[AssetListingItemTypeDef],
+        "additionalAttributes": NotRequired[AssetListingItemAdditionalAttributesTypeDef],
+        "createdAt": NotRequired[datetime],
+        "description": NotRequired[str],
+        "entityId": NotRequired[str],
+        "entityRevision": NotRequired[str],
+        "entityType": NotRequired[str],
+        "glossaryTerms": NotRequired[List[DetailedGlossaryTermTypeDef]],
+        "listingCreatedBy": NotRequired[str],
+        "listingId": NotRequired[str],
+        "listingRevision": NotRequired[str],
+        "listingUpdatedBy": NotRequired[str],
+        "name": NotRequired[str],
+        "owningProjectId": NotRequired[str],
     },
 )
 ListingItemTypeDef = TypedDict(
     "ListingItemTypeDef",
     {
         "assetListing": NotRequired[AssetListingTypeDef],
     },
@@ -2999,14 +3122,15 @@
         "domainId": str,
         "externalIdentifier": str,
         "firstRevisionCreatedAt": datetime,
         "firstRevisionCreatedBy": str,
         "formsOutput": List[FormOutputTypeDef],
         "glossaryTerms": List[str],
         "id": str,
+        "latestTimeSeriesDataPointFormsOutput": List[TimeSeriesDataPointSummaryFormOutputTypeDef],
         "listing": AssetListingDetailsTypeDef,
         "name": str,
         "owningProjectId": str,
         "predictionConfiguration": PredictionConfigurationTypeDef,
         "readOnlyFormsOutput": List[FormOutputTypeDef],
         "revision": str,
         "typeIdentifier": str,
@@ -3037,14 +3161,15 @@
         "domainId": str,
         "externalIdentifier": str,
         "firstRevisionCreatedAt": datetime,
         "firstRevisionCreatedBy": str,
         "formsOutput": List[FormOutputTypeDef],
         "glossaryTerms": List[str],
         "id": str,
+        "latestTimeSeriesDataPointFormsOutput": List[TimeSeriesDataPointSummaryFormOutputTypeDef],
         "listing": AssetListingDetailsTypeDef,
         "name": str,
         "owningProjectId": str,
         "predictionConfiguration": PredictionConfigurationTypeDef,
         "readOnlyFormsOutput": List[FormOutputTypeDef],
         "revision": str,
         "typeIdentifier": str,
@@ -3202,28 +3327,28 @@
     },
 )
 SearchInputSearchPaginateTypeDef = TypedDict(
     "SearchInputSearchPaginateTypeDef",
     {
         "domainIdentifier": str,
         "searchScope": InventorySearchScopeType,
-        "additionalAttributes": NotRequired[Sequence[Literal["FORMS"]]],
+        "additionalAttributes": NotRequired[Sequence[SearchOutputAdditionalAttributeType]],
         "filters": NotRequired[FilterClauseTypeDef],
         "owningProjectIdentifier": NotRequired[str],
         "searchIn": NotRequired[Sequence[SearchInItemTypeDef]],
         "searchText": NotRequired[str],
         "sort": NotRequired[SearchSortTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 SearchListingsInputSearchListingsPaginateTypeDef = TypedDict(
     "SearchListingsInputSearchListingsPaginateTypeDef",
     {
         "domainIdentifier": str,
-        "additionalAttributes": NotRequired[Sequence[Literal["FORMS"]]],
+        "additionalAttributes": NotRequired[Sequence[SearchOutputAdditionalAttributeType]],
         "filters": NotRequired[FilterClauseTypeDef],
         "searchIn": NotRequired[Sequence[SearchInItemTypeDef]],
         "searchText": NotRequired[str],
         "sort": NotRequired[SearchSortTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -3240,22 +3365,24 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 GlueRunConfigurationInputTypeDef = TypedDict(
     "GlueRunConfigurationInputTypeDef",
     {
         "relationalFilterConfigurations": Sequence[RelationalFilterConfigurationTypeDef],
+        "autoImportDataQualityResult": NotRequired[bool],
         "dataAccessRole": NotRequired[str],
     },
 )
 GlueRunConfigurationOutputTypeDef = TypedDict(
     "GlueRunConfigurationOutputTypeDef",
     {
         "relationalFilterConfigurations": List[RelationalFilterConfigurationTypeDef],
         "accountId": NotRequired[str],
+        "autoImportDataQualityResult": NotRequired[bool],
         "dataAccessRole": NotRequired[str],
         "region": NotRequired[str],
     },
 )
 SearchTypesResultItemTypeDef = TypedDict(
     "SearchTypesResultItemTypeDef",
     {
@@ -3362,14 +3489,24 @@
         "subscriptionId": str,
         "subscriptionTargetId": str,
         "updatedAt": datetime,
         "updatedBy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+PostTimeSeriesDataPointsInputRequestTypeDef = TypedDict(
+    "PostTimeSeriesDataPointsInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "forms": Sequence[TimeSeriesDataPointFormInputTypeDef],
+        "clientToken": NotRequired[str],
+    },
+)
 ProjectMemberTypeDef = TypedDict(
     "ProjectMemberTypeDef",
     {
         "designation": UserDesignationType,
         "memberDetails": MemberDetailsTypeDef,
     },
 )
@@ -3476,21 +3613,18 @@
     {
         "assetItem": NotRequired[AssetItemTypeDef],
         "dataProductItem": NotRequired[DataProductSummaryTypeDef],
         "glossaryItem": NotRequired[GlossaryItemTypeDef],
         "glossaryTermItem": NotRequired[GlossaryTermItemTypeDef],
     },
 )
-SearchListingsOutputTypeDef = TypedDict(
-    "SearchListingsOutputTypeDef",
+SearchResultItemTypeDef = TypedDict(
+    "SearchResultItemTypeDef",
     {
-        "items": List[SearchResultItemTypeDef],
-        "nextToken": str,
-        "totalMatchCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assetListing": NotRequired[AssetListingItemTypeDef],
     },
 )
 GetListingOutputTypeDef = TypedDict(
     "GetListingOutputTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
@@ -3595,14 +3729,23 @@
     {
         "items": List[SearchInventoryResultItemTypeDef],
         "nextToken": str,
         "totalMatchCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SearchListingsOutputTypeDef = TypedDict(
+    "SearchListingsOutputTypeDef",
+    {
+        "items": List[SearchResultItemTypeDef],
+        "nextToken": str,
+        "totalMatchCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 AcceptSubscriptionRequestOutputTypeDef = TypedDict(
     "AcceptSubscriptionRequestOutputTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
         "decisionComment": str,
         "domainId": str,
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone/type_defs.pyi` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,23 @@
     InventorySearchScopeType,
     ListingStatusType,
     MetadataGenerationRunStatusType,
     NotificationRoleType,
     NotificationTypeType,
     ProjectStatusType,
     RejectRuleBehaviorType,
+    SearchOutputAdditionalAttributeType,
     SortKeyType,
     SortOrderType,
     SubscriptionGrantOverallStatusType,
     SubscriptionGrantStatusType,
     SubscriptionRequestStatusType,
     SubscriptionStatusType,
     TaskStatusType,
+    TimeSeriesEntityTypeType,
     TimezoneType,
     TypesSearchScopeType,
     UserAssignmentType,
     UserDesignationType,
     UserProfileStatusType,
     UserProfileTypeType,
     UserSearchTypeType,
@@ -76,16 +78,16 @@
 
 __all__ = (
     "AcceptChoiceTypeDef",
     "AcceptRuleTypeDef",
     "ResponseMetadataTypeDef",
     "AcceptSubscriptionRequestInputRequestTypeDef",
     "FormOutputTypeDef",
+    "TimeSeriesDataPointSummaryFormOutputTypeDef",
     "AssetListingDetailsTypeDef",
-    "AssetListingItemAdditionalAttributesTypeDef",
     "DetailedGlossaryTermTypeDef",
     "AssetRevisionTypeDef",
     "AssetTargetNameMapTypeDef",
     "FormEntryOutputTypeDef",
     "BusinessNameGenerationConfigurationTypeDef",
     "CancelMetadataGenerationRunInputRequestTypeDef",
     "CancelSubscriptionInputRequestTypeDef",
@@ -125,14 +127,15 @@
     "DeleteGlossaryInputRequestTypeDef",
     "DeleteGlossaryTermInputRequestTypeDef",
     "DeleteListingInputRequestTypeDef",
     "DeleteProjectInputRequestTypeDef",
     "DeleteSubscriptionGrantInputRequestTypeDef",
     "DeleteSubscriptionRequestInputRequestTypeDef",
     "DeleteSubscriptionTargetInputRequestTypeDef",
+    "DeleteTimeSeriesDataPointsInputRequestTypeDef",
     "EnvironmentErrorTypeDef",
     "DomainSummaryTypeDef",
     "EnvironmentBlueprintConfigurationItemTypeDef",
     "EnvironmentProfileSummaryTypeDef",
     "EnvironmentSummaryTypeDef",
     "FailureCauseTypeDef",
     "FilterTypeDef",
@@ -156,14 +159,16 @@
     "GetMetadataGenerationRunInputRequestTypeDef",
     "MetadataGenerationRunTargetTypeDef",
     "GetProjectInputRequestTypeDef",
     "GetSubscriptionGrantInputRequestTypeDef",
     "GetSubscriptionInputRequestTypeDef",
     "GetSubscriptionRequestDetailsInputRequestTypeDef",
     "GetSubscriptionTargetInputRequestTypeDef",
+    "GetTimeSeriesDataPointInputRequestTypeDef",
+    "TimeSeriesDataPointFormOutputTypeDef",
     "GetUserProfileInputRequestTypeDef",
     "GlossaryItemTypeDef",
     "TermRelationsPaginatorTypeDef",
     "ListingRevisionInputTypeDef",
     "ListingRevisionTypeDef",
     "GroupDetailsTypeDef",
     "GroupProfileSummaryTypeDef",
@@ -228,16 +233,17 @@
     "ListTagsForResourceResponseTypeDef",
     "PutEnvironmentBlueprintConfigurationOutputTypeDef",
     "RejectPredictionsOutputTypeDef",
     "StartMetadataGenerationRunOutputTypeDef",
     "UpdateGlossaryOutputTypeDef",
     "UpdateGroupProfileOutputTypeDef",
     "AssetItemAdditionalAttributesTypeDef",
+    "AssetListingItemAdditionalAttributesTypeDef",
+    "ListTimeSeriesDataPointsOutputTypeDef",
     "GetAssetOutputTypeDef",
-    "AssetListingItemTypeDef",
     "AssetListingTypeDef",
     "SubscribedAssetListingTypeDef",
     "ListAssetRevisionsOutputTypeDef",
     "AssetTypeItemTypeDef",
     "CreateAssetTypeOutputTypeDef",
     "GetAssetTypeOutputTypeDef",
     "PredictionConfigurationTypeDef",
@@ -290,14 +296,16 @@
     "FilterClauseTypeDef",
     "RelationalFilterConfigurationTypeDef",
     "FormTypeDataTypeDef",
     "GetFormTypeOutputTypeDef",
     "GetMetadataGenerationRunOutputTypeDef",
     "MetadataGenerationRunItemTypeDef",
     "StartMetadataGenerationRunInputRequestTypeDef",
+    "GetTimeSeriesDataPointOutputTypeDef",
+    "PostTimeSeriesDataPointsOutputTypeDef",
     "GlossaryTermItemPaginatorTypeDef",
     "GrantedEntityInputTypeDef",
     "GrantedEntityTypeDef",
     "SearchGroupProfilesOutputTypeDef",
     "ListAssetRevisionsInputListAssetRevisionsPaginateTypeDef",
     "ListDataSourceRunActivitiesInputListDataSourceRunActivitiesPaginateTypeDef",
     "ListDataSourceRunsInputListDataSourceRunsPaginateTypeDef",
@@ -314,26 +322,29 @@
     "ListSubscriptionRequestsInputListSubscriptionRequestsPaginateTypeDef",
     "ListSubscriptionTargetsInputListSubscriptionTargetsPaginateTypeDef",
     "ListSubscriptionsInputListSubscriptionsPaginateTypeDef",
     "SearchGroupProfilesInputSearchGroupProfilesPaginateTypeDef",
     "SearchUserProfilesInputSearchUserProfilesPaginateTypeDef",
     "ListNotificationsInputListNotificationsPaginateTypeDef",
     "ListNotificationsInputRequestTypeDef",
+    "ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef",
+    "ListTimeSeriesDataPointsInputRequestTypeDef",
+    "TimeSeriesDataPointFormInputTypeDef",
     "MemberDetailsTypeDef",
     "TopicTypeDef",
     "RedshiftStorageTypeDef",
     "RejectPredictionsInputRequestTypeDef",
     "SearchInputRequestTypeDef",
     "SearchListingsInputRequestTypeDef",
     "SearchTypesInputRequestTypeDef",
     "UserProfileDetailsTypeDef",
     "SubscribedPrincipalInputTypeDef",
     "SubscribedPrincipalTypeDef",
     "AssetItemTypeDef",
-    "SearchResultItemTypeDef",
+    "AssetListingItemTypeDef",
     "ListingItemTypeDef",
     "SubscribedListingItemTypeDef",
     "CreateAssetInputRequestTypeDef",
     "CreateAssetOutputTypeDef",
     "CreateAssetRevisionInputRequestTypeDef",
     "CreateAssetRevisionOutputTypeDef",
     "EnvironmentBlueprintSummaryTypeDef",
@@ -355,38 +366,40 @@
     "ListMetadataGenerationRunsOutputTypeDef",
     "CreateSubscriptionGrantInputRequestTypeDef",
     "CreateSubscriptionGrantOutputTypeDef",
     "DeleteSubscriptionGrantOutputTypeDef",
     "GetSubscriptionGrantOutputTypeDef",
     "SubscriptionGrantSummaryTypeDef",
     "UpdateSubscriptionGrantStatusOutputTypeDef",
+    "PostTimeSeriesDataPointsInputRequestTypeDef",
     "ProjectMemberTypeDef",
     "NotificationOutputTypeDef",
     "RedshiftRunConfigurationInputTypeDef",
     "RedshiftRunConfigurationOutputTypeDef",
     "CreateUserProfileOutputTypeDef",
     "GetUserProfileOutputTypeDef",
     "UpdateUserProfileOutputTypeDef",
     "UserProfileSummaryTypeDef",
     "CreateSubscriptionRequestInputRequestTypeDef",
     "SearchInventoryResultItemPaginatorTypeDef",
     "SearchInventoryResultItemTypeDef",
-    "SearchListingsOutputTypeDef",
+    "SearchResultItemTypeDef",
     "GetListingOutputTypeDef",
     "SubscribedListingTypeDef",
     "ListEnvironmentBlueprintsOutputTypeDef",
     "SearchTypesOutputTypeDef",
     "ListSubscriptionGrantsOutputTypeDef",
     "ListProjectMembershipsOutputTypeDef",
     "ListNotificationsOutputTypeDef",
     "DataSourceConfigurationInputTypeDef",
     "DataSourceConfigurationOutputTypeDef",
     "SearchUserProfilesOutputTypeDef",
     "SearchOutputPaginatorTypeDef",
     "SearchOutputTypeDef",
+    "SearchListingsOutputTypeDef",
     "AcceptSubscriptionRequestOutputTypeDef",
     "CancelSubscriptionOutputTypeDef",
     "CreateSubscriptionRequestOutputTypeDef",
     "GetSubscriptionOutputTypeDef",
     "GetSubscriptionRequestDetailsOutputTypeDef",
     "RejectSubscriptionRequestOutputTypeDef",
     "RevokeSubscriptionOutputTypeDef",
@@ -441,27 +454,32 @@
     {
         "formName": str,
         "content": NotRequired[str],
         "typeName": NotRequired[str],
         "typeRevision": NotRequired[str],
     },
 )
+TimeSeriesDataPointSummaryFormOutputTypeDef = TypedDict(
+    "TimeSeriesDataPointSummaryFormOutputTypeDef",
+    {
+        "formName": str,
+        "timestamp": datetime,
+        "typeIdentifier": str,
+        "contentSummary": NotRequired[str],
+        "id": NotRequired[str],
+        "typeRevision": NotRequired[str],
+    },
+)
 AssetListingDetailsTypeDef = TypedDict(
     "AssetListingDetailsTypeDef",
     {
         "listingId": str,
         "listingStatus": ListingStatusType,
     },
 )
-AssetListingItemAdditionalAttributesTypeDef = TypedDict(
-    "AssetListingItemAdditionalAttributesTypeDef",
-    {
-        "forms": NotRequired[str],
-    },
-)
 DetailedGlossaryTermTypeDef = TypedDict(
     "DetailedGlossaryTermTypeDef",
     {
         "name": NotRequired[str],
         "shortDescription": NotRequired[str],
     },
 )
@@ -811,14 +829,24 @@
     "DeleteSubscriptionTargetInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "environmentIdentifier": str,
         "identifier": str,
     },
 )
+DeleteTimeSeriesDataPointsInputRequestTypeDef = TypedDict(
+    "DeleteTimeSeriesDataPointsInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "formName": str,
+        "clientToken": NotRequired[str],
+    },
+)
 EnvironmentErrorTypeDef = TypedDict(
     "EnvironmentErrorTypeDef",
     {
         "message": str,
         "code": NotRequired[str],
     },
 )
@@ -1064,14 +1092,35 @@
     "GetSubscriptionTargetInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "environmentIdentifier": str,
         "identifier": str,
     },
 )
+GetTimeSeriesDataPointInputRequestTypeDef = TypedDict(
+    "GetTimeSeriesDataPointInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "formName": str,
+        "identifier": str,
+    },
+)
+TimeSeriesDataPointFormOutputTypeDef = TypedDict(
+    "TimeSeriesDataPointFormOutputTypeDef",
+    {
+        "formName": str,
+        "timestamp": datetime,
+        "typeIdentifier": str,
+        "content": NotRequired[str],
+        "id": NotRequired[str],
+        "typeRevision": NotRequired[str],
+    },
+)
 GetUserProfileInputRequestTypeDef = TypedDict(
     "GetUserProfileInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "userIdentifier": str,
         "type": NotRequired[UserProfileTypeType],
     },
@@ -1726,67 +1775,73 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 AssetItemAdditionalAttributesTypeDef = TypedDict(
     "AssetItemAdditionalAttributesTypeDef",
     {
         "formsOutput": NotRequired[List[FormOutputTypeDef]],
+        "latestTimeSeriesDataPointFormsOutput": NotRequired[
+            List[TimeSeriesDataPointSummaryFormOutputTypeDef]
+        ],
         "readOnlyFormsOutput": NotRequired[List[FormOutputTypeDef]],
     },
 )
+AssetListingItemAdditionalAttributesTypeDef = TypedDict(
+    "AssetListingItemAdditionalAttributesTypeDef",
+    {
+        "forms": NotRequired[str],
+        "latestTimeSeriesDataPointForms": NotRequired[
+            List[TimeSeriesDataPointSummaryFormOutputTypeDef]
+        ],
+    },
+)
+ListTimeSeriesDataPointsOutputTypeDef = TypedDict(
+    "ListTimeSeriesDataPointsOutputTypeDef",
+    {
+        "items": List[TimeSeriesDataPointSummaryFormOutputTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GetAssetOutputTypeDef = TypedDict(
     "GetAssetOutputTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
         "description": str,
         "domainId": str,
         "externalIdentifier": str,
         "firstRevisionCreatedAt": datetime,
         "firstRevisionCreatedBy": str,
         "formsOutput": List[FormOutputTypeDef],
         "glossaryTerms": List[str],
         "id": str,
+        "latestTimeSeriesDataPointFormsOutput": List[TimeSeriesDataPointSummaryFormOutputTypeDef],
         "listing": AssetListingDetailsTypeDef,
         "name": str,
         "owningProjectId": str,
         "readOnlyFormsOutput": List[FormOutputTypeDef],
         "revision": str,
         "typeIdentifier": str,
         "typeRevision": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-AssetListingItemTypeDef = TypedDict(
-    "AssetListingItemTypeDef",
-    {
-        "additionalAttributes": NotRequired[AssetListingItemAdditionalAttributesTypeDef],
-        "createdAt": NotRequired[datetime],
-        "description": NotRequired[str],
-        "entityId": NotRequired[str],
-        "entityRevision": NotRequired[str],
-        "entityType": NotRequired[str],
-        "glossaryTerms": NotRequired[List[DetailedGlossaryTermTypeDef]],
-        "listingCreatedBy": NotRequired[str],
-        "listingId": NotRequired[str],
-        "listingRevision": NotRequired[str],
-        "listingUpdatedBy": NotRequired[str],
-        "name": NotRequired[str],
-        "owningProjectId": NotRequired[str],
-    },
-)
 AssetListingTypeDef = TypedDict(
     "AssetListingTypeDef",
     {
         "assetId": NotRequired[str],
         "assetRevision": NotRequired[str],
         "assetType": NotRequired[str],
         "createdAt": NotRequired[datetime],
         "forms": NotRequired[str],
         "glossaryTerms": NotRequired[List[DetailedGlossaryTermTypeDef]],
+        "latestTimeSeriesDataPointForms": NotRequired[
+            List[TimeSeriesDataPointSummaryFormOutputTypeDef]
+        ],
         "owningProjectId": NotRequired[str],
     },
 )
 SubscribedAssetListingTypeDef = TypedDict(
     "SubscribedAssetListingTypeDef",
     {
         "entityId": NotRequired[str],
@@ -2592,14 +2647,35 @@
         "domainIdentifier": str,
         "owningProjectIdentifier": str,
         "target": MetadataGenerationRunTargetTypeDef,
         "type": Literal["BUSINESS_DESCRIPTIONS"],
         "clientToken": NotRequired[str],
     },
 )
+GetTimeSeriesDataPointOutputTypeDef = TypedDict(
+    "GetTimeSeriesDataPointOutputTypeDef",
+    {
+        "domainId": str,
+        "entityId": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "form": TimeSeriesDataPointFormOutputTypeDef,
+        "formName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+PostTimeSeriesDataPointsOutputTypeDef = TypedDict(
+    "PostTimeSeriesDataPointsOutputTypeDef",
+    {
+        "domainId": str,
+        "entityId": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "forms": List[TimeSeriesDataPointFormOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 GlossaryTermItemPaginatorTypeDef = TypedDict(
     "GlossaryTermItemPaginatorTypeDef",
     {
         "domainId": str,
         "glossaryId": str,
         "id": str,
         "name": str,
@@ -2839,14 +2915,49 @@
         "beforeTimestamp": NotRequired[TimestampTypeDef],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "subjects": NotRequired[Sequence[str]],
         "taskStatus": NotRequired[TaskStatusType],
     },
 )
+ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef = TypedDict(
+    "ListTimeSeriesDataPointsInputListTimeSeriesDataPointsPaginateTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "formName": str,
+        "endedAt": NotRequired[TimestampTypeDef],
+        "startedAt": NotRequired[TimestampTypeDef],
+        "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
+    },
+)
+ListTimeSeriesDataPointsInputRequestTypeDef = TypedDict(
+    "ListTimeSeriesDataPointsInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "formName": str,
+        "endedAt": NotRequired[TimestampTypeDef],
+        "maxResults": NotRequired[int],
+        "nextToken": NotRequired[str],
+        "startedAt": NotRequired[TimestampTypeDef],
+    },
+)
+TimeSeriesDataPointFormInputTypeDef = TypedDict(
+    "TimeSeriesDataPointFormInputTypeDef",
+    {
+        "formName": str,
+        "timestamp": TimestampTypeDef,
+        "typeIdentifier": str,
+        "content": NotRequired[str],
+        "typeRevision": NotRequired[str],
+    },
+)
 MemberDetailsTypeDef = TypedDict(
     "MemberDetailsTypeDef",
     {
         "group": NotRequired[GroupDetailsTypeDef],
         "user": NotRequired[UserDetailsTypeDef],
     },
 )
@@ -2877,29 +2988,29 @@
     },
 )
 SearchInputRequestTypeDef = TypedDict(
     "SearchInputRequestTypeDef",
     {
         "domainIdentifier": str,
         "searchScope": InventorySearchScopeType,
-        "additionalAttributes": NotRequired[Sequence[Literal["FORMS"]]],
+        "additionalAttributes": NotRequired[Sequence[SearchOutputAdditionalAttributeType]],
         "filters": NotRequired["FilterClauseTypeDef"],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "owningProjectIdentifier": NotRequired[str],
         "searchIn": NotRequired[Sequence[SearchInItemTypeDef]],
         "searchText": NotRequired[str],
         "sort": NotRequired[SearchSortTypeDef],
     },
 )
 SearchListingsInputRequestTypeDef = TypedDict(
     "SearchListingsInputRequestTypeDef",
     {
         "domainIdentifier": str,
-        "additionalAttributes": NotRequired[Sequence[Literal["FORMS"]]],
+        "additionalAttributes": NotRequired[Sequence[SearchOutputAdditionalAttributeType]],
         "filters": NotRequired["FilterClauseTypeDef"],
         "maxResults": NotRequired[int],
         "nextToken": NotRequired[str],
         "searchIn": NotRequired[Sequence[SearchInItemTypeDef]],
         "searchText": NotRequired[str],
         "sort": NotRequired[SearchSortTypeDef],
     },
@@ -2952,18 +3063,30 @@
         "description": NotRequired[str],
         "externalIdentifier": NotRequired[str],
         "firstRevisionCreatedAt": NotRequired[datetime],
         "firstRevisionCreatedBy": NotRequired[str],
         "glossaryTerms": NotRequired[List[str]],
     },
 )
-SearchResultItemTypeDef = TypedDict(
-    "SearchResultItemTypeDef",
+AssetListingItemTypeDef = TypedDict(
+    "AssetListingItemTypeDef",
     {
-        "assetListing": NotRequired[AssetListingItemTypeDef],
+        "additionalAttributes": NotRequired[AssetListingItemAdditionalAttributesTypeDef],
+        "createdAt": NotRequired[datetime],
+        "description": NotRequired[str],
+        "entityId": NotRequired[str],
+        "entityRevision": NotRequired[str],
+        "entityType": NotRequired[str],
+        "glossaryTerms": NotRequired[List[DetailedGlossaryTermTypeDef]],
+        "listingCreatedBy": NotRequired[str],
+        "listingId": NotRequired[str],
+        "listingRevision": NotRequired[str],
+        "listingUpdatedBy": NotRequired[str],
+        "name": NotRequired[str],
+        "owningProjectId": NotRequired[str],
     },
 )
 ListingItemTypeDef = TypedDict(
     "ListingItemTypeDef",
     {
         "assetListing": NotRequired[AssetListingTypeDef],
     },
@@ -2999,14 +3122,15 @@
         "domainId": str,
         "externalIdentifier": str,
         "firstRevisionCreatedAt": datetime,
         "firstRevisionCreatedBy": str,
         "formsOutput": List[FormOutputTypeDef],
         "glossaryTerms": List[str],
         "id": str,
+        "latestTimeSeriesDataPointFormsOutput": List[TimeSeriesDataPointSummaryFormOutputTypeDef],
         "listing": AssetListingDetailsTypeDef,
         "name": str,
         "owningProjectId": str,
         "predictionConfiguration": PredictionConfigurationTypeDef,
         "readOnlyFormsOutput": List[FormOutputTypeDef],
         "revision": str,
         "typeIdentifier": str,
@@ -3037,14 +3161,15 @@
         "domainId": str,
         "externalIdentifier": str,
         "firstRevisionCreatedAt": datetime,
         "firstRevisionCreatedBy": str,
         "formsOutput": List[FormOutputTypeDef],
         "glossaryTerms": List[str],
         "id": str,
+        "latestTimeSeriesDataPointFormsOutput": List[TimeSeriesDataPointSummaryFormOutputTypeDef],
         "listing": AssetListingDetailsTypeDef,
         "name": str,
         "owningProjectId": str,
         "predictionConfiguration": PredictionConfigurationTypeDef,
         "readOnlyFormsOutput": List[FormOutputTypeDef],
         "revision": str,
         "typeIdentifier": str,
@@ -3202,28 +3327,28 @@
     },
 )
 SearchInputSearchPaginateTypeDef = TypedDict(
     "SearchInputSearchPaginateTypeDef",
     {
         "domainIdentifier": str,
         "searchScope": InventorySearchScopeType,
-        "additionalAttributes": NotRequired[Sequence[Literal["FORMS"]]],
+        "additionalAttributes": NotRequired[Sequence[SearchOutputAdditionalAttributeType]],
         "filters": NotRequired[FilterClauseTypeDef],
         "owningProjectIdentifier": NotRequired[str],
         "searchIn": NotRequired[Sequence[SearchInItemTypeDef]],
         "searchText": NotRequired[str],
         "sort": NotRequired[SearchSortTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 SearchListingsInputSearchListingsPaginateTypeDef = TypedDict(
     "SearchListingsInputSearchListingsPaginateTypeDef",
     {
         "domainIdentifier": str,
-        "additionalAttributes": NotRequired[Sequence[Literal["FORMS"]]],
+        "additionalAttributes": NotRequired[Sequence[SearchOutputAdditionalAttributeType]],
         "filters": NotRequired[FilterClauseTypeDef],
         "searchIn": NotRequired[Sequence[SearchInItemTypeDef]],
         "searchText": NotRequired[str],
         "sort": NotRequired[SearchSortTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
@@ -3240,22 +3365,24 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 GlueRunConfigurationInputTypeDef = TypedDict(
     "GlueRunConfigurationInputTypeDef",
     {
         "relationalFilterConfigurations": Sequence[RelationalFilterConfigurationTypeDef],
+        "autoImportDataQualityResult": NotRequired[bool],
         "dataAccessRole": NotRequired[str],
     },
 )
 GlueRunConfigurationOutputTypeDef = TypedDict(
     "GlueRunConfigurationOutputTypeDef",
     {
         "relationalFilterConfigurations": List[RelationalFilterConfigurationTypeDef],
         "accountId": NotRequired[str],
+        "autoImportDataQualityResult": NotRequired[bool],
         "dataAccessRole": NotRequired[str],
         "region": NotRequired[str],
     },
 )
 SearchTypesResultItemTypeDef = TypedDict(
     "SearchTypesResultItemTypeDef",
     {
@@ -3362,14 +3489,24 @@
         "subscriptionId": str,
         "subscriptionTargetId": str,
         "updatedAt": datetime,
         "updatedBy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+PostTimeSeriesDataPointsInputRequestTypeDef = TypedDict(
+    "PostTimeSeriesDataPointsInputRequestTypeDef",
+    {
+        "domainIdentifier": str,
+        "entityIdentifier": str,
+        "entityType": TimeSeriesEntityTypeType,
+        "forms": Sequence[TimeSeriesDataPointFormInputTypeDef],
+        "clientToken": NotRequired[str],
+    },
+)
 ProjectMemberTypeDef = TypedDict(
     "ProjectMemberTypeDef",
     {
         "designation": UserDesignationType,
         "memberDetails": MemberDetailsTypeDef,
     },
 )
@@ -3476,21 +3613,18 @@
     {
         "assetItem": NotRequired[AssetItemTypeDef],
         "dataProductItem": NotRequired[DataProductSummaryTypeDef],
         "glossaryItem": NotRequired[GlossaryItemTypeDef],
         "glossaryTermItem": NotRequired[GlossaryTermItemTypeDef],
     },
 )
-SearchListingsOutputTypeDef = TypedDict(
-    "SearchListingsOutputTypeDef",
+SearchResultItemTypeDef = TypedDict(
+    "SearchResultItemTypeDef",
     {
-        "items": List[SearchResultItemTypeDef],
-        "nextToken": str,
-        "totalMatchCount": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "assetListing": NotRequired[AssetListingItemTypeDef],
     },
 )
 GetListingOutputTypeDef = TypedDict(
     "GetListingOutputTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
@@ -3595,14 +3729,23 @@
     {
         "items": List[SearchInventoryResultItemTypeDef],
         "nextToken": str,
         "totalMatchCount": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SearchListingsOutputTypeDef = TypedDict(
+    "SearchListingsOutputTypeDef",
+    {
+        "items": List[SearchResultItemTypeDef],
+        "nextToken": str,
+        "totalMatchCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 AcceptSubscriptionRequestOutputTypeDef = TypedDict(
     "AcceptSubscriptionRequestOutputTypeDef",
     {
         "createdAt": datetime,
         "createdBy": str,
         "decisionComment": str,
         "domainId": str,
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/PKG-INFO` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-datazone
-Version: 1.34.75
-Summary: Type annotations for boto3.DataZone 1.34.75 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.77
+Summary: Type annotations for boto3.DataZone 1.34.77 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,15 +39,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-datazone.svg?color=blue)](https://pypi.org/project/mypy-boto3-datazone)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_datazone/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-datazone)](https://pepy.tech/project/mypy-boto3-datazone)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.DataZone 1.34.75](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
+[boto3.DataZone 1.34.77](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/datazone.html#DataZone)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -297,14 +297,15 @@
     ListNotificationsPaginator,
     ListProjectMembershipsPaginator,
     ListProjectsPaginator,
     ListSubscriptionGrantsPaginator,
     ListSubscriptionRequestsPaginator,
     ListSubscriptionTargetsPaginator,
     ListSubscriptionsPaginator,
+    ListTimeSeriesDataPointsPaginator,
     SearchPaginator,
     SearchGroupProfilesPaginator,
     SearchListingsPaginator,
     SearchTypesPaginator,
     SearchUserProfilesPaginator,
 )
 
@@ -351,14 +352,17 @@
 )
 list_subscription_targets_paginator: ListSubscriptionTargetsPaginator = client.get_paginator(
     "list_subscription_targets"
 )
 list_subscriptions_paginator: ListSubscriptionsPaginator = client.get_paginator(
     "list_subscriptions"
 )
+list_time_series_data_points_paginator: ListTimeSeriesDataPointsPaginator = client.get_paginator(
+    "list_time_series_data_points"
+)
 search_paginator: SearchPaginator = client.get_paginator("search")
 search_group_profiles_paginator: SearchGroupProfilesPaginator = client.get_paginator(
     "search_group_profiles"
 )
 search_listings_paginator: SearchListingsPaginator = client.get_paginator("search_listings")
 search_types_paginator: SearchTypesPaginator = client.get_paginator("search_types")
 search_user_profiles_paginator: SearchUserProfilesPaginator = client.get_paginator(
```

### Comparing `mypy-boto3-datazone-1.34.75/mypy_boto3_datazone.egg-info/SOURCES.txt` & `mypy-boto3-datazone-1.34.77/mypy_boto3_datazone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-datazone-1.34.75/setup.py` & `mypy-boto3-datazone-1.34.77/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-datazone",
-    version="1.34.75",
+    version="1.34.77",
     packages=["mypy_boto3_datazone"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.DataZone 1.34.75 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.DataZone 1.34.77 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

