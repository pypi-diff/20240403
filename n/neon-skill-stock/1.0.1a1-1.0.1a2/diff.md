# Comparing `tmp/neon-skill-stock-1.0.1a1.tar.gz` & `tmp/neon-skill-stock-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-stock-1.0.1a1.tar", last modified: Mon Feb  5 23:19:21 2024, max compression
+gzip compressed data, was "neon-skill-stock-1.0.1a2.tar", last modified: Tue Apr  2 22:10:43 2024, max compression
```

## Comparing `neon-skill-stock-1.0.1a1.tar` & `neon-skill-stock-1.0.1a2.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11558 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.143888 neon-skill-stock-1.0.1a1/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/ca-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/ca-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/ca-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.143888 neon-skill-stock-1.0.1a1/locale/ca-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/ca-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.143888 neon-skill-stock-1.0.1a1/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/de-de/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/de-de/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/de-de/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.143888 neon-skill-stock-1.0.1a1/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/de-de/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/el-gr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.143888 neon-skill-stock-1.0.1a1/locale/el-gr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/el-gr/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/el-gr/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.143888 neon-skill-stock-1.0.1a1/locale/el-gr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/el-gr/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.143888 neon-skill-stock-1.0.1a1/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/en-us/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/en-us/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/en-us/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.143888 neon-skill-stock-1.0.1a1/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/en-us/intent/stock_price.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/es-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/es-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/es-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/es-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/es-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/es-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/fr-fr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/fr-fr/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/fr-fr/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/fr-fr/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/fr-fr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/fr-fr/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/gl-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/gl-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/gl-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/gl-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/gl-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/hu-hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/hu-hu/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/hu-hu/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/hu-hu/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/hu-hu/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/hu-hu/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/it-it/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/it-it/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/it-it/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/it-it/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/it-it/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/it-it/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/nl-nl/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/nl-nl/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/nl-nl/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/nl-nl/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/nl-nl/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/nl-nl/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/pt-br/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/pt-br/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/pt-br/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/pt-br/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/pt-br/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.147888 neon-skill-stock-1.0.1a1/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/ru-ru/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/ru-ru/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/locale/ru-ru/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/ru-ru/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.139888 neon-skill-stock-1.0.1a1/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/sv-se/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/sv-se/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/sv-se/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/locale/sv-se/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/locale/sv-se/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-02-05 23:19:21.000000 neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-02-05 23:19:21.000000 neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 23:19:21.000000 neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-05 23:19:21.000000 neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-05 23:19:21.000000 neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-05 23:19:21.000000 neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 23:19:21.151888 neon-skill-stock-1.0.1a1/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/ui/Stock.qml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-05 23:19:17.000000 neon-skill-stock-1.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11558 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ca-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ca-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ca-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/ca-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ca-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/de-de/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/de-de/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/de-de/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/de-de/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/el-gr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/el-gr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/el-gr/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/el-gr/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/el-gr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/el-gr/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/en-us/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/en-us/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/en-us/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/en-us/intent/stock_price.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/es-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/es-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/es-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/es-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/es-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/es-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/fr-fr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/fr-fr/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/fr-fr/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/fr-fr/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/fr-fr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/fr-fr/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.134620 neon-skill-stock-1.0.1a2/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/gl-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/gl-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/gl-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/gl-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/gl-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/hu-hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/hu-hu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/hu-hu/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/hu-hu/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/hu-hu/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/hu-hu/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/it-it/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/it-it/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/it-it/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/it-it/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/it-it/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/it-it/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.142620 neon-skill-stock-1.0.1a2/locale/nl-nl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/nl-nl/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/nl-nl/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/nl-nl/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/nl-nl/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/nl-nl/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/pt-br/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/pt-br/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/pt-br/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/pt-br/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/pt-br/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ru-ru/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ru-ru/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/ru-ru/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/ru-ru/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.138620 neon-skill-stock-1.0.1a2/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/sv-se/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/sv-se/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/sv-se/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/locale/sv-se/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/locale/sv-se/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 22:10:43.000000 neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:10:43.146620 neon-skill-stock-1.0.1a2/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/ui/Stock.qml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 22:10:39.000000 neon-skill-stock-1.0.1a2/version.py
```

### Comparing `neon-skill-stock-1.0.1a1/LICENSE` & `neon-skill-stock-1.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/LICENSE.md` & `neon-skill-stock-1.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/PKG-INFO` & `neon-skill-stock-1.0.1a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-stock
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-stock
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-stock-1.0.1a1/README.md` & `neon-skill-stock-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/__init__.py` & `neon-skill-stock-1.0.1a2/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/PKG-INFO` & `neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-stock
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-stock
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-stock-1.0.1a1/neon_skill_stock.egg-info/SOURCES.txt` & `neon-skill-stock-1.0.1a2/neon_skill_stock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/setup.py` & `neon-skill-stock-1.0.1a2/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/skill.json` & `neon-skill-stock-1.0.1a2/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/test/test_skill.py` & `neon-skill-stock-1.0.1a2/test/test_skill.py`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/ui/Stock.qml` & `neon-skill-stock-1.0.1a2/ui/Stock.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a1/version.py` & `neon-skill-stock-1.0.1a2/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a1"
+__version__ = "1.0.1a2"
```

