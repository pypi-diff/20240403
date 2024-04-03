# Comparing `tmp/django_twc_toolbox-0.3.0.tar.gz` & `tmp/django_twc_toolbox-0.3.1.tar.gz`

## Comparing `django_twc_toolbox-0.3.0.tar` & `django_twc_toolbox-0.3.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/RELEASING.md
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/noxfile.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/.vscode/extensions.json
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/.vscode/settings.json.example
--rw-r--r--   0        0        0     3663 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/docs/conf.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/docs/index.md
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/docs/requirements.in
--rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/docs/development/just.md
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/src/django_twc_toolbox/__init__.py
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/src/django_twc_toolbox/apps.py
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/src/django_twc_toolbox/models.py
--rw-r--r--   0        0        0    10715 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/src/django_twc_toolbox/paginator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/tests/settings.py
--rw-r--r--   0        0        0    30152 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/tests/test_paginator.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/tests/test_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/tests/dummy/__init__.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/tests/dummy/models.py
--rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/.gitignore
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/AUTHORS.md
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/LICENSE
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/README.md
--rw-r--r--   0        0        0     5102 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     3741 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/RELEASING.md
+-rw-r--r--   0        0        0     3010 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/noxfile.py
+-rw-r--r--   0        0        0     3707 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/docs/conf.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/docs/index.md
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/docs/_static/css/custom.css
+-rw-r--r--   0        0        0     1267 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/docs/development/just.md
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/__init__.py
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/apps.py
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/models.py
+-rw-r--r--   0        0        0    10715 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/paginator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/src/django_twc_toolbox/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/settings.py
+-rw-r--r--   0        0        0    30152 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/test_paginator.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/test_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/dummy/__init__.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/tests/dummy/models.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/.gitignore
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/AUTHORS.md
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/README.md
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4599 2020-02-02 00:00:00.000000 django_twc_toolbox-0.3.1/PKG-INFO
```

### Comparing `django_twc_toolbox-0.3.0/CHANGELOG.md` & `django_twc_toolbox-0.3.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,61 +14,71 @@
 ### Fixed - for any bug fixes
 ### Security - in case of vulnerabilities
 [${version}]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v${version}
 -->
 
 ## [Unreleased]
 
+## [0.3.1]
+
+### Added
+
+-   `py.typed` added to the project.
+
+### Changed
+
+-   Now using v2024.27 of `django-twc-package`.
+
 ## [0.3.0]
 
 ### Added
 
-- Added the `page_date_range` argument to the `DatePaginator`, taking the place of the existing `date_range` argument. This change clarifies that it represents constraining the range of dates for each page, not the entire range of dates for the paginator.
+-   Added the `page_date_range` argument to the `DatePaginator`, taking the place of the existing `date_range` argument. This change clarifies that it represents constraining the range of dates for each page, not the entire range of dates for the paginator.
 
 ### Changed
 
-- Updated the `DatePaginator` class to use the `page_date_range` argument instead of the deprecated `date_range` argument.
-- `DatePage.min_date`, `DatePage.max_date`, and `DatePage.date_range` are now `cached_property` attributes instead of being set in the `__init__` method.
-- Now using [`django-twc-package`](https://github.com/westerveltco/django-twc-package) template for repository and package structure.
+-   Updated the `DatePaginator` class to use the `page_date_range` argument instead of the deprecated `date_range` argument.
+-   `DatePage.min_date`, `DatePage.max_date`, and `DatePage.date_range` are now `cached_property` attributes instead of being set in the `__init__` method.
+-   Now using [`django-twc-package`](https://github.com/westerveltco/django-twc-package) template for repository and package structure.
 
 ### Deprecated
 
-- The `date_range` argument of the `DatePaginator` class is now deprecated. It will be removed in version 0.4.0.
+-   The `date_range` argument of the `DatePaginator` class is now deprecated. It will be removed in version 0.4.0.
 
 ### Removed
 
-- Removed the `orphans` kwarg from `DatePaginator`, which is inherited from Django's built-in `Paginator`. Given its date range-based pagination, the concept of orphans, applicable to item count per page, is not super useful. If it is passed in, a warning will be issued.
+-   Removed the `orphans` kwarg from `DatePaginator`, which is inherited from Django's built-in `Paginator`. Given its date range-based pagination, the concept of orphans, applicable to item count per page, is not super useful. If it is passed in, a warning will be issued.
 
 ## [0.2.1]
 
 ### Fixed
 
-- `DatePage.min_date` and `DatePage.max_date` now return the correct dates for the page. `DatePage.min_date` returns the oldest date and `DatePage.max_date` returns the newest date.
-- `DatePage.date_range` now returns the correct range of dates for the page.
+-   `DatePage.min_date` and `DatePage.max_date` now return the correct dates for the page. `DatePage.min_date` returns the oldest date and `DatePage.max_date` returns the newest date.
+-   `DatePage.date_range` now returns the correct range of dates for the page.
 
 ## [0.2.0]
 
 ### Added
 
-- `DatePaginator` and `DatePage` classes, extending Django's built-in `Paginator` and `Page` classes, respectively. These new classes enable pagination based on a specified date field, making it easier to work with date-based data. Useful for applications that require handling of time-series data or chronological records, such as a blog or an event archive.
+-   `DatePaginator` and `DatePage` classes, extending Django's built-in `Paginator` and `Page` classes, respectively. These new classes enable pagination based on a specified date field, making it easier to work with date-based data. Useful for applications that require handling of time-series data or chronological records, such as a blog or an event archive.
 
 ## [0.1.1]
 
 Initial release!
 
 ### Added
 
-- Initial documentation.
-- Initial tests.
-- Initial CI/CD (GitHub Actions).
-- A `TimeStamped` abstract model for adding `created_at` and `updated_at` fields to models.
+-   Initial documentation.
+-   Initial tests.
+-   Initial CI/CD (GitHub Actions).
+-   A `TimeStamped` abstract model for adding `created_at` and `updated_at` fields to models.
 
 ### New Contributors
 
-- Josh Thomas <josh@joshthomas.dev> (maintainer)
+-   Josh Thomas <josh@joshthomas.dev> (maintainer)
 
-[unreleased]: https://github.com/westerveltco/django-twc-toolbox.git/compare/v0.3.0...HEAD
+[unreleased]: https://github.com/westerveltco/django-twc-toolbox/compare/v0.3.1...HEAD
 [0.2.1]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.2.1
 [0.2.0]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.2.0
 [0.1.1]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.1.1
-
 [0.3.0]: https://github.com/westerveltco/django-twc-toolbox.git/releases/tag/v0.3.0
+[0.3.1]: https://github.com/westerveltco/django-twc-toolbox/releases/tag/v0.3.1
```

### Comparing `django_twc_toolbox-0.3.0/CONTRIBUTING.md` & `django_twc_toolbox-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/RELEASING.md` & `django_twc_toolbox-0.3.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/noxfile.py` & `django_twc_toolbox-0.3.1/noxfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
 
 import nox
 
+nox.options.default_venv_backend = "uv|virtualenv"
+nox.options.reuse_existing_virtualenvs = True
+
 PY38 = "3.8"
 PY39 = "3.9"
 PY310 = "3.10"
 PY311 = "3.11"
 PY312 = "3.12"
 PY_VERSIONS = [PY38, PY39, PY310, PY311, PY312]
 PY_DEFAULT = PY_VERSIONS[0]
@@ -60,27 +63,29 @@
         (python, django)
         for python in PY_VERSIONS
         for django in DJ_VERSIONS
         if not should_skip(python, django)
     ],
 )
 def tests(session, django):
-    session.install(".[dev]")
+    session.install("django-twc-toolbox[dev] @ .")
 
     if django == DJMAIN:
-        session.install("https://github.com/django/django/archive/refs/heads/main.zip")
+        session.install(
+            "django @ https://github.com/django/django/archive/refs/heads/main.zip"
+        )
     else:
         session.install(f"django=={django}")
 
     session.run("python", "-m", "pytest")
 
 
 @nox.session
 def coverage(session):
-    session.install(".[dev]")
+    session.install("django-twc-toolbox[dev] @ .")
     session.run("python", "-m", "pytest", "--cov=django_twc_toolbox")
 
     try:
         summary = os.environ["GITHUB_STEP_SUMMARY"]
         with Path(summary).open("a") as output_buffer:
             output_buffer.write("")
             output_buffer.write("### Coverage\n\n")
@@ -101,15 +106,15 @@
         )
 
     session.run("python", "-m", "coverage", "report")
 
 
 @nox.session
 def lint(session):
-    session.install(".[lint]")
+    session.install("django-twc-toolbox[lint] @ .")
     session.run("python", "-m", "pre_commit", "run", "--all-files")
 
 
 @nox.session
 def mypy(session):
-    session.install(".[dev]")
+    session.install("django-twc-toolbox[dev] @ .")
     session.run("python", "-m", "mypy", ".")
```

### Comparing `django_twc_toolbox-0.3.0/docs/conf.py` & `django_twc_toolbox-0.3.1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,18 @@
 html_theme = "furo"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
+html_css_files = [
+    "css/custom.css",
+]
+
 html_title = project
 
 html_theme_options = {
     "footer_icons": [
         {
             "name": "GitHub",
             "url": "https://github.com/westerveltco/django-twc-toolbox",
```

### Comparing `django_twc_toolbox-0.3.0/docs/development/just.md` & `django_twc_toolbox-0.3.1/docs/development/just.md`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/src/django_twc_toolbox/models.py` & `django_twc_toolbox-0.3.1/src/django_twc_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/src/django_twc_toolbox/paginator.py` & `django_twc_toolbox-0.3.1/src/django_twc_toolbox/paginator.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/tests/settings.py` & `django_twc_toolbox-0.3.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/tests/test_paginator.py` & `django_twc_toolbox-0.3.1/tests/test_paginator.py`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/.gitignore` & `django_twc_toolbox-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/LICENSE` & `django_twc_toolbox-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/README.md` & `django_twc_toolbox-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `django_twc_toolbox-0.3.0/pyproject.toml` & `django_twc_toolbox-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   "coverage[toml]",
   "django-stubs",
   "django-stubs-ext",
   "faker",
   "hatch",
   "mypy",
   "model-bakery",
-  "nox",
+  "nox[uv]",
   "pytest",
   "pytest-cov",
   "pytest-django",
   "pytest-randomly",
   "pytest-reverse",
   "pytest-xdist"
 ]
@@ -70,15 +70,15 @@
 Documentation = "https://django-twc-toolbox.westervelt.dev/"
 Issues = "https://github.com/westerveltco/django-twc-toolbox/issues"
 Source = "https://github.com/westerveltco/django-twc-toolbox"
 
 [tool.bumpver]
 commit = true
 commit_message = ":bookmark: bump version {old_version} -> {new_version}"
-current_version = "0.3.0"
+current_version = "0.3.1"
 push = false  # set to false for CI
 tag = false
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 
 [tool.bumpver.file_patterns]
 ".copier/package.yml" = [
   'current_version: {version}'
@@ -158,16 +158,14 @@
 django_find_project = false
 norecursedirs = ".* bin build dist *.egg htmlcov logs node_modules templates venv"
 python_files = "tests.py test_*.py *_tests.py"
 pythonpath = "src"
 testpaths = ["tests"]
 
 [tool.ruff]
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 # Exclude a variety of commonly ignored directories.
 exclude = [
   ".bzr",
   ".direnv",
   ".eggs",
   ".git",
   ".github",
@@ -182,44 +180,48 @@
   "build",
   "dist",
   "migrations",
   "node_modules",
   "venv"
 ]
 extend-include = ["*.pyi?"]
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F", "I"]
-ignore = ["E501", "E741"]  # temporary
 indent-width = 4
 # Same as Black.
 line-length = 88
-select = [
-  "B",  # flake8-bugbear
-  "E",  # Pycodestyle
-  "F",  # Pyflakes
-  "I",  # isort
-  "UP"  # pyupgrade
-]
-# Assume Python >3.8.
+# Assume Python >3.8
 target-version = "py38"
-unfixable = []
 
 [tool.ruff.format]
 # Like Black, indent with spaces, rather than tabs.
 indent-style = "space"
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 # Like Black, use double quotes for strings.
 quote-style = "double"
 
-[tool.ruff.isort]
+[tool.ruff.lint]
+# Allow unused variables when underscore-prefixed.
+dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
+# Allow autofix for all enabled rules (when `--fix`) is provided.
+fixable = ["A", "B", "C", "D", "E", "F", "I"]
+ignore = ["E501", "E741"]  # temporary
+select = [
+  "B",  # flake8-bugbear
+  "E",  # Pycodestyle
+  "F",  # Pyflakes
+  "I",  # isort
+  "UP"  # pyupgrade
+]
+unfixable = []
+
+[tool.ruff.lint.isort]
 force-single-line = true
 known-first-party = ["django_twc_toolbox"]
 required-imports = ["from __future__ import annotations"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
-[tool.ruff.pyupgrade]
+[tool.ruff.lint.pyupgrade]
 # Preserve types, even if a file imports `from __future__ import annotations`.
 keep-runtime-typing = true
```

### Comparing `django_twc_toolbox-0.3.0/PKG-INFO` & `django_twc_toolbox-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: django-twc-toolbox
-Version: 0.3.0
+Version: 0.3.1
 Summary: Various tools for Django projects at The Westervelt Company.
 Project-URL: Documentation, https://django-twc-toolbox.westervelt.dev/
 Project-URL: Issues, https://github.com/westerveltco/django-twc-toolbox/issues
 Project-URL: Source, https://github.com/westerveltco/django-twc-toolbox
 Author-email: Josh Thomas <josh@joshthomas.dev>
 License: MIT License
         
@@ -42,15 +42,15 @@
 Requires-Dist: coverage[toml]; extra == 'dev'
 Requires-Dist: django-stubs; extra == 'dev'
 Requires-Dist: django-stubs-ext; extra == 'dev'
 Requires-Dist: faker; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: model-bakery; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: nox; extra == 'dev'
+Requires-Dist: nox[uv]; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
 Requires-Dist: pytest-django; extra == 'dev'
 Requires-Dist: pytest-randomly; extra == 'dev'
 Requires-Dist: pytest-reverse; extra == 'dev'
 Requires-Dist: pytest-xdist; extra == 'dev'
 Provides-Extra: docs
```

