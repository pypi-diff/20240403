# Comparing `tmp/codeforces-scraper-0.3.1.tar.gz` & `tmp/codeforces-scraper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeforces-scraper-0.3.1.tar", last modified: Sun Aug 13 14:58:48 2023, max compression
+gzip compressed data, was "codeforces-scraper-0.3.2.tar", last modified: Wed Apr  3 18:56:57 2024, max compression
```

## Comparing `codeforces-scraper-0.3.1.tar` & `codeforces-scraper-0.3.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2023-08-13 14:58:48.366723 codeforces-scraper-0.3.1/
--rw-------   0 thematdev  (1000) thematdev  (1000)     1211 2023-01-24 17:57:52.000000 codeforces-scraper-0.3.1/LICENSE
--rw-r--r--   0 thematdev  (1000) thematdev  (1000)      208 2023-08-13 14:58:48.366723 codeforces-scraper-0.3.1/PKG-INFO
--rw-------   0 thematdev  (1000) thematdev  (1000)      713 2023-02-17 15:55:45.000000 codeforces-scraper-0.3.1/README.md
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2023-08-13 14:58:48.363389 codeforces-scraper-0.3.1/codeforces_scraper/
--rw-------   0 thematdev  (1000) thematdev  (1000)       81 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.1/codeforces_scraper/__init__.py
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2023-08-13 14:58:48.366723 codeforces-scraper-0.3.1/codeforces_scraper/assets/
--rw-------   0 thematdev  (1000) thematdev  (1000)        1 2022-10-29 14:40:08.000000 codeforces-scraper-0.3.1/codeforces_scraper/assets/__init__.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     3505 2022-10-29 17:02:59.000000 codeforces-scraper-0.3.1/codeforces_scraper/assets/all_language_compilers.json
--rw-------   0 thematdev  (1000) thematdev  (1000)     1580 2023-01-22 07:08:22.000000 codeforces-scraper-0.3.1/codeforces_scraper/languages.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     5045 2023-06-26 16:52:05.000000 codeforces-scraper-0.3.1/codeforces_scraper/models.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     8474 2023-08-13 14:52:10.000000 codeforces-scraper-0.3.1/codeforces_scraper/scraper.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     1236 2023-08-13 14:49:00.000000 codeforces-scraper-0.3.1/codeforces_scraper/utils.py
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2023-08-13 14:58:48.366723 codeforces-scraper-0.3.1/codeforces_scraper.egg-info/
--rw-------   0 thematdev  (1000) thematdev  (1000)      208 2023-08-13 14:58:48.000000 codeforces-scraper-0.3.1/codeforces_scraper.egg-info/PKG-INFO
--rw-------   0 thematdev  (1000) thematdev  (1000)      596 2023-08-13 14:58:48.000000 codeforces-scraper-0.3.1/codeforces_scraper.egg-info/SOURCES.txt
--rw-------   0 thematdev  (1000) thematdev  (1000)        1 2023-08-13 14:58:48.000000 codeforces-scraper-0.3.1/codeforces_scraper.egg-info/dependency_links.txt
--rw-------   0 thematdev  (1000) thematdev  (1000)       27 2023-08-13 14:58:48.000000 codeforces-scraper-0.3.1/codeforces_scraper.egg-info/requires.txt
--rw-------   0 thematdev  (1000) thematdev  (1000)       19 2023-08-13 14:58:48.000000 codeforces-scraper-0.3.1/codeforces_scraper.egg-info/top_level.txt
--rw-------   0 thematdev  (1000) thematdev  (1000)        1 2022-10-29 16:51:50.000000 codeforces-scraper-0.3.1/codeforces_scraper.egg-info/zip-safe
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2023-08-13 14:58:48.366723 codeforces-scraper-0.3.1/fetch_compilers_info/
--rw-------   0 thematdev  (1000) thematdev  (1000)      830 2022-11-10 18:28:48.000000 codeforces-scraper-0.3.1/fetch_compilers_info/fetch.py
--rw-------   0 thematdev  (1000) thematdev  (1000)      100 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.1/pyproject.toml
--rw-r--r--   0 thematdev  (1000) thematdev  (1000)       38 2023-08-13 14:58:48.366723 codeforces-scraper-0.3.1/setup.cfg
--rw-------   0 thematdev  (1000) thematdev  (1000)      565 2023-06-26 17:02:01.000000 codeforces-scraper-0.3.1/setup.py
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2023-08-13 14:58:48.366723 codeforces-scraper-0.3.1/tests/
--rw-------   0 thematdev  (1000) thematdev  (1000)        0 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.1/tests/__init__.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     1746 2022-04-14 13:26:19.000000 codeforces-scraper-0.3.1/tests/test_main.py
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/
+-rw-------   0 thematdev  (1000) thematdev  (1000)     1211 2023-01-24 17:57:52.000000 codeforces-scraper-0.3.2/LICENSE
+-rw-r--r--   0 thematdev  (1000) thematdev  (1000)      295 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/PKG-INFO
+-rw-------   0 thematdev  (1000) thematdev  (1000)      713 2023-02-17 15:55:45.000000 codeforces-scraper-0.3.2/README.md
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/codeforces_scraper/
+-rw-------   0 thematdev  (1000) thematdev  (1000)       81 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.2/codeforces_scraper/__init__.py
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/codeforces_scraper/assets/
+-rw-------   0 thematdev  (1000) thematdev  (1000)        1 2022-10-29 14:40:08.000000 codeforces-scraper-0.3.2/codeforces_scraper/assets/__init__.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     3505 2022-10-29 17:02:59.000000 codeforces-scraper-0.3.2/codeforces_scraper/assets/all_language_compilers.json
+-rw-------   0 thematdev  (1000) thematdev  (1000)     1580 2023-01-22 07:08:22.000000 codeforces-scraper-0.3.2/codeforces_scraper/languages.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     5044 2024-04-03 18:46:44.000000 codeforces-scraper-0.3.2/codeforces_scraper/models.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     8474 2023-08-13 14:52:10.000000 codeforces-scraper-0.3.2/codeforces_scraper/scraper.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     1236 2023-08-13 14:49:00.000000 codeforces-scraper-0.3.2/codeforces_scraper/utils.py
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/
+-rw-r--r--   0 thematdev  (1000) thematdev  (1000)      295 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/PKG-INFO
+-rw-------   0 thematdev  (1000) thematdev  (1000)      596 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/SOURCES.txt
+-rw-------   0 thematdev  (1000) thematdev  (1000)        1 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/dependency_links.txt
+-rw-------   0 thematdev  (1000) thematdev  (1000)       27 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/requires.txt
+-rw-------   0 thematdev  (1000) thematdev  (1000)       19 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/top_level.txt
+-rw-------   0 thematdev  (1000) thematdev  (1000)        1 2022-10-29 16:51:50.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/zip-safe
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/fetch_compilers_info/
+-rw-------   0 thematdev  (1000) thematdev  (1000)      830 2024-03-06 19:52:13.000000 codeforces-scraper-0.3.2/fetch_compilers_info/fetch.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)      100 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.2/pyproject.toml
+-rw-r--r--   0 thematdev  (1000) thematdev  (1000)       38 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/setup.cfg
+-rw-------   0 thematdev  (1000) thematdev  (1000)      565 2024-04-03 18:56:20.000000 codeforces-scraper-0.3.2/setup.py
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/tests/
+-rw-------   0 thematdev  (1000) thematdev  (1000)        0 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.2/tests/__init__.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     1746 2022-04-14 13:26:19.000000 codeforces-scraper-0.3.2/tests/test_main.py
```

### Comparing `codeforces-scraper-0.3.1/LICENSE` & `codeforces-scraper-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.1/README.md` & `codeforces-scraper-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.1/codeforces_scraper/assets/all_language_compilers.json` & `codeforces-scraper-0.3.2/codeforces_scraper/assets/all_language_compilers.json`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.1/codeforces_scraper/languages.py` & `codeforces-scraper-0.3.2/codeforces_scraper/languages.py`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.1/codeforces_scraper/models.py` & `codeforces-scraper-0.3.2/codeforces_scraper/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 class Hack(APIModel):
     id: int
     creation_time_seconds: int
     hacker: Party
     defender: Party
     problem: Problem
     test: Optional[str]
-    judge_protocol = JudgeProtocol
+    judge_protocol: JudgeProtocol
 
 
 class ProblemResult(APIModel):
     points: float
     penalty: int
     rejected_attempt_count: int
     type: ProblemResultType
```

### Comparing `codeforces-scraper-0.3.1/codeforces_scraper/scraper.py` & `codeforces-scraper-0.3.2/codeforces_scraper/scraper.py`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.1/codeforces_scraper/utils.py` & `codeforces-scraper-0.3.2/codeforces_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.1/codeforces_scraper.egg-info/SOURCES.txt` & `codeforces-scraper-0.3.2/codeforces_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.1/fetch_compilers_info/fetch.py` & `codeforces-scraper-0.3.2/fetch_compilers_info/fetch.py`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.1/setup.py` & `codeforces-scraper-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
         name='codeforces-scraper',
-        version='0.3.1',
+        version='0.3.2',
         author='thematdev',
         author_email='thematdev@thematdev.org',
         description='Utility to do actions on codeforces',
         packages=['codeforces_scraper', 'codeforces_scraper.assets'],
         install_requires=[
             'bs4',
             'lxml',
```

### Comparing `codeforces-scraper-0.3.1/tests/test_main.py` & `codeforces-scraper-0.3.2/tests/test_main.py`

 * *Files identical despite different names*

