# Comparing `tmp/interva-0.0.6.tar.gz` & `tmp/interva-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interva-0.0.6.tar", last modified: Wed Jul 26 19:46:18 2023, max compression
+gzip compressed data, was "interva-0.0.7.tar", last modified: Wed Apr  3 20:19:45 2024, max compression
```

## Comparing `interva-0.0.6.tar` & `interva-0.0.7.tar`

### file list

```diff
@@ -1,271 +1,30 @@
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.772920 interva-0.0.6/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    35149 2022-07-29 15:44:16.000000 interva-0.0.6/LICENSE
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      114 2022-07-29 16:28:38.000000 interva-0.0.6/MANIFEST.in
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-07-26 19:46:18.772365 interva-0.0.6/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3462 2023-03-13 22:54:59.000000 interva-0.0.6/README.md
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.578948 interva-0.0.6/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.599965 interva-0.0.6/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.579188 interva-0.0.6/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.599252 interva-0.0.6/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.579523 interva-0.0.6/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.598685 interva-0.0.6/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.579941 interva-0.0.6/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.597729 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.580372 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.596719 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.580788 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.595670 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.581035 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.594922 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.581420 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.594058 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.581850 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.593126 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.582311 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.592180 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.582728 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.590935 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.583047 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.590116 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.583336 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.589309 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.583860 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.588163 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.584271 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.586759 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.584717 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.585646 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.608922 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.610404 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.613818 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.618613 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.619381 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.621820 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.626904 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.627820 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.631137 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.636053 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.637079 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.640105 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.644861 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.645796 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.648945 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.653357 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.654373 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.657408 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.662220 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.663450 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.666768 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.672169 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.673276 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.676437 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.681302 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.682403 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.687498 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.695228 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.696500 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.700135 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.705581 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.706673 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.709733 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.714236 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.715267 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.718343 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.722983 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.724007 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.726916 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.731541 interva-0.0.6/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.732793 interva-0.0.6/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.735636 interva-0.0.6/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.740044 interva-0.0.6/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.741051 interva-0.0.6/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.743906 interva-0.0.6/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.748310 interva-0.0.6/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.6/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.749281 interva-0.0.6/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/build/lib/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.6/build/lib/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19003 2023-07-10 20:59:55.000000 interva-0.0.6/build/lib/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.752115 interva-0.0.6/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/build/lib/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.6/build/lib/tests/test_utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.756702 interva-0.0.6/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.6/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-07-11 18:27:06.000000 interva-0.0.6/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.762835 interva-0.0.6/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.6/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   459264 2023-03-22 19:50:10.000000 interva-0.0.6/interva/data/probbase.xls
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   164661 2022-07-29 16:52:08.000000 interva-0.0.6/interva/data/probbaseV5_19.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   286521 2022-11-03 17:23:26.000000 interva-0.0.6/interva/data/randomva5.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.6/interva/exceptions.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    41483 2023-07-22 00:30:31.000000 interva-0.0.6/interva/interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    19116 2023-07-18 17:19:33.000000 interva-0.0.6/interva/utils.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.770901 interva-0.0.6/interva.egg-info/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    18050 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       26 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/requires.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       25 2023-07-26 19:46:18.000000 interva-0.0.6/interva.egg-info/top_level.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       87 2022-07-29 15:51:31.000000 interva-0.0.6/pyproject.toml
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       38 2023-07-26 19:46:18.773107 interva-0.0.6/setup.cfg
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1367 2023-03-13 22:54:59.000000 interva-0.0.6/setup.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-07-26 19:46:18.767465 interva-0.0.6/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.6/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.6/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.6/tests/test_interva5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4718 2023-07-11 18:18:34.000000 interva-0.0.6/tests/test_utils.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      570 2023-07-26 13:34:24.000000 interva-0.0.6/tests/tmp.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.162723 interva-0.0.7/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    35149 2022-07-29 15:44:16.000000 interva-0.0.7/LICENSE
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      126 2024-04-03 19:06:42.000000 interva-0.0.7/MANIFEST.in
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4514 2024-04-03 20:19:45.161797 interva-0.0.7/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     3462 2023-03-13 22:54:59.000000 interva-0.0.7/README.md
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1376 2024-04-03 19:07:52.000000 interva-0.0.7/pyproject.toml
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-03 20:19:45.163200 interva-0.0.7/setup.cfg
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-03 19:09:08.000000 interva-0.0.7/setup.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.139001 interva-0.0.7/src/
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.146562 interva-0.0.7/src/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      150 2023-02-09 17:14:38.000000 interva-0.0.7/src/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      290 2023-08-09 13:57:17.000000 interva-0.0.7/src/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.155549 interva-0.0.7/src/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     5724 2023-05-12 20:38:51.000000 interva-0.0.7/src/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   459264 2023-03-22 19:50:10.000000 interva-0.0.7/src/interva/data/probbase.xls
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   164661 2022-07-29 16:52:08.000000 interva-0.0.7/src/interva/data/probbaseV5_19.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   286521 2022-11-03 17:23:26.000000 interva-0.0.7/src/interva/data/randomva5.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      518 2023-05-11 15:53:16.000000 interva-0.0.7/src/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    42335 2024-04-03 19:51:03.000000 interva-0.0.7/src/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    19211 2024-04-03 19:24:32.000000 interva-0.0.7/src/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.159959 interva-0.0.7/src/interva.egg-info/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4514 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      542 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        1 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       26 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/requires.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        8 2024-04-03 20:19:45.000000 interva-0.0.7/src/interva.egg-info/top_level.txt
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 20:19:45.158764 interva-0.0.7/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     3833 2024-04-03 19:46:40.000000 interva-0.0.7/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    10772 2023-05-12 16:39:17.000000 interva-0.0.7/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     4733 2024-04-03 20:08:46.000000 interva-0.0.7/tests/test_utils.py
```

### Comparing `interva-0.0.6/LICENSE` & `interva-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `interva-0.0.6/PKG-INFO` & `interva-0.0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: interva
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python implementation of the InterVA Algorithm.
-Home-page: https://github.com/verbal-autopsy-software/interva
-Author: Sherry Zhao & Jason Thomas
-Author-email: zhao.3248@buckeyemail.osu.edu
+Author-email: Sherry Zhao <zhao.3248@buckeyemail.osu.edu>, Jason Thomas <jarathomas@gmail.com>
+Maintainer-email: Jason Thomas <jarathomas@gmail.com>
 License: GPLv3
+Project-URL: Homepage, https://github.com/verbal-autopsy-software/interva
+Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/interva/issues
+Keywords: verbal autopsy
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: vacheck
+Requires-Dist: xlrd
 
 # interva
 
 [![image](https://img.shields.io/pypi/pyversions/interva)](https://pypi.org/project/interva/)
 [![pytest](https://github.com/verbal-autopsy-software/interva/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/interva/actions)
 
 Python implementation of the InterVA algorithm for assigning causes of death to verbal autopsy data
```

### Comparing `interva-0.0.6/README.md` & `interva-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.7/src/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/exceptions.py` & `interva-0.0.7/src/interva/exceptions.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.7/src/interva/interva5.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from math import isclose
 from os import path, chdir, getcwd, mkdir
 from logging import INFO, FileHandler, getLogger
 from csv import writer
 import datetime
 from pkgutil import get_data
 from io import BytesIO
+import warnings
 
 from interva.data.causetext import CAUSETEXTV5
 from interva.utils import _get_dem_groups
 from vacheck.datacheck5 import datacheck5
 
 
 class InterVA5:
@@ -131,17 +132,17 @@
                 data_msg = "No VA records!\n"
             msg = "InterVA5:\n" + data_msg
             msg = msg + (f"HIV parameter is {self.hiv}\n"
                          f"Malaria parameter is {self.malaria}\n"
                          "No results (need to use run() method).")
             return msg
         else:
-            n_processed = self.results["VA5"].shape[0]
+            n_processed = self.va_input.shape[0]
             n_undetermined = sum(
-                self.results["VA5"]["CAUSE1"] == "Undetermined")
+                self.results["VA5"]["CAUSE1"] == " ")
             n_miss = n_processed - self.results["VA5"].shape[0]
             n_male = sum(self.dem_group["sex"] == "male")
             n_female = sum(self.dem_group["sex"] == "female")
             n_adult = sum(self.dem_group["age"] == "adult")
             n_child = sum(self.dem_group["age"] == "child")
             n_neo = sum(self.dem_group["age"] == "neonate")
             msg = ("InterVA5:\n"
@@ -409,24 +410,33 @@
             input_current[:][input_current[:] == "1"] = 1
 
             input_current[0] = 0
             if nansum(input_current[5:12]) < 1:
                 if self.write:
                     logger.info(index_current +
                                 " Error in age indicator: Not Specified")
+                if self.openva_app:
+                    progress = int(100 * k / N)
+                    self.openva_app.emit(progress)
                 continue
             if nansum(input_current[3:5]) < 1:
                 if self.write:
                     logger.info(index_current +
                                 " Error in sex indicator: Not Specified")
+                if self.openva_app:
+                    progress = int(100 * k / N)
+                    self.openva_app.emit(progress)
                 continue
             if nansum(input_current[20:328]) < 1:
                 if self.write:
                     logger.info(index_current +
                                 " Error in indicators: No symptoms specified")
+                if self.openva_app:
+                    progress = int(100 * k / N)
+                    self.openva_app.emit(progress)
                 continue
 
             input_current = Series(input_current, index=va_input_names)
             tmp = datacheck5(va_input=input_current, va_id=index_current,
                              probbase=pb_for_datacheck)
 
             list_dem_group.append(_get_dem_groups(tmp["output"]))
@@ -539,15 +549,15 @@
             comnum = None
             if nansum(prob_C) > 0:
                 prob_C = prob_C / nansum(prob_C)
             if nanmax(prob_C) < 0.5:
                 comcat = "Multiple"
                 comnum = " "
             if nanmax(prob_C) >= 0.5:
-                comcat = prob_C_names[where(prob_C == nanmax(prob_C))[0][0]]
+                comcat = prob_C_names.iloc[where(prob_C == nanmax(prob_C))[0][0]]
                 comnum = round(nanmax(prob_C) * 100)
 
             ID_list[i] = index_current
             combined_prob = Series(concatenate((prob_A, prob_B, prob_C)),
                                    index=prob_names)
             VA_result[i] = InterVA5._va5(index_current, self.malaria, self.hiv,
                                          preg_state, lik_preg, cause1, lik1,
@@ -594,18 +604,24 @@
             VA_result = DataFrame(VA_result)
             VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT",
                                  "PREGLIK", "CAUSE1", "LIK1", "CAUSE2", "LIK2",
                                  "CAUSE3", "LIK3", "INDET", "COMCAT", "COMNUM",
                                  "WHOLEPROB"]
             VA_result.drop(nan_indices, axis=0, inplace=True)
         else:
+            # TODO: add get_errors() function (similar to pyinsilicova)
+            warnings.warn(
+                "NO VALID VA RECORDS (datacheck procedure invalidated all "
+                "deaths)!  Check error log for more details."
+            )
             VA_result = None
 
-        dem_group = DataFrame(list_dem_group)
-        self.dem_group = dem_group.set_index("ID")
+        if len(list_dem_group) > 0:
+            dem_group = DataFrame(list_dem_group)
+            self.dem_group = dem_group.set_index("ID")
 
         self.results = {"ID": ID_list,
                         "VA5": VA_result,
                         "Malaria": self.malaria,
                         "HIV": self.hiv,
                         "checked_data": self.checked_data}
 
@@ -623,29 +639,29 @@
 
     def set_hiv(self, hiv_level: str) -> str:
         """Set HIV parameter."""
 
         hiv_lvl = hiv_level.lower()
         if hiv_lvl in ["h", "l", "v"]:
             self.hiv = hiv_lvl
+            print(f"HIV parameter is {self.hiv}")
         else:
             print(f"The provided HIV level '{hiv_level}' is invalid.")
         return self.hiv
-        print(f"HIV parameter is {self.hiv}")
 
     def set_malaria(self, malaria_level: str) -> str:
         """Set malaria parameter."""
 
         malaria_lvl = malaria_level.lower()
         if malaria_lvl in ["h", "l", "v"]:
             self.malaria = malaria_lvl
+            print(f"Malaria parameter is {self.malaria}")
         else:
             print(f"The provided malaria level '{malaria_level}' is invalid.")
         return self.malaria
-        print(f"Malaria parameter is {self.malaria}")
 
     def get_ids(self) -> Series:
         """Return pandas series of ID column in data."""
 
         va_df = self.va_input
         if isinstance(va_df, str) and va_df[-4:] == ".csv":
             va_df = read_csv(va_df)
@@ -664,23 +680,32 @@
         :param groupcode: a logical value indicating if the group code will be
         included in the cause names.
         :type groupcode: bool
         :return: the top causes in CSMF with their values.
         :rtype: pandas.series
         """
 
+        if len(self.results) == 0:
+            print("No results.  Use run() method to assign causes.")
+            return None
+        if self.results["VA5"] is None:
+            print("No results found.  Check error log.  It is likely that "
+                  "all records failed the data consistency checks.")
+            return None
         va = self.results["VA5"]
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
 
         # for future compatibility with non-standard input
         causenames = causeindex = []
         for i in range(va.shape[0]):
-            if va.loc[i, "WHOLEPROB"] is not None:
-                causenames = va.loc[i, "WHOLEPROB"].index
+            # if va.loc[i, "WHOLEPROB"] is not None:
+            #     causenames = va.loc[i, "WHOLEPROB"].index
+            if va.iloc[i]["WHOLEPROB"] is not None:
+                causenames = va.iloc[i]["WHOLEPROB"].index
                 causeindex = [x for x in range(len(causenames))]
                 break
         include_probAC = False
 
         if self.groupcode:
             temp_names = ["" for _ in range(len(causenames))]
             for i in range(len(causenames)):
@@ -723,16 +748,18 @@
         if len(va) < 1:
             print("No va5 object found")
             return None
         # Initialize the population distribution
         dist = None
         for i in range(len(va)):
             if va.iloc[i, 14] is not None:
-                dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
+                # dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
+                dist = array([0] * len(va.iloc[i, 14]))
                 break
+        # what if dist is still None at this point? ex dataset 2?
         undeter = 0
 
         # Pick not simply the top # causes,
         # but the top # causes reported by InterVA5
         for i in range(len(va)):
             if va.iloc[i, 14] is None:  # wholeprob exists
                 continue
@@ -771,18 +798,19 @@
 
                 close_indices.sort(reverse=True)
                 for k in close_indices:
                     undeter = undeter + this_dist[k]
                     this_dist[k] = 0
 
                 if va.iloc[i, 14] is not None:
-                    if i == 0:
-                        dist = this_dist
-                    else:
-                        dist = dist + this_dist
+                    # if i == 0:
+                    #     dist = this_dist
+                    # else:
+                    #     dist = dist + this_dist
+                    dist = dist + this_dist
 
         dist = Series(dist)
         dist_cod = None
         # Normalize the probability for CODs
         if undeter > 0:
             dist_cod = dist.iloc[causeindex].copy()
             dist_cod.loc[causeindex[len(causeindex)-1]+1] = undeter
@@ -795,19 +823,19 @@
         if (isna(dist_cod).sum() == len(dist_cod)).all():
             dist_cod[isna(dist_cod)] = 0
 
         dist_cod_sorted = dist_cod.copy()
         dist_cod_sorted.sort_values(ascending=False, inplace=True)
         # show causes with top non-zero values
         show_top = 0
-        while dist_cod_sorted[show_top] > 0 and show_top < top:
+        while dist_cod_sorted.iloc[show_top] > 0 and show_top < top:
             show_top = show_top + 1
         if show_top == top:
-            a = dist_cod_sorted[show_top]
-            b = dist_cod_sorted[show_top-1]
+            a = dist_cod_sorted.iloc[show_top]
+            b = dist_cod_sorted.iloc[show_top-1]
             while show_top < len(dist_cod_sorted) and \
                     (abs(a-b) < (a+b) * 1e-5):
                 show_top = show_top + 1
                 a = dist_cod_sorted[show_top]
                 b = dist_cod_sorted[show_top-1]
         top_csmf = dist_cod_sorted.head(show_top)
         return top_csmf
@@ -857,15 +885,16 @@
                 name = "CAUSE" + str(i+1)
                 column_names.append(name)
                 if include_propensities:
                     prob = "PROPENSITY" + str(i+1) + ""
                     column_names.append(prob)
 
         for indiv in range(num_indiv):
-            wholeprob = VA5.loc[indiv, "WHOLEPROB"]
+            # wholeprob = VA5.loc[indiv, "WHOLEPROB"]
+            wholeprob = VA5.iloc[indiv]["WHOLEPROB"]
             prob_B = wholeprob.iloc[3:64].copy()
 
             if top == 0 or top is None:
                 cod_list[indiv] = prob_B
             if top > 0:
                 prob_temp = prob_B.to_numpy()
                 prob_temp_names = prob_B.index
```

### Comparing `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/utils.py` & `interva-0.0.7/src/interva/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """Retrieve sex (male/female/unknown) from the VA record."""
 
     if not isinstance(va_series, Series):
         raise ArgumentException(
             "The argument for va_series must be a pandas.Series")
 
     yes = [1, "y", "Y", "yes", "Yes", "YES"]
-    no = [0, "n", "N", ".", "no", "No", "NO"]
+    no = [0, "n", "N", ".", "-", "no", "No", "NO"]
     va_sex = "unknown"
     if va_series["i019a"] in yes and (va_series["i019b"] in no or
                                       isna(va_series["i019b"])):
         va_sex = "male"
     elif va_series["i019b"] in yes and (va_series["i019a"] in no or
                                         isna(va_series["i019a"])):
         va_sex = "female"
@@ -145,17 +145,17 @@
     :type sex: str
     :type top_aggregate: Union[int, None]
 
     :return: the top causes in CSMF with their values.
     :rtype: pandas.series
     """
 
-    if not isinstance(iva5, interva.interva5.InterVA5):
-        raise ArgumentException(
-            "The argument for va5 must be an instance of the InterVA5 class")
+    # if not isinstance(iva5, interva.interva5.InterVA5):
+    #     raise ArgumentException(
+    #         "The argument for iva5 must be an instance of the InterVA5 class")
     if len(iva5.results) == 0:
         raise ArgumentException("No results (need to use run() method).")
     if age is not None:
         age_groups = ["adult", "child", "neonate"]
         if not isinstance(age, str) or age.lower() not in age_groups:
             raise ArgumentException(
                 "The age parameter must be " + ", ".join(age_groups))
@@ -191,23 +191,23 @@
     if dist_cod is None:
         return None
 
     dist_cod.sort_values(ascending=False, inplace=True)
 
     # show causes with top non-zero values
     show_top = 0
-    while dist_cod[show_top] > 0 and show_top < top:
+    while dist_cod.iloc[show_top] > 0 and show_top < top:
         show_top = show_top + 1
     if show_top == top:
-        a = dist_cod[show_top]
-        b = dist_cod[show_top - 1]
+        a = dist_cod.iloc[show_top]
+        b = dist_cod.iloc[show_top - 1]
         while show_top < len(dist_cod) and (abs(a - b) < (a + b) * 1e-5):
             show_top = show_top + 1
-            a = dist_cod[show_top]
-            b = dist_cod[show_top - 1]
+            a = dist_cod.iloc[show_top]
+            b = dist_cod.iloc[show_top - 1]
     top_csmf = dist_cod.head(show_top)
 
     return top_csmf
 
 
 def _csmf_without_interva_rule(
         va5: DataFrame,
@@ -348,14 +348,15 @@
         print("No va5 object found")
         return None
     # Initialize the population distribution
     dist = None
     for i in va.index:
         if va.loc[i, "WHOLEPROB"] is not None:
             dist = zeros(len(va.loc[i, "WHOLEPROB"]))
+            # TODO: this has been changed (to fix bug) in interva5.py
             break
     undetermined = 0
 
     # Pick not simply the top # causes,
     # but the top # causes reported by InterVA5
     for i in va.index:
         whole_prob = va.loc[i, "WHOLEPROB"]
@@ -428,17 +429,17 @@
     :type iva5: interva.interva5.InterVA5
 
     :return: VA5 results with age and sex indicators included as columns,
     and ID set as the index.
     :rtype: pandas.DataFrame
     """
 
-    if not isinstance(iva5, interva.interva5.InterVA5):
-        raise ArgumentException(
-            "The argument for va5 must be an instance of the InterVA5 class")
+    # if not isinstance(iva5, interva.interva5.InterVA5):
+    #     raise ArgumentException(
+    #         "The argument for va5 must be an instance of the InterVA5 class")
     if len(iva5.results) == 0:
         raise ArgumentException("No results (need to use run() method).")
 
     va5_results = iva5.results["VA5"].copy()
     va5_results = va5_results.set_index("ID")
 
     all_results = va5_results.merge(iva5.dem_group, on="ID")
@@ -453,14 +454,16 @@
     """Get individual causes of death distribution.
 
     :param iva5: instance of InterVA5 with results
     :type iva5: interva.interva5.InterVA5
     :param top: number of top causes to be determined. If top is 0 or None,
     all propensities be returned (unordered).
     :type top: integer or None
+    :param interva_rule: Use the InterVA threshold for assigning undetermined.
+    :type: bool
     :param include_propensities: a logical value indicating whether the
     propensities of top causes should be included. If top is 0 or None,
     this boolean is automatically set to True.
     :return: the individual cause of death distribution.
     :rtype: pandas DataFrame
     """
```

### Comparing `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.7/tests/test_compare_r.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,45 +53,45 @@
                   top=15, top_aggregate=8)
 
 
 def test_r_va5_comparison():
     for i in range(r_prob_check.shape[0]):
         for j in range(r_prob_check.shape[1]):
             a = round(r_prob_check.iloc[i, j], 10)
-            b = round(py_prob_check[i][j], 10)
+            b = round(py_prob_check.iloc[i].iloc[j], 10)
             assert a == b
 
 
 def test_r_csmf_top15_comparison():
     assert (py_csmf_top15_check.index == r_csmf_top15_check.index).all()
     py_csmf_top15 = py_csmf_top15_check.to_numpy()
     r_csmf_top15 = r_csmf_top15_check.to_numpy()
     for i in range(len(r_csmf_top15_check)):
         a = round(float(py_csmf_top15[i]), 10)
-        b = round(float(r_csmf_top15[i]), 10)
+        b = round(float(r_csmf_top15[i][0]), 10)
         assert a == b
 
 
 def tests_utils_csmf_1():
     r_csmf5_1_top15 = r_csmf5_1.sort_values(
         by="csmf5_no_rule", ascending=False)[0:15]
     py_csmf5_1_top15 = py_csmf5_1.sort_values(ascending=False)
     assert (r_csmf5_1_top15.index == py_csmf5_1_top15.index).all()
     py_csmf5_1_top15 = py_csmf5_1_top15.to_numpy()
     r_csmf5_1_top15 = r_csmf5_1_top15.to_numpy()
     for i in range(len(r_csmf5_1_top15)):
         a = round(float(py_csmf5_1_top15[i]), 10)
-        b = round(float(r_csmf5_1_top15[i]), 10)
+        b = round(float(r_csmf5_1_top15[i][0]), 10)
         assert a == b
 
 
 def tests_utils_csmf_2():
     r_csmf5_2_top15 = r_csmf5_2.sort_values(
         by="csmf5_no_rule2", ascending=False)[0:15]
     py_csmf5_2_top15 = py_csmf5_2.sort_values(ascending=False)
     assert (r_csmf5_2_top15.index == py_csmf5_2_top15.index).all()
     py_csmf5_2_top15 = py_csmf5_2_top15.to_numpy()
     r_csmf5_2_top15 = r_csmf5_2_top15.to_numpy()
     for i in range(len(r_csmf5_2_top15)):
         a = round(float(py_csmf5_2_top15[i]), 4)
-        b = round(float(r_csmf5_2_top15[i]), 4)
+        b = round(float(r_csmf5_2_top15[i][0]), 4)
         assert a == b
```

### Comparing `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.7/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.6/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_utils.py` & `interva-0.0.7/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
               ("age 1-4", "child"), ("age 1-11m", "child"),
               ("age 0-27d", "neonate")]
 all_age_groups = dict(zip(age_indicators, age_labels))
 
 
 def make_age_test_data(age_group, yes, no):
     sex_groups = Series({"ID": "d1", "i019a": "y", "i019b": "n"})
-    age_groups = Series({f"i022{i}": no for i in age_letters})
+    age_groups = Series({f"i022{i}": no for i in age_letters}).astype(object)
     age_groups[age_group] = yes
     va_record = concat([sex_groups, age_groups])
     age_all, age = all_age_groups[age_group]
     return va_record, age, age_all
 
 
 def test_get_sex_group_exception():
@@ -83,27 +83,30 @@
 
 def test_get_age_groups_unknown():
     va_record, age_label, age_all_label = make_age_test_data("i022a", 0, 0)
     assert _get_age_group(va_record) == "unknown"
     assert _get_dem_groups(va_record).get("age") == "unknown"
 
 
-def test_csmf_exception_df_input():
-    with pytest.raises(ArgumentException):
-        csmf("a")
+# def test_csmf_exception_df_input():
+#     with pytest.raises(ArgumentException):
+#         csmf("a")
 
 
 def test_csmf_exception_zero_rows():
+    bad_input = InterVA5(va_data, hiv="h", malaria="l", write=False)
     with pytest.raises(ArgumentException):
-        csmf(DataFrame({"a": []}))
+        csmf(bad_input)
 
 
 def test_csmf_exception_df_columns():
+    bad_input = InterVA5(va_data, hiv="h", malaria="l", write=False)
+    bad_input.results["VA5"] = iv5out.results["VA5"].drop(columns="MALPREV")
     with pytest.raises(ArgumentException):
-        csmf(DataFrame(range(12)))
+        csmf(bad_input)
 
 
 def test_csmf_returns_series():
     out1 = csmf(iv5out, top=10, interva_rule=True, top_aggregate=None)
     out2 = csmf(iv5out, top=10, interva_rule=False, top_aggregate=None)
     out3 = csmf(iv5out, top=10, interva_rule=True, top_aggregate=10)
     out4 = csmf(iv5out)
```

### Comparing `interva-0.0.6/interva/data/probbase.xls` & `interva-0.0.7/src/interva/data/probbase.xls`

 * *Files identical despite different names*

### Comparing `interva-0.0.6/interva/data/probbaseV5_19.csv` & `interva-0.0.7/src/interva/data/probbaseV5_19.csv`

 * *Files identical despite different names*

### Comparing `interva-0.0.6/interva/data/randomva5.csv` & `interva-0.0.7/src/interva/data/randomva5.csv`

 * *Files identical despite different names*

### Comparing `interva-0.0.6/interva.egg-info/PKG-INFO` & `interva-0.0.7/src/interva.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 Metadata-Version: 2.1
 Name: interva
-Version: 0.0.6
+Version: 0.0.7
 Summary: Python implementation of the InterVA Algorithm.
-Home-page: https://github.com/verbal-autopsy-software/interva
-Author: Sherry Zhao & Jason Thomas
-Author-email: zhao.3248@buckeyemail.osu.edu
+Author-email: Sherry Zhao <zhao.3248@buckeyemail.osu.edu>, Jason Thomas <jarathomas@gmail.com>
+Maintainer-email: Jason Thomas <jarathomas@gmail.com>
 License: GPLv3
+Project-URL: Homepage, https://github.com/verbal-autopsy-software/interva
+Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/interva/issues
+Keywords: verbal autopsy
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
+Requires-Dist: vacheck
+Requires-Dist: xlrd
 
 # interva
 
 [![image](https://img.shields.io/pypi/pyversions/interva)](https://pypi.org/project/interva/)
 [![pytest](https://github.com/verbal-autopsy-software/interva/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/interva/actions)
 
 Python implementation of the InterVA algorithm for assigning causes of death to verbal autopsy data
```

