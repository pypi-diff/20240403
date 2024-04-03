# Comparing `tmp/xyzservices-2023.7.0.tar.gz` & `tmp/xyzservices-2024.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xyzservices-2023.7.0.tar", last modified: Thu Jul 13 20:07:04 2023, max compression
+gzip compressed data, was "xyzservices-2024.4.0.tar", last modified: Wed Apr  3 18:47:56 2024, max compression
```

## Comparing `xyzservices-2023.7.0.tar` & `xyzservices-2024.4.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.443049 xyzservices-2023.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/workflows/release_to_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.github/workflows/update_providers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-13 20:07:04.443049 xyzservices-2023.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/ci/latest.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/ci/update_providers.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.435048 xyzservices-2023.7.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/_static/generate_gallery.js
--rw-r--r--   0 runner    (1001) docker     (123)   380575 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/_static/xyzmaps.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/gallery.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    35770 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/registration.md
--rw-r--r--   0 runner    (1001) docker     (123)   663316 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/doc/source/tiles.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/provider_sources/
--rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/provider_sources/_compress_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/provider_sources/_parse_leaflet_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)   143871 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/provider_sources/leaflet-providers-parsed.json
--rw-r--r--   0 runner    (1001) docker     (123)    25567 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/provider_sources/xyzservices-providers.json
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 20:07:04.443049 xyzservices-2023.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/xyzservices/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/xyzservices/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   432759 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/data/providers.json
--rw-r--r--   0 runner    (1001) docker     (123)    21475 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.443049 xyzservices-2023.7.0/xyzservices/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-13 20:06:57.000000 xyzservices-2023.7.0/xyzservices/tests/test_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 20:07:04.439048 xyzservices-2023.7.0/xyzservices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-13 20:07:04.000000 xyzservices-2023.7.0/xyzservices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-13 20:07:04.000000 xyzservices-2023.7.0/xyzservices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 20:07:04.000000 xyzservices-2023.7.0/xyzservices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 20:07:04.000000 xyzservices-2023.7.0/xyzservices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.065918 xyzservices-2024.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.057917 xyzservices-2024.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.057917 xyzservices-2024.4.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.057917 xyzservices-2024.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/.github/workflows/release_to_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/.github/workflows/update_providers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-03 18:47:56.065918 xyzservices-2024.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.057917 xyzservices-2024.4.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/ci/latest.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/ci/update_providers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.057917 xyzservices-2024.4.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.057917 xyzservices-2024.4.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.061918 xyzservices-2024.4.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)    10052 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/_static/generate_gallery.js
+-rw-r--r--   0 runner    (1001) docker     (127)   380575 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/_static/xyzmaps.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/gallery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4045 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35770 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4471 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/registration.md
+-rw-r--r--   0 runner    (1001) docker     (127)   663316 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/doc/source/tiles.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.061918 xyzservices-2024.4.0/provider_sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/provider_sources/_compress_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/provider_sources/_parse_leaflet_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151640 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/provider_sources/leaflet-providers-parsed.json
+-rw-r--r--   0 runner    (1001) docker     (127)    25927 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/provider_sources/xyzservices-providers.json
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:47:56.065918 xyzservices-2024.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.061918 xyzservices-2024.4.0/xyzservices/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/xyzservices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.065918 xyzservices-2024.4.0/xyzservices/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/xyzservices/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   701813 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/xyzservices/data/providers.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21475 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/xyzservices/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/xyzservices/providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.065918 xyzservices-2024.4.0/xyzservices/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/xyzservices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9139 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/xyzservices/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-03 18:47:48.000000 xyzservices-2024.4.0/xyzservices/tests/test_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:47:56.065918 xyzservices-2024.4.0/xyzservices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2024-04-03 18:47:56.000000 xyzservices-2024.4.0/xyzservices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-03 18:47:56.000000 xyzservices-2024.4.0/xyzservices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:47:56.000000 xyzservices-2024.4.0/xyzservices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 18:47:56.000000 xyzservices-2024.4.0/xyzservices.egg-info/top_level.txt
```

### Comparing `xyzservices-2023.7.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md` & `xyzservices-2024.4.0/.github/PULL_REQUEST_TEMPLATE/community_contribution.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/.github/workflows/release_to_pypi.yml` & `xyzservices-2024.4.0/.github/workflows/release_to_pypi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 jobs:
   build-n-publish:
     name: Build and publish xyzservices to PyPI
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout source
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: Set up Python
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: "3.x"
 
       - name: Build a binary wheel and a source tarball
         run: |
           python -m pip install --upgrade pip
           pip install setuptools wheel
```

### Comparing `xyzservices-2023.7.0/.github/workflows/tests.yaml` & `xyzservices-2024.4.0/.github/workflows/tests.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     - cron: "59 23 * * 3"
 
 jobs:
   Linting:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4
-      - uses: pre-commit/action@v3.0.0
+      - uses: actions/checkout@v4
+      - uses: actions/setup-python@v5
+      - uses: pre-commit/action@v3.0.1
 
   unittests:
     name: ${{ matrix.os }}, ${{ matrix.environment-file }}
     runs-on: ${{ matrix.os }}
     timeout-minutes: 120
     strategy:
       matrix:
@@ -38,32 +38,32 @@
       STADIA: ${{ secrets.STADIA }}
     defaults:
       run:
         shell: bash -l {0}
 
     steps:
       - name: checkout repo
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: setup micromamba
-        uses: mamba-org/provision-with-micromamba@main
+        uses: mamba-org/setup-micromamba@v1
         with:
           environment-file: ${{ matrix.environment-file }}
           micromamba-version: "latest"
 
       - name: Install xyzservices
         run: pip install .
 
       - name: run tests - bash
         run: pytest -v . -m "not request" --cov=xyzservices --cov-append --cov-report term-missing --cov-report xml --color=yes
 
       - name: test providers - bash
-        run: pytest -v . -m request --cov=xyzservices --cov-append --cov-report term-missing --cov-report xml --color=yes
+        run: pytest -v . -m request --cov=xyzservices --cov-append --cov-report term-missing --cov-report xml --color=yes -n auto
         if: matrix.os == 'ubuntu-latest'
 
       - name: remove JSON from share and test fallback
         run: |
           python -c 'import os, sys; os.remove(os.path.join(sys.prefix, "share", "xyzservices", "providers.json"))'
           pytest -v . -m "not request" --cov=xyzservices --cov-append --cov-report term-missing --cov-report xml --color=yes
         if: matrix.os != 'windows-latest'
 
-      - uses: codecov/codecov-action@v3
+      - uses: codecov/codecov-action@v4
```

### Comparing `xyzservices-2023.7.0/.github/workflows/update_providers.yaml` & `xyzservices-2024.4.0/.github/workflows/update_providers.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -17,18 +17,18 @@
     timeout-minutes: 30
     strategy:
       matrix:
         environment-file: [ci/update_providers.yaml]
 
     steps:
       - name: checkout repo
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
 
       - name: setup micromamba
-        uses: mamba-org/provision-with-micromamba@main
+        uses: mamba-org/setup-micromamba@v1
         with:
           environment-file: ${{ matrix.environment-file }}
           micromamba-version: 'latest'
 
       - name: Parse leaflet providers/compress output
         shell: bash -l {0}
         run: |
```

### Comparing `xyzservices-2023.7.0/.gitignore` & `xyzservices-2024.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/CHANGELOG.md` & `xyzservices-2024.4.0/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,41 @@
 Changelog
 =========
 
+xyzservices 2024.4.0 (April 3, 2024)
+------------------------------------
+
+Providers:
+
+- ``GeoportailFrance`` tiles are now using the new ``data.geopf.fr`` domain instead
+  of deprecated ``wxs.ign.fr`` (#166)
+- ``NASAGIBS.BlueMarble3413`` and ``NASAGIBS.BlueMarble3031`` URLs are now fixed (#162)
+- ```NASAGIBS.BlueMarble`` was removed as the URL no longer works.
+- ``Esri.DeLorme`` and ``NASAGIBS.ModisTerraChlorophyll`` are marked as broken.
+- Added ``BaseMapDE`` and ``TopPlusOpen`` providers.
+- Addded ``Jawg.Lagoon``, ``MapTiler.Ocean``, ``MapTiler.Backdrop``, ``MapTiler.Dataviz`` tiles.
+- Updated ``NLS`` to use their new ``MapTiler`` service.
+
+
+xyzservices 2023.10.1 (October 26, 2023)
+----------------------------------------
+
+Providers:
+
+- ``Stamen`` tiles have been removed due to their upstream deprecation.
+  Use ``Stamen`` styles of ``Stadia`` provider instead.
+- ``JusticeMap`` tiles are temporarily marked as broken.
+
+xyzservices 2023.10.0 (October 5, 2023)
+---------------------------------------
+
+Providers:
+
+- ``Stamen`` tiles are now available under ``Stadia`` provider.
+
 xyzservices 2023.7.0 (July 13, 2023)
 ------------------------------------
 
 Providers:
 
 - Added ``GeoportailFrance`` ``Orthoimagery_Orthophotos_Irc_express_2023`` and
   ``Orthoimagery_Orthophotos_Ortho_express_2023`` layers
```

### Comparing `xyzservices-2023.7.0/CONTRIBUTING.md` & `xyzservices-2024.4.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/LICENSE` & `xyzservices-2024.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/PKG-INFO` & `xyzservices-2024.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyzservices
-Version: 2023.7.0
+Version: 2024.4.0
 Summary: Source of XYZ tiles providers
 Home-page: https://github.com/geopandas/xyzservices
 Author: Dani Arribas-Bel, Martin Fleischmann
 Author-email: daniel.arribas.bel@gmail.com, martin@martinfleischmann.net
 License: 3-Clause BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyzservices-2023.7.0/README.md` & `xyzservices-2024.4.0/README.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/Makefile` & `xyzservices-2024.4.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/make.bat` & `xyzservices-2024.4.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/_static/custom.css` & `xyzservices-2024.4.0/doc/source/_static/custom.css`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/_static/generate_gallery.js` & `xyzservices-2024.4.0/doc/source/_static/generate_gallery.js`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/_static/xyzmaps.jpg` & `xyzservices-2024.4.0/doc/source/_static/xyzmaps.jpg`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/api.rst` & `xyzservices-2024.4.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/conf.py` & `xyzservices-2024.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/contributing.md` & `xyzservices-2024.4.0/doc/source/contributing.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/gallery.rst` & `xyzservices-2024.4.0/doc/source/gallery.rst`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/index.md` & `xyzservices-2024.4.0/doc/source/index.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/introduction.ipynb` & `xyzservices-2024.4.0/doc/source/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/registration.md` & `xyzservices-2024.4.0/doc/source/registration.md`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/doc/source/tiles.png` & `xyzservices-2024.4.0/doc/source/tiles.png`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/provider_sources/_compress_providers.py` & `xyzservices-2024.4.0/provider_sources/_compress_providers.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,28 +11,40 @@
 import warnings
 from datetime import date
 
 import requests
 import xmltodict
 
 # list of providers known to be broken and should be marked as broken in the JSON
-# last update: 14 Apr 2022
-BROKEN_PROVIDERS = []
+# last update: 4 Feb 2024
+BROKEN_PROVIDERS = [
+    "JusticeMap.income",
+    "JusticeMap.americanIndian",
+    "JusticeMap.asian",
+    "JusticeMap.black",
+    "JusticeMap.hispanic",
+    "JusticeMap.multi",
+    "JusticeMap.nonWhite",
+    "JusticeMap.white",
+    "JusticeMap.plurality",
+    "Esri.DeLorme",
+    "NASAGIBS.ModisTerraChlorophyll"
+]
 
 with open("./leaflet-providers-parsed.json") as f:
     leaflet = json.load(f)
     # remove meta data
     leaflet.pop("_meta", None)
 
 
 with open("./xyzservices-providers.json") as f:
     xyz = json.load(f)
 
 for provider in BROKEN_PROVIDERS:
-    provider = provider.replace(".", " ").split()
+    provider = provider.split(".")
     try:
         if len(provider) == 1:
             leaflet[provider[0]]["status"] = "broken"
         else:
             leaflet[provider[0]][provider[1]]["status"] = "broken"
     except:
         warnings.warn(
@@ -68,135 +80,118 @@
             leaflet[key].update(xyz[key])
         else:
             leaflet[key] = xyz[key]
     else:
         leaflet[key] = xyz[key]
 
 
-# add the IGN tile layers
+# Add IGN WMTS services (Tile images)
 
-leaflet["GeoportailFrance"]["plan"] = {}
-leaflet["GeoportailFrance"]["orthos"] = {}
-leaflet["GeoportailFrance"]["parcels"] = {}
-tilelayers_list = []
-apikey_list = [
-    "administratif",
-    "agriculture",
-    "altimetrie",
-    "cartes",
-    "clc",
-    "economie",
-    "environnement",
-    "essentiels",
-    "lambert93",
-    "ocsge",
-    "ortho",
-    "orthohisto",
-    "satellite",
-    "sol",
-    "topographie",
-    "transports",
-]
-url_template = (
-    "https://wxs.ign.fr/apikey/geoportail/wmts?REQUEST=GetCapabilities&SERVICE=wmts"
+ign_wmts_url = (
+    "https://data.geopf.fr/wmts?SERVICE=WMTS&VERSION=1.0.0&REQUEST=GetCapabilities"
 )
-for j in range(0, len(apikey_list)):
-    apikey = apikey_list[j]
-    url = url_template.replace("apikey", apikey)
-    resp = requests.get(url)
-    resp_dict = xmltodict.parse(resp.content)
-    layer_list = resp_dict["Capabilities"]["Contents"]["Layer"]
-    addictionnal_dict = {}
-
-    for i in range(len(layer_list)):
-        layer = resp_dict["Capabilities"]["Contents"]["Layer"][i]
-        variant = layer["ows:Identifier"]
-        name = ""
-        if "." not in variant:
-            name = variant.lower().capitalize()
-        else:
-            name = variant.split(".")[0].lower().capitalize()
-            for i in range(1, len(variant.split("."))):
-                name = name + "_" + (variant.split(".")[i]).lower().capitalize()
-                name = name.replace("-", "_")
-
-        if variant == "GEOGRAPHICALGRIDSYSTEMS.PLANIGNV2":
-            name = "plan"
-        if variant == "ORTHOIMAGERY.ORTHOPHOTOS":
-            name = "orthos"
-        if variant == "CADASTRALPARCELS.PARCELLAIRE_EXPRESS":
-            name = "parcels"
-
-        if "Style" in layer:
-            if type(layer["Style"]) is dict:
-                style = layer["Style"]["ows:Identifier"]
 
-            elif type(layer["Style"]) is list:
-                style = layer["Style"][1]["ows:Identifier"]
-        else:
-            style = "normal"
+response = requests.get(ign_wmts_url)
+response_dict = xmltodict.parse(response.content)
+layers_list = response_dict["Capabilities"]["Contents"]["Layer"] # 556 layers
+
+wmts_layers_list = []
+for i in range(len(layers_list)):
+    layer = response_dict["Capabilities"]["Contents"]["Layer"][i]
+    variant = layer.get("ows:Identifier")
+
+    # Rename for better readability
+    name = ""
+    if "." not in variant:
+        name = variant.lower().capitalize()
+    else:
+        name = variant.split(".")[0].lower().capitalize()
+        for i in range(1, len(variant.split("."))):
+            name = name + "_" + (variant.split(".")[i]).lower().capitalize()
+            name = name.replace("-", "_")
+
+    # Rename for better readability (Frequent cases)
+    variant_to_name = {
+        "CADASTRALPARCELS.PARCELLAIRE_EXPRESS": "parcels",
+        "GEOGRAPHICALGRIDSYSTEMS.PLANIGNV2": "plan",
+        "ORTHOIMAGERY.ORTHOPHOTOS": "orthos"
+    }
+
+    if variant in variant_to_name:
+        name = variant_to_name[variant]
+
+    # Get layer style
+    style = layer.get("Style")
+    if isinstance(style, dict):
+        style = style.get("ows:Identifier")
 
-        TileMatrixSetLimits = layer["TileMatrixSetLink"]["TileMatrixSetLimits"][
-            "TileMatrixLimits"
-        ]
-        min_zoom = int(TileMatrixSetLimits[0]["TileMatrix"])
-        max_zoom = int(TileMatrixSetLimits[-1]["TileMatrix"])
-        TileMatrixSet = layer["TileMatrixSetLink"]["TileMatrixSet"]
-        format = layer["Format"]
-        bounding_lowerleft_corner = layer["ows:WGS84BoundingBox"][
-            "ows:LowerCorner"
-        ]  # given with lon/lat order
-        bounding_upperright_corner = layer["ows:WGS84BoundingBox"][
-            "ows:UpperCorner"
-        ]  # given with lon/lat order
-        lowerleft_corner_lon, lowerleft_corner_lat = bounding_lowerleft_corner.split(
-            " "
-        )
-        upperright_corner_lon, upperright_corner_lat = bounding_upperright_corner.split(
-            " "
-        )
-        bounds = [
-            [float(lowerleft_corner_lat), float(lowerleft_corner_lon)],
-            [float(upperright_corner_lat), float(upperright_corner_lon)],
-        ]
-
-        if format == "application/x-protobuf":
-            pass
-        elif format == "image/x-bil;bits=32":
-            pass
-        elif apikey == "lambert93":
-            pass
-        else:
-            tilelayers_list.append("GeoportailFrance." + name)
-            leaflet["GeoportailFrance"][name] = {
-                "url": """https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}""",
-                "html_attribution": """<a target="_blank"href="https://www.geoportail.gouv.fr/">Geoportail France</a>""",
-                "attribution": "Geoportail France",
-                "bounds": bounds,
-                "min_zoom": min_zoom,
-                "max_zoom": max_zoom,
-                "apikey": apikey,
-                "format": format,
-                "style": style,
-                "variant": variant,
-                "name": "GeoportailFrance." + name,
-                "TileMatrixSet": TileMatrixSet,
-            }
-
-            possibly_broken = [
-                "Ocsge_Constructions_2002",
-                "Ocsge_Constructions_2014",
-                "Ocsge_Couverture_2002",
-                "Ocsge_Couverture_2014",
-                "Ocsge_Usage_2002",
-                "Ocsge_Usage_2014",
-                "Orthoimagery_Orthophotos_Coast2000",
-                "Pcrs_Lamb93",
-                "Orthoimagery_Ortho_sat_Spot_2013",
-                "Orthoimagery_Orthophotos_1980_1995",
-            ]
+    elif isinstance(style, list):
+        style = style[1].get("ows:Identifier") if len(style) > 1 else None
+    else:
+        style = "normal"
+
+    # Resolution levels (pyramid)
+    TileMatrixSet = layer["TileMatrixSetLink"]["TileMatrixSet"]
+
+    # Zoom levels
+    TileMatrixSetLimits = layer["TileMatrixSetLink"]["TileMatrixSetLimits"][
+        "TileMatrixLimits"
+    ]
+    min_zoom = int(TileMatrixSetLimits[0]["TileMatrix"])
+    max_zoom = int(TileMatrixSetLimits[-1]["TileMatrix"])
+
+    # Tile format
+    output_format = layer.get("Format") # image/png...
+    if output_format == "application/x-protobuf" or output_format == "image/x-bil;bits=32":
+        continue
+
+    # Layer extent
+    bbox_lower_left = layer["ows:WGS84BoundingBox"][
+        "ows:LowerCorner"
+    ]  # given with lon/lat order
+    bbox_upper_right = layer["ows:WGS84BoundingBox"][
+        "ows:UpperCorner"
+    ]  # given with lon/lat order
+    lower_left_corner_lon, lower_left_corner_lat = bbox_lower_left.split(
+        " "
+    )
+    upper_right_corner_lon, upper_right_corner_lat = bbox_upper_right.split(
+        " "
+    )
+    bounds = [
+        [float(lower_left_corner_lat), float(lower_left_corner_lon)],
+        [float(upper_right_corner_lat), float(upper_right_corner_lon)],
+    ]
+
+    wmts_layers_list.append("GeoportailFrance." + name)
+    leaflet["GeoportailFrance"][name] = {
+        "url": """https://data.geopf.fr/wmts?SERVICE=WMTS&VERSION=1.0.0&REQUEST=GetTile&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}""",
+        "html_attribution": """<a target="_blank"href="https://www.geoportail.gouv.fr/">Geoportail France</a>""",
+        "attribution": "Geoportail France",
+        "bounds": bounds,
+        "min_zoom": min_zoom,
+        "max_zoom": max_zoom,
+        "format": output_format,
+        "style": style,
+        "variant": variant,
+        "name": "GeoportailFrance." + name,
+        "TileMatrixSet": TileMatrixSet,
+        "apikey": "your_api_key_here",
+    }
+
+    # Handle broken providers
+    possibly_broken_providers = [
+        "Ocsge_Constructions_2002",
+        "Ocsge_Constructions_2014",
+        "Orthoimagery_Orthophotos_Coast2000",
+        "Ocsge_Couverture_2002",
+        "Ocsge_Couverture_2014",
+        "Ocsge_Usage_2002",
+        "Ocsge_Usage_2014",
+        "Pcrs_Lamb93",
+    ]
 
-            if name in possibly_broken:
-                leaflet["GeoportailFrance"][name]["status"] = "broken"
+    if name in possibly_broken_providers:
+        leaflet["GeoportailFrance"][name]["status"] = "broken"
 
 with open("../xyzservices/data/providers.json", "w") as f:
     json.dump(leaflet, f, indent=4)
```

### Comparing `xyzservices-2023.7.0/provider_sources/_parse_leaflet_providers.py` & `xyzservices-2024.4.0/provider_sources/_parse_leaflet_providers.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/provider_sources/leaflet-providers-parsed.json` & `xyzservices-2024.4.0/provider_sources/leaflet-providers-parsed.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8875586970899472%*

 * *Differences: {"'BaseMapDE'": "OrderedDict([('Color', OrderedDict([('url', "*

 * *                "'https://sgx.geodatenzentrum.de/wmts_basemapde/tile/1.0.0/{variant}/default/GLOBAL_WEBMERCATOR/{z}/{y}/{x}.png'), "*

 * *                "('html_attribution', 'Map data: &copy; <a "*

 * *                'href="http://www.govdata.de/dl-de/by-2-0">dl-de/by-2-0</a>\'), (\'attribution\', '*

 * *                "'Map data: (C) dl-de/by-2-0'), ('variant', 'de_basemapde_web_raster_farbe'), "*

 * *                "('name', 'BaseMapDE.Color')])), ('Grey', O […]*

```diff
@@ -69,14 +69,30 @@
             "name": "AzureMaps.MicrosoftWeatherRadarMain",
             "subscriptionKey": "<insert your subscription key here>",
             "timeStamp": "2021-05-08T09:03:00Z",
             "url": "https://atlas.microsoft.com/map/tile?api-version={apiVersion}&tilesetId={variant}&x={x}&y={y}&zoom={z}&timeStamp={timeStamp}&language={language}&subscription-key={subscriptionKey}",
             "variant": "microsoft.weather.radar.main"
         }
     },
+    "BaseMapDE": {
+        "Color": {
+            "attribution": "Map data: (C) dl-de/by-2-0",
+            "html_attribution": "Map data: &copy; <a href=\"http://www.govdata.de/dl-de/by-2-0\">dl-de/by-2-0</a>",
+            "name": "BaseMapDE.Color",
+            "url": "https://sgx.geodatenzentrum.de/wmts_basemapde/tile/1.0.0/{variant}/default/GLOBAL_WEBMERCATOR/{z}/{y}/{x}.png",
+            "variant": "de_basemapde_web_raster_farbe"
+        },
+        "Grey": {
+            "attribution": "Map data: (C) dl-de/by-2-0",
+            "html_attribution": "Map data: &copy; <a href=\"http://www.govdata.de/dl-de/by-2-0\">dl-de/by-2-0</a>",
+            "name": "BaseMapDE.Grey",
+            "url": "https://sgx.geodatenzentrum.de/wmts_basemapde/tile/1.0.0/{variant}/default/GLOBAL_WEBMERCATOR/{z}/{y}/{x}.png",
+            "variant": "de_basemapde_web_raster_grau"
+        }
+    },
     "BasemapAT": {
         "basemap": {
             "attribution": "Datenquelle: basemap.at",
             "bounds": [
                 [
                     46.35877,
                     8.782379
@@ -86,23 +102,16 @@
                     17.189532
                 ]
             ],
             "format": "png",
             "html_attribution": "Datenquelle: <a href=\"https://www.basemap.at\">basemap.at</a>",
             "max_zoom": 20,
             "name": "BasemapAT.basemap",
-            "subdomains": [
-                "",
-                "1",
-                "2",
-                "3",
-                "4"
-            ],
             "type": "normal",
-            "url": "https://maps{s}.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
+            "url": "https://mapsneu.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
             "variant": "geolandbasemap"
         },
         "grau": {
             "attribution": "Datenquelle: basemap.at",
             "bounds": [
                 [
                     46.35877,
@@ -113,23 +122,16 @@
                     17.189532
                 ]
             ],
             "format": "png",
             "html_attribution": "Datenquelle: <a href=\"https://www.basemap.at\">basemap.at</a>",
             "max_zoom": 19,
             "name": "BasemapAT.grau",
-            "subdomains": [
-                "",
-                "1",
-                "2",
-                "3",
-                "4"
-            ],
             "type": "normal",
-            "url": "https://maps{s}.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
+            "url": "https://mapsneu.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
             "variant": "bmapgrau"
         },
         "highdpi": {
             "attribution": "Datenquelle: basemap.at",
             "bounds": [
                 [
                     46.35877,
@@ -140,23 +142,16 @@
                     17.189532
                 ]
             ],
             "format": "jpeg",
             "html_attribution": "Datenquelle: <a href=\"https://www.basemap.at\">basemap.at</a>",
             "max_zoom": 19,
             "name": "BasemapAT.highdpi",
-            "subdomains": [
-                "",
-                "1",
-                "2",
-                "3",
-                "4"
-            ],
             "type": "normal",
-            "url": "https://maps{s}.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
+            "url": "https://mapsneu.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
             "variant": "bmaphidpi"
         },
         "orthofoto": {
             "attribution": "Datenquelle: basemap.at",
             "bounds": [
                 [
                     46.35877,
@@ -167,23 +162,16 @@
                     17.189532
                 ]
             ],
             "format": "jpeg",
             "html_attribution": "Datenquelle: <a href=\"https://www.basemap.at\">basemap.at</a>",
             "max_zoom": 20,
             "name": "BasemapAT.orthofoto",
-            "subdomains": [
-                "",
-                "1",
-                "2",
-                "3",
-                "4"
-            ],
             "type": "normal",
-            "url": "https://maps{s}.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
+            "url": "https://mapsneu.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
             "variant": "bmaporthofoto30cm"
         },
         "overlay": {
             "attribution": "Datenquelle: basemap.at",
             "bounds": [
                 [
                     46.35877,
@@ -194,23 +182,16 @@
                     17.189532
                 ]
             ],
             "format": "png",
             "html_attribution": "Datenquelle: <a href=\"https://www.basemap.at\">basemap.at</a>",
             "max_zoom": 19,
             "name": "BasemapAT.overlay",
-            "subdomains": [
-                "",
-                "1",
-                "2",
-                "3",
-                "4"
-            ],
             "type": "normal",
-            "url": "https://maps{s}.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
+            "url": "https://mapsneu.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
             "variant": "bmapoverlay"
         },
         "surface": {
             "attribution": "Datenquelle: basemap.at",
             "bounds": [
                 [
                     46.35877,
@@ -221,23 +202,16 @@
                     17.189532
                 ]
             ],
             "format": "jpeg",
             "html_attribution": "Datenquelle: <a href=\"https://www.basemap.at\">basemap.at</a>",
             "max_zoom": 19,
             "name": "BasemapAT.surface",
-            "subdomains": [
-                "",
-                "1",
-                "2",
-                "3",
-                "4"
-            ],
             "type": "grau",
-            "url": "https://maps{s}.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
+            "url": "https://mapsneu.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
             "variant": "bmapoberflaeche"
         },
         "terrain": {
             "attribution": "Datenquelle: basemap.at",
             "bounds": [
                 [
                     46.35877,
@@ -248,23 +222,16 @@
                     17.189532
                 ]
             ],
             "format": "jpeg",
             "html_attribution": "Datenquelle: <a href=\"https://www.basemap.at\">basemap.at</a>",
             "max_zoom": 19,
             "name": "BasemapAT.terrain",
-            "subdomains": [
-                "",
-                "1",
-                "2",
-                "3",
-                "4"
-            ],
             "type": "grau",
-            "url": "https://maps{s}.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
+            "url": "https://mapsneu.wien.gv.at/basemap/{variant}/{type}/google3857/{z}/{y}/{x}.{format}",
             "variant": "bmapgelaende"
         }
     },
     "CartoDB": {
         "DarkMatter": {
             "attribution": "(C) OpenStreetMap contributors (C) CARTO",
             "html_attribution": "&copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors &copy; <a href=\"https://carto.com/attributions\">CARTO</a>",
@@ -460,1031 +427,1031 @@
         "min_zoom": 8,
         "name": "FreeMapSK",
         "subdomains": "abcd",
         "url": "https://{s}.freemap.sk/T/{z}/{x}/{y}.jpeg"
     },
     "GeoportailFrance": {
         "orthos": {
-            "apikey": "choisirgeoportail",
+            "TileMatrixSet": "PM",
             "attribution": "Geoportail France",
             "bounds": [
                 [
-                    -75,
-                    -180
+                    -89.0,
+                    -180.0
                 ],
                 [
-                    81,
-                    180
+                    89.0,
+                    180.0
                 ]
             ],
             "format": "image/jpeg",
-            "html_attribution": "<a target=\"_blank\" href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
-            "max_zoom": 19,
-            "min_zoom": 2,
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 20,
+            "min_zoom": 0,
             "name": "GeoportailFrance.orthos",
             "style": "normal",
-            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET=PM&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "url": "https://data.geopf.fr/wmts?SERVICE=WMTS&VERSION=1.0.0&REQUEST=GetTile&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "ORTHOIMAGERY.ORTHOPHOTOS"
         },
         "parcels": {
-            "apikey": "choisirgeoportail",
+            "TileMatrixSet": "PM",
             "attribution": "Geoportail France",
             "bounds": [
                 [
-                    -75,
-                    -180
+                    -21.4756,
+                    -63.3725
                 ],
                 [
-                    81,
-                    180
+                    51.3121,
+                    55.9259
                 ]
             ],
             "format": "image/png",
-            "html_attribution": "<a target=\"_blank\" href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
-            "max_zoom": 20,
-            "min_zoom": 2,
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 19,
+            "min_zoom": 0,
             "name": "GeoportailFrance.parcels",
             "style": "PCI vecteur",
-            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET=PM&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "url": "https://data.geopf.fr/wmts?SERVICE=WMTS&VERSION=1.0.0&REQUEST=GetTile&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "CADASTRALPARCELS.PARCELLAIRE_EXPRESS"
         },
         "plan": {
-            "apikey": "choisirgeoportail",
+            "TileMatrixSet": "PM",
             "attribution": "Geoportail France",
             "bounds": [
                 [
-                    -75,
-                    -180
+                    -85.0,
+                    -175.0
                 ],
                 [
-                    81,
-                    180
+                    85.0,
+                    175.0
                 ]
             ],
             "format": "image/png",
-            "html_attribution": "<a target=\"_blank\" href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
-            "max_zoom": 18,
-            "min_zoom": 2,
+            "html_attribution": "<a target=\"_blank\"href=\"https://www.geoportail.gouv.fr/\">Geoportail France</a>",
+            "max_zoom": 19,
+            "min_zoom": 0,
             "name": "GeoportailFrance.plan",
             "style": "normal",
-            "url": "https://wxs.ign.fr/{apikey}/geoportail/wmts?REQUEST=GetTile&SERVICE=WMTS&VERSION=1.0.0&STYLE={style}&TILEMATRIXSET=PM&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
+            "url": "https://data.geopf.fr/wmts?SERVICE=WMTS&VERSION=1.0.0&REQUEST=GetTile&STYLE={style}&TILEMATRIXSET={TileMatrixSet}&FORMAT={format}&LAYER={variant}&TILEMATRIX={z}&TILEROW={y}&TILECOL={x}",
             "variant": "GEOGRAPHICALGRIDSYSTEMS.PLANIGNV2"
         }
     },
     "HERE": {
         "basicMap": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.basicMap",
             "size": "256",
             "subdomains": "1234",
             "type": "basetile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day"
         },
         "carnavDayGrey": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.carnavDayGrey",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "carnav.day.grey"
         },
         "hybridDay": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.hybridDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "hybrid.day"
         },
         "hybridDayGrey": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.hybridDayGrey",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "hybrid.grey.day"
         },
         "hybridDayMobile": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.hybridDayMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "hybrid.day.mobile"
         },
         "hybridDayTraffic": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "traffic",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.hybridDayTraffic",
             "size": "256",
             "subdomains": "1234",
             "type": "traffictile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "hybrid.traffic.day"
         },
         "hybridDayTransit": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.hybridDayTransit",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "hybrid.day.transit"
         },
         "mapLabels": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.mapLabels",
             "size": "256",
             "subdomains": "1234",
             "type": "labeltile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day"
         },
         "normalDay": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day"
         },
         "normalDayCustom": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalDayCustom",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day.custom"
         },
         "normalDayGrey": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalDayGrey",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day.grey"
         },
         "normalDayGreyMobile": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalDayGreyMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day.grey.mobile"
         },
         "normalDayMobile": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalDayMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day.mobile"
         },
         "normalDayTraffic": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "traffic",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalDayTraffic",
             "size": "256",
             "subdomains": "1234",
             "type": "traffictile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.traffic.day"
         },
         "normalDayTransit": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalDayTransit",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day.transit"
         },
         "normalDayTransitMobile": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalDayTransitMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day.transit.mobile"
         },
         "normalNight": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalNight",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.night"
         },
         "normalNightGrey": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalNightGrey",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.night.grey"
         },
         "normalNightGreyMobile": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalNightGreyMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.night.grey.mobile"
         },
         "normalNightMobile": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalNightMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.night.mobile"
         },
         "normalNightTransit": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalNightTransit",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.night.transit"
         },
         "normalNightTransitMobile": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.normalNightTransitMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.night.transit.mobile"
         },
         "pedestrianDay": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.pedestrianDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "pedestrian.day"
         },
         "pedestrianNight": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.pedestrianNight",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "pedestrian.night"
         },
         "reducedDay": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.reducedDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "reduced.day"
         },
         "reducedNight": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.reducedNight",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "reduced.night"
         },
         "satelliteDay": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.satelliteDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "satellite.day"
         },
         "terrainDay": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.terrainDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "terrain.day"
         },
         "terrainDayMobile": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.terrainDayMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "terrain.day.mobile"
         },
         "trafficFlow": {
             "app_code": "<insert your app_code here>",
             "app_id": "<insert your app_id here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "traffic",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HERE.trafficFlow",
             "size": "256",
             "subdomains": "1234",
             "type": "flowtile",
             "url": "https://{s}.{base}.maps.api.here.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?app_id={app_id}&app_code={app_code}&lg={language}",
             "variant": "normal.day"
         }
     },
     "HEREv3": {
         "basicMap": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.basicMap",
             "size": "256",
             "subdomains": "1234",
             "type": "basetile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day"
         },
         "carnavDayGrey": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.carnavDayGrey",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "carnav.day.grey"
         },
         "hybridDay": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.hybridDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "hybrid.day"
         },
         "hybridDayGrey": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.hybridDayGrey",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "hybrid.grey.day"
         },
         "hybridDayMobile": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.hybridDayMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "hybrid.day.mobile"
         },
         "hybridDayTransit": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.hybridDayTransit",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "hybrid.day.transit"
         },
         "mapLabels": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.mapLabels",
             "size": "256",
             "subdomains": "1234",
             "type": "labeltile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day"
         },
         "normalDay": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day"
         },
         "normalDayCustom": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalDayCustom",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day.custom"
         },
         "normalDayGrey": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalDayGrey",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day.grey"
         },
         "normalDayGreyMobile": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalDayGreyMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day.grey.mobile"
         },
         "normalDayMobile": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalDayMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day.mobile"
         },
         "normalDayTransit": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalDayTransit",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day.transit"
         },
         "normalDayTransitMobile": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalDayTransitMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.day.transit.mobile"
         },
         "normalNight": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalNight",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.night"
         },
         "normalNightGrey": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalNightGrey",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.night.grey"
         },
         "normalNightGreyMobile": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalNightGreyMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.night.grey.mobile"
         },
         "normalNightMobile": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalNightMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.night.mobile"
         },
         "normalNightTransit": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalNightTransit",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.night.transit"
         },
         "normalNightTransitMobile": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.normalNightTransitMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "normal.night.transit.mobile"
         },
         "pedestrianDay": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.pedestrianDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "pedestrian.day"
         },
         "pedestrianNight": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.pedestrianNight",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "pedestrian.night"
         },
         "reducedDay": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.reducedDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "reduced.day"
         },
         "reducedNight": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "base",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.reducedNight",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "reduced.night"
         },
         "satelliteDay": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.satelliteDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "satellite.day"
         },
         "terrainDay": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.terrainDay",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "terrain.day"
         },
         "terrainDayMobile": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "aerial",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.terrainDayMobile",
             "size": "256",
             "subdomains": "1234",
             "type": "maptile",
             "url": "https://{s}.{base}.maps.ls.hereapi.com/maptile/2.1/{type}/{mapID}/{variant}/{z}/{x}/{y}/{size}/{format}?apiKey={apiKey}&lg={language}",
             "variant": "terrain.day.mobile"
         },
         "trafficFlow": {
             "apiKey": "<insert your apiKey here>",
-            "attribution": "Map (C) 1987-2023 HERE",
+            "attribution": "Map (C) 1987-2024 HERE",
             "base": "traffic",
             "format": "png8",
-            "html_attribution": "Map &copy; 1987-2023 <a href=\"http://developer.here.com\">HERE</a>",
+            "html_attribution": "Map &copy; 1987-2024 <a href=\"http://developer.here.com\">HERE</a>",
             "language": "eng",
             "mapID": "newest",
             "max_zoom": 20,
             "name": "HEREv3.trafficFlow",
             "size": "256",
             "subdomains": "1234",
             "type": "flowtile",
@@ -1510,75 +1477,79 @@
             "variant": "hillshading"
         }
     },
     "Jawg": {
         "Dark": {
             "accessToken": "<insert your access token here>",
             "attribution": "(C) **Jawg** Maps (C) OpenStreetMap contributors",
-            "html_attribution": "<a href=\"http://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "<a href=\"https://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 22,
             "min_zoom": 0,
             "name": "Jawg.Dark",
-            "subdomains": "abcd",
-            "url": "https://{s}.tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
+            "url": "https://tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
             "variant": "jawg-dark"
         },
+        "Lagoon": {
+            "accessToken": "<insert your access token here>",
+            "attribution": "(C) **Jawg** Maps (C) OpenStreetMap contributors",
+            "html_attribution": "<a href=\"https://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "max_zoom": 22,
+            "min_zoom": 0,
+            "name": "Jawg.Lagoon",
+            "url": "https://tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
+            "variant": "jawg-lagoon"
+        },
         "Light": {
             "accessToken": "<insert your access token here>",
             "attribution": "(C) **Jawg** Maps (C) OpenStreetMap contributors",
-            "html_attribution": "<a href=\"http://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "<a href=\"https://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 22,
             "min_zoom": 0,
             "name": "Jawg.Light",
-            "subdomains": "abcd",
-            "url": "https://{s}.tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
+            "url": "https://tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
             "variant": "jawg-light"
         },
         "Matrix": {
             "accessToken": "<insert your access token here>",
             "attribution": "(C) **Jawg** Maps (C) OpenStreetMap contributors",
-            "html_attribution": "<a href=\"http://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "<a href=\"https://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 22,
             "min_zoom": 0,
             "name": "Jawg.Matrix",
-            "subdomains": "abcd",
-            "url": "https://{s}.tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
+            "url": "https://tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
             "variant": "jawg-matrix"
         },
         "Streets": {
             "accessToken": "<insert your access token here>",
             "attribution": "(C) **Jawg** Maps (C) OpenStreetMap contributors",
-            "html_attribution": "<a href=\"http://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "<a href=\"https://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 22,
             "min_zoom": 0,
             "name": "Jawg.Streets",
-            "subdomains": "abcd",
-            "url": "https://{s}.tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
+            "url": "https://tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
             "variant": "jawg-streets"
         },
         "Sunny": {
             "accessToken": "<insert your access token here>",
             "attribution": "(C) **Jawg** Maps (C) OpenStreetMap contributors",
-            "html_attribution": "<a href=\"http://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "<a href=\"https://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 22,
             "min_zoom": 0,
             "name": "Jawg.Sunny",
-            "subdomains": "abcd",
-            "url": "https://{s}.tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
+            "url": "https://tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
             "variant": "jawg-sunny"
         },
         "Terrain": {
             "accessToken": "<insert your access token here>",
             "attribution": "(C) **Jawg** Maps (C) OpenStreetMap contributors",
-            "html_attribution": "<a href=\"http://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "<a href=\"https://jawg.io\" title=\"Tiles Courtesy of Jawg Maps\" target=\"_blank\">&copy; <b>Jawg</b>Maps</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 22,
             "min_zoom": 0,
             "name": "Jawg.Terrain",
-            "subdomains": "abcd",
-            "url": "https://{s}.tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
+            "url": "https://tile.jawg.io/{variant}/{z}/{x}/{y}{r}.png?access-token={accessToken}",
             "variant": "jawg-terrain"
         }
     },
     "JusticeMap": {
         "americanIndian": {
             "attribution": "Justice Map",
             "bounds": [
@@ -1750,14 +1721,27 @@
         "max_zoom": 18,
         "name": "MapBox",
         "tileSize": 512,
         "url": "https://api.mapbox.com/styles/v1/{id}/tiles/{z}/{x}/{y}{r}?access_token={accessToken}",
         "zoomOffset": -1
     },
     "MapTiler": {
+        "Backdrop": {
+            "attribution": "(C) MapTiler (C) OpenStreetMap contributors",
+            "ext": "png",
+            "html_attribution": "<a href=\"https://www.maptiler.com/copyright/\" target=\"_blank\">&copy; MapTiler</a> <a href=\"https://www.openstreetmap.org/copyright\" target=\"_blank\">&copy; OpenStreetMap contributors</a>",
+            "key": "<insert your MapTiler Cloud API key here>",
+            "max_zoom": 21,
+            "min_zoom": 0,
+            "name": "MapTiler.Backdrop",
+            "tileSize": 512,
+            "url": "https://api.maptiler.com/maps/{variant}/{z}/{x}/{y}{r}.{ext}?key={key}",
+            "variant": "backdrop",
+            "zoomOffset": -1
+        },
         "Basic": {
             "attribution": "(C) MapTiler (C) OpenStreetMap contributors",
             "ext": "png",
             "html_attribution": "<a href=\"https://www.maptiler.com/copyright/\" target=\"_blank\">&copy; MapTiler</a> <a href=\"https://www.openstreetmap.org/copyright\" target=\"_blank\">&copy; OpenStreetMap contributors</a>",
             "key": "<insert your MapTiler Cloud API key here>",
             "max_zoom": 21,
             "min_zoom": 0,
@@ -1776,27 +1760,53 @@
             "min_zoom": 0,
             "name": "MapTiler.Bright",
             "tileSize": 512,
             "url": "https://api.maptiler.com/maps/{variant}/{z}/{x}/{y}{r}.{ext}?key={key}",
             "variant": "bright",
             "zoomOffset": -1
         },
+        "Dataviz": {
+            "attribution": "(C) MapTiler (C) OpenStreetMap contributors",
+            "ext": "png",
+            "html_attribution": "<a href=\"https://www.maptiler.com/copyright/\" target=\"_blank\">&copy; MapTiler</a> <a href=\"https://www.openstreetmap.org/copyright\" target=\"_blank\">&copy; OpenStreetMap contributors</a>",
+            "key": "<insert your MapTiler Cloud API key here>",
+            "max_zoom": 21,
+            "min_zoom": 0,
+            "name": "MapTiler.Dataviz",
+            "tileSize": 512,
+            "url": "https://api.maptiler.com/maps/{variant}/{z}/{x}/{y}{r}.{ext}?key={key}",
+            "variant": "dataviz",
+            "zoomOffset": -1
+        },
         "Hybrid": {
             "attribution": "(C) MapTiler (C) OpenStreetMap contributors",
             "ext": "jpg",
             "html_attribution": "<a href=\"https://www.maptiler.com/copyright/\" target=\"_blank\">&copy; MapTiler</a> <a href=\"https://www.openstreetmap.org/copyright\" target=\"_blank\">&copy; OpenStreetMap contributors</a>",
             "key": "<insert your MapTiler Cloud API key here>",
             "max_zoom": 21,
             "min_zoom": 0,
             "name": "MapTiler.Hybrid",
             "tileSize": 512,
             "url": "https://api.maptiler.com/maps/{variant}/{z}/{x}/{y}{r}.{ext}?key={key}",
             "variant": "hybrid",
             "zoomOffset": -1
         },
+        "Ocean": {
+            "attribution": "(C) MapTiler (C) OpenStreetMap contributors",
+            "ext": "png",
+            "html_attribution": "<a href=\"https://www.maptiler.com/copyright/\" target=\"_blank\">&copy; MapTiler</a> <a href=\"https://www.openstreetmap.org/copyright\" target=\"_blank\">&copy; OpenStreetMap contributors</a>",
+            "key": "<insert your MapTiler Cloud API key here>",
+            "max_zoom": 21,
+            "min_zoom": 0,
+            "name": "MapTiler.Ocean",
+            "tileSize": 512,
+            "url": "https://api.maptiler.com/maps/{variant}/{z}/{x}/{y}{r}.{ext}?key={key}",
+            "variant": "ocean",
+            "zoomOffset": -1
+        },
         "Pastel": {
             "attribution": "(C) MapTiler (C) OpenStreetMap contributors",
             "ext": "png",
             "html_attribution": "<a href=\"https://www.maptiler.com/copyright/\" target=\"_blank\">&copy; MapTiler</a> <a href=\"https://www.openstreetmap.org/copyright\" target=\"_blank\">&copy; OpenStreetMap contributors</a>",
             "key": "<insert your MapTiler Cloud API key here>",
             "max_zoom": 21,
             "min_zoom": 0,
@@ -2064,31 +2074,154 @@
             "tilematrixset": "GoogleMapsCompatible_Level",
             "time": "",
             "url": "https://map1.vis.earthdata.nasa.gov/wmts-webmerc/{variant}/default/{time}/{tilematrixset}{max_zoom}/{z}/{y}/{x}.{format}",
             "variant": "VIIRS_CityLights_2012"
         }
     },
     "NLS": {
-        "attribution": "National Library of Scotland Historic Maps",
-        "bounds": [
-            [
-                49.6,
-                -12
+        "osgb10k1888": {
+            "apikey": "<insert your API key here>",
+            "attribution": "National Library of Scotland Historic Maps",
+            "bounds": [
+                [
+                    49.6,
+                    -12
+                ],
+                [
+                    61.7,
+                    3
+                ]
             ],
-            [
-                61.7,
-                3
-            ]
-        ],
-        "html_attribution": "<a href=\"http://geo.nls.uk/maps/\">National Library of Scotland Historic Maps</a>",
-        "max_zoom": 18,
-        "min_zoom": 1,
-        "name": "NLS",
-        "subdomains": "0123",
-        "url": "https://nls-{s}.tileserver.com/nls/{z}/{x}/{y}.jpg"
+            "html_attribution": "<a href=\"http://maps.nls.uk/projects/subscription-api\">National Library of Scotland Historic Maps</a>",
+            "max_zoom": 18,
+            "min_zoom": 1,
+            "name": "NLS.osgb10k1888",
+            "url": "https://api.maptiler.com/tiles/{variant}/{z}/{x}/{y}.jpg?key={apikey}",
+            "variant": "uk-osgb10k1888"
+        },
+        "osgb1888": {
+            "apikey": "<insert your API key here>",
+            "attribution": "National Library of Scotland Historic Maps",
+            "bounds": [
+                [
+                    49.6,
+                    -12
+                ],
+                [
+                    61.7,
+                    3
+                ]
+            ],
+            "html_attribution": "<a href=\"http://maps.nls.uk/projects/subscription-api\">National Library of Scotland Historic Maps</a>",
+            "max_zoom": 18,
+            "min_zoom": 1,
+            "name": "NLS.osgb1888",
+            "url": "https://api.maptiler.com/tiles/{variant}/{z}/{x}/{y}.jpg?key={apikey}",
+            "variant": "uk-osgb1888"
+        },
+        "osgb1919": {
+            "apikey": "<insert your API key here>",
+            "attribution": "National Library of Scotland Historic Maps",
+            "bounds": [
+                [
+                    49.6,
+                    -12
+                ],
+                [
+                    61.7,
+                    3
+                ]
+            ],
+            "html_attribution": "<a href=\"http://maps.nls.uk/projects/subscription-api\">National Library of Scotland Historic Maps</a>",
+            "max_zoom": 18,
+            "min_zoom": 1,
+            "name": "NLS.osgb1919",
+            "url": "https://api.maptiler.com/tiles/{variant}/{z}/{x}/{y}.jpg?key={apikey}",
+            "variant": "uk-osgb1919"
+        },
+        "osgb25k1937": {
+            "apikey": "<insert your API key here>",
+            "attribution": "National Library of Scotland Historic Maps",
+            "bounds": [
+                [
+                    49.6,
+                    -12
+                ],
+                [
+                    61.7,
+                    3
+                ]
+            ],
+            "html_attribution": "<a href=\"http://maps.nls.uk/projects/subscription-api\">National Library of Scotland Historic Maps</a>",
+            "max_zoom": 18,
+            "min_zoom": 1,
+            "name": "NLS.osgb25k1937",
+            "url": "https://api.maptiler.com/tiles/{variant}/{z}/{x}/{y}.jpg?key={apikey}",
+            "variant": "uk-osgb25k1937"
+        },
+        "osgb63k1885": {
+            "apikey": "<insert your API key here>",
+            "attribution": "National Library of Scotland Historic Maps",
+            "bounds": [
+                [
+                    49.6,
+                    -12
+                ],
+                [
+                    61.7,
+                    3
+                ]
+            ],
+            "html_attribution": "<a href=\"http://maps.nls.uk/projects/subscription-api\">National Library of Scotland Historic Maps</a>",
+            "max_zoom": 18,
+            "min_zoom": 1,
+            "name": "NLS.osgb63k1885",
+            "url": "https://api.maptiler.com/tiles/{variant}/{z}/{x}/{y}.jpg?key={apikey}",
+            "variant": "uk-osgb63k1885"
+        },
+        "osgb63k1955": {
+            "apikey": "<insert your API key here>",
+            "attribution": "National Library of Scotland Historic Maps",
+            "bounds": [
+                [
+                    49.6,
+                    -12
+                ],
+                [
+                    61.7,
+                    3
+                ]
+            ],
+            "html_attribution": "<a href=\"http://maps.nls.uk/projects/subscription-api\">National Library of Scotland Historic Maps</a>",
+            "max_zoom": 18,
+            "min_zoom": 1,
+            "name": "NLS.osgb63k1955",
+            "url": "https://api.maptiler.com/tiles/{variant}/{z}/{x}/{y}.jpg?key={apikey}",
+            "variant": "uk-osgb63k1955"
+        },
+        "oslondon1k1893": {
+            "apikey": "<insert your API key here>",
+            "attribution": "National Library of Scotland Historic Maps",
+            "bounds": [
+                [
+                    49.6,
+                    -12
+                ],
+                [
+                    61.7,
+                    3
+                ]
+            ],
+            "html_attribution": "<a href=\"http://maps.nls.uk/projects/subscription-api\">National Library of Scotland Historic Maps</a>",
+            "max_zoom": 18,
+            "min_zoom": 1,
+            "name": "NLS.oslondon1k1893",
+            "url": "https://api.maptiler.com/tiles/{variant}/{z}/{x}/{y}.jpg?key={apikey}",
+            "variant": "uk-oslondon1k1893"
+        }
     },
     "OPNVKarte": {
         "attribution": "Map memomaps.de CC-BY-SA, map data (C) OpenStreetMap contributors",
         "html_attribution": "Map <a href=\"https://memomaps.de/\">memomaps.de</a> <a href=\"http://creativecommons.org/licenses/by-sa/2.0/\">CC-BY-SA</a>, map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
         "max_zoom": 18,
         "name": "OPNVKarte",
         "url": "https://tileserver.memomaps.de/tilegen/{z}/{x}/{y}.png"
@@ -2421,195 +2554,152 @@
         "html_attribution": "Map data: &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors | Map style: &copy; <a href=\"https://blog.safecast.org/about/\">SafeCast</a> (<a href=\"https://creativecommons.org/licenses/by-sa/3.0/\">CC-BY-SA</a>)",
         "max_zoom": 16,
         "name": "SafeCast",
         "url": "https://s3.amazonaws.com/te512.safecast.org/{z}/{x}/{y}.png"
     },
     "Stadia": {
         "AlidadeSmooth": {
-            "attribution": "(C) Stadia Maps, (C) OpenMapTiles (C) OpenStreetMap contributors",
-            "html_attribution": "&copy; <a href=\"https://stadiamaps.com/\">Stadia Maps</a>, &copy; <a href=\"https://openmaptiles.org/\">OpenMapTiles</a> &copy; <a href=\"http://openstreetmap.org\">OpenStreetMap</a> contributors",
+            "attribution": "(C) Stadia Maps (C) OpenMapTiles (C) OpenStreetMap contributors",
+            "ext": "png",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
+            "min_zoom": 0,
             "name": "Stadia.AlidadeSmooth",
-            "url": "https://tiles.stadiamaps.com/tiles/alidade_smooth/{z}/{x}/{y}{r}.png"
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "alidade_smooth"
         },
         "AlidadeSmoothDark": {
-            "attribution": "(C) Stadia Maps, (C) OpenMapTiles (C) OpenStreetMap contributors",
-            "html_attribution": "&copy; <a href=\"https://stadiamaps.com/\">Stadia Maps</a>, &copy; <a href=\"https://openmaptiles.org/\">OpenMapTiles</a> &copy; <a href=\"http://openstreetmap.org\">OpenStreetMap</a> contributors",
+            "attribution": "(C) Stadia Maps (C) OpenMapTiles (C) OpenStreetMap contributors",
+            "ext": "png",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
+            "min_zoom": 0,
             "name": "Stadia.AlidadeSmoothDark",
-            "url": "https://tiles.stadiamaps.com/tiles/alidade_smooth_dark/{z}/{x}/{y}{r}.png"
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "alidade_smooth_dark"
         },
         "OSMBright": {
-            "attribution": "(C) Stadia Maps, (C) OpenMapTiles (C) OpenStreetMap contributors",
-            "html_attribution": "&copy; <a href=\"https://stadiamaps.com/\">Stadia Maps</a>, &copy; <a href=\"https://openmaptiles.org/\">OpenMapTiles</a> &copy; <a href=\"http://openstreetmap.org\">OpenStreetMap</a> contributors",
+            "attribution": "(C) Stadia Maps (C) OpenMapTiles (C) OpenStreetMap contributors",
+            "ext": "png",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
+            "min_zoom": 0,
             "name": "Stadia.OSMBright",
-            "url": "https://tiles.stadiamaps.com/tiles/osm_bright/{z}/{x}/{y}{r}.png"
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "osm_bright"
         },
         "Outdoors": {
-            "attribution": "(C) Stadia Maps, (C) OpenMapTiles (C) OpenStreetMap contributors",
-            "html_attribution": "&copy; <a href=\"https://stadiamaps.com/\">Stadia Maps</a>, &copy; <a href=\"https://openmaptiles.org/\">OpenMapTiles</a> &copy; <a href=\"http://openstreetmap.org\">OpenStreetMap</a> contributors",
-            "max_zoom": 20,
-            "name": "Stadia.Outdoors",
-            "url": "https://tiles.stadiamaps.com/tiles/outdoors/{z}/{x}/{y}{r}.png"
-        }
-    },
-    "Stamen": {
-        "Terrain": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+            "attribution": "(C) Stadia Maps (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
-            "max_zoom": 18,
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "max_zoom": 20,
             "min_zoom": 0,
-            "name": "Stamen.Terrain",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "terrain"
+            "name": "Stadia.Outdoors",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "outdoors"
         },
-        "TerrainBackground": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenTerrain": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 18,
             "min_zoom": 0,
-            "name": "Stamen.TerrainBackground",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "terrain-background"
+            "name": "Stadia.StamenTerrain",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_terrain"
         },
-        "TerrainLabels": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenTerrainBackground": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 18,
             "min_zoom": 0,
-            "name": "Stamen.TerrainLabels",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "terrain-labels"
+            "name": "Stadia.StamenTerrainBackground",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_terrain_background"
         },
-        "Toner": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenTerrainLabels": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
-            "max_zoom": 20,
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "max_zoom": 18,
             "min_zoom": 0,
-            "name": "Stamen.Toner",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "toner"
+            "name": "Stadia.StamenTerrainLabels",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_terrain_labels"
         },
-        "TonerBackground": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenTerrainLines": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
-            "max_zoom": 20,
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "max_zoom": 18,
             "min_zoom": 0,
-            "name": "Stamen.TonerBackground",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "toner-background"
+            "name": "Stadia.StamenTerrainLines",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_terrain_lines"
         },
-        "TonerHybrid": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenToner": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
             "min_zoom": 0,
-            "name": "Stamen.TonerHybrid",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "toner-hybrid"
+            "name": "Stadia.StamenToner",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_toner"
         },
-        "TonerLabels": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenTonerBackground": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
             "min_zoom": 0,
-            "name": "Stamen.TonerLabels",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "toner-labels"
+            "name": "Stadia.StamenTonerBackground",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_toner_background"
         },
-        "TonerLines": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenTonerLabels": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
             "min_zoom": 0,
-            "name": "Stamen.TonerLines",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "toner-lines"
+            "name": "Stadia.StamenTonerLabels",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_toner_labels"
         },
-        "TonerLite": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenTonerLines": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
             "min_zoom": 0,
-            "name": "Stamen.TonerLite",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "toner-lite"
+            "name": "Stadia.StamenTonerLines",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_toner_lines"
         },
-        "TopOSMFeatures": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
-            "bounds": [
-                [
-                    22,
-                    -132
-                ],
-                [
-                    51,
-                    -56
-                ]
-            ],
+        "StamenTonerLite": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "png",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
-            "max_zoom": 20,
-            "min_zoom": 0,
-            "name": "Stamen.TopOSMFeatures",
-            "opacity": 0.9,
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}{r}.{ext}",
-            "variant": "toposm-features"
-        },
-        "TopOSMRelief": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
-            "bounds": [
-                [
-                    22,
-                    -132
-                ],
-                [
-                    51,
-                    -56
-                ]
-            ],
-            "ext": "jpg",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 20,
             "min_zoom": 0,
-            "name": "Stamen.TopOSMRelief",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}.{ext}",
-            "variant": "toposm-color-relief"
+            "name": "Stadia.StamenTonerLite",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}{r}.{ext}",
+            "variant": "stamen_toner_lite"
         },
-        "Watercolor": {
-            "attribution": "Map tiles by Stamen Design, CC BY 3.0 -- Map data (C) OpenStreetMap contributors",
+        "StamenWatercolor": {
+            "attribution": "(C) Stadia Maps (C) Stamen Design (C) OpenMapTiles (C) OpenStreetMap contributors",
             "ext": "jpg",
-            "html_attribution": "Map tiles by <a href=\"http://stamen.com\">Stamen Design</a>, <a href=\"http://creativecommons.org/licenses/by/3.0\">CC BY 3.0</a> &mdash; Map data &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
+            "html_attribution": "&copy; <a href=\"https://www.stadiamaps.com/\" target=\"_blank\">Stadia Maps</a> &copy; <a href=\"https://www.stamen.com/\" target=\"_blank\">Stamen Design</a> &copy; <a href=\"https://openmaptiles.org/\" target=\"_blank\">OpenMapTiles</a> &copy; <a href=\"https://www.openstreetmap.org/copyright\">OpenStreetMap</a> contributors",
             "max_zoom": 16,
             "min_zoom": 1,
-            "name": "Stamen.Watercolor",
-            "subdomains": "abcd",
-            "url": "https://stamen-tiles-{s}.a.ssl.fastly.net/{variant}/{z}/{x}/{y}.{ext}",
-            "variant": "watercolor"
+            "name": "Stadia.StamenWatercolor",
+            "url": "https://tiles.stadiamaps.com/tiles/{variant}/{z}/{x}/{y}.{ext}",
+            "variant": "stamen_watercolor"
         }
     },
     "SwissFederalGeoportal": {
         "NationalMapColor": {
             "attribution": "(C) swisstopo",
             "bounds": [
                 [
@@ -2749,49 +2839,67 @@
             "url": "https://{s}.tile.thunderforest.com/{variant}/{z}/{x}/{y}.png?apikey={apikey}",
             "variant": "transport-dark"
         }
     },
     "TomTom": {
         "Basic": {
             "apikey": "<insert your API key here>",
-            "attribution": "(C) 1992 - 2023 TomTom.",
+            "attribution": "(C) 1992 - 2024 TomTom.",
             "ext": "png",
-            "html_attribution": "<a href=\"https://tomtom.com\" target=\"_blank\">&copy;  1992 - 2023 TomTom.</a> ",
+            "html_attribution": "<a href=\"https://tomtom.com\" target=\"_blank\">&copy;  1992 - 2024 TomTom.</a> ",
             "max_zoom": 22,
             "name": "TomTom.Basic",
             "style": "main",
             "subdomains": "abcd",
             "url": "https://{s}.api.tomtom.com/map/1/tile/{variant}/{style}/{z}/{x}/{y}.{ext}?key={apikey}",
             "variant": "basic"
         },
         "Hybrid": {
             "apikey": "<insert your API key here>",
-            "attribution": "(C) 1992 - 2023 TomTom.",
+            "attribution": "(C) 1992 - 2024 TomTom.",
             "ext": "png",
-            "html_attribution": "<a href=\"https://tomtom.com\" target=\"_blank\">&copy;  1992 - 2023 TomTom.</a> ",
+            "html_attribution": "<a href=\"https://tomtom.com\" target=\"_blank\">&copy;  1992 - 2024 TomTom.</a> ",
             "max_zoom": 22,
             "name": "TomTom.Hybrid",
             "style": "main",
             "subdomains": "abcd",
             "url": "https://{s}.api.tomtom.com/map/1/tile/{variant}/{style}/{z}/{x}/{y}.{ext}?key={apikey}",
             "variant": "hybrid"
         },
         "Labels": {
             "apikey": "<insert your API key here>",
-            "attribution": "(C) 1992 - 2023 TomTom.",
+            "attribution": "(C) 1992 - 2024 TomTom.",
             "ext": "png",
-            "html_attribution": "<a href=\"https://tomtom.com\" target=\"_blank\">&copy;  1992 - 2023 TomTom.</a> ",
+            "html_attribution": "<a href=\"https://tomtom.com\" target=\"_blank\">&copy;  1992 - 2024 TomTom.</a> ",
             "max_zoom": 22,
             "name": "TomTom.Labels",
             "style": "main",
             "subdomains": "abcd",
             "url": "https://{s}.api.tomtom.com/map/1/tile/{variant}/{style}/{z}/{x}/{y}.{ext}?key={apikey}",
             "variant": "labels"
         }
     },
+    "TopPlusOpen": {
+        "Color": {
+            "attribution": "Map data: (C) dl-de/by-2-0",
+            "html_attribution": "Map data: &copy; <a href=\"http://www.govdata.de/dl-de/by-2-0\">dl-de/by-2-0</a>",
+            "max_zoom": 18,
+            "name": "TopPlusOpen.Color",
+            "url": "http://sgx.geodatenzentrum.de/wmts_topplus_open/tile/1.0.0/{variant}/default/WEBMERCATOR/{z}/{y}/{x}.png",
+            "variant": "web"
+        },
+        "Grey": {
+            "attribution": "Map data: (C) dl-de/by-2-0",
+            "html_attribution": "Map data: &copy; <a href=\"http://www.govdata.de/dl-de/by-2-0\">dl-de/by-2-0</a>",
+            "max_zoom": 18,
+            "name": "TopPlusOpen.Grey",
+            "url": "http://sgx.geodatenzentrum.de/wmts_topplus_open/tile/1.0.0/{variant}/default/WEBMERCATOR/{z}/{y}/{x}.png",
+            "variant": "web_grau"
+        }
+    },
     "USGS": {
         "USImagery": {
             "attribution": "Tiles courtesy of the U.S. Geological Survey",
             "html_attribution": "Tiles courtesy of the <a href=\"https://usgs.gov/\">U.S. Geological Survey</a>",
             "max_zoom": 20,
             "name": "USGS.USImagery",
             "url": "https://basemap.nationalmap.gov/arcgis/rest/services/USGSImageryOnly/MapServer/tile/{z}/{y}/{x}"
@@ -2858,16 +2966,16 @@
             "max_zoom": 18,
             "name": "WaymarkedTrails.slopes",
             "url": "https://tile.waymarkedtrails.org/{variant}/{z}/{x}/{y}.png",
             "variant": "slopes"
         }
     },
     "_meta": {
-        "commit": "commit 15b5c38a104a6e71f69b4ab48ea5b0b13835d5d2 (openstreetmap.de)",
-        "date_of_creation": "2023-07-13",
+        "commit": "commit d279aa29f9bd10ed303c07b5fbf84699720af2a4 (Bump eslint from 8.56.0 to 8.57.0\n\nBumps [eslint](https://github.com/eslint/eslint) from 8.56.0 to 8.57.0.\n- [Release notes](https://github.com/eslint/eslint/releases)\n- [Changelog](https://github.com/eslint/eslint/blob/main/CHANGELOG.md)\n- [Commits](https://github.com/eslint/eslint/compare/v8.56.0...v8.57.0)\n\n---\nupdated-dependencies:\n- dependency-name: eslint\n  dependency-type: direct:development\n  update-type: version-update:semver-minor\n...\n\nSigned-off-by: dependabot[bot] <support@github.com>)",
+        "date_of_creation": "2024-03-15",
         "description": "JSON representation of the leaflet providers defined by the leaflet-providers.js extension to Leaflet (https://github.com/leaflet-extras/leaflet-providers)"
     },
     "nlmaps": {
         "grijs": {
             "attribution": "Kaartgegevens (C) Kadaster",
             "bounds": [
                 [
```

### Comparing `xyzservices-2023.7.0/provider_sources/xyzservices-providers.json` & `xyzservices-2024.4.0/provider_sources/xyzservices-providers.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9915364583333333%*

 * *Differences: {"'NASAGIBS'": "{'BlueMarble3413': {'url': "*

 * *               "'https://gibs.earthdata.nasa.gov/wmts/epsg3413/best/BlueMarble_NextGeneration/default/500m/{z}/{y}/{x}.jpeg'}, "*

 * *               "'BlueMarble3031': {'url': "*

 * *               "'https://gibs.earthdata.nasa.gov/wmts/epsg3031/best/BlueMarble_NextGeneration/default/500m/{z}/{y}/{x}.jpeg'}, "*

 * *               "delete: ['BlueMarble']}"}*

```diff
@@ -193,36 +193,29 @@
         "ASTER_GDEM_Greyscale_Shaded_Relief": {
             "attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (ESDIS) with funding provided by NASA/HQ.",
             "html_attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (<a href=\"https://earthdata.nasa.gov\">ESDIS</a>) with funding provided by NASA/HQ.",
             "max_zoom": 12,
             "name": "NASAGIBS.ASTER_GDEM_Greyscale_Shaded_Relief",
             "url": "https://gibs.earthdata.nasa.gov/wmts/epsg3857/best/ASTER_GDEM_Greyscale_Shaded_Relief/default/GoogleMapsCompatible_Level12/{z}/{y}/{x}.jpg"
         },
-        "BlueMarble": {
-            "attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (ESDIS) with funding provided by NASA/HQ.",
-            "html_attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (<a href=\"https://earthdata.nasa.gov\">ESDIS</a>) with funding provided by NASA/HQ.",
-            "max_zoom": 8,
-            "name": "NASAGIBS.BlueMarble",
-            "url": "https://gibs.earthdata.nasa.gov/wmts/epsg3857/best/BlueMarble_NextGeneration/default/EPSG3857_500m/{z}/{y}/{x}.jpeg"
-        },
         "BlueMarble3031": {
             "attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (ESDIS) with funding provided by NASA/HQ.",
             "crs": "EPSG:3031",
             "html_attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (<a href=\"https://earthdata.nasa.gov\">ESDIS</a>) with funding provided by NASA/HQ.",
             "max_zoom": 5,
             "name": "NASAGIBS.BlueMarble3031",
-            "url": "https://gibs.earthdata.nasa.gov/wmts/epsg3031/best/BlueMarble_NextGeneration/default/EPSG3031_500m/{z}/{y}/{x}.jpeg"
+            "url": "https://gibs.earthdata.nasa.gov/wmts/epsg3031/best/BlueMarble_NextGeneration/default/500m/{z}/{y}/{x}.jpeg"
         },
         "BlueMarble3413": {
             "attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (ESDIS) with funding provided by NASA/HQ.",
             "crs": "EPSG:3413",
             "html_attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (<a href=\"https://earthdata.nasa.gov\">ESDIS</a>) with funding provided by NASA/HQ.",
             "max_zoom": 5,
             "name": "NASAGIBS.BlueMarble3413",
-            "url": "https://gibs.earthdata.nasa.gov/wmts/epsg3413/best/BlueMarble_NextGeneration/default/EPSG3413_500m/{z}/{y}/{x}.jpeg"
+            "url": "https://gibs.earthdata.nasa.gov/wmts/epsg3413/best/BlueMarble_NextGeneration/default/500m/{z}/{y}/{x}.jpeg"
         },
         "ModisAquaBands721CR": {
             "attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (ESDIS) with funding provided by NASA/HQ.",
             "html_attribution": "Imagery provided by services from the Global Imagery Browse Services (GIBS), operated by the NASA/GSFC/Earth Science Data and Information System (<a href=\"https://earthdata.nasa.gov\">ESDIS</a>) with funding provided by NASA/HQ.",
             "max_zoom": 9,
             "name": "NASAGIBS.ModisAquaBands721CR",
             "time": "",
```

### Comparing `xyzservices-2023.7.0/setup.py` & `xyzservices-2024.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/xyzservices/lib.py` & `xyzservices-2024.4.0/xyzservices/lib.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/xyzservices/tests/test_lib.py` & `xyzservices-2024.4.0/xyzservices/tests/test_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,20 +178,21 @@
     basic2 = basic_provider.copy()
     assert isinstance(basic2, TileProvider)
 
 
 def test_callable():
     # only testing the callable functionality to override a keyword, as we
     # cannot test the actual providers that need an API key
-    updated_provider = xyz.GeoportailFrance.plan(apikey="mykey")
+    original_key = str(xyz.OpenWeatherMap.CloudsClassic["apiKey"])
+    updated_provider = xyz.OpenWeatherMap.CloudsClassic(apiKey="mykey")
     assert isinstance(updated_provider, TileProvider)
     assert "url" in updated_provider
-    assert updated_provider["apikey"] == "mykey"
+    assert updated_provider["apiKey"] == "mykey"
     # check that original provider dict is not modified
-    assert xyz.GeoportailFrance.plan["apikey"] == "essentiels"
+    assert xyz.OpenWeatherMap.CloudsClassic["apiKey"] == original_key
 
 
 def test_html_attribution_fallback(basic_provider, html_attr_provider):
     # TileProvider.html_attribution falls back to .attribution if the former not present
     assert basic_provider.html_attribution == basic_provider.attribution
     assert (
         html_attr_provider.html_attribution
```

### Comparing `xyzservices-2023.7.0/xyzservices/tests/test_providers.py` & `xyzservices-2024.4.0/xyzservices/tests/test_providers.py`

 * *Files identical despite different names*

### Comparing `xyzservices-2023.7.0/xyzservices.egg-info/PKG-INFO` & `xyzservices-2024.4.0/xyzservices.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyzservices
-Version: 2023.7.0
+Version: 2024.4.0
 Summary: Source of XYZ tiles providers
 Home-page: https://github.com/geopandas/xyzservices
 Author: Dani Arribas-Bel, Martin Fleischmann
 Author-email: daniel.arribas.bel@gmail.com, martin@martinfleischmann.net
 License: 3-Clause BSD
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xyzservices-2023.7.0/xyzservices.egg-info/SOURCES.txt` & `xyzservices-2024.4.0/xyzservices.egg-info/SOURCES.txt`

 * *Files identical despite different names*

