# Comparing `tmp/remarshal-0.9.2.tar.gz` & `tmp/remarshal-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/remarshal-0.9.2.tar", last modified: Thu Apr  4 20:27:49 2019, max compression
+gzip compressed data, was "remarshal-1.0.0rc1.tar", max compression
```

## Comparing `remarshal-0.9.2.tar` & `remarshal-1.0.0rc1.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 20:27:49.000000 remarshal-0.9.2/
-drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      236 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/PKG-INFO
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      608 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/SOURCES.txt
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)        1 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/dependency_links.txt
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      289 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/entry_points.txt
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       50 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/requires.txt
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       10 2019-04-04 20:27:49.000000 remarshal-0.9.2/remarshal.egg-info/top_level.txt
-drwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)        0 2019-04-04 20:27:49.000000 remarshal-0.9.2/tests/
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)        0 2016-09-02 12:13:21.000000 remarshal-0.9.2/tests/__init__.py
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       26 2016-09-02 12:13:21.000000 remarshal-0.9.2/tests/array.json
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       41 2019-04-04 20:12:19.000000 remarshal-0.9.2/tests/array.toml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       81 2016-09-02 12:13:21.000000 remarshal-0.9.2/tests/context.py
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)       34 2016-09-03 12:23:17.000000 remarshal-0.9.2/tests/garbage
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      157 2016-09-02 18:25:18.000000 remarshal-0.9.2/tests/long-line-default.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      170 2016-09-02 18:35:31.000000 remarshal-0.9.2/tests/long-line-double-quote.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      177 2016-09-02 18:36:30.000000 remarshal-0.9.2/tests/long-line-gt.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      173 2016-09-02 18:36:37.000000 remarshal-0.9.2/tests/long-line-pipe.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      167 2016-09-02 18:35:22.000000 remarshal-0.9.2/tests/long-line-single-quote.yaml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      180 2016-09-02 18:23:56.000000 remarshal-0.9.2/tests/long-line.json
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       39 2018-11-02 13:38:02.000000 remarshal-0.9.2/tests/order.json
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       24 2018-11-02 13:38:02.000000 remarshal-0.9.2/tests/order.toml
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       21 2018-11-02 13:38:02.000000 remarshal-0.9.2/tests/order.yaml
--rwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)     9602 2019-04-04 20:21:38.000000 remarshal-0.9.2/tests/test_remarshal.py
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       76 2019-04-04 20:21:38.000000 remarshal-0.9.2/MANIFEST.in
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)     5308 2019-04-04 20:21:38.000000 remarshal-0.9.2/README.md
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      889 2016-09-02 12:13:21.000000 remarshal-0.9.2/example.json
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)      875 2019-04-04 20:12:19.000000 remarshal-0.9.2/example.toml
--rw-r--r--   0 dbohdan   (1000) dbohdan   (1000)      563 2016-09-02 12:13:21.000000 remarshal-0.9.2/example.yaml
--rwxrwxr-x   0 dbohdan   (1000) dbohdan   (1000)     9751 2019-04-04 20:21:38.000000 remarshal-0.9.2/remarshal.py
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)     1262 2019-04-04 20:21:38.000000 remarshal-0.9.2/setup.py
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)      236 2019-04-04 20:27:49.000000 remarshal-0.9.2/PKG-INFO
--rw-rw-r--   0 dbohdan   (1000) dbohdan   (1000)       38 2019-04-04 20:27:49.000000 remarshal-0.9.2/setup.cfg
+-rw-r--r--   0        0        0     1064 2023-07-19 12:01:05.000000 remarshal-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     7675 2024-01-02 17:35:56.413952 remarshal-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      424 2020-03-13 16:57:15.000000 remarshal-1.0.0rc1/example.cbor
+-rw-r--r--   0        0        0      889 2016-09-02 12:13:21.000000 remarshal-1.0.0rc1/example.json
+-rw-r--r--   0        0        0      402 2019-07-18 19:58:25.000000 remarshal-1.0.0rc1/example.msgpack
+-rw-r--r--   0        0        0      875 2023-09-25 19:26:23.000000 remarshal-1.0.0rc1/example.toml
+-rw-r--r--   0        0        0      563 2016-09-02 12:13:21.000000 remarshal-1.0.0rc1/example.yaml
+-rw-r--r--   0        0        0     5842 2024-01-02 17:35:56.413952 remarshal-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0       43 2023-10-19 09:22:50.000000 remarshal-1.0.0rc1/src/remarshal/__init__.py
+-rw-r--r--   0        0        0       71 2023-10-19 09:22:50.000000 remarshal-1.0.0rc1/src/remarshal/__main__.py
+-rwxr-xr-x   0        0        0    20650 2024-01-02 17:35:56.413952 remarshal-1.0.0rc1/src/remarshal/main.py
+-rw-r--r--   0        0        0        0 2023-10-19 09:22:50.000000 remarshal-1.0.0rc1/src/remarshal/py.typed
+-rw-r--r--   0        0        0        0 2016-09-02 12:13:21.000000 remarshal-1.0.0rc1/tests/__init__.py
+-rw-r--r--   0        0        0       26 2016-09-02 12:13:21.000000 remarshal-1.0.0rc1/tests/array.json
+-rw-r--r--   0        0        0       41 2019-04-04 20:12:19.000000 remarshal-1.0.0rc1/tests/array.toml
+-rw-r--r--   0        0        0      417 2019-07-18 18:59:48.000000 remarshal-1.0.0rc1/tests/bin.msgpack
+-rw-r--r--   0        0        0      876 2019-07-19 08:07:58.000000 remarshal-1.0.0rc1/tests/bin.yml
+-rw-r--r--   0        0        0       67 2023-07-19 12:01:05.345524 remarshal-1.0.0rc1/tests/bool-null-key.json
+-rw-r--r--   0        0        0       60 2023-09-05 13:28:50.000000 remarshal-1.0.0rc1/tests/bool-null-key.toml
+-rw-r--r--   0        0        0       46 2023-07-19 12:01:05.000000 remarshal-1.0.0rc1/tests/bool-null-key.yaml
+-rw-r--r--   0        0        0       19 2023-09-05 13:28:50.000000 remarshal-1.0.0rc1/tests/empty-mapping.toml
+-rw-r--r--   0        0        0       12 2023-09-05 13:28:50.247583 remarshal-1.0.0rc1/tests/empty-mapping.yaml
+-rw-r--r--   0        0        0       34 2016-09-03 12:23:17.000000 remarshal-1.0.0rc1/tests/garbage
+-rw-r--r--   0        0        0      634 2023-09-05 13:28:50.247583 remarshal-1.0.0rc1/tests/lol.yml
+-rw-r--r--   0        0        0      157 2016-09-02 18:25:18.000000 remarshal-1.0.0rc1/tests/long-line-default.yaml
+-rw-r--r--   0        0        0      170 2016-09-02 18:35:31.000000 remarshal-1.0.0rc1/tests/long-line-double-quote.yaml
+-rw-r--r--   0        0        0      177 2016-09-02 18:36:30.000000 remarshal-1.0.0rc1/tests/long-line-gt.yaml
+-rw-r--r--   0        0        0      173 2016-09-02 18:36:37.000000 remarshal-1.0.0rc1/tests/long-line-pipe.yaml
+-rw-r--r--   0        0        0      167 2016-09-02 18:35:22.000000 remarshal-1.0.0rc1/tests/long-line-single-quote.yaml
+-rw-r--r--   0        0        0      180 2016-09-02 18:23:56.000000 remarshal-1.0.0rc1/tests/long-line.json
+-rw-r--r--   0        0        0       11 2023-09-05 13:28:50.247583 remarshal-1.0.0rc1/tests/numeric-key-null-value.toml
+-rw-r--r--   0        0        0        8 2023-09-05 13:28:50.000000 remarshal-1.0.0rc1/tests/numeric-key-null-value.yaml
+-rw-r--r--   0        0        0       39 2018-11-02 13:38:02.000000 remarshal-1.0.0rc1/tests/order.json
+-rw-r--r--   0        0        0       24 2018-11-02 13:38:02.000000 remarshal-1.0.0rc1/tests/order.toml
+-rw-r--r--   0        0        0       21 2018-11-02 13:38:02.000000 remarshal-1.0.0rc1/tests/order.yaml
+-rwxr-xr-x   0        0        0    21320 2024-01-02 17:35:56.413952 remarshal-1.0.0rc1/tests/test_remarshal.py
+-rw-r--r--   0        0        0       29 2023-09-05 13:28:50.251583 remarshal-1.0.0rc1/tests/timestamp-key.toml
+-rw-r--r--   0        0        0       17 2023-09-05 13:28:50.251583 remarshal-1.0.0rc1/tests/timestamp-key.yaml
+-rw-r--r--   0        0        0      235 2023-10-19 14:02:06.000000 remarshal-1.0.0rc1/tox.ini
+-rw-r--r--   0        0        0     9162 1970-01-01 00:00:00.000000 remarshal-1.0.0rc1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `remarshal-0.9.2/example.json` & `remarshal-1.0.0rc1/example.json`

 * *Files identical despite different names*

### Comparing `remarshal-0.9.2/example.toml` & `remarshal-1.0.0rc1/example.toml`

 * *Files identical despite different names*

### Comparing `remarshal-0.9.2/example.yaml` & `remarshal-1.0.0rc1/example.yaml`

 * *Files identical despite different names*

