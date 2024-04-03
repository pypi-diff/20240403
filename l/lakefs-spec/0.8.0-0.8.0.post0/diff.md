# Comparing `tmp/lakefs-spec-0.8.0.tar.gz` & `tmp/lakefs-spec-0.8.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lakefs-spec-0.8.0.tar", last modified: Tue Apr  2 08:38:52 2024, max compression
+gzip compressed data, was "lakefs-spec-0.8.0.post0.tar", last modified: Wed Apr  3 10:23:13 2024, max compression
```

## Comparing `lakefs-spec-0.8.0.tar` & `lakefs-spec-0.8.0.post0.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/bug-report.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/feature-request.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.838780 lakefs-spec-0.8.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/actions/mike-docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/actions/mike-docs/action.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/actions/python-deps/
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/actions/python-deps/action.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/pull-request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/workflows/python.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/assets/lakefs-spec-logo-all.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.842780 lakefs-spec-0.8.0/docs/_code/
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/duckdb_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/pandas_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/polars_example.py
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/pyarrow_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_code/quickstart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_images/
--rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/aai-favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    26004 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/aai-logo-cropped.png
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/lakefs-spec-favicon.png
--rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/lakefs-spec-logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    31995 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/lakefs-spec-logo-light.png
--rw-r--r--   0 runner    (1001) docker     (127)    40636 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-repositories.png
--rw-r--r--   0 runner    (1001) docker     (127)   123174 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-sample-repo.png
--rw-r--r--   0 runner    (1001) docker     (127)    32617 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-ui.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_scripts/gen_api_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_scripts/jupytext_convert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_styles/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_styles/extra.css
--rw-r--r--   0 runner    (1001) docker     (127)    41136 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_styles/neoteroi-mkdocs.css
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_styles/theme.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_theme_overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_theme_overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/_theme_overrides/partials/
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/_theme_overrides/partials/header.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/configuration.md
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/filesystem-usage.md
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/integrations.md
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/guides/transactions.md
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/tutorials/.lakectl.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/tutorials/demo_data_science_project.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/docs/tutorials/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/hack/
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.846780 lakefs-spec-0.8.0/hack/config/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/config/s3.json
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/lakefs-s3-local.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/hack/lock-deps.sh
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.838780 lakefs-spec-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.850780 lakefs-spec-0.8.0/src/lakefs_spec/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    30309 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/src/lakefs_spec/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 08:38:52.000000 lakefs-spec-0.8.0/src/lakefs_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 08:38:52.854780 lakefs-spec-0.8.0/tests/smoke_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/smoke_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/smoke_tests/test_abstractfilesystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/smoke_tests/test_integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_copy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_get_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_internals.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_lakefs_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_put_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_rm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_spec_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-02 08:37:50.000000 lakefs-spec-0.8.0/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.792932 lakefs-spec-0.8.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.772932 lakefs-spec-0.8.0.post0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/bug-report.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/feature-request.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.772932 lakefs-spec-0.8.0.post0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/.github/actions/mike-docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/actions/mike-docs/action.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/.github/actions/python-deps/
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/actions/python-deps/action.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/pull-request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/workflows/python.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-03 10:23:13.792932 lakefs-spec-0.8.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    14056 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/assets/lakefs-spec-logo-all.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.776932 lakefs-spec-0.8.0.post0/docs/_code/
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/duckdb_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/hf_datasets_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/pandas_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/polars_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/pyarrow_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_code/quickstart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_images/
+-rw-r--r--   0 runner    (1001) docker     (127)    12318 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/aai-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    26004 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/aai-logo-cropped.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31995 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-logo-light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40636 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-repositories.png
+-rw-r--r--   0 runner    (1001) docker     (127)   123174 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-sample-repo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32617 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-ui.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_scripts/gen_api_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_scripts/jupytext_convert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_styles/extra.css
+-rw-r--r--   0 runner    (1001) docker     (127)    41136 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_styles/neoteroi-mkdocs.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_styles/theme.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_theme_overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_theme_overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/_theme_overrides/partials/
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/_theme_overrides/partials/header.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (127)     4324 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/filesystem-usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6001 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/integrations.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/guides/transactions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.780932 lakefs-spec-0.8.0.post0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/tutorials/.lakectl.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16283 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/tutorials/demo_data_science_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/docs/tutorials/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.784932 lakefs-spec-0.8.0.post0/hack/
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.784932 lakefs-spec-0.8.0.post0/hack/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/config/s3.json
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/lakefs-s3-local.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      429 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/hack/lock-deps.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 10:23:13.792932 lakefs-spec-0.8.0.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.772932 lakefs-spec-0.8.0.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.784932 lakefs-spec-0.8.0.post0/src/lakefs_spec/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    30309 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9153 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.788932 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 10:23:13.000000 lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.788932 lakefs-spec-0.8.0.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 10:23:13.788932 lakefs-spec-0.8.0.post0/tests/smoke_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/smoke_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6771 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/smoke_tests/test_abstractfilesystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/smoke_tests/test_integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_get_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_internals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_lakefs_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2527 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_put_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_rm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_spec_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-03 10:22:17.000000 lakefs-spec-0.8.0.post0/tests/util.py
```

### Comparing `lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/bug-report.yaml` & `lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/bug-report.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/.github/ISSUE_TEMPLATE/feature-request.yaml` & `lakefs-spec-0.8.0.post0/.github/ISSUE_TEMPLATE/feature-request.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/.github/actions/mike-docs/action.yaml` & `lakefs-spec-0.8.0.post0/.github/actions/mike-docs/action.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/.github/actions/python-deps/action.yaml` & `lakefs-spec-0.8.0.post0/.github/actions/python-deps/action.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/.github/workflows/python.yaml` & `lakefs-spec-0.8.0.post0/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/.github/workflows/release.yaml` & `lakefs-spec-0.8.0.post0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/.gitignore` & `lakefs-spec-0.8.0.post0/.gitignore`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/.pre-commit-config.yaml` & `lakefs-spec-0.8.0.post0/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,28 @@
       - id: check-json
       - id: check-toml
       - id: check-yaml
         exclude: "mkdocs.yml"
       - id: end-of-file-fixer
       - id: mixed-line-ending
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.8.0
+    rev: v1.9.0
     hooks:
       # See https://github.com/pre-commit/mirrors-mypy/blob/main/.pre-commit-hooks.yaml
       - id: mypy
         types_or: [python, pyi]
         args: [--ignore-missing-imports, --scripts-are-modules]
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.1
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.7
+    rev: 1.7.8
     hooks:
       - id: bandit
         args: [-c, pyproject.toml]
         additional_dependencies: ["bandit[toml]"]
   - repo: https://github.com/jsh9/pydoclint
     rev: 0.4.1
     hooks:
```

### Comparing `lakefs-spec-0.8.0/CONTRIBUTING.md` & `lakefs-spec-0.8.0.post0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/LICENSE` & `lakefs-spec-0.8.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/PKG-INFO` & `lakefs-spec-0.8.0.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-spec
-Version: 0.8.0
+Version: 0.8.0.post0
 Summary: An fsspec implementation for lakeFS.
 Author-email: appliedAI Institute for Europe <lakefs-spec@appliedai-institute.de>
 Maintainer-email: Nicholas Junge <n.junge@appliedai-institute.de>, Max Mynter <m.mynter@appliedai-institute.de>, Adrian Rumpold <a.rumpold@appliedai-institute.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/aai-institute/lakefs-spec
 Project-URL: Repository, https://github.com/aai-institute/lakefs-spec.git
 Project-URL: Issues, https://github.com/aai-institute/lakefs-spec/issues
@@ -72,15 +72,15 @@
 Our primary goal is to streamline versioned data operations in lakeFS, enabling seamless integration with popular data science tools such as Pandas, Polars, and DuckDB directly from Python.
 
 Highlights:
 
 - Simple repository operations in lakeFS
 - Easy access to underlying storage and versioning operations
 - Seamless integration with the fsspec ecosystem
-- Directly access lakeFS objects from popular data science libraries (including Pandas, Polars, DuckDB, PyArrow) with minimal code
+- Directly access lakeFS objects from popular data science libraries (including Pandas, Polars, DuckDB, Hugging Face Datasets, PyArrow) with minimal code
 - Transaction support for reliable data version control
 - Smart data transfers through client-side caching (up-/download)
 - Auto-discovery configuration
 
 > [!NOTE]
 > We are seeking early adopters who would like to actively participate in our feedback process and shape the future of the library.
 If you are interested in using the library and want to get in touch with us, please reach out via [Github Discussions](https://github.com/aai-institute/lakefs-spec/discussions).
```

### Comparing `lakefs-spec-0.8.0/README.md` & `lakefs-spec-0.8.0.post0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Our primary goal is to streamline versioned data operations in lakeFS, enabling seamless integration with popular data science tools such as Pandas, Polars, and DuckDB directly from Python.
 
 Highlights:
 
 - Simple repository operations in lakeFS
 - Easy access to underlying storage and versioning operations
 - Seamless integration with the fsspec ecosystem
-- Directly access lakeFS objects from popular data science libraries (including Pandas, Polars, DuckDB, PyArrow) with minimal code
+- Directly access lakeFS objects from popular data science libraries (including Pandas, Polars, DuckDB, Hugging Face Datasets, PyArrow) with minimal code
 - Transaction support for reliable data version control
 - Smart data transfers through client-side caching (up-/download)
 - Auto-discovery configuration
 
 > [!NOTE]
 > We are seeking early adopters who would like to actively participate in our feedback process and shape the future of the library.
 If you are interested in using the library and want to get in touch with us, please reach out via [Github Discussions](https://github.com/aai-institute/lakefs-spec/discussions).
```

### Comparing `lakefs-spec-0.8.0/assets/lakefs-spec-logo-all.svg` & `lakefs-spec-0.8.0.post0/assets/lakefs-spec-logo-all.svg`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/CONTRIBUTING.md` & `lakefs-spec-0.8.0.post0/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_code/pyarrow_example.py` & `lakefs-spec-0.8.0.post0/docs/_code/pyarrow_example.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_code/quickstart.py` & `lakefs-spec-0.8.0.post0/docs/_code/quickstart.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_images/aai-favicon.png` & `lakefs-spec-0.8.0.post0/docs/_images/aai-favicon.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_images/aai-logo-cropped.png` & `lakefs-spec-0.8.0.post0/docs/_images/aai-logo-cropped.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_images/lakefs-spec-favicon.png` & `lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-favicon.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_images/lakefs-spec-logo-dark.png` & `lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-logo-dark.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_images/lakefs-spec-logo-light.png` & `lakefs-spec-0.8.0.post0/docs/_images/lakefs-spec-logo-light.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-repositories.png` & `lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-repositories.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-sample-repo.png` & `lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-sample-repo.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_images/quickstart-lakefs-ui.png` & `lakefs-spec-0.8.0.post0/docs/_images/quickstart-lakefs-ui.png`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_scripts/gen_api_ref_pages.py` & `lakefs-spec-0.8.0.post0/docs/_scripts/gen_api_ref_pages.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_scripts/jupytext_convert.py` & `lakefs-spec-0.8.0.post0/docs/_scripts/jupytext_convert.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_styles/extra.css` & `lakefs-spec-0.8.0.post0/docs/_styles/extra.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_styles/neoteroi-mkdocs.css` & `lakefs-spec-0.8.0.post0/docs/_styles/neoteroi-mkdocs.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_styles/theme.css` & `lakefs-spec-0.8.0.post0/docs/_styles/theme.css`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/_theme_overrides/partials/header.html` & `lakefs-spec-0.8.0.post0/docs/_theme_overrides/partials/header.html`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/guides/configuration.md` & `lakefs-spec-0.8.0.post0/docs/guides/configuration.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/guides/filesystem-usage.md` & `lakefs-spec-0.8.0.post0/docs/guides/filesystem-usage.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/guides/index.md` & `lakefs-spec-0.8.0.post0/docs/guides/index.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/guides/integrations.md` & `lakefs-spec-0.8.0.post0/docs/guides/integrations.md`

 * *Files 14% similar despite different names*

```diff
@@ -34,14 +34,26 @@
 
 ```python hl_lines="6 9 11"
 --8<-- "docs/_code/duckdb_example.py"
 ```
 
 1. Makes the lakeFS-spec file system known to DuckDB (`duckdb.register_filesystem(fsspec.filesystem("lakefs"))` can also be used to avoid the direct import of `LakeFSFileSystem`)
 
+## Hugging Face Datasets
+
+[Hugging Face :hugging_face: Datasets](https://huggingface.co/docs/datasets/index){: target="_blank" rel="noopener"} is a library for easily accessing and sharing datasets for Audio, Computer Vision, and Natural Language Processing (NLP) tasks.
+It uses [fsspec internally](https://huggingface.co/docs/datasets/filesystems){: target="_blank" rel="noopener"} to retrieve and store datasets located outside the Hugging Face Hub.
+
+Reading a dataset from a lakeFS repository is as simple as passing the `data_files` argument to the `load_dataset` function with a generic dataset script (e.g., `csv` or `parquet` - see the [docs](https://huggingface.co/docs/datasets/en/loading#local-and-remote-files){: target="_blank" rel="noopener"} for a list of available types).
+Datasets can be saved to a lakeFS repository by passing the repository URL to the `save_to_disk()` method of the dataset.
+
+```python hl_lines="8 10"
+--8<-- "docs/_code/hf_datasets_example.py"
+```
+
 ## Polars
 
 !!! warning
     There is an ongoing discussion in the Polars development team whether to remove support for fsspec file systems, with no clear outcome as of the time this page was written.
     Please refer to the discussion on the relevant [GitHub issue](https://github.com/pola-rs/polars/issues/11056){: target="_blank" rel="noopener"} in case you encounter any problems.
 
 The Python API wrapper for the Rust-based [Polars](https://pola-rs.github.io/polars/){: target="_blank" rel="noopener"} DataFrame library can access remote storage through fsspec, similar to Pandas (see the official [documentation on cloud storage](https://pola-rs.github.io/polars/user-guide/io/cloud-storage/){: target="_blank" rel="noopener"}).
```

### Comparing `lakefs-spec-0.8.0/docs/guides/transactions.md` & `lakefs-spec-0.8.0.post0/docs/guides/transactions.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/index.md` & `lakefs-spec-0.8.0.post0/docs/index.md`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Our primary goal is to streamline versioned data operations in lakeFS, enabling seamless integration with popular data science tools such as Pandas, Polars, and DuckDB directly from Python.
 
 Highlights:
 
 - Simple repository operations in lakeFS
 - Easy access to underlying storage and versioning operations
 - Seamless integration with the fsspec ecosystem
-- Directly access lakeFS objects from popular data science libraries (including Pandas, Polars, DuckDB, PyArrow) with minimal code
+- Directly access lakeFS objects from popular data science libraries (including Pandas, Polars, DuckDB, Hugging Face Datasets, PyArrow) with minimal code
 - Transaction support for reliable data version control
 - Smart data transfers through client-side caching (up-/download)
 - Auto-discovery configuration
 
 !!! tip "Early Adopters"
     We are seeking early adopters who would like to actively participate in our feedback process and shape the future of the library.
     If you are interested in using the library and want to get in touch with us, please reach out via [Github Discussions](https://github.com/aai-institute/lakefs-spec/discussions){: target="_blank" rel="noopener"}.
```

### Comparing `lakefs-spec-0.8.0/docs/quickstart.md` & `lakefs-spec-0.8.0.post0/docs/quickstart.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/docs/tutorials/demo_data_science_project.py` & `lakefs-spec-0.8.0.post0/docs/tutorials/demo_data_science_project.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/hack/README.md` & `lakefs-spec-0.8.0.post0/hack/README.md`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/hack/docker-compose.yml` & `lakefs-spec-0.8.0.post0/hack/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/hack/lakefs-s3-local.yml` & `lakefs-spec-0.8.0.post0/hack/lakefs-s3-local.yml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/mkdocs.yml` & `lakefs-spec-0.8.0.post0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/pyproject.toml` & `lakefs-spec-0.8.0.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/requirements-dev.txt` & `lakefs-spec-0.8.0.post0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/requirements-docs.txt` & `lakefs-spec-0.8.0.post0/requirements-docs.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 argon2-cffi-bindings==21.2.0
 arrow==1.3.0
 asttokens==2.4.1
 async-lru==2.0.4
 attrs==23.2.0
 babel==2.14.0
 beautifulsoup4==4.12.3
-black==24.1.1
+black==24.3.0
 bleach==6.1.0
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 click==8.1.7
 colorama==0.4.6
 comm==0.2.1
```

### Comparing `lakefs-spec-0.8.0/src/lakefs_spec/errors.py` & `lakefs-spec-0.8.0.post0/src/lakefs_spec/errors.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/src/lakefs_spec/spec.py` & `lakefs-spec-0.8.0.post0/src/lakefs_spec/spec.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/src/lakefs_spec/transaction.py` & `lakefs-spec-0.8.0.post0/src/lakefs_spec/transaction.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/src/lakefs_spec/util.py` & `lakefs-spec-0.8.0.post0/src/lakefs_spec/util.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/src/lakefs_spec.egg-info/PKG-INFO` & `lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lakefs-spec
-Version: 0.8.0
+Version: 0.8.0.post0
 Summary: An fsspec implementation for lakeFS.
 Author-email: appliedAI Institute for Europe <lakefs-spec@appliedai-institute.de>
 Maintainer-email: Nicholas Junge <n.junge@appliedai-institute.de>, Max Mynter <m.mynter@appliedai-institute.de>, Adrian Rumpold <a.rumpold@appliedai-institute.de>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/aai-institute/lakefs-spec
 Project-URL: Repository, https://github.com/aai-institute/lakefs-spec.git
 Project-URL: Issues, https://github.com/aai-institute/lakefs-spec/issues
@@ -72,15 +72,15 @@
 Our primary goal is to streamline versioned data operations in lakeFS, enabling seamless integration with popular data science tools such as Pandas, Polars, and DuckDB directly from Python.
 
 Highlights:
 
 - Simple repository operations in lakeFS
 - Easy access to underlying storage and versioning operations
 - Seamless integration with the fsspec ecosystem
-- Directly access lakeFS objects from popular data science libraries (including Pandas, Polars, DuckDB, PyArrow) with minimal code
+- Directly access lakeFS objects from popular data science libraries (including Pandas, Polars, DuckDB, Hugging Face Datasets, PyArrow) with minimal code
 - Transaction support for reliable data version control
 - Smart data transfers through client-side caching (up-/download)
 - Auto-discovery configuration
 
 > [!NOTE]
 > We are seeking early adopters who would like to actively participate in our feedback process and shape the future of the library.
 If you are interested in using the library and want to get in touch with us, please reach out via [Github Discussions](https://github.com/aai-institute/lakefs-spec/discussions).
```

### Comparing `lakefs-spec-0.8.0/src/lakefs_spec.egg-info/SOURCES.txt` & `lakefs-spec-0.8.0.post0/src/lakefs_spec.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 .github/workflows/python.yaml
 .github/workflows/release.yaml
 assets/lakefs-spec-logo-all.svg
 docs/CONTRIBUTING.md
 docs/index.md
 docs/quickstart.md
 docs/_code/duckdb_example.py
+docs/_code/hf_datasets_example.py
 docs/_code/pandas_example.py
 docs/_code/polars_example.py
 docs/_code/pyarrow_example.py
 docs/_code/quickstart.py
 docs/_images/aai-favicon.png
 docs/_images/aai-logo-cropped.png
 docs/_images/lakefs-spec-favicon.png
```

### Comparing `lakefs-spec-0.8.0/tests/conftest.py` & `lakefs-spec-0.8.0.post0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/smoke_tests/test_abstractfilesystem.py` & `lakefs-spec-0.8.0.post0/tests/smoke_tests/test_abstractfilesystem.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/smoke_tests/test_integrations.py` & `lakefs-spec-0.8.0.post0/tests/smoke_tests/test_integrations.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_checksum.py` & `lakefs-spec-0.8.0.post0/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_copy.py` & `lakefs-spec-0.8.0.post0/tests/test_copy.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_errors.py` & `lakefs-spec-0.8.0.post0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_exists.py` & `lakefs-spec-0.8.0.post0/tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_fs.py` & `lakefs-spec-0.8.0.post0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_get_file.py` & `lakefs-spec-0.8.0.post0/tests/test_get_file.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_info.py` & `lakefs-spec-0.8.0.post0/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_internals.py` & `lakefs-spec-0.8.0.post0/tests/test_internals.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_lakefs_file.py` & `lakefs-spec-0.8.0.post0/tests/test_lakefs_file.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_ls.py` & `lakefs-spec-0.8.0.post0/tests/test_ls.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_put_file.py` & `lakefs-spec-0.8.0.post0/tests/test_put_file.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_rm.py` & `lakefs-spec-0.8.0.post0/tests/test_rm.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_spec_utils.py` & `lakefs-spec-0.8.0.post0/tests/test_spec_utils.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/test_transactions.py` & `lakefs-spec-0.8.0.post0/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `lakefs-spec-0.8.0/tests/util.py` & `lakefs-spec-0.8.0.post0/tests/util.py`

 * *Files identical despite different names*

