# Comparing `tmp/pzen-0.0.2.tar.gz` & `tmp/pzen-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pzen-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pzen-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pzen-0.0.2.tar` & `pzen-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      114 2024-03-14 21:06:12.177417 pzen-0.0.2/.flake8
--rw-r--r--   0        0        0     2014 2024-03-14 21:06:12.177417 pzen-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0        0        0       26 2024-03-14 21:06:12.177417 pzen-0.0.2/.gitignore
--rw-r--r--   0        0        0     1080 2024-03-14 21:06:12.177417 pzen-0.0.2/LICENSE
--rw-r--r--   0        0        0       29 2024-03-14 21:06:12.181417 pzen-0.0.2/README.md
--rw-r--r--   0        0        0       22 2024-03-14 21:06:12.181417 pzen-0.0.2/env.sh
--rw-r--r--   0        0        0      177 2024-03-14 21:06:12.181417 pzen-0.0.2/mypy.ini
--rw-r--r--   0        0        0      317 2024-03-14 21:06:12.181417 pzen-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       53 2024-03-14 21:06:12.181417 pzen-0.0.2/pzen/__init__.py
--rw-r--r--   0        0        0       47 2024-03-14 21:06:12.181417 pzen-0.0.2/pzen/core_types.py
--rw-r--r--   0        0        0     2072 2024-03-14 21:06:12.181417 pzen-0.0.2/pzen/soundfile_utils.py
--rw-r--r--   0        0        0       43 2024-03-14 21:06:12.181417 pzen-0.0.2/requirements_dev.txt
--rw-r--r--   0        0        0       22 2024-03-14 21:06:12.181417 pzen-0.0.2/requirements_opt.txt
--rwxr-xr-x   0        0        0      112 2024-03-14 21:06:12.181417 pzen-0.0.2/scripts/ci_all
--rwxr-xr-x   0        0        0       99 2024-03-14 21:06:12.181417 pzen-0.0.2/scripts/setup_dependencies.sh
--rwxr-xr-x   0        0        0      105 2024-03-14 21:06:12.181417 pzen-0.0.2/scripts/setup_venv.sh
--rw-r--r--   0        0        0      871 2024-03-14 21:06:12.181417 pzen-0.0.2/tests/pzen/test_soundfile_utils.py
--rw-r--r--   0        0        0      195 1970-01-01 00:00:00.000000 pzen-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      114 2024-04-03 20:02:19.932095 pzen-0.0.3/.flake8
+-rw-r--r--   0        0        0     2014 2024-04-03 20:02:19.932095 pzen-0.0.3/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0       26 2024-04-03 20:02:19.932095 pzen-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1080 2024-04-03 20:02:19.932095 pzen-0.0.3/LICENSE
+-rw-r--r--   0        0        0       29 2024-04-03 20:02:19.932095 pzen-0.0.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-03 20:02:19.932095 pzen-0.0.3/env.sh
+-rw-r--r--   0        0        0      222 2024-04-03 20:02:19.932095 pzen-0.0.3/mypy.ini
+-rw-r--r--   0        0        0      317 2024-04-03 20:02:19.932095 pzen-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       53 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/core_types.py
+-rw-r--r--   0        0        0     1988 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/numpy_utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/py.typed
+-rw-r--r--   0        0        0     2072 2024-04-03 20:02:19.932095 pzen-0.0.3/pzen/soundfile_utils.py
+-rw-r--r--   0        0        0       43 2024-04-03 20:02:19.932095 pzen-0.0.3/requirements_dev.txt
+-rw-r--r--   0        0        0       28 2024-04-03 20:02:19.932095 pzen-0.0.3/requirements_opt.txt
+-rwxr-xr-x   0        0        0      112 2024-04-03 20:02:19.932095 pzen-0.0.3/scripts/ci_all
+-rwxr-xr-x   0        0        0       99 2024-04-03 20:02:19.932095 pzen-0.0.3/scripts/setup_dependencies.sh
+-rwxr-xr-x   0        0        0      105 2024-04-03 20:02:19.932095 pzen-0.0.3/scripts/setup_venv.sh
+-rw-r--r--   0        0        0      952 2024-04-03 20:02:19.932095 pzen-0.0.3/tests/pzen/test_numpy_utils.py
+-rw-r--r--   0        0        0      871 2024-04-03 20:02:19.932095 pzen-0.0.3/tests/pzen/test_soundfile_utils.py
+-rw-r--r--   0        0        0      195 1970-01-01 00:00:00.000000 pzen-0.0.3/PKG-INFO
```

### Comparing `pzen-0.0.2/.github/workflows/ci.yaml` & `pzen-0.0.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pzen-0.0.2/LICENSE` & `pzen-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pzen-0.0.2/pzen/soundfile_utils.py` & `pzen-0.0.3/pzen/soundfile_utils.py`

 * *Files identical despite different names*

### Comparing `pzen-0.0.2/tests/pzen/test_soundfile_utils.py` & `pzen-0.0.3/tests/pzen/test_soundfile_utils.py`

 * *Files identical despite different names*

