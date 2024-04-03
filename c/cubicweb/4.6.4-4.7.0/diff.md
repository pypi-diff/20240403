# Comparing `tmp/cubicweb-4.6.4.tar.gz` & `tmp/cubicweb-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-4.6.4.tar", last modified: Wed Mar 13 14:14:30 2024, max compression
+gzip compressed data, was "cubicweb-4.7.0.tar", last modified: Wed Apr  3 11:58:52 2024, max compression
```

## Comparing `cubicweb-4.6.4.tar` & `cubicweb-4.7.0.tar`

### file list

```diff
@@ -1,1319 +1,1370 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.769694 cubicweb-4.6.4/
--rw-rw-rw-   0 root         (0) root         (0)     2002 2024-03-13 14:13:59.000000 cubicweb-4.6.4/CONTRIBUTING.rst
--rw-rw-rw-   0 root         (0) root         (0)    17987 2024-03-13 14:13:59.000000 cubicweb-4.6.4/COPYING
--rw-rw-rw-   0 root         (0) root         (0)    26527 2024-03-13 14:13:59.000000 cubicweb-4.6.4/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)     4977 2024-03-13 14:13:59.000000 cubicweb-4.6.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5135 2024-03-13 14:14:30.769694 cubicweb-4.6.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.177682 cubicweb-4.6.4/cubicweb/
--rw-rw-rw-   0 root         (0) root         (0)     7503 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       69 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     6885 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3860 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/_gcdebug.py
--rw-rw-rw-   0 root         (0) root         (0)     5211 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/appobject.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)    66337 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/cwconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    32638 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/cwctl.py
--rw-rw-rw-   0 root         (0) root         (0)     4899 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/cwgettext.py
--rw-rw-rw-   0 root         (0) root         (0)    25982 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/cwvreg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.185682 cubicweb-4.6.4/cubicweb/dataimport/
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3274 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    21081 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/importer.py
--rw-rw-rw-   0 root         (0) root         (0)    26515 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/massive_store.py
--rw-rw-rw-   0 root         (0) root         (0)    15503 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/pgstore.py
--rw-rw-rw-   0 root         (0) root         (0)    18127 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/stores.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.185682 cubicweb-4.6.4/cubicweb/dataimport/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.189682 cubicweb-4.6.4/cubicweb/dataimport/test/data/
--rw-rw-rw-   0 root         (0) root         (0)   474710 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/data/geonames.csv
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/data/people.csv
--rw-rw-rw-   0 root         (0) root         (0)     1231 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12362 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/data/timeZones.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.189682 cubicweb-4.6.4/cubicweb/dataimport/test/data-massimport/
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/data-massimport/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/test_csv.py
--rw-rw-rw-   0 root         (0) root         (0)    16176 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/test_massive_store.py
--rw-rw-rw-   0 root         (0) root         (0)     4179 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/test_pgstore.py
--rw-rw-rw-   0 root         (0) root         (0)     8221 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/test_stores.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/dataimport/test/unittest_importer.py
--rw-rw-rw-   0 root         (0) root         (0)     2669 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.197682 cubicweb-4.6.4/cubicweb/devtools/
--rw-rw-rw-   0 root         (0) root         (0)    27112 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5449 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/apptest_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.201682 cubicweb-4.6.4/cubicweb/devtools/data/
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/data/cwmock.js
--rw-rw-rw-   0 root         (0) root         (0)     5146 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/data/qunit.css
--rw-rw-rw-   0 root         (0) root         (0)   115758 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/data/qunit.js
--rw-rw-rw-   0 root         (0) root         (0)    39808 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/devctl.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/fake.py
--rw-rw-rw-   0 root         (0) root         (0)    24531 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/fill.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/fix_po_encoding
--rw-rw-rw-   0 root         (0) root         (0)    10982 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/htmlparser.py
--rw-rw-rw-   0 root         (0) root         (0)     5298 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/httptest.py
--rw-rw-rw-   0 root         (0) root         (0)     9195 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/realdbtest.py
--rw-rw-rw-   0 root         (0) root         (0)    10873 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/repotest.py
--rw-rw-rw-   0 root         (0) root         (0)     6796 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/stresstester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.201682 cubicweb-4.6.4/cubicweb/devtools/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.205682 cubicweb-4.6.4/cubicweb/devtools/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)    11311 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/firstnames.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.085680 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.205682 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      460 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.205682 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.205682 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.209682 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
--rw-rw-rw-   0 root         (0) root         (0)     1720 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.085680 cubicweb-4.6.4/cubicweb/devtools/test/data/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.209682 cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/dep_1.js
--rw-rw-rw-   0 root         (0) root         (0)       10 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/deps_2.js
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
--rw-rw-rw-   0 root         (0) root         (0)      321 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4354 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/unittest_dbfill.py
--rw-rw-rw-   0 root         (0) root         (0)     6402 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/unittest_devctl.py
--rw-rw-rw-   0 root         (0) root         (0)     2475 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/unittest_fill.py
--rw-rw-rw-   0 root         (0) root         (0)     3225 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/unittest_i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     4687 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/test/unittest_testlib.py
--rw-rw-rw-   0 root         (0) root         (0)    20848 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/devtools/testlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.213682 cubicweb-4.6.4/cubicweb/entities/
--rw-rw-rw-   0 root         (0) root         (0)     5324 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24563 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)     6476 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/authobjs.py
--rw-rw-rw-   0 root         (0) root         (0)     4193 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     5944 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/schemaobjs.py
--rw-rw-rw-   0 root         (0) root         (0)     4095 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.217682 cubicweb-4.6.4/cubicweb/entities/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.217682 cubicweb-4.6.4/cubicweb/entities/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.217682 cubicweb-4.6.4/cubicweb/entities/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/test/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     1307 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9992 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/test/unittest_base.py
--rw-rw-rw-   0 root         (0) root         (0)    36719 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/test/unittest_wfobjs.py
--rw-rw-rw-   0 root         (0) root         (0)    22858 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entities/wfobjs.py
--rw-rw-rw-   0 root         (0) root         (0)    59290 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.217682 cubicweb-4.6.4/cubicweb/ext/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5821 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/ext/html4zope.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/ext/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.217682 cubicweb-4.6.4/cubicweb/ext/test/
--rw-rw-rw-   0 root         (0) root         (0)     2013 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/ext/test/unittest_markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.225683 cubicweb-4.6.4/cubicweb/hooks/
--rw-rw-rw-   0 root         (0) root         (0)     4593 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/email.py
--rw-rw-rw-   0 root         (0) root         (0)    13217 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     5680 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     9725 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     8157 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/security.py
--rw-rw-rw-   0 root         (0) root         (0)    10630 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/synccomputed.py
--rw-rw-rw-   0 root         (0) root         (0)    60802 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/syncschema.py
--rw-rw-rw-   0 root         (0) root         (0)     4913 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/syncsession.py
--rw-rw-rw-   0 root         (0) root         (0)     2952 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/syncsources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.229683 cubicweb-4.6.4/cubicweb/hooks/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.229683 cubicweb-4.6.4/cubicweb/hooks/test/data/
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2728 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.233683 cubicweb-4.6.4/cubicweb/hooks/test/data-computed/
--rw-rw-rw-   0 root         (0) root         (0)     1700 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/data-computed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1729 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_bookmarks.py
--rw-rw-rw-   0 root         (0) root         (0)    13062 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     8490 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_notificationhooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2308 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_security.py
--rw-rw-rw-   0 root         (0) root         (0)     6277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_synccomputed.py
--rw-rw-rw-   0 root         (0) root         (0)    24424 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_syncschema.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_syncsession.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/test/unittest_syncsources.py
--rw-rw-rw-   0 root         (0) root         (0)    15886 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/hooks/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.233683 cubicweb-4.6.4/cubicweb/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    93082 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/i18n/de.po
--rw-rw-rw-   0 root         (0) root         (0)    61668 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)   112148 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)   106920 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     3749 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     5624 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3352 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/md5crypt.py
--rw-rw-rw-   0 root         (0) root         (0)    22356 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/migration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.237683 cubicweb-4.6.4/cubicweb/misc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.241683 cubicweb-4.6.4/cubicweb/misc/migration/
--rw-rw-rw-   0 root         (0) root         (0)      688 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.22.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.22.1_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.22.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.23.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.24.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     1410 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.24.4_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.27.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.30.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.31.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.32.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/3.38.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)    20108 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/bootstrapmigration_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     3368 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/migration/postcreate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.245683 cubicweb-4.6.4/cubicweb/misc/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1446 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/scripts/chpasswd.py
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/scripts/detect_cycle.py
--rw-rw-rw-   0 root         (0) root         (0)     5710 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/scripts/fast_drop_entities.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/scripts/ldap_change_base_dn.py
--rw-rw-rw-   0 root         (0) root         (0)     3466 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/scripts/migration_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/misc/source_highlight.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/mttransforms.py
--rw-rw-rw-   0 root         (0) root         (0)    17397 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/multipart.py
--rw-rw-rw-   0 root         (0) root         (0)    50906 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/predicates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.253683 cubicweb-4.6.4/cubicweb/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)     9523 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11835 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4474 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1483 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/csrf.py
--rw-rw-rw-   0 root         (0) root         (0)     7077 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/debug_source_code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.257683 cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/
--rw-rw-rw-   0 root         (0) root         (0)     1927 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
--rw-rw-rw-   0 root         (0) root         (0)     3912 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     1592 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     4852 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     2980 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     8484 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/debugtoolbar_panels.py
--rw-rw-rw-   0 root         (0) root         (0)     1489 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/default_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/development.ini.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     3767 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     1843 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/pyramid.ini.tmpl
--rw-rw-rw-   0 root         (0) root         (0)    13622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/pyramidctl.py
--rw-rw-rw-   0 root         (0) root         (0)     5309 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     7395 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     9651 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.257683 cubicweb-4.6.4/cubicweb/pyramid/test/
--rw-rw-rw-   0 root         (0) root         (0)     2447 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.257683 cubicweb-4.6.4/cubicweb/pyramid/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.261683 cubicweb-4.6.4/cubicweb/pyramid/test/data/cubicweb_blog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3624 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/test_auth.py
--rw-rw-rw-   0 root         (0) root         (0)     3652 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6447 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/test_content_negociation.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/test/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pyramid/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1929 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/pytestconf.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/rdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/repoapi.py
--rw-rw-rw-   0 root         (0) root         (0)    17494 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/req.py
--rw-rw-rw-   0 root         (0) root         (0)    41745 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/rqlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)    11503 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/rqlsuggestions.py
--rw-rw-rw-   0 root         (0) root         (0)    27291 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/rset.py
--rw-rw-rw-   0 root         (0) root         (0)    11656 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/rtags.py
--rw-rw-rw-   0 root         (0) root         (0)    57848 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     6149 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/schema_exporters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.261683 cubicweb-4.6.4/cubicweb/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     2279 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/schemas/Bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/schemas/_regproc.postgres.sql
--rw-rw-rw-   0 root         (0) root         (0)    13898 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/schemas/base.py
--rw-rw-rw-   0 root         (0) root         (0)    15024 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/schemas/bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)    11853 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/schemas/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.273684 cubicweb-4.6.4/cubicweb/server/
--rw-rw-rw-   0 root         (0) root         (0)    14107 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3275 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/check_unused_index.py
--rw-rw-rw-   0 root         (0) root         (0)    23043 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/checkintegrity.py
--rw-rw-rw-   0 root         (0) root         (0)     6110 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/edition.py
--rw-rw-rw-   0 root         (0) root         (0)    38571 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/hook.py
--rw-rw-rw-   0 root         (0) root         (0)    77833 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/migractions.py
--rw-rw-rw-   0 root         (0) root         (0)    35925 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/querier.py
--rw-rw-rw-   0 root         (0) root         (0)    47931 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/repository.py
--rw-rw-rw-   0 root         (0) root         (0)    19156 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/rqlannotation.py
--rw-rw-rw-   0 root         (0) root         (0)    13785 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/schema2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    28692 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/schemaserial.py
--rw-rw-rw-   0 root         (0) root         (0)     3168 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/serverconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    56184 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/serverctl.py
--rw-rw-rw-   0 root         (0) root         (0)    32564 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.277684 cubicweb-4.6.4/cubicweb/server/sources/
--rw-rw-rw-   0 root         (0) root         (0)    13281 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18181 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/sources/datafeed.py
--rw-rw-rw-   0 root         (0) root         (0)    16896 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/sources/ldapfeed.py
--rw-rw-rw-   0 root         (0) root         (0)    78080 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/sources/native.py
--rw-rw-rw-   0 root         (0) root         (0)    71034 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/sources/rql2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    11149 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/sources/storages.py
--rw-rw-rw-   0 root         (0) root         (0)    22712 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)    22485 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/ssplanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.289684 cubicweb-4.6.4/cubicweb/server/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.293684 cubicweb-4.6.4/cubicweb/server/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.329685 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.329685 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.333685 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.333685 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.333685 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.345685 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/ldap_test.ldif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.345685 cubicweb-4.6.4/cubicweb/server/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/slapd.conf.in
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/sources_extern
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data/sources_multi
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.297684 cubicweb-4.6.4/cubicweb/server/test/data-cwep002/
--rw-rw-rw-   0 root         (0) root         (0)     1299 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-cwep002/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.297684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.297684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.301684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.301684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.305684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.305684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.305684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.309684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.309684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.309684 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.313685 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.313685 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.317685 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.317685 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.321685 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.321685 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.321685 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.325685 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/Company.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/Dates.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/State.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3778 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/toignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.325685 cubicweb-4.6.4/cubicweb/server/test/data-schemaserial/
--rw-rw-rw-   0 root         (0) root         (0)     1345 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schemaserial/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/data-schemaserial/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.345685 cubicweb-4.6.4/cubicweb/server/test/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.345685 cubicweb-4.6.4/cubicweb/server/test/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8829 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_datafeed.py
--rw-rw-rw-   0 root         (0) root         (0)     2192 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_edition.py
--rw-rw-rw-   0 root         (0) root         (0)     4875 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_hook.py
--rw-rw-rw-   0 root         (0) root         (0)    26126 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_ldapsource.py
--rw-rw-rw-   0 root         (0) root         (0)    96689 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_querier.py
--rw-rw-rw-   0 root         (0) root         (0)   101040 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_rql2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    23306 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_rqlannotation.py
--rw-rw-rw-   0 root         (0) root         (0)    11087 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_schema2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    28561 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_schemaserial.py
--rw-rw-rw-   0 root         (0) root         (0)    38100 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_server_security.py
--rw-rw-rw-   0 root         (0) root         (0)     5431 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3908 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_serverctl.py
--rw-rw-rw-   0 root         (0) root         (0)     2296 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_sources_native.py
--rw-rw-rw-   0 root         (0) root         (0)     2449 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_ssplanner.py
--rw-rw-rw-   0 root         (0) root         (0)    17465 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    21764 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_undo.py
--rw-rw-rw-   0 root         (0) root         (0)     2619 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test/unittest_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.349685 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.353685 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.353685 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.357685 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.357685 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.361686 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.361686 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.361686 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.365686 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     3596 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.365686 cubicweb-4.6.4/cubicweb/server/test_migractions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.369686 cubicweb-4.6.4/cubicweb/server/test_migractions/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.397686 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.397686 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.401686 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.401686 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.401686 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.401686 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.405686 cubicweb-4.6.4/cubicweb/server/test_migractions/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.369686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.369686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.373686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.373686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.377686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.377686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.381686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.381686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.385686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.385686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.385686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.389686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.389686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.393686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.393686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.397686 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.405686 cubicweb-4.6.4/cubicweb/server/test_migractions/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.405686 cubicweb-4.6.4/cubicweb/server/test_migractions/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    47791 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.405686 cubicweb-4.6.4/cubicweb/server/test_migractions2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.409687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.437687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.437687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.441687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.441687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.445687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.445687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.445687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.409687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.413687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.413687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.413687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.417687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.417687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.421687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.421687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.425687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.425687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.425687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.429687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.429687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.433687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.433687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.437687 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.445687 cubicweb-4.6.4/cubicweb/server/test_migractions2/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.449687 cubicweb-4.6.4/cubicweb/server/test_migractions2/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9724 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions2/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.449687 cubicweb-4.6.4/cubicweb/server/test_migractions3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.449687 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.477688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.477688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.481688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.481688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.485688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.485688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.485688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.453688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.453688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.453688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.457688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.457688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.461688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.461688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.461688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.465688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.465688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.469688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.469688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.469688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.473688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.473688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.473688 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.485688 cubicweb-4.6.4/cubicweb/server/test_migractions3/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.489688 cubicweb-4.6.4/cubicweb/server/test_migractions3/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_migractions3/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.489688 cubicweb-4.6.4/cubicweb/server/test_postgres/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.493688 cubicweb-4.6.4/cubicweb/server/test_postgres/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.493688 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.493688 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.497688 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.497688 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.501689 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.501689 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.501689 cubicweb-4.6.4/cubicweb/server/test_postgres/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    10298 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_postgres/unittest_postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.501689 cubicweb-4.6.4/cubicweb/server/test_repository/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.505689 cubicweb-4.6.4/cubicweb/server/test_repository/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.509689 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.509689 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.513689 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.513689 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.513689 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.517689 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.509689 cubicweb-4.6.4/cubicweb/server/test_repository/data-schemaserial/
--rw-rw-rw-   0 root         (0) root         (0)     1345 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data-schemaserial/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    38041 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/test_repository/unittest_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     5178 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/server/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.521689 cubicweb-4.6.4/cubicweb/skeleton/
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/.gitlab-ci.yml.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      262 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/.hgignore.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/.yamllint.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/Dockerfile.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      367 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/skeleton/MANIFEST.in.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     1484 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/README.rst.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.525689 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/
--rw-rw-rw-   0 root         (0) root         (0)       97 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      593 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.525689 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/data/
--rw-rw-rw-   0 root         (0) root         (0)       24 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.525689 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.529689 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/migration/
--rw-rw-rw-   0 root         (0) root         (0)      425 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     2030 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.529689 cubicweb-4.6.4/cubicweb/skeleton/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.529689 cubicweb-4.6.4/cubicweb/skeleton/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     2001 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/test/realdb_test_CUBENAME.py
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/skeleton/tox.ini.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.529689 cubicweb-4.6.4/cubicweb/smoke_test/
--rw-rw-rw-   0 root         (0) root         (0)     1504 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.533689 cubicweb-4.6.4/cubicweb/sobjects/
--rw-rw-rw-   0 root         (0) root         (0)     1364 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/sobjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12938 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/ldapparser.py
--rw-rw-rw-   0 root         (0) root         (0)    14419 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5861 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/services.py
--rw-rw-rw-   0 root         (0) root         (0)     8236 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/supervising.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.533689 cubicweb-4.6.4/cubicweb/sobjects/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.537689 cubicweb-4.6.4/cubicweb/sobjects/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       13 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.537689 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.541689 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.541689 cubicweb-4.6.4/cubicweb/sobjects/test/data/sobjects/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/data/sobjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4020 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/unittest_email.py
--rw-rw-rw-   0 root         (0) root         (0)     3059 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/sobjects/test/unittest_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5404 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/unittest_register_user.py
--rw-rw-rw-   0 root         (0) root         (0)     5051 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/sobjects/test/unittest_supervising.py
--rw-rw-rw-   0 root         (0) root         (0)     1994 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.549690 cubicweb-4.6.4/cubicweb/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.557690 cubicweb-4.6.4/cubicweb/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       31 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.561690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.565690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.565690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/entities.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.565690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/views/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.569690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.569690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/entities/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.569690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/hooks/
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.569690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_forge/
--rw-rw-rw-   0 root         (0) root         (0)      819 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_forge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.573690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.573690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_mycube/
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_mycube/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_mycube/ccplugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.577690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_required_variables/
--rw-rw-rw-   0 root         (0) root         (0)      857 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_required_variables/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.577690 cubicweb-4.6.4/cubicweb/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_tag/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/erqlexpr_on_ertype.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/lowered_etype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.581690 cubicweb-4.6.4/cubicweb/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/migration/0.0.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/migration/0.0.4_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/migration/0.1.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/migration/0.1.0_common.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/migration/0.1.0_repository.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/migration/0.1.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/rqlexpr_on_computedrel.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/rqlexpr_on_ertype_read.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/rrqlexpr_on_attr.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/rrqlexpr_on_eetype.py
--rw-rw-rw-   0 root         (0) root         (0)     4319 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.581690 cubicweb-4.6.4/cubicweb/test/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      164 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/scripts/script1.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/scripts/script2.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/scripts/script3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.585690 cubicweb-4.6.4/cubicweb/test/data/server_migration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/server_migration/2.10.2_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data/server_migration/2.5.0_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/server_migration/2.6.0_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)      882 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data/uppered_rtype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.557690 cubicweb-4.6.4/cubicweb/test/data-rewrite/
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.557690 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.561690 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3723 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data-rewrite/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.585690 cubicweb-4.6.4/cubicweb/test/data_schemareader/
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/data_schemareader/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2304 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/unittest_binary.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_crypto.py
--rw-rw-rw-   0 root         (0) root         (0)    17592 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_cwconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     7457 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/unittest_cwctl.py
--rw-rw-rw-   0 root         (0) root         (0)    48020 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_entity.py
--rw-rw-rw-   0 root         (0) root         (0)     4855 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_fast_drop_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     8357 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_mail.py
--rw-rw-rw-   0 root         (0) root         (0)     7471 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_migration.py
--rw-rw-rw-   0 root         (0) root         (0)    15441 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/unittest_predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     3879 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_repoapi.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_req.py
--rw-rw-rw-   0 root         (0) root         (0)    46300 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/unittest_rqlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     6503 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_rqlsuggestions.py
--rw-rw-rw-   0 root         (0) root         (0)    32589 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_rset.py
--rw-rw-rw-   0 root         (0) root         (0)     6543 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_rtags.py
--rw-rw-rw-   0 root         (0) root         (0)    34435 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4047 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/unittest_toolsutils.py
--rw-rw-rw-   0 root         (0) root         (0)     9658 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_uilib.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/test/unittest_vregistry.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/test/unittest_wfutils.py
--rw-rw-rw-   0 root         (0) root         (0)    16545 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/toolsutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3836 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)    19507 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/uilib.py
--rw-rw-rw-   0 root         (0) root         (0)    12356 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-03-13 14:14:00.000000 cubicweb-4.6.4/cubicweb/wfutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2024-03-13 14:13:59.000000 cubicweb-4.6.4/cubicweb/xy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.765694 cubicweb-4.6.4/cubicweb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5135 2024-03-13 14:14:29.000000 cubicweb-4.6.4/cubicweb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    51719 2024-03-13 14:14:30.000000 cubicweb-4.6.4/cubicweb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 14:14:29.000000 cubicweb-4.6.4/cubicweb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2024-03-13 14:14:29.000000 cubicweb-4.6.4/cubicweb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-13 14:14:29.000000 cubicweb-4.6.4/cubicweb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      474 2024-03-13 14:14:29.000000 cubicweb-4.6.4/cubicweb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-03-13 14:14:29.000000 cubicweb-4.6.4/cubicweb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.589691 cubicweb-4.6.4/doc/
--rw-rw-rw-   0 root         (0) root         (0)     7511 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/4.0.0_how_to_migrate.rst
--rw-rw-rw-   0 root         (0) root         (0)     2811 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.589691 cubicweb-4.6.4/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)    34494 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/_static/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     9202 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/_static/logo-cubicweb.svg
--rw-rw-rw-   0 root         (0) root         (0)     1681 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/announce.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     1982 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/announce.fr.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.597691 cubicweb-4.6.4/doc/api/
--rw-rw-rw-   0 root         (0) root         (0)     2251 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/api/__init__.rst
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/appobject.rst
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/cwvreg.rst
--rw-rw-rw-   0 root         (0) root         (0)      491 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/api/dataimport.rst
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2540 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/predicates.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.601691 cubicweb-4.6.4/doc/api/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/pyramid/auth.rst
--rw-rw-rw-   0 root         (0) root         (0)      358 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/api/pyramid/bwcompat.rst
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/pyramid/core.rst
--rw-rw-rw-   0 root         (0) root         (0)      296 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/pyramid/login.rst
--rw-rw-rw-   0 root         (0) root         (0)      259 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/api/pyramid/profile.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/pyramid/session.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/pyramid/url_redirection.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/pyramid.rst
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/req.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/rset.rst
--rw-rw-rw-   0 root         (0) root         (0)      781 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/api/urlpublishing.rst
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/urlrewrite.rst
--rw-rw-rw-   0 root         (0) root         (0)      520 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/api/web.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.601691 cubicweb-4.6.4/doc/book/
--rw-rw-rw-   0 root         (0) root         (0)    14655 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/MERGE_ME-tut-create-app.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     7806 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/MERGE_ME-tut-create-gae-app.en.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.601691 cubicweb-4.6.4/doc/book/_maybe_to_integrate/
--rw-rw-rw-   0 root         (0) root         (0)      225 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/_maybe_to_integrate/D050-architecture.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     1286 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/_maybe_to_integrate/rss-xml.rst
--rw-rw-rw-   0 root         (0) root         (0)      751 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/_maybe_to_integrate/template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.605691 cubicweb-4.6.4/doc/book/additionnal_services/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/additionnal_services/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    13562 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/additionnal_services/undo.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.613691 cubicweb-4.6.4/doc/book/admin/
--rw-rw-rw-   0 root         (0) root         (0)     2253 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/backups.rst
--rw-rw-rw-   0 root         (0) root         (0)     5658 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/admin/config.rst
--rw-rw-rw-   0 root         (0) root         (0)     3879 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/create-instance.rst
--rw-rw-rw-   0 root         (0) root         (0)     3396 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/cubicweb-ctl.rst
--rw-rw-rw-   0 root         (0) root         (0)     4034 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/deploy.rst
--rw-rw-rw-   0 root         (0) root         (0)      409 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5265 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/admin/instance-config.rst
--rw-rw-rw-   0 root         (0) root         (0)     4825 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/ldap.rst
--rw-rw-rw-   0 root         (0) root         (0)      130 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/multisources.rst
--rw-rw-rw-   0 root         (0) root         (0)      366 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/admin/rql-logs.rst
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/setup.rst
--rw-rw-rw-   0 root         (0) root         (0)     3596 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/admin/site-config.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.617691 cubicweb-4.6.4/doc/book/annexes/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/depends.rst
--rw-rw-rw-   0 root         (0) root         (0)     3257 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/docstrings-conventions.rst
--rw-rw-rw-   0 root         (0) root         (0)    16153 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/annexes/faq.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3481 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/mercurial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.621691 cubicweb-4.6.4/doc/book/annexes/rql/
--rw-rw-rw-   0 root         (0) root         (0)     2115 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/annexes/rql/Graph-ex.gif
--rw-rw-rw-   0 root         (0) root         (0)     1167 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/rql/debugging.rst
--rw-rw-rw-   0 root         (0) root         (0)     4697 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/rql/implementation.rst
--rw-rw-rw-   0 root         (0) root         (0)      267 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/rql/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5570 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/rql/intro.rst
--rw-rw-rw-   0 root         (0) root         (0)    27490 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/annexes/rql/language.rst
--rw-rw-rw-   0 root         (0) root         (0)     2703 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/annexes/rql/usecases.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.625691 cubicweb-4.6.4/doc/book/devrepo/
--rw-rw-rw-   0 root         (0) root         (0)     2147 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/connections_pooler.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.629691 cubicweb-4.6.4/doc/book/devrepo/cubes/
--rw-rw-rw-   0 root         (0) root         (0)     2645 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devrepo/cubes/available-cubes.rst
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/cubes/cc-newcube.rst
--rw-rw-rw-   0 root         (0) root         (0)      208 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/cubes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6827 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/cubes/layout.rst
--rw-rw-rw-   0 root         (0) root         (0)     1967 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/cubes/what-is-a-cube.rst
--rw-rw-rw-   0 root         (0) root         (0)     4021 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devrepo/dataimport.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.629691 cubicweb-4.6.4/doc/book/devrepo/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)     1389 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/datamodel/baseschema.rst
--rw-rw-rw-   0 root         (0) root         (0)     6178 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/datamodel/define-workflows.rst
--rw-rw-rw-   0 root         (0) root         (0)    34880 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devrepo/datamodel/definition.rst
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/datamodel/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/datamodel/metadata.rst
--rw-rw-rw-   0 root         (0) root         (0)     2940 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/debug_channels.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.629691 cubicweb-4.6.4/doc/book/devrepo/devcore/
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/devcore/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1129 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devrepo/devcore/reqbase.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.633691 cubicweb-4.6.4/doc/book/devrepo/entityclasses/
--rw-rw-rw-   0 root         (0) root         (0)     5159 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/entityclasses/adapters.rst
--rw-rw-rw-   0 root         (0) root         (0)     7268 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/entityclasses/application-logic.rst
--rw-rw-rw-   0 root         (0) root         (0)     5285 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devrepo/entityclasses/data-as-objects.rst
--rw-rw-rw-   0 root         (0) root         (0)      303 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/entityclasses/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1719 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/entityclasses/load-sort.rst
--rw-rw-rw-   0 root         (0) root         (0)     4399 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/fti.rst
--rw-rw-rw-   0 root         (0) root         (0)      504 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     9469 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devrepo/migration.rst
--rw-rw-rw-   0 root         (0) root         (0)     2668 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/profiling.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.637692 cubicweb-4.6.4/doc/book/devrepo/repo/
--rw-rw-rw-   0 root         (0) root         (0)     9731 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/repo/hooks.rst
--rw-rw-rw-   0 root         (0) root         (0)      155 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devrepo/repo/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1087 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/repo/notifications.rst
--rw-rw-rw-   0 root         (0) root         (0)    11467 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/repo/sessions.rst
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/repo/tasks.rst
--rw-rw-rw-   0 root         (0) root         (0)    21316 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devrepo/testing.rst
--rw-rw-rw-   0 root         (0) root         (0)    18289 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devrepo/vreg.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.645692 cubicweb-4.6.4/doc/book/devweb/
--rw-rw-rw-   0 root         (0) root         (0)      915 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/ajax.rst
--rw-rw-rw-   0 root         (0) root         (0)     3473 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/controllers.rst
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devweb/css.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.645692 cubicweb-4.6.4/doc/book/devweb/edition/
--rw-rw-rw-   0 root         (0) root         (0)    11979 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/edition/dissection.rst
--rw-rw-rw-   0 root         (0) root         (0)     3955 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/edition/editcontroller.rst
--rw-rw-rw-   0 root         (0) root         (0)     9905 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/edition/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)    15506 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/edition/form.rst
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devweb/edition/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      698 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/facets.rst
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/httpcaching.rst
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devweb/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    10057 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/internationalization.rst
--rw-rw-rw-   0 root         (0) root         (0)    14107 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/js.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/property.rst
--rw-rw-rw-   0 root         (0) root         (0)     2017 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/publisher.rst
--rw-rw-rw-   0 root         (0) root         (0)     5119 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devweb/request.rst
--rw-rw-rw-   0 root         (0) root         (0)      709 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/resource.rst
--rw-rw-rw-   0 root         (0) root         (0)      454 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/rtags.rst
--rw-rw-rw-   0 root         (0) root         (0)     1418 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devweb/searchbar.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.653692 cubicweb-4.6.4/doc/book/devweb/views/
--rw-rw-rw-   0 root         (0) root         (0)     5889 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/basetemplates.rst
--rw-rw-rw-   0 root         (0) root         (0)      701 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/baseviews.rst
--rw-rw-rw-   0 root         (0) root         (0)     1291 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/boxes.rst
--rw-rw-rw-   0 root         (0) root         (0)     2320 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/breadcrumbs.rst
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devweb/views/idownloadable.rst
--rw-rw-rw-   0 root         (0) root         (0)      476 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    10179 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/primary.rst
--rw-rw-rw-   0 root         (0) root         (0)     5991 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devweb/views/reledit.rst
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/startup.rst
--rw-rw-rw-   0 root         (0) root         (0)     5919 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/table.rst
--rw-rw-rw-   0 root         (0) root         (0)     5506 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/urlpublish.rst
--rw-rw-rw-   0 root         (0) root         (0)     4192 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/views.rst
--rw-rw-rw-   0 root         (0) root         (0)      347 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/devweb/views/wdoc.rst
--rw-rw-rw-   0 root         (0) root         (0)     1703 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/views/xmlrss.rst
--rw-rw-rw-   0 root         (0) root         (0)      947 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/devweb/warning.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.657692 cubicweb-4.6.4/doc/book/intro/
--rw-rw-rw-   0 root         (0) root         (0)    10427 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/intro/concepts.rst
--rw-rw-rw-   0 root         (0) root         (0)     1369 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/intro/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      385 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/intro/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.657692 cubicweb-4.6.4/doc/book/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)     1371 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/pyramid/auth.rst
--rw-rw-rw-   0 root         (0) root         (0)     1314 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/pyramid/ctl.rst
--rw-rw-rw-   0 root         (0) root         (0)     3771 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/pyramid/debug_toolbar.rst
--rw-rw-rw-   0 root         (0) root         (0)      844 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/pyramid/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1795 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/pyramid/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     5411 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/book/pyramid/settings.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.661692 cubicweb-4.6.4/doc/book/security/
--rw-rw-rw-   0 root         (0) root         (0)     8041 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/security/csrf.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.661692 cubicweb-4.6.4/doc/book/src/
--rw-rw-rw-   0 root         (0) root         (0)     2930 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/src/archi_globale.dia
--rw-rw-rw-   0 root         (0) root         (0)     1735 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/book/src/main_template_layout.dia
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.677692 cubicweb-4.6.4/doc/changes/
--rw-rw-rw-   0 root         (0) root         (0)     6619 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.14.rst
--rw-rw-rw-   0 root         (0) root         (0)     3904 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/3.15.rst
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.16.rst
--rw-rw-rw-   0 root         (0) root         (0)     1815 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.17.rst
--rw-rw-rw-   0 root         (0) root         (0)     3632 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/3.18.rst
--rw-rw-rw-   0 root         (0) root         (0)     6757 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.19.rst
--rw-rw-rw-   0 root         (0) root         (0)     3165 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.20.rst
--rw-rw-rw-   0 root         (0) root         (0)     2991 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.21.rst
--rw-rw-rw-   0 root         (0) root         (0)     3689 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.22.rst
--rw-rw-rw-   0 root         (0) root         (0)     2799 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/3.23.rst
--rw-rw-rw-   0 root         (0) root         (0)     4033 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.24.rst
--rw-rw-rw-   0 root         (0) root         (0)     4655 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.25.rst
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/3.26.rst
--rw-rw-rw-   0 root         (0) root         (0)     6870 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.27.rst
--rw-rw-rw-   0 root         (0) root         (0)     2656 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.28.rst
--rw-rw-rw-   0 root         (0) root         (0)     1249 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.29.rst
--rw-rw-rw-   0 root         (0) root         (0)     5588 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.30.rst
--rw-rw-rw-   0 root         (0) root         (0)     3683 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/3.31.rst
--rw-rw-rw-   0 root         (0) root         (0)     7979 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.32.rst
--rw-rw-rw-   0 root         (0) root         (0)     1728 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.32_reledit.rst
--rw-rw-rw-   0 root         (0) root         (0)     5635 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/3.33.rst
--rw-rw-rw-   0 root         (0) root         (0)     4524 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.34.rst
--rw-rw-rw-   0 root         (0) root         (0)     4849 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.35.rst
--rw-rw-rw-   0 root         (0) root         (0)     4507 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/3.36.rst
--rw-rw-rw-   0 root         (0) root         (0)     5437 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/3.37.rst
--rw-rw-rw-   0 root         (0) root         (0)     8587 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/3.38.rst
--rw-rw-rw-   0 root         (0) root         (0)     6425 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      914 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/4.2.rst
--rw-rw-rw-   0 root         (0) root         (0)     2656 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/4.3.rst
--rw-rw-rw-   0 root         (0) root         (0)      264 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/4.4.rst
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/4.5.rst
--rw-rw-rw-   0 root         (0) root         (0)     1949 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/4.6.rst
--rw-rw-rw-   0 root         (0) root         (0)      725 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/changes/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/changes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     7654 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.745694 cubicweb-4.6.4/doc/images/
--rw-rw-rw-   0 root         (0) root         (0)    98393 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/03-transitions-view_en.png
--rw-rw-rw-   0 root         (0) root         (0)    12650 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/breadcrumbs_header.png
--rw-rw-rw-   0 root         (0) root         (0)    85073 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/debugtoolbar_general_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   124385 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/debugtoolbar_registry_content_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   111325 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/debugtoolbar_registry_decisions_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   134505 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/debugtoolbar_rql_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   192629 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/debugtoolbar_rql_traceback_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   107766 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/debugtoolbar_show_source.png
--rw-rw-rw-   0 root         (0) root         (0)    55625 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/debugtoolbar_show_source_link.png
--rw-rw-rw-   0 root         (0) root         (0)   126845 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/debugtoolbar_sql_panel.png
--rw-rw-rw-   0 root         (0) root         (0)    97343 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/debugtoolbar_traceback_source_link.png
--rw-rw-rw-   0 root         (0) root         (0)    57300 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/example-card-with-rql-directive.png
--rw-rw-rw-   0 root         (0) root         (0)    55168 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/example-card-with-rql-table-directive.png
--rw-rw-rw-   0 root         (0) root         (0)     2277 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/facet_date_range.png
--rw-rw-rw-   0 root         (0) root         (0)     6013 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/facet_has_image.png
--rw-rw-rw-   0 root         (0) root         (0)    22016 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/facet_overview.png
--rw-rw-rw-   0 root         (0) root         (0)     1873 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/facet_range.png
--rw-rw-rw-   0 root         (0) root         (0)    21685 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/lax-book_00-login_en.png
--rw-rw-rw-   0 root         (0) root         (0)    30326 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/lax-book_01-start_en.png
--rw-rw-rw-   0 root         (0) root         (0)    35859 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/lax-book_02-cookie-values_en.png
--rw-rw-rw-   0 root         (0) root         (0)    33922 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/lax-book_02-create-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    28123 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/lax-book_03-list-one-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    82897 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/lax-book_03-site-config-panel_en.png
--rw-rw-rw-   0 root         (0) root         (0)   119813 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/lax-book_03-state-submitted_en.png
--rw-rw-rw-   0 root         (0) root         (0)    98393 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/lax-book_03-transitions-view_en.png
--rw-rw-rw-   0 root         (0) root         (0)    34771 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/lax-book_04-detail-one-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    28345 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/lax-book_05-list-two-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    49230 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/lax-book_06-add-relation-entryof_en.png
--rw-rw-rw-   0 root         (0) root         (0)    96838 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/lax-book_06-main-template-logo_en.png
--rw-rw-rw-   0 root         (0) root         (0)    40383 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/lax-book_07-detail-one-blogentry_en.png
--rw-rw-rw-   0 root         (0) root         (0)    30591 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/lax-book_08-schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    33091 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/lax-book_09-new-view-blogentry_en.png
--rw-rw-rw-   0 root         (0) root         (0)    42230 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/lax-book_10-blog-with-two-entries_en.png
--rw-rw-rw-   0 root         (0) root         (0)    17757 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/main_template.png
--rw-rw-rw-   0 root         (0) root         (0)     8674 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/main_template.svg
--rw-rw-rw-   0 root         (0) root         (0)    13842 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/main_template_layout.png
--rw-rw-rw-   0 root         (0) root         (0)    46411 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/primaryview_template.png
--rw-rw-rw-   0 root         (0) root         (0)    14758 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/primaryview_template.svg
--rw-rw-rw-   0 root         (0) root         (0)    22773 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/request_session.png
--rw-rw-rw-   0 root         (0) root         (0)     7211 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/request_session.svg
--rw-rw-rw-   0 root         (0) root         (0)    12030 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/server-class-diagram.png
--rw-rw-rw-   0 root         (0) root         (0)    62022 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_blog-form_en.png
--rw-rw-rw-   0 root         (0) root         (0)   105173 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_blog-primary-after-post-creation_en.png
--rw-rw-rw-   0 root         (0) root         (0)    58500 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_blog-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    42013 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_blogs-list_en.png
--rw-rw-rw-   0 root         (0) root         (0)   109769 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_form-generic-relations_en.png
--rw-rw-rw-   0 root         (0) root         (0)    65646 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_index_en.png
--rw-rw-rw-   0 root         (0) root         (0)    13605 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_index_gettext_en.png
--rw-rw-rw-   0 root         (0) root         (0)    88970 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_index_logged_in_en.png
--rw-rw-rw-   0 root         (0) root         (0)    11548 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_login-form_en.png
--rw-rw-rw-   0 root         (0) root         (0)   100347 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    63097 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_myblog-community-custom-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    62431 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_myblog-community-default-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    74856 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_myblog-community-taggable-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    79709 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_myblog-custom-footer_en.png
--rw-rw-rw-   0 root         (0) root         (0)   128406 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_myblog-schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    71500 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_myblog-siteinfo_en.png
--rw-rw-rw-   0 root         (0) root         (0)   104834 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    22098 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-base_schema_graphviz_en.png
--rw-rw-rw-   0 root         (0) root         (0)   150520 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-base_siteconfig_en.png
--rw-rw-rw-   0 root         (0) root         (0)    60672 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-museum_admin.png
--rw-rw-rw-   0 root         (0) root         (0)    61388 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-museum_city_created.png
--rw-rw-rw-   0 root         (0) root         (0)    50694 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-museum_city_creation.png
--rw-rw-rw-   0 root         (0) root         (0)    71561 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-museum_data_model_schema.png
--rw-rw-rw-   0 root         (0) root         (0)    48896 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-museum_empty_instance.png
--rw-rw-rw-   0 root         (0) root         (0)    55671 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-museum_finished_import.png
--rw-rw-rw-   0 root         (0) root         (0)    57063 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-museum_list_view.png
--rw-rw-rw-   0 root         (0) root         (0)    70893 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-museum_museum_created.png
--rw-rw-rw-   0 root         (0) root         (0)    61656 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-museum_museum_creation.png
--rw-rw-rw-   0 root         (0) root         (0)    74005 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-museum_museum_with_city_name.png
--rw-rw-rw-   0 root         (0) root         (0)   225824 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-museum_react_map.png
--rw-rw-rw-   0 root         (0) root         (0)    53544 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-museum_with_schema.png
--rw-rw-rw-   0 root         (0) root         (0)   354637 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_background-image.png
--rw-rw-rw-   0 root         (0) root         (0)    30437 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_boxes.png
--rw-rw-rw-   0 root         (0) root         (0)    54643 2024-03-13 14:13:59.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_breadcrumbs.png
--rw-rw-rw-   0 root         (0) root         (0)   324086 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_facets.png
--rw-rw-rw-   0 root         (0) root         (0)    40520 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_grey-box.png
--rw-rw-rw-   0 root         (0) root         (0)    16843 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_index-after.png
--rw-rw-rw-   0 root         (0) root         (0)    26875 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_index-before.png
--rw-rw-rw-   0 root         (0) root         (0)    17580 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_login-box.png
--rw-rw-rw-   0 root         (0) root         (0)    57814 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_prevnext.png
--rw-rw-rw-   0 root         (0) root         (0)    81362 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_ui1.png
--rw-rw-rw-   0 root         (0) root         (0)    93291 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_ui2.png
--rw-rw-rw-   0 root         (0) root         (0)   290338 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/tutos-photowebsite_ui3.png
--rw-rw-rw-   0 root         (0) root         (0)    43051 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/undo_history-view_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    26036 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/undo_mesage_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    39625 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/undo_startup-link_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    17558 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/views-table-filter-shadow.png
--rw-rw-rw-   0 root         (0) root         (0)    14013 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/views-table-filter.png
--rw-rw-rw-   0 root         (0) root         (0)    12375 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/views-table-shadow.png
--rw-rw-rw-   0 root         (0) root         (0)     9676 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/images/views-table.png
--rw-rw-rw-   0 root         (0) root         (0)     7344 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2011 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/plan_formation_python_cubicweb.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/stdlib.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.749694 cubicweb-4.6.4/doc/tools/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tools/generate_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tools/mode_plan.py
--rwxrwxrwx   0 root         (0) root         (0)     4944 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tools/pyjsrest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.749694 cubicweb-4.6.4/doc/tutorials/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.753694 cubicweb-4.6.4/doc/tutorials/advanced/
--rw-rw-rw-   0 root         (0) root         (0)      604 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/advanced/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5486 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/advanced/part01_create-cube.rst
--rw-rw-rw-   0 root         (0) root         (0)    17016 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/advanced/part02_security.rst
--rw-rw-rw-   0 root         (0) root         (0)     5614 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/advanced/part03_bfss.rst
--rw-rw-rw-   0 root         (0) root         (0)    15384 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/advanced/part04_ui-base.rst
--rw-rw-rw-   0 root         (0) root         (0)    15114 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/advanced/part05_ui-advanced.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.753694 cubicweb-4.6.4/doc/tutorials/base/
--rw-rw-rw-   0 root         (0) root         (0)     3867 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/base/blog-in-five-minutes.rst
--rw-rw-rw-   0 root         (0) root         (0)      675 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/base/conclusion.rst
--rw-rw-rw-   0 root         (0) root         (0)    20435 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/base/customizing-the-application.rst
--rw-rw-rw-   0 root         (0) root         (0)     7821 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/base/discovering-the-ui.rst
--rw-rw-rw-   0 root         (0) root         (0)     1340 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/base/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.757694 cubicweb-4.6.4/doc/tutorials/dataimport/
--rw-rw-rw-   0 root         (0) root         (0)     9014 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/dataimport/diseasome_import.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/dataimport/diseasome_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    29917 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/dataimport/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6576 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/dataimport/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      568 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.757694 cubicweb-4.6.4/doc/tutorials/museum/
--rw-rw-rw-   0 root         (0) root         (0)     5961 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/museum/data-management.rst
--rw-rw-rw-   0 root         (0) root         (0)     6403 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/museum/develop-app.rst
--rw-rw-rw-   0 root         (0) root         (0)     3860 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/museum/develop-ui.rst
--rw-rw-rw-   0 root         (0) root         (0)     8840 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/museum/enhance-views.rst
--rw-rw-rw-   0 root         (0) root         (0)     2702 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/museum/getting-started.rst
--rw-rw-rw-   0 root         (0) root         (0)     1595 2024-03-13 14:14:00.000000 cubicweb-4.6.4/doc/tutorials/museum/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.761694 cubicweb-4.6.4/extras/
--rw-rw-rw-   0 root         (0) root         (0)     3545 2024-03-13 14:14:00.000000 cubicweb-4.6.4/extras/cubicweb-ctl.bash_completion
--rw-rw-rw-   0 root         (0) root         (0)     7414 2024-03-13 14:14:00.000000 cubicweb-4.6.4/jshintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.761694 cubicweb-4.6.4/man/
--rw-rw-rw-   0 root         (0) root         (0)      651 2024-03-13 14:14:00.000000 cubicweb-4.6.4/man/cubicweb-ctl.1
--rw-rw-rw-   0 root         (0) root         (0)       56 2024-03-13 14:14:00.000000 cubicweb-4.6.4/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-03-13 14:14:00.000000 cubicweb-4.6.4/pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-13 14:14:30.765694 cubicweb-4.6.4/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      174 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/dev.txt
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/doc.txt
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/from-forge.txt
--rw-rw-rw-   0 root         (0) root         (0)      380 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/test-base.txt
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/test-dataimport.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/test-devtools.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/test-ext.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/test-hooks.txt
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/test-pyramid.txt
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-03-13 14:14:00.000000 cubicweb-4.6.4/requirements/test-server.txt
--rw-rw-rw-   0 root         (0) root         (0)      115 2024-03-13 14:14:30.769694 cubicweb-4.6.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3249 2024-03-13 14:14:00.000000 cubicweb-4.6.4/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     9036 2024-03-13 14:14:00.000000 cubicweb-4.6.4/tox.ini
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.138896 cubicweb-4.7.0/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2002 2024-04-03 11:58:45.000000 cubicweb-4.7.0/CONTRIBUTING.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17987 2021-04-20 14:56:24.000000 cubicweb-4.7.0/COPYING
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    26527 2021-04-20 14:56:24.000000 cubicweb-4.7.0/COPYING.LESSER
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4977 2024-04-03 11:58:45.000000 cubicweb-4.7.0/MANIFEST.in
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4250 2024-04-03 11:58:52.138896 cubicweb-4.7.0/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3819 2024-04-03 11:58:45.000000 cubicweb-4.7.0/README.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.018895 cubicweb-4.7.0/cubicweb/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7503 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/__init__.py
+-rwxr-xr-x   0 schabot   (1000) schabot   (1000)       69 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/__main__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1665 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6885 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/_exceptions.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3860 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/_gcdebug.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5211 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/appobject.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1671 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/crypto.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    66337 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/cwconfig.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    32638 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/cwctl.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4899 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/cwgettext.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    25982 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/cwvreg.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.018895 cubicweb-4.7.0/cubicweb/dataimport/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1987 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3274 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/csv.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    21081 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/importer.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    26515 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/massive_store.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15503 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/pgstore.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    18127 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/stores.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.018895 cubicweb-4.7.0/cubicweb/dataimport/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/dataimport/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   474710 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data/geonames.csv
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      113 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data/people.csv
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1231 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    12362 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data/timeZones.txt
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/dataimport/test/data-massimport/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1987 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/test/data-massimport/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2513 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/test/test_csv.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    16176 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/test/test_massive_store.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4179 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/dataimport/test/test_pgstore.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8221 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/test/test_stores.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10720 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/dataimport/test/unittest_importer.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2669 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/debug.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    27112 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5449 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/apptest_config.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      266 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/data/cwmock.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5146 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/data/qunit.css
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   115758 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/data/qunit.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    39808 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/devctl.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3702 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/fake.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    24531 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/fill.py
+-rwxr-xr-x   0 schabot   (1000) schabot   (1000)     1011 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/fix_po_encoding
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10982 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/htmlparser.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5298 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/httptest.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9195 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/instrument.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2354 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/realdbtest.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10873 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/repotest.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6796 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/stresstester.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/bootstrap_cubes
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11311 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/firstnames.txt
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:51.998895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      460 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2657 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.022895 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       13 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1720 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1679 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:51.998895 cubicweb-4.7.0/cubicweb/devtools/test/data/static/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/dep_1.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       10 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/deps_2.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      353 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      321 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      136 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      136 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      719 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/utils.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4354 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_dbfill.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6402 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_devctl.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2475 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_fill.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3225 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_i18n.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4687 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/test/unittest_testlib.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    20848 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/devtools/testlib.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/entities/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5324 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    24563 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/adapters.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6476 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/entities/authobjs.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4193 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/lib.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5944 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/schemaobjs.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4095 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/sources.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/entities/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/entities/test/data/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/entities/test/data/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      893 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/entities/test/data/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1307 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/entities/test/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9992 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/test/unittest_base.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    36719 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/test/unittest_wfobjs.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22858 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entities/wfobjs.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    59384 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/entity.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/ext/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/ext/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5821 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/ext/html4zope.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1839 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/ext/markdown.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/ext/test/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2013 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/ext/test/unittest_markdown.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.026895 cubicweb-4.7.0/cubicweb/hooks/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4593 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1544 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/bookmark.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3089 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/email.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13217 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/integrity.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5680 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/metadata.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9725 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/notification.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8157 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/security.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10630 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/synccomputed.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    60802 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/syncschema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4913 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/syncsession.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2952 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/syncsources.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/hooks/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/hooks/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      291 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/data/hooks.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2728 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/data/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/hooks/test/data-computed/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1700 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/data-computed/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1729 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_bookmarks.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13062 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_hooks.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8490 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_integrity.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1513 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_notificationhooks.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2308 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_security.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_synccomputed.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    24424 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncschema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4778 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncsession.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2667 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncsources.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15886 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/hooks/workflow.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/i18n/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    93082 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n/de.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    61668 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n/en.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   112148 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n/es.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   106920 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n/fr.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3749 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/i18n.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5624 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/mail.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3352 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/md5crypt.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22356 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/migration.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/misc/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/misc/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      688 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.22.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      395 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.22.1_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.22.3_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3186 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.23.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      913 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.24.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1410 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.24.4_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      117 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.27.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      217 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.30.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.31.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      423 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.32.3_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       25 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/migration/3.38.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    20108 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/bootstrapmigration_repository.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3368 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/migration/postcreate.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.030895 cubicweb-4.7.0/cubicweb/misc/scripts/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1446 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/scripts/chpasswd.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      393 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/scripts/detect_cycle.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5710 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/scripts/fast_drop_entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      799 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/scripts/ldap_change_base_dn.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3466 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/misc/scripts/migration_helper.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1097 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/misc/source_highlight.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3270 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/mttransforms.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17397 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/multipart.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    50906 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/predicates.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9523 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11835 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/auth.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4474 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/config.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7548 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/core.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1483 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pyramid/csrf.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7077 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_source_code.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1927 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1505 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3912 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1592 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4852 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2980 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8484 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/debugtoolbar_panels.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1489 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/default_session.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1837 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/development.ini.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3767 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/predicates.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1843 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/pyramid.ini.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/pyramidctl.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5309 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/resources.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7395 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/rest_api.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9651 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/session.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/test/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2447 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        5 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      416 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1327 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3624 2024-02-23 08:55:59.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_auth.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3652 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_config.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6447 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_content_negociation.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      782 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_core.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      986 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pyramid/test/test_tools.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2065 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pyramid/tools.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1929 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/pytestconf.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1802 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/rdf.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2170 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/repoapi.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17494 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/req.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    41745 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/rqlrewrite.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11503 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/rqlsuggestions.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    27291 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/rset.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11656 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/rtags.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    57848 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6149 2024-02-23 08:55:59.000000 cubicweb-4.7.0/cubicweb/schema_exporters.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.034895 cubicweb-4.7.0/cubicweb/schemas/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2279 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/Bookmark.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1696 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1662 2022-08-09 14:03:17.000000 cubicweb-4.7.0/cubicweb/schemas/_regproc.postgres.sql
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13898 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/base.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15024 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/bootstrap.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11853 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/schemas/workflow.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.038895 cubicweb-4.7.0/cubicweb/server/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    14107 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3275 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/check_unused_index.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    23043 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/checkintegrity.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6110 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/edition.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    38571 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/hook.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    77833 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/migractions.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    35925 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/querier.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    47931 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/repository.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    19156 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/rqlannotation.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13785 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/schema2sql.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    28692 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/schemaserial.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3168 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/serverconfig.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    56184 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/serverctl.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    32564 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/session.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.038895 cubicweb-4.7.0/cubicweb/server/sources/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13281 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    18181 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/datafeed.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    16896 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/ldapfeed.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    78080 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/native.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    71034 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/rql2sql.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11149 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sources/storages.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22712 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/sqlutils.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22485 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/ssplanner.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1087 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/hooks.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1503 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/ldap_test.ldif
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/data/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data/site_cubicweb.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1565 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/data/slapd.conf.in
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       77 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/sources_extern
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       97 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data/sources_multi
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-cwep002/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1299 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-cwep002/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      153 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1562 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2876 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.042895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8437 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9716 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-migractions/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2510 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/Company.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1242 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/Dates.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3298 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/State.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      980 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3778 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/toignore
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.046895 cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1345 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/datacomputed/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test/datacomputed/migratedapp/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/datacomputed/migratedapp/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1851 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/datacomputed/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8829 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_datafeed.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2192 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_edition.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4875 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_hook.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    26126 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_ldapsource.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    96689 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_querier.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   101040 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_rql2sql.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    23306 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_rqlannotation.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11087 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_schema2sql.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    28561 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_schemaserial.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    38100 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_server_security.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5431 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_server_utils.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3908 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_serverctl.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2296 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_session.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1609 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_sources_native.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2449 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_sqlutils.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3285 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_ssplanner.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17465 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_storage.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1139 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_tools.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    21764 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_undo.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2619 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test/unittest_utils.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/hooks.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3596 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.050895 cubicweb-4.7.0/cubicweb/server/test_migractions/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/hooks.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      153 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1562 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2876 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.054895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8437 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9716 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/migratedapp/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1851 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    47791 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions/unittest_migractions.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions2/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/hooks.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.058895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      153 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1562 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2876 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.062895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8437 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9716 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1851 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9724 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions2/unittest_migractions.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions3/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/hooks.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       50 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.066895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      153 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      470 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1562 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2876 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.070895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8437 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9716 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1851 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1972 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_migractions3/unittest_migractions.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.074895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/hooks.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_postgres/data/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1420 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/migration/postcreate.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/data/site_cubicweb.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10298 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_postgres/unittest_postgres.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       40 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      774 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1277 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      569 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1202 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/hooks.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10285 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.078895 cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1345 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1121 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    38041 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/test_repository/unittest_repository.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5178 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/server/utils.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1112 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      262 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/.hgignore.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      109 2022-08-09 14:03:17.000000 cubicweb-4.7.0/cubicweb/skeleton/.yamllint.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      249 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/Dockerfile.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      367 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/MANIFEST.in.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1484 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/skeleton/README.rst.tmpl
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       97 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      593 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       24 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      190 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      203 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      248 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      248 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      248 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      425 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      378 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      180 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      221 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      747 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      215 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2030 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/setup.py.tmpl
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/skeleton/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       13 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2001 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      377 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1351 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/skeleton/tox.ini.tmpl
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/smoke_test/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1504 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1455 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/sobjects/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1364 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    12938 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/ldapparser.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    14419 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/notification.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5861 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/services.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8236 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/supervising.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/sobjects/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.082895 cubicweb-4.7.0/cubicweb/sobjects/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       13 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      441 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1030 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1052 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1154 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/sobjects/test/data/sobjects/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1079 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/data/sobjects/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4020 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/test/unittest_email.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3059 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/test/unittest_notification.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5404 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/sobjects/test/unittest_register_user.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5051 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/sobjects/test/unittest_supervising.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1994 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/tags.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/test/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.086895 cubicweb-4.7.0/cubicweb/test/data/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       31 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/data/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      441 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1030 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1109 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1128 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/hooks.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/views/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/views/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1024 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/entities/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/entities/__init__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/hooks/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/hooks/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        7 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/views.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      819 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1153 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      845 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      875 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       51 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/ccplugin.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      857 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      887 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      657 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      157 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      622 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1565 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1555 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/erqlexpr_on_ertype.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       77 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/lowered_etype.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/cubicweb/test/data/migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      835 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.0.3_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      835 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.0.4_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      835 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      855 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_common.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      847 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_repository.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      835 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/migration/0.1.2_Any.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      402 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/rqlexpr_on_computedrel.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1555 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/rqlexpr_on_ertype_read.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1401 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/rrqlexpr_on_attr.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1182 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/rrqlexpr_on_eetype.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4319 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/cubicweb/test/data/scripts/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      164 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/scripts/script1.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      168 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/scripts/script2.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      187 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/scripts/script3.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/cubicweb/test/data/server_migration/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/server_migration/2.10.2_Any.sql
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/server_migration/2.5.0_Any.sql
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data/server_migration/2.6.0_Any.sql
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      882 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      131 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data/uppered_rtype.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data-rewrite/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       16 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/bootstrap_cubes
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      441 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      664 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.090896 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        0 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       41 2021-09-01 09:36:34.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1516 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3723 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data-rewrite/schema.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/cubicweb/test/data_schemareader/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      732 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/data_schemareader/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2304 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_binary.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      404 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_crypto.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17592 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_cwconfig.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7457 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_cwctl.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    48020 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_entity.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4855 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_fast_drop_entities.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8357 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_mail.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7471 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_migration.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15441 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_predicates.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3879 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_repoapi.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5850 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_req.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    46300 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_rqlrewrite.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6503 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_rqlsuggestions.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    32589 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_rset.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6543 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_rtags.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    34435 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4047 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_toolsutils.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9658 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_uilib.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3202 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/test/unittest_vregistry.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3998 2024-01-16 10:36:25.000000 cubicweb-4.7.0/cubicweb/test/unittest_wfutils.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    16545 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/toolsutils.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3836 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/transaction.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    19530 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/uilib.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    12356 2024-04-03 11:58:45.000000 cubicweb-4.7.0/cubicweb/utils.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5113 2024-03-26 15:31:00.000000 cubicweb-4.7.0/cubicweb/wfutils.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1578 2024-02-05 14:10:08.000000 cubicweb-4.7.0/cubicweb/xy.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.018895 cubicweb-4.7.0/cubicweb.egg-info/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4250 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/PKG-INFO
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    53563 2024-04-03 11:58:51.000000 cubicweb-4.7.0/cubicweb.egg-info/SOURCES.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/dependency_links.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      117 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/entry_points.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        1 2021-11-04 14:45:29.000000 cubicweb-4.7.0/cubicweb.egg-info/not-zip-safe
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      500 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/requires.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        9 2024-04-03 11:58:50.000000 cubicweb-4.7.0/cubicweb.egg-info/top_level.txt
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/doc/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7511 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/4.0.0_how_to_migrate.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2811 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/Makefile
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/doc/_static/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    34494 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/_static/favicon.ico
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    34494 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/_static/favicon.ico.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9202 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/_static/logo-cubicweb.svg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9202 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/_static/logo-cubicweb.svg.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1681 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/announce.en.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1982 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/announce.fr.txt
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.094895 cubicweb-4.7.0/doc/api/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2251 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/api/__init__.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      181 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/api/appobject.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      830 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/cwvreg.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      491 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/dataimport.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       87 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/api/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2540 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/predicates.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/api/pyramid/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      249 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/auth.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      358 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/pyramid/bwcompat.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      613 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/pyramid/core.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      296 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/login.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      259 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/profile.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      200 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/session.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      289 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid/url_redirection.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      234 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/pyramid.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      144 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/api/req.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      140 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/api/rset.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      781 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/urlpublishing.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      393 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/urlrewrite.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      520 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/api/web.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/book/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    14655 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/MERGE_ME-tut-create-app.en.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7806 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/book/_maybe_to_integrate/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      225 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/_maybe_to_integrate/D050-architecture.en.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1286 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/_maybe_to_integrate/rss-xml.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      751 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/_maybe_to_integrate/template.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/book/additionnal_services/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      369 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/additionnal_services/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13562 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/additionnal_services/undo.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.098895 cubicweb-4.7.0/doc/book/admin/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2253 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/book/admin/backups.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5658 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/admin/config.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3879 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/create-instance.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3879 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/create-instance.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3396 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/cubicweb-ctl.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3396 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/cubicweb-ctl.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4034 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/deploy.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4034 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/deploy.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      409 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      409 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/index.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5265 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/instance-config.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5265 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/instance-config.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4825 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/admin/ldap.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      130 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/admin/multisources.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      366 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/admin/rql-logs.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2064 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/admin/setup.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2064 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/admin/setup.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3596 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/admin/site-config.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/annexes/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1893 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/annexes/depends.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3257 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/annexes/docstrings-conventions.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    16153 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/annexes/faq.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    16153 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/annexes/faq.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      234 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/annexes/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3481 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/annexes/mercurial.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/annexes/rql/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2115 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/annexes/rql/Graph-ex.gif
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1167 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/annexes/rql/debugging.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4697 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/annexes/rql/implementation.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      267 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/annexes/rql/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5570 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/annexes/rql/intro.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    27490 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/annexes/rql/language.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2703 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/annexes/rql/usecases.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2703 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/annexes/rql/usecases.rst.orig
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/devrepo/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2147 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/connections_pooler.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/devrepo/cubes/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2645 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/available-cubes.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      932 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/cc-newcube.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      208 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6827 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/layout.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6827 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/layout.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1967 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/cubes/what-is-a-cube.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4021 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/dataimport.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/devrepo/datamodel/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1389 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/baseschema.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6178 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/define-workflows.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    34880 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/definition.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      248 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1043 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/datamodel/metadata.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2940 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/debug_channels.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.102895 cubicweb-4.7.0/doc/book/devrepo/devcore/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       67 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/devcore/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1129 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/devcore/reqbase.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.106896 cubicweb-4.7.0/doc/book/devrepo/entityclasses/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5159 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/adapters.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7268 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/application-logic.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5285 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/data-as-objects.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      303 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1719 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/entityclasses/load-sort.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4399 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/fti.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      504 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9469 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/migration.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2668 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/profiling.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.106896 cubicweb-4.7.0/doc/book/devrepo/repo/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9731 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/repo/hooks.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      155 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/repo/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1087 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/book/devrepo/repo/notifications.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11467 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/book/devrepo/repo/sessions.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       75 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/devrepo/repo/tasks.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    21316 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/devrepo/testing.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    18289 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devrepo/vreg.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    18289 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devrepo/vreg.rst.orig
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.106896 cubicweb-4.7.0/doc/book/devweb/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      915 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/ajax.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      915 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/ajax.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3473 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/controllers.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3473 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/controllers.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      890 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/css.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      890 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/css.rst.orig
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.110895 cubicweb-4.7.0/doc/book/devweb/edition/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11979 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/dissection.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11979 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/dissection.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3955 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/editcontroller.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3955 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/editcontroller.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9905 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/examples.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9905 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/examples.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15506 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/form.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15506 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/form.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      286 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/edition/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      286 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/edition/index.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      698 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/facets.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      698 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/facets.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      675 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/httpcaching.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      675 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/httpcaching.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      392 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      392 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/index.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10057 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/internationalization.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10057 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/internationalization.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    14107 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/js.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    14107 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/js.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      265 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/property.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      265 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/property.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2017 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/publisher.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2017 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/publisher.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5119 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/request.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5119 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/request.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      709 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/resource.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      709 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/resource.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      454 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/rtags.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      454 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/rtags.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1418 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/searchbar.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1418 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/searchbar.rst.orig
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.110895 cubicweb-4.7.0/doc/book/devweb/views/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5889 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/basetemplates.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5889 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/basetemplates.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      701 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/baseviews.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      701 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/baseviews.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1291 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/boxes.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1291 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/boxes.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2320 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/breadcrumbs.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2320 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/breadcrumbs.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      657 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/idownloadable.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      657 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/idownloadable.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      476 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      476 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/index.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10179 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/primary.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10179 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/primary.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5991 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/reledit.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5991 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/reledit.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      521 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/startup.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      521 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/startup.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5919 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/table.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5919 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/table.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5506 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/urlpublish.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5506 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/urlpublish.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4192 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/views.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4192 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/views.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      347 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/wdoc.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      347 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/wdoc.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1703 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/views/xmlrss.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1703 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/devweb/views/xmlrss.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      947 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/devweb/warning.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.110895 cubicweb-4.7.0/doc/book/intro/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    10427 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/intro/concepts.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1369 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/intro/history.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      385 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/intro/index.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.114895 cubicweb-4.7.0/doc/book/pyramid/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1371 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/pyramid/auth.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1371 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/pyramid/auth.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1314 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/pyramid/ctl.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3771 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/pyramid/debug_toolbar.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3771 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/pyramid/debug_toolbar.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      844 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/book/pyramid/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1795 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/pyramid/quickstart.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1795 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/pyramid/quickstart.rst.orig
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5411 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/pyramid/settings.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5411 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/pyramid/settings.rst.orig
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.114895 cubicweb-4.7.0/doc/book/security/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8041 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/book/security/csrf.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8041 2024-04-03 11:36:43.000000 cubicweb-4.7.0/doc/book/security/csrf.rst.orig
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.114895 cubicweb-4.7.0/doc/book/src/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2930 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/src/archi_globale.dia
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1735 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/book/src/main_template_layout.dia
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.118896 cubicweb-4.7.0/doc/changes/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6619 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.14.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3904 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.15.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3647 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.16.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1815 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.17.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3632 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/changes/3.18.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6757 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.19.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3165 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.20.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2991 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.21.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3689 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.22.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2799 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.23.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4033 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.24.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4655 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.25.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      434 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.26.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6870 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.27.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2656 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/changes/3.28.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1249 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.29.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5588 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.30.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3683 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.31.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7979 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.32.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1728 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/3.32_reledit.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5635 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.33.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4524 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.34.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4849 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.35.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     4507 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.36.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5437 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.37.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8870 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/3.38.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6425 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.0.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      914 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.1.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      233 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.2.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2656 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.3.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      264 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.4.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      848 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.5.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1949 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.6.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      126 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/4.7.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      746 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/changes/changelog.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       99 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/changes/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7654 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/conf.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/images/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    98393 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/03-transitions-view_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    12650 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/breadcrumbs_header.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    85073 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_general_panel.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   124385 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_registry_content_panel.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   111325 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_registry_decisions_panel.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   134505 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_rql_panel.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   192629 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_rql_traceback_panel.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   107766 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_show_source.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    55625 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_show_source_link.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   126845 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_sql_panel.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    97343 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/debugtoolbar_traceback_source_link.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    57300 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/example-card-with-rql-directive.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    55168 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/images/example-card-with-rql-table-directive.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2277 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/facet_date_range.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6013 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/facet_has_image.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22016 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/facet_overview.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1873 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/facet_range.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    21685 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_00-login_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    30326 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_01-start_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    35859 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_02-cookie-values_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    33922 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_02-create-blog_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    28123 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_03-list-one-blog_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    82897 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_03-site-config-panel_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   119813 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_03-state-submitted_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    98393 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_03-transitions-view_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    34771 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_04-detail-one-blog_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    28345 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_05-list-two-blog_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    49230 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_06-add-relation-entryof_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    96838 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_06-main-template-logo_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    40383 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_07-detail-one-blogentry_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    30591 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_08-schema_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    33091 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_09-new-view-blogentry_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    42230 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/lax-book_10-blog-with-two-entries_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17757 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/main_template.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8674 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/main_template.svg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13842 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/main_template_layout.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    46411 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/primaryview_template.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    14758 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/primaryview_template.svg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22773 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/request_session.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7211 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/request_session.svg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    12030 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/server-class-diagram.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    62022 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_blog-form_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   105173 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    58500 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_blog-primary_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    42013 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_blogs-list_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   109769 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_form-generic-relations_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    65646 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_index_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    13605 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_index_gettext_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    88970 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_index_logged_in_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    11548 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_login-form_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   100347 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    63097 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-community-custom-primary_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    62431 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-community-default-primary_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    74856 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    79709 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-custom-footer_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   128406 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-schema_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    71500 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_myblog-siteinfo_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   104834 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_schema_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    22098 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_schema_graphviz_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   150520 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/images/tutos-base_siteconfig_en.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    60672 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_admin.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    61388 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_city_created.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    50694 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_city_creation.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    71561 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_data_model_schema.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    48896 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_empty_instance.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    55671 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_finished_import.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    57063 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_list_view.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    70893 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_museum_created.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    61656 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_museum_creation.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    74005 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_museum_with_city_name.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   225824 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_react_map.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    53544 2022-08-09 14:03:17.000000 cubicweb-4.7.0/doc/images/tutos-museum_with_schema.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   354637 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_background-image.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    30437 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_boxes.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    54643 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_breadcrumbs.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   324086 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_facets.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    40520 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_grey-box.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    16843 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_index-after.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    26875 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_index-before.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17580 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_login-box.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    57814 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_prevnext.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    81362 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_ui1.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    93291 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_ui2.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)   290338 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/tutos-photowebsite_ui3.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    43051 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/undo_history-view_w600.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    26036 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/undo_mesage_w600.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    39625 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/undo_startup-link_w600.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17558 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/views-table-filter-shadow.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    14013 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/views-table-filter.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    12375 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/views-table-shadow.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9676 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/images/views-table.png
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7344 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2011 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/plan_formation_python_cubicweb.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      139 2021-04-20 14:56:24.000000 cubicweb-4.7.0/doc/stdlib.txt
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tools/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1462 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tools/generate_modules.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1624 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tools/mode_plan.py
+-rwxr-xr-x   0 schabot   (1000) schabot   (1000)     4944 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tools/pyjsrest.py
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/advanced/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      604 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/advanced/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5486 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/advanced/part01_create-cube.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    17016 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/advanced/part02_security.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5614 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/advanced/part03_bfss.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15384 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/advanced/part04_ui-base.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    15114 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/advanced/part05_ui-advanced.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/base/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3867 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/base/blog-in-five-minutes.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      675 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/base/conclusion.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    20435 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/base/customizing-the-application.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7821 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/base/discovering-the-ui.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1340 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/base/index.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/dataimport/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9014 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/dataimport/diseasome_import.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3336 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/dataimport/diseasome_parser.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)    29917 2021-09-01 09:36:34.000000 cubicweb-4.7.0/doc/tutorials/dataimport/index.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6576 2024-01-16 10:36:25.000000 cubicweb-4.7.0/doc/tutorials/dataimport/schema.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      568 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/index.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/doc/tutorials/museum/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     5961 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/data-management.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     6403 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/develop-app.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3860 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/develop-ui.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     8840 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/enhance-views.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     2702 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/getting-started.rst
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     1595 2024-04-03 11:58:45.000000 cubicweb-4.7.0/doc/tutorials/museum/index.rst
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/extras/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3545 2021-09-01 09:36:34.000000 cubicweb-4.7.0/extras/cubicweb-ctl.bash_completion
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     7414 2021-04-20 14:56:24.000000 cubicweb-4.7.0/jshintrc
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.134896 cubicweb-4.7.0/man/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      651 2024-01-16 10:36:25.000000 cubicweb-4.7.0/man/cubicweb-ctl.1
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       56 2024-01-16 10:36:25.000000 cubicweb-4.7.0/mypy.ini
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      536 2021-09-01 09:36:34.000000 cubicweb-4.7.0/pylintrc
+drwxr-xr-x   0 schabot   (1000) schabot   (1000)        0 2024-04-03 11:58:52.138896 cubicweb-4.7.0/requirements/
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      174 2024-04-03 11:58:45.000000 cubicweb-4.7.0/requirements/dev.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      310 2024-04-03 11:58:45.000000 cubicweb-4.7.0/requirements/doc.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      377 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/from-forge.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      380 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-base.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       16 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-dataimport.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       15 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-devtools.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)        9 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-ext.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       39 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-hooks.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      128 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-pyramid.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)       35 2024-01-16 10:36:25.000000 cubicweb-4.7.0/requirements/test-server.txt
+-rw-r--r--   0 schabot   (1000) schabot   (1000)      115 2024-04-03 11:58:52.138896 cubicweb-4.7.0/setup.cfg
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     3279 2024-04-03 11:58:45.000000 cubicweb-4.7.0/setup.py
+-rw-r--r--   0 schabot   (1000) schabot   (1000)     9036 2024-04-03 11:58:45.000000 cubicweb-4.7.0/tox.ini
```

### Comparing `cubicweb-4.6.4/CONTRIBUTING.rst` & `cubicweb-4.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/COPYING` & `cubicweb-4.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/COPYING.LESSER` & `cubicweb-4.7.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/MANIFEST.in` & `cubicweb-4.7.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/README.rst` & `cubicweb-4.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/__init__.py` & `cubicweb-4.7.0/cubicweb/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/__pkginfo__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """cubicweb global packaging information for the cubicweb knowledge management
 software
 """
 
 modname = distname = "cubicweb"
 
-numversion = (4, 6, 4)
+numversion = (4, 7, 0)
 version = ".".join(str(num) for num in numversion)
 
 description = "a repository of entities / relations for knowledge management"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = "https://www.cubicweb.org"
 license = "LGPL"
```

### Comparing `cubicweb-4.6.4/cubicweb/_exceptions.py` & `cubicweb-4.7.0/cubicweb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/_gcdebug.py` & `cubicweb-4.7.0/cubicweb/_gcdebug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/appobject.py` & `cubicweb-4.7.0/cubicweb/appobject.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/crypto.py` & `cubicweb-4.7.0/cubicweb/crypto.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/cwconfig.py` & `cubicweb-4.7.0/cubicweb/cwconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/cwctl.py` & `cubicweb-4.7.0/cubicweb/cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/cwgettext.py` & `cubicweb-4.7.0/cubicweb/cwgettext.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/cwvreg.py` & `cubicweb-4.7.0/cubicweb/cwvreg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/__init__.py` & `cubicweb-4.7.0/cubicweb/dataimport/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/csv.py` & `cubicweb-4.7.0/cubicweb/dataimport/csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/importer.py` & `cubicweb-4.7.0/cubicweb/dataimport/importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/massive_store.py` & `cubicweb-4.7.0/cubicweb/dataimport/massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/pgstore.py` & `cubicweb-4.7.0/cubicweb/dataimport/pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/stores.py` & `cubicweb-4.7.0/cubicweb/dataimport/stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/data/geonames.csv` & `cubicweb-4.7.0/cubicweb/dataimport/test/data/geonames.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/data/schema.py` & `cubicweb-4.7.0/cubicweb/dataimport/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/data/timeZones.txt` & `cubicweb-4.7.0/cubicweb/dataimport/test/data/timeZones.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/data-massimport/schema.py` & `cubicweb-4.7.0/cubicweb/dataimport/test/data-massimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/test_csv.py` & `cubicweb-4.7.0/cubicweb/dataimport/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/test_massive_store.py` & `cubicweb-4.7.0/cubicweb/dataimport/test/test_massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/test_pgstore.py` & `cubicweb-4.7.0/cubicweb/dataimport/test/test_pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/test_stores.py` & `cubicweb-4.7.0/cubicweb/dataimport/test/test_stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/dataimport/test/unittest_importer.py` & `cubicweb-4.7.0/cubicweb/dataimport/test/unittest_importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/debug.py` & `cubicweb-4.7.0/cubicweb/debug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/__init__.py` & `cubicweb-4.7.0/cubicweb/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/apptest_config.py` & `cubicweb-4.7.0/cubicweb/devtools/apptest_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/data/qunit.css` & `cubicweb-4.7.0/cubicweb/devtools/data/qunit.css`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/data/qunit.js` & `cubicweb-4.7.0/cubicweb/devtools/data/qunit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/devctl.py` & `cubicweb-4.7.0/cubicweb/devtools/devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/fake.py` & `cubicweb-4.7.0/cubicweb/devtools/fake.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/fill.py` & `cubicweb-4.7.0/cubicweb/devtools/fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/fix_po_encoding` & `cubicweb-4.7.0/cubicweb/devtools/fix_po_encoding`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/htmlparser.py` & `cubicweb-4.7.0/cubicweb/devtools/htmlparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/httptest.py` & `cubicweb-4.7.0/cubicweb/devtools/httptest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/instrument.py` & `cubicweb-4.7.0/cubicweb/devtools/instrument.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/realdbtest.py` & `cubicweb-4.7.0/cubicweb/devtools/realdbtest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/repotest.py` & `cubicweb-4.7.0/cubicweb/devtools/repotest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/stresstester.py` & `cubicweb-4.7.0/cubicweb/devtools/stresstester.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/data/firstnames.txt` & `cubicweb-4.7.0/cubicweb/devtools/test/data/firstnames.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref` & `cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py` & `cubicweb-4.7.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/data/schema.py` & `cubicweb-4.7.0/cubicweb/devtools/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/data/static/js_examples/utils.js` & `cubicweb-4.7.0/cubicweb/devtools/test/data/static/js_examples/utils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/unittest_dbfill.py` & `cubicweb-4.7.0/cubicweb/devtools/test/unittest_dbfill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/unittest_devctl.py` & `cubicweb-4.7.0/cubicweb/devtools/test/unittest_devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/unittest_fill.py` & `cubicweb-4.7.0/cubicweb/devtools/test/unittest_fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/unittest_i18n.py` & `cubicweb-4.7.0/cubicweb/devtools/test/unittest_i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/test/unittest_testlib.py` & `cubicweb-4.7.0/cubicweb/devtools/test/unittest_testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/devtools/testlib.py` & `cubicweb-4.7.0/cubicweb/devtools/testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/__init__.py` & `cubicweb-4.7.0/cubicweb/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/adapters.py` & `cubicweb-4.7.0/cubicweb/entities/adapters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/authobjs.py` & `cubicweb-4.7.0/cubicweb/entities/authobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/lib.py` & `cubicweb-4.7.0/cubicweb/entities/lib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/schemaobjs.py` & `cubicweb-4.7.0/cubicweb/entities/schemaobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/sources.py` & `cubicweb-4.7.0/cubicweb/entities/sources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/test/data/migration/postcreate.py` & `cubicweb-4.7.0/cubicweb/entities/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/test/data/schema.py` & `cubicweb-4.7.0/cubicweb/entities/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/test/unittest_base.py` & `cubicweb-4.7.0/cubicweb/entities/test/unittest_base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/test/unittest_wfobjs.py` & `cubicweb-4.7.0/cubicweb/entities/test/unittest_wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entities/wfobjs.py` & `cubicweb-4.7.0/cubicweb/entities/wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/entity.py` & `cubicweb-4.7.0/cubicweb/entity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2024 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of CubicWeb.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -518,23 +518,27 @@
         ...                              works_for=c)
 
         You can also set relations where the entity has 'object' role by
         prefixing the relation name by 'reverse_'. Also, relation values may be
         an entity or eid, a list of entities or eids.
         """
         rql, qargs, pendingrels, attrcache = cls._cw_build_entity_query(kwargs)
+        assert isinstance(rql, str)
+        entity_type = cls.__regid__
+        assert entity_type
         if rql:
-            rql = f"INSERT {cls.__regid__} X: {rql}"
+            rql = f"INSERT {entity_type} X: {rql}"
         else:
-            rql = f"INSERT {cls.__regid__} X"
+            rql = f"INSERT {entity_type} X"
+
         try:
             created = execute(rql, qargs).get_entity(0, 0)
         except IndexError:
             raise Exception(
-                f"could not create a {cls.__regid__!r} with {rql!r} ({qargs!r})"
+                f"could not create a {entity_type!r} with {rql!r} ({qargs!r})"
             )
         created._cw_update_attr_cache(attrcache)
         cls._cw_handle_pending_relations(created.eid, pendingrels, execute)
         return created
 
     def __init__(self, req, rset=None, row=None, col=0):
         AppObject.__init__(self, req, rset=rset, row=row, col=col)
```

### Comparing `cubicweb-4.6.4/cubicweb/ext/__init__.py` & `cubicweb-4.7.0/cubicweb/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/ext/html4zope.py` & `cubicweb-4.7.0/cubicweb/ext/html4zope.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/ext/markdown.py` & `cubicweb-4.7.0/cubicweb/ext/markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/ext/test/unittest_markdown.py` & `cubicweb-4.7.0/cubicweb/ext/test/unittest_markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/__init__.py` & `cubicweb-4.7.0/cubicweb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/bookmark.py` & `cubicweb-4.7.0/cubicweb/hooks/bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/email.py` & `cubicweb-4.7.0/cubicweb/hooks/email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/integrity.py` & `cubicweb-4.7.0/cubicweb/hooks/integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/metadata.py` & `cubicweb-4.7.0/cubicweb/hooks/metadata.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/notification.py` & `cubicweb-4.7.0/cubicweb/hooks/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/security.py` & `cubicweb-4.7.0/cubicweb/hooks/security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/synccomputed.py` & `cubicweb-4.7.0/cubicweb/hooks/synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/syncschema.py` & `cubicweb-4.7.0/cubicweb/hooks/syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/syncsession.py` & `cubicweb-4.7.0/cubicweb/hooks/syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/syncsources.py` & `cubicweb-4.7.0/cubicweb/hooks/syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/data/schema.py` & `cubicweb-4.7.0/cubicweb/hooks/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/data-computed/schema.py` & `cubicweb-4.7.0/cubicweb/hooks/test/data-computed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_bookmarks.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_bookmarks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_hooks.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_integrity.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_notificationhooks.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_notificationhooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_security.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_synccomputed.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_syncschema.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_syncsession.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/test/unittest_syncsources.py` & `cubicweb-4.7.0/cubicweb/hooks/test/unittest_syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/hooks/workflow.py` & `cubicweb-4.7.0/cubicweb/hooks/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/i18n/de.po` & `cubicweb-4.7.0/cubicweb/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/i18n/en.po` & `cubicweb-4.7.0/cubicweb/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/i18n/es.po` & `cubicweb-4.7.0/cubicweb/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/i18n/fr.po` & `cubicweb-4.7.0/cubicweb/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/i18n.py` & `cubicweb-4.7.0/cubicweb/i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/mail.py` & `cubicweb-4.7.0/cubicweb/mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/md5crypt.py` & `cubicweb-4.7.0/cubicweb/md5crypt.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/migration.py` & `cubicweb-4.7.0/cubicweb/migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/migration/3.22.0_Any.py` & `cubicweb-4.7.0/cubicweb/misc/migration/3.22.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/migration/3.23.0_Any.py` & `cubicweb-4.7.0/cubicweb/misc/migration/3.23.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/migration/3.24.0_Any.py` & `cubicweb-4.7.0/cubicweb/misc/migration/3.24.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/migration/3.24.4_Any.py` & `cubicweb-4.7.0/cubicweb/misc/migration/3.24.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/migration/bootstrapmigration_repository.py` & `cubicweb-4.7.0/cubicweb/misc/migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/migration/postcreate.py` & `cubicweb-4.7.0/cubicweb/misc/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/scripts/chpasswd.py` & `cubicweb-4.7.0/cubicweb/misc/scripts/chpasswd.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/scripts/fast_drop_entities.py` & `cubicweb-4.7.0/cubicweb/misc/scripts/fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/scripts/ldap_change_base_dn.py` & `cubicweb-4.7.0/cubicweb/misc/scripts/ldap_change_base_dn.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/scripts/migration_helper.py` & `cubicweb-4.7.0/cubicweb/misc/scripts/migration_helper.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/misc/source_highlight.py` & `cubicweb-4.7.0/cubicweb/misc/source_highlight.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/mttransforms.py` & `cubicweb-4.7.0/cubicweb/mttransforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/multipart.py` & `cubicweb-4.7.0/cubicweb/multipart.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/predicates.py` & `cubicweb-4.7.0/cubicweb/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/__init__.py` & `cubicweb-4.7.0/cubicweb/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/auth.py` & `cubicweb-4.7.0/cubicweb/pyramid/auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/config.py` & `cubicweb-4.7.0/cubicweb/pyramid/config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/core.py` & `cubicweb-4.7.0/cubicweb/pyramid/core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/csrf.py` & `cubicweb-4.7.0/cubicweb/pyramid/csrf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/debug_source_code.py` & `cubicweb-4.7.0/cubicweb/pyramid/debug_source_code.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako` & `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako` & `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako` & `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako` & `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako` & `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako` & `cubicweb-4.7.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/debugtoolbar_panels.py` & `cubicweb-4.7.0/cubicweb/pyramid/debugtoolbar_panels.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/default_session.py` & `cubicweb-4.7.0/cubicweb/pyramid/default_session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/development.ini.tmpl` & `cubicweb-4.7.0/cubicweb/pyramid/development.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/predicates.py` & `cubicweb-4.7.0/cubicweb/pyramid/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/pyramid.ini.tmpl` & `cubicweb-4.7.0/cubicweb/pyramid/pyramid.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/pyramidctl.py` & `cubicweb-4.7.0/cubicweb/pyramid/pyramidctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/resources.py` & `cubicweb-4.7.0/cubicweb/pyramid/resources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/rest_api.py` & `cubicweb-4.7.0/cubicweb/pyramid/rest_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/session.py` & `cubicweb-4.7.0/cubicweb/pyramid/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/test/__init__.py` & `cubicweb-4.7.0/cubicweb/pyramid/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/test/data/cubicweb_blog/schema.py` & `cubicweb-4.7.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/test/test_auth.py` & `cubicweb-4.7.0/cubicweb/pyramid/test/test_auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/test/test_config.py` & `cubicweb-4.7.0/cubicweb/pyramid/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/test/test_content_negociation.py` & `cubicweb-4.7.0/cubicweb/pyramid/test/test_content_negociation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/test/test_core.py` & `cubicweb-4.7.0/cubicweb/pyramid/test/test_core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/test/test_tools.py` & `cubicweb-4.7.0/cubicweb/pyramid/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pyramid/tools.py` & `cubicweb-4.7.0/cubicweb/pyramid/tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/pytestconf.py` & `cubicweb-4.7.0/cubicweb/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/rdf.py` & `cubicweb-4.7.0/cubicweb/rdf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/repoapi.py` & `cubicweb-4.7.0/cubicweb/repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/req.py` & `cubicweb-4.7.0/cubicweb/req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/rqlrewrite.py` & `cubicweb-4.7.0/cubicweb/rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/rqlsuggestions.py` & `cubicweb-4.7.0/cubicweb/rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/rset.py` & `cubicweb-4.7.0/cubicweb/rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/rtags.py` & `cubicweb-4.7.0/cubicweb/rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/schema.py` & `cubicweb-4.7.0/cubicweb/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/schema_exporters.py` & `cubicweb-4.7.0/cubicweb/schema_exporters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/schemas/Bookmark.py` & `cubicweb-4.7.0/cubicweb/schemas/Bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/schemas/__init__.py` & `cubicweb-4.7.0/cubicweb/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/schemas/_regproc.postgres.sql` & `cubicweb-4.7.0/cubicweb/schemas/_regproc.postgres.sql`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/schemas/base.py` & `cubicweb-4.7.0/cubicweb/schemas/base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/schemas/bootstrap.py` & `cubicweb-4.7.0/cubicweb/schemas/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/schemas/workflow.py` & `cubicweb-4.7.0/cubicweb/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/__init__.py` & `cubicweb-4.7.0/cubicweb/server/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/check_unused_index.py` & `cubicweb-4.7.0/cubicweb/server/check_unused_index.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/checkintegrity.py` & `cubicweb-4.7.0/cubicweb/server/checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/edition.py` & `cubicweb-4.7.0/cubicweb/server/edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/hook.py` & `cubicweb-4.7.0/cubicweb/server/hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/migractions.py` & `cubicweb-4.7.0/cubicweb/server/migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/querier.py` & `cubicweb-4.7.0/cubicweb/server/querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/repository.py` & `cubicweb-4.7.0/cubicweb/server/repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/rqlannotation.py` & `cubicweb-4.7.0/cubicweb/server/rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/schema2sql.py` & `cubicweb-4.7.0/cubicweb/server/schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/schemaserial.py` & `cubicweb-4.7.0/cubicweb/server/schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/serverconfig.py` & `cubicweb-4.7.0/cubicweb/server/serverconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/serverctl.py` & `cubicweb-4.7.0/cubicweb/server/serverctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/session.py` & `cubicweb-4.7.0/cubicweb/server/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/sources/__init__.py` & `cubicweb-4.7.0/cubicweb/server/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/sources/datafeed.py` & `cubicweb-4.7.0/cubicweb/server/sources/datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/sources/ldapfeed.py` & `cubicweb-4.7.0/cubicweb/server/sources/ldapfeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/sources/native.py` & `cubicweb-4.7.0/cubicweb/server/sources/native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/sources/rql2sql.py` & `cubicweb-4.7.0/cubicweb/server/sources/rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/sources/storages.py` & `cubicweb-4.7.0/cubicweb/server/sources/storages.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/sqlutils.py` & `cubicweb-4.7.0/cubicweb/server/sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/ssplanner.py` & `cubicweb-4.7.0/cubicweb/server/ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/entities.py` & `cubicweb-4.7.0/cubicweb/server/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/hooks.py` & `cubicweb-4.7.0/cubicweb/server/test/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/ldap_test.ldif` & `cubicweb-4.7.0/cubicweb/server/test/data/ldap_test.ldif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/migration/postcreate.py` & `cubicweb-4.7.0/cubicweb/server/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data/slapd.conf.in` & `cubicweb-4.7.0/cubicweb/server/test/data/slapd.conf.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-cwep002/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-cwep002/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/__init__.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/migratedapp/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-migractions/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/Company.py` & `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/Company.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/Dates.py` & `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/Dates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/State.py` & `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/State.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/__init__.py` & `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-schema2sql/schema/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-schema2sql/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-schemaserial/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/data-schemaserial/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/datacomputed/migratedapp/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/datacomputed/schema.py` & `cubicweb-4.7.0/cubicweb/server/test/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_datafeed.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_edition.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_hook.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_ldapsource.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_ldapsource.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_querier.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_rql2sql.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_rqlannotation.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_schema2sql.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_schemaserial.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_server_security.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_server_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_server_utils.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_server_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_serverctl.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_serverctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_session.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_sources_native.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_sources_native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_sqlutils.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_ssplanner.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_storage.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_storage.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_tools.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_undo.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_undo.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test/unittest_utils.py` & `cubicweb-4.7.0/cubicweb/server/test/unittest_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/entities.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/hooks.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/migration/postcreate.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/data/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py` & `cubicweb-4.7.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/entities.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/hooks.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/migration/postcreate.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/data-migractions/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/datacomputed/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions/unittest_migractions.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/entities.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/hooks.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/migration/postcreate.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/data-migractions/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/datacomputed/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions2/unittest_migractions.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions2/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/entities.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/hooks.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/migration/postcreate.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/data-migractions/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/datacomputed/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_migractions3/unittest_migractions.py` & `cubicweb-4.7.0/cubicweb/server/test_migractions3/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/entities.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/hooks.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/migration/postcreate.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/data/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_postgres/unittest_postgres.py` & `cubicweb-4.7.0/cubicweb/server/test_postgres/unittest_postgres.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_basket/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_file/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/entities.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/hooks.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data-schemaserial/schema.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/test_repository/unittest_repository.py` & `cubicweb-4.7.0/cubicweb/server/test_repository/unittest_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/server/utils.py` & `cubicweb-4.7.0/cubicweb/server/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/skeleton/.gitlab-ci.yml.tmpl` & `cubicweb-4.7.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/skeleton/README.rst.tmpl` & `cubicweb-4.7.0/cubicweb/skeleton/README.rst.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl` & `cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl` & `cubicweb-4.7.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/skeleton/setup.py.tmpl` & `cubicweb-4.7.0/cubicweb/skeleton/setup.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/skeleton/test/realdb_test_CUBENAME.py` & `cubicweb-4.7.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/skeleton/tox.ini.tmpl` & `cubicweb-4.7.0/cubicweb/skeleton/tox.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py` & `cubicweb-4.7.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py` & `cubicweb-4.7.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/__init__.py` & `cubicweb-4.7.0/cubicweb/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/ldapparser.py` & `cubicweb-4.7.0/cubicweb/sobjects/ldapparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/notification.py` & `cubicweb-4.7.0/cubicweb/sobjects/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/services.py` & `cubicweb-4.7.0/cubicweb/sobjects/services.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/supervising.py` & `cubicweb-4.7.0/cubicweb/sobjects/supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/data/schema.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/data/sobjects/__init__.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/data/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/unittest_email.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/unittest_email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/unittest_notification.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/unittest_notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/unittest_register_user.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/unittest_register_user.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/sobjects/test/unittest_supervising.py` & `cubicweb-4.7.0/cubicweb/sobjects/test/unittest_supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/tags.py` & `cubicweb-4.7.0/cubicweb/tags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_comment/schema.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/__init__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_email/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/__init__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_file/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_forge/__init__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_forge/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_mycube/__init__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_required_variables/__init__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/cubicweb_tag/schema.py` & `cubicweb-4.7.0/cubicweb/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/entities.py` & `cubicweb-4.7.0/cubicweb/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/erqlexpr_on_ertype.py` & `cubicweb-4.7.0/cubicweb/test/data/erqlexpr_on_ertype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/migration/0.0.3_Any.py` & `cubicweb-4.7.0/cubicweb/test/data/migration/0.0.3_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/migration/0.0.4_Any.py` & `cubicweb-4.7.0/cubicweb/test/data/migration/0.0.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/migration/0.1.0_Any.py` & `cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/migration/0.1.0_common.py` & `cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_common.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/migration/0.1.0_repository.py` & `cubicweb-4.7.0/cubicweb/test/data/migration/0.1.0_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/migration/0.1.2_Any.py` & `cubicweb-4.7.0/cubicweb/test/data/migration/0.1.2_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/rqlexpr_on_ertype_read.py` & `cubicweb-4.7.0/cubicweb/test/data/rqlexpr_on_ertype_read.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/rrqlexpr_on_attr.py` & `cubicweb-4.7.0/cubicweb/test/data/rrqlexpr_on_attr.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/rrqlexpr_on_eetype.py` & `cubicweb-4.7.0/cubicweb/test/data/rrqlexpr_on_eetype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/schema.py` & `cubicweb-4.7.0/cubicweb/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data/server_migration/bootstrapmigration_repository.py` & `cubicweb-4.7.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_card/schema.py` & `cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py` & `cubicweb-4.7.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data-rewrite/schema.py` & `cubicweb-4.7.0/cubicweb/test/data-rewrite/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/data_schemareader/schema.py` & `cubicweb-4.7.0/cubicweb/test/data_schemareader/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_binary.py` & `cubicweb-4.7.0/cubicweb/test/unittest_binary.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_cwconfig.py` & `cubicweb-4.7.0/cubicweb/test/unittest_cwconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_cwctl.py` & `cubicweb-4.7.0/cubicweb/test/unittest_cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_entity.py` & `cubicweb-4.7.0/cubicweb/test/unittest_entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_fast_drop_entities.py` & `cubicweb-4.7.0/cubicweb/test/unittest_fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_mail.py` & `cubicweb-4.7.0/cubicweb/test/unittest_mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_migration.py` & `cubicweb-4.7.0/cubicweb/test/unittest_migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_predicates.py` & `cubicweb-4.7.0/cubicweb/test/unittest_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_repoapi.py` & `cubicweb-4.7.0/cubicweb/test/unittest_repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_req.py` & `cubicweb-4.7.0/cubicweb/test/unittest_req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_rqlrewrite.py` & `cubicweb-4.7.0/cubicweb/test/unittest_rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_rqlsuggestions.py` & `cubicweb-4.7.0/cubicweb/test/unittest_rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_rset.py` & `cubicweb-4.7.0/cubicweb/test/unittest_rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_rtags.py` & `cubicweb-4.7.0/cubicweb/test/unittest_rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_schema.py` & `cubicweb-4.7.0/cubicweb/test/unittest_schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_toolsutils.py` & `cubicweb-4.7.0/cubicweb/test/unittest_toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_uilib.py` & `cubicweb-4.7.0/cubicweb/test/unittest_uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_vregistry.py` & `cubicweb-4.7.0/cubicweb/test/unittest_vregistry.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/test/unittest_wfutils.py` & `cubicweb-4.7.0/cubicweb/test/unittest_wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/toolsutils.py` & `cubicweb-4.7.0/cubicweb/toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/transaction.py` & `cubicweb-4.7.0/cubicweb/transaction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/uilib.py` & `cubicweb-4.7.0/cubicweb/uilib.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 from io import StringIO
 from datetime import timedelta
 from functools import wraps
 
 from logilab.common.date import ustrftime
 from logilab.mtconverter import xml_escape, html_unescape
 from lxml import etree
-from lxml.html import defs, clean
+from lxml.html import defs
+from lxml_html_clean import Cleaner
 
 from cubicweb import _
 from cubicweb.utils import js_dumps
 from cubicweb.ext.markdown import markdown_publish  # noqa
 
 
 def rql_for_eid(eid):
@@ -242,15 +243,15 @@
     | defs.list_tags
     | defs.table_tags
     | defs.phrase_tags
     | defs.font_style_tags
     | {"span", "a", "br", "img", "map", "area", "sub", "sup", "canvas"}
 )
 
-CLEANER = clean.Cleaner(
+CLEANER = Cleaner(
     allow_tags=ALLOWED_TAGS,
     remove_unknown_tags=False,
     style=True,
     safe_attrs_only=True,
     add_nofollow=False,
 )
```

### Comparing `cubicweb-4.6.4/cubicweb/utils.py` & `cubicweb-4.7.0/cubicweb/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/wfutils.py` & `cubicweb-4.7.0/cubicweb/wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb/xy.py` & `cubicweb-4.7.0/cubicweb/xy.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/cubicweb.egg-info/SOURCES.txt` & `cubicweb-4.7.0/cubicweb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -773,15 +773,17 @@
 doc/announce.en.txt
 doc/announce.fr.txt
 doc/conf.py
 doc/index.rst
 doc/plan_formation_python_cubicweb.txt
 doc/stdlib.txt
 doc/_static/favicon.ico
+doc/_static/favicon.ico.orig
 doc/_static/logo-cubicweb.svg
+doc/_static/logo-cubicweb.svg.orig
 doc/api/__init__.rst
 doc/api/appobject.rst
 doc/api/cwvreg.rst
 doc/api/dataimport.rst
 doc/api/index.rst
 doc/api/predicates.rst
 doc/api/pyramid.rst
@@ -803,48 +805,58 @@
 doc/book/_maybe_to_integrate/rss-xml.rst
 doc/book/_maybe_to_integrate/template.rst
 doc/book/additionnal_services/index.rst
 doc/book/additionnal_services/undo.rst
 doc/book/admin/backups.rst
 doc/book/admin/config.rst
 doc/book/admin/create-instance.rst
+doc/book/admin/create-instance.rst.orig
 doc/book/admin/cubicweb-ctl.rst
+doc/book/admin/cubicweb-ctl.rst.orig
 doc/book/admin/deploy.rst
+doc/book/admin/deploy.rst.orig
 doc/book/admin/index.rst
+doc/book/admin/index.rst.orig
 doc/book/admin/instance-config.rst
+doc/book/admin/instance-config.rst.orig
 doc/book/admin/ldap.rst
 doc/book/admin/multisources.rst
 doc/book/admin/rql-logs.rst
 doc/book/admin/setup.rst
+doc/book/admin/setup.rst.orig
 doc/book/admin/site-config.rst
 doc/book/annexes/depends.rst
 doc/book/annexes/docstrings-conventions.rst
 doc/book/annexes/faq.rst
+doc/book/annexes/faq.rst.orig
 doc/book/annexes/index.rst
 doc/book/annexes/mercurial.rst
 doc/book/annexes/rql/Graph-ex.gif
 doc/book/annexes/rql/debugging.rst
 doc/book/annexes/rql/implementation.rst
 doc/book/annexes/rql/index.rst
 doc/book/annexes/rql/intro.rst
 doc/book/annexes/rql/language.rst
 doc/book/annexes/rql/usecases.rst
+doc/book/annexes/rql/usecases.rst.orig
 doc/book/devrepo/connections_pooler.rst
 doc/book/devrepo/dataimport.rst
 doc/book/devrepo/debug_channels.rst
 doc/book/devrepo/fti.rst
 doc/book/devrepo/index.rst
 doc/book/devrepo/migration.rst
 doc/book/devrepo/profiling.rst
 doc/book/devrepo/testing.rst
 doc/book/devrepo/vreg.rst
+doc/book/devrepo/vreg.rst.orig
 doc/book/devrepo/cubes/available-cubes.rst
 doc/book/devrepo/cubes/cc-newcube.rst
 doc/book/devrepo/cubes/index.rst
 doc/book/devrepo/cubes/layout.rst
+doc/book/devrepo/cubes/layout.rst.orig
 doc/book/devrepo/cubes/what-is-a-cube.rst
 doc/book/devrepo/datamodel/baseschema.rst
 doc/book/devrepo/datamodel/define-workflows.rst
 doc/book/devrepo/datamodel/definition.rst
 doc/book/devrepo/datamodel/index.rst
 doc/book/devrepo/datamodel/metadata.rst
 doc/book/devrepo/devcore/index.rst
@@ -856,57 +868,95 @@
 doc/book/devrepo/entityclasses/load-sort.rst
 doc/book/devrepo/repo/hooks.rst
 doc/book/devrepo/repo/index.rst
 doc/book/devrepo/repo/notifications.rst
 doc/book/devrepo/repo/sessions.rst
 doc/book/devrepo/repo/tasks.rst
 doc/book/devweb/ajax.rst
+doc/book/devweb/ajax.rst.orig
 doc/book/devweb/controllers.rst
+doc/book/devweb/controllers.rst.orig
 doc/book/devweb/css.rst
+doc/book/devweb/css.rst.orig
 doc/book/devweb/facets.rst
+doc/book/devweb/facets.rst.orig
 doc/book/devweb/httpcaching.rst
+doc/book/devweb/httpcaching.rst.orig
 doc/book/devweb/index.rst
+doc/book/devweb/index.rst.orig
 doc/book/devweb/internationalization.rst
+doc/book/devweb/internationalization.rst.orig
 doc/book/devweb/js.rst
+doc/book/devweb/js.rst.orig
 doc/book/devweb/property.rst
+doc/book/devweb/property.rst.orig
 doc/book/devweb/publisher.rst
+doc/book/devweb/publisher.rst.orig
 doc/book/devweb/request.rst
+doc/book/devweb/request.rst.orig
 doc/book/devweb/resource.rst
+doc/book/devweb/resource.rst.orig
 doc/book/devweb/rtags.rst
+doc/book/devweb/rtags.rst.orig
 doc/book/devweb/searchbar.rst
+doc/book/devweb/searchbar.rst.orig
 doc/book/devweb/warning.rst
 doc/book/devweb/edition/dissection.rst
+doc/book/devweb/edition/dissection.rst.orig
 doc/book/devweb/edition/editcontroller.rst
+doc/book/devweb/edition/editcontroller.rst.orig
 doc/book/devweb/edition/examples.rst
+doc/book/devweb/edition/examples.rst.orig
 doc/book/devweb/edition/form.rst
+doc/book/devweb/edition/form.rst.orig
 doc/book/devweb/edition/index.rst
+doc/book/devweb/edition/index.rst.orig
 doc/book/devweb/views/basetemplates.rst
+doc/book/devweb/views/basetemplates.rst.orig
 doc/book/devweb/views/baseviews.rst
+doc/book/devweb/views/baseviews.rst.orig
 doc/book/devweb/views/boxes.rst
+doc/book/devweb/views/boxes.rst.orig
 doc/book/devweb/views/breadcrumbs.rst
+doc/book/devweb/views/breadcrumbs.rst.orig
 doc/book/devweb/views/idownloadable.rst
+doc/book/devweb/views/idownloadable.rst.orig
 doc/book/devweb/views/index.rst
+doc/book/devweb/views/index.rst.orig
 doc/book/devweb/views/primary.rst
+doc/book/devweb/views/primary.rst.orig
 doc/book/devweb/views/reledit.rst
+doc/book/devweb/views/reledit.rst.orig
 doc/book/devweb/views/startup.rst
+doc/book/devweb/views/startup.rst.orig
 doc/book/devweb/views/table.rst
+doc/book/devweb/views/table.rst.orig
 doc/book/devweb/views/urlpublish.rst
+doc/book/devweb/views/urlpublish.rst.orig
 doc/book/devweb/views/views.rst
+doc/book/devweb/views/views.rst.orig
 doc/book/devweb/views/wdoc.rst
+doc/book/devweb/views/wdoc.rst.orig
 doc/book/devweb/views/xmlrss.rst
+doc/book/devweb/views/xmlrss.rst.orig
 doc/book/intro/concepts.rst
 doc/book/intro/history.rst
 doc/book/intro/index.rst
 doc/book/pyramid/auth.rst
+doc/book/pyramid/auth.rst.orig
 doc/book/pyramid/ctl.rst
 doc/book/pyramid/debug_toolbar.rst
+doc/book/pyramid/debug_toolbar.rst.orig
 doc/book/pyramid/index.rst
 doc/book/pyramid/quickstart.rst
+doc/book/pyramid/quickstart.rst.orig
 doc/book/pyramid/settings.rst
+doc/book/pyramid/settings.rst.orig
 doc/book/security/csrf.rst
+doc/book/security/csrf.rst.orig
 doc/book/src/archi_globale.dia
 doc/book/src/main_template_layout.dia
 doc/changes/3.14.rst
 doc/changes/3.15.rst
 doc/changes/3.16.rst
 doc/changes/3.17.rst
 doc/changes/3.18.rst
@@ -934,14 +984,15 @@
 doc/changes/4.0.rst
 doc/changes/4.1.rst
 doc/changes/4.2.rst
 doc/changes/4.3.rst
 doc/changes/4.4.rst
 doc/changes/4.5.rst
 doc/changes/4.6.rst
+doc/changes/4.7.rst
 doc/changes/changelog.rst
 doc/changes/index.rst
 doc/images/03-transitions-view_en.png
 doc/images/breadcrumbs_header.png
 doc/images/debugtoolbar_general_panel.png
 doc/images/debugtoolbar_registry_content_panel.png
 doc/images/debugtoolbar_registry_decisions_panel.png
```

### Comparing `cubicweb-4.6.4/doc/4.0.0_how_to_migrate.rst` & `cubicweb-4.7.0/doc/4.0.0_how_to_migrate.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/Makefile` & `cubicweb-4.7.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/_static/favicon.ico` & `cubicweb-4.7.0/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/_static/logo-cubicweb.svg` & `cubicweb-4.7.0/doc/_static/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/announce.en.txt` & `cubicweb-4.7.0/doc/announce.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/announce.fr.txt` & `cubicweb-4.7.0/doc/announce.fr.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/api/__init__.rst` & `cubicweb-4.7.0/doc/api/__init__.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/api/cwvreg.rst` & `cubicweb-4.7.0/doc/api/cwvreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/api/predicates.rst` & `cubicweb-4.7.0/doc/api/predicates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/api/pyramid/core.rst` & `cubicweb-4.7.0/doc/api/pyramid/core.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/api/urlpublishing.rst` & `cubicweb-4.7.0/doc/api/urlpublishing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/api/web.rst` & `cubicweb-4.7.0/doc/api/web.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/MERGE_ME-tut-create-app.en.txt` & `cubicweb-4.7.0/doc/book/MERGE_ME-tut-create-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/MERGE_ME-tut-create-gae-app.en.txt` & `cubicweb-4.7.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/_maybe_to_integrate/rss-xml.rst` & `cubicweb-4.7.0/doc/book/_maybe_to_integrate/rss-xml.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/_maybe_to_integrate/template.rst` & `cubicweb-4.7.0/doc/book/_maybe_to_integrate/template.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/additionnal_services/undo.rst` & `cubicweb-4.7.0/doc/book/additionnal_services/undo.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/backups.rst` & `cubicweb-4.7.0/doc/book/admin/backups.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/config.rst` & `cubicweb-4.7.0/doc/book/admin/config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/create-instance.rst` & `cubicweb-4.7.0/doc/book/admin/create-instance.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/cubicweb-ctl.rst` & `cubicweb-4.7.0/doc/book/admin/cubicweb-ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/deploy.rst` & `cubicweb-4.7.0/doc/book/admin/deploy.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/instance-config.rst` & `cubicweb-4.7.0/doc/book/admin/instance-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/ldap.rst` & `cubicweb-4.7.0/doc/book/admin/ldap.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/setup.rst` & `cubicweb-4.7.0/doc/book/admin/setup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/admin/site-config.rst` & `cubicweb-4.7.0/doc/book/admin/site-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/depends.rst` & `cubicweb-4.7.0/doc/book/annexes/depends.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/docstrings-conventions.rst` & `cubicweb-4.7.0/doc/book/annexes/docstrings-conventions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/faq.rst` & `cubicweb-4.7.0/doc/book/annexes/faq.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/mercurial.rst` & `cubicweb-4.7.0/doc/book/annexes/mercurial.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/rql/Graph-ex.gif` & `cubicweb-4.7.0/doc/book/annexes/rql/Graph-ex.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/rql/debugging.rst` & `cubicweb-4.7.0/doc/book/annexes/rql/debugging.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/rql/implementation.rst` & `cubicweb-4.7.0/doc/book/annexes/rql/implementation.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/rql/intro.rst` & `cubicweb-4.7.0/doc/book/annexes/rql/intro.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/rql/language.rst` & `cubicweb-4.7.0/doc/book/annexes/rql/language.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/annexes/rql/usecases.rst` & `cubicweb-4.7.0/doc/book/annexes/rql/usecases.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/connections_pooler.rst` & `cubicweb-4.7.0/doc/book/devrepo/connections_pooler.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/cubes/available-cubes.rst` & `cubicweb-4.7.0/doc/book/devrepo/cubes/available-cubes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/cubes/cc-newcube.rst` & `cubicweb-4.7.0/doc/book/devrepo/cubes/cc-newcube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/cubes/layout.rst` & `cubicweb-4.7.0/doc/book/devrepo/cubes/layout.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/cubes/what-is-a-cube.rst` & `cubicweb-4.7.0/doc/book/devrepo/cubes/what-is-a-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/dataimport.rst` & `cubicweb-4.7.0/doc/book/devrepo/dataimport.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/datamodel/baseschema.rst` & `cubicweb-4.7.0/doc/book/devrepo/datamodel/baseschema.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/datamodel/define-workflows.rst` & `cubicweb-4.7.0/doc/book/devrepo/datamodel/define-workflows.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/datamodel/definition.rst` & `cubicweb-4.7.0/doc/book/devrepo/datamodel/definition.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/datamodel/metadata.rst` & `cubicweb-4.7.0/doc/book/devrepo/datamodel/metadata.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/debug_channels.rst` & `cubicweb-4.7.0/doc/book/devrepo/debug_channels.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/devcore/reqbase.rst` & `cubicweb-4.7.0/doc/book/devrepo/devcore/reqbase.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/entityclasses/adapters.rst` & `cubicweb-4.7.0/doc/book/devrepo/entityclasses/adapters.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/entityclasses/application-logic.rst` & `cubicweb-4.7.0/doc/book/devrepo/entityclasses/application-logic.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/entityclasses/data-as-objects.rst` & `cubicweb-4.7.0/doc/book/devrepo/entityclasses/data-as-objects.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/entityclasses/load-sort.rst` & `cubicweb-4.7.0/doc/book/devrepo/entityclasses/load-sort.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/fti.rst` & `cubicweb-4.7.0/doc/book/devrepo/fti.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/migration.rst` & `cubicweb-4.7.0/doc/book/devrepo/migration.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/profiling.rst` & `cubicweb-4.7.0/doc/book/devrepo/profiling.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/repo/hooks.rst` & `cubicweb-4.7.0/doc/book/devrepo/repo/hooks.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/repo/notifications.rst` & `cubicweb-4.7.0/doc/book/devrepo/repo/notifications.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/repo/sessions.rst` & `cubicweb-4.7.0/doc/book/devrepo/repo/sessions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/testing.rst` & `cubicweb-4.7.0/doc/book/devrepo/testing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devrepo/vreg.rst` & `cubicweb-4.7.0/doc/book/devrepo/vreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/ajax.rst` & `cubicweb-4.7.0/doc/book/devweb/ajax.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/controllers.rst` & `cubicweb-4.7.0/doc/book/devweb/controllers.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/css.rst` & `cubicweb-4.7.0/doc/book/devweb/css.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/edition/dissection.rst` & `cubicweb-4.7.0/doc/book/devweb/edition/dissection.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/edition/editcontroller.rst` & `cubicweb-4.7.0/doc/book/devweb/edition/editcontroller.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/edition/examples.rst` & `cubicweb-4.7.0/doc/book/devweb/edition/examples.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/edition/form.rst` & `cubicweb-4.7.0/doc/book/devweb/edition/form.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/facets.rst` & `cubicweb-4.7.0/doc/book/devweb/facets.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/httpcaching.rst` & `cubicweb-4.7.0/doc/book/devweb/httpcaching.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/internationalization.rst` & `cubicweb-4.7.0/doc/book/devweb/internationalization.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/js.rst` & `cubicweb-4.7.0/doc/book/devweb/js.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/publisher.rst` & `cubicweb-4.7.0/doc/book/devweb/publisher.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/request.rst` & `cubicweb-4.7.0/doc/book/devweb/request.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/resource.rst` & `cubicweb-4.7.0/doc/book/devweb/resource.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/searchbar.rst` & `cubicweb-4.7.0/doc/book/devweb/searchbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/basetemplates.rst` & `cubicweb-4.7.0/doc/book/devweb/views/basetemplates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/baseviews.rst` & `cubicweb-4.7.0/doc/book/devweb/views/baseviews.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/boxes.rst` & `cubicweb-4.7.0/doc/book/devweb/views/boxes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/breadcrumbs.rst` & `cubicweb-4.7.0/doc/book/devweb/views/breadcrumbs.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/idownloadable.rst` & `cubicweb-4.7.0/doc/book/devweb/views/idownloadable.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/primary.rst` & `cubicweb-4.7.0/doc/book/devweb/views/primary.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/reledit.rst` & `cubicweb-4.7.0/doc/book/devweb/views/reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/startup.rst` & `cubicweb-4.7.0/doc/book/devweb/views/startup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/table.rst` & `cubicweb-4.7.0/doc/book/devweb/views/table.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/urlpublish.rst` & `cubicweb-4.7.0/doc/book/devweb/views/urlpublish.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/views.rst` & `cubicweb-4.7.0/doc/book/devweb/views/views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/views/xmlrss.rst` & `cubicweb-4.7.0/doc/book/devweb/views/xmlrss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/devweb/warning.rst` & `cubicweb-4.7.0/doc/book/devweb/warning.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/intro/concepts.rst` & `cubicweb-4.7.0/doc/book/intro/concepts.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/intro/history.rst` & `cubicweb-4.7.0/doc/book/intro/history.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/pyramid/auth.rst` & `cubicweb-4.7.0/doc/book/pyramid/auth.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/pyramid/ctl.rst` & `cubicweb-4.7.0/doc/book/pyramid/ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/pyramid/debug_toolbar.rst` & `cubicweb-4.7.0/doc/book/pyramid/debug_toolbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/pyramid/index.rst` & `cubicweb-4.7.0/doc/book/pyramid/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/pyramid/quickstart.rst` & `cubicweb-4.7.0/doc/book/pyramid/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/pyramid/settings.rst` & `cubicweb-4.7.0/doc/book/pyramid/settings.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/security/csrf.rst` & `cubicweb-4.7.0/doc/book/security/csrf.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/src/archi_globale.dia` & `cubicweb-4.7.0/doc/book/src/archi_globale.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/book/src/main_template_layout.dia` & `cubicweb-4.7.0/doc/book/src/main_template_layout.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.14.rst` & `cubicweb-4.7.0/doc/changes/3.14.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.15.rst` & `cubicweb-4.7.0/doc/changes/3.15.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.16.rst` & `cubicweb-4.7.0/doc/changes/3.16.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.17.rst` & `cubicweb-4.7.0/doc/changes/3.17.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.18.rst` & `cubicweb-4.7.0/doc/changes/3.18.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.19.rst` & `cubicweb-4.7.0/doc/changes/3.19.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.20.rst` & `cubicweb-4.7.0/doc/changes/3.20.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.21.rst` & `cubicweb-4.7.0/doc/changes/3.21.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.22.rst` & `cubicweb-4.7.0/doc/changes/3.22.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.23.rst` & `cubicweb-4.7.0/doc/changes/3.23.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.24.rst` & `cubicweb-4.7.0/doc/changes/3.24.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.25.rst` & `cubicweb-4.7.0/doc/changes/3.25.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.27.rst` & `cubicweb-4.7.0/doc/changes/3.27.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.28.rst` & `cubicweb-4.7.0/doc/changes/3.28.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.29.rst` & `cubicweb-4.7.0/doc/changes/3.29.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.30.rst` & `cubicweb-4.7.0/doc/changes/3.30.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.31.rst` & `cubicweb-4.7.0/doc/changes/3.31.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.32.rst` & `cubicweb-4.7.0/doc/changes/3.32.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.32_reledit.rst` & `cubicweb-4.7.0/doc/changes/3.32_reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.33.rst` & `cubicweb-4.7.0/doc/changes/3.33.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.34.rst` & `cubicweb-4.7.0/doc/changes/3.34.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.35.rst` & `cubicweb-4.7.0/doc/changes/3.35.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.36.rst` & `cubicweb-4.7.0/doc/changes/3.36.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.37.rst` & `cubicweb-4.7.0/doc/changes/3.37.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/3.38.rst` & `cubicweb-4.7.0/doc/changes/3.38.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+3.38.16 (2024-04-03)
+====================
+
+👷 Bug fixes
+-----------
+
+- install lxml[html_clean] >= 5.2.0, and fix CLEANER instanciation
+
+3.38.15 (2024-03-20)
+====================
+👷 Bug fixes
+-----------
+
+- session: using unsafe_cnx_context_manager invoke a recursive auth loop
+
 3.38.14 (2024-02-07)
 ====================
 🎉 New features
 --------------
 
 - auth: add an authentication ticket mechanism to ensure cookies invalidation
 - skeleton: add --diff option to black job
```

### Comparing `cubicweb-4.6.4/doc/changes/4.0.rst` & `cubicweb-4.7.0/doc/changes/4.0.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/4.1.rst` & `cubicweb-4.7.0/doc/changes/4.1.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/4.3.rst` & `cubicweb-4.7.0/doc/changes/4.3.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/4.5.rst` & `cubicweb-4.7.0/doc/changes/4.5.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/4.6.rst` & `cubicweb-4.7.0/doc/changes/4.6.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/changes/changelog.rst` & `cubicweb-4.7.0/doc/changes/changelog.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .. -*- coding: utf-8 -*-
 
+.. include:: 4.7.rst
 .. include:: 4.6.rst
 .. include:: 4.5.rst
 .. include:: 4.4.rst
 .. include:: 4.3.rst
 .. include:: 4.2.rst
 .. include:: 4.1.rst
 .. include:: 4.0.rst
```

### Comparing `cubicweb-4.6.4/doc/conf.py` & `cubicweb-4.7.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/03-transitions-view_en.png` & `cubicweb-4.7.0/doc/images/03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/breadcrumbs_header.png` & `cubicweb-4.7.0/doc/images/breadcrumbs_header.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_general_panel.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_general_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_registry_content_panel.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_registry_content_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_registry_decisions_panel.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_registry_decisions_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_rql_panel.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_rql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_rql_traceback_panel.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_rql_traceback_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_show_source.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_show_source.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_show_source_link.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_show_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_sql_panel.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_sql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/debugtoolbar_traceback_source_link.png` & `cubicweb-4.7.0/doc/images/debugtoolbar_traceback_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/example-card-with-rql-directive.png` & `cubicweb-4.7.0/doc/images/example-card-with-rql-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/example-card-with-rql-table-directive.png` & `cubicweb-4.7.0/doc/images/example-card-with-rql-table-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/facet_date_range.png` & `cubicweb-4.7.0/doc/images/facet_date_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/facet_has_image.png` & `cubicweb-4.7.0/doc/images/facet_has_image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/facet_overview.png` & `cubicweb-4.7.0/doc/images/facet_overview.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/facet_range.png` & `cubicweb-4.7.0/doc/images/facet_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_00-login_en.png` & `cubicweb-4.7.0/doc/images/lax-book_00-login_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_01-start_en.png` & `cubicweb-4.7.0/doc/images/lax-book_01-start_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_02-cookie-values_en.png` & `cubicweb-4.7.0/doc/images/lax-book_02-cookie-values_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_02-create-blog_en.png` & `cubicweb-4.7.0/doc/images/lax-book_02-create-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_03-list-one-blog_en.png` & `cubicweb-4.7.0/doc/images/lax-book_03-list-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_03-site-config-panel_en.png` & `cubicweb-4.7.0/doc/images/lax-book_03-site-config-panel_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_03-state-submitted_en.png` & `cubicweb-4.7.0/doc/images/lax-book_03-state-submitted_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_03-transitions-view_en.png` & `cubicweb-4.7.0/doc/images/lax-book_03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_04-detail-one-blog_en.png` & `cubicweb-4.7.0/doc/images/lax-book_04-detail-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_05-list-two-blog_en.png` & `cubicweb-4.7.0/doc/images/lax-book_05-list-two-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_06-add-relation-entryof_en.png` & `cubicweb-4.7.0/doc/images/lax-book_06-add-relation-entryof_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_06-main-template-logo_en.png` & `cubicweb-4.7.0/doc/images/lax-book_06-main-template-logo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_07-detail-one-blogentry_en.png` & `cubicweb-4.7.0/doc/images/lax-book_07-detail-one-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_08-schema_en.png` & `cubicweb-4.7.0/doc/images/lax-book_08-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_09-new-view-blogentry_en.png` & `cubicweb-4.7.0/doc/images/lax-book_09-new-view-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/lax-book_10-blog-with-two-entries_en.png` & `cubicweb-4.7.0/doc/images/lax-book_10-blog-with-two-entries_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/main_template.png` & `cubicweb-4.7.0/doc/images/main_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/main_template.svg` & `cubicweb-4.7.0/doc/images/main_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/main_template_layout.png` & `cubicweb-4.7.0/doc/images/main_template_layout.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/primaryview_template.png` & `cubicweb-4.7.0/doc/images/primaryview_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/primaryview_template.svg` & `cubicweb-4.7.0/doc/images/primaryview_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/request_session.png` & `cubicweb-4.7.0/doc/images/request_session.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/request_session.svg` & `cubicweb-4.7.0/doc/images/request_session.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/server-class-diagram.png` & `cubicweb-4.7.0/doc/images/server-class-diagram.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_blog-form_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_blog-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_blog-primary-after-post-creation_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_blog-primary_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_blog-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_blogs-list_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_blogs-list_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_form-generic-relations_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_form-generic-relations_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_index_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_index_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_index_gettext_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_index_gettext_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_index_logged_in_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_index_logged_in_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_login-form_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_login-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_myblog-community-custom-primary_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_myblog-community-custom-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_myblog-community-default-primary_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_myblog-community-default-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_myblog-community-taggable-primary_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_myblog-custom-footer_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_myblog-custom-footer_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_myblog-schema_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_myblog-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_myblog-siteinfo_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_myblog-siteinfo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_schema_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_schema_graphviz_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_schema_graphviz_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-base_siteconfig_en.png` & `cubicweb-4.7.0/doc/images/tutos-base_siteconfig_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_admin.png` & `cubicweb-4.7.0/doc/images/tutos-museum_admin.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_city_created.png` & `cubicweb-4.7.0/doc/images/tutos-museum_city_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_city_creation.png` & `cubicweb-4.7.0/doc/images/tutos-museum_city_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_data_model_schema.png` & `cubicweb-4.7.0/doc/images/tutos-museum_data_model_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_empty_instance.png` & `cubicweb-4.7.0/doc/images/tutos-museum_empty_instance.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_finished_import.png` & `cubicweb-4.7.0/doc/images/tutos-museum_finished_import.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_list_view.png` & `cubicweb-4.7.0/doc/images/tutos-museum_list_view.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_museum_created.png` & `cubicweb-4.7.0/doc/images/tutos-museum_museum_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_museum_creation.png` & `cubicweb-4.7.0/doc/images/tutos-museum_museum_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_museum_with_city_name.png` & `cubicweb-4.7.0/doc/images/tutos-museum_museum_with_city_name.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_react_map.png` & `cubicweb-4.7.0/doc/images/tutos-museum_react_map.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-museum_with_schema.png` & `cubicweb-4.7.0/doc/images/tutos-museum_with_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_background-image.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_background-image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_boxes.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_boxes.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_breadcrumbs.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_breadcrumbs.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_facets.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_facets.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_grey-box.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_grey-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_index-after.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_index-after.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_index-before.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_index-before.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_login-box.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_login-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_prevnext.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_prevnext.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_ui1.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_ui1.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_ui2.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_ui2.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/tutos-photowebsite_ui3.png` & `cubicweb-4.7.0/doc/images/tutos-photowebsite_ui3.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/undo_history-view_w600.png` & `cubicweb-4.7.0/doc/images/undo_history-view_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/undo_mesage_w600.png` & `cubicweb-4.7.0/doc/images/undo_mesage_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/undo_startup-link_w600.png` & `cubicweb-4.7.0/doc/images/undo_startup-link_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/views-table-filter-shadow.png` & `cubicweb-4.7.0/doc/images/views-table-filter-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/views-table-filter.png` & `cubicweb-4.7.0/doc/images/views-table-filter.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/views-table-shadow.png` & `cubicweb-4.7.0/doc/images/views-table-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/images/views-table.png` & `cubicweb-4.7.0/doc/images/views-table.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/index.rst` & `cubicweb-4.7.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/plan_formation_python_cubicweb.txt` & `cubicweb-4.7.0/doc/plan_formation_python_cubicweb.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tools/generate_modules.py` & `cubicweb-4.7.0/doc/tools/generate_modules.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tools/mode_plan.py` & `cubicweb-4.7.0/doc/tools/mode_plan.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tools/pyjsrest.py` & `cubicweb-4.7.0/doc/tools/pyjsrest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/advanced/index.rst` & `cubicweb-4.7.0/doc/tutorials/advanced/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/advanced/part01_create-cube.rst` & `cubicweb-4.7.0/doc/tutorials/advanced/part01_create-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/advanced/part02_security.rst` & `cubicweb-4.7.0/doc/tutorials/advanced/part02_security.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/advanced/part03_bfss.rst` & `cubicweb-4.7.0/doc/tutorials/advanced/part03_bfss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/advanced/part04_ui-base.rst` & `cubicweb-4.7.0/doc/tutorials/advanced/part04_ui-base.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/advanced/part05_ui-advanced.rst` & `cubicweb-4.7.0/doc/tutorials/advanced/part05_ui-advanced.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/base/blog-in-five-minutes.rst` & `cubicweb-4.7.0/doc/tutorials/base/blog-in-five-minutes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/base/conclusion.rst` & `cubicweb-4.7.0/doc/tutorials/base/conclusion.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/base/customizing-the-application.rst` & `cubicweb-4.7.0/doc/tutorials/base/customizing-the-application.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/base/discovering-the-ui.rst` & `cubicweb-4.7.0/doc/tutorials/base/discovering-the-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/base/index.rst` & `cubicweb-4.7.0/doc/tutorials/base/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/dataimport/diseasome_import.py` & `cubicweb-4.7.0/doc/tutorials/dataimport/diseasome_import.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/dataimport/diseasome_parser.py` & `cubicweb-4.7.0/doc/tutorials/dataimport/diseasome_parser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/dataimport/index.rst` & `cubicweb-4.7.0/doc/tutorials/dataimport/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/dataimport/schema.py` & `cubicweb-4.7.0/doc/tutorials/dataimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/index.rst` & `cubicweb-4.7.0/doc/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/museum/data-management.rst` & `cubicweb-4.7.0/doc/tutorials/museum/data-management.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/museum/develop-app.rst` & `cubicweb-4.7.0/doc/tutorials/museum/develop-app.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/museum/develop-ui.rst` & `cubicweb-4.7.0/doc/tutorials/museum/develop-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/museum/enhance-views.rst` & `cubicweb-4.7.0/doc/tutorials/museum/enhance-views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/museum/getting-started.rst` & `cubicweb-4.7.0/doc/tutorials/museum/getting-started.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/doc/tutorials/museum/index.rst` & `cubicweb-4.7.0/doc/tutorials/museum/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/extras/cubicweb-ctl.bash_completion` & `cubicweb-4.7.0/extras/cubicweb-ctl.bash_completion`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/jshintrc` & `cubicweb-4.7.0/jshintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/man/cubicweb-ctl.1` & `cubicweb-4.7.0/man/cubicweb-ctl.1`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/pylintrc` & `cubicweb-4.7.0/pylintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.6.4/setup.py` & `cubicweb-4.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     package_data=package_data,
     include_package_data=True,
     install_requires=[
         "logilab-common >= 1.8.3, < 2.0.0",
         "logilab-mtconverter >= 0.9.2, < 1.0.0",
         "rql >= 0.39, < 1.0.0",
         "yams >= 0.50.0, < 1.0.0",
-        "lxml",
+        "lxml[html_clean] >= 5.2.0, < 6.0.0",
         "logilab-database >= 1.18.6, < 2.0.0",
         "passlib >= 1.7",
         "pytz",
         "Markdown >= 3.4.0",
         "filelock",
         "rdflib >= 6.0.0",
         "pyramid >= 1.9.0, < 2.0.0",
```

### Comparing `cubicweb-4.6.4/tox.ini` & `cubicweb-4.7.0/tox.ini`

 * *Files identical despite different names*

