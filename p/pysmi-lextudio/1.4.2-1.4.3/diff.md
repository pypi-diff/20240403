# Comparing `tmp/pysmi_lextudio-1.4.2.tar.gz` & `tmp/pysmi_lextudio-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysmi_lextudio-1.4.2.tar", max compression
+gzip compressed data, was "pysmi_lextudio-1.4.3.tar", max compression
```

## Comparing `pysmi_lextudio-1.4.2.tar` & `pysmi_lextudio-1.4.3.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0     1393 2024-03-03 19:59:37.388220 pysmi_lextudio-1.4.2/LICENSE.rst
--rw-r--r--   0        0        0     6749 2024-03-18 00:54:20.733734 pysmi_lextudio-1.4.2/README.md
--rw-r--r--   0        0        0     7414 2022-11-10 22:58:18.709426 pysmi_lextudio-1.4.2/docs/Makefile
--rw-r--r--   0        0        0      218 2022-11-10 22:58:18.709486 pysmi_lextudio-1.4.2/docs/README.txt
--rw-r--r--   0        0        0      232 2022-11-10 22:58:18.709639 pysmi_lextudio-1.4.2/docs/source/_static/css/rtdimproved.css
--rw-r--r--   0        0        0     4030 2022-11-10 22:58:18.709709 pysmi_lextudio-1.4.2/docs/source/_static/favicon.ico
--rw-r--r--   0        0        0      143 2024-03-20 02:56:59.834419 pysmi_lextudio-1.4.2/docs/source/_static/google_analytics_tracker.js
--rw-r--r--   0        0        0    13811 2022-11-10 22:58:18.709805 pysmi_lextudio-1.4.2/docs/source/_static/logo.svg
--rw-r--r--   0        0        0     1162 2024-03-21 16:10:05.139171 pysmi_lextudio-1.4.2/docs/source/_templates/page.html
--rw-r--r--   0        0        0       53 2022-11-10 22:58:18.709858 pysmi_lextudio-1.4.2/docs/source/changelog.rst
--rw-r--r--   0        0        0    11404 2024-03-26 02:10:25.762143 pysmi_lextudio-1.4.2/docs/source/conf.py
--rw-r--r--   0        0        0     4066 2024-03-14 23:45:25.236724 pysmi_lextudio-1.4.2/docs/source/docs/api-reference.rst
--rw-r--r--   0        0        0      144 2022-11-10 22:58:18.711083 pysmi_lextudio-1.4.2/docs/source/docs/borrower/anyfile/anyfileborrower.rst
--rw-r--r--   0        0        0      146 2022-11-10 22:58:18.711164 pysmi_lextudio-1.4.2/docs/source/docs/borrower/pyfile/pyfileborrower.rst
--rw-r--r--   0        0        0      146 2022-11-10 22:58:18.711278 pysmi_lextudio-1.4.2/docs/source/docs/codegen/jsondoc/jsoncodegen.rst
--rw-r--r--   0        0        0      134 2022-11-10 22:58:18.711359 pysmi_lextudio-1.4.2/docs/source/docs/codegen/null/nullcodegen.rst
--rw-r--r--   0        0        0      142 2022-11-10 22:58:18.711441 pysmi_lextudio-1.4.2/docs/source/docs/codegen/pysnmp/pysnmpcodegen.rst
--rw-r--r--   0        0        0      109 2022-11-10 22:58:18.711523 pysmi_lextudio-1.4.2/docs/source/docs/compiler/mibcompiler.rst
--rw-r--r--   0        0        0      249 2022-11-10 22:58:18.711580 pysmi_lextudio-1.4.2/docs/source/docs/compiler/mibstatus.rst
--rw-r--r--   0        0        0     4259 2024-03-03 20:09:15.719538 pysmi_lextudio-1.4.2/docs/source/docs/mibcopy.rst
--rw-r--r--   0        0        0    12293 2024-03-03 20:09:22.269505 pysmi_lextudio-1.4.2/docs/source/docs/mibdump.rst
--rw-r--r--   0        0        0     1083 2022-11-10 22:58:18.711701 pysmi_lextudio-1.4.2/docs/source/docs/parser/smi/dialect.rst
--rw-r--r--   0        0        0      992 2022-11-10 22:58:18.711771 pysmi_lextudio-1.4.2/docs/source/docs/parser/smi/parserfactory.rst
--rw-r--r--   0        0        0      217 2022-11-10 22:58:18.711904 pysmi_lextudio-1.4.2/docs/source/docs/reader/callback/callbackreader.rst
--rw-r--r--   0        0        0      202 2022-11-10 22:58:18.712093 pysmi_lextudio-1.4.2/docs/source/docs/reader/httpclient/httpreader.rst
--rw-r--r--   0        0        0      229 2022-11-10 22:58:18.712187 pysmi_lextudio-1.4.2/docs/source/docs/reader/localfile/filereader.rst
--rw-r--r--   0        0        0      267 2022-11-10 22:58:18.712284 pysmi_lextudio-1.4.2/docs/source/docs/reader/zipreader/zipreader.rst
--rw-r--r--   0        0        0      260 2022-11-10 22:58:18.712428 pysmi_lextudio-1.4.2/docs/source/docs/searcher/pyfile/pyfilesearcher.rst
--rw-r--r--   0        0        0      317 2022-11-10 22:58:18.712522 pysmi_lextudio-1.4.2/docs/source/docs/searcher/pypackage/pypackagesearcher.rst
--rw-r--r--   0        0        0      468 2022-11-10 22:58:18.712628 pysmi_lextudio-1.4.2/docs/source/docs/searcher/stub/stubsearcher.rst
--rw-r--r--   0        0        0      232 2022-11-10 22:58:18.712777 pysmi_lextudio-1.4.2/docs/source/docs/writer/callback/callbackwriter.rst
--rw-r--r--   0        0        0      121 2022-11-10 22:58:18.712881 pysmi_lextudio-1.4.2/docs/source/docs/writer/localfile/filewriter.rst
--rw-r--r--   0        0        0      133 2022-11-10 22:58:18.712980 pysmi_lextudio-1.4.2/docs/source/docs/writer/pyfile/pyfilewriter.rst
--rw-r--r--   0        0        0      707 2024-03-03 19:58:02.541295 pysmi_lextudio-1.4.2/docs/source/download.rst
--rw-r--r--   0        0        0      329 2024-03-02 21:30:01.122321 pysmi_lextudio-1.4.2/docs/source/examples/always-borrow-precompiled-pysnmp-files.rst
--rw-r--r--   0        0        0      341 2024-03-02 21:30:01.122907 pysmi_lextudio-1.4.2/docs/source/examples/borrow-precompiled-pysnmp-files-on-failure.rst
--rw-r--r--   0        0        0      359 2024-03-02 21:30:01.123447 pysmi_lextudio-1.4.2/docs/source/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.rst
--rw-r--r--   0        0        0      350 2024-03-02 21:30:01.123861 pysmi_lextudio-1.4.2/docs/source/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.rst
--rw-r--r--   0        0        0      344 2024-03-02 21:30:01.124277 pysmi_lextudio-1.4.2/docs/source/examples/download-and-compile-smistar-mibs-into-json.rst
--rw-r--r--   0        0        0      368 2024-03-02 21:30:01.124652 pysmi_lextudio-1.4.2/docs/source/examples/download-and-compile-smistar-mibs-into-pysnmp-files.rst
--rw-r--r--   0        0        0     1688 2024-03-03 19:57:15.957101 pysmi_lextudio-1.4.2/docs/source/includes/_links.rst
--rw-r--r--   0        0        0     4374 2024-03-25 05:22:51.472248 pysmi_lextudio-1.4.2/docs/source/index.rst
--rw-r--r--   0        0        0       49 2022-11-10 22:58:18.710745 pysmi_lextudio-1.4.2/docs/source/license.rst
--rw-r--r--   0        0        0     6406 2024-03-20 04:33:17.459386 pysmi_lextudio-1.4.2/docs/source/quick-start.rst
--rw-r--r--   0        0        0     1968 2024-03-20 04:33:22.418416 pysmi_lextudio-1.4.2/docs/source/troubleshooting.rst
--rw-r--r--   0        0        0     1171 2024-03-14 23:45:41.722612 pysmi_lextudio-1.4.2/examples/always-borrow-precompiled-pysnmp-files.py
--rw-r--r--   0        0        0     1666 2024-03-15 07:08:54.599939 pysmi_lextudio-1.4.2/examples/borrow-precompiled-pysnmp-files-on-failure.py
--rw-r--r--   0        0        0     1864 2024-03-14 23:46:38.663074 pysmi_lextudio-1.4.2/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.py
--rw-r--r--   0        0        0     1343 2024-03-14 23:46:50.174172 pysmi_lextudio-1.4.2/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.py
--rw-r--r--   0        0        0     1465 2024-03-15 07:11:40.889129 pysmi_lextudio-1.4.2/examples/download-and-compile-smistar-mibs-into-json.py
--rw-r--r--   0        0        0     1386 2024-03-14 23:47:24.805594 pysmi_lextudio-1.4.2/examples/download-and-compile-smistar-mibs-into-pysnmp-files.py
--rw-r--r--   0        0        0     1695 2024-03-26 02:10:25.743102 pysmi_lextudio-1.4.2/pyproject.toml
--rw-r--r--   0        0        0       65 2024-03-26 02:10:25.761131 pysmi_lextudio-1.4.2/pysmi/__init__.py
--rw-r--r--   0        0        0      258 2024-03-02 20:37:00.057929 pysmi_lextudio-1.4.2/pysmi/borrower/__init__.py
--rw-r--r--   0        0        0      303 2024-03-02 20:36:21.940312 pysmi_lextudio-1.4.2/pysmi/borrower/anyfile.py
--rw-r--r--   0        0        0     1614 2024-03-14 23:22:43.516346 pysmi_lextudio-1.4.2/pysmi/borrower/base.py
--rw-r--r--   0        0        0      596 2024-03-02 21:27:03.643240 pysmi_lextudio-1.4.2/pysmi/borrower/pyfile.py
--rw-r--r--   0        0        0      294 2024-03-02 21:26:35.316735 pysmi_lextudio-1.4.2/pysmi/codegen/__init__.py
--rw-r--r--   0        0        0    15766 2024-03-02 21:26:35.443382 pysmi_lextudio-1.4.2/pysmi/codegen/base.py
--rw-r--r--   0        0        0    34408 2024-03-26 01:12:31.398896 pysmi_lextudio-1.4.2/pysmi/codegen/intermediate.py
--rw-r--r--   0        0        0      256 2024-03-02 20:58:05.531069 pysmi_lextudio-1.4.2/pysmi/codegen/jfilters.py
--rw-r--r--   0        0        0     5324 2024-03-15 07:42:39.028123 pysmi_lextudio-1.4.2/pysmi/codegen/jsondoc.py
--rw-r--r--   0        0        0      705 2024-03-15 07:42:38.919028 pysmi_lextudio-1.4.2/pysmi/codegen/null.py
--rw-r--r--   0        0        0     5532 2024-03-15 05:54:06.690898 pysmi_lextudio-1.4.2/pysmi/codegen/pysnmp.py
--rw-r--r--   0        0        0    22072 2024-03-26 01:12:31.415909 pysmi_lextudio-1.4.2/pysmi/codegen/symtable.py
--rw-r--r--   0        0        0       62 2024-03-02 19:37:21.647269 pysmi_lextudio-1.4.2/pysmi/codegen/templates/jsondoc/base.j2
--rw-r--r--   0        0        0      557 2024-03-18 01:09:07.596350 pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/base.j2
--rw-r--r--   0        0        0     3545 2024-03-02 19:38:43.699737 pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/managed-objects-instances.j2
--rw-r--r--   0        0        0    19012 2024-03-02 19:39:48.820829 pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/mib-definitions.j2
--rw-r--r--   0        0        0     6298 2024-03-02 20:58:05.572316 pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/mib-instrumentation/managed-objects-instances.j2
--rw-r--r--   0        0        0     5847 2024-03-02 20:58:05.573546 pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/mib-instrumentation/managed-objects.j2
--rw-r--r--   0        0        0      365 2024-03-02 21:27:18.237828 pysmi_lextudio-1.4.2/pysmi/compat.py
--rw-r--r--   0        0        0    22502 2024-03-18 01:25:08.509433 pysmi_lextudio-1.4.2/pysmi/compiler.py
--rw-r--r--   0        0        0      318 2024-03-26 01:12:31.417397 pysmi_lextudio-1.4.2/pysmi/config.py
--rw-r--r--   0        0        0     3436 2024-03-14 23:49:39.494053 pysmi_lextudio-1.4.2/pysmi/debug.py
--rw-r--r--   0        0        0     1710 2024-03-15 07:36:28.536646 pysmi_lextudio-1.4.2/pysmi/error.py
--rw-r--r--   0        0        0      197 2024-03-02 20:36:21.963576 pysmi_lextudio-1.4.2/pysmi/lexer/__init__.py
--rw-r--r--   0        0        0      238 2024-03-02 20:36:21.963558 pysmi_lextudio-1.4.2/pysmi/lexer/base.py
--rw-r--r--   0        0        0    13398 2024-03-26 02:09:53.451037 pysmi_lextudio-1.4.2/pysmi/lexer/smi.py
--rw-r--r--   0        0        0      817 2024-03-02 21:27:18.246818 pysmi_lextudio-1.4.2/pysmi/mibinfo.py
--rw-r--r--   0        0        0      355 2024-03-02 20:36:21.963602 pysmi_lextudio-1.4.2/pysmi/parser/__init__.py
--rw-r--r--   0        0        0      313 2024-03-02 20:36:21.963617 pysmi_lextudio-1.4.2/pysmi/parser/base.py
--rw-r--r--   0        0        0      624 2024-03-02 21:28:00.067993 pysmi_lextudio-1.4.2/pysmi/parser/dialect.py
--rw-r--r--   0        0        0      399 2024-03-02 21:28:00.067027 pysmi_lextudio-1.4.2/pysmi/parser/null.py
--rw-r--r--   0        0        0    45140 2024-03-15 05:55:54.089858 pysmi_lextudio-1.4.2/pysmi/parser/smi.py
--rw-r--r--   0        0        0      299 2024-03-02 20:36:22.015087 pysmi_lextudio-1.4.2/pysmi/parser/smiv1.py
--rw-r--r--   0        0        0      353 2024-03-02 20:36:22.015144 pysmi_lextudio-1.4.2/pysmi/parser/smiv1compat.py
--rw-r--r--   0        0        0      299 2024-03-02 20:36:22.015040 pysmi_lextudio-1.4.2/pysmi/parser/smiv2.py
--rw-r--r--   0        0        0      393 2024-03-02 20:36:22.015067 pysmi_lextudio-1.4.2/pysmi/reader/__init__.py
--rw-r--r--   0        0        0     1457 2024-03-02 21:25:51.732165 pysmi_lextudio-1.4.2/pysmi/reader/base.py
--rw-r--r--   0        0        0     1604 2024-03-02 21:25:51.729226 pysmi_lextudio-1.4.2/pysmi/reader/callback.py
--rw-r--r--   0        0        0     3789 2024-03-15 06:06:49.851956 pysmi_lextudio-1.4.2/pysmi/reader/httpclient.py
--rw-r--r--   0        0        0     5172 2024-03-15 05:57:50.070669 pysmi_lextudio-1.4.2/pysmi/reader/localfile.py
--rw-r--r--   0        0        0     1342 2024-03-14 23:50:06.262567 pysmi_lextudio-1.4.2/pysmi/reader/url.py
--rw-r--r--   0        0        0     5826 2024-03-15 06:04:19.379607 pysmi_lextudio-1.4.2/pysmi/reader/zipreader.py
--rw-r--r--   0        0        0    10073 2024-03-15 08:00:45.476444 pysmi_lextudio-1.4.2/pysmi/scripts/mibcopy.py
--rw-r--r--   0        0        0    15388 2024-03-26 01:12:31.699105 pysmi_lextudio-1.4.2/pysmi/scripts/mibdump.py
--rw-r--r--   0        0        0      358 2024-03-02 20:36:22.015418 pysmi_lextudio-1.4.2/pysmi/searcher/__init__.py
--rw-r--r--   0        0        0     2023 2024-03-15 05:59:33.826153 pysmi_lextudio-1.4.2/pysmi/searcher/anyfile.py
--rw-r--r--   0        0        0      399 2024-03-02 21:26:13.610708 pysmi_lextudio-1.4.2/pysmi/searcher/base.py
--rw-r--r--   0        0        0     3930 2024-03-15 07:42:39.020346 pysmi_lextudio-1.4.2/pysmi/searcher/pyfile.py
--rw-r--r--   0        0        0     5436 2024-03-15 07:42:39.071541 pysmi_lextudio-1.4.2/pysmi/searcher/pypackage.py
--rw-r--r--   0        0        0     1279 2024-03-15 07:23:27.338835 pysmi_lextudio-1.4.2/pysmi/searcher/stub.py
--rw-r--r--   0        0        0      298 2024-03-02 20:36:22.015326 pysmi_lextudio-1.4.2/pysmi/writer/__init__.py
--rw-r--r--   0        0        0      475 2024-03-02 21:25:26.206974 pysmi_lextudio-1.4.2/pysmi/writer/base.py
--rw-r--r--   0        0        0     1553 2024-03-14 23:50:38.638870 pysmi_lextudio-1.4.2/pysmi/writer/callback.py
--rw-r--r--   0        0        0     2669 2024-03-15 07:17:34.470206 pysmi_lextudio-1.4.2/pysmi/writer/localfile.py
--rw-r--r--   0        0        0     3291 2024-03-15 07:24:55.175667 pysmi_lextudio-1.4.2/pysmi/writer/pyfile.py
--rw-r--r--   0        0        0       59 2024-03-04 16:49:01.391040 pysmi_lextudio-1.4.2/tests/__init__.py
--rw-r--r--   0        0        0     1010 2024-03-04 16:49:01.391837 pysmi_lextudio-1.4.2/tests/__main__.py
--rwxr-xr-x   0        0        0    70680 2024-03-02 20:19:01.884677 pysmi_lextudio-1.4.2/tests/data/asn1/MIKROTIK-MIB
--rw-r--r--   0        0        0     2711 2024-03-04 16:49:01.392218 pysmi_lextudio-1.4.2/tests/test_agentcapabilities_smiv2_pysnmp.py
--rw-r--r--   0        0        0     1640 2024-03-04 16:49:01.392555 pysmi_lextudio-1.4.2/tests/test_imports_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2295 2024-03-04 16:49:01.392938 pysmi_lextudio-1.4.2/tests/test_modulecompliance_smiv2_pysnmp.py
--rw-r--r--   0        0        0     3349 2024-03-04 16:49:01.393247 pysmi_lextudio-1.4.2/tests/test_moduleidentity_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2360 2024-03-04 16:49:01.393640 pysmi_lextudio-1.4.2/tests/test_notificationgroup_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2278 2024-03-04 16:49:01.393885 pysmi_lextudio-1.4.2/tests/test_notificationtype_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2460 2024-03-04 16:49:01.394115 pysmi_lextudio-1.4.2/tests/test_objectgroup_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2188 2024-03-04 16:49:01.394394 pysmi_lextudio-1.4.2/tests/test_objectidentity_smiv2_pysnmp.py
--rw-r--r--   0        0        0    18349 2024-03-04 16:49:01.394633 pysmi_lextudio-1.4.2/tests/test_objecttype_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2397 2024-03-04 16:49:01.395035 pysmi_lextudio-1.4.2/tests/test_smiv1_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2255 2024-03-04 16:49:01.395248 pysmi_lextudio-1.4.2/tests/test_traptype_smiv2_pysnmp.py
--rw-r--r--   0        0        0     3082 2024-03-14 23:51:16.712683 pysmi_lextudio-1.4.2/tests/test_typedeclaration_smiv1_pysnmp.py
--rw-r--r--   0        0        0     5598 2024-03-14 23:51:28.509868 pysmi_lextudio-1.4.2/tests/test_typedeclaration_smiv2_pysnmp.py
--rw-r--r--   0        0        0     2657 2024-03-04 16:49:01.395999 pysmi_lextudio-1.4.2/tests/test_valuedeclaration_smiv2_pysnmp.py
--rw-r--r--   0        0        0    33763 2024-03-04 16:49:01.396461 pysmi_lextudio-1.4.2/tests/test_zipreader.py
--rw-r--r--   0        0        0     8161 1970-01-01 00:00:00.000000 pysmi_lextudio-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1393 2024-04-03 15:23:11.772383 pysmi_lextudio-1.4.3/LICENSE.rst
+-rw-r--r--   0        0        0     6749 2024-04-03 15:23:11.787164 pysmi_lextudio-1.4.3/README.md
+-rw-r--r--   0        0        0     7414 2022-11-10 22:58:18.709426 pysmi_lextudio-1.4.3/docs/Makefile
+-rw-r--r--   0        0        0      218 2022-11-10 22:58:18.709486 pysmi_lextudio-1.4.3/docs/README.txt
+-rw-r--r--   0        0        0      232 2024-04-03 15:23:11.787926 pysmi_lextudio-1.4.3/docs/source/_static/css/rtdimproved.css
+-rw-r--r--   0        0        0     4030 2024-04-03 15:23:11.788210 pysmi_lextudio-1.4.3/docs/source/_static/favicon.ico
+-rw-r--r--   0        0        0      143 2024-04-03 15:23:11.818715 pysmi_lextudio-1.4.3/docs/source/_static/google_analytics_tracker.js
+-rw-r--r--   0        0        0    13811 2024-04-03 15:23:11.819549 pysmi_lextudio-1.4.3/docs/source/_static/logo.svg
+-rw-r--r--   0        0        0     1162 2024-04-03 15:23:11.877289 pysmi_lextudio-1.4.3/docs/source/_templates/page.html
+-rw-r--r--   0        0        0       53 2022-11-10 22:58:18.709858 pysmi_lextudio-1.4.3/docs/source/changelog.rst
+-rw-r--r--   0        0        0    11436 2024-04-03 15:30:21.659866 pysmi_lextudio-1.4.3/docs/source/conf.py
+-rw-r--r--   0        0        0     4066 2024-04-03 15:23:11.945056 pysmi_lextudio-1.4.3/docs/source/docs/api-reference.rst
+-rw-r--r--   0        0        0      144 2024-04-03 15:23:11.945996 pysmi_lextudio-1.4.3/docs/source/docs/borrower/anyfile/anyfileborrower.rst
+-rw-r--r--   0        0        0      146 2024-04-03 15:23:11.946413 pysmi_lextudio-1.4.3/docs/source/docs/borrower/pyfile/pyfileborrower.rst
+-rw-r--r--   0        0        0      146 2024-04-03 15:23:11.947056 pysmi_lextudio-1.4.3/docs/source/docs/codegen/jsondoc/jsoncodegen.rst
+-rw-r--r--   0        0        0      134 2024-04-03 15:23:11.947835 pysmi_lextudio-1.4.3/docs/source/docs/codegen/null/nullcodegen.rst
+-rw-r--r--   0        0        0      142 2024-04-03 15:23:11.948487 pysmi_lextudio-1.4.3/docs/source/docs/codegen/pysnmp/pysnmpcodegen.rst
+-rw-r--r--   0        0        0      109 2024-04-03 15:23:11.949253 pysmi_lextudio-1.4.3/docs/source/docs/compiler/mibcompiler.rst
+-rw-r--r--   0        0        0      249 2024-04-03 15:23:11.949587 pysmi_lextudio-1.4.3/docs/source/docs/compiler/mibstatus.rst
+-rw-r--r--   0        0        0     4259 2024-04-03 15:23:11.982774 pysmi_lextudio-1.4.3/docs/source/docs/mibcopy.rst
+-rw-r--r--   0        0        0    12293 2024-04-03 15:23:11.987038 pysmi_lextudio-1.4.3/docs/source/docs/mibdump.rst
+-rw-r--r--   0        0        0     1083 2024-04-03 15:23:11.987456 pysmi_lextudio-1.4.3/docs/source/docs/parser/smi/dialect.rst
+-rw-r--r--   0        0        0      992 2024-04-03 15:23:11.987591 pysmi_lextudio-1.4.3/docs/source/docs/parser/smi/parserfactory.rst
+-rw-r--r--   0        0        0      217 2024-04-03 15:23:11.987873 pysmi_lextudio-1.4.3/docs/source/docs/reader/callback/callbackreader.rst
+-rw-r--r--   0        0        0      202 2024-04-03 15:23:11.988323 pysmi_lextudio-1.4.3/docs/source/docs/reader/httpclient/httpreader.rst
+-rw-r--r--   0        0        0      229 2024-04-03 15:23:11.988678 pysmi_lextudio-1.4.3/docs/source/docs/reader/localfile/filereader.rst
+-rw-r--r--   0        0        0      267 2024-04-03 15:23:11.988880 pysmi_lextudio-1.4.3/docs/source/docs/reader/zipreader/zipreader.rst
+-rw-r--r--   0        0        0      260 2024-04-03 15:23:11.989153 pysmi_lextudio-1.4.3/docs/source/docs/searcher/pyfile/pyfilesearcher.rst
+-rw-r--r--   0        0        0      317 2024-04-03 15:23:11.989346 pysmi_lextudio-1.4.3/docs/source/docs/searcher/pypackage/pypackagesearcher.rst
+-rw-r--r--   0        0        0      468 2024-04-03 15:23:11.989539 pysmi_lextudio-1.4.3/docs/source/docs/searcher/stub/stubsearcher.rst
+-rw-r--r--   0        0        0      232 2024-04-03 15:23:11.989797 pysmi_lextudio-1.4.3/docs/source/docs/writer/callback/callbackwriter.rst
+-rw-r--r--   0        0        0      121 2024-04-03 15:23:11.990000 pysmi_lextudio-1.4.3/docs/source/docs/writer/localfile/filewriter.rst
+-rw-r--r--   0        0        0      133 2024-04-03 15:23:11.990193 pysmi_lextudio-1.4.3/docs/source/docs/writer/pyfile/pyfilewriter.rst
+-rw-r--r--   0        0        0      707 2024-04-03 15:23:11.992521 pysmi_lextudio-1.4.3/docs/source/download.rst
+-rw-r--r--   0        0        0      329 2024-04-03 15:23:11.994381 pysmi_lextudio-1.4.3/docs/source/examples/always-borrow-precompiled-pysnmp-files.rst
+-rw-r--r--   0        0        0      341 2024-04-03 15:23:11.996700 pysmi_lextudio-1.4.3/docs/source/examples/borrow-precompiled-pysnmp-files-on-failure.rst
+-rw-r--r--   0        0        0      359 2024-04-03 15:23:11.999254 pysmi_lextudio-1.4.3/docs/source/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.rst
+-rw-r--r--   0        0        0      350 2024-04-03 15:23:12.001933 pysmi_lextudio-1.4.3/docs/source/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.rst
+-rw-r--r--   0        0        0      344 2024-04-03 15:23:12.004037 pysmi_lextudio-1.4.3/docs/source/examples/download-and-compile-smistar-mibs-into-json.rst
+-rw-r--r--   0        0        0      368 2024-04-03 15:23:12.007357 pysmi_lextudio-1.4.3/docs/source/examples/download-and-compile-smistar-mibs-into-pysnmp-files.rst
+-rw-r--r--   0        0        0     1688 2024-04-03 15:23:12.009242 pysmi_lextudio-1.4.3/docs/source/includes/_links.rst
+-rw-r--r--   0        0        0     4374 2024-04-03 15:23:12.011573 pysmi_lextudio-1.4.3/docs/source/index.rst
+-rw-r--r--   0        0        0       49 2022-11-10 22:58:18.710745 pysmi_lextudio-1.4.3/docs/source/license.rst
+-rw-r--r--   0        0        0     6406 2024-04-03 15:23:12.014829 pysmi_lextudio-1.4.3/docs/source/quick-start.rst
+-rw-r--r--   0        0        0     1968 2024-04-03 15:23:12.018889 pysmi_lextudio-1.4.3/docs/source/troubleshooting.rst
+-rw-r--r--   0        0        0     1171 2024-04-03 15:23:12.020563 pysmi_lextudio-1.4.3/examples/always-borrow-precompiled-pysnmp-files.py
+-rw-r--r--   0        0        0     1666 2024-04-03 15:23:12.024276 pysmi_lextudio-1.4.3/examples/borrow-precompiled-pysnmp-files-on-failure.py
+-rw-r--r--   0        0        0     1864 2024-04-03 15:23:12.025745 pysmi_lextudio-1.4.3/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.py
+-rw-r--r--   0        0        0     1343 2024-04-03 15:23:12.027054 pysmi_lextudio-1.4.3/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.py
+-rw-r--r--   0        0        0     1465 2024-04-03 15:23:12.030505 pysmi_lextudio-1.4.3/examples/download-and-compile-smistar-mibs-into-json.py
+-rw-r--r--   0        0        0     1386 2024-04-03 15:23:12.032481 pysmi_lextudio-1.4.3/examples/download-and-compile-smistar-mibs-into-pysnmp-files.py
+-rw-r--r--   0        0        0     1720 2024-04-03 15:30:21.645835 pysmi_lextudio-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-04-03 15:30:21.659191 pysmi_lextudio-1.4.3/pysmi/__init__.py
+-rw-r--r--   0        0        0      258 2024-04-03 15:23:12.095814 pysmi_lextudio-1.4.3/pysmi/borrower/__init__.py
+-rw-r--r--   0        0        0      303 2024-04-03 15:23:12.097179 pysmi_lextudio-1.4.3/pysmi/borrower/anyfile.py
+-rw-r--r--   0        0        0     1614 2024-04-03 15:23:12.102901 pysmi_lextudio-1.4.3/pysmi/borrower/base.py
+-rw-r--r--   0        0        0      596 2024-04-03 15:23:12.110386 pysmi_lextudio-1.4.3/pysmi/borrower/pyfile.py
+-rw-r--r--   0        0        0      294 2024-04-03 15:23:12.193856 pysmi_lextudio-1.4.3/pysmi/codegen/__init__.py
+-rw-r--r--   0        0        0    15766 2024-04-03 15:23:12.200600 pysmi_lextudio-1.4.3/pysmi/codegen/base.py
+-rw-r--r--   0        0        0    34408 2024-04-03 15:23:12.246281 pysmi_lextudio-1.4.3/pysmi/codegen/intermediate.py
+-rw-r--r--   0        0        0      256 2024-04-03 15:23:12.249414 pysmi_lextudio-1.4.3/pysmi/codegen/jfilters.py
+-rw-r--r--   0        0        0     5324 2024-04-03 15:23:12.307595 pysmi_lextudio-1.4.3/pysmi/codegen/jsondoc.py
+-rw-r--r--   0        0        0      705 2024-04-03 15:23:12.353884 pysmi_lextudio-1.4.3/pysmi/codegen/null.py
+-rw-r--r--   0        0        0     5532 2024-04-03 15:23:12.367822 pysmi_lextudio-1.4.3/pysmi/codegen/pysnmp.py
+-rw-r--r--   0        0        0    22072 2024-04-03 15:23:12.375896 pysmi_lextudio-1.4.3/pysmi/codegen/symtable.py
+-rw-r--r--   0        0        0       62 2024-03-02 19:37:21.647269 pysmi_lextudio-1.4.3/pysmi/codegen/templates/jsondoc/base.j2
+-rw-r--r--   0        0        0      557 2024-04-03 15:23:12.415756 pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/base.j2
+-rw-r--r--   0        0        0     3545 2024-03-02 19:38:43.699737 pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/managed-objects-instances.j2
+-rw-r--r--   0        0        0    19012 2024-03-02 19:39:48.820829 pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/mib-definitions.j2
+-rw-r--r--   0        0        0     6298 2024-04-03 15:23:12.422765 pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/mib-instrumentation/managed-objects-instances.j2
+-rw-r--r--   0        0        0     5847 2024-04-03 15:23:12.429973 pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/mib-instrumentation/managed-objects.j2
+-rw-r--r--   0        0        0      365 2024-04-03 15:23:12.512384 pysmi_lextudio-1.4.3/pysmi/compat.py
+-rw-r--r--   0        0        0    22502 2024-04-03 15:23:12.564607 pysmi_lextudio-1.4.3/pysmi/compiler.py
+-rw-r--r--   0        0        0      318 2024-04-03 15:23:12.570744 pysmi_lextudio-1.4.3/pysmi/config.py
+-rw-r--r--   0        0        0     3436 2024-04-03 15:23:12.618754 pysmi_lextudio-1.4.3/pysmi/debug.py
+-rw-r--r--   0        0        0     1710 2024-04-03 15:23:12.634093 pysmi_lextudio-1.4.3/pysmi/error.py
+-rw-r--r--   0        0        0      197 2024-04-03 15:23:12.634864 pysmi_lextudio-1.4.3/pysmi/lexer/__init__.py
+-rw-r--r--   0        0        0      238 2024-04-03 15:23:12.635425 pysmi_lextudio-1.4.3/pysmi/lexer/base.py
+-rw-r--r--   0        0        0    13398 2024-04-03 15:23:12.669583 pysmi_lextudio-1.4.3/pysmi/lexer/smi.py
+-rw-r--r--   0        0        0      817 2024-04-03 15:23:12.674085 pysmi_lextudio-1.4.3/pysmi/mibinfo.py
+-rw-r--r--   0        0        0      355 2024-04-03 15:23:12.674991 pysmi_lextudio-1.4.3/pysmi/parser/__init__.py
+-rw-r--r--   0        0        0      313 2024-04-03 15:23:12.675754 pysmi_lextudio-1.4.3/pysmi/parser/base.py
+-rw-r--r--   0        0        0      624 2024-04-03 15:23:12.681146 pysmi_lextudio-1.4.3/pysmi/parser/dialect.py
+-rw-r--r--   0        0        0      399 2024-04-03 15:23:12.720372 pysmi_lextudio-1.4.3/pysmi/parser/null.py
+-rw-r--r--   0        0        0    45140 2024-04-03 15:23:12.774931 pysmi_lextudio-1.4.3/pysmi/parser/smi.py
+-rw-r--r--   0        0        0      299 2024-04-03 15:23:12.781847 pysmi_lextudio-1.4.3/pysmi/parser/smiv1.py
+-rw-r--r--   0        0        0      353 2024-04-03 15:23:12.782608 pysmi_lextudio-1.4.3/pysmi/parser/smiv1compat.py
+-rw-r--r--   0        0        0      299 2024-04-03 15:23:12.783308 pysmi_lextudio-1.4.3/pysmi/parser/smiv2.py
+-rw-r--r--   0        0        0      393 2024-04-03 15:23:12.784048 pysmi_lextudio-1.4.3/pysmi/reader/__init__.py
+-rw-r--r--   0        0        0     1457 2024-04-03 15:23:12.836761 pysmi_lextudio-1.4.3/pysmi/reader/base.py
+-rw-r--r--   0        0        0     1604 2024-04-03 15:23:12.840212 pysmi_lextudio-1.4.3/pysmi/reader/callback.py
+-rw-r--r--   0        0        0     3789 2024-04-03 15:23:12.851937 pysmi_lextudio-1.4.3/pysmi/reader/httpclient.py
+-rw-r--r--   0        0        0     5172 2024-04-03 15:23:12.856999 pysmi_lextudio-1.4.3/pysmi/reader/localfile.py
+-rw-r--r--   0        0        0     1342 2024-04-03 15:23:12.862315 pysmi_lextudio-1.4.3/pysmi/reader/url.py
+-rw-r--r--   0        0        0     5826 2024-04-03 15:23:12.865933 pysmi_lextudio-1.4.3/pysmi/reader/zipreader.py
+-rw-r--r--   0        0        0    10073 2024-04-03 15:23:46.217225 pysmi_lextudio-1.4.3/pysmi/scripts/mibcopy.py
+-rw-r--r--   0        0        0    15773 2024-04-03 15:28:05.337218 pysmi_lextudio-1.4.3/pysmi/scripts/mibdump.py
+-rw-r--r--   0        0        0      358 2024-04-03 15:23:12.872204 pysmi_lextudio-1.4.3/pysmi/searcher/__init__.py
+-rw-r--r--   0        0        0     2023 2024-04-03 15:23:12.875421 pysmi_lextudio-1.4.3/pysmi/searcher/anyfile.py
+-rw-r--r--   0        0        0      399 2024-04-03 15:23:12.879625 pysmi_lextudio-1.4.3/pysmi/searcher/base.py
+-rw-r--r--   0        0        0     3930 2024-04-03 15:23:12.882602 pysmi_lextudio-1.4.3/pysmi/searcher/pyfile.py
+-rw-r--r--   0        0        0     5436 2024-04-03 15:23:12.886406 pysmi_lextudio-1.4.3/pysmi/searcher/pypackage.py
+-rw-r--r--   0        0        0     1279 2024-04-03 15:23:12.890559 pysmi_lextudio-1.4.3/pysmi/searcher/stub.py
+-rw-r--r--   0        0        0      298 2024-04-03 15:23:12.891419 pysmi_lextudio-1.4.3/pysmi/writer/__init__.py
+-rw-r--r--   0        0        0      475 2024-04-03 15:23:12.893812 pysmi_lextudio-1.4.3/pysmi/writer/base.py
+-rw-r--r--   0        0        0     1553 2024-04-03 15:23:12.895823 pysmi_lextudio-1.4.3/pysmi/writer/callback.py
+-rw-r--r--   0        0        0     2669 2024-04-03 15:23:12.898444 pysmi_lextudio-1.4.3/pysmi/writer/localfile.py
+-rw-r--r--   0        0        0     3291 2024-04-03 15:23:12.903477 pysmi_lextudio-1.4.3/pysmi/writer/pyfile.py
+-rw-r--r--   0        0        0       59 2024-03-04 16:49:01.391040 pysmi_lextudio-1.4.3/tests/__init__.py
+-rw-r--r--   0        0        0     1010 2024-04-03 15:23:12.906562 pysmi_lextudio-1.4.3/tests/__main__.py
+-rwxr-xr-x   0        0        0    70680 2024-04-03 15:23:12.907010 pysmi_lextudio-1.4.3/tests/data/asn1/MIKROTIK-MIB
+-rw-r--r--   0        0        0     2711 2024-04-03 15:23:12.909688 pysmi_lextudio-1.4.3/tests/test_agentcapabilities_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     1640 2024-04-03 15:23:12.912644 pysmi_lextudio-1.4.3/tests/test_imports_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2295 2024-04-03 15:23:12.915804 pysmi_lextudio-1.4.3/tests/test_modulecompliance_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     3349 2024-04-03 15:23:12.919452 pysmi_lextudio-1.4.3/tests/test_moduleidentity_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2360 2024-04-03 15:23:12.922415 pysmi_lextudio-1.4.3/tests/test_notificationgroup_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2278 2024-04-03 15:23:12.924561 pysmi_lextudio-1.4.3/tests/test_notificationtype_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2460 2024-04-03 15:23:12.926265 pysmi_lextudio-1.4.3/tests/test_objectgroup_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2188 2024-04-03 15:23:12.927772 pysmi_lextudio-1.4.3/tests/test_objectidentity_smiv2_pysnmp.py
+-rw-r--r--   0        0        0    18349 2024-04-03 15:23:12.929477 pysmi_lextudio-1.4.3/tests/test_objecttype_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2397 2024-04-03 15:23:12.932119 pysmi_lextudio-1.4.3/tests/test_smiv1_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2255 2024-04-03 15:23:12.934616 pysmi_lextudio-1.4.3/tests/test_traptype_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     3082 2024-04-03 15:23:12.936617 pysmi_lextudio-1.4.3/tests/test_typedeclaration_smiv1_pysnmp.py
+-rw-r--r--   0        0        0     5598 2024-04-03 15:23:12.938370 pysmi_lextudio-1.4.3/tests/test_typedeclaration_smiv2_pysnmp.py
+-rw-r--r--   0        0        0     2657 2024-04-03 15:23:12.941124 pysmi_lextudio-1.4.3/tests/test_valuedeclaration_smiv2_pysnmp.py
+-rw-r--r--   0        0        0    33763 2024-04-03 15:23:12.944225 pysmi_lextudio-1.4.3/tests/test_zipreader.py
+-rw-r--r--   0        0        0     8111 1970-01-01 00:00:00.000000 pysmi_lextudio-1.4.3/PKG-INFO
```

### Comparing `pysmi_lextudio-1.4.2/LICENSE.rst` & `pysmi_lextudio-1.4.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/README.md` & `pysmi_lextudio-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/Makefile` & `pysmi_lextudio-1.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/_static/favicon.ico` & `pysmi_lextudio-1.4.3/docs/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/_static/logo.svg` & `pysmi_lextudio-1.4.3/docs/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/_templates/page.html` & `pysmi_lextudio-1.4.3/docs/source/_templates/page.html`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/conf.py` & `pysmi_lextudio-1.4.3/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     "sphinx.ext.todo",
     "sphinx_sitemap",
     "sphinx_copybutton",
 ]
 
 html_baseurl = "https://docs.lextudio.com/pysmi/"
 sitemap_url_scheme = "{link}"
+sitemap_suffix_included = False
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 # source_suffix = ['.rst', '.md']
@@ -61,15 +62,15 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = "1.4"
 # The full version, including alpha/beta/rc tags.
-release = "1.4.2"
+release = "1.4.3"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
```

### Comparing `pysmi_lextudio-1.4.2/docs/source/docs/api-reference.rst` & `pysmi_lextudio-1.4.3/docs/source/docs/api-reference.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/docs/mibcopy.rst` & `pysmi_lextudio-1.4.3/docs/source/docs/mibcopy.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/docs/mibdump.rst` & `pysmi_lextudio-1.4.3/docs/source/docs/mibdump.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/docs/parser/smi/dialect.rst` & `pysmi_lextudio-1.4.3/docs/source/docs/parser/smi/dialect.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/docs/parser/smi/parserfactory.rst` & `pysmi_lextudio-1.4.3/docs/source/docs/parser/smi/parserfactory.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/download.rst` & `pysmi_lextudio-1.4.3/docs/source/download.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/includes/_links.rst` & `pysmi_lextudio-1.4.3/docs/source/includes/_links.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/index.rst` & `pysmi_lextudio-1.4.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/quick-start.rst` & `pysmi_lextudio-1.4.3/docs/source/quick-start.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/docs/source/troubleshooting.rst` & `pysmi_lextudio-1.4.3/docs/source/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/examples/always-borrow-precompiled-pysnmp-files.py` & `pysmi_lextudio-1.4.3/examples/always-borrow-precompiled-pysnmp-files.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/examples/borrow-precompiled-pysnmp-files-on-failure.py` & `pysmi_lextudio-1.4.3/examples/borrow-precompiled-pysnmp-files-on-failure.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.py` & `pysmi_lextudio-1.4.3/examples/compile-smistar-mibs-into-pysnmp-files-if-needed.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.py` & `pysmi_lextudio-1.4.3/examples/compile-smiv2-mibs-from-text-into-pysnmp-code.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/examples/download-and-compile-smistar-mibs-into-json.py` & `pysmi_lextudio-1.4.3/examples/download-and-compile-smistar-mibs-into-json.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/examples/download-and-compile-smistar-mibs-into-pysnmp-files.py` & `pysmi_lextudio-1.4.3/examples/download-and-compile-smistar-mibs-into-pysnmp-files.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pyproject.toml` & `pysmi_lextudio-1.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysmi-lextudio"
-version = "1.4.2"
+version = "1.4.3"
 description = "A pure-Python implementation of SNMP/SMI MIB parsing and conversion library."
 authors = ["Ilya Etingof <etingof@gmail.com>", "LeXtudio Inc. <support@lextudio.com>"]
 license = "BSD-2-Clause"
 repository = "https://github.com/lextudio/pysmi"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
@@ -21,32 +21,33 @@
 
 packages = [
     { include = "pysmi" },
 ]
 include = ["docs", "tests", "examples", "scripts"]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 ply = "^3.11"
 Jinja2 = "^3.1.3"
 requests = "^2.26.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pysnmp-lextudio = "^5.0.0"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 black = "=22.3.0"
 pre-commit = "2.21.0"
 isort = "^5.10.1"
 importlib-metadata = { version = ">=0.12", python = "<3.8" }
-sphinx-sitemap = "^2.5.1"
+sphinx-sitemap-lextudio = "^2.5.2"
 sphinx = "^5.0.0"
 furo = "^2023.1.1"
 sphinx-copybutton = "^0.5.2"
+doc8 = "^1.1.1"
 
 [tool.poetry_bumpversion.file."pysmi/__init__.py"]
 
 [tool.poetry_bumpversion.file."docs/source/conf.py"]
 search = "release = \"{current_version}\""
 replace = "release = \"{new_version}\""
```

### Comparing `pysmi_lextudio-1.4.2/pysmi/borrower/base.py` & `pysmi_lextudio-1.4.3/pysmi/borrower/base.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/borrower/pyfile.py` & `pysmi_lextudio-1.4.3/pysmi/borrower/pyfile.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/base.py` & `pysmi_lextudio-1.4.3/pysmi/codegen/base.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/intermediate.py` & `pysmi_lextudio-1.4.3/pysmi/codegen/intermediate.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/jsondoc.py` & `pysmi_lextudio-1.4.3/pysmi/codegen/jsondoc.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/null.py` & `pysmi_lextudio-1.4.3/pysmi/codegen/null.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/pysnmp.py` & `pysmi_lextudio-1.4.3/pysmi/codegen/pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/symtable.py` & `pysmi_lextudio-1.4.3/pysmi/codegen/symtable.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/base.j2` & `pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/base.j2`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/managed-objects-instances.j2` & `pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/managed-objects-instances.j2`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/mib-definitions.j2` & `pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/mib-definitions.j2`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/mib-instrumentation/managed-objects-instances.j2` & `pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/mib-instrumentation/managed-objects-instances.j2`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/codegen/templates/pysnmp/mib-instrumentation/managed-objects.j2` & `pysmi_lextudio-1.4.3/pysmi/codegen/templates/pysnmp/mib-instrumentation/managed-objects.j2`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/compiler.py` & `pysmi_lextudio-1.4.3/pysmi/compiler.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/debug.py` & `pysmi_lextudio-1.4.3/pysmi/debug.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/error.py` & `pysmi_lextudio-1.4.3/pysmi/error.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/lexer/smi.py` & `pysmi_lextudio-1.4.3/pysmi/lexer/smi.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/mibinfo.py` & `pysmi_lextudio-1.4.3/pysmi/mibinfo.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/parser/dialect.py` & `pysmi_lextudio-1.4.3/pysmi/parser/dialect.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/parser/smi.py` & `pysmi_lextudio-1.4.3/pysmi/parser/smi.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/reader/base.py` & `pysmi_lextudio-1.4.3/pysmi/reader/base.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/reader/callback.py` & `pysmi_lextudio-1.4.3/pysmi/reader/callback.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/reader/httpclient.py` & `pysmi_lextudio-1.4.3/pysmi/reader/httpclient.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/reader/localfile.py` & `pysmi_lextudio-1.4.3/pysmi/reader/localfile.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/reader/url.py` & `pysmi_lextudio-1.4.3/pysmi/reader/url.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/reader/zipreader.py` & `pysmi_lextudio-1.4.3/pysmi/reader/zipreader.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/scripts/mibcopy.py` & `pysmi_lextudio-1.4.3/pysmi/scripts/mibcopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # This file is part of pysmi software.
 #
-# Copyright (c) 2015-2019, Ilya Etingof <etingof@gmail.com>
+# Copyright (c) 2015-2020, Ilya Etingof <etingof@gmail.com>
 # License: https://www.pysnmp.com/pysmi/license.html
 #
 # SNMP SMI/MIB copying tool
 #
 import os
 import sys
 import getopt
```

### Comparing `pysmi_lextudio-1.4.2/pysmi/scripts/mibdump.py` & `pysmi_lextudio-1.4.3/pysmi/scripts/mibdump.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 #
 # This file is part of pysmi software.
 #
-# Copyright (c) 2015-2019, Ilya Etingof <etingof@gmail.com>
+# Copyright (c) 2015-2020, Ilya Etingof <etingof@gmail.com>
 # License: https://www.pysnmp.com/pysmi/license.html
 #
 # SNMP SMI/MIB data management tool
 #
 import os
 import sys
 import getopt
@@ -38,14 +38,15 @@
     verboseFlag = True
     mibSources = []
     doFuzzyMatchingFlag = True
     mibSearchers = []
     mibStubs = []
     mibBorrowers = []
     dstFormat = None
+    dstTemplate = None
     dstDirectory = None
     cacheDirectory = ""
     nodepsFlag = False
     rebuildFlag = False
     dryrunFlag = False
     genMibTextsFlag = False
     keepTextsLayout = False
@@ -62,14 +63,15 @@
         [--strict]
         [--debug=<{"|".join(sorted(debug.flagMap))}>]
         [--mib-source=<URI>]
         [--mib-searcher=<PATH|PACKAGE>]
         [--mib-stub=<MIB-NAME>]
         [--mib-borrower=<PATH>]
         [--destination-format=<FORMAT>]
+        [--destination-template=<PATH>]
         [--destination-directory=<DIRECTORY>]
         [--cache-directory=<DIRECTORY>]
         [--disable-fuzzy-source]
         [--no-dependencies]
         [--no-python-compile]
         [--python-optimization-level]
         [--ignore-errors]
@@ -81,15 +83,17 @@
         [--keep-texts-layout]
         <MIB-NAME> [MIB-NAME [...]]]
     Where:
         URI      - file, zip, http, https schemes are supported.
                 Use @mib@ placeholder token in URI to refer directly to
                 the required MIB module when source does not support
                 directory listing (e.g. HTTP).
-        FORMAT   - pysnmp, json, null"""
+        FORMAT   - pysnmp, json, null
+        TEMPLATE - path to a Jinja2 template extending the base one (see
+                documentation for details)"""
 
     try:
         opts, inputMibs = getopt.getopt(
             sys.argv[1:],
             "hv",
             [
                 "help",
@@ -98,14 +102,15 @@
                 "strict",
                 "debug=",
                 "mib-source=",
                 "mib-searcher=",
                 "mib-stub=",
                 "mib-borrower=",
                 "destination-format=",
+                "destination-template=",
                 "destination-directory=",
                 "cache-directory=",
                 "no-dependencies",
                 "no-python-compile",
                 "python-optimization-level=",
                 "ignore-errors",
                 "build-index",
@@ -172,14 +177,17 @@
 
         if opt[0] == "--mib-borrower":
             mibBorrowers.append((opt[1], genMibTextsFlag))
 
         if opt[0] == "--destination-format":
             dstFormat = opt[1]
 
+        if opt[0] == "--destination-template":
+            dstTemplate = opt[1]
+
         if opt[0] == "--destination-directory":
             dstDirectory = opt[1]
 
         if opt[0] == "--cache-directory":
             cacheDirectory = opt[1]
 
         if opt[0] == "--no-dependencies":
@@ -376,14 +384,15 @@
 Source MIB repositories: {', '.join(mibSources)}
 Borrow missing/failed MIBs from: {', '.join([x[0] for x in mibBorrowers if x[1] == genMibTextsFlag])}
 Existing/compiled MIB locations: {', '.join(mibSearchers)}
 Compiled MIBs destination directory: {dstDirectory}
 MIBs excluded from code generation: {', '.join(sorted(mibStubs))}
 MIBs to compile: {', '.join(inputMibs)}
 Destination format: {dstFormat}
+Custom destination template: {dstTemplate}
 Parser grammar cache directory: {cacheDirectory or "not used"}
 Also compile all relevant MIBs: {"no" if nodepsFlag else "yes"}
 Rebuild MIBs regardless of age: {"yes" if rebuildFlag else "no"}
 Dry run mode: {"yes" if dryrunFlag else "no"}
 Create/update MIBs: {"yes" if writeMibsFlag else "no"}
 Byte-compile Python modules: {"yes" if dstFormat == "pysnmp" and pyCompileFlag else "no"} (optimization level {"yes" if dstFormat == "pysnmp" and pyOptimizationLevel else "no"})
 Ignore compilation errors: {"yes" if ignoreErrorsFlag else "no"}
@@ -411,14 +420,15 @@
 
         processed = mibCompiler.compile(
             *inputMibs,
             **dict(
                 noDeps=nodepsFlag,
                 rebuild=rebuildFlag,
                 dryRun=dryrunFlag,
+                dstTemplate=dstTemplate,
                 genTexts=genMibTextsFlag,
                 textFilter=keepTextsLayout and (lambda symbol, text: text) or None,
                 writeMibs=writeMibsFlag,
                 ignoreErrors=ignoreErrorsFlag,
             ),
         )
```

### Comparing `pysmi_lextudio-1.4.2/pysmi/searcher/anyfile.py` & `pysmi_lextudio-1.4.3/pysmi/searcher/anyfile.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/searcher/pyfile.py` & `pysmi_lextudio-1.4.3/pysmi/searcher/pyfile.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/searcher/pypackage.py` & `pysmi_lextudio-1.4.3/pysmi/searcher/pypackage.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/searcher/stub.py` & `pysmi_lextudio-1.4.3/pysmi/searcher/stub.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/writer/callback.py` & `pysmi_lextudio-1.4.3/pysmi/writer/callback.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/writer/localfile.py` & `pysmi_lextudio-1.4.3/pysmi/writer/localfile.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/pysmi/writer/pyfile.py` & `pysmi_lextudio-1.4.3/pysmi/writer/pyfile.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/__main__.py` & `pysmi_lextudio-1.4.3/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/data/asn1/MIKROTIK-MIB` & `pysmi_lextudio-1.4.3/tests/data/asn1/MIKROTIK-MIB`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_agentcapabilities_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_agentcapabilities_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_imports_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_imports_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_modulecompliance_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_modulecompliance_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_moduleidentity_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_moduleidentity_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_notificationgroup_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_notificationgroup_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_notificationtype_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_notificationtype_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_objectgroup_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_objectgroup_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_objectidentity_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_objectidentity_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_objecttype_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_objecttype_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_smiv1_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_smiv1_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_traptype_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_traptype_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_typedeclaration_smiv1_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_typedeclaration_smiv1_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_typedeclaration_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_typedeclaration_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_valuedeclaration_smiv2_pysnmp.py` & `pysmi_lextudio-1.4.3/tests/test_valuedeclaration_smiv2_pysnmp.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/tests/test_zipreader.py` & `pysmi_lextudio-1.4.3/tests/test_zipreader.py`

 * *Files identical despite different names*

### Comparing `pysmi_lextudio-1.4.2/PKG-INFO` & `pysmi_lextudio-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: pysmi-lextudio
-Version: 1.4.2
+Version: 1.4.3
 Summary: A pure-Python implementation of SNMP/SMI MIB parsing and conversion library.
 Home-page: https://github.com/lextudio/pysmi
 License: BSD-2-Clause
 Author: Ilya Etingof
 Author-email: etingof@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

