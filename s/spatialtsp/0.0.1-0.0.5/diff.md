# Comparing `tmp/spatialtsp-0.0.1.tar.gz` & `tmp/spatialtsp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialtsp-0.0.1.tar", last modified: Thu Feb 22 03:32:04 2024, max compression
+gzip compressed data, was "spatialtsp-0.0.5.tar", last modified: Wed Apr  3 06:27:19 2024, max compression
```

## Comparing `spatialtsp-0.0.1.tar` & `spatialtsp-0.0.5.tar`

### file list

```diff
@@ -1,52 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.629288 spatialtsp-0.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.633288 spatialtsp-0.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.633288 spatialtsp-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1984 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/workflows/docs-build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/workflows/installation.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/workflows/macos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/workflows/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.github/workflows/windows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/common.md
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/contributing.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/examples/intro.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/installation.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/spatialtsp.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/spatialtsp/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/spatialtsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/spatialtsp/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/spatialtsp/spatialtsp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/spatialtsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-02-22 03:32:04.000000 spatialtsp-0.0.1/spatialtsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-02-22 03:32:04.000000 spatialtsp-0.0.1/spatialtsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-22 03:32:04.000000 spatialtsp-0.0.1/spatialtsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-22 03:32:04.000000 spatialtsp-0.0.1/spatialtsp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-22 03:32:04.000000 spatialtsp-0.0.1/spatialtsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-22 03:32:04.000000 spatialtsp-0.0.1/spatialtsp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-22 03:32:04.637288 spatialtsp-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-02-22 03:31:50.000000 spatialtsp-0.0.1/tests/test_spatialtsp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.127397 spatialtsp-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.103397 spatialtsp-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.107397 spatialtsp-0.0.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.107397 spatialtsp-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/workflows/docs-build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/workflows/installation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/workflows/macos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/workflows/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.github/workflows/windows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-03 06:27:19.127397 spatialtsp-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.107397 spatialtsp-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.107397 spatialtsp-0.0.5/docs/class510/
+-rw-r--r--   0 runner    (1001) docker     (127)    26407 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/class510/lab4.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    42402 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/class510/lab5.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/class510/responses.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/common.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/contributing.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.123397 spatialtsp-0.0.5/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/Vector.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  8054961 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/continents.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    91209 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)   241236 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)   241236 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.json
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.prj
+-rw-r--r--   0 runner    (1001) docker     (127)   171476 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.shp
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.shx
+-rw-r--r--   0 runner    (1001) docker     (127)   232511 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/countries.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/csv.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   117900 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/europe_110.geo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/intro.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/ipyleaflet.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    13584 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/spatialtsp.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.123397 spatialtsp-0.0.5/docs/examples/temp_shp/
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/temp_shp/us_states.cpg
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/temp_shp/us_states.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     8148 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/temp_shp/us_states.dbf
+-rw-r--r--   0 runner    (1001) docker     (127)   103466 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/temp_shp/us_states.geojson
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/temp_shp/us_states.prj
+-rw-r--r--   0 runner    (1001) docker     (127)    59376 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/temp_shp/us_states.shp
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/examples/temp_shp/us_states.shx
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/installation.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.123397 spatialtsp-0.0.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/spatialtsp.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/docs/utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 06:27:19.127397 spatialtsp-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.123397 spatialtsp-0.0.5/spatialtsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/spatialtsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/spatialtsp/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/spatialtsp/spatialtsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/spatialtsp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.127397 spatialtsp-0.0.5/spatialtsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-03 06:27:19.000000 spatialtsp-0.0.5/spatialtsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-03 06:27:19.000000 spatialtsp-0.0.5/spatialtsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 06:27:19.000000 spatialtsp-0.0.5/spatialtsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 06:27:19.000000 spatialtsp-0.0.5/spatialtsp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 06:27:19.000000 spatialtsp-0.0.5/spatialtsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 06:27:19.000000 spatialtsp-0.0.5/spatialtsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    13856 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/spatialtsp.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 06:27:19.123397 spatialtsp-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 06:27:03.000000 spatialtsp-0.0.5/tests/test_spatialtsp.py
```

### Comparing `spatialtsp-0.0.1/.github/workflows/docs-build.yml` & `spatialtsp-0.0.5/.github/workflows/docs-build.yml`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                   gdalinfo --version
             - name: Install dependencies
               run: |
                   pip install --no-cache-dir Cython
                   pip install -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
-              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git" --ignore-words-list="aci,acount,hist"
+              run: codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,*.pdf,./.git,*.txt" --ignore-words-list="aci,acount,hist"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - name: Build docs
               run: |
                   mkdocs build
             # - name: Deploy to Netlify
```

### Comparing `spatialtsp-0.0.1/.github/workflows/docs.yml` & `spatialtsp-0.0.5/.github/workflows/docs.yml`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,18 @@
             - uses: actions/setup-python@v5
               with:
                   python-version: "3.11"
 
             - name: Install dependencies
               run: |
                   python -m pip install --upgrade pip
-                  pip install --user --no-cache-dir Cython
-                  pip install --user -r requirements.txt -r requirements_dev.txt
+                  pip install --no-cache-dir Cython
+                  pip install -r requirements.txt -r requirements_dev.txt
                   pip install .
             - name: Discover typos with codespell
               run: |
-                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git" --ignore-words-list="aci,hist"
+                  codespell --skip="*.csv,*.geojson,*.json,*.js,*.html,*cff,./.git,*.txt,*.data_types.ipynb" --ignore-words-list="aci,hist,vor"
             - name: PKG-TEST
               run: |
                   python -m unittest discover tests/
             - run: mkdocs gh-deploy --force
```

### Comparing `spatialtsp-0.0.1/.github/workflows/installation.yml` & `spatialtsp-0.0.5/.github/workflows/installation.yml`

 * *Files identical despite different names*

### Comparing `spatialtsp-0.0.1/.github/workflows/macos.yml` & `spatialtsp-0.0.5/.github/workflows/macos.yml`

 * *Files identical despite different names*

### Comparing `spatialtsp-0.0.1/.github/workflows/pypi.yml` & `spatialtsp-0.0.5/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `spatialtsp-0.0.1/.github/workflows/ubuntu.yml` & `spatialtsp-0.0.5/.github/workflows/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `spatialtsp-0.0.1/.github/workflows/windows.yml` & `spatialtsp-0.0.5/.github/workflows/windows.yml`

 * *Files identical despite different names*

### Comparing `spatialtsp-0.0.1/.gitignore` & `spatialtsp-0.0.5/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Byte-compiled / optimized / DLL files
 __pycache__/
 private/
 *.py[cod]
 *$py.class
+*.json
 
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 env/
```

### Comparing `spatialtsp-0.0.1/PKG-INFO` & `spatialtsp-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialtsp
-Version: 0.0.1
+Version: 0.0.5
 Summary: A python package demo for spatially informed TSP
 Author-email: Wanhee Kim <wkim15@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/whkim15/spatialtsp
 Keywords: spatialtsp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ipyleaflet
 Requires-Dist: numpy
+Requires-Dist: pyshp
+Requires-Dist: pandas
+Requires-Dist: scipy>=1.7.1
+Requires-Dist: scikit-learn
+Requires-Dist: geopandas
+Requires-Dist: shapely
+Requires-Dist: requests
 Provides-Extra: all
 Requires-Dist: spatialtsp[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # spatialtsp
```

### Comparing `spatialtsp-0.0.1/docs/contributing.md` & `spatialtsp-0.0.5/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `spatialtsp-0.0.1/docs/installation.md` & `spatialtsp-0.0.5/docs/installation.md`

 * *Files identical despite different names*

### Comparing `spatialtsp-0.0.1/mkdocs.yml` & `spatialtsp-0.0.5/mkdocs.yml`

 * *Files 10% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     - git-revision-date-localized:
           enable_creation_date: true
           type: timeago
     # - pdf-export
     - mkdocs-jupyter:
           include_source: True
           ignore_h1_titles: True
-          execute: True
+          execute: false
           allow_errors: false
           ignore: ["conf.py"]
           execute_ignore: ["*ignore.ipynb"]
           
 markdown_extensions:
     - admonition
     - abbr
@@ -77,10 +77,18 @@
     - Usage: usage.md
     - Contributing: contributing.md
     - FAQ: faq.md
     - Changelog: changelog.md
     - Report Issues: https://github.com/whkim15/spatialtsp/issues
     - Examples:
         - examples/intro.ipynb
+        - examples/spatialtsp.ipynb
+        - examples/ipyleaflet.ipynb
+        - examples/Vector.ipynb
+        - examples/csv.ipynb
     - API Reference:
           - spatialtsp module: spatialtsp.md
           - common module: common.md
+          - utils module: utils.md 
+    - Class510 Test:
+        - class510/lab4.ipynb
+        - class510/lab5.ipynb
```

### Comparing `spatialtsp-0.0.1/pyproject.toml` & `spatialtsp-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spatialtsp"
-version = "0.0.1"
+version = "0.0.5"
 dynamic = [
     "dependencies",
 ]
 description = "A python package demo for spatially informed TSP"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = [
@@ -48,15 +48,15 @@
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
 [tool.bumpversion]
-current_version = "0.0.1"
+current_version = "0.0.5"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `spatialtsp-0.0.1/spatialtsp.egg-info/PKG-INFO` & `spatialtsp-0.0.5/spatialtsp.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialtsp
-Version: 0.0.1
+Version: 0.0.5
 Summary: A python package demo for spatially informed TSP
 Author-email: Wanhee Kim <wkim15@vols.utk.edu>
 License: MIT License
 Project-URL: Homepage, https://github.com/whkim15/spatialtsp
 Keywords: spatialtsp
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: ipyleaflet
 Requires-Dist: numpy
+Requires-Dist: pyshp
+Requires-Dist: pandas
+Requires-Dist: scipy>=1.7.1
+Requires-Dist: scikit-learn
+Requires-Dist: geopandas
+Requires-Dist: shapely
+Requires-Dist: requests
 Provides-Extra: all
 Requires-Dist: spatialtsp[extra]; extra == "all"
 Provides-Extra: extra
 Requires-Dist: pandas; extra == "extra"
 
 # spatialtsp
```

