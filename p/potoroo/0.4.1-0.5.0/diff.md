# Comparing `tmp/potoroo-0.4.1.tar.gz` & `tmp/potoroo-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "potoroo-0.4.1.tar", last modified: Sat Jun  4 17:54:34 2022, max compression
+gzip compressed data, was "potoroo-0.5.0.tar", last modified: Wed Apr  3 21:55:48 2024, max compression
```

## Comparing `potoroo-0.4.1.tar` & `potoroo-0.5.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.341269 potoroo-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-06-04 17:54:09.000000 potoroo-0.4.1/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-06-04 17:54:09.000000 potoroo-0.4.1/.codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      770 2022-06-04 17:54:09.000000 potoroo-0.4.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:09.000000 potoroo-0.4.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/CODEOWNERS
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/ci.md
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/misc.md
--rw-r--r--   0 runner    (1001) docker     (121)      116 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/refactor.md
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/security.md
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/ISSUE_TEMPLATE/tests.md
--rw-r--r--   0 runner    (1001) docker     (121)      941 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/labels.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2672 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-06-04 17:54:09.000000 potoroo-0.4.1/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-06-04 17:54:09.000000 potoroo-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-06-04 17:54:09.000000 potoroo-0.4.1/.hadolint.yml
--rw-r--r--   0 runner    (1001) docker     (121)     8952 2022-06-04 17:54:09.000000 potoroo-0.4.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-06-04 17:54:09.000000 potoroo-0.4.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1779 2022-06-04 17:54:09.000000 potoroo-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)      313 2022-06-04 17:54:09.000000 potoroo-0.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     9765 2022-06-04 17:54:09.000000 potoroo-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-06-04 17:54:09.000000 potoroo-0.4.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-06-04 17:54:09.000000 potoroo-0.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-06-04 17:54:34.341269 potoroo-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3178 2022-06-04 17:54:09.000000 potoroo-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1245 2022-06-04 17:54:09.000000 potoroo-0.4.1/bin/check_cc
--rwxr-xr-x   0 runner    (1001) docker     (121)     1158 2022-06-04 17:54:09.000000 potoroo-0.4.1/bin/publish_docs
--rwxr-xr-x   0 runner    (1001) docker     (121)      681 2022-06-04 17:54:09.000000 potoroo-0.4.1/bin/quick-lints
--rwxr-xr-x   0 runner    (1001) docker     (121)     3403 2022-06-04 17:54:09.000000 potoroo-0.4.1/bin/render_all_cogs
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-06-04 17:54:09.000000 potoroo-0.4.1/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      638 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/docs/design/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/design/design.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/design/design.template.md
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/_static/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/_templates/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/_templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/potoroo.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-06-04 17:54:09.000000 potoroo-0.4.1/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:09.000000 potoroo-0.4.1/dpkg-dependencies.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/lib/
--rw-r--r--   0 runner    (1001) docker     (121)     7833 2022-06-04 17:54:09.000000 potoroo-0.4.1/lib/bugyi.sh
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-06-04 17:54:09.000000 potoroo-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      555 2022-06-04 17:54:09.000000 potoroo-0.4.1/requirements-dev.in
--rw-r--r--   0 runner    (1001) docker     (121)     4856 2022-06-04 17:54:09.000000 potoroo-0.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-04 17:54:09.000000 potoroo-0.4.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-06-04 17:54:09.000000 potoroo-0.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.337269 potoroo-0.4.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-06-04 17:54:09.000000 potoroo-0.4.1/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-06-04 17:54:34.341269 potoroo-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3469 2022-06-04 17:54:09.000000 potoroo-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.333269 potoroo-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.341269 potoroo-0.4.1/src/potoroo/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-06-04 17:54:09.000000 potoroo-0.4.1/src/potoroo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2297 2022-06-04 17:54:09.000000 potoroo-0.4.1/src/potoroo/_repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-06-04 17:54:09.000000 potoroo-0.4.1/src/potoroo/_uow.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:09.000000 potoroo-0.4.1/src/potoroo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.341269 potoroo-0.4.1/src/potoroo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3898 2022-06-04 17:54:34.000000 potoroo-0.4.1/src/potoroo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1535 2022-06-04 17:54:34.000000 potoroo-0.4.1/src/potoroo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 17:54:34.000000 potoroo-0.4.1/src/potoroo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-04 17:54:20.000000 potoroo-0.4.1/src/potoroo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-06-04 17:54:34.000000 potoroo-0.4.1/src/potoroo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-06-04 17:54:34.000000 potoroo-0.4.1/src/potoroo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6187 2022-06-04 17:54:09.000000 potoroo-0.4.1/targets.mk
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-04 17:54:34.341269 potoroo-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-04 17:54:09.000000 potoroo-0.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-04 17:54:09.000000 potoroo-0.4.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2174 2022-06-04 17:54:09.000000 potoroo-0.4.1/tests/test_potoroo.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-06-04 17:54:09.000000 potoroo-0.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.947749 potoroo-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 21:55:40.000000 potoroo-0.5.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 21:55:40.000000 potoroo-0.5.0/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 21:55:40.000000 potoroo-0.5.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.939749 potoroo-0.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/CODEOWNERS
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.939749 potoroo-0.5.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/ci.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/misc.md
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/refactor.md
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/security.md
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/ISSUE_TEMPLATE/tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/labels.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.939749 potoroo-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-03 21:55:40.000000 potoroo-0.5.0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-03 21:55:40.000000 potoroo-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 21:55:40.000000 potoroo-0.5.0/.hadolint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-03 21:55:40.000000 potoroo-0.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-04-03 21:55:40.000000 potoroo-0.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-03 21:55:40.000000 potoroo-0.5.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 21:55:40.000000 potoroo-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9765 2024-04-03 21:55:40.000000 potoroo-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 21:55:40.000000 potoroo-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-03 21:55:40.000000 potoroo-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-03 21:55:48.947749 potoroo-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-03 21:55:40.000000 potoroo-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1245 2024-04-03 21:55:40.000000 potoroo-0.5.0/bin/check_cc
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1158 2024-04-03 21:55:40.000000 potoroo-0.5.0/bin/publish_docs
+-rwxr-xr-x   0 runner    (1001) docker     (127)      681 2024-04-03 21:55:40.000000 potoroo-0.5.0/bin/quick-lints
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3403 2024-04-03 21:55:40.000000 potoroo-0.5.0/bin/render_all_cogs
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 21:55:40.000000 potoroo-0.5.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/design/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/design/design.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/design/design.template.md
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/_static/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/_templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/_templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/potoroo.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 21:55:40.000000 potoroo-0.5.0/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/dpkg-dependencies.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     7833 2024-04-03 21:55:40.000000 potoroo-0.5.0/lib/bugyi.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-03 21:55:40.000000 potoroo-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-03 21:55:40.000000 potoroo-0.5.0/requirements-dev.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-03 21:55:40.000000 potoroo-0.5.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 21:55:40.000000 potoroo-0.5.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-03 21:55:40.000000 potoroo-0.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.943749 potoroo-0.5.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 21:55:40.000000 potoroo-0.5.0/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 21:55:48.947749 potoroo-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-03 21:55:40.000000 potoroo-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.931748 potoroo-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.947749 potoroo-0.5.0/src/potoroo/
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 21:55:40.000000 potoroo-0.5.0/src/potoroo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-04-03 21:55:40.000000 potoroo-0.5.0/src/potoroo/_repo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-03 21:55:40.000000 potoroo-0.5.0/src/potoroo/_uow.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:40.000000 potoroo-0.5.0/src/potoroo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.947749 potoroo-0.5.0/src/potoroo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:55:45.000000 potoroo-0.5.0/src/potoroo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 21:55:48.000000 potoroo-0.5.0/src/potoroo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-03 21:55:40.000000 potoroo-0.5.0/targets.mk
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:55:48.947749 potoroo-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-03 21:55:40.000000 potoroo-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-03 21:55:40.000000 potoroo-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-03 21:55:40.000000 potoroo-0.5.0/tests/test_potoroo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-03 21:55:40.000000 potoroo-0.5.0/tox.ini
```

### Comparing `potoroo-0.4.1/.cruft.json` & `potoroo-0.5.0/.cruft.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'fa0499ecbf36aa3124fad11b92826161d5e424f0'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "4e0a8f622f41f01ab28a11d155a6706761a62165",
+    "commit": "fa0499ecbf36aa3124fad11b92826161d5e424f0",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/python-boltons/cc-python",
             "author": "Bryan M Bugyi",
             "email": "bryanbugyi34@gmail.com",
             "git_org_name": "bbugyi200",
             "git_repo_name": "potoroo",
```

### Comparing `potoroo-0.4.1/.github/labels.yml` & `potoroo-0.5.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/.github/workflows/ci.yml` & `potoroo-0.5.0/.github/workflows/ci.yml`

 * *Files 17% similar despite different names*

```diff
@@ -17,15 +17,17 @@
           fetch-depth: 0
 
       - name: Set up Python
         uses: actions/setup-python@v2
 
       - name: Install Dependencies
         run: |
-          python -m pip install -U pip docker-compose
+          mkdir -p ~/.docker/cli-plugins/
+          curl -SL https://github.com/docker/compose/releases/download/v2.3.3/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose
+          chmod +x ~/.docker/cli-plugins/docker-compose
 
       - name: Unit tests
         run: |
           make test
 
       - name: Publish coverage to codecov.io.
         uses: codecov/codecov-action@v2
@@ -40,15 +42,17 @@
       - uses: actions/checkout@v2
 
       - name: Set up Python
         uses: actions/setup-python@v2
 
       - name: Install Dependencies
         run: |
-          python -m pip install -U pip docker-compose
+          mkdir -p ~/.docker/cli-plugins/
+          curl -SL https://github.com/docker/compose/releases/download/v2.3.3/docker-compose-linux-x86_64 -o ~/.docker/cli-plugins/docker-compose
+          chmod +x ~/.docker/cli-plugins/docker-compose
 
       - name: Run linters.
         run: |
           make lint
   check_cc_and_requirements:
     runs-on: [ubuntu-latest]
     steps:
@@ -93,11 +97,11 @@
       - name: Build docs and publish them back to the master branch if necessary.
         if: github.repository == 'bbugyi200/potoroo' && github.ref == 'refs/heads/master'
         run: |
           ./bin/publish_docs
 
       - name: Publish distribution to PyPI
         if: github.repository == 'bbugyi200/potoroo' && startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
           skip_existing: true
```

### Comparing `potoroo-0.4.1/.gitignore` & `potoroo-0.5.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -113,7 +113,13 @@
 .*.sw?
 
 # Project docker switch file
 .lcldev
 
 # git conflict files
 *.rej
+
+# pyright config file
+pyrightconfig.json
+
+# local sqlite databases
+*.db
```

### Comparing `potoroo-0.4.1/.pylintrc` & `potoroo-0.5.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/CHANGELOG.md` & `potoroo-0.5.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,19 +5,27 @@
 The format is based on [Keep a Changelog], and this project adheres to
 [Semantic Versioning].
 
 [Keep a Changelog]: https://keepachangelog.com/en/1.0.0/
 [Semantic Versioning]: https://semver.org/
 
 
-## [Unreleased](https://github.com/bbugyi200/potoroo/compare/0.4.1...HEAD)
+## [Unreleased](https://github.com/bbugyi200/potoroo/compare/0.5.0...HEAD)
 
 No notable changes have been made.
 
 
+## [0.5.0](https://github.com/bbugyi200/potoroo/compare/0.4.1...0.5.0) - 2024-04-03
+
+### Changed
+
+* *BREAKING CHANGE*: Implement `remove_by_tag()` and `remove_by_key()` and
+  change remove() to accept item.
+
+
 ## [0.4.1](https://github.com/bbugyi200/potoroo/compare/0.4.0...0.4.1) - 2022-06-04
 
 ### Changed
 
 * Improve error handling of default `Repo.update()` implementation.
```

### Comparing `potoroo-0.4.1/CONTRIBUTING.md` & `potoroo-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/Dockerfile` & `potoroo-0.5.0/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-FROM pythonboltons/main:2021.12.22
+FROM pythonboltons/main:2024.01.16
 
 SHELL ["/bin/bash", "-o", "pipefail", "-c"]
 
 ARG USER_ID
 ARG GROUP_ID
 
 ### install dpkgs
 COPY dpkg-dependencies.txt /tmp/
 # hadolint ignore=SC2046
-RUN apt-get install -y --no-install-recommends --allow-unauthenticated $(grep "^[A-Za-z]" /tmp/dpkg-dependencies.txt | perl -nE 'print s/^([^#]+)[ ]+#.*/\1/gr') && \
+RUN apt-get update && \
+    apt-get install -y --no-install-recommends --allow-unauthenticated $(grep "^[A-Za-z]" /tmp/dpkg-dependencies.txt | perl -nE 'print s/^([^#]+)[ ]+#.*/\1/gr') && \
     apt-get clean
 
 ### create new user account ('docker')
 RUN groupadd --gid $GROUP_ID docker && \
         useradd --no-log-init --create-home --uid $USER_ID --gid docker docker && \
         cp /bashrc /home/docker/.bashrc
 USER docker
```

### Comparing `potoroo-0.4.1/Makefile` & `potoroo-0.5.0/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 .DEFAULT_GOAL := help
 .DELETE_ON_ERROR:
 .SHELLFLAGS := -eu -o pipefail -c
 .SUFFIXES:
 MAKEFLAGS += --warn-undefined-variables
 SHELL := /bin/bash
 
-DOCKER_CMD := USER_ID=$(shell id -u) GROUP_ID=$(shell id -g) docker-compose run --rm bbugyi200.potoroo
+DOCKER_CMD := USER_ID=$(shell id -u) GROUP_ID=$(shell id -g) docker compose run --rm bbugyi200.potoroo
 MAKE_CMD := make -f targets.mk
 USE_DOCKER_FILE := .lcldev/use-docker
 
 # If .lcldev/use-docker exists, then set `USE_DOCKER` to True
 ifneq ("$(wildcard $(USE_DOCKER_FILE))","")
 	USE_DOCKER := True
 endif
```

### Comparing `potoroo-0.4.1/PKG-INFO` & `potoroo-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: potoroo
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python implementations of the Repository and UnitOfWork abstractions.
 Home-page: https://github.com/bbugyi200/potoroo
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: bolton-eris~=0.2.3
 
 # potoroo
 
 **Python implementations of the Repository and UnitOfWork abstractions.**
 
 _project status badges:_
 
@@ -29,16 +30,16 @@
 [![Documentation Status](https://readthedocs.org/projects/potoroo/badge/?version=latest)](https://potoroo.readthedocs.io/en/latest/?badge=latest)
 [![Package Health](https://snyk.io/advisor/python/potoroo/badge.svg)](https://snyk.io/advisor/python/potoroo)
 
 _version badges:_
 
 [![Project Version](https://img.shields.io/pypi/v/potoroo)](https://pypi.org/project/potoroo/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/potoroo)](https://pypi.org/project/potoroo/)
-[![Cookiecutter: cc-python](https://img.shields.io/static/v1?label=cc-python&message=2022.01.04&color=d4aa00&logo=cookiecutter&logoColor=d4aa00)](https://github.com/python-boltons/cc-python)
-[![Docker: pythonboltons/main](https://img.shields.io/static/v1?label=pythonboltons%20%2F%20main&message=2021.12.22&color=8ec4ad&logo=docker&logoColor=8ec4ad)](https://github.com/python-boltons/docker-python)
+[![Cookiecutter: cc-python](https://img.shields.io/static/v1?label=cc-python&message=2024.01.16-4&color=d4aa00&logo=cookiecutter&logoColor=d4aa00)](https://github.com/python-boltons/cc-python)
+[![Docker: pythonboltons/main](https://img.shields.io/static/v1?label=pythonboltons%20%2F%20main&message=2024.01.16&color=8ec4ad&logo=docker&logoColor=8ec4ad)](https://github.com/python-boltons/docker-python)
 
 
 ## Installation 🗹
 
 To install `potoroo` using [pip][9], run the following
 commands in your terminal:
 
@@ -85,9 +86,8 @@
 [7]: https://github.com/bbugyi200/potoroo/blob/master/CONTRIBUTING.md
 [8]: https://github.com/bbugyi200/potoroo
 [9]: https://pip.pypa.io
 [10]: http://docs.python-guide.org/en/latest/starting/installation/
 [11]: https://github.com/pypa/pipx
 [12]: https://github.com/cruft/cruft
 [13]: https://github.com/bbugyi200/potoroo/issues/new/choose
-
-
+[14]: https://pypi.org/project/cogapp/
```

### Comparing `potoroo-0.4.1/README.md` & `potoroo-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 [![Documentation Status](https://readthedocs.org/projects/potoroo/badge/?version=latest)](https://potoroo.readthedocs.io/en/latest/?badge=latest)
 [![Package Health](https://snyk.io/advisor/python/potoroo/badge.svg)](https://snyk.io/advisor/python/potoroo)
 
 _version badges:_
 
 [![Project Version](https://img.shields.io/pypi/v/potoroo)](https://pypi.org/project/potoroo/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/potoroo)](https://pypi.org/project/potoroo/)
-[![Cookiecutter: cc-python](https://img.shields.io/static/v1?label=cc-python&message=2022.01.04&color=d4aa00&logo=cookiecutter&logoColor=d4aa00)](https://github.com/python-boltons/cc-python)
-[![Docker: pythonboltons/main](https://img.shields.io/static/v1?label=pythonboltons%20%2F%20main&message=2021.12.22&color=8ec4ad&logo=docker&logoColor=8ec4ad)](https://github.com/python-boltons/docker-python)
+[![Cookiecutter: cc-python](https://img.shields.io/static/v1?label=cc-python&message=2024.01.16-4&color=d4aa00&logo=cookiecutter&logoColor=d4aa00)](https://github.com/python-boltons/cc-python)
+[![Docker: pythonboltons/main](https://img.shields.io/static/v1?label=pythonboltons%20%2F%20main&message=2024.01.16&color=8ec4ad&logo=docker&logoColor=8ec4ad)](https://github.com/python-boltons/docker-python)
 
 
 ## Installation 🗹
 
 To install `potoroo` using [pip][9], run the following
 commands in your terminal:
 
@@ -65,7 +65,8 @@
 [7]: https://github.com/bbugyi200/potoroo/blob/master/CONTRIBUTING.md
 [8]: https://github.com/bbugyi200/potoroo
 [9]: https://pip.pypa.io
 [10]: http://docs.python-guide.org/en/latest/starting/installation/
 [11]: https://github.com/pypa/pipx
 [12]: https://github.com/cruft/cruft
 [13]: https://github.com/bbugyi200/potoroo/issues/new/choose
+[14]: https://pypi.org/project/cogapp/
```

### Comparing `potoroo-0.4.1/bin/check_cc` & `potoroo-0.5.0/bin/check_cc`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/bin/publish_docs` & `potoroo-0.5.0/bin/publish_docs`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/bin/quick-lints` & `potoroo-0.5.0/bin/quick-lints`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/bin/render_all_cogs` & `potoroo-0.5.0/bin/render_all_cogs`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/docs/Makefile` & `potoroo-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/docs/make.bat` & `potoroo-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/docs/source/conf.py` & `potoroo-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/lib/bugyi.sh` & `potoroo-0.5.0/lib/bugyi.sh`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/requirements-dev.txt` & `potoroo-0.5.0/requirements-dev.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,260 +1,269 @@
 #
-# This file is autogenerated by pip-compile with python 3.8
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.10
+# by the following command:
 #
 #    "make update-requirements"
 #
 -e file:.#egg=potoroo>=0.dev
     # via -r requirements-dev.in
-alabaster==0.7.12
+alabaster==0.7.16
     # via sphinx
-arrow==1.2.2
-    # via jinja2-time
-astroid==2.11.5
+arrow==1.3.0
+    # via cookiecutter
+astroid==3.1.0
     # via pylint
-attrs==21.4.0
-    # via pytest
-babel==2.10.1
+babel==2.14.0
     # via sphinx
 binaryornot==0.4.4
     # via cookiecutter
-black==22.3.0
+black==24.3.0
     # via -r requirements-dev.in
 bolton-eris==0.2.3
     # via
     #   -r requirements.in
     #   potoroo
 bolton-ion==0.1.0
     # via bolton-eris
-bolton-metaman==0.1.1
+bolton-metaman==0.1.2
     # via bolton-eris
 bolton-typist==0.2.0
     # via bolton-eris
+build==1.2.1
+    # via pip-tools
 bump2version==1.0.1
     # via -r requirements-dev.in
-certifi==2022.5.18.1
+certifi==2024.2.2
     # via requests
-chardet==4.0.0
+chardet==5.2.0
     # via binaryornot
-charset-normalizer==2.0.12
+charset-normalizer==3.3.2
     # via requests
-click==8.1.3
+click==8.1.7
     # via
     #   black
     #   cookiecutter
     #   cruft
     #   pip-tools
-    #   typer
-cogapp==3.3.0
+    #   typer-slim
+cogapp==3.4.1
     # via -r requirements-dev.in
-colored==1.4.3
-    # via syrupy
-cookiecutter==1.7.3
+cookiecutter==2.6.0
     # via cruft
-coverage[toml]==6.4.1
+coverage[toml]==7.4.4
     # via pytest-cov
-cruft[pyproject]==2.10.2
+cruft[pyproject]==2.15.0
     # via -r requirements-dev.in
-dill==0.3.5.1
+dill==0.3.8
     # via pylint
-distlib==0.3.4
+distlib==0.3.8
     # via virtualenv
-docutils==0.17.1
+docutils==0.20.1
     # via
     #   m2r2
     #   sphinx
     #   sphinx-rtd-theme
-filelock==3.7.1
+exceptiongroup==1.2.0
+    # via pytest
+filelock==3.13.3
     # via
     #   tox
     #   virtualenv
-flake8==4.0.1
+flake8==7.0.0
     # via -r requirements-dev.in
-gitdb==4.0.9
+gitdb==4.0.11
     # via gitpython
-gitpython==3.1.27
+gitpython==3.1.43
     # via cruft
-idna==3.3
+idna==3.6
     # via requests
-imagesize==1.3.0
+imagesize==1.4.1
     # via sphinx
-importlib-metadata==4.11.4
-    # via sphinx
-iniconfig==1.1.1
+iniconfig==2.0.0
     # via pytest
-isort==5.10.1
+isort==5.13.2
     # via
     #   -r requirements-dev.in
     #   pylint
-jinja2==3.1.2
+jinja2==3.1.3
     # via
     #   cookiecutter
-    #   jinja2-time
     #   sphinx
-jinja2-time==0.2.0
-    # via cookiecutter
-lazy-object-proxy==1.7.1
-    # via astroid
-m2r2==0.3.2
+m2r2==0.3.3.post2
     # via -r requirements-dev.in
-markupsafe==2.1.1
+markdown-it-py==3.0.0
+    # via rich
+markupsafe==2.1.5
     # via jinja2
-mccabe==0.6.1
+mccabe==0.7.0
     # via
     #   flake8
     #   pylint
+mdurl==0.1.2
+    # via markdown-it-py
 mistune==0.8.4
     # via m2r2
-mypy==0.960
+mypy==1.9.0
     # via -r requirements-dev.in
-mypy-extensions==0.4.3
+mypy-extensions==1.0.0
     # via
     #   black
     #   mypy
-packaging==21.3
+packaging==24.0
     # via
+    #   black
+    #   build
     #   pytest
     #   setuptools-scm
     #   sphinx
     #   tox
-pathspec==0.9.0
+pathspec==0.12.1
     # via black
-pep517==0.12.0
-    # via pip-tools
-pip-tools==6.6.2
+pip-tools==7.4.1
     # via -r requirements-dev.in
-platformdirs==2.5.2
+platformdirs==4.2.0
     # via
     #   black
     #   pylint
     #   virtualenv
-pluggy==1.0.0
+pluggy==1.4.0
     # via
     #   pytest
     #   tox
-poyo==0.5.0
-    # via cookiecutter
 py==1.11.0
-    # via
-    #   pytest
-    #   tox
-pycodestyle==2.8.0
+    # via tox
+pycodestyle==2.11.1
     # via flake8
-pydocstyle[toml]==6.1.1
+pydocstyle[toml]==6.3.0
     # via -r requirements-dev.in
-pyflakes==2.4.0
+pyflakes==3.2.0
     # via flake8
-pygments==2.12.0
-    # via sphinx
-pylint==2.14.0
+pygments==2.17.2
+    # via
+    #   rich
+    #   sphinx
+pylint==3.1.0
     # via -r requirements-dev.in
-pyparsing==3.0.9
-    # via packaging
-pytest==7.1.2
+pyproject-hooks==1.0.0
+    # via
+    #   build
+    #   pip-tools
+pytest==7.4.4
     # via
     #   -r requirements-dev.in
     #   pytest-cov
     #   pytest-mock
     #   syrupy
-pytest-cov==3.0.0
+pytest-cov==5.0.0
     # via -r requirements-dev.in
-pytest-mock==3.7.0
+pytest-mock==3.14.0
     # via -r requirements-dev.in
-python-dateutil==2.8.2
+python-dateutil==2.9.0.post0
     # via arrow
-python-slugify==6.1.2
+python-slugify==8.0.4
     # via cookiecutter
-pytz==2022.1
-    # via babel
-requests==2.27.1
+pyyaml==6.0.1
+    # via cookiecutter
+requests==2.31.0
     # via
     #   cookiecutter
     #   sphinx
-setuptools-scm==6.4.2
+rich==13.7.1
+    # via
+    #   cookiecutter
+    #   typer-slim
+setuptools-scm==8.0.4
     # via -r requirements-dev.in
+shellingham==1.5.4
+    # via typer-slim
 six==1.16.0
     # via
-    #   cookiecutter
     #   python-dateutil
     #   tox
-    #   virtualenv
-smmap==5.0.0
+smmap==5.0.1
     # via gitdb
 snowballstemmer==2.2.0
     # via
     #   pydocstyle
     #   sphinx
-sphinx==5.0.1
+sphinx==7.2.6
     # via
     #   -r requirements-dev.in
     #   sphinx-autodoc-typehints
     #   sphinx-rtd-theme
-sphinx-autodoc-typehints==1.18.2
+    #   sphinxcontrib-jquery
+sphinx-autodoc-typehints==2.0.0
     # via -r requirements-dev.in
-sphinx-rtd-theme==1.0.0
+sphinx-rtd-theme==2.0.0
     # via -r requirements-dev.in
-sphinxcontrib-applehelp==1.0.2
+sphinxcontrib-applehelp==1.0.8
     # via sphinx
-sphinxcontrib-devhelp==1.0.2
+sphinxcontrib-devhelp==1.0.6
     # via sphinx
-sphinxcontrib-htmlhelp==2.0.0
+sphinxcontrib-htmlhelp==2.0.5
     # via sphinx
+sphinxcontrib-jquery==4.1
+    # via sphinx-rtd-theme
 sphinxcontrib-jsmath==1.0.1
     # via sphinx
-sphinxcontrib-qthelp==1.0.3
+sphinxcontrib-qthelp==1.0.7
     # via sphinx
-sphinxcontrib-serializinghtml==1.1.5
+sphinxcontrib-serializinghtml==1.1.10
     # via sphinx
-syrupy==2.3.0
+syrupy==4.6.1
     # via -r requirements-dev.in
 text-unidecode==1.3
     # via python-slugify
 toml==0.10.2
-    # via
-    #   cruft
-    #   pydocstyle
-    #   tox
+    # via cruft
 tomli==2.0.1
     # via
     #   black
+    #   build
     #   coverage
     #   mypy
-    #   pep517
+    #   pip-tools
+    #   pydocstyle
     #   pylint
+    #   pyproject-hooks
     #   pytest
     #   setuptools-scm
-tomlkit==0.11.0
+    #   tox
+tomlkit==0.12.4
     # via pylint
-tox==3.25.0
+tox==3.28.0
     # via
     #   -r requirements-dev.in
     #   tox-pyenv
 tox-pyenv==1.1.0
     # via -r requirements-dev.in
-typer==0.4.1
+typer==0.12.0
     # via cruft
-typing-extensions==4.2.0
+typer-cli==0.12.0
+    # via typer
+typer-slim[standard]==0.12.0
+    # via
+    #   typer
+    #   typer-cli
+types-python-dateutil==2.9.0.20240316
+    # via arrow
+typing-extensions==4.10.0
     # via
     #   astroid
     #   black
     #   mypy
-    #   pylint
-urllib3==1.26.9
+    #   setuptools-scm
+    #   typer-slim
+urllib3==2.2.1
     # via requests
-virtualenv==20.14.1
+virtualenv==20.25.1
     # via tox
-wheel==0.37.1
+wheel==0.43.0
     # via pip-tools
-wrapt==1.14.1
-    # via astroid
-zipp==3.8.0
-    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
-pip==22.1.2
+pip==24.0
     # via pip-tools
-setuptools==62.3.2
+setuptools==69.2.0
     # via
-    #   astroid
     #   pip-tools
     #   setuptools-scm
```

### Comparing `potoroo-0.4.1/setup.cfg` & `potoroo-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/setup.py` & `potoroo-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 
 
 ###############################################################################
 # Configuration variables that are likely to need changing at some point.
 ###############################################################################
 DESCRIPTION = "Python implementations of the Repository and UnitOfWork abstractions."
 SUPPORTED_PYTHON_VERSIONS = [
-    (3, 8),
     (3, 9),
     (3, 10),
+    (3, 11),
+    (3, 12),
 ]
-USE_SCM_VERSION = {"fallback_version": "0.4.1"}
+USE_SCM_VERSION = {"fallback_version": "0.5.0"}
 
 
 ###############################################################################
 # Helper functions.
 ###############################################################################
 def long_description() -> str:
     """Returns the body of this project's page on PyPI."""
```

### Comparing `potoroo-0.4.1/src/potoroo/_uow.py` & `potoroo-0.5.0/src/potoroo/_uow.py`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/src/potoroo.egg-info/PKG-INFO` & `potoroo-0.5.0/src/potoroo.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: potoroo
-Version: 0.4.1
+Version: 0.5.0
 Summary: Python implementations of the Repository and UnitOfWork abstractions.
 Home-page: https://github.com/bbugyi200/potoroo
 Author: Bryan M Bugyi
 Author-email: bryanbugyi34@gmail.com
 License: MIT license
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: bolton-eris~=0.2.3
 
 # potoroo
 
 **Python implementations of the Repository and UnitOfWork abstractions.**
 
 _project status badges:_
 
@@ -29,16 +30,16 @@
 [![Documentation Status](https://readthedocs.org/projects/potoroo/badge/?version=latest)](https://potoroo.readthedocs.io/en/latest/?badge=latest)
 [![Package Health](https://snyk.io/advisor/python/potoroo/badge.svg)](https://snyk.io/advisor/python/potoroo)
 
 _version badges:_
 
 [![Project Version](https://img.shields.io/pypi/v/potoroo)](https://pypi.org/project/potoroo/)
 [![Python Versions](https://img.shields.io/pypi/pyversions/potoroo)](https://pypi.org/project/potoroo/)
-[![Cookiecutter: cc-python](https://img.shields.io/static/v1?label=cc-python&message=2022.01.04&color=d4aa00&logo=cookiecutter&logoColor=d4aa00)](https://github.com/python-boltons/cc-python)
-[![Docker: pythonboltons/main](https://img.shields.io/static/v1?label=pythonboltons%20%2F%20main&message=2021.12.22&color=8ec4ad&logo=docker&logoColor=8ec4ad)](https://github.com/python-boltons/docker-python)
+[![Cookiecutter: cc-python](https://img.shields.io/static/v1?label=cc-python&message=2024.01.16-4&color=d4aa00&logo=cookiecutter&logoColor=d4aa00)](https://github.com/python-boltons/cc-python)
+[![Docker: pythonboltons/main](https://img.shields.io/static/v1?label=pythonboltons%20%2F%20main&message=2024.01.16&color=8ec4ad&logo=docker&logoColor=8ec4ad)](https://github.com/python-boltons/docker-python)
 
 
 ## Installation 🗹
 
 To install `potoroo` using [pip][9], run the following
 commands in your terminal:
 
@@ -85,9 +86,8 @@
 [7]: https://github.com/bbugyi200/potoroo/blob/master/CONTRIBUTING.md
 [8]: https://github.com/bbugyi200/potoroo
 [9]: https://pip.pypa.io
 [10]: http://docs.python-guide.org/en/latest/starting/installation/
 [11]: https://github.com/pypa/pipx
 [12]: https://github.com/cruft/cruft
 [13]: https://github.com/bbugyi200/potoroo/issues/new/choose
-
-
+[14]: https://pypi.org/project/cogapp/
```

### Comparing `potoroo-0.4.1/src/potoroo.egg-info/SOURCES.txt` & `potoroo-0.5.0/src/potoroo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `potoroo-0.4.1/targets.mk` & `potoroo-0.5.0/targets.mk`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 DOCS_SOURCE := ./docs/source
 DOCS_BUILD_DIR := ./docs/build
 MIN_TEST_COV := 80
 PIP = $(PYTHON) -m pip
 PIP_COMPILE = $(PYTHON) -m piptools compile --allow-unsafe --no-emit-index-url -q --no-emit-trusted-host
 PIP_SYNC = $(PYTHON) -m piptools sync
 PYTHON = $(SOURCE_VENV) python
-PYTHON_VERSION := 3.8
+PYTHON_VERSION := 3.10
 RENDER_ALL_COGS = $(SOURCE_VENV) ./bin/render_all_cogs
 SOURCE_VENV = source $(VENV_ACTIVATE);
 SPHINX_APIDOC = $(SOURCE_VENV) sphinx-apidoc
 SPHINX_BUILD = $(SOURCE_VENV) sphinx-build
 TOX = $(SOURCE_VENV) tox
 VENV := .venv
 VENV_ACTIVATE = $(VENV)/bin/activate
```

### Comparing `potoroo-0.4.1/tests/test_potoroo.py` & `potoroo-0.5.0/tests/test_potoroo.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Tests for the potoroo package."""
 
 from __future__ import annotations
 
-from eris import ErisResult, Ok
+from eris import ErisResult, Err, Ok
 
 from potoroo import Repo, TaggedRepo
 
 
 class FakeDB(Repo[int, str]):
     """Fake database."""
 
@@ -20,51 +20,47 @@
         self._db[key] = some_item
         return Ok(key)
 
     def get(self, key: int) -> ErisResult[str | None]:
         """Fake get."""
         return Ok(self._db[key])
 
-    def remove(self, key: int) -> ErisResult[str | None]:
+    def remove(self, item: str, /) -> ErisResult[str | None]:
         """Fake remove."""
-        return Ok(self._db.pop(key))
-
-    def update(self, key: int, some_item: str, /) -> ErisResult[str]:
-        """Fake update."""
-        self._db[key] = some_item
-        return Ok(some_item)
+        item_key = None
+        for key, value in self._db.items():
+            if value == item:
+                item_key = key
+                break
+        else:
+            return Err(f"Unable to find item | {item=}")
+        return Ok(self._db.pop(item_key))
 
     def all(self) -> ErisResult[list[str]]:
         """Fake all."""
         return Ok(sorted(self._db.values()))
 
 
 class FakeTaggedDB(FakeDB, TaggedRepo[int, str, str]):
     """Fake tagged database."""
 
     def get_by_tag(self, tag: str) -> ErisResult[list[str]]:
         """Fake get_by_tag."""
         return Ok([v for v in self._db.values() if tag in v])
 
-    def remove_by_tag(self, tag: str) -> ErisResult[list[str]]:
-        """Fake remove_by_tag."""
-        res: list[str] = []
-        for k, v in dict(self._db).items():
-            if tag in v:
-                res.append(self._db.pop(k))
-        return Ok(res)
-
 
 def test_repo() -> None:
     """Test the Repo type."""
     db = FakeDB()
     foo_idx = db.add("foo").unwrap()
+    baz_idx = db.add("baz").unwrap()
     assert db.get(foo_idx).unwrap() == "foo"
-    assert db.update(foo_idx, "bar").unwrap() == "bar"
-    assert db.remove(foo_idx).unwrap() == "bar"
+    assert db.update(foo_idx, "bar").unwrap() == "foo"
+    assert db.remove("bar").unwrap() == "bar"
+    assert db.remove_by_key(baz_idx).unwrap() == "baz"
 
 
 def test_tagged_repo() -> None:
     """Test the TaggedRepo type."""
     db = FakeTaggedDB()
     foo_idx = db.add("foo").unwrap()
     db.add("bar").unwrap()
```

