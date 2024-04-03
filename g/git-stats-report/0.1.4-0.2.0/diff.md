# Comparing `tmp/git-stats-report-0.1.4.tar.gz` & `tmp/git-stats-report-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-stats-report-0.1.4.tar", last modified: Wed Apr  3 02:35:20 2024, max compression
+gzip compressed data, was "git-stats-report-0.2.0.tar", last modified: Wed Apr  3 17:35:01 2024, max compression
```

## Comparing `git-stats-report-0.1.4.tar` & `git-stats-report-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:35:20.382696 git-stats-report-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 02:35:20.382696 git-stats-report-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:35:20.378696 git-stats-report-0.1.4/git_stats_report/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/git_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:35:20.382696 git-stats-report-0.1.4/git_stats_report/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/strategy/from_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/strategy/from_latest_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/strategy/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/git_stats_report/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:35:20.378696 git-stats-report-0.1.4/git_stats_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 02:35:20.000000 git-stats-report-0.1.4/git_stats_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 02:35:20.000000 git-stats-report-0.1.4/git_stats_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:35:20.000000 git-stats-report-0.1.4/git_stats_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 02:35:20.000000 git-stats-report-0.1.4/git_stats_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 02:35:20.000000 git-stats-report-0.1.4/git_stats_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 02:35:20.000000 git-stats-report-0.1.4/git_stats_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-03 02:35:12.000000 git-stats-report-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 02:35:20.382696 git-stats-report-0.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/git_stats_report/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/git_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/git_stats_report/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/strategy/from_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/strategy/from_latest_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/strategy/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/git_stats_report/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/git_stats_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 17:35:01.000000 git-stats-report-0.2.0/git_stats_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-03 17:34:53.000000 git-stats-report-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:35:01.894558 git-stats-report-0.2.0/setup.cfg
```

### Comparing `git-stats-report-0.1.4/LICENSE` & `git-stats-report-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.4/PKG-INFO` & `git-stats-report-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.1.4
+Version: 0.2.0
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `git-stats-report-0.1.4/Pipfile` & `git-stats-report-0.2.0/Pipfile`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.4/README.md` & `git-stats-report-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.4/git_stats_report/__main__.py` & `git-stats-report-0.2.0/git_stats_report/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,14 +18,18 @@
         typer.Option("--strategy", "-st", help="Get git report since last merge"),
     ] = Strategy.FROM_DATE,
     since_n_days: Annotated[
         Optional[str],
         typer.Option("--since", "-s", help="Get git report since n days"),
     ] = None,
     *,
+    raw_format: Annotated[
+        bool,
+        typer.Option("--raw", "-r", help="Print raw output string with formatting"),
+    ] = False,
     version: Annotated[
         bool,
         typer.Option("--version", "-V", help="Shows the version of git-stats-report"),
     ] = False,
     verbose: Annotated[
         bool,
         typer.Option("--verbose", "-v", help="Print INFO logging statements"),
@@ -50,14 +54,14 @@
     if extra_verbose:
         logging.basicConfig(level=logging.DEBUG)
 
     if since_n_days and strategy is not Strategy.FROM_DATE:
         error_message = "--since is only allowed with --strategy FROM_DATE"
         raise ValueError(error_message)
 
-    run(strategy, since_n_days)
+    run(strategy, since_n_days, raw_format=raw_format)
 
     raise typer.Exit
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `git-stats-report-0.1.4/git_stats_report/git_stats.py` & `git-stats-report-0.2.0/git_stats_report/git_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,8 @@
         added, deleted, _ = line.split("\t", 2)
 
         files_changed += 1
 
         lines_added += int(added) if added.isdigit() else 0
         lines_deleted += int(deleted) if deleted.isdigit() else 0
 
-    return f"\n* {files_changed} Files Changed, - {lines_deleted} Lines Deleted, + {lines_added} Lines Added\n\n"  # pylint: disable=line-too-long
+    return f"\n* {files_changed} Files Changed, - {lines_deleted} Lines Deleted, + {lines_added} Lines Added\n"  # pylint: disable=line-too-long
```

### Comparing `git-stats-report-0.1.4/git_stats_report/strategy/__init__.py` & `git-stats-report-0.2.0/git_stats_report/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.4/git_stats_report/strategy/from_latest_tag.py` & `git-stats-report-0.2.0/git_stats_report/strategy/from_latest_tag.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.4/git_stats_report.egg-info/PKG-INFO` & `git-stats-report-0.2.0/git_stats_report.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.1.4
+Version: 0.2.0
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `git-stats-report-0.1.4/git_stats_report.egg-info/SOURCES.txt` & `git-stats-report-0.2.0/git_stats_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.4/pyproject.toml` & `git-stats-report-0.2.0/pyproject.toml`

 * *Files identical despite different names*

