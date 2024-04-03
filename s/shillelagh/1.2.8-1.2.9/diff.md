# Comparing `tmp/shillelagh-1.2.8.tar.gz` & `tmp/shillelagh-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-1.2.8.tar", last modified: Sat Oct 21 20:57:36 2023, max compression
+gzip compressed data, was "shillelagh-1.2.9.tar", last modified: Thu Nov  9 04:11:41 2023, max compression
```

## Comparing `shillelagh-1.2.8.tar` & `shillelagh-1.2.9.tar`

### file list

```diff
@@ -1,204 +1,207 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.691288 shillelagh-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      119 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.675289 shillelagh-1.2.8/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.675289 shillelagh-1.2.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.675289 shillelagh-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/workflows/python-integration.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       58 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2525 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-10-21 20:57:22.000000 shillelagh-1.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)    13961 2023-10-21 20:57:22.000000 shillelagh-1.2.8/ARCHITECTURE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-10-21 20:57:22.000000 shillelagh-1.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9154 2023-10-21 20:57:22.000000 shillelagh-1.2.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5223 2023-10-21 20:57:22.000000 shillelagh-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-10-21 20:57:22.000000 shillelagh-1.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-10-21 20:57:22.000000 shillelagh-1.2.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      725 2023-10-21 20:57:22.000000 shillelagh-1.2.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2023-10-21 20:57:36.691288 shillelagh-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2023-10-21 20:57:22.000000 shillelagh-1.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.675289 shillelagh-1.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.675289 shillelagh-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    18529 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9479 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    32853 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      998 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7428 2023-10-21 20:57:22.000000 shillelagh-1.2.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/datasette.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/generic_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/socrata.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-10-21 20:57:22.000000 shillelagh-1.2.8/examples/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-10-21 20:57:22.000000 shillelagh-1.2.8/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-10-21 20:57:22.000000 shillelagh-1.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-21 20:57:22.000000 shillelagh-1.2.8/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (127)      773 2023-10-21 20:57:22.000000 shillelagh-1.2.8/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2023-10-21 20:57:22.000000 shillelagh-1.2.8/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (127)     4091 2023-10-21 20:57:22.000000 shillelagh-1.2.8/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2023-10-21 20:57:36.691288 shillelagh-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      363 2023-10-21 20:57:22.000000 shillelagh-1.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.671289 shillelagh-1.2.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/src/shillelagh/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/src/shillelagh/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/src/shillelagh/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/datasette.py
--rw-r--r--   0 runner    (1001) docker     (127)     4368 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/generic_xml.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/github.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26870 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4116 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/parsing/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    19127 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/parsing/date.py
--rw-r--r--   0 runner    (1001) docker     (127)    18376 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/parsing/number.py
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/html_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    10603 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/s3select.py
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/socrata.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     7461 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/api/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8499 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/src/shillelagh/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10346 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/file/csvfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/src/shillelagh/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/memory/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/adapters/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/src/shillelagh/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/src/shillelagh/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16401 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/backends/apsw/db.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/src/shillelagh/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/backends/apsw/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7407 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/backends/apsw/dialects/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/backends/apsw/dialects/safe.py
--rw-r--r--   0 runner    (1001) docker     (127)    20047 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/backends/apsw/vt.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     3757 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21797 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    11160 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18942 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-10-21 20:57:22.000000 shillelagh-1.2.8/src/shillelagh/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.679288 shillelagh-1.2.8/src/shillelagh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2023-10-21 20:57:36.000000 shillelagh-1.2.8/src/shillelagh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2023-10-21 20:57:36.000000 shillelagh-1.2.8/src/shillelagh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 20:57:36.000000 shillelagh-1.2.8/src/shillelagh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-10-21 20:57:36.000000 shillelagh-1.2.8/src/shillelagh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-21 20:57:36.000000 shillelagh-1.2.8/src/shillelagh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2023-10-21 20:57:36.000000 shillelagh-1.2.8/src/shillelagh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-21 20:57:36.000000 shillelagh-1.2.8/src/shillelagh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/talks/
--rw-r--r--   0 runner    (1001) docker     (127)  2331376 2023-10-21 20:57:22.000000 shillelagh-1.2.8/talks/Python Brasil 2021.pdf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.671289 shillelagh-1.2.8/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/templates/adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2023-10-21 20:57:22.000000 shillelagh-1.2.8/templates/adapter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/templates/adapter/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (127)      267 2023-10-21 20:57:22.000000 shillelagh-1.2.8/templates/adapter/hooks/post_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/templates/adapter/{{cookiecutter.slug}}/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-10-21 20:57:22.000000 shillelagh-1.2.8/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2023-10-21 20:57:22.000000 shillelagh-1.2.8/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.683288 shillelagh-1.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14353 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/datasette_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/generic_json_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/generic_xml_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18505 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/github_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73772 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6163 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20327 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/parsing/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    21594 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/parsing/date_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    14588 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/gsheets/parsing/number_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/html_table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/s3select_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8515 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/socrata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9566 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/system_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    17776 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/api/weatherapi_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12222 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/file/csvfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9285 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/memory/pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/adapters/registry_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14748 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/apsw/db_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/apsw/dbapi_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.687288 shillelagh-1.2.8/tests/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/apsw/dialects/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15699 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/apsw/dialects/gsheets_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/apsw/dialects/safe_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16126 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/backends/apsw/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-21 20:57:36.691288 shillelagh-1.2.8/tests/fakes/
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   400535 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/cdc_data_response.json
--rw-r--r--   0 runner    (1001) docker     (127)   121689 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/cdc_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/datasette_columns_response.json
--rw-r--r--   0 runner    (1001) docker     (127)   369983 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/datasette_data_response_1.json
--rw-r--r--   0 runner    (1001) docker     (127)    60078 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/datasette_data_response_2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/datasette_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (127)   428142 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/datasette_results.json
--rw-r--r--   0 runner    (1001) docker     (127)   220647 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/github_response.json
--rw-r--r--   0 runner    (1001) docker     (127)    18818 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/github_single_response.json
--rw-r--r--   0 runner    (1001) docker     (127)   165205 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/incidents.json
--rw-r--r--   0 runner    (1001) docker     (127)    40785 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fakes/weatherapi_response.json
--rw-r--r--   0 runner    (1001) docker     (127)    13821 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9127 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/functions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13799 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-10-21 20:57:22.000000 shillelagh-1.2.8/tests/types_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.772387 shillelagh-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.748387 shillelagh-1.2.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.748387 shillelagh-1.2.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.748387 shillelagh-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/workflows/python-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2525 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2023-11-09 04:11:30.000000 shillelagh-1.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    13961 2023-11-09 04:11:30.000000 shillelagh-1.2.9/ARCHITECTURE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-11-09 04:11:30.000000 shillelagh-1.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9361 2023-11-09 04:11:30.000000 shillelagh-1.2.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5223 2023-11-09 04:11:30.000000 shillelagh-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-11-09 04:11:30.000000 shillelagh-1.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-11-09 04:11:30.000000 shillelagh-1.2.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2023-11-09 04:11:30.000000 shillelagh-1.2.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2023-11-09 04:11:41.772387 shillelagh-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7956 2023-11-09 04:11:30.000000 shillelagh-1.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.748387 shillelagh-1.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.748387 shillelagh-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    18529 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9479 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32853 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   113600 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7428 2023-11-09 04:11:30.000000 shillelagh-1.2.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.752387 shillelagh-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/generic_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2023-11-09 04:11:30.000000 shillelagh-1.2.9/examples/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-09 04:11:30.000000 shillelagh-1.2.9/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2023-11-09 04:11:30.000000 shillelagh-1.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.752387 shillelagh-1.2.9/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-09 04:11:30.000000 shillelagh-1.2.9/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2023-11-09 04:11:30.000000 shillelagh-1.2.9/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2023-11-09 04:11:30.000000 shillelagh-1.2.9/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2023-11-09 04:11:30.000000 shillelagh-1.2.9/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2023-11-09 04:11:41.772387 shillelagh-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2023-11-09 04:11:30.000000 shillelagh-1.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.740387 shillelagh-1.2.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.752387 shillelagh-1.2.9/src/shillelagh/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.756387 shillelagh-1.2.9/src/shillelagh/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.756387 shillelagh-1.2.9/src/shillelagh/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4376 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/generic_xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7494 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/github.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.756387 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26870 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.756387 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4116 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/parsing/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19127 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/parsing/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18376 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/parsing/number.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/html_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10603 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/s3select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7461 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/api/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8499 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.756387 shillelagh-1.2.9/src/shillelagh/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10346 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/file/csvfile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.760387 shillelagh-1.2.9/src/shillelagh/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2295 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/memory/holidays.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/memory/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/adapters/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.760387 shillelagh-1.2.9/src/shillelagh/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.760387 shillelagh-1.2.9/src/shillelagh/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16401 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/backends/apsw/db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.760387 shillelagh-1.2.9/src/shillelagh/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/backends/apsw/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7407 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/backends/apsw/dialects/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/backends/apsw/dialects/safe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20089 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/backends/apsw/vt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3757 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22414 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11160 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18942 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-11-09 04:11:30.000000 shillelagh-1.2.9/src/shillelagh/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.756387 shillelagh-1.2.9/src/shillelagh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10434 2023-11-09 04:11:41.000000 shillelagh-1.2.9/src/shillelagh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5398 2023-11-09 04:11:41.000000 shillelagh-1.2.9/src/shillelagh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 04:11:41.000000 shillelagh-1.2.9/src/shillelagh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-09 04:11:41.000000 shillelagh-1.2.9/src/shillelagh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-09 04:11:41.000000 shillelagh-1.2.9/src/shillelagh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-11-09 04:11:41.000000 shillelagh-1.2.9/src/shillelagh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-11-09 04:11:41.000000 shillelagh-1.2.9/src/shillelagh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.760387 shillelagh-1.2.9/talks/
+-rw-r--r--   0 runner    (1001) docker     (127)  2331376 2023-11-09 04:11:30.000000 shillelagh-1.2.9/talks/Python Brasil 2021.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.744387 shillelagh-1.2.9/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.764387 shillelagh-1.2.9/templates/adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2023-11-09 04:11:30.000000 shillelagh-1.2.9/templates/adapter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.764387 shillelagh-1.2.9/templates/adapter/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      267 2023-11-09 04:11:30.000000 shillelagh-1.2.9/templates/adapter/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.764387 shillelagh-1.2.9/templates/adapter/{{cookiecutter.slug}}/
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2023-11-09 04:11:30.000000 shillelagh-1.2.9/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4873 2023-11-09 04:11:30.000000 shillelagh-1.2.9/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.764387 shillelagh-1.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.764387 shillelagh-1.2.9/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.764387 shillelagh-1.2.9/tests/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14449 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/datasette_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7577 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/generic_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/generic_xml_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18505 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/github_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.768387 shillelagh-1.2.9/tests/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73772 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20327 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.768387 shillelagh-1.2.9/tests/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/parsing/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21594 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/parsing/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14588 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/gsheets/parsing/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2951 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/html_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/s3select_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8515 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/socrata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9566 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17776 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/api/weatherapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.768387 shillelagh-1.2.9/tests/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12222 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/file/csvfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.768387 shillelagh-1.2.9/tests/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/memory/holidays_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9285 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/memory/pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/adapters/registry_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.768387 shillelagh-1.2.9/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.768387 shillelagh-1.2.9/tests/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14748 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/apsw/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/apsw/dbapi_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.768387 shillelagh-1.2.9/tests/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/apsw/dialects/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15699 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/apsw/dialects/gsheets_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/apsw/dialects/safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16126 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/backends/apsw/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5906 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-09 04:11:41.772387 shillelagh-1.2.9/tests/fakes/
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   400535 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/cdc_data_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   121689 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/cdc_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/datasette_columns_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   369983 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/datasette_data_response_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    60078 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/datasette_data_response_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/datasette_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   428142 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/datasette_results.json
+-rw-r--r--   0 runner    (1001) docker     (127)   220647 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/github_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18818 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/github_single_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)   165205 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (127)    40785 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fakes/weatherapi_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14267 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9127 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2483 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13799 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2023-11-09 04:11:30.000000 shillelagh-1.2.9/tests/types_test.py
```

### Comparing `shillelagh-1.2.8/.coveragerc` & `shillelagh-1.2.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/.github/ISSUE_TEMPLATE/bug_report.md` & `shillelagh-1.2.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/.github/ISSUE_TEMPLATE/feature_request.md` & `shillelagh-1.2.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/.github/pull_request_template.md` & `shillelagh-1.2.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/.github/workflows/codeql-analysis.yml` & `shillelagh-1.2.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/.github/workflows/python-integration.yml` & `shillelagh-1.2.9/.github/workflows/python-integration.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/.github/workflows/python-package-daily.yml` & `shillelagh-1.2.9/.github/workflows/python-package-daily.yml`

 * *Files 11% similar despite different names*

```diff
@@ -25,11 +25,11 @@
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       env:
         VERSION: 3.38.1
         RELEASE: r1
       run: |
         python -m pip install --upgrade pip setuptools
-        pip install -e '.[testing]'
+        python -m pip install -e '.[testing]'
     - name: Test with pytest
       run: |
         pytest --cov-fail-under=100 --cov=src/shillelagh -vv tests/ --doctest-modules src/shillelagh --without-integration --without-slow-integration
```

### Comparing `shillelagh-1.2.8/.github/workflows/python-package.yml` & `shillelagh-1.2.9/.github/workflows/python-package.yml`

 * *Files 8% similar despite different names*

```diff
@@ -26,12 +26,12 @@
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       env:
         VERSION: 3.38.1
         RELEASE: r1
       run: |
         python -m pip install --upgrade pip setuptools
-        pip install -r requirements/test.txt
+        python -m pip install -r requirements/test.txt
     - name: Test with pytest
       run: |
         pre-commit run --all-files
         pytest --cov-fail-under=100 --cov=src/shillelagh -vv tests/ --doctest-modules src/shillelagh --without-integration --without-slow-integration
```

### Comparing `shillelagh-1.2.8/.github/workflows/python-publish.yml` & `shillelagh-1.2.9/.github/workflows/python-publish.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python
       uses: actions/setup-python@v2
       with:
-        python-version: '3.x'
+        python-version: '3.11'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install build
     - name: Build package
       run: python -m build
     - name: Publish package
```

### Comparing `shillelagh-1.2.8/.gitignore` & `shillelagh-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/.pre-commit-config.yaml` & `shillelagh-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/.readthedocs.yml` & `shillelagh-1.2.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/ARCHITECTURE.rst` & `shillelagh-1.2.9/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/CHANGELOG.rst` & `shillelagh-1.2.9/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 1.2.9 - 2023-11-08
+==========================
+
+- Improve Datasette detection (#399)
+- Fix generic JSON handling of null values (#399)
+- Add holidays adapter (#409)
+- Add support for decimals (#410)
+
 Version 1.2.8 - 2023-10-21
 ==========================
 
 - Add new cost model ``NetworkAPICostModel`` (#381)
 - Add a generic XML adapter (#391)
 
 Version 1.2.7 - 2023-08-14
```

### Comparing `shillelagh-1.2.8/CODE_OF_CONDUCT.md` & `shillelagh-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/CONTRIBUTING.rst` & `shillelagh-1.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/LICENSE.txt` & `shillelagh-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/Makefile` & `shillelagh-1.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/PKG-INFO` & `shillelagh-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.8
+Version: 1.2.9
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
@@ -17,14 +17,17 @@
            :target: https://shillelagh.readthedocs.io/en/latest/?badge=latest
            :alt: Documentation Status
         .. image:: https://badge.fury.io/py/shillelagh.svg
            :target: https://badge.fury.io/py/shillelagh
         .. image:: https://img.shields.io/pypi/pyversions/shillelagh
            :alt: PyPI - Python Version
         
+        .. image:: docs/logo.png
+           :width: 25 %
+        
         Shillelagh (ʃɪˈleɪlɪ) is a Python library and CLI that allows you to query many resources (APIs, files, in memory objects) using SQL. It's both user and developer friendly, making it trivial to access resources and easy to add support for new ones.
         
         Learn more on the `documentation <https://shillelagh.readthedocs.io/en/latest/>`_.
         
         The library is an implementation of the `Python DB API 2.0 <https://www.python.org/dev/peps/pep-0249/>`_ based on `SQLite <https://sqlite.org/index.html>`_ (using the `APSW <https://rogerbinns.github.io/apsw/>`_ library):
         
         .. code-block:: python
@@ -178,13 +181,14 @@
 Provides-Extra: docs
 Provides-Extra: console
 Provides-Extra: datasetteapi
 Provides-Extra: genericjsonapi
 Provides-Extra: genericxmlapi
 Provides-Extra: githubapi
 Provides-Extra: gsheetsapi
+Provides-Extra: holidaysmemory
 Provides-Extra: htmltableapi
 Provides-Extra: pandasmemory
 Provides-Extra: s3selectapi
 Provides-Extra: socrataapi
 Provides-Extra: systemapi
 Provides-Extra: weatherapi
```

### Comparing `shillelagh-1.2.8/README.rst` & `shillelagh-1.2.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,17 @@
    :target: https://shillelagh.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 .. image:: https://badge.fury.io/py/shillelagh.svg
    :target: https://badge.fury.io/py/shillelagh
 .. image:: https://img.shields.io/pypi/pyversions/shillelagh
    :alt: PyPI - Python Version
 
+.. image:: docs/logo.png
+   :width: 25 %
+
 Shillelagh (ʃɪˈleɪlɪ) is a Python library and CLI that allows you to query many resources (APIs, files, in memory objects) using SQL. It's both user and developer friendly, making it trivial to access resources and easy to add support for new ones.
 
 Learn more on the `documentation <https://shillelagh.readthedocs.io/en/latest/>`_.
 
 The library is an implementation of the `Python DB API 2.0 <https://www.python.org/dev/peps/pep-0249/>`_ based on `SQLite <https://sqlite.org/index.html>`_ (using the `APSW <https://rogerbinns.github.io/apsw/>`_ library):
 
 .. code-block:: python
```

### Comparing `shillelagh-1.2.8/docs/Makefile` & `shillelagh-1.2.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/docs/adapters.rst` & `shillelagh-1.2.9/docs/adapters.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/docs/conf.py` & `shillelagh-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/docs/development.rst` & `shillelagh-1.2.9/docs/development.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/docs/install.rst` & `shillelagh-1.2.9/docs/install.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/docs/usage.rst` & `shillelagh-1.2.9/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/examples/csvfile.py` & `shillelagh-1.2.9/examples/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/examples/dataframe.py` & `shillelagh-1.2.9/examples/dataframe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/examples/datasette.py` & `shillelagh-1.2.9/examples/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/examples/generic_json.py` & `shillelagh-1.2.9/examples/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/examples/weatherapi.py` & `shillelagh-1.2.9/examples/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/requirements/base.txt` & `shillelagh-1.2.9/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/requirements/test.txt` & `shillelagh-1.2.9/requirements/test.txt`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     # via shillelagh
 google-auth==2.9.1
     # via shillelagh
 greenlet==2.0.2
     # via
     #   shillelagh
     #   sqlalchemy
+holidays==0.35
+    # via shillelagh
 html5lib==1.1
     # via shillelagh
 identify==2.5.2
     # via pre-commit
 idna==3.3
     # via
     #   requests
@@ -147,14 +149,15 @@
     # via shillelagh
 pytest-mock==3.8.2
     # via shillelagh
 python-dateutil==2.8.2
     # via
     #   botocore
     #   freezegun
+    #   holidays
     #   pandas
     #   shillelagh
 pytz==2022.1
     # via pandas
 pyyaml==6.0
     # via
     #   pre-commit
```

### Comparing `shillelagh-1.2.8/setup.cfg` & `shillelagh-1.2.9/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 	beautifulsoup4>=4.11.1
 	boto3>=1.24.28
 	codespell>=2.1.0
 	defusedxml>=0.7.1
 	dill>=0.3.6
 	freezegun>=1.1.0
 	google-auth>=1.23.0
+	holidays>=0.35
 	html5lib>=1.1
 	jsonpath-python>=1.0.5
 	pandas>=1.2.2
 	pip-tools>=6.4.0
 	pre-commit>=2.13.0
 	prison>=0.2.1
 	prompt_toolkit>=3
@@ -78,14 +79,15 @@
 all = 
 	PyYAML>=5.4
 	appdirs>=1.4.4
 	beautifulsoup4>=4.11.1
 	boto3>=1.24.28
 	defusedxml>=0.7.1
 	google-auth>=1.23.0
+	holidays>=0.35
 	html5lib>=1.1
 	jsonpath-python>=1.0.5
 	pandas>=1.2.2
 	prison>=0.2.1
 	prompt_toolkit>=3
 	psutil>=5.8.0
 	pygments>=2.8
@@ -95,14 +97,15 @@
 docs = 
 	sphinx>=4.0.1
 console = 
 	PyYAML>=5.4
 	appdirs>=1.4.4
 	prompt_toolkit>=3
 	pygments>=2.8
+	requests-cache>=0.7.1
 	tabulate==0.8.9
 datasetteapi = 
 	requests-cache>=0.7.1
 genericjsonapi = 
 	jsonpath-python>=1.0.5
 	prison>=0.2.1
 	requests-cache>=0.7.1
@@ -112,14 +115,16 @@
 	prison>=0.2.1
 	requests-cache>=0.7.1
 	yarl>=1.8.1
 githubapi = 
 	jsonpath-python>=1.0.5
 gsheetsapi = 
 	google-auth>=1.23.0
+holidaysmemory = 
+	holidays>=0.35
 htmltableapi = 
 	beautifulsoup4>=4.11.1
 	html5lib>=1.1
 	pandas>=1.2.2
 pandasmemory = 
 	pandas>=1.2.2
 s3selectapi = 
@@ -135,14 +140,15 @@
 shillelagh.adapter = 
 	csvfile = shillelagh.adapters.file.csvfile:CSVFile
 	datasetteapi = shillelagh.adapters.api.datasette:DatasetteAPI
 	genericjsonapi = shillelagh.adapters.api.generic_json:GenericJSONAPI
 	genericxmlapi = shillelagh.adapters.api.generic_xml:GenericXMLAPI
 	githubapi = shillelagh.adapters.api.github:GitHubAPI
 	gsheetsapi = shillelagh.adapters.api.gsheets.adapter:GSheetsAPI
+	holidaysmemory = shillelagh.adapters.memory.holidays:HolidaysMemory
 	htmltableapi = shillelagh.adapters.api.html_table:HTMLTableAPI
 	pandasmemory = shillelagh.adapters.memory.pandas:PandasMemory
 	s3selectapi = shillelagh.adapters.api.s3select:S3SelectAPI
 	socrataapi = shillelagh.adapters.api.socrata:SocrataAPI
 	systemapi = shillelagh.adapters.api.system:SystemAPI
 	weatherapi = shillelagh.adapters.api.weatherapi:WeatherAPI
 sqlalchemy.dialects =
```

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/datasette.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/datasette.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,36 +2,38 @@
 An adapter to Datasette instances.
 
 See https://datasette.io/ for more information.
 """
 
 import logging
 import urllib.parse
+from datetime import timedelta
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Type, cast
 
 import dateutil.parser
-import requests_cache
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.fields import Field, Float, Integer, ISODate, ISODateTime, Order, String
 from shillelagh.filters import Equal, Filter, IsNotNull, IsNull, Like, NotEqual, Range
-from shillelagh.lib import SimpleCostModel, build_sql
+from shillelagh.lib import SimpleCostModel, build_sql, get_session
 from shillelagh.typing import RequestedOrder, Row
 
 _logger = logging.getLogger(__name__)
 
 KNOWN_DOMAINS = {"datasette.io", "datasettes.com"}
 
 # this is just a wild guess; used to estimate query cost
 AVERAGE_NUMBER_OF_ROWS = 1000
 
 # how many rows to get when performing our own pagination
 DEFAULT_LIMIT = 1000
 
+CACHE_EXPIRATION = timedelta(minutes=3)
+
 
 def is_known_domain(netloc: str) -> bool:
     """
     Identify well known Datasette domains.
     """
     for domain in KNOWN_DOMAINS:
         if netloc == domain or netloc.endswith("." + domain):
@@ -49,22 +51,22 @@
         mountpoint, database, table = parsed.path.rsplit("/", 2)
     except ValueError:
         return False
 
     parsed = parsed._replace(path=f"{mountpoint}/-/versions.json")
     uri = urllib.parse.urlunparse(parsed)
 
-    session = requests_cache.CachedSession(
-        cache_name="datasette_cache",
-        backend="sqlite",
-        expire_after=180,
-    )
+    session = get_session({}, "datasette_cache", CACHE_EXPIRATION)
+    response = session.get(uri)
+    try:
+        payload = response.json()
+    except Exception:  # pylint: disable=broad-exception-caught
+        return False
 
-    response = session.head(uri)
-    return cast(bool, response.ok)
+    return "datasette" in payload
 
 
 def get_field(value: Any) -> Field:
     """
     Return a Shillelagh ``Field`` based on the value type.
     """
     class_: Type[Field] = String
@@ -118,19 +120,15 @@
         super().__init__()
 
         self.server_url = server_url
         self.database = database
         self.table = table
 
         # use a cache for the API requests
-        self._session = requests_cache.CachedSession(
-            cache_name="datasette_cache",
-            backend="sqlite",
-            expire_after=180,
-        )
+        self._session = get_session({}, "datasette_cache", CACHE_EXPIRATION)
 
         self._set_columns()
 
     def _run_query(self, sql: str) -> Dict[str, Any]:
         """
         Run a query and return the JSON payload.
         """
```

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/generic_json.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/generic_json.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,13 +136,13 @@
         if not response.ok:
             raise ProgrammingError(f'Error: {payload["message"]}')
 
         parser = JSONPath(self.path)
         for i, row in enumerate(parser.parse(payload)):
             row = {
                 k: v
-                for k, v in row.items()
+                for k, v in (row or {}).items()
                 if requested_columns is None or k in requested_columns
             }
             row["rowid"] = i
             _logger.debug(row)
             yield flatten(row)
```

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/generic_xml.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/generic_xml.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/github.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/github.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/adapter.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/adapter.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/fields.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/lib.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/parsing/base.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/parsing/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/parsing/date.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/parsing/date.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/parsing/number.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/parsing/number.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/types.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/gsheets/typing.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/gsheets/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/html_table.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/html_table.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/s3select.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/s3select.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/socrata.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/socrata.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/system.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/system.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/api/weatherapi.py` & `shillelagh-1.2.9/src/shillelagh/adapters/api/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/base.py` & `shillelagh-1.2.9/src/shillelagh/adapters/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/file/csvfile.py` & `shillelagh-1.2.9/src/shillelagh/adapters/file/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/memory/pandas.py` & `shillelagh-1.2.9/src/shillelagh/adapters/memory/pandas.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/adapters/registry.py` & `shillelagh-1.2.9/src/shillelagh/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/backends/apsw/db.py` & `shillelagh-1.2.9/src/shillelagh/backends/apsw/db.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/backends/apsw/dialects/base.py` & `shillelagh-1.2.9/src/shillelagh/backends/apsw/dialects/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/backends/apsw/dialects/gsheets.py` & `shillelagh-1.2.9/src/shillelagh/backends/apsw/dialects/gsheets.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/backends/apsw/dialects/safe.py` & `shillelagh-1.2.9/src/shillelagh/backends/apsw/dialects/safe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/backends/apsw/vt.py` & `shillelagh-1.2.9/src/shillelagh/backends/apsw/vt.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     Float,
     IntBoolean,
     ISODate,
     ISOTime,
     Order,
     RowID,
     String,
+    StringDecimal,
     StringDuration,
     StringInteger,
 )
 from shillelagh.filters import Filter, Operator
 from shillelagh.lib import best_index_object_available, deserialize
 from shillelagh.typing import (
     Constraint,
@@ -100,22 +101,23 @@
 
 # map for converting between Python native types (boolean, datetime, etc.)
 # and types understood by SQLite (integers, strings, etc.)
 type_map: Dict[str, Type[Field]] = {
     field.type: field  # type: ignore
     for field in [
         Blob,
-        StringDuration,
+        FastISODateTime,
         Float,
-        IntBoolean,
-        StringInteger,
         ISODate,
-        FastISODateTime,
         ISOTime,
+        IntBoolean,
         String,
+        StringDecimal,
+        StringDuration,
+        StringInteger,
     ]
 }
 
 
 # a row with only SQLite-valid types
 SQLiteRow = Dict[str, SQLiteValidType]
```

### Comparing `shillelagh-1.2.8/src/shillelagh/console.py` & `shillelagh-1.2.9/src/shillelagh/console.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/exceptions.py` & `shillelagh-1.2.9/src/shillelagh/exceptions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/fields.py` & `shillelagh-1.2.9/src/shillelagh/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Fields representing columns of different types and capabilities.
 """
 import datetime
+import decimal
 from enum import Enum
 from typing import Any, Collection, Generic, Optional, Type, TypeVar, Union, cast
 
 import dateutil.parser
 
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.filters import Filter
@@ -19,14 +20,15 @@
         int,
         str,
         bool,
         datetime.date,
         datetime.datetime,
         datetime.time,
         datetime.timedelta,
+        decimal.Decimal,
         bytes,
     ],
 )
 
 
 class Order(Enum):
     """An enum for different orders a field can have."""
@@ -734,7 +736,31 @@
             return None
         return 1 if value else 0
 
     def quote(self, value: Optional[int]) -> str:
         if value is None:
             return "NULL"
         return str(value)
+
+
+class StringDecimal(Field[str, decimal.Decimal]):
+    """
+    Decimals as strings.
+    """
+
+    type = "DECIMAL"
+    db_api_type = "NUMBER"
+
+    def parse(self, value: Optional[str]) -> Optional[decimal.Decimal]:
+        if value is None:
+            return None
+        return decimal.Decimal(value)
+
+    def format(self, value: Optional[decimal.Decimal]) -> Optional[str]:
+        if value is None:
+            return None
+        return str(value)
+
+    def quote(self, value: Optional[str]) -> str:
+        if value is None:
+            return "NULL"
+        return value
```

### Comparing `shillelagh-1.2.8/src/shillelagh/filters.py` & `shillelagh-1.2.9/src/shillelagh/filters.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/functions.py` & `shillelagh-1.2.9/src/shillelagh/functions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/lib.py` & `shillelagh-1.2.9/src/shillelagh/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/types.py` & `shillelagh-1.2.9/src/shillelagh/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh/typing.py` & `shillelagh-1.2.9/src/shillelagh/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/src/shillelagh.egg-info/PKG-INFO` & `shillelagh-1.2.9/src/shillelagh.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.8
+Version: 1.2.9
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
@@ -17,14 +17,17 @@
            :target: https://shillelagh.readthedocs.io/en/latest/?badge=latest
            :alt: Documentation Status
         .. image:: https://badge.fury.io/py/shillelagh.svg
            :target: https://badge.fury.io/py/shillelagh
         .. image:: https://img.shields.io/pypi/pyversions/shillelagh
            :alt: PyPI - Python Version
         
+        .. image:: docs/logo.png
+           :width: 25 %
+        
         Shillelagh (ʃɪˈleɪlɪ) is a Python library and CLI that allows you to query many resources (APIs, files, in memory objects) using SQL. It's both user and developer friendly, making it trivial to access resources and easy to add support for new ones.
         
         Learn more on the `documentation <https://shillelagh.readthedocs.io/en/latest/>`_.
         
         The library is an implementation of the `Python DB API 2.0 <https://www.python.org/dev/peps/pep-0249/>`_ based on `SQLite <https://sqlite.org/index.html>`_ (using the `APSW <https://rogerbinns.github.io/apsw/>`_ library):
         
         .. code-block:: python
@@ -178,13 +181,14 @@
 Provides-Extra: docs
 Provides-Extra: console
 Provides-Extra: datasetteapi
 Provides-Extra: genericjsonapi
 Provides-Extra: genericxmlapi
 Provides-Extra: githubapi
 Provides-Extra: gsheetsapi
+Provides-Extra: holidaysmemory
 Provides-Extra: htmltableapi
 Provides-Extra: pandasmemory
 Provides-Extra: s3selectapi
 Provides-Extra: socrataapi
 Provides-Extra: systemapi
 Provides-Extra: weatherapi
```

### Comparing `shillelagh-1.2.8/src/shillelagh.egg-info/SOURCES.txt` & `shillelagh-1.2.9/src/shillelagh.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/development.rst
 docs/index.rst
 docs/install.rst
 docs/license.rst
+docs/logo.png
 docs/requirements.txt
 docs/usage.rst
 docs/_static/.gitignore
 examples/csvfile.py
 examples/dataframe.py
 examples/datasette.py
 examples/generic_json.py
@@ -92,14 +93,15 @@
 src/shillelagh/adapters/api/gsheets/parsing/__init__.py
 src/shillelagh/adapters/api/gsheets/parsing/base.py
 src/shillelagh/adapters/api/gsheets/parsing/date.py
 src/shillelagh/adapters/api/gsheets/parsing/number.py
 src/shillelagh/adapters/file/__init__.py
 src/shillelagh/adapters/file/csvfile.py
 src/shillelagh/adapters/memory/__init__.py
+src/shillelagh/adapters/memory/holidays.py
 src/shillelagh/adapters/memory/pandas.py
 src/shillelagh/backends/__init__.py
 src/shillelagh/backends/apsw/__init__.py
 src/shillelagh/backends/apsw/db.py
 src/shillelagh/backends/apsw/vt.py
 src/shillelagh/backends/apsw/dialects/__init__.py
 src/shillelagh/backends/apsw/dialects/base.py
@@ -139,14 +141,15 @@
 tests/adapters/api/gsheets/parsing/__init__.py
 tests/adapters/api/gsheets/parsing/base_test.py
 tests/adapters/api/gsheets/parsing/date_test.py
 tests/adapters/api/gsheets/parsing/number_test.py
 tests/adapters/file/__init__.py
 tests/adapters/file/csvfile_test.py
 tests/adapters/memory/__init__.py
+tests/adapters/memory/holidays_test.py
 tests/adapters/memory/pandas_test.py
 tests/backends/__init__.py
 tests/backends/apsw/__init__.py
 tests/backends/apsw/db_test.py
 tests/backends/apsw/dbapi_test.py
 tests/backends/apsw/vt_test.py
 tests/backends/apsw/dialects/__init__.py
```

### Comparing `shillelagh-1.2.8/src/shillelagh.egg-info/entry_points.txt` & `shillelagh-1.2.9/src/shillelagh.egg-info/entry_points.txt`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 [shillelagh.adapter]
 csvfile = shillelagh.adapters.file.csvfile:CSVFile
 datasetteapi = shillelagh.adapters.api.datasette:DatasetteAPI
 genericjsonapi = shillelagh.adapters.api.generic_json:GenericJSONAPI
 genericxmlapi = shillelagh.adapters.api.generic_xml:GenericXMLAPI
 githubapi = shillelagh.adapters.api.github:GitHubAPI
 gsheetsapi = shillelagh.adapters.api.gsheets.adapter:GSheetsAPI
+holidaysmemory = shillelagh.adapters.memory.holidays:HolidaysMemory
 htmltableapi = shillelagh.adapters.api.html_table:HTMLTableAPI
 pandasmemory = shillelagh.adapters.memory.pandas:PandasMemory
 s3selectapi = shillelagh.adapters.api.s3select:S3SelectAPI
 socrataapi = shillelagh.adapters.api.socrata:SocrataAPI
 systemapi = shillelagh.adapters.api.system:SystemAPI
 weatherapi = shillelagh.adapters.api.weatherapi:WeatherAPI
```

### Comparing `shillelagh-1.2.8/src/shillelagh.egg-info/requires.txt` & `shillelagh-1.2.9/src/shillelagh.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 [all]
 PyYAML>=5.4
 appdirs>=1.4.4
 beautifulsoup4>=4.11.1
 boto3>=1.24.28
 defusedxml>=0.7.1
 google-auth>=1.23.0
+holidays>=0.35
 html5lib>=1.1
 jsonpath-python>=1.0.5
 pandas>=1.2.2
 prison>=0.2.1
 prompt_toolkit>=3
 psutil>=5.8.0
 pygments>=2.8
@@ -28,14 +29,15 @@
 yarl>=1.8.1
 
 [console]
 PyYAML>=5.4
 appdirs>=1.4.4
 prompt_toolkit>=3
 pygments>=2.8
+requests-cache>=0.7.1
 tabulate==0.8.9
 
 [datasetteapi]
 requests-cache>=0.7.1
 
 [docs]
 sphinx>=4.0.1
@@ -54,14 +56,17 @@
 
 [githubapi]
 jsonpath-python>=1.0.5
 
 [gsheetsapi]
 google-auth>=1.23.0
 
+[holidaysmemory]
+holidays>=0.35
+
 [htmltableapi]
 beautifulsoup4>=4.11.1
 html5lib>=1.1
 pandas>=1.2.2
 
 [pandasmemory]
 pandas>=1.2.2
@@ -81,14 +86,15 @@
 beautifulsoup4>=4.11.1
 boto3>=1.24.28
 codespell>=2.1.0
 defusedxml>=0.7.1
 dill>=0.3.6
 freezegun>=1.1.0
 google-auth>=1.23.0
+holidays>=0.35
 html5lib>=1.1
 jsonpath-python>=1.0.5
 pandas>=1.2.2
 pip-tools>=6.4.0
 pre-commit>=2.13.0
 prison>=0.2.1
 prompt_toolkit>=3
```

### Comparing `shillelagh-1.2.8/talks/Python Brasil 2021.pdf` & `shillelagh-1.2.9/talks/Python Brasil 2021.pdf`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py` & `shillelagh-1.2.9/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py` & `shillelagh-1.2.9/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/datasette_test.py` & `shillelagh-1.2.9/tests/adapters/api/datasette_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # pylint: disable=too-many-lines
 """
 Tests for the Datasette adapter.
 """
+from datetime import timedelta
+
 import pytest
 from pytest_mock import MockerFixture
-from requests import Session
 from requests_mock.mocker import Mocker
 
 from shillelagh.adapters.api.datasette import (
     DatasetteAPI,
     get_field,
     is_datasette,
     is_known_domain,
@@ -21,23 +22,22 @@
     datasette_columns_response,
     datasette_data_response_1,
     datasette_data_response_2,
     datasette_metadata_response,
     datasette_results,
 )
 
+DO_NOT_CACHE = timedelta(seconds=-1)
+
 
 def test_datasette(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test a simple query.
     """
-    mocker.patch(
-        "shillelagh.adapters.api.datasette.requests_cache.CachedSession",
-        return_value=Session(),
-    )
+    mocker.patch("shillelagh.adapters.api.datasette.CACHE_EXPIRATION", DO_NOT_CACHE)
 
     columns_url = (
         "https://global-power-plants.datasettes.com/global-power-plants.json?"
         "sql=SELECT+*+FROM+%22global-power-plants%22+LIMIT+0"
     )
     requests_mock.get(columns_url, json=datasette_columns_response)
     metadata_url = (
@@ -94,18 +94,15 @@
     assert data == datasette_results
 
 
 def test_datasette_limit_offset(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test a simple query with limit/offset.
     """
-    mocker.patch(
-        "shillelagh.adapters.api.datasette.requests_cache.CachedSession",
-        return_value=Session(),
-    )
+    mocker.patch("shillelagh.adapters.api.datasette.CACHE_EXPIRATION", DO_NOT_CACHE)
 
     columns_url = (
         "https://global-power-plants.datasettes.com/global-power-plants.json?"
         "sql=SELECT+*+FROM+%22global-power-plants%22+LIMIT+0"
     )
     requests_mock.get(columns_url, json=datasette_columns_response)
     metadata_url = (
@@ -179,18 +176,16 @@
     assert data == datasette_results
 
 
 def test_datasette_no_data(mocker: MockerFixture) -> None:
     """
     Test result with no rows.
     """
-    CachedSession = mocker.patch(  # pylint: disable=invalid-name
-        "shillelagh.adapters.api.datasette.requests_cache.CachedSession",
-    )
-    CachedSession.return_value.get.return_value.json.return_value = {
+    get_session = mocker.patch("shillelagh.adapters.api.datasette.get_session")
+    get_session().get().json.return_value = {
         "columns": [],
         "rows": [],
     }
 
     with pytest.raises(ProgrammingError) as excinfo:
         DatasetteAPI("https://example.com", "database", "table")
     assert str(excinfo.value) == 'Table "table" has no data'
@@ -239,21 +234,23 @@
     Test ``is_known_domain``.
     """
     assert is_known_domain("latest.datasette.io")
     assert is_known_domain("san-francisco.datasettes.com")
     assert not is_known_domain("example.com")
 
 
-def test_is_datasette(requests_mock: Mocker) -> None:
+def test_is_datasette(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test ``is_datasette``.
     """
+    mocker.patch("shillelagh.adapters.api.datasette.CACHE_EXPIRATION", DO_NOT_CACHE)
+
     assert not is_datasette("https://example.com/")
 
-    requests_mock.head(
+    requests_mock.get(
         "https://example.com/-/versions.json",
         json={
             "python": {
                 "version": "3.8.11",
                 "full": "3.8.11 (default, Aug 17 2021, 15:56:41) \n[GCC 10.2.1 20210110]",
             },
             "datasette": {
@@ -287,23 +284,26 @@
                 ],
             },
             "pysqlite3": "0.4.6",
         },
     )
     assert is_datasette("https://example.com/database/table")
 
+    requests_mock.get(
+        "https://example.com/-/versions.json",
+        text="Invalid page",
+    )
+    assert not is_datasette("https://example.com/database/table")
+
 
 def test_datasette_error(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test error handling.
     """
-    mocker.patch(
-        "shillelagh.adapters.api.datasette.requests_cache.CachedSession",
-        return_value=Session(),
-    )
+    mocker.patch("shillelagh.adapters.api.datasette.CACHE_EXPIRATION", DO_NOT_CACHE)
 
     columns_url = (
         "https://global-power-plants.datasettes.com/global-power-plants.json?"
         "sql=SELECT+*+FROM+%22global-power-plants%22+LIMIT+0"
     )
     requests_mock.get(columns_url, json=datasette_columns_response)
     metadata_url = (
```

### Comparing `shillelagh-1.2.8/tests/adapters/api/generic_json_test.py` & `shillelagh-1.2.9/tests/adapters/api/generic_json_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Test the generic JSON adapter.
 """
 
+import re
 from datetime import timedelta
 
 import pytest
 from pytest_mock import MockerFixture
 from requests_mock.mocker import Mocker
 from yarl import URL
 
@@ -21,22 +22,16 @@
 
 def test_generic_json(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test a simple query.
     """
     mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", DO_NOT_CACHE)
 
-    # for datassette and other probing adapters
-    requests_mock.head(
-        "https://api.stlouisfed.org/-/versions.json?"
-        "series_id=GNPCA&"
-        "api_key=abcdefghijklmnopqrstuvwxyz123456&"
-        "file_type=json#$.seriess%5B*%5D",
-        status_code=404,
-    )
+    # for datassette
+    requests_mock.get(re.compile(".*-/versions.json.*"), status_code=404)
 
     params = {
         "series_id": "GNPCA",
         "api_key": "abcdefghijklmnopqrstuvwxyz123456",
         "file_type": "json",
     }
     url = (baseurl % params).with_fragment("$.seriess[*]")
```

### Comparing `shillelagh-1.2.8/tests/adapters/api/generic_xml_test.py` & `shillelagh-1.2.9/tests/adapters/api/generic_xml_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,16 @@
 
 def test_generic_xml(mocker: MockerFixture, requests_mock: Mocker) -> None:
     """
     Test a simple query.
     """
     mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", DO_NOT_CACHE)
 
-    requests_mock.head(re.compile(".*-/versions.json.*"), status_code=404)
+    # for datassette
+    requests_mock.get(re.compile(".*-/versions.json.*"), status_code=404)
 
     params = {
         "format": "Xml",
         "offset": 0,
         "limit": 2,
         "api_key": "SECRET",
     }
```

### Comparing `shillelagh-1.2.8/tests/adapters/api/github_test.py` & `shillelagh-1.2.9/tests/adapters/api/github_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/gsheets/adapter_test.py` & `shillelagh-1.2.9/tests/adapters/api/gsheets/adapter_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/gsheets/fields_test.py` & `shillelagh-1.2.9/tests/adapters/api/gsheets/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/gsheets/integration_test.py` & `shillelagh-1.2.9/tests/adapters/api/gsheets/integration_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/gsheets/lib_test.py` & `shillelagh-1.2.9/tests/adapters/api/gsheets/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/gsheets/parsing/base_test.py` & `shillelagh-1.2.9/tests/adapters/api/gsheets/parsing/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/gsheets/parsing/date_test.py` & `shillelagh-1.2.9/tests/adapters/api/gsheets/parsing/date_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/gsheets/parsing/number_test.py` & `shillelagh-1.2.9/tests/adapters/api/gsheets/parsing/number_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/html_table_test.py` & `shillelagh-1.2.9/tests/adapters/api/html_table_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/s3select_test.py` & `shillelagh-1.2.9/tests/adapters/api/s3select_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/socrata_test.py` & `shillelagh-1.2.9/tests/adapters/api/socrata_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/system_test.py` & `shillelagh-1.2.9/tests/adapters/api/system_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/api/weatherapi_test.py` & `shillelagh-1.2.9/tests/adapters/api/weatherapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/base_test.py` & `shillelagh-1.2.9/tests/adapters/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/file/csvfile_test.py` & `shillelagh-1.2.9/tests/adapters/file/csvfile_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/memory/pandas_test.py` & `shillelagh-1.2.9/tests/adapters/memory/pandas_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/adapters/registry_test.py` & `shillelagh-1.2.9/tests/adapters/registry_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/backends/apsw/db_test.py` & `shillelagh-1.2.9/tests/backends/apsw/db_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/backends/apsw/dbapi_test.py` & `shillelagh-1.2.9/tests/backends/apsw/dbapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/backends/apsw/dialects/base_test.py` & `shillelagh-1.2.9/tests/backends/apsw/dialects/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/backends/apsw/dialects/gsheets_test.py` & `shillelagh-1.2.9/tests/backends/apsw/dialects/gsheets_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/backends/apsw/dialects/safe_test.py` & `shillelagh-1.2.9/tests/backends/apsw/dialects/safe_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/backends/apsw/vt_test.py` & `shillelagh-1.2.9/tests/backends/apsw/vt_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/conftest.py` & `shillelagh-1.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/console_test.py` & `shillelagh-1.2.9/tests/console_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/__init__.py` & `shillelagh-1.2.9/tests/fakes/__init__.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/cdc_data_response.json` & `shillelagh-1.2.9/tests/fakes/cdc_data_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/cdc_metadata_response.json` & `shillelagh-1.2.9/tests/fakes/cdc_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/datasette_columns_response.json` & `shillelagh-1.2.9/tests/fakes/datasette_columns_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/datasette_data_response_1.json` & `shillelagh-1.2.9/tests/fakes/datasette_data_response_1.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/datasette_data_response_2.json` & `shillelagh-1.2.9/tests/fakes/datasette_data_response_2.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/datasette_metadata_response.json` & `shillelagh-1.2.9/tests/fakes/datasette_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/datasette_results.json` & `shillelagh-1.2.9/tests/fakes/datasette_results.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/github_response.json` & `shillelagh-1.2.9/tests/fakes/github_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/github_single_response.json` & `shillelagh-1.2.9/tests/fakes/github_single_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/incidents.json` & `shillelagh-1.2.9/tests/fakes/incidents.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fakes/weatherapi_response.json` & `shillelagh-1.2.9/tests/fakes/weatherapi_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/fields_test.py` & `shillelagh-1.2.9/tests/fields_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tests for shillelagh.fields.
 """
 import datetime
+import decimal
 import sys
 from typing import Union
 
 import pytest
 
 from shillelagh.adapters.registry import registry
 from shillelagh.backends.apsw.db import connect
@@ -25,14 +26,15 @@
     ISOTime,
     Order,
     String,
     StringBlob,
     StringBoolean,
     StringDate,
     StringDateTime,
+    StringDecimal,
     StringDuration,
     StringTime,
     Time,
 )
 from shillelagh.filters import Equal
 from shillelagh.types import BINARY, DATETIME, NUMBER, STRING
 
@@ -505,7 +507,19 @@
         with pytest.raises(ProgrammingError) as excinfo:
             FastISODateTime().parse("2020-01-01T12:00Z")
         assert str(excinfo.value) == 'Unable to parse "2020-01-01T12:00Z"'
 
     with pytest.raises(ProgrammingError) as excinfo:
         FastISODateTime().parse("invalid")
     assert str(excinfo.value) == 'Unable to parse "invalid"'
+
+
+def test_stringdecimal() -> None:
+    """
+    Test ``StringDecimal``.
+    """
+    assert StringDecimal().parse("1.23") == decimal.Decimal("1.23")
+    assert StringDecimal().parse(None) is None
+    assert StringDecimal().format(decimal.Decimal("1.23")) == "1.23"
+    assert StringDecimal().format(None) is None
+    assert StringDecimal().quote("1.23") == "1.23"
+    assert StringDecimal().quote(None) == "NULL"
```

### Comparing `shillelagh-1.2.8/tests/filters_test.py` & `shillelagh-1.2.9/tests/filters_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/functions_test.py` & `shillelagh-1.2.9/tests/functions_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/lib_test.py` & `shillelagh-1.2.9/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.8/tests/types_test.py` & `shillelagh-1.2.9/tests/types_test.py`

 * *Files identical despite different names*

