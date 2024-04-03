# Comparing `tmp/train_route-0.4.2.tar.gz` & `tmp/train_route-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "train_route-0.4.2.tar", max compression
+gzip compressed data, was "train_route-0.5.0.tar", max compression
```

## Comparing `train_route-0.4.2.tar` & `train_route-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2024-03-24 14:11:14.824841 train_route-0.4.2/LICENSE
--rw-r--r--   0        0        0        0 2024-03-24 14:30:15.824590 train_route-0.4.2/README.md
--rw-r--r--   0        0        0      272 2024-03-28 00:14:34.982414 train_route-0.4.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-24 12:22:27.136302 train_route-0.4.2/train_route/__init__.py
--rw-r--r--   0        0        0      496 2024-03-28 00:12:18.072432 train_route-0.4.2/train_route/rotation.py
--rw-r--r--   0        0        0     3808 2024-03-24 16:54:39.986473 train_route-0.4.2/train_route/route.py
--rw-r--r--   0        0        0     5311 2024-03-28 00:14:05.122419 train_route-0.4.2/train_route/traveler.py
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 train_route-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-03-24 14:11:14.824841 train_route-0.5.0/LICENSE
+-rw-r--r--   0        0        0      228 2024-03-28 11:56:12.497719 train_route-0.5.0/README.md
+-rw-r--r--   0        0        0      407 2024-04-03 16:25:12.785652 train_route-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-24 12:22:27.136302 train_route-0.5.0/train_route/__init__.py
+-rw-r--r--   0        0        0      496 2024-03-28 00:12:18.072432 train_route-0.5.0/train_route/rotation.py
+-rw-r--r--   0        0        0     3808 2024-03-24 16:54:39.986473 train_route-0.5.0/train_route/route.py
+-rw-r--r--   0        0        0     4758 2024-04-03 15:42:56.856101 train_route-0.5.0/train_route/traveler.py
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 train_route-0.5.0/PKG-INFO
```

### Comparing `train_route-0.4.2/LICENSE` & `train_route-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `train_route-0.4.2/train_route/route.py` & `train_route-0.5.0/train_route/route.py`

 * *Files identical despite different names*

