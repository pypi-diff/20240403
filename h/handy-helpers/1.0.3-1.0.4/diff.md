# Comparing `tmp/handy-helpers-1.0.3.tar.gz` & `tmp/handy-helpers-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/handy-helpers-1.0.3.tar", last modified: Wed Apr  3 12:20:07 2024, max compression
+gzip compressed data, was "dist/handy-helpers-1.0.4.tar", last modified: Wed Apr  3 12:49:35 2024, max compression
```

## Comparing `handy-helpers-1.0.3.tar` & `handy-helpers-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      146 2024-04-03 12:19:21.000000 handy-helpers-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)      218 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/handyhelpers/
--rw-r--r--   0 root         (0) root         (0)    11764 2024-04-03 12:19:21.000000 handy-helpers-1.0.3/handyhelpers/util_aliyun.py
--rw-r--r--   0 root         (0) root         (0)     1426 2024-04-03 12:19:21.000000 handy-helpers-1.0.3/handyhelpers/util_linux.py
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 12:19:21.000000 handy-helpers-1.0.3/handyhelpers/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:19:21.000000 handy-helpers-1.0.3/handyhelpers/Workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/handyhelpers/scripts/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:19:21.000000 handy-helpers-1.0.3/handyhelpers/scripts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      405 2024-04-03 12:19:21.000000 handy-helpers-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/handy_helpers.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/handy_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/handy_helpers.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      218 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/handy_helpers.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       93 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/handy_helpers.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      341 2024-04-03 12:20:07.000000 handy-helpers-1.0.3/handy_helpers.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/README.md
+-rw-r--r--   0 root         (0) root         (0)      218 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/handyhelpers/
+-rw-r--r--   0 root         (0) root         (0)    11764 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/util_aliyun.py
+-rw-r--r--   0 root         (0) root         (0)     1426 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/util_linux.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/handyhelpers/aliyun/
+-rw-r--r--   0 root         (0) root         (0)     2085 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/aliyun/RunECSInstanceSettings.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/aliyun/RunCommandHelper.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/aliyun/CloudDiskHelper.py
+-rw-r--r--   0 root         (0) root         (0)      361 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/aliyun/ClientProvider.py
+-rw-r--r--   0 root         (0) root         (0)     4286 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/aliyun/ECSInstance.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:49:06.000000 handy-helpers-1.0.4/handyhelpers/aliyun/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4714 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/aliyun/ECSManager.py
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/Workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/handyhelpers/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/handyhelpers/scripts/linux/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/handyhelpers/scripts/linux/alilinux3/
+-rw-r--r--   0 root         (0) root         (0)       34 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/scripts/linux/alilinux3/devkits.py
+-rw-r--r--   0 root         (0) root         (0)      529 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/scripts/linux/alilinux3/docker.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:49:06.000000 handy-helpers-1.0.4/handyhelpers/scripts/linux/alilinux3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:49:06.000000 handy-helpers-1.0.4/handyhelpers/scripts/linux/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 12:19:21.000000 handy-helpers-1.0.4/handyhelpers/scripts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      405 2024-04-03 12:49:06.000000 handy-helpers-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 12:49:35.000000 handy-helpers-1.0.4/handy_helpers.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 12:49:34.000000 handy-helpers-1.0.4/handy_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-03 12:49:34.000000 handy-helpers-1.0.4/handy_helpers.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      218 2024-04-03 12:49:34.000000 handy-helpers-1.0.4/handy_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       93 2024-04-03 12:49:34.000000 handy-helpers-1.0.4/handy_helpers.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      788 2024-04-03 12:49:34.000000 handy-helpers-1.0.4/handy_helpers.egg-info/SOURCES.txt
```

### Comparing `handy-helpers-1.0.3/handyhelpers/util_aliyun.py` & `handy-helpers-1.0.4/handyhelpers/util_aliyun.py`

 * *Files identical despite different names*

### Comparing `handy-helpers-1.0.3/handyhelpers/util_linux.py` & `handy-helpers-1.0.4/handyhelpers/util_linux.py`

 * *Files identical despite different names*

