# Comparing `tmp/calcbench_api_client-9.1.1.tar.gz` & `tmp/calcbench_api_client-9.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\calcbench_api_client-9.1.1.tar", last modified: Thu Jul 13 20:36:14 2023, max compression
+gzip compressed data, was "dist\calcbench_api_client-9.2.0.tar", last modified: Wed Aug  9 13:07:27 2023, max compression
```

## Comparing `calcbench_api_client-9.1.1.tar` & `calcbench_api_client-9.2.0.tar`

### file list

```diff
@@ -1,103 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.994129 calcbench_api_client-9.1.1/
--rw-rw-rw-   0        0        0      288 2021-05-18 15:59:00.000000 calcbench_api_client-9.1.1/.gitignore
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.645131 calcbench_api_client-9.1.1/.vscode/
--rw-rw-rw-   0        0        0      478 2021-05-18 15:57:34.000000 calcbench_api_client-9.1.1/.vscode/launch.json
--rw-rw-rw-   0        0        0     1988 2023-07-13 20:36:13.993170 calcbench_api_client-9.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      984 2023-06-06 17:23:29.000000 calcbench_api_client-9.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.681172 calcbench_api_client-9.1.1/calcbench/
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.684129 calcbench_api_client-9.1.1/calcbench/.vscode/
--rw-rw-rw-   0        0        0      477 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/calcbench/.vscode/launch.json
--rw-rw-rw-   0        0        0     1812 2023-07-13 20:35:52.000000 calcbench_api_client-9.1.1/calcbench/__init__.py
--rw-rw-rw-   0        0        0    11918 2023-03-16 20:14:00.000000 calcbench_api_client-9.1.1/calcbench/api_client.py
--rw-rw-rw-   0        0        0     2325 2023-07-13 19:10:00.000000 calcbench_api_client-9.1.1/calcbench/api_query_params.py
--rw-rw-rw-   0        0        0    15686 2023-05-08 15:32:07.000000 calcbench_api_client-9.1.1/calcbench/business_combinations.py
--rw-rw-rw-   0        0        0     3920 2021-11-18 16:53:40.000000 calcbench_api_client-9.1.1/calcbench/companies.py
--rw-rw-rw-   0        0        0    17369 2022-02-15 16:51:25.000000 calcbench_api_client-9.1.1/calcbench/dimensional.py
--rw-rw-rw-   0        0        0    18077 2022-11-02 16:00:32.000000 calcbench_api_client-9.1.1/calcbench/disclosures.py
--rw-rw-rw-   0        0        0     5726 2023-05-31 16:10:02.000000 calcbench_api_client-9.1.1/calcbench/downloaders.py
--rw-rw-rw-   0        0        0     3700 2022-05-31 19:56:12.000000 calcbench_api_client-9.1.1/calcbench/face_statements.py
--rw-rw-rw-   0        0        0    11386 2023-01-19 15:50:21.000000 calcbench_api_client-9.1.1/calcbench/filing.py
--rw-rw-rw-   0        0        0     8910 2022-07-15 14:07:23.000000 calcbench_api_client-9.1.1/calcbench/listener.py
--rw-rw-rw-   0        0        0      650 2020-12-11 14:41:26.000000 calcbench_api_client-9.1.1/calcbench/metrics.py
--rw-rw-rw-   0        0        0     3269 2022-11-07 16:43:08.000000 calcbench_api_client-9.1.1/calcbench/press_release.py
--rw-rw-rw-   0        0        0     4456 2021-11-18 17:07:01.000000 calcbench_api_client-9.1.1/calcbench/raw_numeric_XBRL.py
--rw-rw-rw-   0        0        0     5968 2022-03-18 15:19:02.000000 calcbench_api_client-9.1.1/calcbench/raw_numeric_non_XBRL.py
--rw-rw-rw-   0        0        0    20191 2023-07-13 20:35:23.000000 calcbench_api_client-9.1.1/calcbench/standardized_numeric.py
--rw-rw-rw-   0        0        0      664 2023-07-13 18:24:08.000000 calcbench_api_client-9.1.1/calcbench/standardized_parameters.py
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.706135 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/
--rw-rw-rw-   0        0        0     1988 2023-07-13 20:36:13.000000 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-07-13 20:36:13.000000 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 20:36:13.000000 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/dependency_links.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.710128 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/dist/
--rw-rw-rw-   0        0        0    68879 2022-01-27 15:55:06.000000 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
--rw-rw-rw-   0        0        0   418889 2022-01-27 15:55:05.000000 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz
--rw-rw-rw-   0        0        0      270 2023-07-13 20:36:13.000000 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 20:36:13.000000 calcbench_api_client-9.1.1/calcbench_api_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.713136 calcbench_api_client-9.1.1/conda-recipe/
--rw-rw-rw-   0        0        0      909 2022-06-30 14:34:48.000000 calcbench_api_client-9.1.1/conda-recipe/meta.yaml
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.723133 calcbench_api_client-9.1.1/docs/
--rw-rw-rw-   0        0        0        0 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/docs/.nojekyll
--rw-rw-rw-   0        0        0      654 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.855129 calcbench_api_client-9.1.1/docs/html/
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.857176 calcbench_api_client-9.1.1/docs/html/_sources/
--rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.1.1/docs/html/_sources/getting-started.rst.txt
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.951129 calcbench_api_client-9.1.1/docs/html/_static/
--rw-rw-rw-   0        0        0    11885 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/_static/alabaster.css
--rw-rw-rw-   0        0        0    15541 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/_static/basic.css
--rw-rw-rw-   0        0        0       42 2020-03-19 21:59:59.000000 calcbench_api_client-9.1.1/docs/html/_static/custom.css
--rw-rw-rw-   0        0        0     9630 2021-07-29 16:06:08.000000 calcbench_api_client-9.1.1/docs/html/_static/doctools.js
--rw-rw-rw-   0        0        0      361 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/_static/documentation_options.js
--rw-rw-rw-   0        0        0      286 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/docs/html/_static/file.png
--rw-rw-rw-   0        0        0   278292 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/docs/html/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0   280364 2020-03-19 22:00:02.000000 calcbench_api_client-9.1.1/docs/html/_static/jquery-3.4.1.js
--rw-rw-rw-   0        0        0   287630 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.1/docs/html/_static/jquery-3.5.1.js
--rw-rw-rw-   0        0        0    89476 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.1/docs/html/_static/jquery.js
--rw-rw-rw-   0        0        0    11151 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/_static/language_data.js
--rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/docs/html/_static/minus.png
--rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/docs/html/_static/plus.png
--rw-rw-rw-   0        0        0     4874 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/_static/pygments.css
--rw-rw-rw-   0        0        0    16578 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.1/docs/html/_static/searchtools.js
--rw-rw-rw-   0        0        0    68420 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.1/docs/html/_static/underscore-1.13.1.js
--rw-rw-rw-   0        0        0    35168 2020-03-19 22:00:02.000000 calcbench_api_client-9.1.1/docs/html/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    19530 2021-07-29 16:06:09.000000 calcbench_api_client-9.1.1/docs/html/_static/underscore.js
--rw-rw-rw-   0        0        0    20866 2023-07-13 20:35:37.000000 calcbench_api_client-9.1.1/docs/html/business-combinations.html
--rw-rw-rw-   0        0        0    12664 2022-01-27 15:45:17.000000 calcbench_api_client-9.1.1/docs/html/companies.html
--rw-rw-rw-   0        0        0   116341 2023-07-13 20:35:37.000000 calcbench_api_client-9.1.1/docs/html/dimensional.html
--rw-rw-rw-   0        0        0    65621 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.1/docs/html/disclosures.html
--rw-rw-rw-   0        0        0    19795 2023-07-10 22:58:11.000000 calcbench_api_client-9.1.1/docs/html/downloaders.html
--rw-rw-rw-   0        0        0    35986 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.1/docs/html/face-statements.html
--rw-rw-rw-   0        0        0    46164 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/filings.html
--rw-rw-rw-   0        0        0   107809 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/genindex.html
--rw-rw-rw-   0        0        0    14252 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/getting-started.html
--rw-rw-rw-   0        0        0     7429 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/index.html
--rw-rw-rw-   0        0        0     6017 2022-01-27 15:45:17.000000 calcbench_api_client-9.1.1/docs/html/metrics.html
--rw-rw-rw-   0        0        0    39128 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/numeric-data.html
--rw-rw-rw-   0        0        0    20870 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.1/docs/html/press-release.html
--rw-rw-rw-   0        0        0    11099 2023-01-19 19:18:13.000000 calcbench_api_client-9.1.1/docs/html/push-notification.html
--rw-rw-rw-   0        0        0     7083 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/py-modindex.html
--rw-rw-rw-   0        0        0    18689 2022-01-27 15:45:18.000000 calcbench_api_client-9.1.1/docs/html/raw-numeric-XBRL.html
--rw-rw-rw-   0        0        0    36953 2023-07-13 19:26:28.000000 calcbench_api_client-9.1.1/docs/html/raw-numeric-non-XBRL.html
--rw-rw-rw-   0        0        0     4370 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/search.html
--rw-rw-rw-   0        0        0    47639 2023-07-13 20:35:38.000000 calcbench_api_client-9.1.1/docs/html/searchindex.js
--rw-rw-rw-   0        0        0       64 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/docs/index.html
--rwxrwxrwx   0        0        0      796 2020-03-11 15:22:24.000000 calcbench_api_client-9.1.1/docs/make.bat
-drwxrwxrwx   0        0        0        0 2023-07-13 20:36:13.991130 calcbench_api_client-9.1.1/docs/source/
--rw-rw-rw-   0        0        0      274 2021-06-24 19:28:47.000000 calcbench_api_client-9.1.1/docs/source/business-combinations.rst
--rw-rw-rw-   0        0        0      132 2021-02-22 22:31:03.000000 calcbench_api_client-9.1.1/docs/source/companies.rst
--rw-rw-rw-   0        0        0     1907 2022-01-27 15:45:13.000000 calcbench_api_client-9.1.1/docs/source/conf.py
--rw-rw-rw-   0        0        0      275 2021-10-13 15:58:17.000000 calcbench_api_client-9.1.1/docs/source/dimensional.rst
--rw-rw-rw-   0        0        0      369 2021-07-23 16:57:12.000000 calcbench_api_client-9.1.1/docs/source/disclosures.rst
--rw-rw-rw-   0        0        0      113 2022-01-13 16:45:20.000000 calcbench_api_client-9.1.1/docs/source/downloaders.rst
--rw-rw-rw-   0        0        0      176 2022-05-31 19:08:45.000000 calcbench_api_client-9.1.1/docs/source/face-statements.rst
--rw-rw-rw-   0        0        0       90 2022-01-27 17:08:05.000000 calcbench_api_client-9.1.1/docs/source/filings.rst
--rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.1.1/docs/source/getting-started.rst
--rw-rw-rw-   0        0        0      669 2022-01-13 16:44:16.000000 calcbench_api_client-9.1.1/docs/source/index.rst
--rw-rw-rw-   0        0        0       70 2020-11-12 16:28:47.000000 calcbench_api_client-9.1.1/docs/source/metrics.rst
--rw-rw-rw-   0        0        0      906 2022-11-07 16:43:08.000000 calcbench_api_client-9.1.1/docs/source/numeric-data.rst
--rw-rw-rw-   0        0        0      181 2021-11-18 18:30:32.000000 calcbench_api_client-9.1.1/docs/source/press-release.rst
--rw-rw-rw-   0        0        0     1002 2020-12-11 15:03:48.000000 calcbench_api_client-9.1.1/docs/source/push-notification.rst
--rw-rw-rw-   0        0        0      208 2021-05-04 16:55:43.000000 calcbench_api_client-9.1.1/docs/source/raw-numeric-XBRL.rst
--rw-rw-rw-   0        0        0      215 2021-04-05 15:28:06.000000 calcbench_api_client-9.1.1/docs/source/raw-numeric-non-XBRL.rst
--rw-rw-rw-   0        0        0       93 2020-10-22 17:34:48.000000 calcbench_api_client-9.1.1/publish.PS1
--rw-rw-rw-   0        0        0       42 2023-07-13 20:36:13.995128 calcbench_api_client-9.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1418 2023-01-26 15:29:46.000000 calcbench_api_client-9.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:27.090209 calcbench_api_client-9.2.0/
+-rw-rw-rw-   0        0        0      288 2021-05-18 15:59:00.000000 calcbench_api_client-9.2.0/.gitignore
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.184902 calcbench_api_client-9.2.0/.vscode/
+-rw-rw-rw-   0        0        0      478 2021-05-18 15:57:34.000000 calcbench_api_client-9.2.0/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1988 2023-08-09 13:07:27.089218 calcbench_api_client-9.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      984 2023-06-06 17:23:29.000000 calcbench_api_client-9.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.224903 calcbench_api_client-9.2.0/calcbench/
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.239898 calcbench_api_client-9.2.0/calcbench/.vscode/
+-rw-rw-rw-   0        0        0      477 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/calcbench/.vscode/launch.json
+-rw-rw-rw-   0        0        0     1812 2023-08-09 13:07:13.000000 calcbench_api_client-9.2.0/calcbench/__init__.py
+-rw-rw-rw-   0        0        0    11918 2023-03-16 20:14:00.000000 calcbench_api_client-9.2.0/calcbench/api_client.py
+-rw-rw-rw-   0        0        0     2325 2023-07-13 19:10:00.000000 calcbench_api_client-9.2.0/calcbench/api_query_params.py
+-rw-rw-rw-   0        0        0    15686 2023-05-08 15:32:07.000000 calcbench_api_client-9.2.0/calcbench/business_combinations.py
+-rw-rw-rw-   0        0        0     3920 2021-11-18 16:53:40.000000 calcbench_api_client-9.2.0/calcbench/companies.py
+-rw-rw-rw-   0        0        0    17369 2022-02-15 16:51:25.000000 calcbench_api_client-9.2.0/calcbench/dimensional.py
+-rw-rw-rw-   0        0        0    18077 2022-11-02 16:00:32.000000 calcbench_api_client-9.2.0/calcbench/disclosures.py
+-rw-rw-rw-   0        0        0     6285 2023-08-09 13:01:16.000000 calcbench_api_client-9.2.0/calcbench/downloaders.py
+-rw-rw-rw-   0        0        0     3700 2022-05-31 19:56:12.000000 calcbench_api_client-9.2.0/calcbench/face_statements.py
+-rw-rw-rw-   0        0        0    11386 2023-01-19 15:50:21.000000 calcbench_api_client-9.2.0/calcbench/filing.py
+-rw-rw-rw-   0        0        0     8910 2022-07-15 14:07:23.000000 calcbench_api_client-9.2.0/calcbench/listener.py
+-rw-rw-rw-   0        0        0      650 2020-12-11 14:41:26.000000 calcbench_api_client-9.2.0/calcbench/metrics.py
+-rw-rw-rw-   0        0        0     3269 2022-11-07 16:43:08.000000 calcbench_api_client-9.2.0/calcbench/press_release.py
+-rw-rw-rw-   0        0        0     4456 2021-11-18 17:07:01.000000 calcbench_api_client-9.2.0/calcbench/raw_numeric_XBRL.py
+-rw-rw-rw-   0        0        0     5968 2022-03-18 15:19:02.000000 calcbench_api_client-9.2.0/calcbench/raw_numeric_non_XBRL.py
+-rw-rw-rw-   0        0        0    20191 2023-07-13 20:35:23.000000 calcbench_api_client-9.2.0/calcbench/standardized_numeric.py
+-rw-rw-rw-   0        0        0      664 2023-07-13 18:24:08.000000 calcbench_api_client-9.2.0/calcbench/standardized_parameters.py
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.279899 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/
+-rw-rw-rw-   0        0        0     1988 2023-08-09 13:07:25.000000 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-08-09 13:07:26.000000 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-09 13:07:25.000000 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/dependency_links.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.303941 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/dist/
+-rw-rw-rw-   0        0        0    68879 2022-01-27 15:55:06.000000 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl
+-rw-rw-rw-   0        0        0   418889 2022-01-27 15:55:05.000000 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz
+-rw-rw-rw-   0        0        0      270 2023-08-09 13:07:25.000000 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-09 13:07:25.000000 calcbench_api_client-9.2.0/calcbench_api_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.312965 calcbench_api_client-9.2.0/conda-recipe/
+-rw-rw-rw-   0        0        0      909 2022-06-30 14:34:48.000000 calcbench_api_client-9.2.0/conda-recipe/meta.yaml
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.330804 calcbench_api_client-9.2.0/docs/
+-rw-rw-rw-   0        0        0        0 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/docs/.nojekyll
+-rw-rw-rw-   0        0        0      654 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.533189 calcbench_api_client-9.2.0/docs/html/
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.537157 calcbench_api_client-9.2.0/docs/html/_sources/
+-rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.2.0/docs/html/_sources/getting-started.rst.txt
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:26.932659 calcbench_api_client-9.2.0/docs/html/_static/
+-rw-rw-rw-   0        0        0    11885 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/_static/alabaster.css
+-rw-rw-rw-   0        0        0    15541 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/_static/basic.css
+-rw-rw-rw-   0        0        0       42 2020-03-19 21:59:59.000000 calcbench_api_client-9.2.0/docs/html/_static/custom.css
+-rw-rw-rw-   0        0        0     9630 2021-07-29 16:06:08.000000 calcbench_api_client-9.2.0/docs/html/_static/doctools.js
+-rw-rw-rw-   0        0        0      361 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      286 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/docs/html/_static/file.png
+-rw-rw-rw-   0        0        0   278292 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/docs/html/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0   280364 2020-03-19 22:00:02.000000 calcbench_api_client-9.2.0/docs/html/_static/jquery-3.4.1.js
+-rw-rw-rw-   0        0        0   287630 2021-07-29 16:06:09.000000 calcbench_api_client-9.2.0/docs/html/_static/jquery-3.5.1.js
+-rw-rw-rw-   0        0        0    89476 2021-07-29 16:06:09.000000 calcbench_api_client-9.2.0/docs/html/_static/jquery.js
+-rw-rw-rw-   0        0        0    11151 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/_static/language_data.js
+-rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/docs/html/_static/minus.png
+-rw-rw-rw-   0        0        0       90 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/docs/html/_static/plus.png
+-rw-rw-rw-   0        0        0     4874 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/_static/pygments.css
+-rw-rw-rw-   0        0        0    16578 2021-07-29 16:06:09.000000 calcbench_api_client-9.2.0/docs/html/_static/searchtools.js
+-rw-rw-rw-   0        0        0    68420 2021-07-29 16:06:09.000000 calcbench_api_client-9.2.0/docs/html/_static/underscore-1.13.1.js
+-rw-rw-rw-   0        0        0    35168 2020-03-19 22:00:02.000000 calcbench_api_client-9.2.0/docs/html/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    19530 2021-07-29 16:06:09.000000 calcbench_api_client-9.2.0/docs/html/_static/underscore.js
+-rw-rw-rw-   0        0        0    20866 2023-07-13 20:35:37.000000 calcbench_api_client-9.2.0/docs/html/business-combinations.html
+-rw-rw-rw-   0        0        0    12664 2022-01-27 15:45:17.000000 calcbench_api_client-9.2.0/docs/html/companies.html
+-rw-rw-rw-   0        0        0   116341 2023-07-13 20:35:37.000000 calcbench_api_client-9.2.0/docs/html/dimensional.html
+-rw-rw-rw-   0        0        0    65621 2023-07-13 19:26:28.000000 calcbench_api_client-9.2.0/docs/html/disclosures.html
+-rw-rw-rw-   0        0        0    21153 2023-08-09 12:47:24.000000 calcbench_api_client-9.2.0/docs/html/downloaders.html
+-rw-rw-rw-   0        0        0    35986 2023-07-13 19:26:28.000000 calcbench_api_client-9.2.0/docs/html/face-statements.html
+-rw-rw-rw-   0        0        0    46164 2023-07-13 20:35:38.000000 calcbench_api_client-9.2.0/docs/html/filings.html
+-rw-rw-rw-   0        0        0   107809 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/genindex.html
+-rw-rw-rw-   0        0        0    14252 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/getting-started.html
+-rw-rw-rw-   0        0        0     7429 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/index.html
+-rw-rw-rw-   0        0        0     6017 2022-01-27 15:45:17.000000 calcbench_api_client-9.2.0/docs/html/metrics.html
+-rw-rw-rw-   0        0        0    39128 2023-07-13 20:35:38.000000 calcbench_api_client-9.2.0/docs/html/numeric-data.html
+-rw-rw-rw-   0        0        0    20870 2023-07-13 19:26:28.000000 calcbench_api_client-9.2.0/docs/html/press-release.html
+-rw-rw-rw-   0        0        0    11099 2023-01-19 19:18:13.000000 calcbench_api_client-9.2.0/docs/html/push-notification.html
+-rw-rw-rw-   0        0        0     7083 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/py-modindex.html
+-rw-rw-rw-   0        0        0    18689 2022-01-27 15:45:18.000000 calcbench_api_client-9.2.0/docs/html/raw-numeric-XBRL.html
+-rw-rw-rw-   0        0        0    36953 2023-07-13 19:26:28.000000 calcbench_api_client-9.2.0/docs/html/raw-numeric-non-XBRL.html
+-rw-rw-rw-   0        0        0     4370 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/search.html
+-rw-rw-rw-   0        0        0    47693 2023-08-09 12:47:25.000000 calcbench_api_client-9.2.0/docs/html/searchindex.js
+-rw-rw-rw-   0        0        0       64 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/docs/index.html
+-rwxrwxrwx   0        0        0      796 2020-03-11 15:22:24.000000 calcbench_api_client-9.2.0/docs/make.bat
+drwxrwxrwx   0        0        0        0 2023-08-09 13:07:27.087212 calcbench_api_client-9.2.0/docs/source/
+-rw-rw-rw-   0        0        0      274 2021-06-24 19:28:47.000000 calcbench_api_client-9.2.0/docs/source/business-combinations.rst
+-rw-rw-rw-   0        0        0      132 2021-02-22 22:31:03.000000 calcbench_api_client-9.2.0/docs/source/companies.rst
+-rw-rw-rw-   0        0        0     1907 2022-01-27 15:45:13.000000 calcbench_api_client-9.2.0/docs/source/conf.py
+-rw-rw-rw-   0        0        0      275 2021-10-13 15:58:17.000000 calcbench_api_client-9.2.0/docs/source/dimensional.rst
+-rw-rw-rw-   0        0        0      369 2021-07-23 16:57:12.000000 calcbench_api_client-9.2.0/docs/source/disclosures.rst
+-rw-rw-rw-   0        0        0      113 2022-01-13 16:45:20.000000 calcbench_api_client-9.2.0/docs/source/downloaders.rst
+-rw-rw-rw-   0        0        0      176 2022-05-31 19:08:45.000000 calcbench_api_client-9.2.0/docs/source/face-statements.rst
+-rw-rw-rw-   0        0        0       90 2022-01-27 17:08:05.000000 calcbench_api_client-9.2.0/docs/source/filings.rst
+-rw-rw-rw-   0        0        0     1299 2023-01-26 15:56:17.000000 calcbench_api_client-9.2.0/docs/source/getting-started.rst
+-rw-rw-rw-   0        0        0      669 2022-01-13 16:44:16.000000 calcbench_api_client-9.2.0/docs/source/index.rst
+-rw-rw-rw-   0        0        0       70 2020-11-12 16:28:47.000000 calcbench_api_client-9.2.0/docs/source/metrics.rst
+-rw-rw-rw-   0        0        0      906 2022-11-07 16:43:08.000000 calcbench_api_client-9.2.0/docs/source/numeric-data.rst
+-rw-rw-rw-   0        0        0      181 2021-11-18 18:30:32.000000 calcbench_api_client-9.2.0/docs/source/press-release.rst
+-rw-rw-rw-   0        0        0     1002 2020-12-11 15:03:48.000000 calcbench_api_client-9.2.0/docs/source/push-notification.rst
+-rw-rw-rw-   0        0        0      208 2021-05-04 16:55:43.000000 calcbench_api_client-9.2.0/docs/source/raw-numeric-XBRL.rst
+-rw-rw-rw-   0        0        0      215 2021-04-05 15:28:06.000000 calcbench_api_client-9.2.0/docs/source/raw-numeric-non-XBRL.rst
+-rw-rw-rw-   0        0        0       93 2020-10-22 17:34:48.000000 calcbench_api_client-9.2.0/publish.PS1
+-rw-rw-rw-   0        0        0       42 2023-08-09 13:07:27.091210 calcbench_api_client-9.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1418 2023-01-26 15:29:46.000000 calcbench_api_client-9.2.0/setup.py
```

### Comparing `calcbench_api_client-9.1.1/PKG-INFO` & `calcbench_api_client-9.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcbench_api_client
-Version: 9.1.1
+Version: 9.2.0
 Summary: Client for Calcbench data.
 Home-page: https://github.com/calcbench/python_api_client
 Author: Andrew Kittredge
 Author-email: andrew@calcbench.com
 License: Apache2
 Project-URL: Documentation, http://calcbench.github.io/python_api_client/html/index.html
 Project-URL: Examples, https://github.com/calcbench/notebooks
@@ -46,13 +46,13 @@
         @someben https://github.com/calcbench/python_api_client/commit/6c2312525fa365acc91bd8e979037fc2492845f3
         
 Keywords: finance accounting SEC 10-(K|Q)
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: Listener
+Provides-Extra: Backoff
+Provides-Extra: BeautifulSoup
 Provides-Extra: Keyring
+Provides-Extra: pyarrow
 Provides-Extra: tqdm
 Provides-Extra: Pandas
-Provides-Extra: pyarrow
-Provides-Extra: BeautifulSoup
-Provides-Extra: Backoff
```

### Comparing `calcbench_api_client-9.1.1/README.md` & `calcbench_api_client-9.2.0/README.md`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/__init__.py` & `calcbench_api_client-9.2.0/calcbench/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 The "public" properties on the cb module
 
 """
-__version__ = "9.1.1"
+__version__ = "9.2.0"
 from datetime import datetime
 import logging
 from .api_client import (
     enable_backoff,
     html_diff,
     set_credentials,
     set_proxies,
```

### Comparing `calcbench_api_client-9.1.1/calcbench/api_client.py` & `calcbench_api_client-9.2.0/calcbench/api_client.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/api_query_params.py` & `calcbench_api_client-9.2.0/calcbench/api_query_params.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/business_combinations.py` & `calcbench_api_client-9.2.0/calcbench/business_combinations.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/companies.py` & `calcbench_api_client-9.2.0/calcbench/companies.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/dimensional.py` & `calcbench_api_client-9.2.0/calcbench/dimensional.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/disclosures.py` & `calcbench_api_client-9.2.0/calcbench/disclosures.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/downloaders.py` & `calcbench_api_client-9.2.0/calcbench/downloaders.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import shutil
 from typing import Callable, List, Literal, Optional, Sequence, TypeVar, Union
 from pathlib import Path
 
 from requests import HTTPError
 
 
 import calcbench as cb
@@ -118,17 +120,23 @@
 
 
 def iterate_and_save_pyarrow_dataset(
     arguments: Sequence[T],
     f: Callable[[T], pd.DataFrame],
     root_path: Union[str, Path],
     partition_cols: Optional[List[str]] = ["ticker"],
+    write_mode: Literal["w", "a"] = "w",
 ):
     """
     Apply the arguments to a function a save to a pyarrow dataset.
+    :param arguments: Each item in this sequence will be passed to f
+    :param f: Function that generates a pandas dataframe that will be called on arguments
+    :param root_path: folder in which to write the pyarrow dataset
+    :param partion_cols: what to name the files in the dataset
+    :param write_mode: "w" to start by deleting the dataset directory, "a" to add files.
 
     Usage::
 
     >>> %pip install calcbench-api-client[Pandas,Backoff,tqdm,pyarrow]
     >>> tickers = sorted(cb.tickers(entire_universe=True), key=lambda ticker: hash(ticker)) # randomize the order so the time estimate is better
     >>> iterate_and_save_pyarrow_dataset(
     >>>     arguments=tickers,
@@ -148,14 +156,17 @@
     >>> from pyarrow import csv
     >>> csv.write_csv(table, "C:/Users/andre/Downloads/entire_universe_standardized_PIT.csv")
 
     """
     import pyarrow as pa
     import pyarrow.parquet as pq
 
+    root_path = os.path.expanduser(root_path)
+    if write_mode == "w":
+        shutil.rmtree(root_path)
     for argument in tqdm(list(arguments)):
         try:
             df = f(argument)
             if df.empty:
                 continue
         except KeyboardInterrupt:
             raise
```

### Comparing `calcbench_api_client-9.1.1/calcbench/face_statements.py` & `calcbench_api_client-9.2.0/calcbench/face_statements.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/filing.py` & `calcbench_api_client-9.2.0/calcbench/filing.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/listener.py` & `calcbench_api_client-9.2.0/calcbench/listener.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/metrics.py` & `calcbench_api_client-9.2.0/calcbench/metrics.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/press_release.py` & `calcbench_api_client-9.2.0/calcbench/press_release.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/raw_numeric_XBRL.py` & `calcbench_api_client-9.2.0/calcbench/raw_numeric_XBRL.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/raw_numeric_non_XBRL.py` & `calcbench_api_client-9.2.0/calcbench/raw_numeric_non_XBRL.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/standardized_numeric.py` & `calcbench_api_client-9.2.0/calcbench/standardized_numeric.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench/standardized_parameters.py` & `calcbench_api_client-9.2.0/calcbench/standardized_parameters.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench_api_client.egg-info/PKG-INFO` & `calcbench_api_client-9.2.0/calcbench_api_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calcbench-api-client
-Version: 9.1.1
+Version: 9.2.0
 Summary: Client for Calcbench data.
 Home-page: https://github.com/calcbench/python_api_client
 Author: Andrew Kittredge
 Author-email: andrew@calcbench.com
 License: Apache2
 Project-URL: Documentation, http://calcbench.github.io/python_api_client/html/index.html
 Project-URL: Examples, https://github.com/calcbench/notebooks
@@ -46,13 +46,13 @@
         @someben https://github.com/calcbench/python_api_client/commit/6c2312525fa365acc91bd8e979037fc2492845f3
         
 Keywords: finance accounting SEC 10-(K|Q)
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: Listener
+Provides-Extra: Backoff
+Provides-Extra: BeautifulSoup
 Provides-Extra: Keyring
+Provides-Extra: pyarrow
 Provides-Extra: tqdm
 Provides-Extra: Pandas
-Provides-Extra: pyarrow
-Provides-Extra: BeautifulSoup
-Provides-Extra: Backoff
```

### Comparing `calcbench_api_client-9.1.1/calcbench_api_client.egg-info/SOURCES.txt` & `calcbench_api_client-9.2.0/calcbench_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl` & `calcbench_api_client-9.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz` & `calcbench_api_client-9.2.0/calcbench_api_client.egg-info/dist/calcbench_api_client-5.6.1.tar.gz`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/conda-recipe/meta.yaml` & `calcbench_api_client-9.2.0/conda-recipe/meta.yaml`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/Makefile` & `calcbench_api_client-9.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_sources/getting-started.rst.txt` & `calcbench_api_client-9.2.0/docs/html/_sources/getting-started.rst.txt`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/alabaster.css` & `calcbench_api_client-9.2.0/docs/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/basic.css` & `calcbench_api_client-9.2.0/docs/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/doctools.js` & `calcbench_api_client-9.2.0/docs/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/jquery-3.2.1.js` & `calcbench_api_client-9.2.0/docs/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/jquery-3.4.1.js` & `calcbench_api_client-9.2.0/docs/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/jquery-3.5.1.js` & `calcbench_api_client-9.2.0/docs/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/jquery.js` & `calcbench_api_client-9.2.0/docs/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/language_data.js` & `calcbench_api_client-9.2.0/docs/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/pygments.css` & `calcbench_api_client-9.2.0/docs/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/searchtools.js` & `calcbench_api_client-9.2.0/docs/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/underscore-1.13.1.js` & `calcbench_api_client-9.2.0/docs/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/underscore-1.3.1.js` & `calcbench_api_client-9.2.0/docs/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/_static/underscore.js` & `calcbench_api_client-9.2.0/docs/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/business-combinations.html` & `calcbench_api_client-9.2.0/docs/html/business-combinations.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/companies.html` & `calcbench_api_client-9.2.0/docs/html/companies.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/dimensional.html` & `calcbench_api_client-9.2.0/docs/html/dimensional.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/disclosures.html` & `calcbench_api_client-9.2.0/docs/html/disclosures.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/downloaders.html` & `calcbench_api_client-9.2.0/docs/html/downloaders.html`

 * *Files 5% similar despite different names*

```diff
@@ -62,16 +62,25 @@
 <span class="gp">&gt;&gt;&gt; </span><span class="p">)</span>
 </pre></div>
 </div>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="calcbench.downloaders.iterate_and_save_pyarrow_dataset">
-<span class="sig-prename descclassname"><span class="pre">calcbench.downloaders.</span></span><span class="sig-name descname"><span class="pre">iterate_and_save_pyarrow_dataset</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">f</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">root_path</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">partition_cols</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">['ticker']</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.downloaders.iterate_and_save_pyarrow_dataset" title="Permalink to this definition">¶</a></dt>
-<dd><p>Apply the arguments to a function a save to a pyarrow dataset.</p>
+<span class="sig-prename descclassname"><span class="pre">calcbench.downloaders.</span></span><span class="sig-name descname"><span class="pre">iterate_and_save_pyarrow_dataset</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">arguments</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">f</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">root_path</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">partition_cols</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">['ticker']</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">write_mode</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'w'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#calcbench.downloaders.iterate_and_save_pyarrow_dataset" title="Permalink to this definition">¶</a></dt>
+<dd><p>Apply the arguments to a function a save to a pyarrow dataset.
+:type arguments: <code class="xref py py-class docutils literal notranslate"><span class="pre">Sequence</span></code>[~T]
+:param arguments: Each item in this sequence will be passed to f
+:type f: <code class="xref py py-data docutils literal notranslate"><span class="pre">Callable</span></code>[[~T], <code class="xref py py-class docutils literal notranslate"><span class="pre">DataFrame</span></code>]
+:param f: Function that generates a pandas dataframe that will be called on arguments
+:type root_path: <code class="xref py py-data docutils literal notranslate"><span class="pre">Union</span></code>[<code class="xref py py-class docutils literal notranslate"><span class="pre">str</span></code>, <code class="xref py py-class docutils literal notranslate"><span class="pre">Path</span></code>]
+:param root_path: folder in which to write the pyarrow dataset
+:param partion_cols: what to name the files in the dataset
+:type write_mode: <code class="xref py py-data docutils literal notranslate"><span class="pre">Literal</span></code>[‘w’, ‘a’]
+:param write_mode: “w” to start by deleting the dataset directory, “a” to add files.</p>
 <p>Usage:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="gp">&gt;&gt;&gt; </span><span class="o">%</span><span class="n">pip</span> <span class="n">install</span> <span class="n">calcbench</span><span class="o">-</span><span class="n">api</span><span class="o">-</span><span class="n">client</span><span class="p">[</span><span class="n">Pandas</span><span class="p">,</span><span class="n">Backoff</span><span class="p">,</span><span class="n">tqdm</span><span class="p">,</span><span class="n">pyarrow</span><span class="p">]</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">tickers</span> <span class="o">=</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">cb</span><span class="o">.</span><span class="n">tickers</span><span class="p">(</span><span class="n">entire_universe</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span> <span class="n">key</span><span class="o">=</span><span class="k">lambda</span> <span class="n">ticker</span><span class="p">:</span> <span class="nb">hash</span><span class="p">(</span><span class="n">ticker</span><span class="p">))</span> <span class="c1"># randomize the order so the time estimate is better</span>
 <span class="gp">&gt;&gt;&gt; </span><span class="n">iterate_and_save_pyarrow_dataset</span><span class="p">(</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">arguments</span><span class="o">=</span><span class="n">tickers</span><span class="p">,</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">f</span><span class="o">=</span><span class="k">lambda</span> <span class="n">ticker</span><span class="p">:</span> <span class="n">cb</span><span class="o">.</span><span class="n">standardized</span><span class="p">(</span><span class="n">company_identifiers</span><span class="o">=</span><span class="p">[</span><span class="n">ticker</span><span class="p">],</span> <span class="n">point_in_time</span><span class="o">=</span><span class="kc">True</span><span class="p">),</span>
 <span class="gp">&gt;&gt;&gt; </span>    <span class="n">root_path</span><span class="o">=</span><span class="s2">&quot;~/standardized_PIT_arrow/&quot;</span><span class="p">,</span>
```

#### html2text {}

```diff
@@ -24,16 +24,23 @@
       >>> iterate_and_save_pandas(
       >>>    arguments=tickers,
       >>>    f=lambda ticker: cb.standardized(company_identifiers=[ticker],
       point_in_time=True),
       >>>    file_name="calcbench_standardized_PIT.csv",
       >>> )
   calcbench.downloaders.iterate_and_save_pyarrow_dataset(aarrgguummeennttss, ff,
-  rroooott__ppaatthh, ppaarrttiittiioonn__ccoollss==[[''ttiicckkeerr'']])_¶
-      Apply the arguments to a function a save to a pyarrow dataset.
+  rroooott__ppaatthh, ppaarrttiittiioonn__ccoollss==[[''ttiicckkeerr'']], wwrriittee__mmooddee==''ww'')_¶
+      Apply the arguments to a function a save to a pyarrow dataset. :type
+      arguments: Sequence[~T] :param arguments: Each item in this sequence will
+      be passed to f :type f: Callable[[~T], DataFrame] :param f: Function that
+      generates a pandas dataframe that will be called on arguments :type
+      root_path: Union[str, Path] :param root_path: folder in which to write
+      the pyarrow dataset :param partion_cols: what to name the files in the
+      dataset :type write_mode: Literal[‘w’, ‘a’] :param write_mode: “w” to
+      start by deleting the dataset directory, “a” to add files.
       Usage:
       >>> %pip install calcbench-api-client[Pandas,Backoff,tqdm,pyarrow]
       >>> tickers = sorted(cb.tickers(entire_universe=True), key=lambda ticker:
       hash(ticker)) # randomize the order so the time estimate is better
       >>> iterate_and_save_pyarrow_dataset(
       >>>     arguments=tickers,
       >>>     f=lambda ticker: cb.standardized(company_identifiers=[ticker],
```

### Comparing `calcbench_api_client-9.1.1/docs/html/face-statements.html` & `calcbench_api_client-9.2.0/docs/html/face-statements.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/filings.html` & `calcbench_api_client-9.2.0/docs/html/filings.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/genindex.html` & `calcbench_api_client-9.2.0/docs/html/genindex.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/getting-started.html` & `calcbench_api_client-9.2.0/docs/html/getting-started.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/index.html` & `calcbench_api_client-9.2.0/docs/html/index.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/metrics.html` & `calcbench_api_client-9.2.0/docs/html/metrics.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/numeric-data.html` & `calcbench_api_client-9.2.0/docs/html/numeric-data.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/press-release.html` & `calcbench_api_client-9.2.0/docs/html/press-release.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/push-notification.html` & `calcbench_api_client-9.2.0/docs/html/push-notification.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/py-modindex.html` & `calcbench_api_client-9.2.0/docs/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/raw-numeric-XBRL.html` & `calcbench_api_client-9.2.0/docs/html/raw-numeric-XBRL.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/raw-numeric-non-XBRL.html` & `calcbench_api_client-9.2.0/docs/html/raw-numeric-non-XBRL.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/search.html` & `calcbench_api_client-9.2.0/docs/html/search.html`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/html/searchindex.js` & `calcbench_api_client-9.2.0/docs/html/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -850,15 +850,15 @@
         accountingpolici: 2,
         accountsreceiv: 8,
         acquiredfinitelivedintangibleassetsweightedaverageusefullif: 1,
         acquisit: 0,
         acquisition_d: 0,
         across: 11,
         activ: 2,
-        add: 10,
+        add: [3, 10],
         add_handl: [],
         addit: 2,
         additionalsect: 2,
         address: 6,
         advanc: 6,
         after: [2, 5, 8],
         again: 5,
@@ -1143,14 +1143,15 @@
         definedbenefitplantransf: 1,
         definit: 8,
         defm14a: 5,
         defm14c: 5,
         defn14a: 5,
         defr14a: 5,
         defr14c: 5,
+        delet: 3,
         denot: 1,
         depend: 10,
         deprec: [],
         deriv: 2,
         derivativeassetnotionalamount: 1,
         derivativefairvalueofderivativeasset: 1,
         derivativefairvalueofderivativeli: 1,
@@ -1164,14 +1165,15 @@
         dictionari: [],
         differ: 8,
         dimens: 1,
         dimension: 7,
         dimension_memb: 4,
         dimensional_raw: 1,
         dimensionaldatapoint: 1,
+        directori: 3,
         disclosur: [7, 11],
         disclosure_datafram: 2,
         disclosure_list: 2,
         disclosure_nam: 2,
         disclosure_search: 2,
         disclosure_typ: 2,
         disclosure_type_nam: 2,
@@ -1333,14 +1335,15 @@
         fiscal_year_end_d: 9,
         fiscalyear: 11,
         fling_accession_numb: 8,
         flow: [],
         focu: 4,
         focus_neg: 4,
         focusn: 5,
+        folder: 3,
         footnot: [2, 8],
         footnote_fact_id: 4,
         footnote_typ: 2,
         footnote_type_titl: 2,
         footnotetypetitl: 2,
         foramt_typ: [],
         form_3: 5,
@@ -1607,26 +1610,27 @@
         overwrit: 3,
         p: 5,
         packag: [6, 10],
         page: [1, 4, 5, 8],
         page_url: 2,
         panda: 3,
         paper: 5,
-        param: [],
+        param: 3,
         paramet: [0, 1, 2, 3, 4, 5, 6, 8, 10, 11],
         parent_compani: 0,
         parent_company_sic_cod: 0,
         parent_company_st: 0,
         parent_company_tick: 0,
         parquet: 3,
         pars: [2, 8],
         parse_d: [],
         parse_filing_d: 4,
         particular: 11,
         particularli: 8,
+        partion_col: 3,
         partition_col: 3,
         pass: [1, 2, 3, 8, 11],
         password: 6,
         path: 3,
         paymentstoacquirebusinessesgross: 1,
         paymentstoacquirebusinessesnetofcashacquir: 1,
         pc: 3,
@@ -1848,15 +1852,15 @@
         standardized_pit_arrow: 3,
         standardized_ppa_point: 0,
         standardized_raw: 8,
         standardized_xbrl: [5, 10],
         standardizedmetr: 8,
         standardizedpoint: [0, 8],
         stardiz: 8,
-        start: 7,
+        start: [3, 7],
         start_dat: [5, 8],
         start_period: [1, 8],
         start_year: [1, 8],
         state: 11,
         statement: [7, 11],
         statement_typ: [4, 9, 11],
         statementofcomprehensiveincom: [4, 11],
@@ -1960,15 +1964,15 @@
         w: 3,
         wa: [2, 4, 8, 11],
         wai: [],
         warn: [],
         we: [5, 10],
         week: [6, 8],
         went: 8,
-        what: 8,
+        what: [3, 8],
         when: [1, 2, 8, 10, 11],
         where: 8,
         whether: 6,
         which: [0, 3, 5, 8, 11],
         window: [6, 10],
         wire: [5, 8, 10],
         wirepr: 5,
```

### Comparing `calcbench_api_client-9.1.1/docs/make.bat` & `calcbench_api_client-9.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/source/conf.py` & `calcbench_api_client-9.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/source/getting-started.rst` & `calcbench_api_client-9.2.0/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/source/index.rst` & `calcbench_api_client-9.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/source/numeric-data.rst` & `calcbench_api_client-9.2.0/docs/source/numeric-data.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/docs/source/push-notification.rst` & `calcbench_api_client-9.2.0/docs/source/push-notification.rst`

 * *Files identical despite different names*

### Comparing `calcbench_api_client-9.1.1/setup.py` & `calcbench_api_client-9.2.0/setup.py`

 * *Files identical despite different names*

