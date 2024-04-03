# Comparing `tmp/wwvb-3.0.7.tar.gz` & `tmp/wwvb-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwvb-3.0.7.tar", last modified: Tue Mar 19 00:32:28 2024, max compression
+gzip compressed data, was "wwvb-3.0.8.tar", last modified: Wed Apr  3 13:03:52 2024, max compression
```

## Comparing `wwvb-3.0.7.tar` & `wwvb-3.0.8.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.375981 wwvb-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-19 00:32:07.000000 wwvb-3.0.7/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.363981 wwvb-3.0.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.363981 wwvb-3.0.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-03-19 00:32:07.000000 wwvb-3.0.7/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-19 00:32:07.000000 wwvb-3.0.7/.github/workflows/cron.yml
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-19 00:32:07.000000 wwvb-3.0.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-19 00:32:07.000000 wwvb-3.0.7/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-19 00:32:07.000000 wwvb-3.0.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-19 00:32:07.000000 wwvb-3.0.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-03-19 00:32:07.000000 wwvb-3.0.7/.pylintrc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.367981 wwvb-3.0.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-03-19 00:32:07.000000 wwvb-3.0.7/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-03-19 00:32:07.000000 wwvb-3.0.7/LICENSES/CC0-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    34670 2024-03-19 00:32:07.000000 wwvb-3.0.7/LICENSES/GPL-3.0-only.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-19 00:32:07.000000 wwvb-3.0.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-19 00:32:07.000000 wwvb-3.0.7/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-03-19 00:32:28.375981 wwvb-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-03-19 00:32:07.000000 wwvb-3.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.367981 wwvb-3.0.7/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:07.000000 wwvb-3.0.7/_static/.empty
--rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-03-19 00:32:07.000000 wwvb-3.0.7/adafruit_datetime.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:07.000000 wwvb-3.0.7/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-19 00:32:07.000000 wwvb-3.0.7/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-19 00:32:07.000000 wwvb-3.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-19 00:32:07.000000 wwvb-3.0.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-19 00:32:28.375981 wwvb-3.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.367981 wwvb-3.0.7/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5720 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/uwwvb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.367981 wwvb-3.0.7/src/wwvb/
--rw-r--r--   0 runner    (1001) docker     (127)    30100 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-19 00:32:28.000000 wwvb-3.0.7/src/wwvb/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/decode.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      890 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/dut1table.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3792 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/iersdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/iersdata_dist.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10118 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/testcli.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2485 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/testdaylight.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1720 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/testls.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      935 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/testpm.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/testuwwvb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    16143 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/testwwvb.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/tz.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     7362 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/updateiers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4598 2024-03-19 00:32:07.000000 wwvb-3.0.7/src/wwvb/wwvbtk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.371981 wwvb-3.0.7/src/wwvb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-03-19 00:32:28.000000 wwvb-3.0.7/src/wwvb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-03-19 00:32:28.000000 wwvb-3.0.7/src/wwvb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 00:32:28.000000 wwvb-3.0.7/src/wwvb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-19 00:32:28.000000 wwvb-3.0.7/src/wwvb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-03-19 00:32:28.000000 wwvb-3.0.7/src/wwvb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-19 00:32:28.000000 wwvb-3.0.7/src/wwvb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 00:32:28.371981 wwvb-3.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/1998leapsecond
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/2012leapsecond
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/all-headers
--rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/bar
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/both
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/cradek
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/duration
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/enddst-phase
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/enddst-phase-2
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/endleapyear
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/leapday1
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/leapday28
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/leapday29
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/negleapsecond
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/nextdst
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/nextst
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/nonleapday1
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/nonleapday28
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/phase
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/startdst
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/startdst-phase
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/startdst-phase-2
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/startleapyear
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/startst
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/y2k
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/y2k-1
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/y2k1
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-19 00:32:07.000000 wwvb-3.0.7/tests/y2k1-1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.596498 wwvb-3.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 13:03:32.000000 wwvb-3.0.8/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.588498 wwvb-3.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.588498 wwvb-3.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-03 13:03:32.000000 wwvb-3.0.8/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-03 13:03:32.000000 wwvb-3.0.8/.github/workflows/cron.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-03 13:03:32.000000 wwvb-3.0.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-03 13:03:32.000000 wwvb-3.0.8/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-03 13:03:32.000000 wwvb-3.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 13:03:32.000000 wwvb-3.0.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-03 13:03:32.000000 wwvb-3.0.8/.pylintrc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.588498 wwvb-3.0.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-03 13:03:32.000000 wwvb-3.0.8/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-03 13:03:32.000000 wwvb-3.0.8/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    34670 2024-04-03 13:03:32.000000 wwvb-3.0.8/LICENSES/GPL-3.0-only.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-03 13:03:32.000000 wwvb-3.0.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-03 13:03:32.000000 wwvb-3.0.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-03 13:03:52.596498 wwvb-3.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9354 2024-04-03 13:03:32.000000 wwvb-3.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.588498 wwvb-3.0.8/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:32.000000 wwvb-3.0.8/_static/.empty
+-rw-r--r--   0 runner    (1001) docker     (127)    12922 2024-04-03 13:03:32.000000 wwvb-3.0.8/adafruit_datetime.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:32.000000 wwvb-3.0.8/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-03 13:03:32.000000 wwvb-3.0.8/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 13:03:32.000000 wwvb-3.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 13:03:32.000000 wwvb-3.0.8/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 13:03:52.596498 wwvb-3.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.592498 wwvb-3.0.8/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/uwwvb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.592498 wwvb-3.0.8/src/wwvb/
+-rw-r--r--   0 runner    (1001) docker     (127)    29762 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 13:03:52.000000 wwvb-3.0.8/src/wwvb/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/decode.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      890 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/dut1table.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3697 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/iersdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/iersdata_dist.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    10086 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/testcli.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2485 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/testdaylight.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1720 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/testls.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      935 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/testpm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/testuwwvb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16109 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/testwwvb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/tz.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7240 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/updateiers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4525 2024-04-03 13:03:32.000000 wwvb-3.0.8/src/wwvb/wwvbtk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.596498 wwvb-3.0.8/src/wwvb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10290 2024-04-03 13:03:52.000000 wwvb-3.0.8/src/wwvb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 13:03:52.000000 wwvb-3.0.8/src/wwvb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:03:52.000000 wwvb-3.0.8/src/wwvb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-03 13:03:52.000000 wwvb-3.0.8/src/wwvb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 13:03:52.000000 wwvb-3.0.8/src/wwvb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 13:03:52.000000 wwvb-3.0.8/src/wwvb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:03:52.596498 wwvb-3.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/1998leapsecond
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/2012leapsecond
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/all-headers
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/bar
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/both
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/cradek
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/duration
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/enddst-phase
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/enddst-phase-2
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/endleapyear
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/leapday1
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/leapday28
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/leapday29
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/negleapsecond
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/nextdst
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/nextst
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/nonleapday1
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/nonleapday28
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/phase
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/startdst
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/startdst-phase
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/startdst-phase-2
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/startleapyear
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/startst
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/y2k
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/y2k-1
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/y2k1
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-03 13:03:32.000000 wwvb-3.0.8/tests/y2k1-1
```

### Comparing `wwvb-3.0.7/.github/workflows/codeql.yml` & `wwvb-3.0.8/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/.github/workflows/cron.yml` & `wwvb-3.0.8/.github/workflows/cron.yml`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/.github/workflows/release.yml` & `wwvb-3.0.8/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/.github/workflows/test.yml` & `wwvb-3.0.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/.pre-commit-config.yaml` & `wwvb-3.0.8/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,14 @@
       exclude: tests
 - repo: https://github.com/fsfe/reuse-tool
   rev: v3.0.1
   hooks:
   - id: reuse
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: v0.3.3
+  rev: v0.3.5
   hooks:
     # Run the linter.
     - id: ruff
       args: [ --fix ]
     # Run the formatter.
     - id: ruff-format
```

### Comparing `wwvb-3.0.7/.pylintrc` & `wwvb-3.0.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/LICENSES/Apache-2.0.txt` & `wwvb-3.0.8/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/LICENSES/CC0-1.0.txt` & `wwvb-3.0.8/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/LICENSES/GPL-3.0-only.txt` & `wwvb-3.0.8/LICENSES/GPL-3.0-only.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/LICENSES/Unlicense.txt` & `wwvb-3.0.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/Makefile` & `wwvb-3.0.8/Makefile`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/PKG-INFO` & `wwvb-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwvb
-Version: 3.0.7
+Version: 3.0.8
 Summary: Generate WWVB timecodes for any desired time
 Home-page: https://github.com/jepler/wwvbpy
 Author: Jeff Epler
 Author-email: jepler@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `wwvb-3.0.7/README.md` & `wwvb-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/adafruit_datetime.pyi` & `wwvb-3.0.8/adafruit_datetime.pyi`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/conf.py` & `wwvb-3.0.8/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# pylint: disable=all
 # fmt: off
 # Configuration file for the Sphinx documentation builder.
 #
 # This file only contains a selection of the most common options. For a full
 # list see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
```

### Comparing `wwvb-3.0.7/setup.cfg` & `wwvb-3.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/src/uwwvb.py` & `wwvb-3.0.8/src/uwwvb.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         if digit > 9:
             return None
         result += digit * base
         base *= 10
     return result
 
 
-def decode_wwvb(  # pylint: disable=too-many-return-statements
+def decode_wwvb(
     t: list[int] | None,
 ) -> WWVBMinute | None:
     """Convert a received minute of wwvb symbols to a WWVBMinute.  Returns None if any error is detected."""
     if not t:
         return None
     if not all(t[i] == MARK for i in always_mark):
         return None
```

### Comparing `wwvb-3.0.7/src/wwvb/__init__.py` & `wwvb-3.0.8/src/wwvb/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 from . import iersdata
 from .tz import Mountain
 
 HOUR = datetime.timedelta(seconds=3600)
 SECOND = datetime.timedelta(seconds=1)
 DateOrDatetime = TypeVar("DateOrDatetime", datetime.date, datetime.datetime)
-T = TypeVar("T")  # pylint: disable=invalid-name
+T = TypeVar("T")
 
 
 def require(x: Optional[T]) -> T:
     """Assert that an Optional value is not None, and then return the value,
     giving a hint to the type system."""
     assert x is not None
     return x
@@ -332,15 +332,15 @@
     dst: int
     ut1: int
     ly: bool
     ls: bool
 
     epoch: int = 1970
 
-    def __new__(  # pylint: disable=too-many-arguments
+    def __new__(
         cls,
         year: int,
         days: int,
         hour: int,
         minute: int,
         dst: Optional[int] = None,
         ut1: Optional[int] = None,
@@ -530,17 +530,15 @@
         full_seq = info_seq + ftw + info_seq[::-1]
         assert len(full_seq) == 360
 
         offset = minno * 60
         for i in range(60):
             t._put_pm_bit(i, full_seq[i + offset])
 
-    def fill_pm_timecode_regular(  # pylint: disable=too-many-statements
-        self, t: "WWVBTimecode"
-    ) -> None:
+    def fill_pm_timecode_regular(self, t: "WWVBTimecode") -> None:
         """Except during minutes 10..15 and 40..45, the amplitude signal holds 'regular information'"""
         t._put_pm_bin(0, 13, SYNC_T)
 
         moc = self.minute_of_century
         leap_sec = self.leap_sec
         dst_on = self.dst
         dst_ls = dst_ls_lut[dst_on | (leap_sec << 2)]
@@ -606,17 +604,15 @@
 
     def previous_minute(self, newut1: Optional[int] = None, newls: Optional[bool] = None) -> "WWVBMinute":
         """Return an object representing the previous minute"""
         d = self.as_datetime() - datetime.timedelta(minutes=1)
         return self.from_datetime(d, newut1, newls, self)
 
     @classmethod
-    def _get_dut1_info(  # pylint: disable=unused-argument
-        cls: type, year: int, days: int, old_time: "Optional[WWVBMinute]" = None
-    ) -> Tuple[int, bool]:
+    def _get_dut1_info(cls: type, year: int, days: int, old_time: "Optional[WWVBMinute]" = None) -> Tuple[int, bool]:
         """Return the DUT1 information for a given day, possibly propagating information from a previous timestamp"""
         if old_time is not None:
             if old_time.minute_length() != 60:
                 newls = False
                 if old_time.ut1 < 0:
                     newut1 = old_time.ut1 + 1000
                 else:
@@ -660,17 +656,15 @@
         """Construct a WWVBMinute from a datetime, possibly specifying ut1/ls data or propagating it from an old time"""
         u = d.utctimetuple()
         if newls is None and newut1 is None:
             newut1, newls = cls._get_dut1_info(u.tm_year, u.tm_yday, old_time)
         return cls(u.tm_year, u.tm_yday, u.tm_hour, u.tm_min, ut1=newut1, ls=newls)
 
     @classmethod
-    def from_timecode_am(  # pylint: disable=too-many-return-statements
-        cls, t: "WWVBTimecode"
-    ) -> Optional["WWVBMinute"]:
+    def from_timecode_am(cls, t: "WWVBTimecode") -> Optional["WWVBMinute"]:
         """Construct a WWVBMinute from a WWVBTimecode"""
         for i in (0, 9, 19, 29, 39, 49, 59):
             if t.am[i] != AmplitudeModulation.MARK:
                 return None
         for i in (4, 10, 11, 14, 20, 21, 24, 34, 35, 44, 54):
             if t.am[i] != AmplitudeModulation.ZERO:
                 return None
@@ -744,15 +738,15 @@
 class WWVBTimecode:
     """Represent the amplitude and/or phase signal, usually over 1 minute"""
 
     am: List[AmplitudeModulation]
     phase: List[PhaseModulation]
 
     def __init__(self, sz: int) -> None:
-        self.am = [AmplitudeModulation.UNSET] * sz  # pylint: disable=invalid-name
+        self.am = [AmplitudeModulation.UNSET] * sz
         self.phase = [PhaseModulation.UNSET] * sz
 
     def _get_am_bcd(self, *poslist: int) -> Optional[int]:
         """Convert AM data to BCD
 
         The the bits ``self.am[poslist[i]]`` in MSB order are converted from
         BCD to integer"""
@@ -831,15 +825,14 @@
     "duration": ["2", "5", "8"],
     "cradek": ["0", "1", "-"],
     "bar": ["🬍🬎", "🬋🬎", "🬋🬍"],
     "sextant": ["🬍🬎", "🬋🬎", "🬋🬍", "🬩🬹", "🬋🬹", "🬋🬩"],
 }
 
 
-# pylint: disable=too-many-arguments
 def print_timecodes(
     w: WWVBMinute,
     minutes: int,
     channel: str,
     style: str,
     file: TextIO,
     *,
@@ -869,15 +862,14 @@
             if channel in ("phase", "both"):
                 print(f"{pfx} {tc.to_pm_string(style_chars)}", file=file)
             if channel == "both":
                 print(file=file)
         w = w.next_minute()
 
 
-# pylint: disable=too-many-arguments
 def print_timecodes_json(
     w: WWVBMinute,
     minutes: int,
     channel: str,
     file: TextIO,
 ) -> None:
     """Print a range of timecodes with a header.  This header is in a format understood by WWVBMinute.fromstring"""
```

### Comparing `wwvb-3.0.7/src/wwvb/decode.py` & `wwvb-3.0.8/src/wwvb/decode.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #  Other: State 4
 # State 4: Decoding a minute, starting in second 1
 #  Second
 
 always_zero = set((4, 10, 11, 14, 20, 21, 34, 35, 44, 54))
 
 
-def wwvbreceive() -> Generator[Optional[wwvb.WWVBTimecode], wwvb.AmplitudeModulation, None]:  # pylint: disable=too-many-branches
+def wwvbreceive() -> Generator[Optional[wwvb.WWVBTimecode], wwvb.AmplitudeModulation, None]:
     """A stateful decoder of WWVB signals"""
     minute: List[wwvb.AmplitudeModulation] = []
     state = 1
 
     value = yield None
     while True:
         # print(state, value, len(minute), "".join(str(int(i)) for i in minute))
```

### Comparing `wwvb-3.0.7/src/wwvb/dut1table.py` & `wwvb-3.0.8/src/wwvb/dut1table.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/src/wwvb/gen.py` & `wwvb-3.0.8/src/wwvb/gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,15 @@
 
 import click
 import dateutil.parser
 
 from . import WWVBMinute, WWVBMinuteIERS, print_timecodes, print_timecodes_json, styles
 
 
-def parse_timespec(  # pylint: disable=unused-argument
-    ctx: Any, param: Any, value: List[str]
-) -> datetime.datetime:
+def parse_timespec(ctx: Any, param: Any, value: List[str]) -> datetime.datetime:
     """Parse a time specifier from the commandline"""
     try:
         if len(value) == 5:
             year, month, day, hour, minute = map(int, value)
             return datetime.datetime(year, month, day, hour, minute)
         if len(value) == 4:
             year, yday, hour, minute = map(int, value)
@@ -83,15 +81,14 @@
 @click.option(
     "--channel",
     type=click.Choice(["amplitude", "phase", "both"]),
     default="amplitude",
     help="Modulation to show (default: amplitude)",
 )
 @click.argument("timespec", type=str, nargs=-1, callback=parse_timespec)
-# pylint: disable=too-many-arguments, too-many-locals
 def main(
     iers: bool,
     leap_second: bool,
     dut1: int,
     minutes: int,
     style: str,
     channel: str,
```

### Comparing `wwvb-3.0.7/src/wwvb/iersdata.py` & `wwvb-3.0.8/src/wwvb/iersdata.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,13 +17,13 @@
 for location in [
     platformdirs.user_data_dir("wwvbpy", "unpythonic.net"),
     platformdirs.site_data_dir("wwvbpy", "unpythonic.net"),
 ]:  # pragma no cover
     filename = os.path.join(location, "wwvbpy_iersdata.py")
     if os.path.exists(filename):
         with open(filename, encoding="utf-8") as f:
-            exec(f.read(), globals(), globals())  # pylint: disable=exec-used
+            exec(f.read(), globals(), globals())
         break
 
 start = datetime.datetime.combine(DUT1_DATA_START, datetime.time()).replace(tzinfo=datetime.timezone.utc)
 span = datetime.timedelta(days=len(DUT1_OFFSETS))
 end = start + span
```

### Comparing `wwvb-3.0.7/src/wwvb/iersdata_dist.py` & `wwvb-3.0.8/src/wwvb/iersdata_dist.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- python3 -*-
+# fmt: off
 """File generated from public data - not subject to copyright"""
-
 # SPDX-FileCopyrightText: Public domain
 # SPDX-License-Identifier: CC0-1.0
-# fmt: off
 # isort: skip_file
-# pylint: disable=invalid-name
 import datetime
 __all__ = ['DUT1_DATA_START', 'DUT1_OFFSETS']
 DUT1_DATA_START = datetime.date(1972, 1, 1)
 d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s = tuple('defghijklmnopqrs')
 DUT1_OFFSETS = str( # 19720101
     i*182+s*123+k*30+i*31+s*19+r*31+q*29+p*28+o*30+n*36+m*40     # 19730909
     +l*39+k*33+j*31+i*31+h*18+r*19+q*38+p*32+o*31+n*33+m*48+l*45 # 19741010
@@ -32,9 +30,9 @@
     +g*49+f*18+p*59+o*53+n*52+m*57+l*48+k*53+j*127+i*70+h*30     # 19990303
     +r*62+q*79+p*152+o*82+n*106+m*184+l*125+k*217+j*133+i*252    # 20030402
     +h*161+g*392+f*322+e*290+n*116+m*154+l*85+k*83+j*91+i*168    # 20080312
     +h*105+g*147+f*105+e*42+o*70+n*91+m*154+l*119+k*84+j*217     # 20110511
     +i*126+h*176+g*97+f*91+e*52+o*116+n*98+m*70+l*133+k*91+j*91  # 20140507
     +i*77+h*140+g*91+f*84+e*70+d*34+n*72+m*76+l*66+k*53+j*56     # 20160831
     +i*105+h*77+g*45+q*25+p*63+o*91+n*154+m*105+l*190+k*118      # 20190501
-    +j*105+i*807+j*376+k*771+l*42+k*142                          # 20250308
+    +j*105+i*807+j*376+k*775+l*67+k*2+l*6+k*133                  # 20250405
 )
```

### Comparing `wwvb-3.0.7/src/wwvb/testcli.py` & `wwvb-3.0.8/src/wwvb/testcli.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 """Test most wwvblib commandline programs"""
 
 # Copyright (C) 2011-2020 Jeff Epler <jepler@gmail.com>
 # SPDX-FileCopyrightText: 2021 Jeff Epler
 #
 # SPDX-License-Identifier: GPL-3.0-only
 
-# pylint: disable=invalid-name
-
 import json
 import os
 import subprocess
 import sys
 import unittest
 from typing import Any, Sequence
```

### Comparing `wwvb-3.0.7/src/wwvb/testdaylight.py` & `wwvb-3.0.8/src/wwvb/testdaylight.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/src/wwvb/testls.py` & `wwvb-3.0.8/src/wwvb/testls.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/src/wwvb/testpm.py` & `wwvb-3.0.8/src/wwvb/testpm.py`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/src/wwvb/testuwwvb.py` & `wwvb-3.0.8/src/wwvb/testuwwvb.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,15 @@
 
 EitherDatetimeOrNone = Union[None, datetime.datetime, adafruit_datetime.datetime]
 
 
 class WWVBRoundtrip(unittest.TestCase):
     """tests of uwwvb.py"""
 
-    def assertDateTimeEqualExceptTzInfo(  # pylint: disable=invalid-name
-        self, a: EitherDatetimeOrNone, b: EitherDatetimeOrNone
-    ) -> None:
+    def assertDateTimeEqualExceptTzInfo(self, a: EitherDatetimeOrNone, b: EitherDatetimeOrNone) -> None:
         """Test two datetime objects for equality
 
         This equality test excludes tzinfo, and allows adafruit_datetime and core datetime modules to compare equal"""
         assert a
         assert b
         self.assertEqual(
             (a.year, a.month, a.day, a.hour, a.minute, a.second, a.microsecond),
```

### Comparing `wwvb-3.0.7/src/wwvb/testwwvb.py` & `wwvb-3.0.8/src/wwvb/testwwvb.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 class WWVBMinute2k(wwvb.WWVBMinute):
     """Treats the origin of the 2-digit epoch as 2000"""
 
     epoch = 2000
 
 
-# pylint: disable=too-many-locals
 class WWVBTestCase(unittest.TestCase):
     """Test each expected output in tests/.  Some outputs are from another program, some are from us"""
 
     maxDiff = 131072
 
     def test_cases(self) -> None:
         """Generate a test case for each expected output in tests/"""
```

### Comparing `wwvb-3.0.7/src/wwvb/updateiers.py` & `wwvb-3.0.8/src/wwvb/updateiers.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     if url.startswith("http"):
         with requests.get(url, timeout=30) as response:
             return response.text
     else:
         return open(url, encoding="utf-8").read()
 
 
-def update_iersdata(  # pylint: disable=too-many-locals, too-many-branches, too-many-statements
+def update_iersdata(
     target_file: str,
 ) -> None:
     """Update iersdata.py"""
 
     offsets: List[int] = []
     iersdata_text = _get_text(IERS_URL)
     for r in csv.DictReader(io.StringIO(iersdata_text), delimiter=";"):
@@ -126,20 +126,19 @@
     with open(target_file, "wt", encoding="utf-8") as output:
 
         def code(*args: str) -> None:
             """Print to the output file"""
             print(*args, file=output)
 
         code("# -*- python3 -*-")
+        code("# fmt: off")
         code('"""File generated from public data - not subject to copyright"""')
         code("# SPDX" + "-FileCopyrightText: Public domain")
         code("# SPDX" + "-License-Identifier: CC0-1.0")
-        code("# fmt: off")
         code("# isort: skip_file")
-        code("# pylint: disable=invalid-name")
         code("import datetime")
 
         code("__all__ = ['DUT1_DATA_START', 'DUT1_OFFSETS']")
         code(f"DUT1_DATA_START = {repr(table_start)}")
         c = sorted(chr(ord("a") + ch + 10) for ch in set(offsets))
         code(f"{','.join(c)} = tuple({repr(''.join(c))})")
         code(f"DUT1_OFFSETS = str( # {table_start.year:04d}{table_start.month:02d}{table_start.day:02d}")
```

### Comparing `wwvb-3.0.7/src/wwvb/wwvbtk.py` & `wwvb-3.0.8/src/wwvb/wwvbtk.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,31 +5,29 @@
 # SPDX-FileCopyrightText: 2021 Jeff Epler
 #
 # SPDX-License-Identifier: GPL-3.0-only
 
 import functools
 import threading
 import time
-from tkinter import Canvas, TclError, Tk  # pylint: disable=import-error
+from tkinter import Canvas, TclError, Tk
 from typing import Any, Generator, Optional, Tuple
 
 import click
 
 import wwvb
 
 
 @functools.cache
 def _app() -> Tk:
     """Create the Tk application object lazily"""
     return Tk()
 
 
-def validate_colors(  # pylint: disable=unused-argument
-    ctx: Any, param: Any, value: str
-) -> list[str]:
+def validate_colors(ctx: Any, param: Any, value: str) -> list[str]:
     """Check that all colors in a string are valid, splitting it to a list"""
     app = _app()
     colors = value.split()
     if len(colors) not in (2, 3, 4, 6):
         raise click.BadParameter(f"Give 2, 3, 4 or 6 colors (not {len(colors)}")
     for c in colors:
         try:
```

### Comparing `wwvb-3.0.7/src/wwvb.egg-info/PKG-INFO` & `wwvb-3.0.8/src/wwvb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwvb
-Version: 3.0.7
+Version: 3.0.8
 Summary: Generate WWVB timecodes for any desired time
 Home-page: https://github.com/jepler/wwvbpy
 Author: Jeff Epler
 Author-email: jepler@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `wwvb-3.0.7/src/wwvb.egg-info/SOURCES.txt` & `wwvb-3.0.8/src/wwvb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/1998leapsecond` & `wwvb-3.0.8/tests/1998leapsecond`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/all-headers` & `wwvb-3.0.8/tests/all-headers`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/bar` & `wwvb-3.0.8/tests/bar`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/both` & `wwvb-3.0.8/tests/both`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/cradek` & `wwvb-3.0.8/tests/cradek`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/duration` & `wwvb-3.0.8/tests/duration`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/enddst-phase` & `wwvb-3.0.8/tests/enddst-phase`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/enddst-phase-2` & `wwvb-3.0.8/tests/enddst-phase-2`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/negleapsecond` & `wwvb-3.0.8/tests/negleapsecond`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/nextdst` & `wwvb-3.0.8/tests/nextdst`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/nextst` & `wwvb-3.0.8/tests/nextst`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/phase` & `wwvb-3.0.8/tests/phase`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/startdst` & `wwvb-3.0.8/tests/startdst`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/startdst-phase` & `wwvb-3.0.8/tests/startdst-phase`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/startdst-phase-2` & `wwvb-3.0.8/tests/startdst-phase-2`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/startst` & `wwvb-3.0.8/tests/startst`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/y2k` & `wwvb-3.0.8/tests/y2k`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/y2k-1` & `wwvb-3.0.8/tests/y2k-1`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/y2k1` & `wwvb-3.0.8/tests/y2k1`

 * *Files identical despite different names*

### Comparing `wwvb-3.0.7/tests/y2k1-1` & `wwvb-3.0.8/tests/y2k1-1`

 * *Files identical despite different names*

