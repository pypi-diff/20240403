# Comparing `tmp/hmtaiga-0.1.2.tar.gz` & `tmp/hmtaiga-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmtaiga-0.1.2.tar", last modified: Wed Apr  3 01:03:52 2024, max compression
+gzip compressed data, was "hmtaiga-0.1.3.tar", last modified: Wed Apr  3 01:23:52 2024, max compression
```

## Comparing `hmtaiga-0.1.2.tar` & `hmtaiga-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.554834 hmtaiga-0.1.2/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-03 01:03:52.554635 hmtaiga-0.1.2/PKG-INFO
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.554454 hmtaiga-0.1.2/hmtaiga.egg-info/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-03 01:03:52.000000 hmtaiga-0.1.2/hmtaiga.egg-info/PKG-INFO
--rw-r--r--   0 shikhaverma   (501) staff       (20)      353 2024-04-03 01:03:52.000000 hmtaiga-0.1.2/hmtaiga.egg-info/SOURCES.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-03 01:03:52.000000 hmtaiga-0.1.2/hmtaiga.egg-info/dependency_links.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)       21 2024-04-03 01:03:52.000000 hmtaiga-0.1.2/hmtaiga.egg-info/top_level.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-03 01:03:52.554869 hmtaiga-0.1.2/setup.cfg
--rw-r--r--   0 shikhaverma   (501) staff       (20)      182 2024-04-03 00:54:03.000000 hmtaiga-0.1.2/setup.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.552969 hmtaiga-0.1.2/tasks/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/tasks/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/tasks/get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/tasks/get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.553642 hmtaiga-0.1.2/test/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/test/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/test/test_get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/test/test_get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.554185 hmtaiga-0.1.2/userStory/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.2/userStory/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-04-02 23:47:16.000000 hmtaiga-0.1.2/userStory/getBusinessValue.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2298 2024-04-03 00:53:40.000000 hmtaiga-0.1.2/userStory/get_user_story_history.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.504309 hmtaiga-0.1.3/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-03 01:23:52.504132 hmtaiga-0.1.3/PKG-INFO
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.503957 hmtaiga-0.1.3/hmtaiga.egg-info/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-03 01:23:52.000000 hmtaiga-0.1.3/hmtaiga.egg-info/PKG-INFO
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      401 2024-04-03 01:23:52.000000 hmtaiga-0.1.3/hmtaiga.egg-info/SOURCES.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-03 01:23:52.000000 hmtaiga-0.1.3/hmtaiga.egg-info/dependency_links.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       29 2024-04-03 01:23:52.000000 hmtaiga-0.1.3/hmtaiga.egg-info/top_level.txt
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.502071 hmtaiga-0.1.3/project/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.3/project/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     1213 2024-03-25 04:07:28.000000 hmtaiga-0.1.3/project/getProjectBySlug.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-03 01:23:52.504343 hmtaiga-0.1.3/setup.cfg
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      182 2024-04-03 01:23:25.000000 hmtaiga-0.1.3/setup.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.502727 hmtaiga-0.1.3/tasks/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/tasks/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/tasks/get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/tasks/get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.503244 hmtaiga-0.1.3/test/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/test/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/test/test_get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/test/test_get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:23:52.503624 hmtaiga-0.1.3/userStory/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.3/userStory/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/userStory/getBusinessValue.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2298 2024-04-03 01:18:30.000000 hmtaiga-0.1.3/userStory/get_user_story_history.py
```

### Comparing `hmtaiga-0.1.2/tasks/get_task_history.py` & `hmtaiga-0.1.3/tasks/get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.2/tasks/get_tasks.py` & `hmtaiga-0.1.3/tasks/get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.2/test/test_get_task_history.py` & `hmtaiga-0.1.3/test/test_get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.2/test/test_get_tasks.py` & `hmtaiga-0.1.3/test/test_get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.2/userStory/getBusinessValue.py` & `hmtaiga-0.1.3/userStory/getBusinessValue.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.2/userStory/get_user_story_history.py` & `hmtaiga-0.1.3/userStory/get_user_story_history.py`

 * *Files identical despite different names*

