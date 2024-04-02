# Comparing `tmp/mcap-protobuf-support-0.4.1.tar.gz` & `tmp/mcap-protobuf-support-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap-protobuf-support-0.4.1.tar", last modified: Thu Nov 16 18:53:36 2023, max compression
+gzip compressed data, was "mcap-protobuf-support-0.5.0.tar", last modified: Tue Apr  2 22:52:55 2024, max compression
```

## Comparing `mcap-protobuf-support-0.4.1.tar` & `mcap-protobuf-support-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:53:36.435619 mcap-protobuf-support-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-11-16 18:53:36.435619 mcap-protobuf-support-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:53:36.435619 mcap-protobuf-support-0.4.1/mcap_protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/mcap_protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/mcap_protobuf/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/mcap_protobuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/mcap_protobuf/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/mcap_protobuf/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/mcap_protobuf/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:53:36.435619 mcap-protobuf-support-0.4.1/mcap_protobuf_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2023-11-16 18:53:36.000000 mcap-protobuf-support-0.4.1/mcap_protobuf_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      483 2023-11-16 18:53:36.000000 mcap-protobuf-support-0.4.1/mcap_protobuf_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-16 18:53:36.000000 mcap-protobuf-support-0.4.1/mcap_protobuf_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-16 18:53:36.000000 mcap-protobuf-support-0.4.1/mcap_protobuf_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-11-16 18:53:36.000000 mcap-protobuf-support-0.4.1/mcap_protobuf_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      633 2023-11-16 18:53:36.439619 mcap-protobuf-support-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-16 18:53:36.435619 mcap-protobuf-support-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2023-11-16 18:51:07.000000 mcap-protobuf-support-0.4.1/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/mcap_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/tests/test_writer.py
```

### Comparing `mcap-protobuf-support-0.4.1/PKG-INFO` & `mcap-protobuf-support-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mcap-protobuf-support
-Version: 0.4.1
+Version: 0.5.0
 Summary: Protobuf support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: mcap>=0.0.14
-Requires-Dist: protobuf!=4.22.*,!=4.23.*,!=4.24.*,>=3.8
+Requires-Dist: protobuf>=4.25
 
 # Python MCAP protobuf support
 
 This package provides protobuf support for the Python MCAP file format reader.
 
 ## Installation
 
@@ -44,8 +44,8 @@
 
 ```bash
 pipenv run python point_cloud_example.py output.mcap
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-protobuf-support-0.4.1/README.md` & `mcap-protobuf-support-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,8 @@
 
 ```bash
 pipenv run python point_cloud_example.py output.mcap
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-protobuf-support-0.4.1/mcap_protobuf/reader.py` & `mcap-protobuf-support-0.5.0/mcap_protobuf/reader.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.4.1/mcap_protobuf/schema.py` & `mcap-protobuf-support-0.5.0/mcap_protobuf/schema.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.4.1/mcap_protobuf/writer.py` & `mcap-protobuf-support-0.5.0/mcap_protobuf/writer.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.4.1/mcap_protobuf_support.egg-info/PKG-INFO` & `mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: mcap-protobuf-support
-Version: 0.4.1
+Version: 0.5.0
 Summary: Protobuf support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: mcap>=0.0.14
-Requires-Dist: protobuf!=4.22.*,!=4.23.*,!=4.24.*,>=3.8
+Requires-Dist: protobuf>=4.25
 
 # Python MCAP protobuf support
 
 This package provides protobuf support for the Python MCAP file format reader.
 
 ## Installation
 
@@ -44,8 +44,8 @@
 
 ```bash
 pipenv run python point_cloud_example.py output.mcap
 ```
 
 ## Stay in touch
 
-Join our [Slack channel](https://foxglove.dev/join-slack) to ask questions, share feedback, and stay up to date on what our team is working on.
+Join our [Slack channel](https://foxglove.dev/slack) to ask questions, share feedback, and stay up to date on what our team is working on.
```

### Comparing `mcap-protobuf-support-0.4.1/setup.cfg` & `mcap-protobuf-support-0.5.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
 install_requires = 
 	mcap>=0.0.14
-	protobuf>=3.8,!=4.22.*,!=4.23.*,!=4.24.*
+	protobuf>=4.25
 install_package_data = True
 packages = find:
 python_requires = >=3.7
 
 [options.package_data]
 mcap_protobuf = py.typed
```

### Comparing `mcap-protobuf-support-0.4.1/tests/generate.py` & `mcap-protobuf-support-0.5.0/tests/generate.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.4.1/tests/test_decoder.py` & `mcap-protobuf-support-0.5.0/tests/test_decoder.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.4.1/tests/test_writer.py` & `mcap-protobuf-support-0.5.0/tests/test_writer.py`

 * *Files identical despite different names*

