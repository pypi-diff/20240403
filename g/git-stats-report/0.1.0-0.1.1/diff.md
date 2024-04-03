# Comparing `tmp/git-stats-report-0.1.0.tar.gz` & `tmp/git-stats-report-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git-stats-report-0.1.0.tar", last modified: Tue Apr  2 18:50:37 2024, max compression
+gzip compressed data, was "git-stats-report-0.1.1.tar", last modified: Tue Apr  2 23:49:16 2024, max compression
```

## Comparing `git-stats-report-0.1.0.tar` & `git-stats-report-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:50:37.952616 git-stats-report-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-02 18:50:37.952616 git-stats-report-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (127)     6084 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:50:37.948616 git-stats-report-0.1.0/git_report/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/git_stats.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:50:37.948616 git-stats-report-0.1.0/git_report/strategy/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/strategy/from_date.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/strategy/from_latest_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/strategy/strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/git_report/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:50:37.952616 git-stats-report-0.1.0/git_stats_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-02 18:50:37.000000 git-stats-report-0.1.0/git_stats_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 18:50:37.000000 git-stats-report-0.1.0/git_stats_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:50:37.000000 git-stats-report-0.1.0/git_stats_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 18:50:37.000000 git-stats-report-0.1.0/git_stats_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 18:50:37.000000 git-stats-report-0.1.0/git_stats_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 18:50:37.000000 git-stats-report-0.1.0/git_stats_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9485 2024-04-02 18:50:24.000000 git-stats-report-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:50:37.952616 git-stats-report-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:16.030655 git-stats-report-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-02 23:49:16.030655 git-stats-report-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:16.026656 git-stats-report-0.1.1/git_stats_report/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/git_stats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:16.030655 git-stats-report-0.1.1/git_stats_report/strategy/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/strategy/from_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/strategy/from_latest_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/strategy/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/git_stats_report/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 23:49:16.026656 git-stats-report-0.1.1/git_stats_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-02 23:49:16.000000 git-stats-report-0.1.1/git_stats_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-02 23:49:16.000000 git-stats-report-0.1.1/git_stats_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 23:49:16.000000 git-stats-report-0.1.1/git_stats_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 23:49:16.000000 git-stats-report-0.1.1/git_stats_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-02 23:49:16.000000 git-stats-report-0.1.1/git_stats_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 23:49:16.000000 git-stats-report-0.1.1/git_stats_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9372 2024-04-02 23:49:06.000000 git-stats-report-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 23:49:16.030655 git-stats-report-0.1.1/setup.cfg
```

### Comparing `git-stats-report-0.1.0/LICENSE` & `git-stats-report-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.0/Pipfile` & `git-stats-report-0.1.1/Pipfile`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.0/README.md` & `git-stats-report-0.1.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,84 +1,81 @@
-# git-report
+Metadata-Version: 2.1
+Name: git-stats-report
+Version: 0.1.1
+Author-email: Juan José Farina <juanjosefarina.jjf@gmail.com>, "Ezequiel L. Castaño" <castanoezequielleonardo@gmail.com>
+License: MIT
+Project-URL: homepage, https://github.com/JuanJFarina/git-stats-report
+Project-URL: documentation, https://github.com/JuanJFarina/git-stats-report
+Project-URL: repository, https://github.com/JuanJFarina/git-stats-report
+Project-URL: changelog, https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Classifier: Framework :: Pytest
+Classifier: Environment :: Console
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Software Development :: Version Control :: Git
+Classifier: Typing :: Typed
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: typer==0.9.0
+Requires-Dist: typing-extensions==4.10.0
 
-| PyPI    | [![PyPI Downloads](https://img.shields.io/pypi/dm/git-report?style=for-the-badge&label=Installations&color=steelblue&logo=pypi)](https://pypistats.org/packages/git-report) [![PyPI Version](https://img.shields.io/pypi/v/git-report?style=for-the-badge&logo=pypi)](https://pypi.org/project/git-report/) ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/elc/git-report/test.yml?style=for-the-badge&logo=githubactions&label=CICD) <br> ![Unreleased Commits](https://img.shields.io/github/commits-difference/elc/git-report?base=develop&head=master&style=for-the-badge&logo=git&label=Unreleased%20Commits) ![Last Released date](https://img.shields.io/github/last-commit/elc/git-report/master?style=for-the-badge&logo=git&label=Last%20Released%20on) 	|
+# git-stats-report
+
+| PyPI    | [![PyPI Downloads](https://img.shields.io/pypi/dm/git-stats-report?style=for-the-badge&label=Installations&color=steelblue&logo=pypi)](https://pypistats.org/packages/git-stats-report) [![PyPI Version](https://img.shields.io/pypi/v/git-stats-report?style=for-the-badge&logo=pypi)](https://pypi.org/project/git-stats-report/) ![GitHub Workflow Status (with event)](https://img.shields.io/github/actions/workflow/status/juanjfarina/git-stats-report/test.yml?style=for-the-badge&logo=githubactions&label=CICD) <br> ![Unreleased Commits](https://img.shields.io/github/commits-difference/juanjfarina/git-stats-report?base=develop&head=master&style=for-the-badge&logo=git&label=Unreleased%20Commits) ![Last Released date](https://img.shields.io/github/last-commit/juanjfarina/git-stats-report/master?style=for-the-badge&logo=git&label=Last%20Released%20on) 	|
 |---------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------	|
-| Quality | [![Coveralls branch](https://img.shields.io/coverallsCoverage/github/ELC/git-report?branch=master&style=for-the-badge&logo=coveralls)](https://coveralls.io/github/ELC/git-report) [![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability/ELC/git-report?style=for-the-badge&logo=codeclimate)](https://codeclimate.com/github/ELC/git-report) [![Code Climate technical debt](https://img.shields.io/codeclimate/tech-debt/ELC/git-report?style=for-the-badge&logo=codeclimate)](https://codeclimate.com/github/ELC/git-report) <br> ![OSSF-Scorecard Score](https://img.shields.io/ossf-scorecard/github.com/ELC/git-report?style=for-the-badge&label=OpenSSF%20Score) [![Dependabot](https://img.shields.io/badge/Dependabot-Enabled-brightgreen?style=for-the-badge&logo=dependabot)](https://github.com/ELC/git-report/blob/master/.github/dependabot.yml)                                                                                                           	|
+| Quality | [![Coveralls branch](https://img.shields.io/coverallsCoverage/github/JuanJFarina/git-stats-report?branch=master&style=for-the-badge&logo=coveralls)](https://coveralls.io/github/JuanJFarina/git-stats-report) [![Code Climate maintainability](https://img.shields.io/codeclimate/maintainability/JuanJFarina/git-stats-report?style=for-the-badge&logo=codeclimate)](https://codeclimate.com/github/JuanJFarina/git-stats-report) [![Code Climate technical debt](https://img.shields.io/codeclimate/tech-debt/JuanJFarina/git-stats-report?style=for-the-badge&logo=codeclimate)](https://codeclimate.com/github/JuanJFarina/git-stats-report) <br> ![OSSF-Scorecard Score](https://img.shields.io/ossf-scorecard/github.com/JuanJFarina/git-stats-report?style=for-the-badge&label=OpenSSF%20Score) [![Dependabot](https://img.shields.io/badge/Dependabot-Enabled-brightgreen?style=for-the-badge&logo=dependabot)](https://github.com/JuanJFarina/git-stats-report/blob/master/.github/dependabot.yml)                                                                                                           	|
 | Format  | ![Conventional Commits](https://img.shields.io/badge/semantic--release-conventional-steelblue?logo=semantic-release&style=for-the-badge) ![Commitlint](https://img.shields.io/badge/commitlint-%E2%9C%93-brightgreen?logo=commitlint&style=for-the-badge) <br> ![Pre Commit](https://img.shields.io/badge/Pre--Commit-%E2%9C%93-brightgreen?style=for-the-badge&logo=precommit) ![Format](https://img.shields.io/badge/Format-Ruff-brightgreen?style=for-the-badge&color=black) ![Linting](https://img.shields.io/endpoint?url=https%3A%2F%2Fraw.githubusercontent.com%2Fcharliermarsh%2Fruff%2Fmain%2Fassets%2Fbadge%2Fv2.json&style=for-the-badge&label=Linting)                                                                                                                                	|
-| Legal   | [![FOSSA Status](https://img.shields.io/badge/LICENSE%20SCAN-PASSING-CD2956?style=for-the-badge&logo=fossa)](https://app.fossa.com/projects/git%2Bgithub.com%2FELC%2Fgit-report) [![PyPI - License](https://img.shields.io/pypi/l/git-report?style=for-the-badge&logo=opensourceinitiative)](./LICENSE) ![Commercial Use](https://img.shields.io/badge/Comercial_Use-%E2%9C%93-brightgreen?style=for-the-badge)                                                                                                                                                                                                                                                                                                                                                                                  	|
+| Legal   | [![FOSSA Status](https://img.shields.io/badge/LICENSE%20SCAN-PASSING-CD2956?style=for-the-badge&logo=fossa)](https://app.fossa.com/projects/git%2Bgithub.com%2FJuanJFarina%2Fgit-stats-report) [![PyPI - License](https://img.shields.io/pypi/l/git-stats-report?style=for-the-badge&logo=opensourceinitiative)](./LICENSE) ![Commercial Use](https://img.shields.io/badge/Comercial_Use-%E2%9C%93-brightgreen?style=for-the-badge)                                                                                                                                                                                                                                                                                                                                                                                  	|
 
-💢🔍 breaking change detection in Python - Compatible with Semantic Version and Semantic Release
+🔍 Git Stats Reports 🔍
 
 ## Usage
 
 Use the --help flag for detailed options:
 
 ```shell
-git-report --help
-```
-
-git-report can be used in different ways, the most straightforward one is:
-
-```shell
-git-report --paths "tests" --target-version "<to-be-release-version>" --test-command "pytest tests"
-```
-
-The `test-command` could be any command and does not need to be Python specific
-
-### Combine with scripts
-
-It is also possible to simplify the `test-command` by always using something like `pipenv scripts` or `npm scripts`
-
-So in the `project.json` / `Pipfile`, one could define the test command and use git-report with `npm run test` or `pipenv run test` instead:
-
-```shell
-git-report --paths "tests" --target-version "<to-be-release-version>" --test-command "pipenv run test"
-```
-
-```shell
-git-report --paths "tests" --target-version "<to-be-release-version>" --test-command "npm run test"
+git-stats-report --help
 ```
 
-
-## Semantic Release
-
-If using the Python-Semantic-Release module, installable with:
+git-stats-report can be used in different ways, the most straightforward one is:
 
 ```shell
-pipx install python-semantic-release
+git-stats-report
 ```
 
-One can integrate it with git-report by using:
-
-```shell
-git-report -t "$(semantic-release -v version --print)"
-```
+This will return statistics for each contributor since the last merge commit
 
 ## Installation
 
 
 ### With Pipx
 
 Recommended instalation for CICD is through `pipx` with a pinned version:
 
 ```shell
 pip install pipx==1.2.0
-pipx run git-report==0.18.0 --paths "tests" --target-version "<to-be-release-version>" --test-command "pytest tests"
+pipx run git-stats-report==0.2.0
 ```
 
-That command will create a virtual environment just for git-report and run the test command from there.
+That command will create a virtual environment just for git-stats-report and return the
+report.
 
 ### With pip
 
 Instalation can be done with pip as usual:
 
 ```shell
-pip install git-report
+pip install git-stats-report
 ```
 
 Pipenv and poetry equivalents can be used as well.
 
 ## F.A.Q.
 
 ## License
 
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FELC%2Fgit-report.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FELC%2Fgit-report)
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FJuanJFarina%2Fgit-stats-report.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FJuanJFarina%2Fgit-stats-report)
```

### Comparing `git-stats-report-0.1.0/git_report/__main__.py` & `git-stats-report-0.1.1/git_stats_report/__main__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.0/git_report/entrypoint.py` & `git-stats-report-0.1.1/git_stats_report/entrypoint.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,12 +8,14 @@
     datetime_factory = get_datetime_factory_from_strategy(strategy)
     since_datetime = datetime_factory(since)
 
     git_stats = get_git_stats(since_datetime)
     total_commits = get_total_commits(git_stats)
 
     for author in git_stats["authors"]:
+        if not author["value"]:
+            continue
         author_info = get_author_info(author, since_datetime)
         percentage_of_total = (author["value"] * 100) / total_commits
         print(
             f'{author["label"]}: {author["value"]} commits ({percentage_of_total:.2f}% of total) {author_info}\n'  # pylint: disable=line-too-long
         )
```

### Comparing `git-stats-report-0.1.0/git_report/git_stats.py` & `git-stats-report-0.1.1/git_stats_report/git_stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 class GitStatsRawOutput(TypedDict):
     authors: List[AuthorStats]
 
 
 def get_git_stats(since: datetime) -> GitStatsRawOutput:
-    command: str = f"git-stats --raw --authors --since {since}"
+    command: str = f"npx git-stats --raw --authors --since {since}"
     return cast(GitStatsRawOutput, json.loads(run_command(command)))
 
 
 def get_total_commits(git_stats: GitStatsRawOutput) -> int:
     return sum(author["value"] for author in git_stats["authors"])
```

### Comparing `git-stats-report-0.1.0/git_report/strategy/__init__.py` & `git-stats-report-0.1.1/git_stats_report/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `git-stats-report-0.1.0/git_report/strategy/from_latest_tag.py` & `git-stats-report-0.1.1/git_stats_report/strategy/from_latest_tag.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any
 
-from git_report.utils import run_command
+from git_stats_report.utils import run_command
 
 
 def get_latest_tag() -> str:
     command = "git describe --tags --abbrev=0"
     try:
         return run_command(command)
     except Exception as ex:  # noqa: BLE001
```

### Comparing `git-stats-report-0.1.0/pyproject.toml` & `git-stats-report-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -16,43 +16,40 @@
 requires-python = ">=3.8"
 dynamic = ['version', 'readme']
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python",
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
-    "Framework :: Hypothesis",
     "Framework :: Pytest",
     "Environment :: Console",
     "Natural Language :: English",
     "Operating System :: OS Independent",
-    "Topic :: Software Development :: Quality Assurance",
-    "Topic :: Software Development :: Testing",
     "Topic :: Software Development :: Version Control :: Git",
     "Typing :: Typed",
 ]
 
 [project.urls]
 homepage = "https://github.com/JuanJFarina/git-stats-report"
 documentation = "https://github.com/JuanJFarina/git-stats-report"
 repository = "https://github.com/JuanJFarina/git-stats-report"
 changelog = "https://github.com/JuanJFarina/git-stats-report/blob/master/CHANGELOG.md"
 
 [project.scripts]
-git_report = "git_report.__main__:app"
+git_stats_report = "git_stats_report.__main__:app"
 
 #########################
 # Setuptools
 #########################
 
 [tool.setuptools.package-data]
 "*" = ["py.typed", "*.md"]
 
 [tool.setuptools.dynamic]
-version = { attr = "git_report.__version__" }
+version = { attr = "git_stats_report.__version__" }
 readme = { file = ["README.md"], content-type = "text/markdown" }
 
 #########################
 # Setuptools-Pipfile
 #########################
 
 [tool.setuptools-pipfile]
@@ -63,15 +60,15 @@
 
 [tool.semantic_release.branches.main]
 match = "(main|develop)"
 
 [tool.semantic_release]
 commit_message = "chore(release): bump version and update changelog"
 version_source = "tag"
-version_variables = ["git_report/__init__.py:__version__"]
+version_variables = ["git_stats_report/__init__.py:__version__"]
 
 [tool.semantic_release.changelog]
 changelog_file = "CHANGELOG.md"
 exclude_commit_patterns = ["chore*", "Merge*"]
 
 [tool.semantic_release.commit_parser_options]
 allowed_tags = ["chore", "feat", "fix"]
```

