# Comparing `tmp/wbtools-3.0.5.tar.gz` & `tmp/wbtools-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wbtools-3.0.5.tar", last modified: Tue Apr  2 22:17:44 2024, max compression
+gzip compressed data, was "wbtools-3.0.6.tar", last modified: Tue Apr  2 22:21:24 2024, max compression
```

## Comparing `wbtools-3.0.5.tar` & `wbtools-3.0.6.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1060 2021-09-21 20:01:07.000000 wbtools-3.0.5/LICENSE
--rw-r--r--   0 valerio   (1000) valerio   (1000)     3217 2024-04-02 22:17:44.388291 wbtools-3.0.5/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2306 2022-03-11 05:13:49.000000 wbtools-3.0.5/README.md
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       38 2024-04-02 22:17:44.388291 wbtools-3.0.5/setup.cfg
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1121 2024-04-02 22:16:33.000000 wbtools-3.0.5/setup.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.384291 wbtools-3.0.5/tests/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      640 2023-10-12 19:51:59.000000 wbtools-3.0.5/tests/config_reader.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.384291 wbtools-3.0.5/tests/db/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/db/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1050 2021-10-13 16:58:22.000000 wbtools-3.0.5/tests/db/test_afp.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1061 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/db/test_antibody.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1025 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/db/test_expression.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1915 2022-03-11 05:13:49.000000 wbtools-3.0.5/tests/db/test_generic.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.384291 wbtools-3.0.5/tests/lib/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/lib/__init__.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.384291 wbtools-3.0.5/tests/lib/entity_extraction/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/lib/entity_extraction/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1705 2023-10-12 19:51:59.000000 wbtools-3.0.5/tests/lib/entity_extraction/test_email_addresses.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2342 2021-10-01 23:54:11.000000 wbtools-3.0.5/tests/lib/entity_extraction/test_generic.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2455 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/lib/entity_extraction/test_new_variations.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1178 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/lib/test_literature_index.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      510 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/lib/test_scraping.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2937 2023-10-12 19:51:59.000000 wbtools-3.0.5/tests/lib/test_text_preprocessing.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2937 2023-10-12 19:51:59.000000 wbtools-3.0.5/tests/lib/test_text_similarity.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.384291 wbtools-3.0.5/tests/literature/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/tests/literature/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     4721 2023-10-12 19:51:59.000000 wbtools-3.0.5/tests/literature/test_corpus.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     6282 2024-03-14 16:19:03.000000 wbtools-3.0.5/tests/literature/test_paper.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.384291 wbtools-3.0.5/wbtools/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/__init__.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools/db/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/db/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3317 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/db/abstract_manager.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    74412 2023-09-14 17:39:53.000000 wbtools-3.0.5/wbtools/db/afp.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1526 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/db/antibody.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1877 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/db/dbmanager.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      528 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/db/expression.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2399 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/db/gene.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    15760 2023-10-14 22:13:43.000000 wbtools-3.0.5/wbtools/db/generic.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     7517 2023-10-16 00:48:06.000000 wbtools-3.0.5/wbtools/db/paper.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     5930 2022-01-24 21:54:08.000000 wbtools-3.0.5/wbtools/db/person.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools/lib/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/__init__.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools/lib/email/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/email/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1203 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/email/generic.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools/lib/nlp/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/nlp/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1881 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/nlp/common.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools/lib/nlp/entity_extraction/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/nlp/entity_extraction/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      684 2022-03-08 18:09:18.000000 wbtools-3.0.5/wbtools/lib/nlp/entity_extraction/email_addresses.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     9003 2021-10-01 16:15:02.000000 wbtools-3.0.5/wbtools/lib/nlp/entity_extraction/ntt_extractor.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      764 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/nlp/entity_extraction/variations.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools/lib/nlp/literature_index/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/nlp/literature_index/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      310 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/nlp/literature_index/abstract_index.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     2624 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/nlp/literature_index/textpresso.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     3600 2024-03-26 21:21:13.000000 wbtools-3.0.5/wbtools/lib/nlp/text_preprocessing.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1652 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/nlp/text_similarity.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     4183 2023-10-05 19:25:41.000000 wbtools-3.0.5/wbtools/lib/scraping.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      581 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/lib/timeout.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools/literature/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/literature/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    13655 2024-03-26 21:21:13.000000 wbtools-3.0.5/wbtools/literature/corpus.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)    17709 2024-04-02 22:16:12.000000 wbtools-3.0.5/wbtools/literature/paper.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1941 2021-09-21 20:01:07.000000 wbtools-3.0.5/wbtools/literature/person.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools/utils/
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2023-10-12 19:51:59.000000 wbtools-3.0.5/wbtools/utils/__init__.py
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1912 2023-10-12 19:51:59.000000 wbtools-3.0.5/wbtools/utils/okta_utils.py
-drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:17:44.388291 wbtools-3.0.5/wbtools.egg-info/
--rw-r--r--   0 valerio   (1000) valerio   (1000)     3217 2024-04-02 22:17:44.000000 wbtools-3.0.5/wbtools.egg-info/PKG-INFO
--rw-rw-r--   0 valerio   (1000) valerio   (1000)     1791 2024-04-02 22:17:44.000000 wbtools-3.0.5/wbtools.egg-info/SOURCES.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)        1 2024-04-02 22:17:44.000000 wbtools-3.0.5/wbtools.egg-info/dependency_links.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)      209 2024-04-02 22:17:44.000000 wbtools-3.0.5/wbtools.egg-info/requires.txt
--rw-rw-r--   0 valerio   (1000) valerio   (1000)       14 2024-04-02 22:17:44.000000 wbtools-3.0.5/wbtools.egg-info/top_level.txt
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1060 2021-09-21 20:01:07.000000 wbtools-3.0.6/LICENSE
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3217 2024-04-02 22:21:24.528360 wbtools-3.0.6/PKG-INFO
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2306 2022-03-11 05:13:49.000000 wbtools-3.0.6/README.md
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)       38 2024-04-02 22:21:24.528360 wbtools-3.0.6/setup.cfg
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1121 2024-04-02 22:20:25.000000 wbtools-3.0.6/setup.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.524360 wbtools-3.0.6/tests/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      640 2023-10-12 19:51:59.000000 wbtools-3.0.6/tests/config_reader.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.524360 wbtools-3.0.6/tests/db/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/db/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1050 2021-10-13 16:58:22.000000 wbtools-3.0.6/tests/db/test_afp.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1061 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/db/test_antibody.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1025 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/db/test_expression.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1915 2022-03-11 05:13:49.000000 wbtools-3.0.6/tests/db/test_generic.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.524360 wbtools-3.0.6/tests/lib/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/lib/__init__.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.524360 wbtools-3.0.6/tests/lib/entity_extraction/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/lib/entity_extraction/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1705 2023-10-12 19:51:59.000000 wbtools-3.0.6/tests/lib/entity_extraction/test_email_addresses.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2342 2021-10-01 23:54:11.000000 wbtools-3.0.6/tests/lib/entity_extraction/test_generic.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2455 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/lib/entity_extraction/test_new_variations.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1178 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/lib/test_literature_index.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      510 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/lib/test_scraping.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2937 2023-10-12 19:51:59.000000 wbtools-3.0.6/tests/lib/test_text_preprocessing.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2937 2023-10-12 19:51:59.000000 wbtools-3.0.6/tests/lib/test_text_similarity.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.524360 wbtools-3.0.6/tests/literature/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/tests/literature/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     4721 2023-10-12 19:51:59.000000 wbtools-3.0.6/tests/literature/test_corpus.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     6282 2024-03-14 16:19:03.000000 wbtools-3.0.6/tests/literature/test_paper.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.524360 wbtools-3.0.6/wbtools/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/__init__.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools/db/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/db/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     3317 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/db/abstract_manager.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)    74412 2023-09-14 17:39:53.000000 wbtools-3.0.6/wbtools/db/afp.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1526 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/db/antibody.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1877 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/db/dbmanager.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      528 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/db/expression.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2399 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/db/gene.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)    15760 2023-10-14 22:13:43.000000 wbtools-3.0.6/wbtools/db/generic.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     7517 2023-10-16 00:48:06.000000 wbtools-3.0.6/wbtools/db/paper.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     5930 2022-01-24 21:54:08.000000 wbtools-3.0.6/wbtools/db/person.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools/lib/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/__init__.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools/lib/email/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/email/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1203 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/email/generic.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools/lib/nlp/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/nlp/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1881 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/nlp/common.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools/lib/nlp/entity_extraction/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/nlp/entity_extraction/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      684 2022-03-08 18:09:18.000000 wbtools-3.0.6/wbtools/lib/nlp/entity_extraction/email_addresses.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     9003 2021-10-01 16:15:02.000000 wbtools-3.0.6/wbtools/lib/nlp/entity_extraction/ntt_extractor.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      764 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/nlp/entity_extraction/variations.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools/lib/nlp/literature_index/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/nlp/literature_index/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      310 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/nlp/literature_index/abstract_index.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     2624 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/nlp/literature_index/textpresso.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     3600 2024-03-26 21:21:13.000000 wbtools-3.0.6/wbtools/lib/nlp/text_preprocessing.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1652 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/nlp/text_similarity.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     4183 2023-10-05 19:25:41.000000 wbtools-3.0.6/wbtools/lib/scraping.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      581 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/lib/timeout.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools/literature/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/literature/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)    13655 2024-03-26 21:21:13.000000 wbtools-3.0.6/wbtools/literature/corpus.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)    17699 2024-04-02 22:20:25.000000 wbtools-3.0.6/wbtools/literature/paper.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1941 2021-09-21 20:01:07.000000 wbtools-3.0.6/wbtools/literature/person.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools/utils/
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        0 2023-10-12 19:51:59.000000 wbtools-3.0.6/wbtools/utils/__init__.py
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1912 2023-10-12 19:51:59.000000 wbtools-3.0.6/wbtools/utils/okta_utils.py
+drwxrwxr-x   0 valerio   (1000) valerio   (1000)        0 2024-04-02 22:21:24.528360 wbtools-3.0.6/wbtools.egg-info/
+-rw-r--r--   0 valerio   (1000) valerio   (1000)     3217 2024-04-02 22:21:24.000000 wbtools-3.0.6/wbtools.egg-info/PKG-INFO
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)     1791 2024-04-02 22:21:24.000000 wbtools-3.0.6/wbtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)        1 2024-04-02 22:21:24.000000 wbtools-3.0.6/wbtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)      209 2024-04-02 22:21:24.000000 wbtools-3.0.6/wbtools.egg-info/requires.txt
+-rw-rw-r--   0 valerio   (1000) valerio   (1000)       14 2024-04-02 22:21:24.000000 wbtools-3.0.6/wbtools.egg-info/top_level.txt
```

### Comparing `wbtools-3.0.5/LICENSE` & `wbtools-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/PKG-INFO` & `wbtools-3.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbtools
-Version: 3.0.5
+Version: 3.0.6
 Summary: Interface to WormBase (www.wormbase.org) curation data, including literature management and NLP functions
 Home-page: https://github.com/WormBase/wbtools
 Author: Valerio Arnaboldi
 Author-email: valearna@caltech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wbtools-3.0.5/README.md` & `wbtools-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/setup.py` & `wbtools-3.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="wbtools",
-    version="3.0.5",
+    version="3.0.6",
     author="Valerio Arnaboldi",
     author_email="valearna@caltech.edu",
     description="Interface to WormBase (www.wormbase.org) curation data, including literature management and NLP "
                 "functions",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/WormBase/wbtools",
```

### Comparing `wbtools-3.0.5/tests/config_reader.py` & `wbtools-3.0.6/tests/config_reader.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/db/test_afp.py` & `wbtools-3.0.6/tests/db/test_afp.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/db/test_antibody.py` & `wbtools-3.0.6/tests/db/test_antibody.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/db/test_expression.py` & `wbtools-3.0.6/tests/db/test_expression.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/db/test_generic.py` & `wbtools-3.0.6/tests/db/test_generic.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/lib/entity_extraction/test_email_addresses.py` & `wbtools-3.0.6/tests/lib/entity_extraction/test_email_addresses.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/lib/entity_extraction/test_generic.py` & `wbtools-3.0.6/tests/lib/entity_extraction/test_generic.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/lib/entity_extraction/test_new_variations.py` & `wbtools-3.0.6/tests/lib/entity_extraction/test_new_variations.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/lib/test_literature_index.py` & `wbtools-3.0.6/tests/lib/test_literature_index.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/lib/test_text_preprocessing.py` & `wbtools-3.0.6/tests/lib/test_text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/lib/test_text_similarity.py` & `wbtools-3.0.6/tests/lib/test_text_similarity.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/literature/test_corpus.py` & `wbtools-3.0.6/tests/literature/test_corpus.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/tests/literature/test_paper.py` & `wbtools-3.0.6/tests/literature/test_paper.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/abstract_manager.py` & `wbtools-3.0.6/wbtools/db/abstract_manager.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/afp.py` & `wbtools-3.0.6/wbtools/db/afp.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/antibody.py` & `wbtools-3.0.6/wbtools/db/antibody.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/dbmanager.py` & `wbtools-3.0.6/wbtools/db/dbmanager.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/expression.py` & `wbtools-3.0.6/wbtools/db/expression.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/gene.py` & `wbtools-3.0.6/wbtools/db/gene.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/generic.py` & `wbtools-3.0.6/wbtools/db/generic.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/paper.py` & `wbtools-3.0.6/wbtools/db/paper.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/db/person.py` & `wbtools-3.0.6/wbtools/db/person.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/email/generic.py` & `wbtools-3.0.6/wbtools/lib/email/generic.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/nlp/common.py` & `wbtools-3.0.6/wbtools/lib/nlp/common.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/nlp/entity_extraction/email_addresses.py` & `wbtools-3.0.6/wbtools/lib/nlp/entity_extraction/email_addresses.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/nlp/entity_extraction/ntt_extractor.py` & `wbtools-3.0.6/wbtools/lib/nlp/entity_extraction/ntt_extractor.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/nlp/entity_extraction/variations.py` & `wbtools-3.0.6/wbtools/lib/nlp/entity_extraction/variations.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/nlp/literature_index/textpresso.py` & `wbtools-3.0.6/wbtools/lib/nlp/literature_index/textpresso.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/nlp/text_preprocessing.py` & `wbtools-3.0.6/wbtools/lib/nlp/text_preprocessing.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/nlp/text_similarity.py` & `wbtools-3.0.6/wbtools/lib/nlp/text_similarity.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/scraping.py` & `wbtools-3.0.6/wbtools/lib/scraping.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/lib/timeout.py` & `wbtools-3.0.6/wbtools/lib/timeout.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/literature/corpus.py` & `wbtools-3.0.6/wbtools/literature/corpus.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/literature/paper.py` & `wbtools-3.0.6/wbtools/literature/paper.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                     if (len(section.paragraphs) == 3 and section.paragraphs[0][0].text in ['\n', ' ']
                             and section.paragraphs[-1][0].text in ['\n', ' ']):
                         continue
                     # add section titles as sentences
                     if section.name:
                         sentences.append(section.name)
                     for paragraph in section.paragraphs:
-                        for sentence in paragraph.sentences:
+                        for sentence in paragraph:
                             sentences.append(re.sub('<[^<]+>', '', sentence.text))
             else:
                 return []
     except:
         return []
```

### Comparing `wbtools-3.0.5/wbtools/literature/person.py` & `wbtools-3.0.6/wbtools/literature/person.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools/utils/okta_utils.py` & `wbtools-3.0.6/wbtools/utils/okta_utils.py`

 * *Files identical despite different names*

### Comparing `wbtools-3.0.5/wbtools.egg-info/PKG-INFO` & `wbtools-3.0.6/wbtools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wbtools
-Version: 3.0.5
+Version: 3.0.6
 Summary: Interface to WormBase (www.wormbase.org) curation data, including literature management and NLP functions
 Home-page: https://github.com/WormBase/wbtools
 Author: Valerio Arnaboldi
 Author-email: valearna@caltech.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wbtools-3.0.5/wbtools.egg-info/SOURCES.txt` & `wbtools-3.0.6/wbtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

