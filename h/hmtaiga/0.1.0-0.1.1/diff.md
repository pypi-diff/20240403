# Comparing `tmp/hmtaiga-0.1.0.tar.gz` & `tmp/hmtaiga-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmtaiga-0.1.0.tar", last modified: Tue Apr  2 06:03:44 2024, max compression
+gzip compressed data, was "hmtaiga-0.1.1.tar", last modified: Tue Apr  2 23:22:09 2024, max compression
```

## Comparing `hmtaiga-0.1.0.tar` & `hmtaiga-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,21 @@
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-02 06:03:44.955017 hmtaiga-0.1.0/
--rw-r--r--   0 hasanshahid   (501) staff       (20)       94 2024-04-02 06:03:44.954763 hmtaiga-0.1.0/PKG-INFO
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-02 06:03:44.953979 hmtaiga-0.1.0/hmtaiga.egg-info/
--rw-r--r--   0 hasanshahid   (501) staff       (20)       94 2024-04-02 06:03:44.000000 hmtaiga-0.1.0/hmtaiga.egg-info/PKG-INFO
--rw-r--r--   0 hasanshahid   (501) staff       (20)      265 2024-04-02 06:03:44.000000 hmtaiga-0.1.0/hmtaiga.egg-info/SOURCES.txt
--rw-r--r--   0 hasanshahid   (501) staff       (20)        1 2024-04-02 06:03:44.000000 hmtaiga-0.1.0/hmtaiga.egg-info/dependency_links.txt
--rw-r--r--   0 hasanshahid   (501) staff       (20)       11 2024-04-02 06:03:44.000000 hmtaiga-0.1.0/hmtaiga.egg-info/top_level.txt
--rw-r--r--   0 hasanshahid   (501) staff       (20)       38 2024-04-02 06:03:44.955114 hmtaiga-0.1.0/setup.cfg
--rw-r--r--   0 hasanshahid   (501) staff       (20)      182 2024-04-02 06:03:29.000000 hmtaiga-0.1.0/setup.py
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-02 06:03:44.952647 hmtaiga-0.1.0/tasks/
--rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-01 08:55:56.000000 hmtaiga-0.1.0/tasks/__init__.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     5914 2024-04-02 05:19:33.000000 hmtaiga-0.1.0/tasks/get_task_history.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     2446 2024-04-02 05:07:20.000000 hmtaiga-0.1.0/tasks/get_tasks.py
-drwxr-xr-x   0 hasanshahid   (501) staff       (20)        0 2024-04-02 06:03:44.953107 hmtaiga-0.1.0/test/
--rw-r--r--   0 hasanshahid   (501) staff       (20)        0 2024-04-02 01:08:43.000000 hmtaiga-0.1.0/test/__init__.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     4839 2024-04-02 05:20:08.000000 hmtaiga-0.1.0/test/test_get_task_history.py
--rw-r--r--   0 hasanshahid   (501) staff       (20)     4571 2024-04-02 05:20:26.000000 hmtaiga-0.1.0/test/test_get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.698852 hmtaiga-0.1.1/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-02 23:22:09.698668 hmtaiga-0.1.1/PKG-INFO
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.698484 hmtaiga-0.1.1/hmtaiga.egg-info/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-02 23:22:09.000000 hmtaiga-0.1.1/hmtaiga.egg-info/PKG-INFO
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      353 2024-04-02 23:22:09.000000 hmtaiga-0.1.1/hmtaiga.egg-info/SOURCES.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-02 23:22:09.000000 hmtaiga-0.1.1/hmtaiga.egg-info/dependency_links.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       21 2024-04-02 23:22:09.000000 hmtaiga-0.1.1/hmtaiga.egg-info/top_level.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-02 23:22:09.698887 hmtaiga-0.1.1/setup.cfg
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      182 2024-04-02 23:14:28.000000 hmtaiga-0.1.1/setup.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.697008 hmtaiga-0.1.1/tasks/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/tasks/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/tasks/get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/tasks/get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.697700 hmtaiga-0.1.1/test/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/test/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/test/test_get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/test/test_get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.698196 hmtaiga-0.1.1/userStory/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.1/userStory/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-03-13 18:32:23.000000 hmtaiga-0.1.1/userStory/getBusinessValue.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2141 2024-04-02 23:09:48.000000 hmtaiga-0.1.1/userStory/get_user_story_history.py
```

### Comparing `hmtaiga-0.1.0/tasks/get_task_history.py` & `hmtaiga-0.1.1/tasks/get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.0/tasks/get_tasks.py` & `hmtaiga-0.1.1/tasks/get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.0/test/test_get_task_history.py` & `hmtaiga-0.1.1/test/test_get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.0/test/test_get_tasks.py` & `hmtaiga-0.1.1/test/test_get_tasks.py`

 * *Files identical despite different names*

