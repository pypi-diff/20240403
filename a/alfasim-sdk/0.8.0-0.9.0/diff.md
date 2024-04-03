# Comparing `tmp/alfasim_sdk-0.8.0.tar.gz` & `tmp/alfasim_sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alfasim_sdk-0.8.0.tar", last modified: Tue Apr 13 13:16:51 2021, max compression
+gzip compressed data, was "dist/alfasim_sdk-0.9.0.tar", last modified: Tue May  4 12:34:56 2021, max compression
```

## Comparing `alfasim_sdk-0.8.0.tar` & `alfasim_sdk-0.9.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)      308 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)     4153 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      732 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/RELEASING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      952 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/
--rw-r--r--   0 runner    (1001) docker     (121)      352 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/alfasim_sdk.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/detail/
--rw-r--r--   0 runner    (1001) docker     (121)     6176 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/detail/api_pointers.h
--rw-r--r--   0 runner    (1001) docker     (121)     6072 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h
--rw-r--r--   0 runner    (1001) docker     (121)     7326 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h
--rw-r--r--   0 runner    (1001) docker     (121)     3677 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/common.h
--rw-r--r--   0 runner    (1001) docker     (121)    32763 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/api.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/
--rw-r--r--   0 runner    (1001) docker     (121)    74671 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/hook_specs.py
--rw-r--r--   0 runner    (1001) docker     (121)    32221 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2711 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfasim_sdk_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    13372 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1361 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/status.py
--rw-r--r--   0 runner    (1001) docker     (121)     4203 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/variables.py
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/layout.py
--rw-r--r--   0 runner    (1001) docker     (121)    10580 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     6399 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/units.py
--rw-r--r--   0 runner    (1001) docker     (121)     1290 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)    16747 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/hook_specs_gui.py
--rw-r--r--   0 runner    (1001) docker     (121)     5594 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/
--rw-r--r--   0 runner    (1001) docker     (121)    11619 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/generate_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5410 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py
--rw-r--r--   0 runner    (1001) docker     (121)    32601 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/alfatable.py
--rw-r--r--   0 runner    (1001) docker     (121)     8573 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/case_description_attributes.py
--rw-r--r--   0 runner    (1001) docker     (121)    86796 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/case_description.py
--rw-r--r--   0 runner    (1001) docker     (121)    62363 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py
--rw-r--r--   0 runner    (1001) docker     (121)     2819 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/alfacase.py
--rw-r--r--   0 runner    (1001) docker     (121)    14756 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    17717 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/src/alfasim_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-13 13:16:51.000000 alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     2225 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      103 2021-04-13 13:16:46.000000 alfasim_sdk-0.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     4153 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1062 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      308 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/
+-rw-r--r--   0 runner    (1001) docker     (121)      352 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/alfasim_sdk.h
+-rw-r--r--   0 runner    (1001) docker     (121)    32763 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/api.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/
+-rw-r--r--   0 runner    (1001) docker     (121)     6072 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h
+-rw-r--r--   0 runner    (1001) docker     (121)     6176 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/api_pointers.h
+-rw-r--r--   0 runner    (1001) docker     (121)     7326 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h
+-rw-r--r--   0 runner    (1001) docker     (121)     3677 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/common.h
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/
+-rw-r--r--   0 runner    (1001) docker     (121)    11651 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/generate_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8573 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_description_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (121)    62558 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14730 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2370 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfatable.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32796 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2819 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfacase.py
+-rw-r--r--   0 runner    (1001) docker     (121)    87465 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_description.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5410 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32221 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2711 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfasim_sdk_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5188 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/units.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13372 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/context.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16747 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/hook_specs_gui.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3910 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/layout.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5594 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10611 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4203 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1361 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7521 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    77964 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/hook_specs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1290 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      135 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/version.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17717 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/src/alfasim_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1830 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       58 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1159 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/RELEASING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2021-05-04 12:34:56.000000 alfasim_sdk-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2653 2021-05-04 12:34:50.000000 alfasim_sdk-0.9.0/HISTORY.rst
```

### Comparing `alfasim_sdk-0.8.0/CONTRIBUTING.rst` & `alfasim_sdk-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/RELEASING.rst` & `alfasim_sdk-0.9.0/RELEASING.rst`

 * *Files 8% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 
 The version being released is listed in https://github.com/ESSS/alfasim-sdk/blob/master/src/alfasim_sdk/_internal/version.py, if needed this value should be changed to match accordingly.
 
 Any other required changes related to the release should also be included in the same branch.
 
 When all changes are ready the branch should be tagged ``v<release-number>`` and merged.
 
-After released it is advisable to update https://github.com/ESSS/alfasim-sdk/blob/master/src/alfasim_sdk/_internal/version.py with the next release version (increase minor version, for example ``0.6.0`` to ``0.7.0``).
+After released it is advisable to update https://github.com/ESSS/alfasim-sdk/blob/master/src/alfasim_sdk/_internal/version.py with the next release version (increase minor version, for example ``0.6.0`` to ``0.7.0``) and ``HISTORY.rst`` to add a section to next unreleased version.
```

### Comparing `alfasim_sdk-0.8.0/PKG-INFO` & `alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alfasim_sdk
-Version: 0.8.0
+Name: alfasim-sdk
+Version: 0.9.0
 Summary: ALFAsim API/SDK
 Home-page: https://github.com/esss/alfasim-sdk
 Author: ESSS
 Author-email: foss@esss.co
 License: UNKNOWN
 Description: ===========
         alfasim-sdk
```

### Comparing `alfasim_sdk-0.8.0/setup.cfg` & `alfasim_sdk-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/README.rst` & `alfasim_sdk-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/detail/api_pointers.h` & `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/api_pointers.h`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h` & `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_linux.h`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h` & `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/detail/bootstrap_win.h`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/common.h` & `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/common.h`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/alfasim_sdk_api/api.h` & `alfasim_sdk-0.9.0/src/alfasim_sdk/alfasim_sdk_api/api.h`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/hook_specs.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/hook_specs.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,23 +93,23 @@
         :linenos:
         :emphasize-lines: 1
 
         HOOK_FINALIZE(ctx)
         {
             // Threads information
             int n_threads = -1;
-            int errcode = alfasim.get_number_of_threads(ctx, &n_threads);
+            int errcode = alfasim_sdk_api.get_number_of_threads(ctx, &n_threads);
             f (errcode != 0){ // or errcode != OK
                 return errcode;
             }
             const char* plugin_id = get_plugin_id();
             // Plugin internal data
             for (int thread_id = 0; thread_id < n_threads; ++thread_id) {
                 void* data = nullptr;
-                errcode = alfasim.get_plugin_data(
+                errcode = alfasim_sdk_api.get_plugin_data(
                     ctx, &data, plugin_id, thread_id);
                 delete data;
             }
             // Unloading ALFAsim-SDK API
             int load_error_code = alfasim_sdk_close(alfasim_sdk_api)
             if (load_error_code != 0){
                 return load_error_code;
@@ -318,21 +318,21 @@
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_CALCULATE_MASS_SOURCE_TERM(
             ctx, mass_source, n_fields, n_control_volumes)
         {
-            int liq_id = -1;
+            int oil_id = -1;
             errcode = alfasim_sdk_api.get_field_id(
                 ctx, &oil_id, "oil");
             // Convertion from void* to double* and getting the
             // array range related to oil field
             double* oil_mass_source =
-                (double*) mass_source + n_control_volumes * liq_id;
+                (double*) mass_source + n_control_volumes * oil_id;
             // Make some calculations and add it to oil_mass_source.
             // In this example, we add a mass source of 3.1415 kg/s to all control volumes.
             for (int i = 0; i < n_control_volumes; ++i) {
                 oil_mass_source[i] = 3.1415; // [kg/s]
             }
             return OK;
         }
@@ -536,16 +536,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_INITIALIZE_STATE_VARIABLES_CALCULATOR(
-            void* ctx, void* P, void* T, void* T_mix,
-            int n_control_volumes, int n_layers)
+            ctx, P, T, T_mix, n_control_volumes, n_layers)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -558,16 +557,15 @@
             // MyFunction is a function implemented by
             // plugin developer that computes de density
             data.density = MyFunction(P, T_mix, n_control_volumes);
             return OK;
         }
         // Then, to use the cached value:
         HOOK_CALCULATE_STATE_VARIABLE(
-            void* ctx, void* P, void* T, int n_control_volumes, i
-            nt n_layers, int phase_id, int property_id, void* output)
+            ctx, P, T, n_control_volumes, n_layers, phase_id, property_id, output)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -640,17 +638,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_CALCULATE_STATE_VARIABLE(
-            void* ctx, void* P, void* T,
-            int n_control_volumes, int n_layers,
-            int phase_id, int property_id, void* output)
+            ctx, P, T, n_control_volumes, n_layers, phase_id, property_id, output)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -691,15 +687,15 @@
     property_id: "int",
     output: "void*",
 ) -> "int":
     """
     **c++ signature** : ``HOOK_CALCULATE_PHASE_PAIR_STATE_VARIABLE(void* ctx, void* P, void* T_mix, int n_control_volumes,
     int phase1_id, int phase2_id, int property_id, void* output)``
 
-    Hook to calculate the state variable given by the `property_id` (See :cpp:enum:StateVariable values), for the phase
+    Hook to calculate the state variable given by the `property_id` (See :cpp:enum:`StateVariable` values), for the phase
     pair `(phase1_id, phase2_id)` (Note that the phase id is the same as the one retrieved from the :cpp:func:`get_phase_id()`
     API function - It is not advisable to use hardcoded numbers).
 
     List of affected variables:|br|
     - ``Interfacial Tension``
 
     :param ctx: ALFAsim's plugins context
@@ -720,16 +716,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_CALCULATE_PHASE_PAIR_STATE_VARIABLE(
-            void* ctx, void* P, void* T_mix, int n_control_volumes,
-            int phase1_id, int phase2_id, int property_id, void* output)
+            ctx, P, T_mix, n_control_volumes, phase1_id, phase2_id, property_id, output)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -783,15 +778,15 @@
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
-        HOOK_FINALIZE_STATE_VARIABLES_CALCULATOR(void* ctx)
+        HOOK_FINALIZE_STATE_VARIABLES_CALCULATOR(ctx)
         {
             return OK;
         }
 
     """
 
 
@@ -819,16 +814,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_INITIALIZE_PARTICLE_DIAMETER_OF_SOLIDS_FIELDS(
-            void* ctx, void* particle_diameter,
-            int n_control_volumes, int solids_field_id)
+            ctx, particle_diameter, n_control_volumes, solids_field_id)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -837,19 +831,19 @@
             errcode = alfasim_sdk_api.get_plugin_data(
                     ctx, (void**) &data, plugin_id, thread_id);
             if (solids_field_id != data.my_added_solid_field_id) {
                 return OK;
             } else {
                 for (int i = 0; i < n_control_volumes; ++i) {
                     // If the particle size is constant
-                    output[i] = data.constant_particle_size;
+                    particle_diameter[i] = data.constant_particle_size;
                     // The value is calculated
                     // MyStruct has a function
                     // called 'initial_particle_size()'
-                    output[i] = data.initial_particle_size(
+                    particle_diameter[i] = data.initial_particle_size(
                              // List of params that can be
                              // retrieved by get_simulation_array()
                              );
                 }
             }
             return OK;
         }
@@ -881,16 +875,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_UPDATE_PARTICLE_DIAMETER_OF_SOLIDS_FIELDS(
-            void* ctx, void* particle_diameter,
-            int n_control_volumes, int solids_field_id)
+            ctx, particle_diameter, n_control_volumes, solids_field_id)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -899,19 +892,19 @@
             errcode = alfasim_sdk_api.get_plugin_data(
                     ctx, (void**) &data, plugin_id, thread_id);
             if (solids_field_id != data.my_added_solid_field_id) {
                 return OK;
             } else {
                 for (int i = 0; i < n_control_volumes; ++i) {
                     // If the particle size is constant
-                    output[i] = data.constant_particle_size;
+                    particle_diameter[i] = data.constant_particle_size;
                     // The value is calculated
                     // MyStruct has a function
                     // called 'compute_particle_size()'
-                    output[i] = data.compute_particle_size(
+                    particle_diameter[i] = data.compute_particle_size(
                              // List of params that can be
                              // retrieved by get_simulation_array()
                              );
                 }
             }
             return OK;
         }
@@ -986,15 +979,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_INITIALIZE_MASS_FRACTION_OF_TRACER(
-            void* ctx, void* phi_initial, int tracer_index)
+            ctx, phi_initial, tracer_index)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -1043,16 +1036,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_CALCULATE_MASS_FRACTION_OF_TRACER_IN_PHASE(
-            void* ctx, void* phi, void* phi_phase,
-            int tracer_index, int phase_index, int n_control_volumes)
+            ctx, phi, phi_phase, tracer_index, phase_index, n_control_volumes)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -1123,17 +1115,16 @@
      Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_CALCULATE_MASS_FRACTION_OF_TRACER_IN_FIELD(
-            void* ctx, void* phi_phase, void* phi_field,
-            int tracer_index, int field_index,
-            int phase_index_of_field, int n_control_volumes)
+            ctx, phi_phase, phi_field, tracer_index, field_index,
+            phase_index_of_field, n_control_volumes)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -1197,15 +1188,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_SET_PRESCRIBED_BOUNDARY_CONDITION_OF_MASS_FRACTION_OF_TRACER(
-            void* ctx, void* phi_presc, int tracer_index)
+            ctx, phi_presc, tracer_index)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -1256,15 +1247,15 @@
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
         HOOK_UPDATE_BOUNDARY_CONDITION_OF_MASS_FRACTION_OF_TRACER(
-            void* ctx, void* phi_presc, int tracer_index)
+            ctx, phi_presc, tracer_index)
         {
             // getting plugin internal data
             int errcode = -1;
             int thread_id = -1;
             errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
             if (errcode != OK) {
                 return errcode;
@@ -1320,27 +1311,26 @@
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
-        int HOOK_CALCULATE_UCM_FRICTION_FACTOR_STRATIFIED(
-            void* ctx, double* ff_wG, double* ff_wL, double* ff_i)
+        HOOK_CALCULATE_UCM_FRICTION_FACTOR_STRATIFIED(ctx, ff_wG, ff_wL, ff_i)
         {
             int errcode = -1;
             int G = TwoPhaseSystem::GAS;
             int L = TwoPhaseSystem::LIQUID;
 
             // Getting friction factor input data from context
             double alpha[2];
             errcode = alfasim_sdk_api.get_ucm_friction_factor_input_variable(
                 ctx, &alpha[G], "alpha", TwoPhaseSystem::GAS);
             if (errcode != OK){ return errcode; }
-            errcode = alfasim_plugins_api.get_ucm_friction_factor_input_variable(
+            errcode = alfasim_sdk_api.get_ucm_friction_factor_input_variable(
                 ctx, &alpha[L], "alpha", TwoPhaseSystem::LIQUID);
             if (errcode != OK){ return errcode; }
             // And so on to each friction factor input variable
             // U(velocities), rho(densities), mu(viscosities) and D(pipe diameter)
 
              // Getting the fluid geometrical properties
             double S_w[2];
@@ -1399,15 +1389,15 @@
     in the Liquid-Liquid system. The Liquid-Liquid system is a two phase flow with Oil and Water Phases.
     It represents the separation of Liquid phase (into oil and water phases) used in the two phase system
     (Gas-Liquid). The output variables ``ll_fp`` and ``water_vol_frac`` are the liquid-liquid flow pattern
     and volume fraction of water, respectively.
 
     .. note::
         The main input variables needed to estimate the flow pattern is available in the API function
-        :cpp:func:`get_ucm_liqliq_flow_pattern_input_variable`. Note that, the variables listed in the documentation
+        :cpp:func:`get_liq_liq_flow_pattern_input_variable`. Note that, the variables listed in the documentation
         of the cited function are related to one control volume, in which the estimation is applied.
 
     This `hook` allows the developer to implement your own flow pattern estimation algorithm for the liquid-liquid
     system.
 
     The ``ll_fp`` must be one of the following values: |br|
     - `0 - Unknown`: Unknown Flow Pattern. |br|
@@ -1427,36 +1417,35 @@
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
-        int HOOK_CALCULATE_LIQ_LIQ_FLOW_PATTERN(void* ctx, int* ll_fp, double* water_vol_frac)
+        HOOK_CALCULATE_LIQ_LIQ_FLOW_PATTERN(ctx, ll_fp, water_vol_frac)
         {
             int errcode = -1;
             int O = LiquidLiquidSystem::OIL;
             int W = LiquidLiquidSystem::WATER;
 
             // Getting liq-liq Flow Pattern input data from context
             double rho[2];
-            errcode = alfasim_sdk_api.get_ucm_liqliq_flow_pattern_input_variable(
+            errcode = alfasim_sdk_api.get_liq_liq_flow_pattern_input_variable(
                 ctx, &rho[O], "rho", LiquidLiquidSystem::OIL);
             if (errcode != OK){ return errcode; }
-            errcode = alfasim_plugins_api.get_ucm_liqliq_flow_pattern_input_variable(
+            errcode = alfasim_sdk_api.get_liq_liq_flow_pattern_input_variable(
                 ctx, &rho[W], "rho", LiquidLiquidSystem::WATER);
             if (errcode != OK){ return errcode; }
             // And so on to each input variable
             // U_S(superficial velocities), mu(viscosities)
             // and D_h(liquid hydraulic diameter)
 
             // Estimate the liquid-liquid Flow pattern and volume fraction of water
             // using your own algorithm.
 
-
             *ll_fp = flow_pattern;
             *water_vol_frac = alpha_W;
 
             return OK;
         }
     """
 
@@ -1469,15 +1458,15 @@
 
     Internal `hook` to calculate the liquid (Oil-Water) effective viscosity in the Liquid-Liquid system.
     It represents viscosity of a Liquid phase used in the two phase system (Gas-Liquid).
     The output variable ``mu_l_eff`` is the Liquid Effective Viscosity. It has unit equal to ``[Pa.s]``.
 
     .. note::
         The main input variables needed to estimate the liquid effective viscosity is available in the API function
-        :cpp:func:`get_ucm_liquid_effective_viscosity_input_variable`. Note that, the variables listed in the
+        :cpp:func:`get_liquid_effective_viscosity_input_variable`. Note that, the variables listed in the
         documentation of the cited function are related to one control volume, in which the estimation is applied.
 
     This `hook` allows the developer to implement your own liquid effective viscosity correlation to
     represent the viscosity of an unified liquid phase that represents the Oil-Water mixture.
 
     :param ctx: ALFAsim's plugins context
     :param mu_l_eff: Liquid Effective Viscosity
@@ -1486,26 +1475,26 @@
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
-        int HOOK_CALCULATE_LIQUID_EFFECTIVE_VISCOSITY(void* ctx, double* mu_l_eff, int ll_fp)
+        HOOK_CALCULATE_LIQUID_EFFECTIVE_VISCOSITY(ctx, mu_l_eff, ll_fp)
         {
             int errcode = -1;
             int O = LiquidLiquidSystem::OIL;
             int W = LiquidLiquidSystem::WATER;
 
             // Getting liquid Effective Viscosity input data from context
             double rho[2];
-            errcode = alfasim_sdk_api.get_ucm_liquid_effecticve_viscosity_input_variable(
+            errcode = alfasim_sdk_api.get_liquid_effecticve_viscosity_input_variable(
                 ctx, &rho[O], "rho", LiquidLiquidSystem::OIL);
             if (errcode != OK){ return errcode; }
-            errcode = alfasim_plugins_api.get_ucm_liquid_effecticve_viscosity_input_variable(
+            errcode = alfasim_sdk_api.get_liquid_effecticve_viscosity_input_variable(
                 ctx, &rho[W], "rho", LiquidLiquidSystem::WATER);
             if (errcode != OK){ return errcode; }
             // And so on to each input variable
             // U_S(superficial velocities), mu(viscosities for Oil and Water) and
             // D_h(liquid hydraulic diameter)
 
             // Estimate the liquid effective viscosity using your own algorithm.
@@ -1527,15 +1516,15 @@
 
     Internal `hook` to calculate the Gas-liquid Surface Tension based in the Liquid-Liquid System.
     It represents Gas-Liquid surface tension used in the two phase system (Gas-Liquid).
     The output variable ``sigma_gl`` is the Gas-Liquid Surface tension. It has unit equal to ``[N/m]``.
 
     .. note::
         The main input variables needed to estimate the Gas-Liquid Surface Tension is available in the API function
-        :cpp:func:`get_ucm_gasliq_surface_tension_input_variable`. Note that, the variables listed in the
+        :cpp:func:`get_gas_liq_surface_tension_input_variable`. Note that, the variables listed in the
         documentation of the cited function are related to one control volume, in which the estimation is applied.
 
     This `hook` allows the developer to implement your own Gas-liquid Surface Tension correlation for
     an unified liquid phase that represents the Oil-Water mixture.
 
     .. note::
         It is important to note that the Gas-Liquid Surface tension depends on Gas-Oil and Gas-Water
@@ -1549,23 +1538,23 @@
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
-        int HOOK_CALCULATE_GAS_LIQ_SURFACE_TENSION(void* ctx, double* sigma_gl, int ll_fp)
+        HOOK_CALCULATE_GAS_LIQ_SURFACE_TENSION(ctx, sigma_gl, ll_fp)
         {
             int errcode = -1;
             int O = LiquidLiquidSystem::OIL;
             int W = LiquidLiquidSystem::WATER;
 
             // Getting liquid Effective Viscosity input data from context
             double sigma_gll[2];
-            errcode = alfasim_sdk_api.get_ucm_gasliq_surface_tension_input_variable(
+            errcode = alfasim_sdk_api.get_gas_liq_surface_tension_input_variable(
                 ctx, &sigma_gll[O], "sigma_gll", LiquidLiquidSystem::OIL);
             if (errcode != OK){ return errcode; }
             // And so on to each input variable
             // sigma_gw(Surface tension Gas-Water) and alpha_w(Water Volume Fraction)
 
             // Estimate the Gas-Liquid Surface Tension using your own algorithm.
             // Since the Gas-Liquid Surface Tension depends on Liquid-Liquid Flow Pattern,
@@ -1592,15 +1581,15 @@
 
     Internal `hook` to calculate the Shear Force per unit volume for the Liquid-Liquid System.
     Also Field velocities and field volume fraction must be calculated.
     It is important to compute the shear stress term in the momentum equation for the Liquid-Liquid System.
 
     .. note::
         The main input variables needed to estimate the Shear Force is available in the API function
-        :cpp:func:`get_ucm_liqliq_shear_force_per_volume_input_variable`. Note that, the variables listed in the
+        :cpp:func:`get_liq_liq_shear_force_per_volume_input_variable`. Note that, the variables listed in the
         documentation of the cited function are related to one control volume, in which the estimation is applied.
 
     The output variable ``shear_w`` is the Wall Shear Force per unit Volume with size equal to ``2``
     (for Oil and Water phases) and it has unit equal to ``[N/m^3]``.
     The output variable ``shear_i`` is the Interfacial Shear Force per unit Volume between Oil and Water
     phases it has unit equal to ``[N/m^3]``.
     The output variable ``u_fields`` is the field velocities with size ``4`` because values for continuous
@@ -1628,28 +1617,29 @@
 
     Example of usage:
 
     .. code-block:: c++
         :linenos:
         :emphasize-lines: 1
 
-        int HOOK_CALCULATE_LIQ_LIQ_SHEAR_FORCE_PER_VOLUME(void* ctx, double* shear_w,
-            double* shear_i, double* U_fields, double* vol_frac_fields, int ll_fp)
+        HOOK_CALCULATE_LIQ_LIQ_SHEAR_FORCE_PER_VOLUME(ctx, shear_w,
+            shear_i, U_fields, vol_frac_fields, ll_fp)
         {
             int errcode = -1;
             int O = 0;
             int W = 1;
             int OW = 2;
             int WO = 3;
 
             // Getting shear term input data from context
             double rho[2];
-            errcode = alfasim_sdk_api.get_ucm_liqliq_shear_force_per_volume_input_variable(
+            errcode = alfasim_sdk_api.get_liq_liq_shear_force_per_volume_input_variable(
                 ctx, &rho[O], "rho", LiquidLiquidSystem::OIL);
-            errcode = alfasim_sdk_api.get_ucm_liqliq_shear_force_per_volume_input_variable(
+            if (errcode != OK){ return errcode; }
+            errcode = alfasim_sdk_api.get_liq_liq_shear_force_per_volume_input_variable(
                 ctx, &rho[W], "rho", LiquidLiquidSystem::WATER);
             if (errcode != OK){ return errcode; }
             // And so on to each input variable
             // U_S(superficial velocities), mu(viscosities for Oil and Water) and
             // D_h(liquid hydraulic diameter)
 
             // Calculate the wall and interfacial shear force per unit volume, fields (Liquid-Liquid System)
@@ -1668,14 +1658,104 @@
             vol_frac_fields[WO] = alpha[WO];
 
             return OK;
         }
     """
 
 
+def calculate_relative_emulsion_viscosity(
+    ctx: "void*",
+    mu_r: "double*",
+    disp_field_index: "int",
+    layer_index: "int",
+    n_faces: "int",
+) -> "int":
+    """
+    **c++ signature** : ``HOOK_RELATIVE_EMULSION_VISCOSITY(void* ctx, double* mu_r, int disp_field_index, int layer_index, int n_faces)``
+
+    Internal `hook` to calculate the relative emulsion viscosity in the Emulsion Model.
+    This `hook` will be used in the emulsion model to calculate the apparent viscosity of the emulsion
+    (Continuous field + dispersed field).
+
+    The relative emulsion viscosity is defined by:
+
+    .. math::
+
+        \\begin{equation}
+            \\mu_r = \\frac{\\mu_m}{\\mu_c}
+        \\end{equation}
+
+
+    .. rubric:: Where
+
+    :1: :math:`\\mu_r` is the relative emulsion viscosity
+    :2: :math:`\\mu_m` is the apparent viscosity
+    :3: :math:`\\mu_c` is the viscosity of the continuous field
+
+    The output variable ``mu_r`` is the relative emulsion viscosity with size equal to ``n_faces`` and it
+    is dimensionless.
+    The ``disp_field_index`` is the index of the dipersed field. Since it is an emulsion dispersed field,
+    it can have values for ``oil in water`` and ``water in oil`` fields.
+    The ``layer_index`` is the index of the layer and continuous field in the layer. Since it is the index
+    of the main field of the emulsion, it can have values for ``oil``  or ``water`` layers (and/or continuous
+    fields).
+
+    .. Note::
+        It is important to know that the calculations for viscosity is performed over the faces (see
+        ``n_faces`` param). For that, any variable that should be retrieved using :cpp:func:`get_simulation_array`
+        must be use value ``Face`` in the :cpp:enum:`GridScope` param.
+
+    This `hook` allows the implementation of the relative emulsion viscosity correlation. Once the plugin
+    installed it is important to be selected in the emulsion model configuration inside the Physics data
+    tree in the ALFAsim application in order to be used.
+
+    :param ctx: ALFAsim's plugins context
+    :param mu_r: Relative emulsion viscosity
+    :param disp_field_index: Index of the dispersed field
+    :param layer_index: Index of the Layer or Continuous Field
+    :param n_faces: Number of faces.
+    :returns: Return OK if successful or anything different if failed
+
+    Example of usage:
+
+    .. code-block:: c++
+        :linenos:
+        :emphasize-lines: 1
+
+        HOOK_RELATIVE_EMULSION_VISCOSITY(ctx, mu_r, disp_field_index, layer_index, n_faces)
+        {
+            const char* plugin_id = get_plugin_id()
+            errcode = alfasim_sdk_api.get_thread_id(ctx, &thread_id);
+            if (errcode != OK) {
+                return errcode;
+            }
+            // MyStruct is a developer defined struct to hold
+            // all important information for plugin hooks.
+            MyStruct* data = nullptr;
+            errcode = alfasim_sdk_api.get_plugin_data(ctx, (void**) &data, plugin_id, thread_id);
+
+            if (disp_field_index == data.oil_in_water_index){
+                // Calculate the relative emulsion viscosity
+                // for water dominated scenario.
+                // ComputeForWaterDominated is a function implemented
+                // by plugin developer
+                ComputeForWaterDominated(mu_r, n_faces);
+            } else if (disp_field_index == data.water_in_oil_index){
+                // Calculate the relative emulsion viscosity
+                // for oil dominated scenario
+                // ComputeForOilDominated is a function implemented
+                // by plugin developer
+                ComputeForOilDominated(mu_r, n_faces);
+            }
+
+            return OK;
+        }
+    """
+
+
 def friction_factor(v1: "int", v2: "int") -> "int":
     """
     Docs for Friction Factor
     """
 
 
 def env_temperature(v3: "float", v4: "float") -> "float":
@@ -1847,14 +1927,16 @@
         calculate_ucm_friction_factor_stratified,
         calculate_ucm_friction_factor_annular,
         # Hooks related to Liquiq-Liquid Mechanistic Model
         calculate_liq_liq_flow_pattern,
         calculate_liquid_effective_viscosity,
         calculate_gas_liq_surface_tension,
         calculate_liq_liq_shear_force_per_volume,
+        # Hooks related to Emulsion Model
+        calculate_relative_emulsion_viscosity,
         # Extra Hooks (For testing)
         friction_factor,
         env_temperature,
         calculate_entrained_liquid_fraction,
         update_internal_deposition_layer,
     ],
 )
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/types.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/types.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfasim_sdk_utils.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfasim_sdk_utils.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/context.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/context.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/status.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/status.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/variables.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/variables.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/layout.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/layout.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/constants.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
     Mooney1951a = "mooney1951a"
     Mooney1951b = "mooney1951b"
     Hinze1955 = "hinze1955"
     Sleicher1962 = "sleicher1962"
     Brauner2001 = "brauner2001"
     Boxall2012 = "boxall2012"
     Brinkman1952AndYeh1964 = "brinkman1952_and_yeh1964"
+    FromPlugin = "from_plugin"
 
 
 class SolidsModelType(Enum):
     """
     Informs which solid model should be used:
 
     - NoModel - None:RR
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/cli.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -180,14 +180,45 @@
         EXTRAS_REQUIRED_VERSION_KEY: get_extras_default_required_version()
     }
     hm.generate_plugin_package(
         package_name, plugin_dir, dst, extras_defaults=extras_defaults
     )
 
 
+@console_main.command()
+@click.pass_context
+@plugin_dir_option
+def update(ctx, plugin_dir):
+    """
+    Updates plugin files automatically generated by ALFAsim-SDK.
+    The plugin folder is informed with plugin-dir option.
+    When not provided plugin-dir will be the current folder location.
+
+    It is important to update the automatically generated files from each plugin when
+    a new version of ALFAsim-SDK is released. Otherwise compilation problems can occur.
+
+    The files updated are: |br|
+    - ´<plugin_folder>/src/hook_specs.h´ |br|
+    """
+    hook_specs_file_path = _get_hook_specs_file_path()
+    hm = HookManGenerator(hook_spec_file_path=hook_specs_file_path)
+
+    plugin_folder = Path(plugin_dir)
+    hook_specs_h_path = plugin_folder / "src" / "hook_specs.h"
+
+    if not hook_specs_h_path.exists() or not hook_specs_h_path.is_file():
+        raise FileNotFoundError(
+            f"Was not possible to find 'src/hook_specs.h' file in {plugin_dir}"
+        )
+
+    plugin_id = plugin_folder.name
+    plugin_location = plugin_folder.parent
+    hm.generate_hook_specs_header(plugin_id, plugin_location)
+
+
 def _get_hook_specs_file_path() -> Path:
     import alfasim_sdk._internal.hook_specs
 
     return Path(alfasim_sdk._internal.hook_specs.__file__)
 
 
 if __name__ == "__main__":
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/units.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/units.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/validators.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/validators.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/hook_specs_gui.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/hook_specs_gui.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/models.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/models.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/generate_schema.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/generate_schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,14 +241,15 @@
 
 # plugins:
 #   For now, Plugins inputs (GUI) will not be able to be customizable by YAML
 
 IGNORED_PROPERTIES = (
     "plugins",
     "table_parameters",
+    "emulsion_model_plugin_id",
 )
 
 
 def _get_attribute_schema(
     key: str, value: attr.ib, indentation=INDENTANTION * 2
 ) -> str:
     """
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_to_alfacase.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/schema.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # fmt: off
-##[[[cog
+# #[[[cog
 # import cog
 # from alfasim_sdk import CaseDescription
 # from alfasim_sdk._internal.alfacase.generate_schema import get_all_classes_that_needs_schema, generate_alfacase_schema
 # cog.out("from strictyaml import Bool, Enum, Int, Map, MapPattern, Optional, Seq, Str, Float # noreorder")
 # cog.out("\n\n")
 # cog.out("\n\n")
 # list_of_classes_that_needs_schema = get_all_classes_that_needs_schema(CaseDescription)
@@ -222,15 +222,15 @@
         Optional("hydrodynamic_model"): Enum(['hydrodynamic_model_2_fields', 'hydrodynamic_model_4_fields', 'hydrodynamic_model_3_layers_gas_oil_water', 'hydrodynamic_model_5_fields_solid', 'hydrodynamic_model_5_fields_water', 'hydrodynamic_model_5_fields_co2', 'hydrodynamic_model_3_layers_no_bubble_gas_oil_water', 'hydrodynamic_model_3_layers_water_with_co2', 'hydrodynamic_model_3_layers_7_fields_gas_oil_water', 'hydrodynamic_model_3_layers_9_fields_gas_oil_water']),
         Optional("simulation_regime"): Enum(['simulation_regime_transient', 'simulation_regime_steady_state']),
         Optional("energy_model"): Enum(['no_model', 'global_model', 'layers_model']),
         Optional("solids_model"): Enum(['no_model', 'thomas1965_equilibrium', 'mills1985_equilibrium', 'santamaria2010_equilibrium']),
         Optional("initial_condition_strategy"): Enum(['constant', 'steady_state', 'restart']),
         Optional("restart_filepath"): Str(),
         Optional("keep_former_results"): Bool(),
-        Optional("emulsion_model"): Enum(['no_model', 'model_default', 'taylor1932', 'brinkman1952', 'mooney1951a', 'mooney1951b', 'hinze1955', 'sleicher1962', 'brauner2001', 'boxall2012', 'brinkman1952_and_yeh1964']),
+        Optional("emulsion_model"): Enum(['no_model', 'model_default', 'taylor1932', 'brinkman1952', 'mooney1951a', 'mooney1951b', 'hinze1955', 'sleicher1962', 'brauner2001', 'boxall2012', 'brinkman1952_and_yeh1964', 'from_plugin']),
         Optional("flash_model"): Enum(['hydrocarbon_only', 'hydrocarbon_and_water']),
         Optional("correlations_package"): Enum(['correlation_package_classical', 'correlation_package_alfasim', 'correlation_package_isdb_tests']),
     }
 )
 pipe_segments_description_schema = Map(
     {
         "start_positions": Map({"values": Seq(Float()), "unit": Str()}),
@@ -329,17 +329,19 @@
 )
 separator_node_properties_description_schema = Map(
     {
         Optional("environment_temperature"): Map({"value": Float(), "unit": Str()}),
         Optional("geometry"): Enum(['vertical_cylinder', 'horizontal_cylinder', 'sphere']),
         Optional("length"): Map({"value": Float(), "unit": Str()}),
         Optional("overall_heat_transfer_coefficient"): Map({"value": Float(), "unit": Str()}),
-        Optional("radius"): Map({"value": Float(), "unit": Str()}),
+        Optional("diameter"): Map({"value": Float(), "unit": Str()}),
         Optional("nozzles"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
         Optional("initial_phase_volume_fractions"): MapPattern(Str(), Map({"value": Float(), "unit": Str()})),
+        Optional("gas_separation_efficiency"): Map({"value": Float(), "unit": Str()}),
+        Optional("liquid_separation_efficiency"): Map({"value": Float(), "unit": Str()}),
     }
 )
 speed_curve_description_schema = Map(
     {
         Optional("time"): Map({"values": Seq(Float()), "unit": Str()}),
         Optional("speed"): Map({"values": Seq(Float()), "unit": Str()}),
     }
@@ -674,9 +676,9 @@
         Optional("pipes"): Seq(pipe_description_schema),
         Optional("nodes"): Seq(node_description_schema),
         Optional("wells"): Seq(well_description_schema),
         Optional("materials"): Seq(material_description_schema),
         Optional("walls"): Seq(wall_description_schema),
     }
 )
-# [[[end]]] (checksum: 246db83b8565903de6db4af4b62191c7)
+# [[[end]]] (checksum: 41248460c8164bf2648e6a873c1af78f)
 # fmt: on
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/alfatable.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfatable.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/case_description_attributes.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_description_attributes.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/case_description.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/case_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,15 +899,15 @@
     elevation: Optional[Array] = attr.ib(
         default=None, validator=optional(instance_of(Array))
     )
 
     def iter_values_and_unit(
         self,
     ) -> Iterator[Tuple[value_and_unit, value_and_unit]]:
-        """ Returns a pair of values with length and elevation along with their units. """
+        """Returns a pair of values with length and elevation along with their units."""
         length_values = self.length.GetValues(self.length.unit)
         elevation_values = self.elevation.GetValues(self.elevation.unit)
         for length, elevation in zip(length_values, elevation_values):
             yield (length, self.length.unit), (elevation, self.elevation.unit)
 
 
 @attr.s(frozen=True, slots=True)
@@ -922,15 +922,15 @@
 
     x: Optional[Array] = attr.ib(default=None, validator=optional(instance_of(Array)))
     y: Optional[Array] = attr.ib(default=None, validator=optional(instance_of(Array)))
 
     def iter_values_and_unit(
         self,
     ) -> Iterator[Tuple[value_and_unit, value_and_unit]]:
-        """ Returns a pair of values with the x and y value along with their units. """
+        """Returns a pair of values with the x and y value along with their units."""
         for x, y in zip(self.x.GetValues(self.x.unit), self.y.GetValues(self.y.unit)):
             yield (x, self.x.unit), (y, self.y.unit)
 
 
 @attr.s()
 class ProfileDescription:
     """
@@ -1083,37 +1083,49 @@
     .. include:: /alfacase_definitions/list_of_unit_for_volume_fraction.txt
     """
 
     environment_temperature = attrib_scalar(default=Scalar(25.0, "degC"))
     geometry = attrib_enum(default=constants.SeparatorGeometryType.VerticalCylinder)
     length = attrib_scalar(default=Scalar(1.0, "m"))
     overall_heat_transfer_coefficient = attrib_scalar(default=Scalar(0.0, "W/m2.K"))
-    radius = attrib_scalar(default=Scalar(1.0, "m"))
+    diameter = attrib_scalar(default=Scalar(1.0, "m"))
     nozzles: Dict[str, Scalar] = attr.ib(
         default=attr.Factory(dict), validator=optional(dict_with_scalar)
     )
     initial_phase_volume_fractions: Dict[str, Scalar] = attr.ib(
         default={
             constants.FLUID_GAS: Scalar("volume fraction", 0.5, "-"),
             constants.FLUID_OIL: Scalar("volume fraction", 0.5, "-"),
         }
     )
+    gas_separation_efficiency = attrib_scalar(default=Scalar("dimensionless", 1.0, "-"))
+    liquid_separation_efficiency = attrib_scalar(
+        default=Scalar("dimensionless", 1.0, "-")
+    )
 
-    @radius.validator
-    def _validate_radius(self, attribute, value):
+    @diameter.validator
+    def _validate_diameter(self, attribute, value):
         assert (
             isinstance(value, Scalar) and value.GetCategory() == "length"
-        ), "Invalid radius"
+        ), "Invalid diameter"
 
     @length.validator
     def _validate_length(self, attribute, value):
         assert (
             isinstance(value, Scalar) and value.GetCategory() == "length"
         ), "Invalid length"
 
+    @gas_separation_efficiency.validator
+    def _validate_gas_separation_efficiency(self, attribute, value):
+        assert isinstance(value, Scalar) and 0.6 <= value.GetValue("-") <= 1.0
+
+    @liquid_separation_efficiency.validator
+    def _validate_liquid_separation_efficiency(self, attribute, value):
+        assert isinstance(value, Scalar) and 0.6 <= value.GetValue("-") <= 1.0
+
 
 @attr.s(slots=True, kw_only=True)
 class NodeDescription:
     """
     .. include:: /alfacase_definitions/NodeDescription.txt
     """
 
@@ -1980,14 +1992,15 @@
         default=constants.InitialConditionStrategyType.Constant
     )
     restart_filepath: Optional[Path] = attr.ib(
         default=None, validator=optional(instance_of(Path))
     )
     keep_former_results: bool = attr.ib(default=False, validator=instance_of(bool))
     emulsion_model = attrib_enum(default=constants.EmulsionModelType.NoModel)
+    emulsion_model_plugin_id: str = attr.ib(default="", validator=instance_of(str))
     flash_model = attrib_enum(default=constants.FlashModel.HydrocarbonAndWater)
     correlations_package = attrib_enum(
         default=constants.CorrelationPackageType.Classical
     )
 
 
 @attr.s()
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfacase_to_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -945,19 +945,21 @@
     document: DescriptionDocument,
 ) -> case_description.SeparatorNodePropertiesDescription:
     alfacase_to_case_description = {
         "environment_temperature": get_scalar_loader(from_unit="K"),
         "geometry": get_enum_loader(enum_class=constants.SeparatorGeometryType),
         "length": get_scalar_loader(from_unit="m"),
         "overall_heat_transfer_coefficient": get_scalar_loader(from_unit="W/m2.K"),
-        "radius": get_scalar_loader(from_unit="m"),
+        "diameter": get_scalar_loader(from_unit="m"),
         "nozzles": get_dict_with_scalar_loader(category=get_category_for("m")),
         "initial_phase_volume_fractions": get_dict_with_scalar_loader(
             category="volume fraction"
         ),
+        "gas_separation_efficiency": get_scalar_loader(from_unit="%"),
+        "liquid_separation_efficiency": get_scalar_loader(from_unit="%"),
     }
     case_values = to_case_values(document, alfacase_to_case_description)
     return case_description.SeparatorNodePropertiesDescription(**case_values)
 
 
 def load_node_description(
     document: DescriptionDocument,
@@ -1557,14 +1559,15 @@
         'simulation_regime': get_enum_loader(enum_class=constants.SimulationRegimeType),
         'energy_model': get_enum_loader(enum_class=constants.EnergyModel),
         'solids_model': get_enum_loader(enum_class=constants.SolidsModelType),
         'initial_condition_strategy': get_enum_loader(enum_class=constants.InitialConditionStrategyType),
         'restart_filepath': load_path,
         'keep_former_results': load_value,
         'emulsion_model': get_enum_loader(enum_class=constants.EmulsionModelType),
+        'emulsion_model_plugin_id': load_value,
         'flash_model': get_enum_loader(enum_class=constants.FlashModel),
         'correlations_package': get_enum_loader(enum_class=constants.CorrelationPackageType),
     }
     # fmt: on
     case_values = to_case_values(document, alfacase_to_case_description)
     return case_description.PhysicsDescription(**case_values)
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/alfacase.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/alfacase.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/_internal/alfacase/generate_case_description_docstring.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         "volume fraction",
         "volumetric thermal expansion",
     ]
 )
 
 
 def generate_list_of_units(category: str) -> str:
-    """ Return an admonition with toggle to show the units available for a given category. """
+    """Return an admonition with toggle to show the units available for a given category."""
     from barril.units import UnitDatabase
 
     unit_database = UnitDatabase.GetSingleton()
     units = unit_database.GetCategoryInfo(category).valid_units_set
     info = unit_database.unit_to_unit_info
     body = [f'    :"{unit}": {info[unit].name}' for unit in units]
     lines = [
@@ -107,30 +107,30 @@
 
     lines.extend(_generate_declaration_for_schema(class_name))
     lines.append("")
     return "\n".join(lines)
 
 
 def _generate_declaration_for_class(class_: Any) -> List[str]:
-    """ Return all attributes for the given Class with CaseDescription definition. """
+    """Return all attributes for the given Class with CaseDescription definition."""
     class_fields = attr.fields_dict(class_)
     return [
         f"{INDENT*2}class {class_.__name__}",
         *_get_declaration(class_fields, LIST_OF_CASE_ATTRIBUTES),
     ]
 
 
 def _generate_declaration_for_schema(class_: Any) -> List[str]:
-    """ Return all attributes for the given Class using ALFACase schema definition. """
+    """Return all attributes for the given Class using ALFACase schema definition."""
     class_fields = attr.fields_dict(class_)
     return _get_declaration(class_fields, LIST_OF_CASE_SCHEMAS, is_schema=True)
 
 
 def _get_case_attr_default_value(value: attr.Attribute) -> str:
-    """ Return the default value of a CaseDescription. """
+    """Return the default value of a CaseDescription."""
 
     if value.default == attr.NOTHING:
         return ""
 
     default_value_string = " = "
     if isinstance(value.default, enum.Enum):
         default_value_string += (
@@ -154,15 +154,15 @@
 
 
 def _get_declaration(
     class_: Dict[str, Attribute],
     list_of_predicate_and_handles: Sequence[Tuple[Callable, Callable]],
     is_schema: bool = False,
 ) -> List[str]:
-    """ Helper class to extract the logic to iterate over the attributes from the given class. """
+    """Helper class to extract the logic to iterate over the attributes from the given class."""
     lines = []
     for attribute_name, value in class_.items():
         if attribute_name not in IGNORED_PROPERTIES:
             for predicate_function, handle_function in list_of_predicate_and_handles:
                 if predicate_function(value.type):
                     attribute_value = handle_function(value.type)
                     default_value = _get_case_attr_default_value(value)
@@ -192,35 +192,35 @@
     """
     Return the name of the class with a valid reference to be used by sphinx.
     """
     return f"\\ :class:`{visible_name} <{ref}>`\\"
 
 
 def _get_scalar_reference() -> str:
-    """ Return a string with a cross-reference to Scalar documentation. """
+    """Return a string with a cross-reference to Scalar documentation."""
     return _get_class_with_reference(visible_name="Scalar", ref="barril.units.Scalar")
 
 
 def _get_array_reference() -> str:
-    """ Return a string with a cross-reference to Array documentation. """
+    """Return a string with a cross-reference to Array documentation."""
     return _get_class_with_reference(visible_name="Array", ref="barril.units.Array")
 
 
 def _get_list_reference() -> str:
-    """ Return a string with a cross-reference to List documentation. """
+    """Return a string with a cross-reference to List documentation."""
     return _get_class_with_reference(visible_name="List", ref="typing.List")
 
 
 def _get_dict_reference() -> str:
-    """ Return a string with a cross-reference to Dict documentation. """
+    """Return a string with a cross-reference to Dict documentation."""
     return _get_class_with_reference(visible_name="Dict", ref="typing.Dict")
 
 
 def _get_optional_reference() -> str:
-    """ Return a string with a cross-reference to Optional documentation. """
+    """Return a string with a cross-reference to Optional documentation."""
     return _get_class_with_reference(visible_name="Optional", ref="typing.Optional")
 
 
 def attrs_formatted(value: Any) -> str:
     """
     Return the attr class name with a cross-referencing link for the class.
     """
@@ -275,29 +275,29 @@
     else:
         name = ref_value.__name__
 
     return f"{optional_with_reference}[{name}]"
 
 
 def enum_formatted(value: Any) -> str:
-    """ Return the name of the Enum a cross-referencing link for the constants section. """
+    """Return the name of the Enum a cross-referencing link for the constants section."""
     name = value.__name__
     ref_name = f"{value.__module__}.{name}"
     return _get_class_with_reference(visible_name=name, ref=ref_name)
 
 
 def attrs_formatted_for_schema(value: Any) -> str:
-    """ Return the name of the schema with a reference for the API reference section. """
+    """Return the name of the schema with a reference for the API reference section."""
     return _get_class_with_reference(
         visible_name=obtain_schema_name(value), ref=value.__name__
     )
 
 
 def enum_formatted_for_schema(value: enum.EnumMeta) -> str:
-    """ Return the name of the schema with a reference for the API reference section. """
+    """Return the name of the schema with a reference for the API reference section."""
     return _get_class_with_reference(
         visible_name=obtain_schema_name(value),
         ref=f"{value.__module__}.{value.__name__}",
     )
 
 
 def list_formatted_for_schema(value: Any) -> str:
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk/__init__.py` & `alfasim_sdk-0.9.0/src/alfasim_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/PKG-INFO` & `alfasim_sdk-0.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alfasim-sdk
-Version: 0.8.0
+Name: alfasim_sdk
+Version: 0.9.0
 Summary: ALFAsim API/SDK
 Home-page: https://github.com/esss/alfasim-sdk
 Author: ESSS
 Author-email: foss@esss.co
 License: UNKNOWN
 Description: ===========
         alfasim-sdk
```

### Comparing `alfasim_sdk-0.8.0/src/alfasim_sdk.egg-info/SOURCES.txt` & `alfasim_sdk-0.9.0/src/alfasim_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alfasim_sdk-0.8.0/HISTORY.rst` & `alfasim_sdk-0.9.0/HISTORY.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 =======
 History
 =======
 
+0.9.0 (2021-05-04)
+==================
+
+* Add new CLI command called ``update``. It updates files automatically generated by alfasim-sdk.
+* Add gas and liquid separation efficiency to ``Separator`` model.
+* **Breaking Change**: Replaced radius from ``Separator`` geometry definition by diameter.
+* Add new hook to calculate relative emulsion viscosity and also add the possibility of choosing it in the ``PhysicsDescription``.
+
+
 0.8.0 (2021-04-12)
 ==================
 
 * Add context support on ``alfasim_configure_fields``, ``alfasim_configure_layers`` and ``alfasim_configure_phases``.
 * Change category for ``volumetric_flow_rates_std` from ``volume flow rate`` to ``standard volume per time``.
 * Rename ``convert_alfacase_to_case`` to ``convert_alfacase_to_description``.
 * Add new category: ``gas standard volume per time``, with same units as ``standard volume per time``.
```

### Comparing `alfasim_sdk-0.8.0/LICENSE` & `alfasim_sdk-0.9.0/LICENSE`

 * *Files identical despite different names*

