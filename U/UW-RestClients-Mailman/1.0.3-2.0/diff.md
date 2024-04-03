# Comparing `tmp/UW-RestClients-Mailman-1.0.3.tar.gz` & `tmp/UW-RestClients-Mailman-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-Mailman-1.0.3.tar", last modified: Fri Feb 16 18:49:53 2024, max compression
+gzip compressed data, was "UW-RestClients-Mailman-2.0.tar", last modified: Wed Apr  3 20:17:40 2024, max compression
```

## Comparing `UW-RestClients-Mailman-1.0.3.tar` & `UW-RestClients-Mailman-2.0.tar`

### file list

```diff
@@ -1,45 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.343648 UW-RestClients-Mailman-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-16 18:49:53.343648 UW-RestClients-Mailman-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/UW_RestClients_Mailman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-02-16 18:49:53.000000 UW-RestClients-Mailman-1.0.3/UW_RestClients_Mailman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-16 18:49:53.000000 UW-RestClients-Mailman-1.0.3/UW_RestClients_Mailman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-16 18:49:53.000000 UW-RestClients-Mailman-1.0.3/UW_RestClients_Mailman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-16 18:49:53.000000 UW-RestClients-Mailman-1.0.3/UW_RestClients_Mailman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-16 18:49:53.000000 UW-RestClients-Mailman-1.0.3/UW_RestClients_Mailman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-16 18:49:53.343648 UW-RestClients-Mailman-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/uw_mailman/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-16 18:49:51.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/basic_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/course_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/dao.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/instructor_term_list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.339648 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.343648 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_bbio180a_au12
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_bbio180a_au13
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_bill_au13
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_math125g_su13
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_multi_bbio180a_au13
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_multi_math125a_su13
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_multi_math125g_su13
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_tbus310a_au13
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_tbus310a_sp13
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/term_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:53.343648 UW-RestClients-Mailman-1.0.3/uw_mailman/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/tests/test_basic_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/tests/test_course_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/tests/test_instructor_term_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-02-16 18:49:40.000000 UW-RestClients-Mailman-1.0.3/uw_mailman/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.716880 UW-RestClients-Mailman-2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 20:17:40.716880 UW-RestClients-Mailman-2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/UW_RestClients_Mailman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 20:17:40.000000 UW-RestClients-Mailman-2.0/UW_RestClients_Mailman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-03 20:17:40.000000 UW-RestClients-Mailman-2.0/UW_RestClients_Mailman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:17:40.000000 UW-RestClients-Mailman-2.0/UW_RestClients_Mailman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 20:17:40.000000 UW-RestClients-Mailman-2.0/UW_RestClients_Mailman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 20:17:40.000000 UW-RestClients-Mailman-2.0/UW_RestClients_Mailman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:17:40.716880 UW-RestClients-Mailman-2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 20:17:40.000000 UW-RestClients-Mailman-2.0/uw_mailman/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/basic_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/course_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/dao.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/instructor_term_list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_bbio180a_au12
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_bbio180a_au13
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_bill_au13
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_math125g_su13
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_multi_bbio180a_au13
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_multi_math125a_su13
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_multi_math125g_su13
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_tbus310a_au13
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/__mock_key__/admin/v1.0/uwnetid/available/_uwnetid_tbus310a_sp13
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.708880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/bbio180a_au12/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/bbio180a_au12/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/bbio180a_au13/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/bbio180a_au13/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/bbio180a_su13/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/bbio180a_su13/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/bill_au13/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/bill_au13/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/math125g_su13/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/math125g_su13/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/multi_bbio180a_au13/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/multi_bbio180a_au13/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/multi_math125a_su13/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/multi_math125a_su13/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/multi_math125g_su13/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/multi_math125g_su13/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.712880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/tbus310a_au13/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/tbus310a_au13/exists
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.716880 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/tbus310a_sp13/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/resources/mailman/file/uw_list_manager/api/v1/list/tbus310a_sp13/exists
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/term_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:40.716880 UW-RestClients-Mailman-2.0/uw_mailman/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/tests/test_basic_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/tests/test_course_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/tests/test_instructor_term_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 20:17:32.000000 UW-RestClients-Mailman-2.0/uw_mailman/util.py
```

### Comparing `UW-RestClients-Mailman-1.0.3/LICENSE` & `UW-RestClients-Mailman-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Mailman-1.0.3/PKG-INFO` & `UW-RestClients-Mailman-2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-Mailman
-Version: 1.0.3
+Version: 2.0
 Summary: A library for connecting to the mailman API
 Home-page: https://github.com/uw-it-aca/uw-restclients-mailman
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `UW-RestClients-Mailman-1.0.3/README.md` & `UW-RestClients-Mailman-2.0/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Mailman-1.0.3/UW_RestClients_Mailman.egg-info/PKG-INFO` & `UW-RestClients-Mailman-2.0/UW_RestClients_Mailman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UW-RestClients-Mailman
-Version: 1.0.3
+Version: 2.0
 Summary: A library for connecting to the mailman API
 Home-page: https://github.com/uw-it-aca/uw-restclients-mailman
 Author: UW-IT T&LS
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `UW-RestClients-Mailman-1.0.3/setup.py` & `UW-RestClients-Mailman-2.0/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Mailman-1.0.3/uw_mailman/__init__.py` & `UW-RestClients-Mailman-2.0/uw_mailman/__init__.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Mailman-1.0.3/uw_mailman/course_list.py` & `UW-RestClients-Mailman-2.0/uw_mailman/course_list.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Mailman-1.0.3/uw_mailman/instructor_term_list.py` & `UW-RestClients-Mailman-2.0/uw_mailman/instructor_term_list.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Mailman-1.0.3/uw_mailman/tests/test_basic_list.py` & `UW-RestClients-Mailman-2.0/uw_mailman/tests/test_basic_list.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 @fdao_mailman_override
 class TestMailmanBasicList(TestCase):
 
     def test_get_url_path(self):
         self.assertEqual(
             _get_url_path('aaa_au12'),
-            "/__mock_key__/admin/v1.0/uwnetid/available/?uwnetid=aaa_au12")
+            "/uw_list_manager/api/v1/list/aaa_au12/exists")
 
     def test_exists(self):
         self.assertFalse(exists('bbio180a_au12'))
         self.assertTrue(exists('bbio180a_au13'))
         self.assertFalse(exists("tbus310a_au13"))
         self.assertTrue(exists("bill_au13"))
```

### Comparing `UW-RestClients-Mailman-1.0.3/uw_mailman/tests/test_course_list.py` & `UW-RestClients-Mailman-2.0/uw_mailman/tests/test_course_list.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-Mailman-1.0.3/uw_mailman/tests/test_instructor_term_list.py` & `UW-RestClients-Mailman-2.0/uw_mailman/tests/test_instructor_term_list.py`

 * *Files identical despite different names*

