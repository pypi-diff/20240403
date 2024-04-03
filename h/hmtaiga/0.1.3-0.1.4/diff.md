# Comparing `tmp/hmtaiga-0.1.3.tar.gz` & `tmp/hmtaiga-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmtaiga-0.1.3.tar", last modified: Wed Apr  3 01:23:52 2024, max compression
+gzip compressed data, was "hmtaiga-0.1.4.tar", last modified: Wed Apr  3 03:34:23 2024, max compression
```

## Comparing `hmtaiga-0.1.3.tar` & `hmtaiga-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,18 @@
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.504309 hmtaiga-0.1.3/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-03 01:23:52.504132 hmtaiga-0.1.3/PKG-INFO
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.503957 hmtaiga-0.1.3/hmtaiga.egg-info/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-03 01:23:52.000000 hmtaiga-0.1.3/hmtaiga.egg-info/PKG-INFO
--rw-r--r--   0 shikhaverma   (501) staff       (20)      401 2024-04-03 01:23:52.000000 hmtaiga-0.1.3/hmtaiga.egg-info/SOURCES.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-03 01:23:52.000000 hmtaiga-0.1.3/hmtaiga.egg-info/dependency_links.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)       29 2024-04-03 01:23:52.000000 hmtaiga-0.1.3/hmtaiga.egg-info/top_level.txt
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.502071 hmtaiga-0.1.3/project/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.3/project/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     1213 2024-03-25 04:07:28.000000 hmtaiga-0.1.3/project/getProjectBySlug.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-03 01:23:52.504343 hmtaiga-0.1.3/setup.cfg
--rw-r--r--   0 shikhaverma   (501) staff       (20)      182 2024-04-03 01:23:25.000000 hmtaiga-0.1.3/setup.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.502727 hmtaiga-0.1.3/tasks/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/tasks/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/tasks/get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/tasks/get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.503244 hmtaiga-0.1.3/test/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/test/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/test/test_get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/test/test_get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.503624 hmtaiga-0.1.3/userStory/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.3/userStory/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/userStory/getBusinessValue.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2298 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/userStory/get_user_story_history.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:34:23.251896 hmtaiga-0.1.4/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)       94 2024-04-03 03:34:23.251575 hmtaiga-0.1.4/PKG-INFO
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:34:23.251324 hmtaiga-0.1.4/hmtaiga.egg-info/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)       94 2024-04-03 03:34:23.000000 hmtaiga-0.1.4/hmtaiga.egg-info/PKG-INFO
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      295 2024-04-03 03:34:23.000000 hmtaiga-0.1.4/hmtaiga.egg-info/SOURCES.txt
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        1 2024-04-03 03:34:23.000000 hmtaiga-0.1.4/hmtaiga.egg-info/dependency_links.txt
+-rw-r--r--   0 hasanshahid   (501) staff       (20)       11 2024-04-03 03:34:23.000000 hmtaiga-0.1.4/hmtaiga.egg-info/top_level.txt
+-rw-r--r--   0 hasanshahid   (501) staff       (20)       38 2024-04-03 03:34:23.251950 hmtaiga-0.1.4/setup.cfg
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      182 2024-04-03 03:24:51.000000 hmtaiga-0.1.4/setup.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:34:23.250289 hmtaiga-0.1.4/tasks/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:23:28.000000 hmtaiga-0.1.4/tasks/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     5914 2024-04-03 03:23:28.000000 hmtaiga-0.1.4/tasks/get_task_history.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     2446 2024-04-03 03:23:28.000000 hmtaiga-0.1.4/tasks/get_tasks.py
+drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:34:23.251110 hmtaiga-0.1.4/test/
+-rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-03 03:23:28.000000 hmtaiga-0.1.4/test/__init__.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)      939 2024-04-03 03:23:28.000000 hmtaiga-0.1.4/test/test_getProjectBySlug.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     4839 2024-04-03 03:23:28.000000 hmtaiga-0.1.4/test/test_get_task_history.py
+-rw-r--r--   0 hasanshahid   (501) staff       (20)     4571 2024-04-03 03:23:28.000000 hmtaiga-0.1.4/test/test_get_tasks.py
```

### Comparing `hmtaiga-0.1.3/tasks/get_task_history.py` & `hmtaiga-0.1.4/tasks/get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.3/tasks/get_tasks.py` & `hmtaiga-0.1.4/tasks/get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.3/test/test_get_task_history.py` & `hmtaiga-0.1.4/test/test_get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.3/test/test_get_tasks.py` & `hmtaiga-0.1.4/test/test_get_tasks.py`

 * *Files identical despite different names*

