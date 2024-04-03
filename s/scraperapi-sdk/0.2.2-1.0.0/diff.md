# Comparing `tmp/scraperapi_sdk-0.2.2.tar.gz` & `tmp/scraperapi_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scraperapi_sdk-0.2.2.tar", last modified: Sat Feb  8 00:11:04 2020, max compression
+gzip compressed data, was "scraperapi_sdk-1.0.0.tar", max compression
```

## Comparing `scraperapi_sdk-0.2.2.tar` & `scraperapi_sdk-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,7 @@
-drwxr-xr-x   0 aidancunniffe   (501) staff       (20)        0 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/
--rw-r--r--   0 aidancunniffe   (501) staff       (20)      486 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/PKG-INFO
--rw-r--r--   0 aidancunniffe   (501) staff       (20)      141 2020-02-08 00:10:51.000000 scraperapi_sdk-0.2.2/README.md
-drwxr-xr-x   0 aidancunniffe   (501) staff       (20)        0 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/scraper_api/
--rw-r--r--   0 aidancunniffe   (501) staff       (20)     4508 2020-02-08 00:05:54.000000 scraperapi_sdk-0.2.2/scraper_api/__init__.py
-drwxr-xr-x   0 aidancunniffe   (501) staff       (20)        0 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/scraperapi_sdk.egg-info/
--rw-r--r--   0 aidancunniffe   (501) staff       (20)      486 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/scraperapi_sdk.egg-info/PKG-INFO
--rw-r--r--   0 aidancunniffe   (501) staff       (20)      194 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/scraperapi_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 aidancunniffe   (501) staff       (20)        1 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/scraperapi_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 aidancunniffe   (501) staff       (20)       12 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/scraperapi_sdk.egg-info/top_level.txt
--rw-r--r--   0 aidancunniffe   (501) staff       (20)       38 2020-02-08 00:11:04.000000 scraperapi_sdk-0.2.2/setup.cfg
--rw-r--r--   0 aidancunniffe   (501) staff       (20)      506 2020-02-08 00:10:58.000000 scraperapi_sdk-0.2.2/setup.py
+-rw-r--r--   0        0        0     1572 2024-04-03 07:49:15.926495 scraperapi_sdk-1.0.0/README.md
+-rw-r--r--   0        0        0      713 2024-04-03 07:46:42.401487 scraperapi_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       46 2023-12-20 08:41:35.662682 scraperapi_sdk-1.0.0/scraperapi_sdk/__init__.py
+-rw-r--r--   0        0        0       46 2023-12-20 08:42:19.108130 scraperapi_sdk-1.0.0/scraperapi_sdk/__version__.py
+-rw-r--r--   0        0        0     2632 2024-04-03 07:46:57.405216 scraperapi_sdk-1.0.0/scraperapi_sdk/_client.py
+-rw-r--r--   0        0        0      231 2024-04-02 05:51:09.376205 scraperapi_sdk-1.0.0/scraperapi_sdk/exceptions.py
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 scraperapi_sdk-1.0.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

