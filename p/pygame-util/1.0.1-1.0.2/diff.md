# Comparing `tmp/pygame_util-1.0.1.tar.gz` & `tmp/pygame_util-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_util-1.0.1.tar", max compression
+gzip compressed data, was "pygame_util-1.0.2.tar", max compression
```

## Comparing `pygame_util-1.0.1.tar` & `pygame_util-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1068 2024-04-01 21:23:18.515915 pygame_util-1.0.1/LICENSE
--rw-r--r--   0        0        0     1067 2024-04-01 22:28:43.746940 pygame_util-1.0.1/LICENSE.txt
--rw-r--r--   0        0        0       14 2024-04-01 22:03:58.556792 pygame_util-1.0.1/README.md
--rw-r--r--   0        0        0      241 2024-04-01 22:08:08.689356 pygame_util-1.0.1/pygame_util/__init__.py
--rw-r--r--   0        0        0      606 2024-04-01 21:25:21.373656 pygame_util-1.0.1/pygame_util/color.py
--rw-r--r--   0        0        0       67 2024-04-01 22:37:21.939093 pygame_util-1.0.1/pygame_util/dist/pygame_util-0.1.0.tar.gz
--rw-r--r--   0        0        0      659 2024-04-03 16:26:44.962419 pygame_util-1.0.1/pygame_util/image.py
--rw-r--r--   0        0        0     9123 2024-04-01 22:36:15.629750 pygame_util-1.0.1/pygame_util/poetry.lock
--rw-r--r--   0        0        0     2223 2024-04-01 21:25:21.374293 pygame_util-1.0.1/pygame_util/position.py
--rw-r--r--   0        0        0     3697 2024-04-03 16:26:44.905329 pygame_util-1.0.1/pygame_util/text.py
--rw-r--r--   0        0        0     1843 2024-04-01 21:25:21.374949 pygame_util-1.0.1/pygame_util/timer.py
--rw-r--r--   0        0        0     1093 2024-04-03 16:26:43.341380 pygame_util-1.0.1/pygame_util/window.py
--rw-r--r--   0        0        0      314 2024-04-03 16:29:09.999849 pygame_util-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 pygame_util-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-01 21:23:18.515915 pygame_util-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1067 2024-04-01 22:28:43.746940 pygame_util-1.0.2/LICENSE.txt
+-rw-r--r--   0        0        0       14 2024-04-01 22:03:58.556792 pygame_util-1.0.2/README.md
+-rw-r--r--   0        0        0      247 2024-04-03 16:43:29.835528 pygame_util-1.0.2/pygame_util/__init__.py
+-rw-r--r--   0        0        0      606 2024-04-01 21:25:21.373656 pygame_util-1.0.2/pygame_util/color.py
+-rw-r--r--   0        0        0       67 2024-04-01 22:37:21.939093 pygame_util-1.0.2/pygame_util/dist/pygame_util-0.1.0.tar.gz
+-rw-r--r--   0        0        0      659 2024-04-03 16:26:44.962419 pygame_util-1.0.2/pygame_util/image.py
+-rw-r--r--   0        0        0     9123 2024-04-01 22:36:15.629750 pygame_util-1.0.2/pygame_util/poetry.lock
+-rw-r--r--   0        0        0     2223 2024-04-01 21:25:21.374293 pygame_util-1.0.2/pygame_util/position.py
+-rw-r--r--   0        0        0     3697 2024-04-03 16:26:44.905329 pygame_util-1.0.2/pygame_util/text.py
+-rw-r--r--   0        0        0     1843 2024-04-01 21:25:21.374949 pygame_util-1.0.2/pygame_util/timer.py
+-rw-r--r--   0        0        0     1093 2024-04-03 16:26:43.341380 pygame_util-1.0.2/pygame_util/window.py
+-rw-r--r--   0        0        0      314 2024-04-03 16:44:08.493757 pygame_util-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 pygame_util-1.0.2/PKG-INFO
```

### Comparing `pygame_util-1.0.1/LICENSE` & `pygame_util-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.1/LICENSE.txt` & `pygame_util-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.1/pygame_util/color.py` & `pygame_util-1.0.2/pygame_util/color.py`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.1/pygame_util/image.py` & `pygame_util-1.0.2/pygame_util/image.py`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.1/pygame_util/poetry.lock` & `pygame_util-1.0.2/pygame_util/poetry.lock`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.1/pygame_util/position.py` & `pygame_util-1.0.2/pygame_util/position.py`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.1/pygame_util/text.py` & `pygame_util-1.0.2/pygame_util/text.py`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.1/pygame_util/timer.py` & `pygame_util-1.0.2/pygame_util/timer.py`

 * *Files identical despite different names*

### Comparing `pygame_util-1.0.1/pygame_util/window.py` & `pygame_util-1.0.2/pygame_util/window.py`

 * *Files identical despite different names*

