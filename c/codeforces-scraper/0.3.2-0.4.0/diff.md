# Comparing `tmp/codeforces-scraper-0.3.2.tar.gz` & `tmp/codeforces-scraper-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codeforces-scraper-0.3.2.tar", last modified: Wed Apr  3 18:56:57 2024, max compression
+gzip compressed data, was "codeforces-scraper-0.4.0.tar", last modified: Wed Apr  3 19:26:21 2024, max compression
```

## Comparing `codeforces-scraper-0.3.2.tar` & `codeforces-scraper-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/
--rw-------   0 thematdev  (1000) thematdev  (1000)     1211 2023-01-24 17:57:52.000000 codeforces-scraper-0.3.2/LICENSE
--rw-r--r--   0 thematdev  (1000) thematdev  (1000)      295 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/PKG-INFO
--rw-------   0 thematdev  (1000) thematdev  (1000)      713 2023-02-17 15:55:45.000000 codeforces-scraper-0.3.2/README.md
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/codeforces_scraper/
--rw-------   0 thematdev  (1000) thematdev  (1000)       81 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.2/codeforces_scraper/__init__.py
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/codeforces_scraper/assets/
--rw-------   0 thematdev  (1000) thematdev  (1000)        1 2022-10-29 14:40:08.000000 codeforces-scraper-0.3.2/codeforces_scraper/assets/__init__.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     3505 2022-10-29 17:02:59.000000 codeforces-scraper-0.3.2/codeforces_scraper/assets/all_language_compilers.json
--rw-------   0 thematdev  (1000) thematdev  (1000)     1580 2023-01-22 07:08:22.000000 codeforces-scraper-0.3.2/codeforces_scraper/languages.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     5044 2024-04-03 18:46:44.000000 codeforces-scraper-0.3.2/codeforces_scraper/models.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     8474 2023-08-13 14:52:10.000000 codeforces-scraper-0.3.2/codeforces_scraper/scraper.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     1236 2023-08-13 14:49:00.000000 codeforces-scraper-0.3.2/codeforces_scraper/utils.py
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/
--rw-r--r--   0 thematdev  (1000) thematdev  (1000)      295 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/PKG-INFO
--rw-------   0 thematdev  (1000) thematdev  (1000)      596 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/SOURCES.txt
--rw-------   0 thematdev  (1000) thematdev  (1000)        1 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/dependency_links.txt
--rw-------   0 thematdev  (1000) thematdev  (1000)       27 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/requires.txt
--rw-------   0 thematdev  (1000) thematdev  (1000)       19 2024-04-03 18:56:57.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/top_level.txt
--rw-------   0 thematdev  (1000) thematdev  (1000)        1 2022-10-29 16:51:50.000000 codeforces-scraper-0.3.2/codeforces_scraper.egg-info/zip-safe
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/fetch_compilers_info/
--rw-------   0 thematdev  (1000) thematdev  (1000)      830 2024-03-06 19:52:13.000000 codeforces-scraper-0.3.2/fetch_compilers_info/fetch.py
--rw-------   0 thematdev  (1000) thematdev  (1000)      100 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.2/pyproject.toml
--rw-r--r--   0 thematdev  (1000) thematdev  (1000)       38 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/setup.cfg
--rw-------   0 thematdev  (1000) thematdev  (1000)      565 2024-04-03 18:56:20.000000 codeforces-scraper-0.3.2/setup.py
-drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 18:56:57.766745 codeforces-scraper-0.3.2/tests/
--rw-------   0 thematdev  (1000) thematdev  (1000)        0 2021-12-10 19:33:19.000000 codeforces-scraper-0.3.2/tests/__init__.py
--rw-------   0 thematdev  (1000) thematdev  (1000)     1746 2022-04-14 13:26:19.000000 codeforces-scraper-0.3.2/tests/test_main.py
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 19:26:21.446784 codeforces-scraper-0.4.0/
+-rw-------   0 thematdev  (1000) thematdev  (1000)     1211 2023-01-24 17:57:52.000000 codeforces-scraper-0.4.0/LICENSE
+-rw-r--r--   0 thematdev  (1000) thematdev  (1000)      295 2024-04-03 19:26:21.446784 codeforces-scraper-0.4.0/PKG-INFO
+-rw-------   0 thematdev  (1000) thematdev  (1000)      713 2023-02-17 15:55:45.000000 codeforces-scraper-0.4.0/README.md
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 19:26:21.446784 codeforces-scraper-0.4.0/codeforces_scraper/
+-rw-------   0 thematdev  (1000) thematdev  (1000)       81 2021-12-10 19:33:19.000000 codeforces-scraper-0.4.0/codeforces_scraper/__init__.py
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 19:26:21.446784 codeforces-scraper-0.4.0/codeforces_scraper/assets/
+-rw-------   0 thematdev  (1000) thematdev  (1000)        1 2022-10-29 14:40:08.000000 codeforces-scraper-0.4.0/codeforces_scraper/assets/__init__.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     3505 2022-10-29 17:02:59.000000 codeforces-scraper-0.4.0/codeforces_scraper/assets/all_language_compilers.json
+-rw-------   0 thematdev  (1000) thematdev  (1000)     1580 2023-01-22 07:08:22.000000 codeforces-scraper-0.4.0/codeforces_scraper/languages.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     5282 2024-04-03 19:22:06.000000 codeforces-scraper-0.4.0/codeforces_scraper/models.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     8479 2024-04-03 19:22:35.000000 codeforces-scraper-0.4.0/codeforces_scraper/scraper.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     1236 2023-08-13 14:49:00.000000 codeforces-scraper-0.4.0/codeforces_scraper/utils.py
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 19:26:21.446784 codeforces-scraper-0.4.0/codeforces_scraper.egg-info/
+-rw-r--r--   0 thematdev  (1000) thematdev  (1000)      295 2024-04-03 19:26:21.000000 codeforces-scraper-0.4.0/codeforces_scraper.egg-info/PKG-INFO
+-rw-------   0 thematdev  (1000) thematdev  (1000)      596 2024-04-03 19:26:21.000000 codeforces-scraper-0.4.0/codeforces_scraper.egg-info/SOURCES.txt
+-rw-------   0 thematdev  (1000) thematdev  (1000)        1 2024-04-03 19:26:21.000000 codeforces-scraper-0.4.0/codeforces_scraper.egg-info/dependency_links.txt
+-rw-------   0 thematdev  (1000) thematdev  (1000)       27 2024-04-03 19:26:21.000000 codeforces-scraper-0.4.0/codeforces_scraper.egg-info/requires.txt
+-rw-------   0 thematdev  (1000) thematdev  (1000)       19 2024-04-03 19:26:21.000000 codeforces-scraper-0.4.0/codeforces_scraper.egg-info/top_level.txt
+-rw-------   0 thematdev  (1000) thematdev  (1000)        1 2022-10-29 16:51:50.000000 codeforces-scraper-0.4.0/codeforces_scraper.egg-info/zip-safe
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 19:26:21.446784 codeforces-scraper-0.4.0/fetch_compilers_info/
+-rw-------   0 thematdev  (1000) thematdev  (1000)      830 2024-03-06 19:52:13.000000 codeforces-scraper-0.4.0/fetch_compilers_info/fetch.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)      100 2021-12-10 19:33:19.000000 codeforces-scraper-0.4.0/pyproject.toml
+-rw-r--r--   0 thematdev  (1000) thematdev  (1000)       38 2024-04-03 19:26:21.446784 codeforces-scraper-0.4.0/setup.cfg
+-rw-------   0 thematdev  (1000) thematdev  (1000)      565 2024-04-03 19:25:02.000000 codeforces-scraper-0.4.0/setup.py
+drwxr-xr-x   0 thematdev  (1000) thematdev  (1000)        0 2024-04-03 19:26:21.446784 codeforces-scraper-0.4.0/tests/
+-rw-------   0 thematdev  (1000) thematdev  (1000)        0 2021-12-10 19:33:19.000000 codeforces-scraper-0.4.0/tests/__init__.py
+-rw-------   0 thematdev  (1000) thematdev  (1000)     1746 2024-04-03 19:15:46.000000 codeforces-scraper-0.4.0/tests/test_main.py
```

### Comparing `codeforces-scraper-0.3.2/LICENSE` & `codeforces-scraper-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.2/README.md` & `codeforces-scraper-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.2/codeforces_scraper/assets/all_language_compilers.json` & `codeforces-scraper-0.4.0/codeforces_scraper/assets/all_language_compilers.json`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.2/codeforces_scraper/languages.py` & `codeforces-scraper-0.4.0/codeforces_scraper/languages.py`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.2/codeforces_scraper/models.py` & `codeforces-scraper-0.4.0/codeforces_scraper/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,39 +67,39 @@
 class APIModel(BaseModel):
     class Config:
         alias_generator = de_eblanify
 
 
 class JudgeProtocol(APIModel):
     manual: bool
-    protocol: Optional[str]
-    verdict: Optional[str]
+    protocol: Optional[str] = None
+    verdict: Optional[str] = None
 
 
 class BlogEntry(APIModel):
     id: int
     original_locale: str
     creation_time_seconds: int
     author_handle: str
     title: str
-    content: Optional[str]
+    content: Optional[str] = None
     locale: str
     modification_time_seconds: int
     allow_view_history: bool
     tags: List[str]
     rating: int
 
 
 class Comment(APIModel):
     id: int
     creation_time_seconds: int
     commentator_handle: str
     locale: str
     text: str
-    parent_comment_id: Optional[int]
+    parent_comment_id: Optional[int] = None
     rating: int
 
 
 class RecentAction(APIModel):
     time_seconds: int
     blog_entry: BlogEntry
     comment: Comment
@@ -122,34 +122,34 @@
 
 
 class Member(APIModel):
     handle: str
 
 
 class Problem(APIModel):
-    contest_id: Optional[int]
-    problem_set_name: Optional[str]
+    contest_id: Optional[int] = None
+    problem_set_name: Optional[str] = None
     index: str
     name: str
     type: str
-    points: Optional[float]
-    rating: Optional[int]
+    points: Optional[float] = None
+    rating: Optional[int] = None
     tags: List[str]
 
 
 class User(APIModel):
     handle: str
-    email: Optional[str]
-    vk_id: Optional[str]
-    open_id: Optional[str]
-    first_name: Optional[str]
-    last_name: Optional[str]
-    country: Optional[str]
-    city: Optional[str]
-    organization: Optional[str]
+    email: Optional[str] = None
+    vk_id: Optional[str] = None
+    open_id: Optional[str] = None
+    first_name: Optional[str] = None
+    last_name: Optional[str] = None
+    country: Optional[str] = None
+    city: Optional[str] = None
+    organization: Optional[str] = None
     contribution: int
     rank: str
     rating: int
     max_rank: str
     max_rating: int
     last_online_time_seconds: int
     registration_time_seconds: int
@@ -158,64 +158,64 @@
     title_photo: str
 
 
 class Party(APIModel):
     contest_id: int
     members: List[Member]
     participant_type: str
-    team_id: Optional[int]
-    team_name: Optional[str]
+    team_id: Optional[int] = None
+    team_name: Optional[str] = None
     ghost: bool
-    room: Optional[int]
-    start_time_seconds: Optional[int]
+    room: Optional[int] = None
+    start_time_seconds: Optional[int] = None
 
 
 class Submission(APIModel):
     id: int
     contest_id: int
     creation_time_seconds: int
     relative_time_seconds: int
     problem: Problem
     author: Party
     programming_language: str
-    verdict: Optional[Verdict]
+    verdict: Optional[Verdict] = None
     testset: str
     passed_test_count: int
     time_consumed_millis: int
     memory_consumed_bytes: int
-    points: Optional[float]
+    points: Optional[float] = None
 
 
 class Contest(APIModel):
     id: int
     name: str
     type: ContestType
     phase: ContestPhase
     frozen: bool
     duration_seconds: bool
-    start_time_seconds: Optional[int]
-    relative_time_seconds: Optional[int]
-    prepared_by: Optional[str]
-    website_url: Optional[str]
-    description: Optional[str]
-    difficulty: Optional[int]
-    kind: Optional[str]
-    icpc_region: Optional[str]
-    country: Optional[str]
-    city: Optional[str]
-    season: Optional[str]
+    start_time_seconds: Optional[int] = None
+    relative_time_seconds: Optional[int] = None
+    prepared_by: Optional[str] = None
+    website_url: Optional[str] = None
+    description: Optional[str] = None
+    difficulty: Optional[int] = None
+    kind: Optional[str] = None
+    icpc_region: Optional[str] = None
+    country: Optional[str] = None
+    city: Optional[str] = None
+    season: Optional[str] = None
 
 
 class Hack(APIModel):
     id: int
     creation_time_seconds: int
     hacker: Party
     defender: Party
     problem: Problem
-    test: Optional[str]
+    test: Optional[str] = None
     judge_protocol: JudgeProtocol
 
 
 class ProblemResult(APIModel):
     points: float
     penalty: int
     rejected_attempt_count: int
```

### Comparing `codeforces-scraper-0.3.2/codeforces_scraper/scraper.py` & `codeforces-scraper-0.4.0/codeforces_scraper/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
         if username is not None:
             params = {
                 'contestId': contest_id,
                 'handle': username
             }
         else:
             params = {'contestId': contest_id}
-        return [Submission.parse_obj(x) for x in self.api_request('contest.status', params)]
+        return [Submission.model_validate(x) for x in self.api_request('contest.status', params)]
 
     def get_contest_tasks(self, contest_id: int) -> List[Problem]:
         """Get all tasks in contest with id ``contest_id``"""
         params = {
             'from': 1,
             'count': 1
         }
```

### Comparing `codeforces-scraper-0.3.2/codeforces_scraper/utils.py` & `codeforces-scraper-0.4.0/codeforces_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.2/codeforces_scraper.egg-info/SOURCES.txt` & `codeforces-scraper-0.4.0/codeforces_scraper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.2/fetch_compilers_info/fetch.py` & `codeforces-scraper-0.4.0/fetch_compilers_info/fetch.py`

 * *Files identical despite different names*

### Comparing `codeforces-scraper-0.3.2/setup.py` & `codeforces-scraper-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
         name='codeforces-scraper',
-        version='0.3.2',
+        version='0.4.0',
         author='thematdev',
         author_email='thematdev@thematdev.org',
         description='Utility to do actions on codeforces',
         packages=['codeforces_scraper', 'codeforces_scraper.assets'],
         install_requires=[
             'bs4',
             'lxml',
```

### Comparing `codeforces-scraper-0.3.2/tests/test_main.py` & `codeforces-scraper-0.4.0/tests/test_main.py`

 * *Files identical despite different names*

