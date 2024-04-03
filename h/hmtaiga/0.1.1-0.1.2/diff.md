# Comparing `tmp/hmtaiga-0.1.1.tar.gz` & `tmp/hmtaiga-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmtaiga-0.1.1.tar", last modified: Tue Apr  2 23:22:09 2024, max compression
+gzip compressed data, was "hmtaiga-0.1.2.tar", last modified: Wed Apr  3 01:03:52 2024, max compression
```

## Comparing `hmtaiga-0.1.1.tar` & `hmtaiga-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.698852 hmtaiga-0.1.1/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-02 23:22:09.698668 hmtaiga-0.1.1/PKG-INFO
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.698484 hmtaiga-0.1.1/hmtaiga.egg-info/
--rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-02 23:22:09.000000 hmtaiga-0.1.1/hmtaiga.egg-info/PKG-INFO
--rw-r--r--   0 shikhaverma   (501) staff       (20)      353 2024-04-02 23:22:09.000000 hmtaiga-0.1.1/hmtaiga.egg-info/SOURCES.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-02 23:22:09.000000 hmtaiga-0.1.1/hmtaiga.egg-info/dependency_links.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)       21 2024-04-02 23:22:09.000000 hmtaiga-0.1.1/hmtaiga.egg-info/top_level.txt
--rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-02 23:22:09.698887 hmtaiga-0.1.1/setup.cfg
--rw-r--r--   0 shikhaverma   (501) staff       (20)      182 2024-04-02 23:14:28.000000 hmtaiga-0.1.1/setup.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.697008 hmtaiga-0.1.1/tasks/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/tasks/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/tasks/get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/tasks/get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.697700 hmtaiga-0.1.1/test/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/test/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/test/test_get_task_history.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-02 22:47:28.000000 hmtaiga-0.1.1/test/test_get_tasks.py
-drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-02 23:22:09.698196 hmtaiga-0.1.1/userStory/
--rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.1/userStory/__init__.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-03-13 18:32:23.000000 hmtaiga-0.1.1/userStory/getBusinessValue.py
--rw-r--r--   0 shikhaverma   (501) staff       (20)     2141 2024-04-02 23:09:48.000000 hmtaiga-0.1.1/userStory/get_user_story_history.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.554834 hmtaiga-0.1.2/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-03 01:03:52.554635 hmtaiga-0.1.2/PKG-INFO
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.554454 hmtaiga-0.1.2/hmtaiga.egg-info/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       94 2024-04-03 01:03:52.000000 hmtaiga-0.1.2/hmtaiga.egg-info/PKG-INFO
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      353 2024-04-03 01:03:52.000000 hmtaiga-0.1.2/hmtaiga.egg-info/SOURCES.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        1 2024-04-03 01:03:52.000000 hmtaiga-0.1.2/hmtaiga.egg-info/dependency_links.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       21 2024-04-03 01:03:52.000000 hmtaiga-0.1.2/hmtaiga.egg-info/top_level.txt
+-rw-r--r--   0 shikhaverma   (501) staff       (20)       38 2024-04-03 01:03:52.554869 hmtaiga-0.1.2/setup.cfg
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      182 2024-04-03 00:54:03.000000 hmtaiga-0.1.2/setup.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.552969 hmtaiga-0.1.2/tasks/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/tasks/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     5914 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/tasks/get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2446 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/tasks/get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.553642 hmtaiga-0.1.2/test/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/test/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4839 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/test/test_get_task_history.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     4571 2024-04-02 22:47:28.000000 hmtaiga-0.1.2/test/test_get_tasks.py
+drwxr-xr-x   0 shikhaverma   (501) staff       (20)        0 2024-04-03 01:03:52.554185 hmtaiga-0.1.2/userStory/
+-rw-r--r--   0 shikhaverma   (501) staff       (20)        0 2024-02-12 04:15:32.000000 hmtaiga-0.1.2/userStory/__init__.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)      855 2024-04-02 23:47:16.000000 hmtaiga-0.1.2/userStory/getBusinessValue.py
+-rw-r--r--   0 shikhaverma   (501) staff       (20)     2298 2024-04-03 00:53:40.000000 hmtaiga-0.1.2/userStory/get_user_story_history.py
```

### Comparing `hmtaiga-0.1.1/tasks/get_task_history.py` & `hmtaiga-0.1.2/tasks/get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.1/tasks/get_tasks.py` & `hmtaiga-0.1.2/tasks/get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.1/test/test_get_task_history.py` & `hmtaiga-0.1.2/test/test_get_task_history.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.1/test/test_get_tasks.py` & `hmtaiga-0.1.2/test/test_get_tasks.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.1/userStory/getBusinessValue.py` & `hmtaiga-0.1.2/userStory/getBusinessValue.py`

 * *Files identical despite different names*

### Comparing `hmtaiga-0.1.1/userStory/get_user_story_history.py` & `hmtaiga-0.1.2/userStory/get_user_story_history.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-from concurrent.futures import ThreadPoolExecutor
 
 import requests
 from dotenv import load_dotenv
 
 # Load environment variables from .env file
 load_dotenv()
 
@@ -59,8 +58,17 @@
                 "story_points": user_story["total_points"]
             }
             for user_story in user_stories if user_story.get("is_closed")
         ]
 
         return closed_user_stories
     else:
-        return []
+        return []
+
+
+def get_user_story_details_by_id(
+    story,
+    headers,
+    taiga_url
+):
+    task_history_url = f"{taiga_url}/history/userstory/{story['id']}"
+    return requests.get(task_history_url, headers=headers)
```

