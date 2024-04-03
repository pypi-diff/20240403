# Comparing `tmp/turbo_broccoli-4.8.0.tar.gz` & `tmp/turbo_broccoli-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_broccoli-4.8.0.tar", last modified: Wed Apr  3 10:04:18 2024, max compression
+gzip compressed data, was "turbo_broccoli-4.9.0.tar", last modified: Wed Apr  3 10:04:26 2024, max compression
```

## Comparing `turbo_broccoli-4.8.0.tar` & `turbo_broccoli-4.9.0.tar`

### file list

```diff
@@ -1,62 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:18.564490 turbo_broccoli-4.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24079 2024-04-03 10:04:18.564490 turbo_broccoli-4.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23434 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:04:18.564490 turbo_broccoli-4.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:18.560490 turbo_broccoli-4.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    24882 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_bokeh.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_guard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_native.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_nodecode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)    63005 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/tests/test_uuid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:18.560490 turbo_broccoli-4.8.0/turbo_broccoli/
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:18.564490 turbo_broccoli-4.8.0/turbo_broccoli/custom/
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/bokeh.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/dct.py
--rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/embedded.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/keras.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/scipy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/custom/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/guard.py
--rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/native.py
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/turbo_broccoli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-03 10:04:11.000000 turbo_broccoli-4.8.0/turbo_broccoli/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:18.564490 turbo_broccoli-4.8.0/turbo_broccoli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24079 2024-04-03 10:04:18.000000 turbo_broccoli-4.8.0/turbo_broccoli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-03 10:04:18.000000 turbo_broccoli-4.8.0/turbo_broccoli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:04:18.000000 turbo_broccoli-4.8.0/turbo_broccoli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 10:04:18.000000 turbo_broccoli-4.8.0/turbo_broccoli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:26.192397 turbo_broccoli-4.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24880 2024-04-03 10:04:26.192397 turbo_broccoli-4.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:04:26.192397 turbo_broccoli-4.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:26.184397 turbo_broccoli-4.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    24882 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4460 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_nodecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63005 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/tests/test_uuid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:26.184397 turbo_broccoli-4.9.0/turbo_broccoli/
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8843 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:26.188397 turbo_broccoli-4.9.0/turbo_broccoli/custom/
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2738 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/bokeh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4186 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/dct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/embedded.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17069 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/keras.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3510 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/custom/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9067 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/guard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9113 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/native.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8520 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/turbo_broccoli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-03 10:04:16.000000 turbo_broccoli-4.9.0/turbo_broccoli/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:04:26.188397 turbo_broccoli-4.9.0/turbo_broccoli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24880 2024-04-03 10:04:26.000000 turbo_broccoli-4.9.0/turbo_broccoli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-03 10:04:26.000000 turbo_broccoli-4.9.0/turbo_broccoli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:04:26.000000 turbo_broccoli-4.9.0/turbo_broccoli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 10:04:26.000000 turbo_broccoli-4.9.0/turbo_broccoli.egg-info/top_level.txt
```

### Comparing `turbo_broccoli-4.8.0/LICENSE` & `turbo_broccoli-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/PKG-INFO` & `turbo_broccoli-4.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo_broccoli
-Version: 4.8.0
+Version: 4.9.0
 Summary: JSON (de)serialization extensions
 Home-page: https://github.com/altaris/turbo-broccoli
 Author: Cédric Ho Thanh
 Author-email: altaris@users.noreply.github.com
 Project-URL: Issues, https://github.com/altaris/turbo-broccoli/issues
 Platform: any
 Classifier: License :: OSI Approved :: MIT License
@@ -288,16 +288,33 @@
   Secret key used to encrypt/decrypt secrets. The encryption uses [`pynacl`'s
   `SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
   An exception is raised when attempting to serialize a secret type while no
   key is set.
 
 ## Guarded blocks
 
-This is so cool. Check out
-[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler).
+A
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler)
+"guards" a block of code, meaning it prevents it from being executed if it has
+been in the past. Check out [the
+documentation](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html)
+for some examples.
+
+## Guarded-parallel executors
+
+A mix of
+[`joblib.Parallel`](https://joblib.readthedocs.io/en/latest/generated/joblib.Parallel.html)
+and
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler):
+a
+[`turbo_broccoli.Parallel`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/parallel.html#Parallel)
+object can be used to execute jobs in parallel, but those whose results have
+already been obtained in the past are skipped. See [the
+documentation](https://altaris.github.io/turbo-broccoli/turbo_broccoli/parallel.html)
+for some examples.
 
 ## Supported types
 
 ### Basic types
 
 - [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
```

### Comparing `turbo_broccoli-4.8.0/README.md` & `turbo_broccoli-4.9.0/turbo_broccoli.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: turbo_broccoli
+Version: 4.9.0
+Summary: JSON (de)serialization extensions
+Home-page: https://github.com/altaris/turbo-broccoli
+Author: Cédric Ho Thanh
+Author-email: altaris@users.noreply.github.com
+Project-URL: Issues, https://github.com/altaris/turbo-broccoli/issues
+Platform: any
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Turbo Broccoli 🥦
 
 [![Repository](https://img.shields.io/badge/repo-github-pink)](https://github.com/altaris/turbo-broccoli)
 [![PyPI](https://img.shields.io/pypi/v/turbo-broccoli)](https://pypi.org/project/turbo-broccoli/)
 ![License](https://img.shields.io/github/license/altaris/turbo-broccoli)
 [![Code
 style](https://img.shields.io/badge/style-black-black)](https://pypi.org/project/black)
@@ -270,16 +288,33 @@
   Secret key used to encrypt/decrypt secrets. The encryption uses [`pynacl`'s
   `SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
   An exception is raised when attempting to serialize a secret type while no
   key is set.
 
 ## Guarded blocks
 
-This is so cool. Check out
-[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler).
+A
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler)
+"guards" a block of code, meaning it prevents it from being executed if it has
+been in the past. Check out [the
+documentation](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html)
+for some examples.
+
+## Guarded-parallel executors
+
+A mix of
+[`joblib.Parallel`](https://joblib.readthedocs.io/en/latest/generated/joblib.Parallel.html)
+and
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler):
+a
+[`turbo_broccoli.Parallel`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/parallel.html#Parallel)
+object can be used to execute jobs in parallel, but those whose results have
+already been obtained in the past are skipped. See [the
+documentation](https://altaris.github.io/turbo-broccoli/turbo_broccoli/parallel.html)
+for some examples.
 
 ## Supported types
 
 ### Basic types
 
 - [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
```

### Comparing `turbo_broccoli-4.8.0/setup.py` & `turbo_broccoli-4.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """Setup script"""
 
 import setuptools
 
 name = "turbo_broccoli"
-version = "4.8.0"
+version = "4.9.0"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as f:
     requirements = f.read().split()
```

### Comparing `turbo_broccoli-4.8.0/tests/test_bokeh.py` & `turbo_broccoli-4.9.0/tests/test_bokeh.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_bytes.py` & `turbo_broccoli-4.9.0/tests/test_bytes.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_collections.py` & `turbo_broccoli-4.9.0/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_dataclass.py` & `turbo_broccoli-4.9.0/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_datetime.py` & `turbo_broccoli-4.9.0/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_dict.py` & `turbo_broccoli-4.9.0/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_embedded.py` & `turbo_broccoli-4.9.0/tests/test_embedded.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_generic.py` & `turbo_broccoli-4.9.0/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_guard.py` & `turbo_broccoli-4.9.0/tests/test_guard.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_keras.py` & `turbo_broccoli-4.9.0/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_native.py` & `turbo_broccoli-4.9.0/tests/test_native.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_nodecode.py` & `turbo_broccoli-4.9.0/tests/test_nodecode.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_numpy.py` & `turbo_broccoli-4.9.0/tests/test_numpy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_pandas.py` & `turbo_broccoli-4.9.0/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_pytorch.py` & `turbo_broccoli-4.9.0/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_scipy.py` & `turbo_broccoli-4.9.0/tests/test_scipy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_secret.py` & `turbo_broccoli-4.9.0/tests/test_secret.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_sklearn.py` & `turbo_broccoli-4.9.0/tests/test_sklearn.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_tensorflow.py` & `turbo_broccoli-4.9.0/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/tests/test_user.py` & `turbo_broccoli-4.9.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/__init__.py` & `turbo_broccoli-4.9.0/turbo_broccoli/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from pkg_resources import DistributionNotFound, get_distribution
 
 from turbo_broccoli.context import Context
 from turbo_broccoli.custom.embedded import EmbeddedDict, EmbeddedList
 from turbo_broccoli.guard import GuardedBlockHandler
 from turbo_broccoli.native import load, save
+from turbo_broccoli.parallel import Parallel, delayed
 from turbo_broccoli.turbo_broccoli import (
     from_json,
     load_json,
     save_json,
     to_json,
 )
 from turbo_broccoli.user import register_decoder, register_encoder
```

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/context.py` & `turbo_broccoli-4.9.0/turbo_broccoli/context.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/__init__.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/__init__.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/bokeh.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/bokeh.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/bytes.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/bytes.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/collections.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/collections.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/dataclass.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/dataclass.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/datetime.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/datetime.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/dct.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/dct.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/embedded.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/embedded.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/generic.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/generic.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/keras.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/keras.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/numpy.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/numpy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/pandas.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/pandas.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/pytorch.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/pytorch.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/scipy.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/scipy.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/secret.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/secret.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/sklearn.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/sklearn.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/tensorflow.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/tensorflow.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/custom/uuid.py` & `turbo_broccoli-4.9.0/turbo_broccoli/custom/uuid.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/exceptions.py` & `turbo_broccoli-4.9.0/turbo_broccoli/exceptions.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/guard.py` & `turbo_broccoli-4.9.0/turbo_broccoli/guard.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/native.py` & `turbo_broccoli-4.9.0/turbo_broccoli/native.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/turbo_broccoli.py` & `turbo_broccoli-4.9.0/turbo_broccoli/turbo_broccoli.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli/user.py` & `turbo_broccoli-4.9.0/turbo_broccoli/user.py`

 * *Files identical despite different names*

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli.egg-info/PKG-INFO` & `turbo_broccoli-4.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: turbo_broccoli
-Version: 4.8.0
-Summary: JSON (de)serialization extensions
-Home-page: https://github.com/altaris/turbo-broccoli
-Author: Cédric Ho Thanh
-Author-email: altaris@users.noreply.github.com
-Project-URL: Issues, https://github.com/altaris/turbo-broccoli/issues
-Platform: any
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Turbo Broccoli 🥦
 
 [![Repository](https://img.shields.io/badge/repo-github-pink)](https://github.com/altaris/turbo-broccoli)
 [![PyPI](https://img.shields.io/pypi/v/turbo-broccoli)](https://pypi.org/project/turbo-broccoli/)
 ![License](https://img.shields.io/github/license/altaris/turbo-broccoli)
 [![Code
 style](https://img.shields.io/badge/style-black-black)](https://pypi.org/project/black)
@@ -288,16 +270,33 @@
   Secret key used to encrypt/decrypt secrets. The encryption uses [`pynacl`'s
   `SecretBox`](https://pynacl.readthedocs.io/en/latest/secret/#nacl.secret.SecretBox).
   An exception is raised when attempting to serialize a secret type while no
   key is set.
 
 ## Guarded blocks
 
-This is so cool. Check out
-[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler).
+A
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler)
+"guards" a block of code, meaning it prevents it from being executed if it has
+been in the past. Check out [the
+documentation](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html)
+for some examples.
+
+## Guarded-parallel executors
+
+A mix of
+[`joblib.Parallel`](https://joblib.readthedocs.io/en/latest/generated/joblib.Parallel.html)
+and
+[`turbo_broccoli.GuardedBlockHandler`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/guard.html#GuardedBlockHandler):
+a
+[`turbo_broccoli.Parallel`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/parallel.html#Parallel)
+object can be used to execute jobs in parallel, but those whose results have
+already been obtained in the past are skipped. See [the
+documentation](https://altaris.github.io/turbo-broccoli/turbo_broccoli/parallel.html)
+for some examples.
 
 ## Supported types
 
 ### Basic types
 
 - [`bytes`](https://altaris.github.io/turbo-broccoli/turbo_broccoli/bytes.html#to_json)
```

### Comparing `turbo_broccoli-4.8.0/turbo_broccoli.egg-info/SOURCES.txt` & `turbo_broccoli-4.9.0/turbo_broccoli.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,26 +13,28 @@
 tests/test_generic.py
 tests/test_guard.py
 tests/test_keras.py
 tests/test_native.py
 tests/test_nodecode.py
 tests/test_numpy.py
 tests/test_pandas.py
+tests/test_parallel.py
 tests/test_pytorch.py
 tests/test_scipy.py
 tests/test_secret.py
 tests/test_sklearn.py
 tests/test_tensorflow.py
 tests/test_user.py
 tests/test_uuid.py
 turbo_broccoli/__init__.py
 turbo_broccoli/context.py
 turbo_broccoli/exceptions.py
 turbo_broccoli/guard.py
 turbo_broccoli/native.py
+turbo_broccoli/parallel.py
 turbo_broccoli/turbo_broccoli.py
 turbo_broccoli/user.py
 turbo_broccoli.egg-info/PKG-INFO
 turbo_broccoli.egg-info/SOURCES.txt
 turbo_broccoli.egg-info/dependency_links.txt
 turbo_broccoli.egg-info/top_level.txt
 turbo_broccoli/custom/__init__.py
```

