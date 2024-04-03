# Comparing `tmp/pysnmp-pysmi-1.1.7.tar.gz` & `tmp/pysnmp-pysmi-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysnmp-pysmi-1.1.7.tar", max compression
+gzip compressed data, was "pysnmp-pysmi-1.1.8.tar", max compression
```

## Comparing `pysnmp-pysmi-1.1.7.tar` & `pysnmp-pysmi-1.1.8.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0     1333 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/LICENSE.rst
--rw-r--r--   0        0        0     6551 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/README.md
--rw-r--r--   0        0        0     7414 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/Makefile
--rw-r--r--   0        0        0      218 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/README.txt
--rw-r--r--   0        0        0      232 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/.static/css/rtdimproved.css
--rw-r--r--   0        0        0     4030 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/.static/favicon.ico
--rw-r--r--   0        0        0    13811 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/.static/logo.svg
--rw-r--r--   0        0        0       53 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/changelog.rst
--rw-r--r--   0        0        0    10396 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/conf.py
--rw-r--r--   0        0        0     1772 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/contents.rst
--rw-r--r--   0        0        0     1968 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/documentation.rst
--rw-r--r--   0        0        0      355 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/download.rst
--rw-r--r--   0        0        0      326 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/examples/always-borrow-precompiled-pysnmp-files.rst
--rw-r--r--   0        0        0      338 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/examples/borrow-precompiled-pysnmp-files-on-failure.rst
--rw-r--r--   0        0        0      356 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.rst
--rw-r--r--   0        0        0      347 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.rst
--rw-r--r--   0        0        0      341 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/examples/download-and-compile-smistar-mibs-into-json.rst
--rw-r--r--   0        0        0      365 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/examples/download-and-compile-smistar-mibs-into-pysnmp-files.rst
--rw-r--r--   0        0        0     4764 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/library-reference.rst
--rw-r--r--   0        0        0       49 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/license.rst
--rw-r--r--   0        0        0     4647 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/mibcopy.rst
--rw-r--r--   0        0        0    12725 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/mibdump.rst
--rw-r--r--   0        0        0      144 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/borrower/anyfile/anyfileborrower.rst
--rw-r--r--   0        0        0      146 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/borrower/pyfile/pyfileborrower.rst
--rw-r--r--   0        0        0      146 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/codegen/jsondoc/jsoncodegen.rst
--rw-r--r--   0        0        0      134 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/codegen/null/nullcodegen.rst
--rw-r--r--   0        0        0      142 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/codegen/pysnmp/pysnmpcodegen.rst
--rw-r--r--   0        0        0      109 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/compiler/mibcompiler.rst
--rw-r--r--   0        0        0      249 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/compiler/mibstatus.rst
--rw-r--r--   0        0        0     1083 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/parser/smi/dialect.rst
--rw-r--r--   0        0        0      992 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/parser/smi/parserfactory.rst
--rw-r--r--   0        0        0      217 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/reader/callback/callbackreader.rst
--rw-r--r--   0        0        0      202 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/reader/httpclient/httpreader.rst
--rw-r--r--   0        0        0      229 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/reader/localfile/filereader.rst
--rw-r--r--   0        0        0      267 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/reader/zipreader/zipreader.rst
--rw-r--r--   0        0        0      260 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/searcher/pyfile/pyfilesearcher.rst
--rw-r--r--   0        0        0      317 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/searcher/pypackage/pypackagesearcher.rst
--rw-r--r--   0        0        0      468 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/searcher/stub/stubsearcher.rst
--rw-r--r--   0        0        0      232 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/writer/callback/callbackwriter.rst
--rw-r--r--   0        0        0      121 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/writer/localfile/filewriter.rst
--rw-r--r--   0        0        0      133 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/docs/source/pysmi/writer/pyfile/pyfilewriter.rst
--rw-r--r--   0        0        0     1117 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/examples/always-borrow-precompiled-pysnmp-files.py
--rw-r--r--   0        0        0     1569 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/examples/borrow-precompiled-pysnmp-files-on-failure.py
--rw-r--r--   0        0        0     1917 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.py
--rw-r--r--   0        0        0     1350 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.py
--rw-r--r--   0        0        0     1462 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/examples/download-and-compile-smistar-mibs-into-json.py
--rw-r--r--   0        0        0     1431 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/examples/download-and-compile-smistar-mibs-into-pysnmp-files.py
--rw-r--r--   0        0        0     1206 2022-01-05 15:32:15.907206 pysnmp-pysmi-1.1.7/pyproject.toml
--rw-r--r--   0        0        0       65 2022-01-05 15:32:15.907206 pysnmp-pysmi-1.1.7/pysmi/__init__.py
--rw-r--r--   0        0        0      255 2022-01-05 15:31:12.750251 pysnmp-pysmi-1.1.7/pysmi/borrower/__init__.py
--rw-r--r--   0        0        0      300 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/borrower/anyfile.py
--rw-r--r--   0        0        0     1739 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/borrower/base.py
--rw-r--r--   0        0        0      615 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/borrower/pyfile.py
--rw-r--r--   0        0        0      292 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/codegen/__init__.py
--rw-r--r--   0        0        0    17798 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/codegen/base.py
--rw-r--r--   0        0        0    35669 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/codegen/jsondoc.py
--rw-r--r--   0        0        0      685 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/codegen/null.py
--rw-r--r--   0        0        0    43633 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/codegen/pysnmp.py
--rw-r--r--   0        0        0    21738 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/codegen/symtable.py
--rw-r--r--   0        0        0      361 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/compat.py
--rw-r--r--   0        0        0    21676 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/compiler.py
--rw-r--r--   0        0        0     3462 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/debug.py
--rw-r--r--   0        0        0     1732 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/error.py
--rw-r--r--   0        0        0      194 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/lexer/__init__.py
--rw-r--r--   0        0        0      243 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/lexer/base.py
--rw-r--r--   0        0        0    11763 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/lexer/smi.py
--rw-r--r--   0        0        0      822 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/mibinfo.py
--rw-r--r--   0        0        0      352 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/parser/__init__.py
--rw-r--r--   0        0        0      318 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/parser/base.py
--rw-r--r--   0        0        0      630 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/parser/dialect.py
--rw-r--r--   0        0        0      396 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/parser/null.py
--rw-r--r--   0        0        0    49433 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/parser/smi.py
--rw-r--r--   0        0        0      296 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/parser/smiv1.py
--rw-r--r--   0        0        0      350 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/parser/smiv1compat.py
--rw-r--r--   0        0        0      296 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/parser/smiv2.py
--rw-r--r--   0        0        0      390 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/reader/__init__.py
--rw-r--r--   0        0        0     1552 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/reader/base.py
--rw-r--r--   0        0        0     1516 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/reader/callback.py
--rw-r--r--   0        0        0     3600 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/reader/httpclient.py
--rw-r--r--   0        0        0     4937 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/reader/localfile.py
--rw-r--r--   0        0        0     1280 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/reader/url.py
--rw-r--r--   0        0        0     5635 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/reader/zipreader.py
--rw-r--r--   0        0        0     9331 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/scripts/mibcopy.py
--rw-r--r--   0        0        0    13618 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/scripts/mibdump.py
--rw-r--r--   0        0        0      355 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/searcher/__init__.py
--rw-r--r--   0        0        0     1937 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/searcher/anyfile.py
--rw-r--r--   0        0        0      405 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/searcher/base.py
--rw-r--r--   0        0        0     3702 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/searcher/pyfile.py
--rw-r--r--   0        0        0     5189 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/searcher/pypackage.py
--rw-r--r--   0        0        0     1292 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/searcher/stub.py
--rw-r--r--   0        0        0      295 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/writer/__init__.py
--rw-r--r--   0        0        0      479 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/writer/base.py
--rw-r--r--   0        0        0     1521 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/writer/callback.py
--rw-r--r--   0        0        0     2597 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/writer/localfile.py
--rw-r--r--   0        0        0     3208 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/pysmi/writer/pyfile.py
--rw-r--r--   0        0        0       59 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/__init__.py
--rw-r--r--   0        0        0      950 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/__main__.py
--rwxr-xr-x   0        0        0    70680 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/data/asn1/MIKROTIK-MIB
--rw-r--r--   0        0        0     2649 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_agentcapabilities_smiv2_pysnmp.py
--rw-r--r--   0        0        0     1615 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_imports_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2273 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_modulecompliance_smiv2_pysnmp.py
--rw-r--r--   0        0        0     3335 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_moduleidentity_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2324 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_notificationgroup_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2268 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_notificationtype_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2450 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_objectgroup_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2217 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_objectidentity_smiv2_pysnmp.py
--rw-r--r--   0        0        0    17121 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_objecttype_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2359 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_smiv1_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2246 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_traptype_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2949 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_typedeclaration_smiv1_pysnmp.py
--rw-r--r--   0        0        0     5385 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_typedeclaration_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2668 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_valuedeclaration_smiv2_pysnmp.py
--rw-r--r--   0        0        0    13156 2022-01-05 15:31:12.754251 pysnmp-pysmi-1.1.7/tests/test_zipreader.py
--rw-r--r--   0        0        0     7710 2022-01-05 15:32:16.589161 pysnmp-pysmi-1.1.7/setup.py
--rw-r--r--   0        0        0     7699 2022-01-05 15:32:16.589741 pysnmp-pysmi-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1333 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/LICENSE.rst
+-rw-r--r--   0        0        0     6551 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/README.md
+-rw-r--r--   0        0        0     7414 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/Makefile
+-rw-r--r--   0        0        0      218 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/README.txt
+-rw-r--r--   0        0        0      232 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/.static/css/rtdimproved.css
+-rw-r--r--   0        0        0     4030 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/.static/favicon.ico
+-rw-r--r--   0        0        0    13811 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/.static/logo.svg
+-rw-r--r--   0        0        0       53 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/changelog.rst
+-rw-r--r--   0        0        0    10396 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/conf.py
+-rw-r--r--   0        0        0     1772 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/contents.rst
+-rw-r--r--   0        0        0     1968 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/documentation.rst
+-rw-r--r--   0        0        0      355 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/download.rst
+-rw-r--r--   0        0        0      326 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/examples/always-borrow-precompiled-pysnmp-files.rst
+-rw-r--r--   0        0        0      338 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/examples/borrow-precompiled-pysnmp-files-on-failure.rst
+-rw-r--r--   0        0        0      356 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.rst
+-rw-r--r--   0        0        0      347 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.rst
+-rw-r--r--   0        0        0      341 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/examples/download-and-compile-smistar-mibs-into-json.rst
+-rw-r--r--   0        0        0      365 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/examples/download-and-compile-smistar-mibs-into-pysnmp-files.rst
+-rw-r--r--   0        0        0     4764 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/library-reference.rst
+-rw-r--r--   0        0        0       49 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/license.rst
+-rw-r--r--   0        0        0     4647 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/mibcopy.rst
+-rw-r--r--   0        0        0    12725 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/mibdump.rst
+-rw-r--r--   0        0        0      144 2022-01-05 18:28:06.989251 pysnmp-pysmi-1.1.8/docs/source/pysmi/borrower/anyfile/anyfileborrower.rst
+-rw-r--r--   0        0        0      146 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/borrower/pyfile/pyfileborrower.rst
+-rw-r--r--   0        0        0      146 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/codegen/jsondoc/jsoncodegen.rst
+-rw-r--r--   0        0        0      134 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/codegen/null/nullcodegen.rst
+-rw-r--r--   0        0        0      142 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/codegen/pysnmp/pysnmpcodegen.rst
+-rw-r--r--   0        0        0      109 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/compiler/mibcompiler.rst
+-rw-r--r--   0        0        0      249 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/compiler/mibstatus.rst
+-rw-r--r--   0        0        0     1083 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/parser/smi/dialect.rst
+-rw-r--r--   0        0        0      992 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/parser/smi/parserfactory.rst
+-rw-r--r--   0        0        0      217 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/reader/callback/callbackreader.rst
+-rw-r--r--   0        0        0      202 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/reader/httpclient/httpreader.rst
+-rw-r--r--   0        0        0      229 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/reader/localfile/filereader.rst
+-rw-r--r--   0        0        0      267 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/reader/zipreader/zipreader.rst
+-rw-r--r--   0        0        0      260 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/searcher/pyfile/pyfilesearcher.rst
+-rw-r--r--   0        0        0      317 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/searcher/pypackage/pypackagesearcher.rst
+-rw-r--r--   0        0        0      468 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/searcher/stub/stubsearcher.rst
+-rw-r--r--   0        0        0      232 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/writer/callback/callbackwriter.rst
+-rw-r--r--   0        0        0      121 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/writer/localfile/filewriter.rst
+-rw-r--r--   0        0        0      133 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/docs/source/pysmi/writer/pyfile/pyfilewriter.rst
+-rw-r--r--   0        0        0     1117 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/examples/always-borrow-precompiled-pysnmp-files.py
+-rw-r--r--   0        0        0     1569 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/examples/borrow-precompiled-pysnmp-files-on-failure.py
+-rw-r--r--   0        0        0     1917 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.py
+-rw-r--r--   0        0        0     1350 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.py
+-rw-r--r--   0        0        0     1462 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/examples/download-and-compile-smistar-mibs-into-json.py
+-rw-r--r--   0        0        0     1431 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/examples/download-and-compile-smistar-mibs-into-pysnmp-files.py
+-rw-r--r--   0        0        0     1206 2022-01-05 18:29:15.458013 pysnmp-pysmi-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0       65 2022-01-05 18:29:15.454013 pysnmp-pysmi-1.1.8/pysmi/__init__.py
+-rw-r--r--   0        0        0      255 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/borrower/__init__.py
+-rw-r--r--   0        0        0      300 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/borrower/anyfile.py
+-rw-r--r--   0        0        0     1739 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/borrower/base.py
+-rw-r--r--   0        0        0      615 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/borrower/pyfile.py
+-rw-r--r--   0        0        0      292 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/codegen/__init__.py
+-rw-r--r--   0        0        0    17798 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/codegen/base.py
+-rw-r--r--   0        0        0    35669 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/codegen/jsondoc.py
+-rw-r--r--   0        0        0      685 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/codegen/null.py
+-rw-r--r--   0        0        0    43633 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/codegen/pysnmp.py
+-rw-r--r--   0        0        0    21738 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/codegen/symtable.py
+-rw-r--r--   0        0        0      361 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/compat.py
+-rw-r--r--   0        0        0    21676 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/compiler.py
+-rw-r--r--   0        0        0     3462 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/debug.py
+-rw-r--r--   0        0        0     1732 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/error.py
+-rw-r--r--   0        0        0      194 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/lexer/__init__.py
+-rw-r--r--   0        0        0      243 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/lexer/base.py
+-rw-r--r--   0        0        0    11763 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/lexer/smi.py
+-rw-r--r--   0        0        0      822 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/mibinfo.py
+-rw-r--r--   0        0        0      352 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/parser/__init__.py
+-rw-r--r--   0        0        0      318 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/parser/base.py
+-rw-r--r--   0        0        0      630 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/parser/dialect.py
+-rw-r--r--   0        0        0      396 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/parser/null.py
+-rw-r--r--   0        0        0    49433 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/parser/smi.py
+-rw-r--r--   0        0        0      296 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/parser/smiv1.py
+-rw-r--r--   0        0        0      350 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/parser/smiv1compat.py
+-rw-r--r--   0        0        0      296 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/parser/smiv2.py
+-rw-r--r--   0        0        0      390 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/reader/__init__.py
+-rw-r--r--   0        0        0     1552 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/reader/base.py
+-rw-r--r--   0        0        0     1516 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/reader/callback.py
+-rw-r--r--   0        0        0     3600 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/reader/httpclient.py
+-rw-r--r--   0        0        0     4937 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/reader/localfile.py
+-rw-r--r--   0        0        0     1280 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/reader/url.py
+-rw-r--r--   0        0        0     5635 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/reader/zipreader.py
+-rw-r--r--   0        0        0     9331 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/scripts/mibcopy.py
+-rw-r--r--   0        0        0    13620 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/scripts/mibdump.py
+-rw-r--r--   0        0        0      355 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/searcher/__init__.py
+-rw-r--r--   0        0        0     1937 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/searcher/anyfile.py
+-rw-r--r--   0        0        0      405 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/searcher/base.py
+-rw-r--r--   0        0        0     3702 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/searcher/pyfile.py
+-rw-r--r--   0        0        0     5189 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/searcher/pypackage.py
+-rw-r--r--   0        0        0     1292 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/searcher/stub.py
+-rw-r--r--   0        0        0      295 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/writer/__init__.py
+-rw-r--r--   0        0        0      479 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/writer/base.py
+-rw-r--r--   0        0        0     1521 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/writer/callback.py
+-rw-r--r--   0        0        0     2597 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/writer/localfile.py
+-rw-r--r--   0        0        0     3208 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/pysmi/writer/pyfile.py
+-rw-r--r--   0        0        0       59 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/tests/__init__.py
+-rw-r--r--   0        0        0      950 2022-01-05 18:28:06.993251 pysnmp-pysmi-1.1.8/tests/__main__.py
+-rwxr-xr-x   0        0        0    70680 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/data/asn1/MIKROTIK-MIB
+-rw-r--r--   0        0        0     2649 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_agentcapabilities_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     1615 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_imports_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2273 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_modulecompliance_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     3335 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_moduleidentity_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2324 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_notificationgroup_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2268 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_notificationtype_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2450 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_objectgroup_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2217 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_objectidentity_smiv2_pysnmp.py
+-rw-r--r--   0        0        0    17121 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_objecttype_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2359 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_smiv1_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2246 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_traptype_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2949 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_typedeclaration_smiv1_pysnmp.py
+-rw-r--r--   0        0        0     5385 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_typedeclaration_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2668 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_valuedeclaration_smiv2_pysnmp.py
+-rw-r--r--   0        0        0    13156 2022-01-05 18:28:06.997251 pysnmp-pysmi-1.1.8/tests/test_zipreader.py
+-rw-r--r--   0        0        0     7710 2022-01-05 18:29:16.111336 pysnmp-pysmi-1.1.8/setup.py
+-rw-r--r--   0        0        0     7699 2022-01-05 18:29:16.111868 pysnmp-pysmi-1.1.8/PKG-INFO
```

### Comparing `pysnmp-pysmi-1.1.7/LICENSE.rst` & `pysnmp-pysmi-1.1.8/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/README.md` & `pysnmp-pysmi-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/Makefile` & `pysnmp-pysmi-1.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/.static/favicon.ico` & `pysnmp-pysmi-1.1.8/docs/source/.static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/.static/logo.svg` & `pysnmp-pysmi-1.1.8/docs/source/.static/logo.svg`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/conf.py` & `pysnmp-pysmi-1.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/contents.rst` & `pysnmp-pysmi-1.1.8/docs/source/contents.rst`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/documentation.rst` & `pysnmp-pysmi-1.1.8/docs/source/documentation.rst`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/library-reference.rst` & `pysnmp-pysmi-1.1.8/docs/source/library-reference.rst`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/mibcopy.rst` & `pysnmp-pysmi-1.1.8/docs/source/mibcopy.rst`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/mibdump.rst` & `pysnmp-pysmi-1.1.8/docs/source/mibdump.rst`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/pysmi/parser/smi/dialect.rst` & `pysnmp-pysmi-1.1.8/docs/source/pysmi/parser/smi/dialect.rst`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/docs/source/pysmi/parser/smi/parserfactory.rst` & `pysnmp-pysmi-1.1.8/docs/source/pysmi/parser/smi/parserfactory.rst`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/examples/always-borrow-precompiled-pysnmp-files.py` & `pysnmp-pysmi-1.1.8/examples/always-borrow-precompiled-pysnmp-files.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/examples/borrow-precompiled-pysnmp-files-on-failure.py` & `pysnmp-pysmi-1.1.8/examples/borrow-precompiled-pysnmp-files-on-failure.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.py` & `pysnmp-pysmi-1.1.8/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.py` & `pysnmp-pysmi-1.1.8/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/examples/download-and-compile-smistar-mibs-into-json.py` & `pysnmp-pysmi-1.1.8/examples/download-and-compile-smistar-mibs-into-json.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/examples/download-and-compile-smistar-mibs-into-pysnmp-files.py` & `pysnmp-pysmi-1.1.8/examples/download-and-compile-smistar-mibs-into-pysnmp-files.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pyproject.toml` & `pysnmp-pysmi-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysnmp-pysmi"
-version = "1.1.7"
+version = "1.1.8"
 description = ""
 authors = ["rfaircloth-splunk <rfaircloth@splunk.com>"]
 license = "BSD-2-Clause"
 repository = "https://github.com/pysnmp/pysmi"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
```

### Comparing `pysnmp-pysmi-1.1.7/pysmi/borrower/base.py` & `pysnmp-pysmi-1.1.8/pysmi/borrower/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/borrower/pyfile.py` & `pysnmp-pysmi-1.1.8/pysmi/borrower/pyfile.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/codegen/base.py` & `pysnmp-pysmi-1.1.8/pysmi/codegen/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/codegen/jsondoc.py` & `pysnmp-pysmi-1.1.8/pysmi/codegen/jsondoc.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/codegen/null.py` & `pysnmp-pysmi-1.1.8/pysmi/codegen/null.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/codegen/pysnmp.py` & `pysnmp-pysmi-1.1.8/pysmi/codegen/pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/codegen/symtable.py` & `pysnmp-pysmi-1.1.8/pysmi/codegen/symtable.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/compiler.py` & `pysnmp-pysmi-1.1.8/pysmi/compiler.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/debug.py` & `pysnmp-pysmi-1.1.8/pysmi/debug.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/error.py` & `pysnmp-pysmi-1.1.8/pysmi/error.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/lexer/smi.py` & `pysnmp-pysmi-1.1.8/pysmi/lexer/smi.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/mibinfo.py` & `pysnmp-pysmi-1.1.8/pysmi/mibinfo.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/parser/dialect.py` & `pysnmp-pysmi-1.1.8/pysmi/parser/dialect.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/parser/smi.py` & `pysnmp-pysmi-1.1.8/pysmi/parser/smi.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/reader/base.py` & `pysnmp-pysmi-1.1.8/pysmi/reader/base.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/reader/callback.py` & `pysnmp-pysmi-1.1.8/pysmi/reader/callback.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/reader/httpclient.py` & `pysnmp-pysmi-1.1.8/pysmi/reader/httpclient.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/reader/localfile.py` & `pysnmp-pysmi-1.1.8/pysmi/reader/localfile.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/reader/url.py` & `pysnmp-pysmi-1.1.8/pysmi/reader/url.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/reader/zipreader.py` & `pysnmp-pysmi-1.1.8/pysmi/reader/zipreader.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/scripts/mibcopy.py` & `pysnmp-pysmi-1.1.8/pysmi/scripts/mibcopy.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/scripts/mibdump.py` & `pysnmp-pysmi-1.1.8/pysmi/scripts/mibdump.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,16 +211,16 @@
         if not mibSearchers:
             mibSearchers = PySnmpCodeGen.defaultMibPackages
 
         if not mibStubs:
             mibStubs = [x for x in PySnmpCodeGen.baseMibs if x not in PySnmpCodeGen.fakeMibs]
 
         if not mibBorrowers:
-            mibBorrowers = [('http://pysnmp.github.com:443/mibs/notexts/@mib@', False),
-                            ('http://pysnmp.github.com:443/mibs/fulltexts/@mib@', True)]
+            mibBorrowers = [('https://pysnmp.github.com:443/mibs/notexts/@mib@', False),
+                            ('https://pysnmp.github.com:443/mibs/fulltexts/@mib@', True)]
 
         if not dstDirectory:
             dstDirectory = os.path.expanduser("~")
             if sys.platform[:3] == 'win':
                 dstDirectory = os.path.join(dstDirectory, 'PySNMP Configuration', 'mibs')
             else:
                 dstDirectory = os.path.join(dstDirectory, '.pysnmp', 'mibs')
```

### Comparing `pysnmp-pysmi-1.1.7/pysmi/searcher/anyfile.py` & `pysnmp-pysmi-1.1.8/pysmi/searcher/anyfile.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/searcher/pyfile.py` & `pysnmp-pysmi-1.1.8/pysmi/searcher/pyfile.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/searcher/pypackage.py` & `pysnmp-pysmi-1.1.8/pysmi/searcher/pypackage.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/searcher/stub.py` & `pysnmp-pysmi-1.1.8/pysmi/searcher/stub.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/writer/callback.py` & `pysnmp-pysmi-1.1.8/pysmi/writer/callback.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/writer/localfile.py` & `pysnmp-pysmi-1.1.8/pysmi/writer/localfile.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/pysmi/writer/pyfile.py` & `pysnmp-pysmi-1.1.8/pysmi/writer/pyfile.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/__main__.py` & `pysnmp-pysmi-1.1.8/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/data/asn1/MIKROTIK-MIB` & `pysnmp-pysmi-1.1.8/tests/data/asn1/MIKROTIK-MIB`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_agentcapabilities_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_agentcapabilities_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_imports_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_imports_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_modulecompliance_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_modulecompliance_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_moduleidentity_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_moduleidentity_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_notificationgroup_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_notificationgroup_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_notificationtype_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_notificationtype_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_objectgroup_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_objectgroup_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_objectidentity_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_objectidentity_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_objecttype_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_objecttype_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_smiv1_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_smiv1_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_traptype_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_traptype_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_typedeclaration_smiv1_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_typedeclaration_smiv1_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_typedeclaration_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_typedeclaration_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_valuedeclaration_smiv2_pysnmp.py` & `pysnmp-pysmi-1.1.8/tests/test_valuedeclaration_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/tests/test_zipreader.py` & `pysnmp-pysmi-1.1.8/tests/test_zipreader.py`

 * *Files identical despite different names*

### Comparing `pysnmp-pysmi-1.1.7/setup.py` & `pysnmp-pysmi-1.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['mibcopy = pysmi.scripts.mibcopy:start',
                      'mibdump = pysmi.scripts.mibdump:start']}
 
 setup_kwargs = {
     'name': 'pysnmp-pysmi',
-    'version': '1.1.7',
+    'version': '1.1.8',
     'description': '',
     'long_description': '\nSNMP MIB parser\n---------------\n\n[![Python Versions](https://img.shields.io/pypi/pyversions/pysnmp-pysmi.svg)](https://pypi.org/project/pysnmp-pysmi/)\n[![Build status](https://travis-ci.org/etingof/pysmi.svg?branch=master)](https://secure.travis-ci.org/etingof/pysmi)\n[![Coverage Status](https://img.shields.io/codecov/c/github/pysnmp/pysmi.svg)](https://codecov.io/github/pysnmp/pysmi)\n[![GitHub license](https://img.shields.io/badge/license-BSD-blue.svg)](https://raw.githubusercontent.com/pysnmp/pysmi/main/LICENSE.rst)\n\nPySMI is a pure-Python implementation of\n[SNMP SMI](https://en.wikipedia.org/wiki/Management_information_base) MIB parser.\nThis tool is designed to turn ASN.1 MIBs into various formats. As of this moment,\nJSON and [pysnmp](https://github.com/etingof/pysnmp) modules can be generated\nfrom ASN.1 MIBs.\n\nFeatures\n--------\n\n* Understands SMIv1, SMIv2 and de-facto SMI dialects\n* Turns MIBs into pysnmp classes and JSON documents\n* Maintains an index of MIB objects over many MIB modules\n* Automatically pulls ASN.1 MIBs from local directories, ZIP archives,\n  HTTP and FTP servers\n* 100% Python, works with Python 2.4 up to Python 3.7\n\nRendered PySMI documentation can be found at [pysmi site](http://snmplabs.com/pysmi).\n\nHow to use PySMI\n----------------\n\nIf you are using pysnmp, you might never notice pysmi presence - pysnmp\ncalls pysmi for MIB download and compilation behind the scenes (you can\nstill can do that manually by invoking *mibdump.py* tool).\n\nTo turn ASN.1 MIB into a JSON document, call *mibdump.py* tool like this:\n\n```\n$ mibdump.py --generate-mib-texts  --destination-format json IF-MIB\nSource MIB repositories: file:///usr/share/snmp/mibs, https://pysnmp.github.io/mibs/asn1/@mib@\nBorrow missing/failed MIBs from: http://pysnmp.github.io/json/fulltexts/@mib@\nExisting/compiled MIB locations: \nCompiled MIBs destination directory: .\nMIBs excluded from code generation: RFC-1212, RFC-1215, RFC1065-SMI, RFC1155-SMI,\nRFC1158-MIB, RFC1213-MIB, SNMPv2-CONF, SNMPv2-SMI, SNMPv2-TC, SNMPv2-TM\nMIBs to compile: IF-MIB\nDestination format: json\nParser grammar cache directory: not used\nAlso compile all relevant MIBs: yes\nRebuild MIBs regardless of age: yes\nDo not create/update MIBs: no\nByte-compile Python modules: no (optimization level no)\nIgnore compilation errors: no\nGenerate OID->MIB index: no\nGenerate texts in MIBs: yes\nKeep original texts layout: no\nTry various filenames while searching for MIB module: yes\nCreated/updated MIBs: IANAifType-MIB, IF-MIB, SNMPv2-MIB\nPre-compiled MIBs borrowed: \nUp to date MIBs: SNMPv2-CONF, SNMPv2-SMI, SNMPv2-TC\nMissing source MIBs: \nIgnored MIBs: \nFailed MIBs: \n```\n\nJSON document build from\n[IF-MIB module](https://pysnmp.github.io/mibs/asn1IF-MIB)\nwould hold information such as:\n\n```\n   {\n      "ifMIB": {\n          "name": "ifMIB",\n          "oid": "1.3.6.1.2.1.31",\n          "class": "moduleidentity",\n          "revisions": [\n            "2007-02-15 00:00",\n            "1996-02-28 21:55",\n            "1993-11-08 21:55"\n          ]\n        },\n      ...\n      "ifTestTable": {\n        "name": "ifTestTable",\n        "oid": "1.3.6.1.2.1.31.1.3",\n        "nodetype": "table",\n        "class": "objecttype",\n        "maxaccess": "not-accessible"\n      },\n      "ifTestEntry": {\n        "name": "ifTestEntry",\n        "oid": "1.3.6.1.2.1.31.1.3.1",\n        "nodetype": "row",\n        "class": "objecttype",\n        "maxaccess": "not-accessible",\n        "augmention": {\n          "name": "ifTestEntry",\n          "module": "IF-MIB",\n          "object": "ifEntry"\n        }\n      },\n      "ifTestId": {\n        "name": "ifTestId",\n        "oid": "1.3.6.1.2.1.31.1.3.1.1",\n        "nodetype": "column",\n        "class": "objecttype",\n        "syntax": {\n          "type": "TestAndIncr",\n          "class": "type"\n        },\n        "maxaccess": "read-write"\n      },\n      ...\n   }\n```\n\nIn general, converted MIBs capture all aspects of original (ASN.1) MIB contents\nand layout. The snippet above is just a partial example, but here is the\ncomplete [IF-MIB.json](http://pysnmp.github.io/json/fulltexts/IF-MIB.json)\nfile.\n\nBesides one-to-one MIB conversion, PySMI library can produce JSON index to\nfacilitate fast MIB information lookup across large collection of MIB files.\nFor example, JSON index for\n[IP-MIB.json](http://pysnmp.github.io/json/asn1/IP-MIB),\n[TCP-MIB.json](http://pysnmp.github.io/json/asn1/TCP-MIB) and\n[UDP-MIB.json](http://pysnmp.github.io/json/asn1/UDP-MIB)\nmodules would keep information like this:\n\n```\n   {\n      "compliance": {\n         "1.3.6.1.2.1.48.2.1.1": [\n           "IP-MIB"\n         ],\n         "1.3.6.1.2.1.49.2.1.1": [\n           "TCP-MIB"\n         ],\n         "1.3.6.1.2.1.50.2.1.1": [\n           "UDP-MIB"\n         ]\n      },\n      "identity": {\n          "1.3.6.1.2.1.48": [\n            "IP-MIB"\n          ],\n          "1.3.6.1.2.1.49": [\n            "TCP-MIB"\n          ],\n          "1.3.6.1.2.1.50": [\n            "UDP-MIB"\n          ]\n      },\n      "oids": {\n          "1.3.6.1.2.1.4": [\n            "IP-MIB"\n          ],\n          "1.3.6.1.2.1.5": [\n            "IP-MIB"\n          ],\n          "1.3.6.1.2.1.6": [\n            "TCP-MIB"\n          ],\n          "1.3.6.1.2.1.7": [\n            "UDP-MIB"\n          ],\n          "1.3.6.1.2.1.49": [\n            "TCP-MIB"\n          ],\n          "1.3.6.1.2.1.50": [\n            "UDP-MIB"\n          ]\n      }\n   }\n```\n\nWith this example, *compliance* and *identity* keys point to\n*MODULE-COMPLIANCE* and *MODULE-IDENTITY* MIB objects, *oids*\nlist top-level OIDs branches defined in MIB modules. Full index\nbuild over thousands of MIBs could be seen\n[here](http://pysnmp.github.io/json/index.json).\n\nThe PySMI library can automatically fetch required MIBs from HTTP, FTP sites\nor local directories. You could configure any MIB source available to you (including\n[https://pysnmp.github.io/mibs/asn1](https://pysnmp.github.io/mibs/asn1)) for that purpose.\n\nHow to get PySMI\n----------------\n\nThe pysmi package is distributed under terms and conditions of 2-clause\nBSD [license](http://snmplabs.com/pysmi/license.html). Source code is freely\navailable as a GitHub [repo](https://github.com/pysnmp/pysmi).\n\nYou could `pip install pysnmp-pysmi` or download it from [PyPI](https://pypi.org/project/pysnmp-pysmi/).\n\nIf something does not work as expected,\n[open an issue](https://github.com/pysnmp/pysmi/issues) at GitHub or\npost your question [on Stack Overflow](http://stackoverflow.com/questions/ask).\n\nCopyright (c) 2015-2020, [Ilya Etingof](mailto:etingof@gmail.com).\nAll rights reserved.\n',
     'author': 'rfaircloth-splunk',
     'author_email': 'rfaircloth@splunk.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/pysnmp/pysmi',
```

### Comparing `pysnmp-pysmi-1.1.7/PKG-INFO` & `pysnmp-pysmi-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysnmp-pysmi
-Version: 1.1.7
+Version: 1.1.8
 Summary: 
 Home-page: https://github.com/pysnmp/pysmi
 License: BSD-2-Clause
 Author: rfaircloth-splunk
 Author-email: rfaircloth@splunk.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

