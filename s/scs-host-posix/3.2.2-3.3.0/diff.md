# Comparing `tmp/scs-host-posix-3.2.2.tar.gz` & `tmp/scs-host-posix-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scs-host-posix-3.2.2.tar", last modified: Wed Jan 31 08:48:24 2024, max compression
+gzip compressed data, was "scs-host-posix-3.3.0.tar", last modified: Wed Apr  3 10:24:19 2024, max compression
```

## Comparing `scs-host-posix-3.2.2.tar` & `scs-host-posix-3.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:24.446127 scs-host-posix-3.2.2/
--rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/LICENSE
--rw-r--r--   0 bruno      (502) admin       (80)       78 2023-11-22 14:05:55.000000 scs-host-posix-3.2.2/MANIFEST.in
--rw-r--r--   0 bruno      (502) admin       (80)     1204 2024-01-31 08:48:24.445948 scs-host-posix-3.2.2/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)      496 2023-10-17 10:42:18.000000 scs-host-posix-3.2.2/README.md
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/README.rst
--rw-r--r--   0 bruno      (502) admin       (80)        1 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/requirements.txt
--rw-r--r--   0 bruno      (502) admin       (80)       38 2024-01-31 08:48:24.446162 scs-host-posix-3.2.2/setup.cfg
--rwxr-xr-x   0 bruno      (502) admin       (80)     2311 2024-01-31 08:48:18.000000 scs-host-posix-3.2.2/setup.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:24.442532 scs-host-posix-3.2.2/src/
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:24.443438 scs-host-posix-3.2.2/src/scs_host/
--rw-r--r--   0 bruno      (502) admin       (80)      183 2024-01-31 08:48:18.000000 scs-host-posix-3.2.2/src/scs_host/__init__.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:24.443742 scs-host-posix-3.2.2/src/scs_host/client/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/src/scs_host/client/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4760 2024-01-31 08:48:18.000000 scs-host-posix-3.2.2/src/scs_host/client/mqtt_client.py
--rw-r--r--   0 bruno      (502) admin       (80)     3209 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/src/scs_host/client/sftp_client.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:24.444415 scs-host-posix-3.2.2/src/scs_host/comms/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/src/scs_host/comms/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     4972 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/src/scs_host/comms/domain_socket.py
--rw-r--r--   0 bruno      (502) admin       (80)     3433 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/src/scs_host/comms/network_socket.py
--rw-r--r--   0 bruno      (502) admin       (80)     3972 2023-09-15 07:34:31.000000 scs-host-posix-3.2.2/src/scs_host/comms/stdio.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:24.444775 scs-host-posix-3.2.2/src/scs_host/sys/
--rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:22:19.000000 scs-host-posix-3.2.2/src/scs_host/sys/__init__.py
--rw-r--r--   0 bruno      (502) admin       (80)     2465 2023-11-09 16:15:16.000000 scs-host-posix-3.2.2/src/scs_host/sys/host.py
-drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-01-31 08:48:24.445747 scs-host-posix-3.2.2/src/scs_host_posix.egg-info/
--rw-r--r--   0 bruno      (502) admin       (80)     1204 2024-01-31 08:48:24.000000 scs-host-posix-3.2.2/src/scs_host_posix.egg-info/PKG-INFO
--rw-r--r--   0 bruno      (502) admin       (80)      547 2024-01-31 08:48:24.000000 scs-host-posix-3.2.2/src/scs_host_posix.egg-info/SOURCES.txt
--rw-r--r--   0 bruno      (502) admin       (80)        1 2024-01-31 08:48:24.000000 scs-host-posix-3.2.2/src/scs_host_posix.egg-info/dependency_links.txt
--rw-r--r--   0 bruno      (502) admin       (80)        9 2024-01-31 08:48:24.000000 scs-host-posix-3.2.2/src/scs_host_posix.egg-info/top_level.txt
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-03 10:24:19.579651 scs-host-posix-3.3.0/
+-rw-r--r--   0 bruno      (502) admin       (80)     1076 2023-09-11 10:22:19.000000 scs-host-posix-3.3.0/LICENSE
+-rw-r--r--   0 bruno      (502) admin       (80)       78 2023-11-22 14:05:55.000000 scs-host-posix-3.3.0/MANIFEST.in
+-rw-r--r--   0 bruno      (502) admin       (80)     1204 2024-04-03 10:24:19.579492 scs-host-posix-3.3.0/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)      496 2023-10-17 10:42:18.000000 scs-host-posix-3.3.0/README.md
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:22:19.000000 scs-host-posix-3.3.0/README.rst
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2023-09-11 10:22:19.000000 scs-host-posix-3.3.0/requirements.txt
+-rw-r--r--   0 bruno      (502) admin       (80)       38 2024-04-03 10:24:19.579684 scs-host-posix-3.3.0/setup.cfg
+-rwxr-xr-x   0 bruno      (502) admin       (80)     2311 2024-01-31 08:48:18.000000 scs-host-posix-3.3.0/setup.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-03 10:24:19.576412 scs-host-posix-3.3.0/src/
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-03 10:24:19.577302 scs-host-posix-3.3.0/src/scs_host/
+-rw-r--r--   0 bruno      (502) admin       (80)      183 2024-04-03 10:24:14.000000 scs-host-posix-3.3.0/src/scs_host/__init__.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-03 10:24:19.577619 scs-host-posix-3.3.0/src/scs_host/client/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:22:19.000000 scs-host-posix-3.3.0/src/scs_host/client/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4760 2024-01-31 08:48:18.000000 scs-host-posix-3.3.0/src/scs_host/client/mqtt_client.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3209 2023-09-11 10:22:19.000000 scs-host-posix-3.3.0/src/scs_host/client/sftp_client.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-03 10:24:19.578261 scs-host-posix-3.3.0/src/scs_host/comms/
+-rw-r--r--   0 bruno      (502) admin       (80)        0 2023-09-11 10:22:19.000000 scs-host-posix-3.3.0/src/scs_host/comms/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     4972 2023-09-11 10:22:19.000000 scs-host-posix-3.3.0/src/scs_host/comms/domain_socket.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3433 2023-09-11 10:22:19.000000 scs-host-posix-3.3.0/src/scs_host/comms/network_socket.py
+-rw-r--r--   0 bruno      (502) admin       (80)     3972 2023-09-15 07:34:31.000000 scs-host-posix-3.3.0/src/scs_host/comms/stdio.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-03 10:24:19.578603 scs-host-posix-3.3.0/src/scs_host/sys/
+-rw-r--r--   0 bruno      (502) admin       (80)      377 2024-04-03 10:24:14.000000 scs-host-posix-3.3.0/src/scs_host/sys/__init__.py
+-rw-r--r--   0 bruno      (502) admin       (80)     2465 2023-11-09 16:15:16.000000 scs-host-posix-3.3.0/src/scs_host/sys/host.py
+drwxr-xr-x   0 bruno      (502) admin       (80)        0 2024-04-03 10:24:19.579342 scs-host-posix-3.3.0/src/scs_host_posix.egg-info/
+-rw-r--r--   0 bruno      (502) admin       (80)     1204 2024-04-03 10:24:19.000000 scs-host-posix-3.3.0/src/scs_host_posix.egg-info/PKG-INFO
+-rw-r--r--   0 bruno      (502) admin       (80)      547 2024-04-03 10:24:19.000000 scs-host-posix-3.3.0/src/scs_host_posix.egg-info/SOURCES.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        1 2024-04-03 10:24:19.000000 scs-host-posix-3.3.0/src/scs_host_posix.egg-info/dependency_links.txt
+-rw-r--r--   0 bruno      (502) admin       (80)        9 2024-04-03 10:24:19.000000 scs-host-posix-3.3.0/src/scs_host_posix.egg-info/top_level.txt
```

### Comparing `scs-host-posix-3.2.2/LICENSE` & `scs-host-posix-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scs-host-posix-3.2.2/PKG-INFO` & `scs-host-posix-3.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-host-posix
-Version: 3.2.2
+Version: 3.3.0
 Summary: Host abstractions for data consumers running POSIX-compliant operating systems, including Windows 10.
 Home-page: https://github.com/south-coast-science/scs_host_posix
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-host-posix-3.2.2/setup.py` & `scs-host-posix-3.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-3.2.2/src/scs_host/client/mqtt_client.py` & `scs-host-posix-3.3.0/src/scs_host/client/mqtt_client.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-3.2.2/src/scs_host/client/sftp_client.py` & `scs-host-posix-3.3.0/src/scs_host/client/sftp_client.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-3.2.2/src/scs_host/comms/domain_socket.py` & `scs-host-posix-3.3.0/src/scs_host/comms/domain_socket.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-3.2.2/src/scs_host/comms/network_socket.py` & `scs-host-posix-3.3.0/src/scs_host/comms/network_socket.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-3.2.2/src/scs_host/comms/stdio.py` & `scs-host-posix-3.3.0/src/scs_host/comms/stdio.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-3.2.2/src/scs_host/sys/host.py` & `scs-host-posix-3.3.0/src/scs_host/sys/host.py`

 * *Files identical despite different names*

### Comparing `scs-host-posix-3.2.2/src/scs_host_posix.egg-info/PKG-INFO` & `scs-host-posix-3.3.0/src/scs_host_posix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scs-host-posix
-Version: 3.2.2
+Version: 3.3.0
 Summary: Host abstractions for data consumers running POSIX-compliant operating systems, including Windows 10.
 Home-page: https://github.com/south-coast-science/scs_host_posix
 Author: South Coast Science
 Author-email: contact@southcoastscience.com
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scs-host-posix-3.2.2/src/scs_host_posix.egg-info/SOURCES.txt` & `scs-host-posix-3.3.0/src/scs_host_posix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

