# Comparing `tmp/git-stats-report-0.2.0.tar.gz` & `tmp/git-stats-report-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-stats-report-0.2.0.tar", last modified: Wed Apr  3 17:35:01 2024, max compression
+gzip compressed data, was "git-stats-report-0.2.1.tar", last modified: Wed Apr  3 18:12:07 2024, max compression
```

## Comparing `git-stats-report-0.2.0.tar` & `git-stats-report-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/git_stats_report/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/git_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/git_stats_report/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/strategy/from_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/strategy/from_latest_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/strategy/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/git_stats_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:12:07.269931 git-stats-report-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 18:12:07.269931 git-stats-report-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:12:07.265931 git-stats-report-0.2.1/git_stats_report/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/git_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:12:07.269931 git-stats-report-0.2.1/git_stats_report/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/strategy/from_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/strategy/from_latest_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/strategy/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/git_stats_report/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:12:07.269931 git-stats-report-0.2.1/git_stats_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 18:12:07.000000 git-stats-report-0.2.1/git_stats_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 18:12:07.000000 git-stats-report-0.2.1/git_stats_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:12:07.000000 git-stats-report-0.2.1/git_stats_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 18:12:07.000000 git-stats-report-0.2.1/git_stats_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 18:12:07.000000 git-stats-report-0.2.1/git_stats_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 18:12:07.000000 git-stats-report-0.2.1/git_stats_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-03 18:12:00.000000 git-stats-report-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:12:07.269931 git-stats-report-0.2.1/setup.cfg
```

### Comparing `git-stats-report-0.2.0/LICENSE` & `git-stats-report-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.2.0/PKG-INFO` & `git-stats-report-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.2.0
+Version: 0.2.1
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `git-stats-report-0.2.0/Pipfile` & `git-stats-report-0.2.1/Pipfile`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.2.0/README.md` & `git-stats-report-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.2.0/git_stats_report/__main__.py` & `git-stats-report-0.2.1/git_stats_report/__main__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.2.0/git_stats_report/entrypoint.py` & `git-stats-report-0.2.1/git_stats_report/entrypoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,20 +7,19 @@
 def run(strategy: Strategy, since: Optional[str], *, raw_format: bool) -> None:
     datetime_factory = get_datetime_factory_from_strategy(strategy)
     since_datetime = datetime_factory(since)
 
     git_stats = get_git_stats(since_datetime)
     total_commits = get_total_commits(git_stats)
 
+    output: str = ""
+
     for author in git_stats["authors"]:
         if not author["value"]:
             continue
         author_info = get_author_info(author, since_datetime)
         percentage_of_total = (author["value"] * 100) / total_commits
-        output = (
-            f'{author["label"]}: {author["value"]} commits ({percentage_of_total:.2f}% of total) {author_info}\n',
-        )  # pylint: disable=line-too-long
+        tmp_output = f'{author["label"]}: {author["value"]} commits ({percentage_of_total:.2f}% of total) {author_info}\n'  # pylint: disable=line-too-long
         if raw_format:
-            output = (
-                rf'{author["label"]}: {author["value"]} commits ({percentage_of_total:.2f}% of total) {author_info}\n',
-            )  # pylint: disable=line-too-long
-        print(output)
+            tmp_output = rf'{author["label"]}: {author["value"]} commits ({percentage_of_total:.2f}% of total) {author_info}\n'  # pylint: disable=line-too-long
+        output += tmp_output
+    print(output)
```

### Comparing `git-stats-report-0.2.0/git_stats_report/git_stats.py` & `git-stats-report-0.2.1/git_stats_report/git_stats.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.2.0/git_stats_report/strategy/__init__.py` & `git-stats-report-0.2.1/git_stats_report/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.2.0/git_stats_report/strategy/from_latest_tag.py` & `git-stats-report-0.2.1/git_stats_report/strategy/from_latest_tag.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.2.0/git_stats_report.egg-info/PKG-INFO` & `git-stats-report-0.2.1/git_stats_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.2.0
+Version: 0.2.1
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `git-stats-report-0.2.0/git_stats_report.egg-info/SOURCES.txt` & `git-stats-report-0.2.1/git_stats_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.2.0/pyproject.toml` & `git-stats-report-0.2.1/pyproject.toml`

 * *Files identical despite different names*

