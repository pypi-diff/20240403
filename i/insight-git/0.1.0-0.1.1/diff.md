# Comparing `tmp/insight-git-0.1.0.tar.gz` & `tmp/insight-git-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insight-git-0.1.0.tar", last modified: Wed Apr  3 08:48:48 2024, max compression
+gzip compressed data, was "insight-git-0.1.1.tar", last modified: Wed Apr  3 18:51:25 2024, max compression
```

## Comparing `insight-git-0.1.0.tar` & `insight-git-0.1.1.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 08:48:48.562502 insight-git-0.1.0/
--rw-rw-rw-   0        0        0     1128 2024-04-01 09:27:53.000000 insight-git-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4228 2024-04-03 08:48:48.561502 insight-git-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2418 2024-04-02 21:00:36.000000 insight-git-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 08:48:48.490772 insight-git-0.1.0/insight_git/
--rw-rw-rw-   0        0        0      365 2024-04-02 20:37:15.000000 insight-git-0.1.0/insight_git/__init__.py
--rw-rw-rw-   0        0        0      583 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/__main__.py
--rw-rw-rw-   0        0        0     4106 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/callbacks.py
--rw-rw-rw-   0        0        0     3436 2024-04-02 20:37:15.000000 insight-git-0.1.0/insight_git/layout.py
--rw-rw-rw-   0        0        0      870 2024-04-02 21:05:16.000000 insight-git-0.1.0/insight_git/plugin_loader.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:48:48.542421 insight-git-0.1.0/insight_git/plugins/
--rw-rw-rw-   0        0        0        0 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/plugins/__init__.py
--rw-rw-rw-   0        0        0     1739 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/plugins/branch_information.py
--rw-rw-rw-   0        0        0     2515 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/plugins/code_quality.py
--rw-rw-rw-   0        0        0     2672 2024-04-03 08:16:22.000000 insight-git-0.1.0/insight_git/plugins/commit_graph.py
--rw-rw-rw-   0        0        0     2942 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/plugins/commit_type.py
--rw-rw-rw-   0        0        0     4846 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/plugins/contributors_info.py
--rw-rw-rw-   0        0        0     3178 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/plugins/git_statistics.py
--rw-rw-rw-   0        0        0      703 2024-04-01 09:27:53.000000 insight-git-0.1.0/insight_git/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 08:48:48.556410 insight-git-0.1.0/insight_git.egg-info/
--rw-rw-rw-   0        0        0     4228 2024-04-03 08:48:48.000000 insight-git-0.1.0/insight_git.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      838 2024-04-03 08:48:48.000000 insight-git-0.1.0/insight_git.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 08:48:48.000000 insight-git-0.1.0/insight_git.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      457 2024-04-03 08:48:48.000000 insight-git-0.1.0/insight_git.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      315 2024-04-03 08:48:48.000000 insight-git-0.1.0/insight_git.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 08:48:48.000000 insight-git-0.1.0/insight_git.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2892 2024-04-02 21:07:44.000000 insight-git-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-03 08:48:48.562502 insight-git-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-03 08:48:48.554414 insight-git-0.1.0/tests/
--rw-rw-rw-   0        0        0     1382 2024-04-02 20:54:42.000000 insight-git-0.1.0/tests/test_branch_information.py
--rw-rw-rw-   0        0        0     1215 2024-04-02 20:54:42.000000 insight-git-0.1.0/tests/test_callbacks.py
--rw-rw-rw-   0        0        0     3245 2024-04-02 21:01:37.000000 insight-git-0.1.0/tests/test_commit_graph.py
--rw-rw-rw-   0        0        0     1868 2024-04-02 20:54:42.000000 insight-git-0.1.0/tests/test_commit_type.py
--rw-rw-rw-   0        0        0     2051 2024-04-02 20:54:42.000000 insight-git-0.1.0/tests/test_contributors.py
--rw-rw-rw-   0        0        0     1791 2024-04-02 21:01:37.000000 insight-git-0.1.0/tests/test_git_statistics.py
--rw-rw-rw-   0        0        0      727 2024-04-02 20:55:36.000000 insight-git-0.1.0/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.332921 insight-git-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-03 18:51:20.000000 insight-git-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-03 18:51:25.332921 insight-git-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 18:51:20.000000 insight-git-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.324921 insight-git-0.1.1/insight_git/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugin_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.328920 insight-git-0.1.1/insight_git/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/branch_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/commit_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/commit_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/contributors_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3092 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/plugins/git_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-03 18:51:20.000000 insight-git-0.1.1/insight_git/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.328920 insight-git-0.1.1/insight_git.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4125 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 18:51:25.000000 insight-git-0.1.1/insight_git.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-04-03 18:51:20.000000 insight-git-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:51:25.332921 insight-git-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:51:25.328920 insight-git-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_branch_information.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_commit_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_commit_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_contributors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_git_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 18:51:20.000000 insight-git-0.1.1/tests/test_main.py
```

### Comparing `insight-git-0.1.0/LICENSE.txt` & `insight-git-0.1.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-
-### LICENSE (MIT)
-
-```license
-MIT License
-
-Copyright (c) 2023 André F. Costa
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+
+### LICENSE (MIT)
+
+```license
+MIT License
+
+Copyright (c) 2023 André F. Costa
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `insight-git-0.1.0/README.md` & `insight-git-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![Tests](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml/badge.svg?branch=master)](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml)
-[![codecov](https://codecov.io/gh/andrecosta99/insight-git/branch/master/graph/badge.svg)](https://codecov.io/gh/andrecosta99/insight-git)
-[![Docs](https://img.shields.io/badge/docs-click%20here-blue.svg)](https://andrecosta99.github.io/insight-git/)
-[![PyPI version](https://badge.fury.io/py/insight-git.svg)](https://badge.fury.io/py/insight-git)
-![GitHub last commit](https://img.shields.io/github/last-commit/andrecosta99/insight-git)
-![GitHub forks](https://img.shields.io/github/forks/andrecosta99/insight-git)
-
-
-# Insight Git
-
-Insight Git is a tool designed to fetch and present comprehensive statistics from Git repositories. Whether the repository is hosted locally or on platforms like GitHub, Insight Git seamlessly analyzes commit history, contribution patterns, and other vital metrics. This utility is particularly useful for developers and teams looking to gain insights into project trends, contributor activity, and overall repository health. Built with Python and leveraging technologies such as Dash and Plotly, it provides an interactive and visually appealing interface for data representation.
-
-## Features
-
-- **Repository Analysis**: Obtain a detailed view of repository activity, including commits over time, contributions by author, and types of commits.
-- **Interactive Interface**: Explore statistics through an interactive web interface created with Dash and Plotly.
-- **Support for Local and Remote Repositories**: Works with both local Git repositories and remote repository URLs.
-
-## Installation
-
-To install Insight Git, ensure you have Python installed on your system, and run:
-
-```bash
-pip install insight-git
-```
-
-## Usage
-After installation, you can start the application by running:
-
-```bash
-insight-git
-```
-Follow the instructions in the web interface to input the path or URL of the Git repository you wish to analyze.
-
-## Contributing
-Contributions to Insight Git are welcome! If you've found a bug or have a suggestion, please open an issue on GitHub.
-
-## License
-Insight Git is licensed under the MIT License. See the LICENSE file for more details.
+
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![Tests](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml/badge.svg)](https://github.com/andrecosta99/insight-git/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/andrecosta99/insight-git/branch/master/graph/badge.svg)](https://codecov.io/gh/andrecosta99/insight-git)
+[![Docs](https://img.shields.io/badge/docs-click%20here-blue.svg)](https://andrecosta99.github.io/insight-git/)
+[![PyPI version](https://badge.fury.io/py/insight-git.svg)](https://badge.fury.io/py/insight-git)
+![GitHub last commit](https://img.shields.io/github/last-commit/andrecosta99/insight-git)
+![GitHub forks](https://img.shields.io/github/forks/andrecosta99/insight-git)
+
+
+# Insight Git
+
+Insight Git is a tool designed to fetch and present comprehensive statistics from Git repositories. Whether the repository is hosted locally or on platforms like GitHub, Insight Git seamlessly analyzes commit history, contribution patterns, and other vital metrics. This utility is particularly useful for developers and teams looking to gain insights into project trends, contributor activity, and overall repository health. Built with Python and leveraging technologies such as Dash and Plotly, it provides an interactive and visually appealing interface for data representation.
+
+## Features
+
+- **Repository Analysis**: Obtain a detailed view of repository activity, including commits over time, contributions by author, and types of commits.
+- **Interactive Interface**: Explore statistics through an interactive web interface created with Dash and Plotly.
+- **Support for Local and Remote Repositories**: Works with both local Git repositories and remote repository URLs.
+
+## Installation
+
+To install Insight Git, ensure you have Python installed on your system, and run:
+
+```bash
+pip install insight-git
+```
+
+## Usage
+After installation, you can start the application by running:
+
+```bash
+insight-git
+```
+Follow the instructions in the web interface to input the path or URL of the Git repository you wish to analyze.
+
+## Contributing
+Contributions to Insight Git are welcome! If you've found a bug or have a suggestion, please open an issue on GitHub.
+
+## License
+Insight Git is licensed under the MIT License. See the LICENSE file for more details.
```

### Comparing `insight-git-0.1.0/insight_git/__main__.py` & `insight-git-0.1.1/insight_git/__main__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from . import app
-
-
-def main():
-    """Start the Dash server with debug mode enabled and suppress callback exceptions.
-
-    This function initializes the Dash web server. It's configured to run in debug
-    mode for development purposes, allowing live updates on code changes. Additionally,
-    it suppresses callback exceptions to prevent the app from crashing due to unhandled
-    callback errors, improving the debugging experience.
-    """
-    app.run_server(debug=True)
-    app.config.suppress_callback_exceptions = True
-
-
-if __name__ == "__main__":
-    main()
+from . import app
+
+
+def main():
+    """Start the Dash server with debug mode enabled and suppress callback exceptions.
+
+    This function initializes the Dash web server. It's configured to run in debug
+    mode for development purposes, allowing live updates on code changes. Additionally,
+    it suppresses callback exceptions to prevent the app from crashing due to unhandled
+    callback errors, improving the debugging experience.
+    """
+    app.run_server(debug=True)
+    app.config.suppress_callback_exceptions = True
+
+
+if __name__ == "__main__":
+    main()
```

### Comparing `insight-git-0.1.0/insight_git/plugins/branch_information.py` & `insight-git-0.1.1/insight_git/plugins/branch_information.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-import logging
-
-from dash import html
-from git import Repo
-
-
-# Extract branches info
-def extract_branches_info(repo_path):
-    """
-    Extracts information about branches in a Git repository, including the number of commits per branch.
-
-    Args:
-        repo_path (str): Path to the local Git repository.
-
-    Returns:
-        dict: A dictionary where keys are branch names and values are the number of commits in each branch.
-        Returns a dictionary with an 'error' key if an exception occurs.
-    """
-    try:
-        repo = Repo(repo_path)
-        branches_info = {
-            branch.name: sum(1 for _ in repo.iter_commits(branch))
-            for branch in repo.branches
-        }
-        return branches_info
-    except Exception as e:
-        logging.error(f"Error extracting branches information: {e}")
-        return {"error": str(e)}
-
-
-# Display branches info
-def display_branch_information(repo_path):
-    """
-    Creates a Dash HTML component to display information about branches in a Git repository.
-
-    Args:
-        repo_path (str): Path to the local Git repository.
-
-    Returns:
-        dash.html.Div: A Dash HTML component that lists the branches and their respective commit counts.
-        Returns a Div with an error message if there's an error in extracting branch information.
-    """
-    branches_info = extract_branches_info(repo_path)
-    if "error" in branches_info:
-        return html.Div(f"Error: {branches_info['error']}")
-
-    branches_list = html.Ul(
-        [
-            html.Li(f"{branch}: {commits} commits")
-            for branch, commits in branches_info.items()
-        ]
-    )
-
-    return html.Div([html.H5("Branches"), branches_list])
+import logging
+
+from dash import html
+from git import Repo
+
+
+# Extract branches info
+def extract_branches_info(repo_path):
+    """
+    Extracts information about branches in a Git repository, including the number of commits per branch.
+
+    Args:
+        repo_path (str): Path to the local Git repository.
+
+    Returns:
+        dict: A dictionary where keys are branch names and values are the number of commits in each branch.
+        Returns a dictionary with an 'error' key if an exception occurs.
+    """
+    try:
+        repo = Repo(repo_path)
+        branches_info = {
+            branch.name: sum(1 for _ in repo.iter_commits(branch))
+            for branch in repo.branches
+        }
+        return branches_info
+    except Exception as e:
+        logging.error(f"Error extracting branches information: {e}")
+        return {"error": str(e)}
+
+
+# Display branches info
+def display_branch_information(repo_path):
+    """
+    Creates a Dash HTML component to display information about branches in a Git repository.
+
+    Args:
+        repo_path (str): Path to the local Git repository.
+
+    Returns:
+        dash.html.Div: A Dash HTML component that lists the branches and their respective commit counts.
+        Returns a Div with an error message if there's an error in extracting branch information.
+    """
+    branches_info = extract_branches_info(repo_path)
+    if "error" in branches_info:
+        return html.Div(f"Error: {branches_info['error']}")
+
+    branches_list = html.Ul(
+        [
+            html.Li(f"{branch}: {commits} commits")
+            for branch, commits in branches_info.items()
+        ]
+    )
+
+    return html.Div([html.H5("Branches"), branches_list])
```

### Comparing `insight-git-0.1.0/insight_git/plugins/commit_type.py` & `insight-git-0.1.1/insight_git/plugins/commit_type.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from collections import Counter
-
-from dash import html
-from git import Repo
-
-
-# Extract commit types
-def extract_commit_types(repo_path):
-    """
-    Extracts and counts the types of commits in a local Git repository based on commit messages.
-
-    This function iterates over all commits in the specified repository, categorizing each commit
-    according to predefined types (e.g., Bug Fix, Feature, Documentation) based on its message.
-
-    Args:
-        repo_path (str): The file system path to the local Git repository.
-
-    Returns:
-        collections.Counter: A Counter object mapping commit types to their frequencies.
-        Returns a dictionary with an 'error' key if an exception occurs.
-    """
-
-    try:
-        repo = Repo(repo_path)
-        commits = list(repo.iter_commits())
-        commit_types = Counter(
-            categorize_commit_type(commit.message) for commit in commits
-        )
-        return commit_types
-    except Exception as e:
-        return {"error": str(e)}
-
-
-# Categorize commits
-def categorize_commit_type(commit_message):
-    """
-    Categorizes a commit message into predefined types such as Bug Fix, Feature, Documentation, or Other.
-
-    This function analyzes the commit message for keywords that indicate its type.
-
-    Args:
-        commit_message (str): The commit message to categorize.
-
-    Returns:
-        str: The category of the commit based on its message.
-    """
-
-    commit_message = commit_message.lower()
-    if "fix" in commit_message or "bug" in commit_message:
-        return "Bug Fix"
-    elif "feature" in commit_message or "add" in commit_message:
-        return "Feature"
-    elif "doc" in commit_message or "readme" in commit_message:
-        return "Documentation"
-    else:
-        return "Other"
-
-
-# Display commit types
-"""
-Creates a Dash HTML component to display the distribution of commit types in a Git repository.
-
-This function first extracts and categorizes commit types, then constructs a list in HTML to display
-the count of each commit type. If an error occurs during extraction, an error message is displayed instead.
-
-Args:
-    repo_path (str): The file system path to the local Git repository.
-
-Returns:
-    dash.html.Div: A Dash HTML component containing a list of commit types and their counts.
-                   If there's an error in extracting commit types, the component will display the error message.
-"""
-
-
-def display_commit_type(repo_path):
-    commit_type = extract_commit_types(repo_path)
-    if "error" in commit_type:
-        return html.Div(f"Error: {commit_type['error']}")
-
-    commit_types_list = html.Ul(
-        [
-            html.Li(f"{commit_type}: {count}")
-            for commit_type, count in commit_type.items()
-        ]
-    )
-
-    return html.Div(
-        [html.H5("Commits"), commit_types_list], className="commit-types-container"
-    )
+from collections import Counter
+
+from dash import html
+from git import Repo
+
+
+# Extract commit types
+def extract_commit_types(repo_path):
+    """
+    Extracts and counts the types of commits in a local Git repository based on commit messages.
+
+    This function iterates over all commits in the specified repository, categorizing each commit
+    according to predefined types (e.g., Bug Fix, Feature, Documentation) based on its message.
+
+    Args:
+        repo_path (str): The file system path to the local Git repository.
+
+    Returns:
+        collections.Counter: A Counter object mapping commit types to their frequencies.
+        Returns a dictionary with an 'error' key if an exception occurs.
+    """
+
+    try:
+        repo = Repo(repo_path)
+        commits = list(repo.iter_commits())
+        commit_types = Counter(
+            categorize_commit_type(commit.message) for commit in commits
+        )
+        return commit_types
+    except Exception as e:
+        return {"error": str(e)}
+
+
+# Categorize commits
+def categorize_commit_type(commit_message):
+    """
+    Categorizes a commit message into predefined types such as Bug Fix, Feature, Documentation, or Other.
+
+    This function analyzes the commit message for keywords that indicate its type.
+
+    Args:
+        commit_message (str): The commit message to categorize.
+
+    Returns:
+        str: The category of the commit based on its message.
+    """
+
+    commit_message = commit_message.lower()
+    if "fix" in commit_message or "bug" in commit_message:
+        return "Bug Fix"
+    elif "feature" in commit_message or "add" in commit_message:
+        return "Feature"
+    elif "doc" in commit_message or "readme" in commit_message:
+        return "Documentation"
+    else:
+        return "Other"
+
+
+# Display commit types
+"""
+Creates a Dash HTML component to display the distribution of commit types in a Git repository.
+
+This function first extracts and categorizes commit types, then constructs a list in HTML to display
+the count of each commit type. If an error occurs during extraction, an error message is displayed instead.
+
+Args:
+    repo_path (str): The file system path to the local Git repository.
+
+Returns:
+    dash.html.Div: A Dash HTML component containing a list of commit types and their counts.
+                   If there's an error in extracting commit types, the component will display the error message.
+"""
+
+
+def display_commit_type(repo_path):
+    commit_type = extract_commit_types(repo_path)
+    if "error" in commit_type:
+        return html.Div(f"Error: {commit_type['error']}")
+
+    commit_types_list = html.Ul(
+        [
+            html.Li(f"{commit_type}: {count}")
+            for commit_type, count in commit_type.items()
+        ]
+    )
+
+    return html.Div(
+        [html.H5("Commits"), commit_types_list], className="commit-types-container"
+    )
```

### Comparing `insight-git-0.1.0/insight_git/plugins/contributors_info.py` & `insight-git-0.1.1/insight_git/plugins/contributors_info.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,146 +1,146 @@
-from collections import Counter
-
-import dash_bootstrap_components as dbc
-from dash import Input, Output, State, callback, dcc, html
-from dash.exceptions import PreventUpdate
-from git import Repo
-
-
-def extract_contributors(repo_path):
-    """
-    Extracts the contributors and their commit counts from a git repository.
-
-    Args:
-        repo_path: The file system path to the git repository.
-
-    Returns:
-        A Counter object with contributors' names as keys and their commit counts as values.
-        If an error occurs, returns a dict with an 'error' key and the error message.
-    """
-    try:
-        repo = Repo(repo_path)
-        commits = list(repo.iter_commits())
-        contributors = Counter(commit.author.name for commit in commits)
-        return contributors
-    except Exception as e:
-        return {"error": str(e)}
-
-
-def display_contributors_info(repo_path):
-    """
-    Generates a Dash layout component showing the contributors and their commit counts.
-
-    Args:
-        repo_path: The file system path to the git repository.
-
-    Returns:
-        A Dash HTML component with the list of contributors or an error message.
-    """
-    contributors_data = extract_contributors(repo_path)
-    if "error" in contributors_data:
-        return dbc.Alert(f"Error: {contributors_data['error']}", color="danger")
-
-    layout = html.Div(
-        [
-            dcc.Store(id="contributors-store", data=contributors_data),
-            dcc.Store(
-                id="updated-contributors-store"
-            ),  # Store to keep the updated contributors' data
-            html.H5("Contributors", className="mb-3"),
-            dbc.ListGroup(
-                id="contributors-list",
-                children=[
-                    dbc.ListGroupItem(f"{contributor}: {count}")
-                    for contributor, count in contributors_data.items()
-                ],
-                className="mb-4",
-            ),
-            dbc.Row(
-                [
-                    dbc.Col(
-                        dbc.Input(
-                            id="original-name", placeholder="Original Name or Username"
-                        ),
-                        width=4,
-                    ),
-                    dbc.Col(
-                        dbc.Input(id="unified-name", placeholder="Unified Name"),
-                        width=4,
-                    ),
-                    dbc.Col(
-                        dbc.Button(
-                            "Unify", id="unify-btn", color="success", className="me-1"
-                        ),
-                        width=4,
-                    ),
-                ]
-            ),
-        ],
-        style={"maxWidth": "720px", "margin": "0 auto"},
-    )
-
-    return layout
-
-
-@callback(
-    Output("updated-contributors-store", "data"),
-    Input("unify-btn", "n_clicks"),
-    [
-        State("contributors-store", "data"),
-        State("updated-contributors-store", "data"),
-        State("original-name", "value"),
-        State("unified-name", "value"),
-    ],
-    prevent_initial_call=True,
-)
-def update_contributors_data(
-    n_clicks, initial_data, updated_data, original_name, unified_name
-):
-    """
-    Updates the contributors' data by unifying names based on user input.
-
-    Args:
-        n_clicks: Number of times the unify button has been clicked.
-        initial_data: The initial data from the contributors-store.
-        updated_data: The potentially updated data from the updated-contributors-store.
-        original_name: The original name to be replaced.
-        unified_name: The new name that replaces the original.
-
-    Returns:
-        The updated contributors' data.
-    """
-    if not original_name or not unified_name:
-        raise PreventUpdate
-
-    contributors_data = updated_data if updated_data is not None else initial_data
-
-    if original_name in contributors_data:
-        contributors_data[unified_name] = contributors_data.get(
-            unified_name, 0
-        ) + contributors_data.pop(original_name, 0)
-
-    return contributors_data
-
-
-@callback(
-    Output("contributors-list", "children"),
-    [Input("updated-contributors-store", "data")],
-)
-def display_updated_contributors(updated_data):
-    """
-    Updates the displayed list of contributors based on the updated data.
-
-    Args:
-        updated_data: The updated contributors' data from the updated-contributors-store.
-
-    Returns:
-        A list of Dash components representing the updated contributors.
-    """
-    if updated_data is None:
-        raise PreventUpdate
-
-    updated_contributors = [
-        dbc.ListGroupItem(f"{contributor}: {count}")
-        for contributor, count in updated_data.items()
-    ]
-    return updated_contributors
+from collections import Counter
+
+import dash_bootstrap_components as dbc
+from dash import Input, Output, State, callback, dcc, html
+from dash.exceptions import PreventUpdate
+from git import Repo
+
+
+def extract_contributors(repo_path):
+    """
+    Extracts the contributors and their commit counts from a git repository.
+
+    Args:
+        repo_path: The file system path to the git repository.
+
+    Returns:
+        A Counter object with contributors' names as keys and their commit counts as values.
+        If an error occurs, returns a dict with an 'error' key and the error message.
+    """
+    try:
+        repo = Repo(repo_path)
+        commits = list(repo.iter_commits())
+        contributors = Counter(commit.author.name for commit in commits)
+        return contributors
+    except Exception as e:
+        return {"error": str(e)}
+
+
+def display_contributors_info(repo_path):
+    """
+    Generates a Dash layout component showing the contributors and their commit counts.
+
+    Args:
+        repo_path: The file system path to the git repository.
+
+    Returns:
+        A Dash HTML component with the list of contributors or an error message.
+    """
+    contributors_data = extract_contributors(repo_path)
+    if "error" in contributors_data:
+        return dbc.Alert(f"Error: {contributors_data['error']}", color="danger")
+
+    layout = html.Div(
+        [
+            dcc.Store(id="contributors-store", data=contributors_data),
+            dcc.Store(
+                id="updated-contributors-store"
+            ),  # Store to keep the updated contributors' data
+            html.H5("Contributors", className="mb-3"),
+            dbc.ListGroup(
+                id="contributors-list",
+                children=[
+                    dbc.ListGroupItem(f"{contributor}: {count}")
+                    for contributor, count in contributors_data.items()
+                ],
+                className="mb-4",
+            ),
+            dbc.Row(
+                [
+                    dbc.Col(
+                        dbc.Input(
+                            id="original-name", placeholder="Original Name or Username"
+                        ),
+                        width=4,
+                    ),
+                    dbc.Col(
+                        dbc.Input(id="unified-name", placeholder="Unified Name"),
+                        width=4,
+                    ),
+                    dbc.Col(
+                        dbc.Button(
+                            "Unify", id="unify-btn", color="success", className="me-1"
+                        ),
+                        width=4,
+                    ),
+                ]
+            ),
+        ],
+        style={"maxWidth": "720px", "margin": "0 auto"},
+    )
+
+    return layout
+
+
+@callback(
+    Output("updated-contributors-store", "data"),
+    Input("unify-btn", "n_clicks"),
+    [
+        State("contributors-store", "data"),
+        State("updated-contributors-store", "data"),
+        State("original-name", "value"),
+        State("unified-name", "value"),
+    ],
+    prevent_initial_call=True,
+)
+def update_contributors_data(
+    n_clicks, initial_data, updated_data, original_name, unified_name
+):
+    """
+    Updates the contributors' data by unifying names based on user input.
+
+    Args:
+        n_clicks: Number of times the unify button has been clicked.
+        initial_data: The initial data from the contributors-store.
+        updated_data: The potentially updated data from the updated-contributors-store.
+        original_name: The original name to be replaced.
+        unified_name: The new name that replaces the original.
+
+    Returns:
+        The updated contributors' data.
+    """
+    if not original_name or not unified_name:
+        raise PreventUpdate
+
+    contributors_data = updated_data if updated_data is not None else initial_data
+
+    if original_name in contributors_data:
+        contributors_data[unified_name] = contributors_data.get(
+            unified_name, 0
+        ) + contributors_data.pop(original_name, 0)
+
+    return contributors_data
+
+
+@callback(
+    Output("contributors-list", "children"),
+    [Input("updated-contributors-store", "data")],
+)
+def display_updated_contributors(updated_data):
+    """
+    Updates the displayed list of contributors based on the updated data.
+
+    Args:
+        updated_data: The updated contributors' data from the updated-contributors-store.
+
+    Returns:
+        A list of Dash components representing the updated contributors.
+    """
+    if updated_data is None:
+        raise PreventUpdate
+
+    updated_contributors = [
+        dbc.ListGroupItem(f"{contributor}: {count}")
+        for contributor, count in updated_data.items()
+    ]
+    return updated_contributors
```

### Comparing `insight-git-0.1.0/insight_git/plugins/git_statistics.py` & `insight-git-0.1.1/insight_git/plugins/git_statistics.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,86 +1,86 @@
-import logging
-
-from dash import html
-from git import Repo
-
-
-# Analyze Git statistics from a repository's commit history
-def extract_git_stats(repo_path):
-    """
-    Extracts comprehensive Git statistics from a repository's commit history.
-
-    This function collects data on the number of commits, commit dates, total lines added and deleted across all commits,
-    and computes the average lines changed per commit. It provides a broad view of the repository's activity and work volume.
-
-    Args:
-        repo_path (str): The file system path to the local Git repository.
-
-    Returns:
-        dict: A dictionary containing statistics about the repository including the total number of commits,
-              a list of commit dates, and the average lines changed per commit.
-              If an error occurs, returns a dictionary with an 'error' key containing the error message.
-    """
-
-    try:
-        repo = Repo(repo_path)
-        commits = list(repo.iter_commits())
-
-        # Collect commit dates
-        commit_dates = [commit.committed_datetime for commit in commits]
-
-        # Calculate total lines added and deleted
-        total_lines_added = sum(commit.stats.total["insertions"] for commit in commits)
-        total_lines_deleted = sum(commit.stats.total["deletions"] for commit in commits)
-
-        # Compute average lines changed per commit
-        average_lines_per_commit = (
-            ((total_lines_added + total_lines_deleted) / len(commits)) if commits else 0
-        )
-
-        return {
-            "total_commits": len(commits),
-            "commit_dates": commit_dates,
-            "average_lines_per_commit": average_lines_per_commit,
-        }
-
-    except Exception as e:
-        logging.error(f"Error extracting git statistics: {e}")
-        return {"error": str(e)}
-
-
-# Display Git statistics in a Dash component
-"""
-Creates a Dash HTML component displaying general Git statistics for a repository.
-
-This function uses the `extract_git_stats` function to gather statistics about a repository's commit history,
-then constructs a Dash HTML component to visually present these statistics, including the total number of commits
-and the average lines changed per commit.
-
-Args:
-    repo_path (str): The file system path to the local Git repository.
-
-Returns:
-    dash.html.Div: A Dash HTML component containing the visual representation of the repository's general statistics.
-                   If an error occurs during statistics extraction, the component will display the error message.
-"""
-
-
-def display_git_statistics(repo_path):
-    stats = extract_git_stats(repo_path)
-    if "error" in stats:
-        return html.Div(f"Error: {stats['error']}")
-
-    return html.Div(
-        [
-            html.H5("General Statistics"),
-            html.Ul(
-                [
-                    html.Li(f"Total Commits: {stats['total_commits']}"),
-                    html.Li(
-                        f"Average Lines per Commit: {stats['average_lines_per_commit']:.2f}"
-                    ),
-                ]
-            ),
-        ],
-        className="mt-4",
-    )
+import logging
+
+from dash import html
+from git import Repo
+
+
+# Analyze Git statistics from a repository's commit history
+def extract_git_stats(repo_path):
+    """
+    Extracts comprehensive Git statistics from a repository's commit history.
+
+    This function collects data on the number of commits, commit dates, total lines added and deleted across all commits,
+    and computes the average lines changed per commit. It provides a broad view of the repository's activity and work volume.
+
+    Args:
+        repo_path (str): The file system path to the local Git repository.
+
+    Returns:
+        dict: A dictionary containing statistics about the repository including the total number of commits,
+              a list of commit dates, and the average lines changed per commit.
+              If an error occurs, returns a dictionary with an 'error' key containing the error message.
+    """
+
+    try:
+        repo = Repo(repo_path)
+        commits = list(repo.iter_commits())
+
+        # Collect commit dates
+        commit_dates = [commit.committed_datetime for commit in commits]
+
+        # Calculate total lines added and deleted
+        total_lines_added = sum(commit.stats.total["insertions"] for commit in commits)
+        total_lines_deleted = sum(commit.stats.total["deletions"] for commit in commits)
+
+        # Compute average lines changed per commit
+        average_lines_per_commit = (
+            ((total_lines_added + total_lines_deleted) / len(commits)) if commits else 0
+        )
+
+        return {
+            "total_commits": len(commits),
+            "commit_dates": commit_dates,
+            "average_lines_per_commit": average_lines_per_commit,
+        }
+
+    except Exception as e:
+        logging.error(f"Error extracting git statistics: {e}")
+        return {"error": str(e)}
+
+
+# Display Git statistics in a Dash component
+"""
+Creates a Dash HTML component displaying general Git statistics for a repository.
+
+This function uses the `extract_git_stats` function to gather statistics about a repository's commit history,
+then constructs a Dash HTML component to visually present these statistics, including the total number of commits
+and the average lines changed per commit.
+
+Args:
+    repo_path (str): The file system path to the local Git repository.
+
+Returns:
+    dash.html.Div: A Dash HTML component containing the visual representation of the repository's general statistics.
+                   If an error occurs during statistics extraction, the component will display the error message.
+"""
+
+
+def display_git_statistics(repo_path):
+    stats = extract_git_stats(repo_path)
+    if "error" in stats:
+        return html.Div(f"Error: {stats['error']}")
+
+    return html.Div(
+        [
+            html.H5("General Statistics"),
+            html.Ul(
+                [
+                    html.Li(f"Total Commits: {stats['total_commits']}"),
+                    html.Li(
+                        f"Average Lines per Commit: {stats['average_lines_per_commit']:.2f}"
+                    ),
+                ]
+            ),
+        ],
+        className="mt-4",
+    )
```

### Comparing `insight-git-0.1.0/insight_git/utils.py` & `insight-git-0.1.1/insight_git/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import logging
-import shutil
-import tempfile
-
-from git import Repo
-
-
-# Clone a Git repository to a temporary directory and handle errors.
-def clone_remote_repo(url):
-    temp_dir = tempfile.mkdtemp()  # Creates temporary directory
-    try:
-        Repo.clone_from(url, temp_dir)  # Clones the repo
-        logging.info("Repository cloned successfully.")
-        return temp_dir  # Returns path to the cloned repo
-    except Exception as e:
-        logging.error(f"Cloning failed: {e}")  # Logs cloning failure
-        shutil.rmtree(
-            temp_dir, ignore_errors=True
-        )  # Removes the temporary directory on failure
-        return None  # Returns None if cloning fails
+import logging
+import shutil
+import tempfile
+
+from git import Repo
+
+
+# Clone a Git repository to a temporary directory and handle errors.
+def clone_remote_repo(url):
+    temp_dir = tempfile.mkdtemp()  # Creates temporary directory
+    try:
+        Repo.clone_from(url, temp_dir)  # Clones the repo
+        logging.info("Repository cloned successfully.")
+        return temp_dir  # Returns path to the cloned repo
+    except Exception as e:
+        logging.error(f"Cloning failed: {e}")  # Logs cloning failure
+        shutil.rmtree(
+            temp_dir, ignore_errors=True
+        )  # Removes the temporary directory on failure
+        return None  # Returns None if cloning fails
```

### Comparing `insight-git-0.1.0/insight_git.egg-info/SOURCES.txt` & `insight-git-0.1.1/insight_git.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 insight_git.egg-info/SOURCES.txt
 insight_git.egg-info/dependency_links.txt
 insight_git.egg-info/entry_points.txt
 insight_git.egg-info/requires.txt
 insight_git.egg-info/top_level.txt
 insight_git/plugins/__init__.py
 insight_git/plugins/branch_information.py
-insight_git/plugins/code_quality.py
 insight_git/plugins/commit_graph.py
 insight_git/plugins/commit_type.py
 insight_git/plugins/contributors_info.py
 insight_git/plugins/git_statistics.py
 tests/test_branch_information.py
 tests/test_callbacks.py
 tests/test_commit_graph.py
```

### Comparing `insight-git-0.1.0/pyproject.toml` & `insight-git-0.1.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,105 +1,106 @@
-[build-system]
-requires = ["setuptools>=40.6.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "insight-git"
-version = "0.1.0"
-description = "Insight Git analyzes Git repositories to present comprehensive statistics."
-authors = [{name = "André F. Costa", email = "afmcosta@gmail.com"}]
-readme = "README.md"
-requires-python = ">=3.10"
-license = {text = "MIT"}
-keywords = ["git", "analysis", "commit", "education"]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Intended Audience :: Developers",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Topic :: Software Development :: Version Control :: Git"
-]
-dependencies = [
-    "dash",
-    "GitPython",
-    "pandas",
-    "plotly",
-    "dash-bootstrap-components"
-
-]
-
-[project.scripts]
-insight-git = "insight_git.__main__:main"
-
-[project.entry-points."insight_git.plugins"]
-branch_information = "insight_git.plugins.branch_information:display_branch_information"
-commit_graph = "insight_git.plugins.commit_graph:display_commit_graph"
-contributors = "insight_git.plugins.contributors_info:display_contributors_info"
-commit_type = "insight_git.plugins.commit_type:display_commit_type"
-git_statistics = "insight_git.plugins.git_statistics:display_git_statistics"
-
-[project.optional-dependencies]
-dev = [
-    "black",
-    "flake8 >= 6.0.0",
-    "flake8-black",
-    "flake8-builtins",
-    "flake8-bugbear",
-    "flake8-comprehensions",
-    "flake8-docstrings",
-    "flake8-isort",
-    "flake8-pytest-style",
-    "flake8-simplify",
-    "Flake8-pyproject",
-    "isort",
-    "pre-commit",
-    "pytest >= 8.0",
-    "pytest-cov >= 3.0.0",
-    "mkdocs",
-    "mkdocs-material",
-    "mkdocstrings",
-]
-
-[project.urls]
-Homepage = "https://github.com/andrecosta99/insight-git"
-Documentation = "https://github.com/andrecosta99/insight-git#readme"
-Repository = "https://github.com/andrecosta99/insight-git"
-
-[tool.setuptools]
-packages = [
-    "insight_git",
-    "insight_git.plugins",
-]
-
-[tool.pytest.ini_options]
-minversion = "8.0"
-addopts = "--doctest-modules"
-testpaths = ["tests"]
-
-[tool.black]
-line-length = 88
-
-[tool.isort]
-profile = "black"
-line_length = 88
-
-[tool.flake8]
-extend-select = ["B9", "C4"]
-max-line-length = 120
-max-doc-length = 120
-ignore = [
-    "B905", "E203", "D100", "D104", "E501", "W503", "D103", "D202", "D205", "D212", "D415", "W505", "B950", "E402", "PT001", "PT004", "SIM117", "D200", "F401", "D103", "D202", "D205", "D212", "D415", "W505", "B950", "E402", "PT001", "D200", "F401", "PT004", "SIM117", "W505", "B950", "D103", "D202", "D205", "D212", "D415"
-]
-doctests = true
-exclude = [
-    ".git",
-    "__pycache__",
-    ".*cache",
-    "build",
-    "dist",
-    "env",
-    "venv",
-    ".eggs",
-    "*.egg",
-    "docs"
-]
-docstring-convention = "google"
+[build-system]
+requires = ["setuptools>=58.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+
+[project]
+name = "insight-git"
+version = "0.1.1"
+description = "Insight Git analyzes Git repositories to present comprehensive statistics."
+authors = [{name = "André F. Costa", email = "afmcosta@gmail.com"}]
+readme = "README.md"
+requires-python = ">=3.10"
+license = {text = "MIT"}
+keywords = ["git", "analysis", "commit", "education"]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Topic :: Software Development :: Version Control :: Git"
+]
+dependencies = [
+    "dash",
+    "GitPython",
+    "pandas",
+    "plotly",
+    "dash-bootstrap-components"
+
+]
+
+[project.scripts]
+insight-git = "insight_git.__main__:main"
+
+[project.entry-points."insight_git.plugins"]
+branch_information = "insight_git.plugins.branch_information:display_branch_information"
+commit_graph = "insight_git.plugins.commit_graph:display_commit_graph"
+contributors = "insight_git.plugins.contributors_info:display_contributors_info"
+commit_type = "insight_git.plugins.commit_type:display_commit_type"
+git_statistics = "insight_git.plugins.git_statistics:display_git_statistics"
+
+[project.optional-dependencies]
+dev = [
+    "black",
+    "flake8 >= 6.0.0",
+    "flake8-black",
+    "flake8-builtins",
+    "flake8-bugbear",
+    "flake8-comprehensions",
+    "flake8-docstrings",
+    "flake8-isort",
+    "flake8-pytest-style",
+    "flake8-simplify",
+    "Flake8-pyproject",
+    "isort",
+    "pre-commit",
+    "pytest >= 8.0",
+    "pytest-cov >= 3.0.0",
+    "mkdocs",
+    "mkdocs-material",
+    "mkdocstrings",
+]
+
+[project.urls]
+Homepage = "https://github.com/andrecosta99/insight-git"
+Documentation = "https://andrecosta99.github.io/insight-git/"
+Repository = "https://github.com/andrecosta99/insight-git"
+
+[tool.setuptools]
+packages = [
+    "insight_git",
+    "insight_git.plugins",
+]
+
+[tool.pytest.ini_options]
+minversion = "8.0"
+addopts = "--doctest-modules"
+testpaths = ["tests"]
+
+[tool.black]
+line-length = 88
+
+[tool.isort]
+profile = "black"
+line_length = 88
+
+[tool.flake8]
+extend-select = ["B9", "C4"]
+max-line-length = 120
+max-doc-length = 120
+ignore = [
+    "B905", "E203", "D100", "D104", "E501", "W503", "D103", "D202", "D205", "D212", "D415", "W505", "B950", "E402", "PT001", "PT004", "SIM117", "D200", "F401", "D103", "D202", "D205", "D212", "D415", "W505", "B950", "E402", "PT001", "D200", "F401", "PT004", "SIM117", "W505", "B950", "D103", "D202", "D205", "D212", "D415"
+]
+doctests = true
+exclude = [
+    ".git",
+    "__pycache__",
+    ".*cache",
+    "build",
+    "dist",
+    "env",
+    "venv",
+    ".eggs",
+    "*.egg",
+    "docs"
+]
+docstring-convention = "google"
```

### Comparing `insight-git-0.1.0/tests/test_branch_information.py` & `insight-git-0.1.1/tests/test_branch_information.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import os
-import sys
-from unittest.mock import MagicMock, patch
-
-import pytest
-
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
-
-
-from insight_git.plugins.branch_information import extract_branches_info
-
-
-@pytest.fixture
-def git_branches_mock():
-    # Mock the Repo object and its methods to simulate different branches and their commit counts.
-    with patch("insight_git.plugins.branch_information.Repo") as mock_repo:
-        mock_main_branch = MagicMock()
-        mock_develop_branch = MagicMock()
-
-        # Setting branch names
-        mock_main_branch.name = "main"
-        mock_develop_branch.name = "develop"
-
-        # Simulating commit counts for each branch
-        mock_repo.return_value.iter_commits.side_effect = [
-            list(range(10)),  # For 'main' branch
-            list(range(5)),  # For 'develop' branch
-        ]
-
-        # Assigning the mocked branches to the repo
-        mock_repo.return_value.branches = [mock_main_branch, mock_develop_branch]
-
-        yield mock_repo
-
-
-def test_extract_branches_info_success(git_branches_mock):
-    # Testing successful extraction of branches information
-    expected_output = {"main": 10, "develop": 5}
-    repo_path = "dummy/path/to/repo"
-    branches_info = extract_branches_info(repo_path)
-    assert branches_info == expected_output
+import os
+import sys
+from unittest.mock import MagicMock, patch
+
+import pytest
+
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
+
+
+from insight_git.plugins.branch_information import extract_branches_info
+
+
+@pytest.fixture
+def git_branches_mock():
+    # Mock the Repo object and its methods to simulate different branches and their commit counts.
+    with patch("insight_git.plugins.branch_information.Repo") as mock_repo:
+        mock_main_branch = MagicMock()
+        mock_develop_branch = MagicMock()
+
+        # Setting branch names
+        mock_main_branch.name = "main"
+        mock_develop_branch.name = "develop"
+
+        # Simulating commit counts for each branch
+        mock_repo.return_value.iter_commits.side_effect = [
+            list(range(10)),  # For 'main' branch
+            list(range(5)),  # For 'develop' branch
+        ]
+
+        # Assigning the mocked branches to the repo
+        mock_repo.return_value.branches = [mock_main_branch, mock_develop_branch]
+
+        yield mock_repo
+
+
+def test_extract_branches_info_success(git_branches_mock):
+    # Testing successful extraction of branches information
+    expected_output = {"main": 10, "develop": 5}
+    repo_path = "dummy/path/to/repo"
+    branches_info = extract_branches_info(repo_path)
+    assert branches_info == expected_output
```

### Comparing `insight-git-0.1.0/tests/test_commit_type.py` & `insight-git-0.1.1/tests/test_commit_type.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import os
-import sys
-from collections import Counter
-from unittest.mock import MagicMock, patch
-
-import pytest
-
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
-
-
-# Import the function under test.
-from insight_git.plugins.commit_type import extract_commit_types
-
-
-@pytest.fixture
-def git_repo_mock():
-    # Mock the Repo object and its iter_commits method to simulate a repository with a predefined set of commits.
-    with patch("insight_git.plugins.commit_type.Repo") as mock_repo:
-        # Define a series of mock commits with various commit messages to test categorization.
-        mock_repo.return_value.iter_commits.return_value = [
-            MagicMock(message="fixed a bug in the login feature"),
-            MagicMock(message="add a new feature for user profiles"),
-            MagicMock(message="updated the README with new instructions"),
-            MagicMock(message="refactored the entire codebase for clarity"),
-            MagicMock(message="fixed another bug in the login feature"),
-            MagicMock(message="new feature added for user profiles"),
-            MagicMock(message="updated the README with more new instructions"),
-            MagicMock(message="more refactoring of the entire codebase"),
-            MagicMock(message="a final bug fix in the login feature"),
-            MagicMock(message="final new feature for user profiles"),
-        ]
-        yield mock_repo
-
-
-def test_extract_commit_types_success(git_repo_mock):
-    # Test the successful extraction and categorization of commit types from the mock repository.
-    repo_path = "dummy/path/to/repo"
-    expected_output = Counter(
-        {"Bug Fix": 3, "Feature": 3, "Documentation": 2, "Other": 2}
-    )
-    commit_types = extract_commit_types(repo_path)
-    assert commit_types == expected_output
+import os
+import sys
+from collections import Counter
+from unittest.mock import MagicMock, patch
+
+import pytest
+
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
+
+
+# Import the function under test.
+from insight_git.plugins.commit_type import extract_commit_types
+
+
+@pytest.fixture
+def git_repo_mock():
+    # Mock the Repo object and its iter_commits method to simulate a repository with a predefined set of commits.
+    with patch("insight_git.plugins.commit_type.Repo") as mock_repo:
+        # Define a series of mock commits with various commit messages to test categorization.
+        mock_repo.return_value.iter_commits.return_value = [
+            MagicMock(message="fixed a bug in the login feature"),
+            MagicMock(message="add a new feature for user profiles"),
+            MagicMock(message="updated the README with new instructions"),
+            MagicMock(message="refactored the entire codebase for clarity"),
+            MagicMock(message="fixed another bug in the login feature"),
+            MagicMock(message="new feature added for user profiles"),
+            MagicMock(message="updated the README with more new instructions"),
+            MagicMock(message="more refactoring of the entire codebase"),
+            MagicMock(message="a final bug fix in the login feature"),
+            MagicMock(message="final new feature for user profiles"),
+        ]
+        yield mock_repo
+
+
+def test_extract_commit_types_success(git_repo_mock):
+    # Test the successful extraction and categorization of commit types from the mock repository.
+    repo_path = "dummy/path/to/repo"
+    expected_output = Counter(
+        {"Bug Fix": 3, "Feature": 3, "Documentation": 2, "Other": 2}
+    )
+    commit_types = extract_commit_types(repo_path)
+    assert commit_types == expected_output
```

### Comparing `insight-git-0.1.0/tests/test_contributors.py` & `insight-git-0.1.1/tests/test_contributors.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import os
-import sys
-from collections import Counter
-from unittest.mock import MagicMock, patch
-
-import pytest
-
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
-
-
-from insight_git.plugins.contributors_info import (
-    display_contributors_info,
-    extract_contributors,
-)
-
-
-@pytest.fixture
-def git_repo_mock_contributors():
-    """
-    Mock the Repo object to simulate a repository with commits from different authors.
-
-    This allows testing of contributor extraction functionality without a real repository.
-    """
-    with patch("insight_git.plugins.contributors_info.Repo") as mock_repo:
-        mock_commit_1 = MagicMock()
-        mock_commit_1.author.name = "John Doe"
-
-        mock_commit_2 = MagicMock()
-        mock_commit_2.author.name = "Jane Doe"
-
-        mock_commit_3 = MagicMock()
-        mock_commit_3.author.name = "John Doe"
-
-        # Return a simulated list of commits from iter_commits
-        mock_repo.return_value.iter_commits.return_value = [
-            mock_commit_1,
-            mock_commit_2,
-            mock_commit_3,
-        ]
-        yield mock_repo
-
-
-def test_extract_contributors_success(git_repo_mock_contributors):
-    """
-    Test the successful extraction of contributor information.
-
-    Verifies that the correct counts of commits for each contributor are extracted.
-    """
-    repo_path = "dummy/path/to/repo"
-    expected_contributors = Counter({"John Doe": 2, "Jane Doe": 1})
-    contributors = extract_contributors(repo_path)
-    assert contributors == expected_contributors
-
-
-def test_display_contributors_success(git_repo_mock_contributors):
-    """
-    Verify the successful display of contributors in a Dash component.
-
-    Checks that the component correctly reflects the contribution counts for each contributor.
-    """
-    repo_path = "dummy/path/to/repo"
-    component = display_contributors_info(repo_path)
-    assert "John Doe: 2" in str(component)
-    assert "Jane Doe: 1" in str(component)
+import os
+import sys
+from collections import Counter
+from unittest.mock import MagicMock, patch
+
+import pytest
+
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
+
+
+from insight_git.plugins.contributors_info import (
+    display_contributors_info,
+    extract_contributors,
+)
+
+
+@pytest.fixture
+def git_repo_mock_contributors():
+    """
+    Mock the Repo object to simulate a repository with commits from different authors.
+
+    This allows testing of contributor extraction functionality without a real repository.
+    """
+    with patch("insight_git.plugins.contributors_info.Repo") as mock_repo:
+        mock_commit_1 = MagicMock()
+        mock_commit_1.author.name = "John Doe"
+
+        mock_commit_2 = MagicMock()
+        mock_commit_2.author.name = "Jane Doe"
+
+        mock_commit_3 = MagicMock()
+        mock_commit_3.author.name = "John Doe"
+
+        # Return a simulated list of commits from iter_commits
+        mock_repo.return_value.iter_commits.return_value = [
+            mock_commit_1,
+            mock_commit_2,
+            mock_commit_3,
+        ]
+        yield mock_repo
+
+
+def test_extract_contributors_success(git_repo_mock_contributors):
+    """
+    Test the successful extraction of contributor information.
+
+    Verifies that the correct counts of commits for each contributor are extracted.
+    """
+    repo_path = "dummy/path/to/repo"
+    expected_contributors = Counter({"John Doe": 2, "Jane Doe": 1})
+    contributors = extract_contributors(repo_path)
+    assert contributors == expected_contributors
+
+
+def test_display_contributors_success(git_repo_mock_contributors):
+    """
+    Verify the successful display of contributors in a Dash component.
+
+    Checks that the component correctly reflects the contribution counts for each contributor.
+    """
+    repo_path = "dummy/path/to/repo"
+    component = display_contributors_info(repo_path)
+    assert "John Doe: 2" in str(component)
+    assert "Jane Doe: 1" in str(component)
```

### Comparing `insight-git-0.1.0/tests/test_git_statistics.py` & `insight-git-0.1.1/tests/test_git_statistics.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,53 @@
-import os
-import sys
-from datetime import datetime, timedelta
-from unittest.mock import MagicMock, patch
-
-import pytest
-
-sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
-
-
-from insight_git.plugins.git_statistics import display_git_statistics, extract_git_stats
-
-
-@pytest.fixture()
-def git_repo_mock():
-    """
-    Mock the Git repository for testing statistics extraction.
-
-    Yields:
-        MagicMock object: A mock of the Repo object with predefined commits and stats.
-    """
-    with patch("insight_git.plugins.git_statistics.Repo") as mock_repo:
-        mock_commit = MagicMock()
-        mock_commit.committed_datetime = datetime.now() - timedelta(days=1)
-        mock_commit.stats.total = {"insertions": 10, "deletions": 5}
-
-        mock_commit_2 = MagicMock()
-        mock_commit_2.committed_datetime = datetime.now() - timedelta(days=2)
-        mock_commit_2.stats.total = {"insertions": 20, "deletions": 10}
-
-        mock_repo.return_value.iter_commits.return_value = [mock_commit, mock_commit_2]
-        yield mock_repo
-
-
-def test_extract_git_stats_success(git_repo_mock):
-    """
-    Test successful git statistics extraction.
-    """
-    repo_path = "dummy/path/to/repo"
-    stats = extract_git_stats(repo_path)
-    assert stats["total_commits"] == 2
-    assert len(stats["commit_dates"]) == 2
-    assert stats["average_lines_per_commit"] == 22.5
-
-
-def test_display_git_statistics_success(git_repo_mock):
-    """
-    Test the successful display of git statistics in a Dash component.
-    """
-    repo_path = "dummy/path/to/repo"
-    component = display_git_statistics(repo_path)
-    assert "Total Commits: 2" in str(component)
-    assert "Average Lines per Commit: 22.50" in str(component)
+import os
+import sys
+from datetime import datetime, timedelta
+from unittest.mock import MagicMock, patch
+
+import pytest
+
+sys.path.insert(0, os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
+
+
+from insight_git.plugins.git_statistics import display_git_statistics, extract_git_stats
+
+
+@pytest.fixture()
+def git_repo_mock():
+    """
+    Mock the Git repository for testing statistics extraction.
+
+    Yields:
+        MagicMock object: A mock of the Repo object with predefined commits and stats.
+    """
+    with patch("insight_git.plugins.git_statistics.Repo") as mock_repo:
+        mock_commit = MagicMock()
+        mock_commit.committed_datetime = datetime.now() - timedelta(days=1)
+        mock_commit.stats.total = {"insertions": 10, "deletions": 5}
+
+        mock_commit_2 = MagicMock()
+        mock_commit_2.committed_datetime = datetime.now() - timedelta(days=2)
+        mock_commit_2.stats.total = {"insertions": 20, "deletions": 10}
+
+        mock_repo.return_value.iter_commits.return_value = [mock_commit, mock_commit_2]
+        yield mock_repo
+
+
+def test_extract_git_stats_success(git_repo_mock):
+    """
+    Test successful git statistics extraction.
+    """
+    repo_path = "dummy/path/to/repo"
+    stats = extract_git_stats(repo_path)
+    assert stats["total_commits"] == 2
+    assert len(stats["commit_dates"]) == 2
+    assert stats["average_lines_per_commit"] == 22.5
+
+
+def test_display_git_statistics_success(git_repo_mock):
+    """
+    Test the successful display of git statistics in a Dash component.
+    """
+    repo_path = "dummy/path/to/repo"
+    component = display_git_statistics(repo_path)
+    assert "Total Commits: 2" in str(component)
+    assert "Average Lines per Commit: 22.50" in str(component)
```

### Comparing `insight-git-0.1.0/tests/test_main.py` & `insight-git-0.1.1/tests/test_main.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from unittest.mock import patch
-
-from insight_git import __main__
-
-
-def test_main_calls_run_server_with_debug_true():
-    """
-    Test if main function starts Dash server with debug mode enabled.
-
-    This test checks whether the 'run_server' method of the 'app' object
-    is called with 'debug=True' when the 'main' function is executed.
-    It uses patching to mock the 'run_server' method and assert it's called
-    with expected arguments.
-    """
-    with patch.object(__main__.app, "run_server") as mock_run_server:
-        # Call the 'main' function
-        __main__.main()
-
-        # Assert 'run_server' was called once with 'debug=True'
-        mock_run_server.assert_called_once_with(debug=True)
+from unittest.mock import patch
+
+from insight_git import __main__
+
+
+def test_main_calls_run_server_with_debug_true():
+    """
+    Test if main function starts Dash server with debug mode enabled.
+
+    This test checks whether the 'run_server' method of the 'app' object
+    is called with 'debug=True' when the 'main' function is executed.
+    It uses patching to mock the 'run_server' method and assert it's called
+    with expected arguments.
+    """
+    with patch.object(__main__.app, "run_server") as mock_run_server:
+        # Call the 'main' function
+        __main__.main()
+
+        # Assert 'run_server' was called once with 'debug=True'
+        mock_run_server.assert_called_once_with(debug=True)
```

