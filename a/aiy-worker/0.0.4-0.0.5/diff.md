# Comparing `tmp/aiy_worker-0.0.4.tar.gz` & `tmp/aiy_worker-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiy_worker-0.0.4.tar", last modified: Sun Mar 31 12:51:38 2024, max compression
+gzip compressed data, was "aiy_worker-0.0.5.tar", last modified: Wed Apr  3 11:33:46 2024, max compression
```

## Comparing `aiy_worker-0.0.4.tar` & `aiy_worker-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-03-31 12:51:38.491132 aiy_worker-0.0.4/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-03-31 12:51:38.490489 aiy_worker-0.0.4/PKG-INFO
--rw-r--r--   0 liaojinlong   (501) staff       (20)       15 2024-03-23 04:15:41.000000 aiy_worker-0.0.4/README.md
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-03-31 12:51:38.486137 aiy_worker-0.0.4/aiy_worker/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      110 2024-03-25 08:59:00.000000 aiy_worker-0.0.4/aiy_worker/__init__.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     1402 2024-03-31 08:13:49.000000 aiy_worker-0.0.4/aiy_worker/types.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     4459 2024-03-31 12:11:49.000000 aiy_worker-0.0.4/aiy_worker/utils.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)     5900 2024-03-31 12:50:09.000000 aiy_worker-0.0.4/aiy_worker/worker.py
--rw-r--r--   0 liaojinlong   (501) staff       (20)    10341 2024-03-23 04:39:20.000000 aiy_worker-0.0.4/aiy_worker/ws_client.py
-drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-03-31 12:51:38.489606 aiy_worker-0.0.4/aiy_worker.egg-info/
--rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-03-31 12:51:38.000000 aiy_worker-0.0.4/aiy_worker.egg-info/PKG-INFO
--rw-r--r--   0 liaojinlong   (501) staff       (20)      295 2024-03-31 12:51:38.000000 aiy_worker-0.0.4/aiy_worker.egg-info/SOURCES.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)        1 2024-03-31 12:51:38.000000 aiy_worker-0.0.4/aiy_worker.egg-info/dependency_links.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)      115 2024-03-31 12:51:38.000000 aiy_worker-0.0.4/aiy_worker.egg-info/requires.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)       11 2024-03-31 12:51:38.000000 aiy_worker-0.0.4/aiy_worker.egg-info/top_level.txt
--rw-r--r--   0 liaojinlong   (501) staff       (20)       38 2024-03-31 12:51:38.491274 aiy_worker-0.0.4/setup.cfg
--rw-r--r--   0 liaojinlong   (501) staff       (20)     1302 2024-03-31 12:51:11.000000 aiy_worker-0.0.4/setup.py
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-04-03 11:33:46.911033 aiy_worker-0.0.5/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-04-03 11:33:46.910574 aiy_worker-0.0.5/PKG-INFO
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       15 2024-03-23 04:15:41.000000 aiy_worker-0.0.5/README.md
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-04-03 11:33:46.907728 aiy_worker-0.0.5/aiy_worker/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      110 2024-03-25 08:59:00.000000 aiy_worker-0.0.5/aiy_worker/__init__.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     1527 2024-04-03 11:31:23.000000 aiy_worker-0.0.5/aiy_worker/types.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     4459 2024-03-31 12:11:49.000000 aiy_worker-0.0.5/aiy_worker/utils.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     5956 2024-04-03 11:32:09.000000 aiy_worker-0.0.5/aiy_worker/worker.py
+-rw-r--r--   0 liaojinlong   (501) staff       (20)    10341 2024-03-23 04:39:20.000000 aiy_worker-0.0.5/aiy_worker/ws_client.py
+drwxr-xr-x   0 liaojinlong   (501) staff       (20)        0 2024-04-03 11:33:46.910014 aiy_worker-0.0.5/aiy_worker.egg-info/
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      455 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/PKG-INFO
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      295 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)        1 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)      115 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/requires.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       11 2024-04-03 11:33:46.000000 aiy_worker-0.0.5/aiy_worker.egg-info/top_level.txt
+-rw-r--r--   0 liaojinlong   (501) staff       (20)       38 2024-04-03 11:33:46.911133 aiy_worker-0.0.5/setup.cfg
+-rw-r--r--   0 liaojinlong   (501) staff       (20)     1302 2024-04-03 11:33:06.000000 aiy_worker-0.0.5/setup.py
```

### Comparing `aiy_worker-0.0.4/aiy_worker/types.py` & `aiy_worker-0.0.5/aiy_worker/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,14 +19,17 @@
         self.path = error['path']
 
 class Text2ImageProps:
     def __init__(self, props: dict) -> None:
         self.prompt = props.get('prompt')
         self.negative_prompt = props.get('negativePrompt')
         self.seed = props.get('seed')
+        self.width = props.get('width')
+        self.height = props.get('height')
+        self.n_steps = props.get('nSteps')
 
 class Task:
     def __init__(self, data: dict):
         if data is None:
             return
         subscribe_task: dict = data.get('subscribeTasks')
         if subscribe_task:
```

### Comparing `aiy_worker-0.0.4/aiy_worker/utils.py` & `aiy_worker-0.0.5/aiy_worker/utils.py`

 * *Files identical despite different names*

### Comparing `aiy_worker-0.0.4/aiy_worker/worker.py` & `aiy_worker-0.0.5/aiy_worker/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,17 @@
   subscription ($token: String!) {
     subscribeTasks(token: $token) {
         id
         text2Image {
             prompt
             negativePrompt
             seed
+            width
+            height
+            nSteps
         }
     }
   }
 """
 
 
 def wait_shutdown(fn: Callable):
```

### Comparing `aiy_worker-0.0.4/aiy_worker/ws_client.py` & `aiy_worker-0.0.5/aiy_worker/ws_client.py`

 * *Files identical despite different names*

### Comparing `aiy_worker-0.0.4/setup.py` & `aiy_worker-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 if os.path.exists("requirements.txt"):
     install_requires = [i for i in io.open("requirements.txt").read().split("\n") if i]
 else:
     install_requires = []
 print(install_requires)
 setuptools.setup(
     name="aiy_worker",
-    version="0.0.4",
+    version="0.0.5",
     author="zgljl2012",
     # license = 'MIT License',
     # author_email="pengshiyuyx@gmail.com",
     description="aiy worker",
     long_description=long_description,
     # long_description_content_type="text/x-rst",
     # url="https://github.com/mouday/chinesename",
```

