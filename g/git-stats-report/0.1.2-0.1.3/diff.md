# Comparing `tmp/git-stats-report-0.1.2.tar.gz` & `tmp/git-stats-report-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-stats-report-0.1.2.tar", last modified: Wed Apr  3 00:23:16 2024, max compression
+gzip compressed data, was "git-stats-report-0.1.3.tar", last modified: Wed Apr  3 01:42:27 2024, max compression
```

## Comparing `git-stats-report-0.1.2.tar` & `git-stats-report-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:23:16.160631 git-stats-report-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 00:23:16.160631 git-stats-report-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:23:16.156631 git-stats-report-0.1.2/git_stats_report/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/git_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:23:16.160631 git-stats-report-0.1.2/git_stats_report/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/strategy/from_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/strategy/from_latest_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/strategy/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/git_stats_report/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:23:16.160631 git-stats-report-0.1.2/git_stats_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 00:23:16.000000 git-stats-report-0.1.2/git_stats_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 00:23:16.000000 git-stats-report-0.1.2/git_stats_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:23:16.000000 git-stats-report-0.1.2/git_stats_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 00:23:16.000000 git-stats-report-0.1.2/git_stats_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 00:23:16.000000 git-stats-report-0.1.2/git_stats_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 00:23:16.000000 git-stats-report-0.1.2/git_stats_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-04-03 00:23:01.000000 git-stats-report-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:23:16.160631 git-stats-report-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:42:27.091386 git-stats-report-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 01:42:27.091386 git-stats-report-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:42:27.087386 git-stats-report-0.1.3/git_stats_report/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/git_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:42:27.091386 git-stats-report-0.1.3/git_stats_report/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/strategy/from_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/strategy/from_latest_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/strategy/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/git_stats_report/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:42:27.087386 git-stats-report-0.1.3/git_stats_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-03 01:42:27.000000 git-stats-report-0.1.3/git_stats_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 01:42:27.000000 git-stats-report-0.1.3/git_stats_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:42:27.000000 git-stats-report-0.1.3/git_stats_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 01:42:27.000000 git-stats-report-0.1.3/git_stats_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 01:42:27.000000 git-stats-report-0.1.3/git_stats_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 01:42:27.000000 git-stats-report-0.1.3/git_stats_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9489 2024-04-03 01:42:18.000000 git-stats-report-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:42:27.091386 git-stats-report-0.1.3/setup.cfg
```

### Comparing `git-stats-report-0.1.2/LICENSE` & `git-stats-report-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.2/PKG-INFO` & `git-stats-report-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.1.2
+Version: 0.1.3
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `git-stats-report-0.1.2/Pipfile` & `git-stats-report-0.1.3/Pipfile`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.2/README.md` & `git-stats-report-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.2/git_stats_report/__main__.py` & `git-stats-report-0.1.3/git_stats_report/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,29 +14,35 @@
 @app.callback(invoke_without_command=True)
 def main(
     strategy: Annotated[
         Strategy,
         typer.Option("--strategy", "-st", help="Get git report since last merge"),
     ] = Strategy.FROM_DATE,
     since_n_days: Annotated[
-        Optional[str], typer.Option("--since", "-s", help="Get git report since n days")
+        Optional[str],
+        typer.Option("--since", "-s", help="Get git report since n days"),
     ] = None,
+    *,
     version: Annotated[
         bool,
         typer.Option("--version", "-V", help="Shows the version of git-stats-report"),
     ] = False,
     verbose: Annotated[
-        bool, typer.Option("--verbose", "-v", help="Print INFO logging statements")
+        bool,
+        typer.Option("--verbose", "-v", help="Print INFO logging statements"),
     ] = False,
     extra_verbose: Annotated[
-        bool, typer.Option("-vv", help="Print DEBUG logging statements")
+        bool,
+        typer.Option("-vv", help="Print DEBUG logging statements"),
     ] = False,
 ) -> None:
-    """Returns a report with all commits authors, amount of commits, percentage of total
-    , and also number of files changed, lines added and lines deleted"""
+    """
+    Returns a report with all commits authors, amount of commits, percentage of
+    total, and also number of files changed, lines added and lines deleted
+    """
 
     if version:
         typer.echo(__version__)
         raise typer.Exit
 
     if verbose:
         logging.basicConfig(level=logging.INFO)
```

### Comparing `git-stats-report-0.1.2/git_stats_report/entrypoint.py` & `git-stats-report-0.1.3/git_stats_report/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,9 +13,9 @@
 
     for author in git_stats["authors"]:
         if not author["value"]:
             continue
         author_info = get_author_info(author, since_datetime)
         percentage_of_total = (author["value"] * 100) / total_commits
         print(
-            f'{author["label"]}: {author["value"]} commits ({percentage_of_total:.2f}% of total) {author_info}\n'  # pylint: disable=line-too-long
+            f'{author["label"]}: {author["value"]} commits ({percentage_of_total:.2f}% of total) {author_info}\n',  # pylint: disable=line-too-long
         )
```

### Comparing `git-stats-report-0.1.2/git_stats_report/git_stats.py` & `git-stats-report-0.1.3/git_stats_report/git_stats.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+from contextlib import suppress
 from datetime import datetime
 from typing import List, cast
 
 from typing_extensions import TypedDict
 
 from .utils import run_command
 
@@ -15,42 +16,43 @@
 
 
 class GitStatsRawOutput(TypedDict):
     authors: List[AuthorStats]
 
 
 def get_git_stats(since: datetime) -> GitStatsRawOutput:
-    command: str = ""
-    try:
+    with suppress(Exception):
         command = f"git-stats --raw --authors --since {since}"
-    except Exception:  # noqa
-        try:
-            command = f"npx git-stats --raw --authors --since {since}"
-        except Exception as exc:  # noqa
-            msg = "Either git-stats or node.js must be installed"
-            raise Exception(msg) from exc  # noqa
-    return cast(GitStatsRawOutput, json.loads(run_command(command)))
+        return cast(GitStatsRawOutput, json.loads(run_command(command)))
+
+    with suppress(Exception):
+        command = f"npx git-stats --raw --authors --since {since}"
+        return cast(GitStatsRawOutput, json.loads(run_command(command)))
+
+    msg = "Either git-stats or npx (node) must be installed"
+    raise ValueError(msg)
 
 
 def get_total_commits(git_stats: GitStatsRawOutput) -> int:
     return sum(author["value"] for author in git_stats["authors"] if author["value"])
 
 
 def get_author_info(author: AuthorStats, since: datetime) -> str:
-    author_name: str = author["label"]
-    command: str = (
+    author_name = author["label"]
+    command = (
         f'git log --author="{author_name}" --numstat --since="{since}" --format=""'
     )
-    log: str = run_command(command)
-    files_changed: int = 0
-    lines_added: int = 0
-    lines_deleted: int = 0
+    log = run_command(command)
+    files_changed = 0
+    lines_added = 0
+    lines_deleted = 0
     for line in log.splitlines():
         if not line:
             continue
         added, deleted, _ = line.split("\t", 2)
+
         files_changed += 1
-        if added[-1] in NUM_CHARS:
-            lines_added += int(added)
-        if added[-1] in NUM_CHARS:
-            lines_deleted += int(deleted)
+
+        lines_added += int(added) if added.isdigit() else 0
+        lines_deleted += int(deleted) if deleted.isdigit() else 0
+
     return f"\n* {files_changed} Files Changed, - {lines_deleted} Lines Deleted, + {lines_added} Lines Added\n\n"  # pylint: disable=line-too-long
```

### Comparing `git-stats-report-0.1.2/git_stats_report/strategy/__init__.py` & `git-stats-report-0.1.3/git_stats_report/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.2/git_stats_report/strategy/from_latest_tag.py` & `git-stats-report-0.1.3/git_stats_report/strategy/from_latest_tag.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.2/git_stats_report.egg-info/PKG-INFO` & `git-stats-report-0.1.3/git_stats_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-stats-report
-Version: 0.1.2
+Version: 0.1.3
 Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
 Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
 Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
 Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
 Classifier: Development Status :: 4 - Beta
```

### Comparing `git-stats-report-0.1.2/git_stats_report.egg-info/SOURCES.txt` & `git-stats-report-0.1.3/git_stats_report.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.2/pyproject.toml` & `git-stats-report-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -84,29 +84,30 @@
 
 #########################
 # MyPy
 #########################
 
 [tool.mypy]
 strict = true
+disallow_untyped_defs = true
 ignore_missing_imports = true
 
 #########################
 # RUFF
 #########################
 
 [tool.ruff]
 fix = true
 preview = true
 
 [tool.ruff.lint]
 extend-select = [
     #   "D",   # pydocstyle
-    # "FBT",   # flake8-boolean-trap
-    # "COM",   # flake8-commas
+    "FBT",  # flake8-boolean-trap
+    "COM",  # flake8-commas
     "E",    # pycodestyle
     "UP",   # pyupgrade
     "BLE",  # flake8-blind-except
     "B",    # flake8-bugbear
     "A",    # flake8-builtins
     "C4",   # flake8-comprehensions
     "ICN",  # flake8-import-conventions
@@ -133,17 +134,18 @@
     "PERF", # Perflint
     "FURB", # refurb
     "RUF",  # ruff
 ]
 
 ignore = [
     "ANN401", # Dynamically typed expressions
-    "E501", # Line too long
-    "T201", # `print` found
-    "ISC001",
+    "E501",   # Line too long
+    "T201",   # `print` found
+    "ISC001", # Keep to avoid issues with formatter
+    "COM812", # Keep to avoid issues with formatter
 ]
 
 [tool.ruff.format]
 # Set Ruff to imitate Black
 quote-style = "double"
 indent-style = "space"
 skip-magic-trailing-comma = false
```

