# Comparing `tmp/elasticsearch_ir_evaluator-0.4.3.tar.gz` & `tmp/elasticsearch_ir_evaluator-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elasticsearch_ir_evaluator-0.4.3.tar", last modified: Tue Apr  2 02:55:30 2024, max compression
+gzip compressed data, was "elasticsearch_ir_evaluator-0.4.4.tar", last modified: Wed Apr  3 04:39:52 2024, max compression
```

## Comparing `elasticsearch_ir_evaluator-0.4.3.tar` & `elasticsearch_ir_evaluator-0.4.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-02 02:55:30.397906 elasticsearch_ir_evaluator-0.4.3/
--rw-r--r--   0 hinatades   (501) staff       (20)    11357 2023-12-30 14:43:03.000000 elasticsearch_ir_evaluator-0.4.3/LICENSE
--rw-r--r--   0 hinatades   (501) staff       (20)     6288 2024-04-02 02:55:30.397753 elasticsearch_ir_evaluator-0.4.3/PKG-INFO
--rw-r--r--   0 hinatades   (501) staff       (20)     5870 2024-04-02 02:24:49.000000 elasticsearch_ir_evaluator-0.4.3/README.md
-drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-02 02:55:30.396282 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator/
--rw-r--r--   0 hinatades   (501) staff       (20)       83 2024-01-01 18:30:57.000000 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator/__init__.py
--rw-r--r--   0 hinatades   (501) staff       (20)    29687 2024-04-02 02:53:34.000000 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator/evaluator.py
--rw-r--r--   0 hinatades   (501) staff       (20)     2429 2024-03-28 17:34:09.000000 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator/types.py
-drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-02 02:55:30.397206 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator.egg-info/
--rw-r--r--   0 hinatades   (501) staff       (20)     6288 2024-04-02 02:55:30.000000 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator.egg-info/PKG-INFO
--rw-r--r--   0 hinatades   (501) staff       (20)      432 2024-04-02 02:55:30.000000 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator.egg-info/SOURCES.txt
--rw-r--r--   0 hinatades   (501) staff       (20)        1 2024-04-02 02:55:30.000000 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator.egg-info/dependency_links.txt
--rw-r--r--   0 hinatades   (501) staff       (20)       40 2024-04-02 02:55:30.000000 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator.egg-info/requires.txt
--rw-r--r--   0 hinatades   (501) staff       (20)       33 2024-04-02 02:55:30.000000 elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator.egg-info/top_level.txt
--rw-r--r--   0 hinatades   (501) staff       (20)       38 2024-04-02 02:55:30.397954 elasticsearch_ir_evaluator-0.4.3/setup.cfg
--rw-r--r--   0 hinatades   (501) staff       (20)      675 2024-04-02 02:53:52.000000 elasticsearch_ir_evaluator-0.4.3/setup.py
-drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-02 02:55:30.397471 elasticsearch_ir_evaluator-0.4.3/tests/
--rw-r--r--   0 hinatades   (501) staff       (20)        0 2024-01-01 15:00:06.000000 elasticsearch_ir_evaluator-0.4.3/tests/__init__.py
--rw-r--r--   0 hinatades   (501) staff       (20)     2157 2024-03-28 17:34:09.000000 elasticsearch_ir_evaluator-0.4.3/tests/test_evaluator.py
+drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-03 04:39:52.883530 elasticsearch_ir_evaluator-0.4.4/
+-rw-r--r--   0 hinatades   (501) staff       (20)    11357 2023-12-30 14:43:03.000000 elasticsearch_ir_evaluator-0.4.4/LICENSE
+-rw-r--r--   0 hinatades   (501) staff       (20)     6288 2024-04-03 04:39:52.883346 elasticsearch_ir_evaluator-0.4.4/PKG-INFO
+-rw-r--r--   0 hinatades   (501) staff       (20)     5870 2024-04-02 02:24:49.000000 elasticsearch_ir_evaluator-0.4.4/README.md
+drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-03 04:39:52.881613 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator/
+-rw-r--r--   0 hinatades   (501) staff       (20)       83 2024-01-01 18:30:57.000000 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator/__init__.py
+-rw-r--r--   0 hinatades   (501) staff       (20)    29697 2024-04-02 04:28:38.000000 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator/evaluator.py
+-rw-r--r--   0 hinatades   (501) staff       (20)     2429 2024-03-28 17:34:09.000000 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator/types.py
+drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-03 04:39:52.882591 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator.egg-info/
+-rw-r--r--   0 hinatades   (501) staff       (20)     6288 2024-04-03 04:39:52.000000 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator.egg-info/PKG-INFO
+-rw-r--r--   0 hinatades   (501) staff       (20)      432 2024-04-03 04:39:52.000000 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator.egg-info/SOURCES.txt
+-rw-r--r--   0 hinatades   (501) staff       (20)        1 2024-04-03 04:39:52.000000 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator.egg-info/dependency_links.txt
+-rw-r--r--   0 hinatades   (501) staff       (20)       40 2024-04-03 04:39:52.000000 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator.egg-info/requires.txt
+-rw-r--r--   0 hinatades   (501) staff       (20)       33 2024-04-03 04:39:52.000000 elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator.egg-info/top_level.txt
+-rw-r--r--   0 hinatades   (501) staff       (20)       38 2024-04-03 04:39:52.883582 elasticsearch_ir_evaluator-0.4.4/setup.cfg
+-rw-r--r--   0 hinatades   (501) staff       (20)      675 2024-04-03 04:38:08.000000 elasticsearch_ir_evaluator-0.4.4/setup.py
+drwxr-xr-x   0 hinatades   (501) staff       (20)        0 2024-04-03 04:39:52.882839 elasticsearch_ir_evaluator-0.4.4/tests/
+-rw-r--r--   0 hinatades   (501) staff       (20)        0 2024-01-01 15:00:06.000000 elasticsearch_ir_evaluator-0.4.4/tests/__init__.py
+-rw-r--r--   0 hinatades   (501) staff       (20)     2157 2024-03-28 17:34:09.000000 elasticsearch_ir_evaluator-0.4.4/tests/test_evaluator.py
```

### Comparing `elasticsearch_ir_evaluator-0.4.3/LICENSE` & `elasticsearch_ir_evaluator-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `elasticsearch_ir_evaluator-0.4.3/PKG-INFO` & `elasticsearch_ir_evaluator-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch_ir_evaluator
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python package for easily calculating information retrieval (IR) accuracy metrics using Elasticsearch and datasets.
 Home-page: https://github.com/hinatades/elasticsearch-ir-evaluator
 Author: Taisuke Hinata
 Author-email: hnttisk@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `elasticsearch_ir_evaluator-0.4.3/README.md` & `elasticsearch_ir_evaluator-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator/evaluator.py` & `elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator/evaluator.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,14 +226,15 @@
 
         Args:
             actions (List[Dict]): A list of actions (documents) to be bulk indexed.
         """
         retries = 0
         while retries < self.max_retries:
             try:
+                self.logger.info(f"Bulking {len(actions)} documents to {self.index_name}")
                 bulk(self.es, actions)
                 break
             except BulkIndexError as e:
                 self.logger.warning(f"Bulk indexing failed: {e.errors}")
                 actions = [
                     action
                     for action, error in zip(actions, e.errors)
@@ -260,15 +261,14 @@
             self._create_index(documents[0])
 
         actions = []
         doc_count = len(documents)
         skip = True if self.last_processed_id else False
         skip_count = 0
         end = 0
-        self.logger.info(f"Indexing {doc_count} documents to {self.index_name}")
         for doc in documents:
 
             if skip:
                 skip_count += 1
                 if doc.id == self.last_processed_id:
                     self.logger.info(f"Skipped {skip_count} documents")
                     self.logger.info(f"Resume indexing from ID:{self.last_processed_id}")
```

### Comparing `elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator/types.py` & `elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator/types.py`

 * *Files identical despite different names*

### Comparing `elasticsearch_ir_evaluator-0.4.3/elasticsearch_ir_evaluator.egg-info/PKG-INFO` & `elasticsearch_ir_evaluator-0.4.4/elasticsearch_ir_evaluator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticsearch-ir-evaluator
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python package for easily calculating information retrieval (IR) accuracy metrics using Elasticsearch and datasets.
 Home-page: https://github.com/hinatades/elasticsearch-ir-evaluator
 Author: Taisuke Hinata
 Author-email: hnttisk@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `elasticsearch_ir_evaluator-0.4.3/setup.py` & `elasticsearch_ir_evaluator-0.4.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="elasticsearch_ir_evaluator",
-    version="0.4.3",
+    version="0.4.4",
     description="A Python package for easily calculating information retrieval (IR) accuracy metrics using Elasticsearch and datasets.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     python_requires=">=3.8",
     url="https://github.com/hinatades/elasticsearch-ir-evaluator",
     author="Taisuke Hinata",
     author_email="hnttisk@gmail.com",
```

### Comparing `elasticsearch_ir_evaluator-0.4.3/tests/test_evaluator.py` & `elasticsearch_ir_evaluator-0.4.4/tests/test_evaluator.py`

 * *Files identical despite different names*

