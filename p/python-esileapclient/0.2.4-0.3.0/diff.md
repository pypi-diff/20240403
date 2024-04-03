# Comparing `tmp/python-esileapclient-0.2.4.tar.gz` & `tmp/python-esileapclient-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/tzumainn/development/python-esileapclient/dist/tmpgxlvyxk4/python-esileapclient-0.2.4.tar", last modified: Tue Mar 26 13:13:01 2024, max compression
+gzip compressed data, was "/home/tzumainn/development/python-esileapclient/dist/tmpllk7bwqj/python-esileapclient-0.3.0.tar", last modified: Wed Apr  3 14:14:24 2024, max compression
```

## Comparing `python-esileapclient-0.2.4.tar` & `python-esileapclient-0.3.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/.github/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/.github/workflows/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      616 2023-06-02 12:59:58.000000 python-esileapclient-0.2.4/.github/workflows/tests.yml
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/common/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/common/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     6595 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/common/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3453 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/common/http.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/osc/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/mdc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/mdc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3765 2023-07-12 20:08:01.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/mdc/mdc_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8043 2022-07-25 14:22:51.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/mdc/mdc_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2793 2023-07-12 20:08:01.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7997 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1798 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9366 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/osc/v1/offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/osc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2033 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/osc/plugin.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/utils/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/utils/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1056 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/utils/dummy_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3162 2023-06-02 12:59:58.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/utils/esi_interfaces.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1412 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/utils/output_utils.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    19558 2023-06-02 12:59:58.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/v1/test_basic.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9801 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/v1/test_policy.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10562 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/v1/test_sublease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    25162 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/v1/test_time.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2730 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7658 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/functional/base.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/common/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/common/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9296 2023-06-02 12:59:58.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/common/test_base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3007 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/common/test_http.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/mdc/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/mdc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5936 2023-07-12 20:08:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/mdc/test_mdc_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13531 2023-07-12 20:08:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/mdc/test_mdc_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1059 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/base.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3474 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/fakes.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2027 2023-07-12 20:08:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/test_event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10041 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/test_lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2831 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/test_node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10921 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/test_offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2326 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/osc/test_plugin.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1505 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/v1/test_client.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/unit/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/tests/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/esileapclient/v1/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/v1/__init__.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1795 2023-07-12 20:08:01.000000 python-esileapclient-0.2.4/esileapclient/v1/client.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2232 2023-07-12 20:08:01.000000 python-esileapclient-0.2.4/esileapclient/v1/event.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3910 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/v1/lease.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2283 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/v1/node.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4275 2024-03-26 13:12:29.000000 python-esileapclient-0.2.4/esileapclient/v1/offer.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      674 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/esileapclient/__init__.py
-drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3032 2024-03-26 13:13:00.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/PKG-INFO
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2495 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/SOURCES.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-03-26 13:13:00.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/dependency_links.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      900 2024-03-26 13:13:00.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/entry_points.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-07-25 14:25:40.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/not-zip-safe
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2024-03-26 13:13:00.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/pbr.json
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       81 2024-03-26 13:13:00.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/requires.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       14 2024-03-26 13:13:00.000000 python-esileapclient-0.2.4/python_esileapclient.egg-info/top_level.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      358 2024-03-26 13:13:00.000000 python-esileapclient-0.2.4/AUTHORS
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2415 2024-03-26 13:13:00.000000 python-esileapclient-0.2.4/ChangeLog
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11357 2022-06-16 16:55:03.000000 python-esileapclient-0.2.4/LICENSE
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2054 2022-07-25 14:22:51.000000 python-esileapclient-0.2.4/README.md
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      932 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/conftest.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       94 2023-07-12 20:08:01.000000 python-esileapclient-0.2.4/requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1739 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/setup.cfg
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1169 2022-06-16 16:55:03.000000 python-esileapclient-0.2.4/setup.py
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      259 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/test-requirements.txt
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      969 2022-06-16 16:54:31.000000 python-esileapclient-0.2.4/tox.ini
--rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3032 2024-03-26 13:13:01.000000 python-esileapclient-0.2.4/PKG-INFO
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/.github/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/.github/workflows/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      616 2023-06-02 12:59:58.000000 python-esileapclient-0.3.0/.github/workflows/tests.yml
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/common/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/common/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7929 2024-04-03 14:13:09.000000 python-esileapclient-0.3.0/esileapclient/common/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3453 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/common/http.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/osc/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/mdc/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/mdc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3765 2023-07-12 20:08:01.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/mdc/mdc_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     8043 2022-07-25 14:22:51.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/mdc/mdc_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2793 2023-07-12 20:08:01.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9004 2024-04-03 14:13:09.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1798 2024-03-26 13:12:29.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9366 2024-03-26 13:12:29.000000 python-esileapclient-0.3.0/esileapclient/osc/v1/offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/osc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2033 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/osc/plugin.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/utils/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/utils/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1056 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/utils/dummy_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3162 2023-06-02 12:59:58.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/utils/esi_interfaces.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1412 2024-03-26 13:12:29.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/utils/output_utils.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    19558 2023-06-02 12:59:58.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/v1/test_basic.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     9801 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/v1/test_policy.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10562 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/v1/test_sublease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    25162 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/v1/test_time.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2730 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     7658 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/functional/base.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/common/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/common/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10445 2024-04-03 14:13:09.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/common/test_base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3007 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/common/test_http.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/mdc/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/mdc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     5936 2023-07-12 20:08:01.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/mdc/test_mdc_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    13531 2023-07-12 20:08:01.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/mdc/test_mdc_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1059 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/base.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3474 2024-03-26 13:12:29.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/fakes.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2027 2023-07-12 20:08:01.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/test_event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11062 2024-04-03 14:13:09.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/test_lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2831 2024-03-26 13:12:29.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/test_node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    10921 2024-03-26 13:12:29.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/test_offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2326 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/osc/test_plugin.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1505 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/v1/test_client.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/unit/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/tests/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/esileapclient/v1/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        0 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/v1/__init__.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1795 2023-07-12 20:08:01.000000 python-esileapclient-0.3.0/esileapclient/v1/client.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2232 2023-07-12 20:08:01.000000 python-esileapclient-0.3.0/esileapclient/v1/event.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4305 2024-04-03 14:13:09.000000 python-esileapclient-0.3.0/esileapclient/v1/lease.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2283 2024-03-26 13:12:29.000000 python-esileapclient-0.3.0/esileapclient/v1/node.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     4275 2024-03-26 13:12:29.000000 python-esileapclient-0.3.0/esileapclient/v1/offer.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      674 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/esileapclient/__init__.py
+drwxrwxr-x   0 tzumainn  (3390) tzumainn  (3390)        0 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3032 2024-04-03 14:14:23.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/PKG-INFO
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2495 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2024-04-03 14:14:23.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      958 2024-04-03 14:14:23.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/entry_points.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)        1 2022-07-25 14:25:40.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/not-zip-safe
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       47 2024-04-03 14:14:23.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/pbr.json
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       81 2024-04-03 14:14:23.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/requires.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       14 2024-04-03 14:14:23.000000 python-esileapclient-0.3.0/python_esileapclient.egg-info/top_level.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      358 2024-04-03 14:14:23.000000 python-esileapclient-0.3.0/AUTHORS
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2460 2024-04-03 14:14:23.000000 python-esileapclient-0.3.0/ChangeLog
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)    11357 2022-06-16 16:55:03.000000 python-esileapclient-0.3.0/LICENSE
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     2054 2022-07-25 14:22:51.000000 python-esileapclient-0.3.0/README.md
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      932 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/conftest.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)       94 2023-07-12 20:08:01.000000 python-esileapclient-0.3.0/requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1798 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/setup.cfg
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     1169 2022-06-16 16:55:03.000000 python-esileapclient-0.3.0/setup.py
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      259 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/test-requirements.txt
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)      969 2022-06-16 16:54:31.000000 python-esileapclient-0.3.0/tox.ini
+-rw-rw-r--   0 tzumainn  (3390) tzumainn  (3390)     3032 2024-04-03 14:14:24.000000 python-esileapclient-0.3.0/PKG-INFO
```

### Comparing `python-esileapclient-0.2.4/.github/workflows/tests.yml` & `python-esileapclient-0.3.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/common/base.py` & `python-esileapclient-0.3.0/esileapclient/common/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -92,14 +92,47 @@
         resp, body = self.api.json_request('POST', url, body=new, **headers)
 
         if resp.status_code == 201:
             return self.resource_class(self, body)
         else:
             raise exceptions.CommandError(json.loads(resp.text)['faultstring'])
 
+    def _update(self, resource_id, os_esileap_api_version=None, **kwargs):
+        """Update a resource based on a kwargs dictionary of attributes.
+        :param kwargs: A dictionary containing the attributes of the resource
+                       that will be updated.
+        """
+
+        new = {}
+        invalid = []
+        for (key, value) in kwargs.items():
+            if key in self.resource_class._update_attributes:
+                new[key] = value
+            else:
+                invalid.append(key)
+        if invalid:
+            raise Exception('The attribute(s) "%(attrs)s" '
+                            'are invalid; they are not '
+                            'needed to update %(resource)s.' %
+                            {'resource': self._resource_name,
+                             'attrs': '","'.join(invalid)})
+
+        headers = {}
+        if os_esileap_api_version is not None:
+            headers['headers'] = {'X-OpenStack-ESI-Leap-API-Version':
+                                  os_esileap_api_version}
+
+        url = self._path(resource_id)
+        resp, body = self.api.json_request('PATCH', url, body=new, **headers)
+
+        if resp.status_code == 200:
+            return self.resource_class(self, body)
+        else:
+            raise exceptions.CommandError(json.loads(resp.text)['faultstring'])
+
     def _list(self, url, obj_class=None, os_esileap_api_version=None):
         if obj_class is None:
             obj_class = self.resource_class
 
         kwargs = {}
 
         if os_esileap_api_version is not None:
```

### Comparing `python-esileapclient-0.2.4/esileapclient/common/http.py` & `python-esileapclient-0.3.0/esileapclient/common/http.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/osc/v1/mdc/mdc_lease.py` & `python-esileapclient-0.3.0/esileapclient/osc/v1/mdc/mdc_lease.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/osc/v1/mdc/mdc_offer.py` & `python-esileapclient-0.3.0/esileapclient/osc/v1/mdc/mdc_offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/osc/v1/event.py` & `python-esileapclient-0.3.0/esileapclient/osc/v1/event.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/osc/v1/lease.py` & `python-esileapclient-0.3.0/esileapclient/osc/v1/lease.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,14 +84,48 @@
 
         data = dict([(f, getattr(lease, f, '')) for f in
                     LEASE_RESOURCE.fields])
 
         return self.dict2columns(data)
 
 
+class UpdateLease(command.ShowOne):
+    """Update a lease."""
+
+    log = logging.getLogger(__name__ + ".UpdateLease")
+
+    def get_parser(self, prog_name):
+        parser = super(UpdateLease, self).get_parser(prog_name)
+
+        parser.add_argument(
+            "uuid",
+            metavar="<uuid>",
+            help="UUID of the lease")
+        parser.add_argument(
+            '--end-time',
+            dest='end_time',
+            required=False,
+            help="Time when the lease will expire.")
+        return parser
+
+    def take_action(self, parsed_args):
+        client = self.app.client_manager.lease
+
+        field_list = LEASE_RESOURCE._update_attributes
+        fields = dict((k, v) for (k, v) in vars(parsed_args).items()
+                      if k in field_list and v is not None)
+
+        lease = client.lease.update(parsed_args.uuid, **fields)
+
+        data = dict([(f, getattr(lease, f, '')) for f in
+                    LEASE_RESOURCE.fields])
+
+        return self.dict2columns(data)
+
+
 class ListLease(command.Lister):
     """List leases."""
 
     log = logging.getLogger(__name__ + ".ListLease")
 
     def get_parser(self, prog_name):
         parser = super(ListLease, self).get_parser(prog_name)
```

### Comparing `python-esileapclient-0.2.4/esileapclient/osc/v1/node.py` & `python-esileapclient-0.3.0/esileapclient/osc/v1/node.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/osc/v1/offer.py` & `python-esileapclient-0.3.0/esileapclient/osc/v1/offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/osc/plugin.py` & `python-esileapclient-0.3.0/esileapclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/utils/dummy_node.py` & `python-esileapclient-0.3.0/esileapclient/tests/functional/utils/dummy_node.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/utils/esi_interfaces.py` & `python-esileapclient-0.3.0/esileapclient/tests/functional/utils/esi_interfaces.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/utils/output_utils.py` & `python-esileapclient-0.3.0/esileapclient/tests/functional/utils/output_utils.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/v1/test_basic.py` & `python-esileapclient-0.3.0/esileapclient/tests/functional/v1/test_basic.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/v1/test_policy.py` & `python-esileapclient-0.3.0/esileapclient/tests/functional/v1/test_policy.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/v1/test_sublease.py` & `python-esileapclient-0.3.0/esileapclient/tests/functional/v1/test_sublease.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/v1/test_time.py` & `python-esileapclient-0.3.0/esileapclient/tests/functional/v1/test_time.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/README.md` & `python-esileapclient-0.3.0/esileapclient/tests/functional/README.md`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/functional/base.py` & `python-esileapclient-0.3.0/esileapclient/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/common/test_base.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/common/test_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,22 @@
     'attribute2': '4',
 }
 
 
 CREATE_FAKE_RESOURCE = copy.deepcopy(FAKE_RESOURCE)
 del CREATE_FAKE_RESOURCE['uuid']
 
+UPDATE_FAKE_RESOURCE = {
+    'attribute1': '5',
+}
+
+INVALID_UPDATE_FAKE_RESOURCE = {
+    'attribute2': '6',
+}
+
 INVALID_ATTRIBUTE_FAKE_RESOURCE = {
     'non-existent-attribute': 'bad',
     'attribute1': '1',
     'attribute2': '2',
 }
 
 
@@ -69,14 +77,15 @@
         'uuid': 'UUID',
         'attribute1': 'Attribute 1',
         'attribute2': 'Attribute 2',
         'attribute3': 'Attribute 3',
     }
 
     _creation_attributes = ['attribute1', 'attribute2']
+    _update_attributes = ['attribute1']
 
     def __repr__(self):
         return "<FakeResource %s>" % self._info
 
 
 class FakeResourceManager(base.Manager):
     resource_class = FakeResource
@@ -129,14 +138,42 @@
         with mock.patch.object(manager, 'api'):
 
             self.assertRaises(
                 Exception,
                 manager._create,
                 **INVALID_ATTRIBUTE_FAKE_RESOURCE)
 
+    def test__update(self):
+        manager = FakeResourceManager(None)
+        with mock.patch.object(manager, 'api') as mock_api:
+
+            mock_api.json_request.return_value = (
+                VALID_RESPONSE,
+                FAKE_RESOURCE)
+
+            resource = manager._update(FAKE_RESOURCE['uuid'],
+                                       **UPDATE_FAKE_RESOURCE)
+
+            mock_api.json_request.assert_called_once_with(
+                'PATCH', '/v1/fakeresources/%s' % FAKE_RESOURCE['uuid'],
+                **{'body': UPDATE_FAKE_RESOURCE})
+
+            self.assertIsInstance(resource, FakeResource)
+            self.assertEqual(resource._info, FAKE_RESOURCE)
+
+    def test__update_with_invalid_attribute(self):
+        manager = FakeResourceManager(None)
+        with mock.patch.object(manager, 'api'):
+
+            self.assertRaises(
+                Exception,
+                manager._update,
+                FAKE_RESOURCE['uuid'],
+                **INVALID_UPDATE_FAKE_RESOURCE)
+
     def test__list(self):
 
         manager = FakeResourceManager(None)
         with mock.patch.object(manager, 'api') as mock_api:
 
             mock_api.json_request.return_value = (
                 VALID_RESPONSE,
```

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/common/test_http.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/common/test_http.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/mdc/test_mdc_lease.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/mdc/test_mdc_lease.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/mdc/test_mdc_offer.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/mdc/test_mdc_offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/base.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/fakes.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/fakes.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/test_event.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/test_event.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/test_lease.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/test_lease.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,14 +78,52 @@
             'start_time': fakes.lease_start_time,
             'purpose': fakes.lease_purpose,
         }
 
         self.client_mock.lease.create.assert_called_once_with(**args)
 
 
+class TestUpdateLease(TestLease):
+
+    def setUp(self):
+        super(TestUpdateLease, self).setUp()
+
+        self.client_mock.lease.update.return_value = (
+            base.FakeResource(copy.deepcopy(fakes.LEASE))
+        )
+
+        # Get the command object to test
+        self.cmd = lease.UpdateLease(self.app, None)
+
+    def test_lease_update(self):
+
+        arglist = [
+            fakes.lease_uuid,
+            '--end-time', fakes.lease_end_time,
+        ]
+
+        verifylist = [
+            ('uuid', fakes.lease_uuid),
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+
+        self.cmd.take_action(parsed_args)
+
+        self.client_mock.lease.update.assert_called_once_with(
+            fakes.lease_uuid, end_time=fakes.lease_end_time)
+
+    def test_update_show_no_id(self):
+        arglist = []
+        verifylist = []
+        self.assertRaises(osctestutils.ParserException,
+                          self.check_parser,
+                          self.cmd, arglist, verifylist)
+
+
 class TestLeaseList(TestLease):
 
     def setUp(self):
         super(TestLeaseList, self).setUp()
 
         self.client_mock.lease.list.return_value = [
             base.FakeResource(copy.deepcopy(fakes.LEASE))
```

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/test_node.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/test_node.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/v1/test_offer.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/v1/test_offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/osc/test_plugin.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/osc/test_plugin.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/tests/unit/v1/test_client.py` & `python-esileapclient-0.3.0/esileapclient/tests/unit/v1/test_client.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/v1/client.py` & `python-esileapclient-0.3.0/esileapclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/v1/event.py` & `python-esileapclient-0.3.0/esileapclient/v1/event.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/v1/lease.py` & `python-esileapclient-0.3.0/esileapclient/v1/lease.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,14 +71,15 @@
         'status': "Status",
         'purpose': "Purpose",
     }
 
     _creation_attributes = ['start_time', 'end_time', 'status', 'name',
                             'properties', 'project_id', 'resource_type',
                             'resource_uuid', 'purpose']
+    _update_attributes = ['end_time']
 
     def __repr__(self):
         return "<Lease %s>" % self._info
 
 
 class LeaseManager(base.Manager):
     resource_class = Lease
@@ -90,14 +91,26 @@
         """
 
         lease = self._create(os_esileap_api_version=os_esileap_api_version,
                              **kwargs)
 
         return lease
 
+    def update(self, lease_uuid, os_esileap_api_version=None, **kwargs):
+        """Update a lease based on a kwargs dictionary of attributes.
+        :returns: a :class: `Lease` object
+        """
+
+        lease = self._update(
+            lease_uuid,
+            os_esileap_api_version=os_esileap_api_version,
+            **kwargs)
+
+        return lease
+
     def list(self, filters, os_esileap_api_version=None):
         """Retrieve a list of leases.
         :returns: A list of leases.
         """
 
         resource_id = ""
```

### Comparing `python-esileapclient-0.2.4/esileapclient/v1/node.py` & `python-esileapclient-0.3.0/esileapclient/v1/node.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/v1/offer.py` & `python-esileapclient-0.3.0/esileapclient/v1/offer.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/esileapclient/__init__.py` & `python-esileapclient-0.3.0/esileapclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/python_esileapclient.egg-info/PKG-INFO` & `python-esileapclient-0.3.0/python_esileapclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esileapclient
-Version: 0.2.4
+Version: 0.3.0
 Summary: ESI-LEAP CLI
 Home-page: UNKNOWN
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

### Comparing `python-esileapclient-0.2.4/python_esileapclient.egg-info/SOURCES.txt` & `python-esileapclient-0.3.0/python_esileapclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/python_esileapclient.egg-info/entry_points.txt` & `python-esileapclient-0.3.0/python_esileapclient.egg-info/entry_points.txt`

 * *Files 22% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 [openstack.lease.v1]
 esi_event_list = esileapclient.osc.v1.event:ListEvent
 esi_lease_create = esileapclient.osc.v1.lease:CreateLease
 esi_lease_delete = esileapclient.osc.v1.lease:DeleteLease
 esi_lease_list = esileapclient.osc.v1.lease:ListLease
 esi_lease_show = esileapclient.osc.v1.lease:ShowLease
+esi_lease_update = esileapclient.osc.v1.lease:UpdateLease
 esi_mdc_lease_list = esileapclient.osc.v1.mdc.mdc_lease:MDCListLease
 esi_mdc_offer_claim = esileapclient.osc.v1.mdc.mdc_offer:MDCClaimOffer
 esi_mdc_offer_list = esileapclient.osc.v1.mdc.mdc_offer:MDCListOffer
 esi_node_list = esileapclient.osc.v1.node:ListNode
 esi_offer_claim = esileapclient.osc.v1.offer:ClaimOffer
 esi_offer_create = esileapclient.osc.v1.offer:CreateOffer
 esi_offer_delete = esileapclient.osc.v1.offer:DeleteOffer
```

### Comparing `python-esileapclient-0.2.4/ChangeLog` & `python-esileapclient-0.3.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+0.3.0
+-----
+
+* Added "lease update" command
+
 0.2.4
 -----
 
 * Add node properties/resource class to lease/offer/node results
 
 0.2.3
 -----
```

### Comparing `python-esileapclient-0.2.4/LICENSE` & `python-esileapclient-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/README.md` & `python-esileapclient-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/conftest.py` & `python-esileapclient-0.3.0/conftest.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/setup.cfg` & `python-esileapclient-0.3.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 [entry_points]
 openstack.cli.extension = 
 	lease = esileapclient.osc.plugin
 openstack.lease.v1 = 
 	esi_event_list = esileapclient.osc.v1.event:ListEvent
 	esi_lease_list = esileapclient.osc.v1.lease:ListLease
 	esi_lease_create = esileapclient.osc.v1.lease:CreateLease
+	esi_lease_update = esileapclient.osc.v1.lease:UpdateLease
 	esi_lease_show = esileapclient.osc.v1.lease:ShowLease
 	esi_lease_delete = esileapclient.osc.v1.lease:DeleteLease
 	esi_mdc_lease_list = esileapclient.osc.v1.mdc.mdc_lease:MDCListLease
 	esi_mdc_offer_claim = esileapclient.osc.v1.mdc.mdc_offer:MDCClaimOffer
 	esi_mdc_offer_list = esileapclient.osc.v1.mdc.mdc_offer:MDCListOffer
 	esi_node_list = esileapclient.osc.v1.node:ListNode
 	esi_offer_list = esileapclient.osc.v1.offer:ListOffer
```

### Comparing `python-esileapclient-0.2.4/setup.py` & `python-esileapclient-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/tox.ini` & `python-esileapclient-0.3.0/tox.ini`

 * *Files identical despite different names*

### Comparing `python-esileapclient-0.2.4/PKG-INFO` & `python-esileapclient-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-esileapclient
-Version: 0.2.4
+Version: 0.3.0
 Summary: ESI-LEAP CLI
 Home-page: UNKNOWN
 Author: ESI
 Author-email: esi@lists.massopen.cloud
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Classifier: Environment :: Console
```

