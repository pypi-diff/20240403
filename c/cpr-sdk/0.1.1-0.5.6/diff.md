# Comparing `tmp/cpr-sdk-0.1.1.tar.gz` & `tmp/cpr_sdk-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpr-sdk-0.1.1.tar", last modified: Tue Apr  2 15:29:50 2024, max compression
+gzip compressed data, was "cpr_sdk-0.5.6.tar", max compression
```

## Comparing `cpr-sdk-0.1.1.tar` & `cpr_sdk-0.5.6.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:29:50.429822 cpr-sdk-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 15:29:37.000000 cpr-sdk-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-02 15:29:50.429822 cpr-sdk-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 15:29:37.000000 cpr-sdk-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:29:50.425822 cpr-sdk-0.1.1/cpr_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 15:29:37.000000 cpr-sdk-0.1.1/cpr_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:29:37.000000 cpr-sdk-0.1.1/cpr_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-02 15:29:37.000000 cpr-sdk-0.1.1/cpr_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:29:50.425822 cpr-sdk-0.1.1/cpr_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-02 15:29:50.000000 cpr-sdk-0.1.1/cpr_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 15:29:50.000000 cpr-sdk-0.1.1/cpr_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:29:50.000000 cpr-sdk-0.1.1/cpr_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-02 15:29:50.000000 cpr-sdk-0.1.1/cpr_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 15:29:50.000000 cpr-sdk-0.1.1/cpr_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-02 15:29:37.000000 cpr-sdk-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 15:29:50.429822 cpr-sdk-0.1.1/setup.cfg
+-rw-r--r--   0        0        0     6189 2024-04-03 09:56:37.652945 cpr_sdk-0.5.6/README.md
+-rw-r--r--   0        0        0     2334 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/__init__.py
+-rw-r--r--   0        0        0     5693 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/data_adaptors.py
+-rw-r--r--   0        0        0     1118 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/embedding.py
+-rw-r--r--   0        0        0      797 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/exceptions.py
+-rw-r--r--   0        0        0    50630 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/models/__init__.py
+-rw-r--r--   0        0        0    11754 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/models/search.py
+-rw-r--r--   0        0        0    12721 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/parser_models.py
+-rw-r--r--   0        0        0     2679 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/pipeline_general_models.py
+-rw-r--r--   0        0        0    71013 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/resources/sensitive_query_terms.tsv
+-rw-r--r--   0        0        0     2791 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/s3.py
+-rw-r--r--   0        0        0     4584 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/search_adaptors.py
+-rw-r--r--   0        0        0     4044 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/utils.py
+-rw-r--r--   0        0        0     6979 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/vespa.py
+-rw-r--r--   0        0        0     6732 2024-04-03 09:56:37.656945 cpr_sdk-0.5.6/src/cpr_sdk/yql_builder.py
+-rw-r--r--   0        0        0     7584 1970-01-01 00:00:00.000000 cpr_sdk-0.5.6/setup.py
+-rw-r--r--   0        0        0     7296 1970-01-01 00:00:00.000000 cpr_sdk-0.5.6/PKG-INFO
```

