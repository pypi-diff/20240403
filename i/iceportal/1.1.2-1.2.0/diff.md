# Comparing `tmp/iceportal-1.1.2.tar.gz` & `tmp/iceportal-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iceportal-1.1.2.tar", max compression
+gzip compressed data, was "iceportal-1.2.0.tar", max compression
```

## Comparing `iceportal-1.1.2.tar` & `iceportal-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1110 2023-03-30 07:28:11.839510 iceportal-1.1.2/LICENSE
--rw-r--r--   0        0        0     2827 2022-12-24 11:53:26.778637 iceportal-1.1.2/iceportal/__init__.py
--rw-r--r--   0        0        0      345 2019-11-22 10:22:04.282814 iceportal-1.1.2/iceportal/exceptions.py
--rw-r--r--   0        0        0      469 2023-11-17 13:00:23.530741 iceportal-1.1.2/pyproject.toml
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 iceportal-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1110 2024-04-02 22:04:33.800813 iceportal-1.2.0/LICENSE
+-rw-r--r--   0        0        0     2827 2022-12-24 11:53:26.778637 iceportal-1.2.0/iceportal/__init__.py
+-rw-r--r--   0        0        0      345 2019-11-22 10:22:04.282814 iceportal-1.2.0/iceportal/exceptions.py
+-rw-r--r--   0        0        0      465 2024-04-02 22:13:51.894315 iceportal-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      451 1970-01-01 00:00:00.000000 iceportal-1.2.0/PKG-INFO
```

### Comparing `iceportal-1.1.2/LICENSE` & `iceportal-1.2.0/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2019-2023 Fabian Affolter <fabian@affolter-engineering.ch>
+Copyright (c) 2019-2024 Fabian Affolter <fabian@affolter-engineering.ch>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `iceportal-1.1.2/iceportal/__init__.py` & `iceportal-1.2.0/iceportal/__init__.py`

 * *Files identical despite different names*

