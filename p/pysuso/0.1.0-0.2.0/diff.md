# Comparing `tmp/pysuso-0.1.0.tar.gz` & `tmp/pysuso-0.2.0.tar.gz`

## Comparing `pysuso-0.1.0.tar` & `pysuso-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pysuso-0.1.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pysuso-0.1.0/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pysuso-0.1.0/README.md
--rw-r--r--   0        0        0     3307 2020-02-02 00:00:00.000000 pysuso-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pysuso-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3110 2020-02-02 00:00:00.000000 pysuso-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pysuso-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 pysuso-0.2.0/README.md
+-rw-r--r--   0        0        0     3492 2020-02-02 00:00:00.000000 pysuso-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2723 2020-02-02 00:00:00.000000 pysuso-0.2.0/PKG-INFO
```

### Comparing `pysuso-0.1.0/.gitignore` & `pysuso-0.2.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -155,7 +155,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+.vscode/launch.json
```

### Comparing `pysuso-0.1.0/LICENSE` & `pysuso-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pysuso-0.1.0/README.md` & `pysuso-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pysuso-0.1.0/pyproject.toml` & `pysuso-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -12,33 +12,14 @@
 
 [project.urls]
 Home="https://mcneall.github.io/PySuSo/"
 Repository="https://github.com/McNeall/PySuSo"
 Documentation="https://mcneall.github.io/PySuSo/"
 pypi = "https://pypi.org/project/pysuso"
 
-[tool.pdm]
-distribution = true
-
-[tool.pdm.scripts]
-format-check = "ruff format --check --quiet"
-lint-check = "ruff check --quiet"
-type-check = "pyright"
-tests = "coverage run -m pytest"
-report = "coverage report --skip-empty --skip-covered --show-missing"
-coverage = {composite = ["tests", "report"]}
-
-[tool.pdm.dev-dependencies]
-dev = [
-    "mypy>=1.8.0",
-    "ruff>=0.3.2",
-    "pyright>=1.1.353",
-    "coverage>=7.4.4",
-]
-
 [project.optional-dependencies]
 test = [
     "pytest>=8.0.2",
 ]
 docs = [
     "mkdocs>=1.5.3",
     "mkdocs-material>=9.5.13",
@@ -66,15 +47,15 @@
   "src"
 ]
 
 [tool.ruff]
 line-length = 120
 indent-width = 4
 target-version = "py312"
-include = ["pyproject.toml", "src/**/*.py", "tests/**/*.py"]
+include = ["pyproject.toml", "src/**/*.py", "tests/**/*.py", "docs/hooks/**/*.py"]
 exclude = [
     ".bzr",
     ".direnv",
     ".eggs",
     ".git",
     ".git-rewrite",
     ".hg",
@@ -94,26 +75,26 @@
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "site-packages",
     "venv",
-    "docs",
 ]
 
 [tool.ruff.lint]
 select = ["ALL"]
 ignore = [
     "D203", # Checks for blank line between class and docstring. Incompatible with D211.
     "D213",  # docstring summary on second line of docstring.
     "COM812", # Conflicts with formatter.
     "ISC001",
     "ANN101", # Deprecated
-    "ANN102" # Deprecated
+    "ANN102", # Deprecated
+    "N818" # Rule seems to give false positives for Exceptions that do not have Error as suffix.
 ]
 fixable = ["ALL"]
 unfixable = [
     "F401" # Do not autofix unused imports.
 ]
 extend-safe-fixes = [
     "D400" # Add periods at end of docstring summary.
@@ -147,7 +128,27 @@
 method = "git"
 match = ["v*"]
 default-tag= "0.1.0"
 
 
 [tool.versioningit.tag2version]
 method = "basic"
+
+[tool.pdm]
+distribution = true
+
+[tool.pdm.scripts]
+format-check = "ruff format --check --quiet"
+lint-check = "ruff check --quiet"
+type-check = "pyright"
+tests = "coverage run -m pytest"
+coverage-summary = "coverage report --skip-empty --skip-covered --show-missing"
+coverage-xml = "coverage xml -q --data-file=.coverage -o coverage.xml"
+coverage-report = {composite = ["tests", "coverage-xml"]}
+
+[tool.pdm.dev-dependencies]
+dev = [
+    "ruff>=0.3.2",
+    "pyright>=1.1.353",
+    "coverage>=7.4.4",
+]
+
```

### Comparing `pysuso-0.1.0/PKG-INFO` & `pysuso-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pysuso
-Version: 0.1.0
+Version: 0.2.0
 Summary: Sudoku sovler written in Python
 Project-URL: Home, https://mcneall.github.io/PySuSo/
 Project-URL: Repository, https://github.com/McNeall/PySuSo
 Project-URL: Documentation, https://mcneall.github.io/PySuSo/
 Project-URL: pypi, https://pypi.org/project/pysuso
 Author-email: Robert Schmidt <allthingscoding21th@gmail.com>
 License: MIT
```

