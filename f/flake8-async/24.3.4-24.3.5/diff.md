# Comparing `tmp/flake8-async-24.3.4.tar.gz` & `tmp/flake8-async-24.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8-async-24.3.4.tar", last modified: Tue Mar 19 18:57:21 2024, max compression
+gzip compressed data, was "flake8-async-24.3.5.tar", last modified: Wed Mar 20 22:13:27 2024, max compression
```

## Comparing `flake8-async-24.3.4.tar` & `flake8-async-24.3.5.tar`

### file list

```diff
@@ -1,117 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:57:21.449340 flake8-async-24.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-03-19 18:57:13.000000 flake8-async-24.3.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-03-19 18:57:13.000000 flake8-async-24.3.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-19 18:57:13.000000 flake8-async-24.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-19 18:57:13.000000 flake8-async-24.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21297 2024-03-19 18:57:21.449340 flake8-async-24.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-03-19 18:57:18.000000 flake8-async-24.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:57:21.433340 flake8-async-24.3.4/flake8_async/
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:57:21.437340 flake8-async-24.3.4/flake8_async/visitors/
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/flake8asyncvisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor100.py
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor101.py
--rw-r--r--   0 runner    (1001) docker     (127)     4620 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor102.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor103_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor105.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor111.py
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor118.py
--rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor2xx.py
--rw-r--r--   0 runner    (1001) docker     (127)    32696 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor91x.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitor_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-03-19 18:57:13.000000 flake8-async-24.3.4/flake8_async/visitors/visitors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:57:21.449340 flake8-async-24.3.4/flake8_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21297 2024-03-19 18:57:21.000000 flake8-async-24.3.4/flake8_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-03-19 18:57:21.000000 flake8-async-24.3.4/flake8_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 18:57:21.000000 flake8-async-24.3.4/flake8_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-19 18:57:21.000000 flake8-async-24.3.4/flake8_async.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 18:57:21.000000 flake8-async-24.3.4/flake8_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-19 18:57:21.000000 flake8-async-24.3.4/flake8_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-19 18:57:21.000000 flake8-async-24.3.4/flake8_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-19 18:57:13.000000 flake8-async-24.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 18:57:21.449340 flake8-async-24.3.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-03-19 18:57:13.000000 flake8-async-24.3.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:57:21.441340 flake8-async-24.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:57:21.441340 flake8-async-24.3.4/tests/autofix_files/
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/autofix_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/autofix_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/autofix_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    28720 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/autofix_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/autofix_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/autofix_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/autofix_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 18:57:21.449340 flake8-async-24.3.4/tests/eval_files/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/anyio_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async100.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async100_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async100_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async100_simple_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async101.py
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async102.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async102_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async102_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async102_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async103.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async103_all_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async103_both_imported.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async103_no_104.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async103_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async104.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async104_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async104_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async105.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async105_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async106.py
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async109.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async110.py
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async111.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async112.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async113.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async113_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async113_trio.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async114.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async115.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async116.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async118.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async200.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async210.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async211.py
--rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async212.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async22x.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async22x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async232.py
--rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async232_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async23x.py
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async23x_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async240.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async250.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async250_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async251.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async251_multi_library.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async900.py
--rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async910.py
--rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async911.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async91x_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/async91x_noautofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/no_library.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/noqa.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/noqa_no_autofix.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/noqa_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/eval_files/trio_anyio.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/test_all_visitors_imported.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/test_changelog_and_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/test_config_and_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/test_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/test_exception_on_invalid_code.py
--rw-r--r--   0 runner    (1001) docker     (127)    28954 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/test_flake8_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/test_formatting.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3240 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/test_messages_documented.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tests/trio_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-19 18:57:13.000000 flake8-async-24.3.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:13:27.606760 flake8-async-24.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     7330 2024-03-20 22:13:17.000000 flake8-async-24.3.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-03-20 22:13:17.000000 flake8-async-24.3.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-20 22:13:17.000000 flake8-async-24.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-20 22:13:17.000000 flake8-async-24.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21505 2024-03-20 22:13:27.606760 flake8-async-24.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13236 2024-03-20 22:13:25.000000 flake8-async-24.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:13:27.590760 flake8-async-24.3.5/flake8_async/
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:13:27.594760 flake8-async-24.3.5/flake8_async/visitors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8896 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/flake8asyncvisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13307 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor100.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor102.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor103_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor105.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor118.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14407 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor2xx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32696 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor91x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitor_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-03-20 22:13:17.000000 flake8-async-24.3.5/flake8_async/visitors/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:13:27.606760 flake8-async-24.3.5/flake8_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21505 2024-03-20 22:13:27.000000 flake8-async-24.3.5/flake8_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-03-20 22:13:27.000000 flake8-async-24.3.5/flake8_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 22:13:27.000000 flake8-async-24.3.5/flake8_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-20 22:13:27.000000 flake8-async-24.3.5/flake8_async.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 22:13:27.000000 flake8-async-24.3.5/flake8_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-20 22:13:27.000000 flake8-async-24.3.5/flake8_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-20 22:13:27.000000 flake8-async-24.3.5/flake8_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4188 2024-03-20 22:13:17.000000 flake8-async-24.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 22:13:27.606760 flake8-async-24.3.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2098 2024-03-20 22:13:17.000000 flake8-async-24.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:13:27.598760 flake8-async-24.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:13:27.598760 flake8-async-24.3.5/tests/autofix_files/
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/autofix_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/autofix_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/autofix_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28720 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/autofix_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/autofix_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/autofix_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/autofix_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 22:13:27.606760 flake8-async-24.3.5/tests/eval_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/anyio_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async100_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async100_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async100_simple_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async101.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7082 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async102.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async102_aclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async102_aclose_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async102_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async102_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async102_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async103.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async103_all_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async103_both_imported.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async103_no_104.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async103_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async104.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async104_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async104_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async105.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async105_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async106.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async109.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async110.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async111.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async112.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async113.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async113_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async113_trio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async114.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async115.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async116.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async118.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async200.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async210.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async211.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2715 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async212.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async22x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async22x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async232.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6255 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async232_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async23x.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async23x_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async240.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async250.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async250_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async251.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async251_multi_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async900.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10585 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async910.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23988 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async911.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async91x_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/async91x_noautofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/no_library.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/noqa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/noqa_no_autofix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/noqa_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/eval_files/trio_anyio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/test_all_visitors_imported.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3604 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/test_changelog_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11124 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/test_config_and_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3455 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/test_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/test_exception_on_invalid_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28954 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/test_flake8_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/test_formatting.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3407 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/test_messages_documented.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tests/trio_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-20 22:13:17.000000 flake8-async-24.3.5/tox.ini
```

### Comparing `flake8-async-24.3.4/CHANGELOG.md` & `flake8-async-24.3.5/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.3.5
+- ASYNC102 (no await inside finally or critical except) no longer raises warnings for calls to `aclose()` on objects in trio/anyio code. See https://github.com/python-trio/flake8-async/issues/156
+
 ## 24.3.4
-- ASYNC110 (don't loop sleep) now also warns if looping `[trio/anyio].lowlevel.checkpoint()`
+- ASYNC110 (don't loop sleep) now also warns if looping `[trio/anyio].lowlevel.checkpoint()`.
 
 ## 24.3.3
 - Add ASYNC251: `time.sleep()` in async method.
 
 ## 24.3.2
 - Add ASYNC250: blocking sync call `input()` in async method.
```

### Comparing `flake8-async-24.3.4/CONTRIBUTING.md` & `flake8-async-24.3.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/LICENSE` & `flake8-async-24.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/PKG-INFO` & `flake8-async-24.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.3.4
+Version: 24.3.5
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/python-trio/flake8-async
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -105,15 +105,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.3.4
+  rev: 24.3.5
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -217,16 +217,19 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.3.5
+- ASYNC102 (no await inside finally or critical except) no longer raises warnings for calls to `aclose()` on objects in trio/anyio code. See https://github.com/python-trio/flake8-async/issues/156
+
 ## 24.3.4
-- ASYNC110 (don't loop sleep) now also warns if looping `[trio/anyio].lowlevel.checkpoint()`
+- ASYNC110 (don't loop sleep) now also warns if looping `[trio/anyio].lowlevel.checkpoint()`.
 
 ## 24.3.3
 - Add ASYNC251: `time.sleep()` in async method.
 
 ## 24.3.2
 - Add ASYNC250: blocking sync call `input()` in async method.
```

### Comparing `flake8-async-24.3.4/README.md` & `flake8-async-24.3.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.3.4
+  rev: 24.3.5
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
```

### Comparing `flake8-async-24.3.4/flake8_async/__init__.py` & `flake8-async-24.3.5/flake8_async/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
     from flake8.options.manager import OptionManager
 
     from .base import Error
 
 
 # CalVer: YY.month.patch, e.g. first release of July 2022 == "22.7.1"
-__version__ = "24.3.4"
+__version__ = "24.3.5"
 
 
 # taken from https://github.com/Zac-HD/shed
 @functools.lru_cache
 def _get_git_repo_root(cwd: str | None = None) -> str:
     return subprocess.run(
         ["git", "rev-parse", "--show-toplevel"],
```

### Comparing `flake8-async-24.3.4/flake8_async/base.py` & `flake8-async-24.3.5/flake8_async/base.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/runner.py` & `flake8-async-24.3.5/flake8_async/runner.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/__init__.py` & `flake8-async-24.3.5/flake8_async/visitors/__init__.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/flake8asyncvisitor.py` & `flake8-async-24.3.5/flake8_async/visitors/flake8asyncvisitor.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/helpers.py` & `flake8-async-24.3.5/flake8_async/visitors/helpers.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor100.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor101.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor101.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor103_104.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor103_104.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor105.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor105.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor111.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor111.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor118.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor118.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor2xx.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor2xx.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor91x.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor91x.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitor_utility.py` & `flake8-async-24.3.5/flake8_async/visitors/visitor_utility.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async/visitors/visitors.py` & `flake8-async-24.3.5/flake8_async/visitors/visitors.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/flake8_async.egg-info/PKG-INFO` & `flake8-async-24.3.5/flake8_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-async
-Version: 24.3.4
+Version: 24.3.5
 Summary: A highly opinionated flake8 plugin for Trio-related problems.
 Home-page: https://github.com/python-trio/flake8-async
 Author: Zac Hatfield-Dodds, John Litborn, and Contributors
 Author-email: zac@zhd.dev
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flake8
@@ -105,15 +105,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with flake8-async by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/python-trio/flake8-async
-  rev: 24.3.4
+  rev: 24.3.5
   hooks:
     - id: flake8-async
       # args: [--enable=ASYNC, --disable=ASYNC9, --autofix=ASYNC]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
 can avoid running `flake8-async` on unchanged files.
@@ -217,16 +217,19 @@
     arbitrary_other_function(my_blocking_call=None)
 ```
 
 
 # Changelog
 *[CalVer, YY.month.patch](https://calver.org/)*
 
+## 24.3.5
+- ASYNC102 (no await inside finally or critical except) no longer raises warnings for calls to `aclose()` on objects in trio/anyio code. See https://github.com/python-trio/flake8-async/issues/156
+
 ## 24.3.4
-- ASYNC110 (don't loop sleep) now also warns if looping `[trio/anyio].lowlevel.checkpoint()`
+- ASYNC110 (don't loop sleep) now also warns if looping `[trio/anyio].lowlevel.checkpoint()`.
 
 ## 24.3.3
 - Add ASYNC251: `time.sleep()` in async method.
 
 ## 24.3.2
 - Add ASYNC250: blocking sync call `input()` in async method.
```

### Comparing `flake8-async-24.3.4/flake8_async.egg-info/SOURCES.txt` & `flake8-async-24.3.5/flake8_async.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,16 @@
 tests/eval_files/anyio_trio.py
 tests/eval_files/async100.py
 tests/eval_files/async100_asyncio.py
 tests/eval_files/async100_noautofix.py
 tests/eval_files/async100_simple_autofix.py
 tests/eval_files/async101.py
 tests/eval_files/async102.py
+tests/eval_files/async102_aclose.py
+tests/eval_files/async102_aclose_args.py
 tests/eval_files/async102_anyio.py
 tests/eval_files/async102_asyncio.py
 tests/eval_files/async102_trio.py
 tests/eval_files/async103.py
 tests/eval_files/async103_all_imported.py
 tests/eval_files/async103_both_imported.py
 tests/eval_files/async103_no_104.py
```

### Comparing `flake8-async-24.3.4/pyproject.toml` & `flake8-async-24.3.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/setup.py` & `flake8-async-24.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/autofix_files/async100.py` & `flake8-async-24.3.5/tests/autofix_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/autofix_files/async100_simple_autofix.py` & `flake8-async-24.3.5/tests/autofix_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/autofix_files/async910.py` & `flake8-async-24.3.5/tests/autofix_files/async910.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/autofix_files/async911.py` & `flake8-async-24.3.5/tests/autofix_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/autofix_files/async91x_autofix.py` & `flake8-async-24.3.5/tests/autofix_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/autofix_files/noqa.py` & `flake8-async-24.3.5/tests/autofix_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/conftest.py` & `flake8-async-24.3.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async100.py` & `flake8-async-24.3.5/tests/eval_files/async100.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async100_asyncio.py` & `flake8-async-24.3.5/tests/eval_files/async100_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async100_noautofix.py` & `flake8-async-24.3.5/tests/eval_files/async100_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async100_simple_autofix.py` & `flake8-async-24.3.5/tests/eval_files/async100_simple_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async101.py` & `flake8-async-24.3.5/tests/eval_files/async101.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async102.py` & `flake8-async-24.3.5/tests/eval_files/async102.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,7 +248,20 @@
             await foo()
         except BaseException:
             await foo()  # error: 12, Statement("BaseException", lineno-1)
         except:
             await foo()
         await foo()
     await foo()
+
+
+# double check that this works nested inside an async for
+async def foo_nested_async_for():
+
+    async for i in trio.bypasslinters:
+        try:
+            ...
+        except BaseException:
+            async for (  # error: 12, Statement("BaseException", lineno-1)
+                j
+            ) in trio.bypasslinters:
+                ...
```

### Comparing `flake8-async-24.3.4/tests/eval_files/async102_anyio.py` & `flake8-async-24.3.5/tests/eval_files/async102_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async102_asyncio.py` & `flake8-async-24.3.5/tests/eval_files/async102_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async102_trio.py` & `flake8-async-24.3.5/tests/eval_files/async102_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async103.py` & `flake8-async-24.3.5/tests/eval_files/async103.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async103_all_imported.py` & `flake8-async-24.3.5/tests/eval_files/async103_all_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async103_both_imported.py` & `flake8-async-24.3.5/tests/eval_files/async103_both_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async103_trio.py` & `flake8-async-24.3.5/tests/eval_files/async103_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async104.py` & `flake8-async-24.3.5/tests/eval_files/async104.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async104_anyio.py` & `flake8-async-24.3.5/tests/eval_files/async104_anyio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async105.py` & `flake8-async-24.3.5/tests/eval_files/async105.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async106.py` & `flake8-async-24.3.5/tests/eval_files/async106.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async109.py` & `flake8-async-24.3.5/tests/eval_files/async109.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async110.py` & `flake8-async-24.3.5/tests/eval_files/async110.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async111.py` & `flake8-async-24.3.5/tests/eval_files/async111.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async112.py` & `flake8-async-24.3.5/tests/eval_files/async112.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async113.py` & `flake8-async-24.3.5/tests/eval_files/async113.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async113_trio.py` & `flake8-async-24.3.5/tests/eval_files/async113_trio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async114.py` & `flake8-async-24.3.5/tests/eval_files/async114.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async115.py` & `flake8-async-24.3.5/tests/eval_files/async115.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async116.py` & `flake8-async-24.3.5/tests/eval_files/async116.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async118.py` & `flake8-async-24.3.5/tests/eval_files/async118.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async200.py` & `flake8-async-24.3.5/tests/eval_files/async200.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async210.py` & `flake8-async-24.3.5/tests/eval_files/async210.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async211.py` & `flake8-async-24.3.5/tests/eval_files/async211.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async212.py` & `flake8-async-24.3.5/tests/eval_files/async212.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async22x.py` & `flake8-async-24.3.5/tests/eval_files/async22x.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async22x_asyncio.py` & `flake8-async-24.3.5/tests/eval_files/async22x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async232.py` & `flake8-async-24.3.5/tests/eval_files/async232.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async232_asyncio.py` & `flake8-async-24.3.5/tests/eval_files/async232_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async23x.py` & `flake8-async-24.3.5/tests/eval_files/async23x.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async23x_asyncio.py` & `flake8-async-24.3.5/tests/eval_files/async23x_asyncio.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async240.py` & `flake8-async-24.3.5/tests/eval_files/async240.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async900.py` & `flake8-async-24.3.5/tests/eval_files/async900.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async910.py` & `flake8-async-24.3.5/tests/eval_files/async910.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async911.py` & `flake8-async-24.3.5/tests/eval_files/async911.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async91x_autofix.py` & `flake8-async-24.3.5/tests/eval_files/async91x_autofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/async91x_noautofix.py` & `flake8-async-24.3.5/tests/eval_files/async91x_noautofix.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/eval_files/noqa.py` & `flake8-async-24.3.5/tests/eval_files/noqa.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/test_all_visitors_imported.py` & `flake8-async-24.3.5/tests/test_all_visitors_imported.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/test_changelog_and_version.py` & `flake8-async-24.3.5/tests/test_changelog_and_version.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/test_config_and_args.py` & `flake8-async-24.3.5/tests/test_config_and_args.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/test_decorator.py` & `flake8-async-24.3.5/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/test_exception_on_invalid_code.py` & `flake8-async-24.3.5/tests/test_exception_on_invalid_code.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/test_flake8_async.py` & `flake8-async-24.3.5/tests/test_flake8_async.py`

 * *Files identical despite different names*

### Comparing `flake8-async-24.3.4/tests/test_messages_documented.py` & `flake8-async-24.3.5/tests/test_messages_documented.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,17 @@
     # get tested error codes from file names and from `# ARG --enable` lines
     documented_errors["eval_files"] = set()
     p = Path(__file__).parent / "eval_files"
     for file_path in p.iterdir():
         if not file_path.is_file():
             continue
 
-        if m := re.search(r"async\d\d\d", str(file_path)):
+        # only look in the stem (final part of the path), so as not to get tripped
+        # up by [git worktree] directories with an exception code in the name
+        if m := re.search(r"^async\d\d\d", str(file_path.stem)):
             documented_errors["eval_files"].add(m.group().upper())
 
         with open(file_path) as file:
             for line in file:
                 if line.startswith("# ARG --enable"):
                     for m in re.findall(r"async\d\d\d", line, re.IGNORECASE):
                         # pyright types m as `Any` (as it is in typeshed)
```

### Comparing `flake8-async-24.3.4/tox.ini` & `flake8-async-24.3.5/tox.ini`

 * *Files identical despite different names*

