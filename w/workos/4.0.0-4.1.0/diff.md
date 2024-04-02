# Comparing `tmp/workos-4.0.0.tar.gz` & `tmp/workos-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workos-4.0.0.tar", last modified: Thu Mar 21 20:16:15 2024, max compression
+gzip compressed data, was "workos-4.1.0.tar", last modified: Tue Apr  2 23:20:33 2024, max compression
```

## Comparing `workos-4.0.0.tar` & `workos-4.1.0.tar`

### file list

```diff
@@ -1,61 +1,49 @@
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2024-03-21 20:16:15.355764 workos-4.0.0/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1063 2024-03-21 20:16:04.000000 workos-4.0.0/LICENSE
--rw-r--r--   0 semaphore  (1001) semaphore  (1001)     3031 2024-03-21 20:16:15.354764 workos-4.0.0/PKG-INFO
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1780 2024-03-21 20:16:04.000000 workos-4.0.0/README.md
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       38 2024-03-21 20:16:15.355764 workos-4.0.0/setup.cfg
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1662 2024-03-21 20:16:04.000000 workos-4.0.0/setup.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2024-03-21 20:16:15.349764 workos-4.0.0/tests/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     8754 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_audit_logs.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3562 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_client.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    20293 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_directory_sync.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1342 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_events.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    10171 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_mfa.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    11468 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_organizations.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1479 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_passwordless.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1688 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_portal.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    21555 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_sso.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    33820 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_user_management.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4717 2024-03-21 20:16:04.000000 workos-4.0.0/tests/test_webhooks.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2024-03-21 20:16:15.351764 workos-4.0.0/workos/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      405 2024-03-21 20:16:04.000000 workos-4.0.0/workos/__about__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      207 2024-03-21 20:16:04.000000 workos-4.0.0/workos/__init__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     4328 2024-03-21 20:16:04.000000 workos-4.0.0/workos/audit_logs.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2130 2024-03-21 20:16:04.000000 workos-4.0.0/workos/client.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    17286 2024-03-21 20:16:04.000000 workos-4.0.0/workos/directory_sync.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2233 2024-03-21 20:16:04.000000 workos-4.0.0/workos/events.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2719 2024-03-21 20:16:04.000000 workos-4.0.0/workos/exceptions.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     7334 2024-03-21 20:16:04.000000 workos-4.0.0/workos/mfa.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     8615 2024-03-21 20:16:04.000000 workos-4.0.0/workos/organizations.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2674 2024-03-21 20:16:04.000000 workos-4.0.0/workos/passwordless.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1813 2024-03-21 20:16:04.000000 workos-4.0.0/workos/portal.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2024-03-21 20:16:15.352764 workos-4.0.0/workos/resources/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/__init__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      806 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/audit_logs_export.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1024 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/base.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2634 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/directory_sync.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1101 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/event.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      339 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/event_action.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3009 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/list.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3170 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/mfa.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      762 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/organizations.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      843 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/passwordless.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     2261 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/sso.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3983 2024-03-21 20:16:04.000000 workos-4.0.0/workos/resources/user_management.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    12585 2024-03-21 20:16:04.000000 workos-4.0.0/workos/sso.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)    37275 2024-03-21 20:16:04.000000 workos-4.0.0/workos/user_management.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2024-03-21 20:16:15.353764 workos-4.0.0/workos/utils/
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        0 2024-03-21 20:16:04.000000 workos-4.0.0/workos/utils/__init__.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1458 2024-03-21 20:16:04.000000 workos-4.0.0/workos/utils/connection_types.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)       77 2024-03-21 20:16:04.000000 workos-4.0.0/workos/utils/pagination_order.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3130 2024-03-21 20:16:04.000000 workos-4.0.0/workos/utils/request.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      155 2024-03-21 20:16:04.000000 workos-4.0.0/workos/utils/sso_provider_types.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      190 2024-03-21 20:16:04.000000 workos-4.0.0/workos/utils/um_provider_types.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1606 2024-03-21 20:16:04.000000 workos-4.0.0/workos/utils/validation.py
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     3280 2024-03-21 20:16:04.000000 workos-4.0.0/workos/webhooks.py
-drwxrwxr-x   0 semaphore  (1001) semaphore  (1001)        0 2024-03-21 20:16:15.353764 workos-4.0.0/workos.egg-info/
--rw-r--r--   0 semaphore  (1001) semaphore  (1001)     3031 2024-03-21 20:16:15.000000 workos-4.0.0/workos.egg-info/PKG-INFO
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)     1315 2024-03-21 20:16:15.000000 workos-4.0.0/workos.egg-info/SOURCES.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2024-03-21 20:16:15.000000 workos-4.0.0/workos.egg-info/dependency_links.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        1 2024-03-21 20:16:14.000000 workos-4.0.0/workos.egg-info/not-zip-safe
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)      166 2024-03-21 20:16:15.000000 workos-4.0.0/workos.egg-info/requires.txt
--rw-rw-r--   0 semaphore  (1001) semaphore  (1001)        7 2024-03-21 20:16:15.000000 workos-4.0.0/workos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.309790 workos-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 23:20:25.000000 workos-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-02 23:20:33.309790 workos-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-02 23:20:25.000000 workos-4.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:20:33.309790 workos-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-04-02 23:20:25.000000 workos-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.305790 workos-4.1.0/workos/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-02 23:20:25.000000 workos-4.1.0/workos/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 23:20:25.000000 workos-4.1.0/workos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4328 2024-04-02 23:20:25.000000 workos-4.1.0/workos/audit_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-02 23:20:25.000000 workos-4.1.0/workos/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17286 2024-04-02 23:20:25.000000 workos-4.1.0/workos/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-02 23:20:25.000000 workos-4.1.0/workos/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-02 23:20:25.000000 workos-4.1.0/workos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7334 2024-04-02 23:20:25.000000 workos-4.1.0/workos/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-04-02 23:20:25.000000 workos-4.1.0/workos/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-02 23:20:25.000000 workos-4.1.0/workos/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-02 23:20:25.000000 workos-4.1.0/workos/portal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.309790 workos-4.1.0/workos/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/audit_logs_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/directory_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/event_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/passwordless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4872 2024-04-02 23:20:25.000000 workos-4.1.0/workos/resources/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-02 23:20:25.000000 workos-4.1.0/workos/sso.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38748 2024-04-02 23:20:25.000000 workos-4.1.0/workos/user_management.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.309790 workos-4.1.0/workos/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/connection_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/pagination_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/sso_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/um_provider_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-02 23:20:25.000000 workos-4.1.0/workos/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-04-02 23:20:25.000000 workos-4.1.0/workos/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:20:33.309790 workos-4.1.0/workos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2615 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:20:31.000000 workos-4.1.0/workos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 23:20:33.000000 workos-4.1.0/workos.egg-info/top_level.txt
```

### Comparing `workos-4.0.0/LICENSE` & `workos-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/PKG-INFO` & `workos-4.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.0.0
+Version: 4.1.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.22.0
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pytest==4.6.9; extra == "dev"
-Requires-Dist: pytest-cov==2.8.1; extra == "dev"
-Requires-Dist: six==1.13.0; extra == "dev"
-Requires-Dist: black==22.3.0; extra == "dev"
-Requires-Dist: twine==4.0.2; extra == "dev"
-Requires-Dist: requests==2.30.0; extra == "dev"
-Requires-Dist: urllib3==2.0.2; extra == "dev"
-Requires-Dist: enum34; python_version < "3.4"
+License-File: LICENSE
 
 # WorkOS Python Library
 
 ![PyPI](https://img.shields.io/pypi/v/workos)
 [![Build Status](https://workos.semaphoreci.com/badges/workos-python/branches/main.svg?style=shields&key=9e4cb5bb-86a4-4938-9ec2-fc9f9fc512be)](https://workos.semaphoreci.com/projects/workos-python)
 
 The WorkOS library for Python provides convenient access to the WorkOS API from applications written in Python, [hosted on PyPi](https://pypi.org/project/workos/)
@@ -73,7 +64,9 @@
 
 ## More Information
 
 - [Single Sign-On Guide](https://workos.com/docs/sso/guide)
 - [Directory Sync Guide](https://workos.com/docs/directory-sync/guide)
 - [Admin Portal Guide](https://workos.com/docs/admin-portal/guide)
 - [Magic Link Guide](https://workos.com/docs/magic-link/guide)
+
+
```

### Comparing `workos-4.0.0/README.md` & `workos-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/setup.py` & `workos-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     ),
     zip_safe=False,
     license=about["__license__"],
     install_requires=["requests>=2.22.0"],
     extras_require={
         "dev": [
             "flake8",
-            "pytest==4.6.9",
+            "pytest==8.1.1",
             "pytest-cov==2.8.1",
             "six==1.13.0",
             "black==22.3.0",
             "twine==4.0.2",
             "requests==2.30.0",
             "urllib3==2.0.2",
         ],
```

### Comparing `workos-4.0.0/workos/audit_logs.py` & `workos-4.1.0/workos/audit_logs.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/client.py` & `workos-4.1.0/workos/client.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/directory_sync.py` & `workos-4.1.0/workos/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/events.py` & `workos-4.1.0/workos/events.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/exceptions.py` & `workos-4.1.0/workos/exceptions.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/mfa.py` & `workos-4.1.0/workos/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/organizations.py` & `workos-4.1.0/workos/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/passwordless.py` & `workos-4.1.0/workos/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/portal.py` & `workos-4.1.0/workos/portal.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/audit_logs_export.py` & `workos-4.1.0/workos/resources/audit_logs_export.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/base.py` & `workos-4.1.0/workos/resources/base.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/directory_sync.py` & `workos-4.1.0/workos/resources/directory_sync.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/event.py` & `workos-4.1.0/workos/resources/event.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/list.py` & `workos-4.1.0/workos/resources/list.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/mfa.py` & `workos-4.1.0/workos/resources/mfa.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/organizations.py` & `workos-4.1.0/workos/resources/organizations.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/passwordless.py` & `workos-4.1.0/workos/resources/passwordless.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/sso.py` & `workos-4.1.0/workos/resources/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/resources/user_management.py` & `workos-4.1.0/workos/resources/user_management.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,17 @@
     """Representation of a User and Organization ID response as returned by WorkOS through User Management features."""
 
     """Attributes:
         OBJECT_FIELDS (list): List of fields a WorkOSAuthenticationResponse comprises.
     """
 
     OBJECT_FIELDS = [
+        "access_token",
         "organization_id",
+        "refresh_token",
     ]
 
     @classmethod
     def construct_from_response(cls, response):
         authentication_response = super(
             WorkOSAuthenticationResponse, cls
         ).construct_from_response(response)
@@ -41,14 +43,42 @@
 
         if self.impersonator:
             authentication_response_dict["impersonator"] = self.impersonator.to_dict()
 
         return authentication_response_dict
 
 
+class WorkOSRefreshTokenAuthenticationResponse(WorkOSBaseResource):
+    """Representation of refresh token authentication response as returned by WorkOS through User Management features."""
+
+    """Attributes:
+        OBJECT_FIELDS (list): List of fields a WorkOSRefreshTokenAuthenticationResponse comprises.
+    """
+
+    OBJECT_FIELDS = [
+        "access_token",
+        "refresh_token",
+    ]
+
+    @classmethod
+    def construct_from_response(cls, response):
+        authentication_response = super(
+            WorkOSRefreshTokenAuthenticationResponse, cls
+        ).construct_from_response(response)
+
+        return authentication_response
+
+    def to_dict(self):
+        authentication_response_dict = super(
+            WorkOSRefreshTokenAuthenticationResponse, self
+        ).to_dict()
+
+        return authentication_response_dict
+
+
 class WorkOSInvitation(WorkOSBaseResource):
     """Representation of an Invitation as returned by WorkOS through User Management features.
 
     Attributes:
         OBJECT_FIELDS (list): List of fields a WorkOSInvitation comprises.
     """
```

### Comparing `workos-4.0.0/workos/sso.py` & `workos-4.1.0/workos/sso.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/user_management.py` & `workos-4.1.0/workos/user_management.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from requests import Request
 import workos
 from workos.resources.list import WorkOSListResource
 from workos.resources.mfa import WorkOSAuthenticationFactorTotp, WorkOSChallenge
 from workos.resources.user_management import (
     WorkOSAuthenticationResponse,
+    WorkOSRefreshTokenAuthenticationResponse,
     WorkOSInvitation,
     WorkOSOrganizationMembership,
     WorkOSPasswordChallengeResponse,
     WorkOSUser,
 )
 from workos.utils.pagination_order import Order
 from workos.utils.um_provider_types import UserManagementProviderType
@@ -705,14 +706,59 @@
             method=REQUEST_METHOD_POST,
             headers=headers,
             params=payload,
         )
 
         return WorkOSAuthenticationResponse.construct_from_response(response).to_dict()
 
+    def authenticate_with_refresh_token(
+        self,
+        refresh_token,
+        ip_address=None,
+        user_agent=None,
+    ):
+        """Authenticates a user with a refresh token.
+
+        Kwargs:
+            refresh_token (str): The token associated to the user.
+            ip_address (str): The IP address of the request from the user who is attempting to authenticate. (Optional)
+            user_agent (str): The user agent of the request from the user who is attempting to authenticate. (Optional)
+
+        Returns:
+            (dict): Refresh Token Authentication response from WorkOS.
+                [access_token] (str): The refreshed access token
+                [refresh_token] (str): The new refresh token.
+        """
+
+        headers = {}
+
+        payload = {
+            "client_id": workos.client_id,
+            "client_secret": workos.api_key,
+            "refresh_token": refresh_token,
+            "grant_type": "refresh_token",
+        }
+
+        if ip_address:
+            payload["ip_address"] = ip_address
+
+        if user_agent:
+            payload["user_agent"] = user_agent
+
+        response = self.request_helper.request(
+            USER_AUTHENTICATE_PATH,
+            method=REQUEST_METHOD_POST,
+            headers=headers,
+            params=payload,
+        )
+
+        return WorkOSRefreshTokenAuthenticationResponse.construct_from_response(
+            response
+        ).to_dict()
+
     def send_password_reset_email(
         self,
         email,
         password_reset_url,
     ):
         """Sends a password reset email to a user.
```

### Comparing `workos-4.0.0/workos/utils/connection_types.py` & `workos-4.1.0/workos/utils/connection_types.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/utils/request.py` & `workos-4.1.0/workos/utils/request.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/utils/validation.py` & `workos-4.1.0/workos/utils/validation.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos/webhooks.py` & `workos-4.1.0/workos/webhooks.py`

 * *Files identical despite different names*

### Comparing `workos-4.0.0/workos.egg-info/PKG-INFO` & `workos-4.1.0/workos.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,30 @@
 Metadata-Version: 2.1
 Name: workos
-Version: 4.0.0
+Version: 4.1.0
 Summary: WorkOS Python Client
 Home-page: https://github.com/workos-inc/workos-python
 Author: WorkOS
 Author-email: team@workos.com
 License: MIT
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.22.0
 Provides-Extra: dev
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: pytest==4.6.9; extra == "dev"
-Requires-Dist: pytest-cov==2.8.1; extra == "dev"
-Requires-Dist: six==1.13.0; extra == "dev"
-Requires-Dist: black==22.3.0; extra == "dev"
-Requires-Dist: twine==4.0.2; extra == "dev"
-Requires-Dist: requests==2.30.0; extra == "dev"
-Requires-Dist: urllib3==2.0.2; extra == "dev"
-Requires-Dist: enum34; python_version < "3.4"
+License-File: LICENSE
 
 # WorkOS Python Library
 
 ![PyPI](https://img.shields.io/pypi/v/workos)
 [![Build Status](https://workos.semaphoreci.com/badges/workos-python/branches/main.svg?style=shields&key=9e4cb5bb-86a4-4938-9ec2-fc9f9fc512be)](https://workos.semaphoreci.com/projects/workos-python)
 
 The WorkOS library for Python provides convenient access to the WorkOS API from applications written in Python, [hosted on PyPi](https://pypi.org/project/workos/)
@@ -73,7 +64,9 @@
 
 ## More Information
 
 - [Single Sign-On Guide](https://workos.com/docs/sso/guide)
 - [Directory Sync Guide](https://workos.com/docs/directory-sync/guide)
 - [Admin Portal Guide](https://workos.com/docs/admin-portal/guide)
 - [Magic Link Guide](https://workos.com/docs/magic-link/guide)
+
+
```

