# Comparing `tmp/talisman-tools-0.6.2.tar.gz` & `tmp/talisman-tools-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "talisman-tools-0.6.2.tar", last modified: Wed Mar 20 12:52:55 2024, max compression
+gzip compressed data, was "talisman-tools-0.6.3.tar", last modified: Wed Apr  3 08:39:21 2024, max compression
```

## Comparing `talisman-tools-0.6.2.tar` & `talisman-tools-0.6.3.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:55.014146 talisman-tools-0.6.2/
--rw-r--r--   0 root         (0) root         (0)      713 2024-03-20 12:52:55.014146 talisman-tools-0.6.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/README.md
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-03-19 10:09:27.000000 talisman-tools-0.6.2/VERSION
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-20 12:52:55.014146 talisman-tools-0.6.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1665 2024-03-20 12:41:59.000000 talisman-tools-0.6.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.966147 talisman-tools-0.6.2/talisman_tools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/talisman_tools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       35 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.966147 talisman-tools-0.6.2/talisman_tools/arguments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/talisman_tools/arguments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/arguments/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/arguments/loader.py
--rw-rw-rw-   0 root         (0) root         (0)     1461 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/arguments/processor.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/arguments/reader.py
--rw-rw-rw-   0 root         (0) root         (0)      834 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/arguments/serializer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.966147 talisman-tools-0.6.2/talisman_tools/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.966147 talisman-tools-0.6.2/talisman_tools/commands/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/dataset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.966147 talisman-tools-0.6.2/talisman_tools/commands/dataset/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/dataset/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.966147 talisman-tools-0.6.2/talisman_tools/commands/dataset/commands/convert/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/dataset/commands/convert/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/dataset/commands/convert/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      360 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/dataset/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      667 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/dataset/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.966147 talisman-tools-0.6.2/talisman_tools/commands/model/
--rw-rw-rw-   0 root         (0) root         (0)       82 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.970147 talisman-tools-0.6.2/talisman_tools/commands/model/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.970147 talisman-tools-0.6.2/talisman_tools/commands/model/commands/check_performance/
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/check_performance/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2893 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/check_performance/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/check_performance/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.970147 talisman-tools-0.6.2/talisman_tools/commands/model/commands/configure/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/configure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/configure/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.970147 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/
--rw-rw-rw-   0 root         (0) root         (0)       88 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3605 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/action.py
--rw-rw-rw-   0 root         (0) root         (0)     4892 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.970147 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/
--rw-rw-rw-   0 root         (0) root         (0)      708 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5244 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/disambiguation_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1821 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/nerc.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/relext.py
--rw-rw-rw-   0 root         (0) root         (0)     5278 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)    15234 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1322 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.970147 talisman-tools-0.6.2/talisman_tools/commands/model/commands/process/
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/process/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      607 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/process/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/process/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      978 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/model/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.990146 talisman-tools-0.6.2/talisman_tools/commands/servers/
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.990146 talisman-tools-0.6.2/talisman_tools/commands/servers/arguments/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/arguments/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1612 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/arguments/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.990146 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.990146 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      673 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.990146 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2857 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/methods/convert.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.990146 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/
--rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      816 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.994146 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/methods/load.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.994146 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/
--rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1698 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.994146 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/methods/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/methods/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2571 2024-03-13 14:18:05.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/methods/process.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/methods/update.py
--rw-rw-rw-   0 root         (0) root         (0)      927 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/commands/subparsers.py
--rw-rw-rw-   0 root         (0) root         (0)      779 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/parser.py
--rw-rw-rw-   0 root         (0) root         (0)     3064 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/servers/server_helper.py
--rw-rw-rw-   0 root         (0) root         (0)      777 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/subparsers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:55.014146 talisman-tools-0.6.2/talisman_tools/commands/train/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/talisman_tools/commands/train/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/train/action.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/commands/train/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:55.014146 talisman-tools-0.6.2/talisman_tools/configure/
--rw-rw-rw-   0 root         (0) root         (0)      241 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/configure/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5626 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/configure/configure.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/configure/wrap.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:55.014146 talisman-tools-0.6.2/talisman_tools/configure/wrapper/
--rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/configure/wrapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1377 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/configure/wrapper/actions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:55.014146 talisman-tools-0.6.2/talisman_tools/helper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-20 12:52:37.000000 talisman-tools-0.6.2/talisman_tools/helper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/helper/concurrency.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-03-19 10:09:27.000000 talisman-tools-0.6.2/talisman_tools/helper/env.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-03-19 10:09:27.000000 talisman-tools-0.6.2/talisman_tools/helper/log_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      660 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/helper/multiprocessing.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/parser_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:55.014146 talisman-tools-0.6.2/talisman_tools/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     1159 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1840 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/abstract.py
--rw-rw-rw-   0 root         (0) root         (0)      995 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/domain.py
--rw-rw-rw-   0 root         (0) root         (0)      669 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)      331 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/kb.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/processor.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/reader.py
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/trainer.py
--rw-rw-rw-   0 root         (0) root         (0)      337 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/wrapper.py
--rw-rw-rw-   0 root         (0) root         (0)      942 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/plugin/wrapper_actions.py
--rw-rw-rw-   0 root         (0) root         (0)      796 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/talisman.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-03-05 14:17:49.000000 talisman-tools-0.6.2/talisman_tools/talisman_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-20 12:52:54.966147 talisman-tools-0.6.2/talisman_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)      713 2024-03-20 12:52:54.000000 talisman-tools-0.6.2/talisman_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4615 2024-03-20 12:52:54.000000 talisman-tools-0.6.2/talisman_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-20 12:52:54.000000 talisman-tools-0.6.2/talisman_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2024-03-20 12:52:54.000000 talisman-tools-0.6.2/talisman_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      312 2024-03-20 12:52:54.000000 talisman-tools-0.6.2/talisman_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-03-20 12:52:54.000000 talisman-tools-0.6.2/talisman_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.824861 talisman-tools-0.6.3/
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-03 08:39:21.824861 talisman-tools-0.6.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-04-03 08:39:08.000000 talisman-tools-0.6.3/VERSION
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:39:21.824861 talisman-tools-0.6.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-04-03 08:39:08.000000 talisman-tools-0.6.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.812861 talisman-tools-0.6.3/talisman_tools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/talisman_tools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       35 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/arguments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/talisman_tools/arguments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/arguments/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/arguments/loader.py
+-rw-rw-rw-   0 root         (0) root         (0)     1461 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/arguments/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/arguments/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      834 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/arguments/serializer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/dataset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/dataset/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/dataset/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/dataset/commands/convert/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/dataset/commands/convert/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/dataset/commands/convert/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      360 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/dataset/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      667 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/dataset/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/model/
+-rw-rw-rw-   0 root         (0) root         (0)       82 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/model/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/model/commands/check_performance/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/check_performance/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2893 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/check_performance/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/check_performance/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/model/commands/configure/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/configure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/configure/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/
+-rw-rw-rw-   0 root         (0) root         (0)       88 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3605 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     4892 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/
+-rw-rw-rw-   0 root         (0) root         (0)      708 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5244 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/disambiguation_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1821 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/nerc.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/relext.py
+-rw-rw-rw-   0 root         (0) root         (0)     5278 2024-03-28 14:30:26.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)    15234 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1322 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/model/commands/process/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/process/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      607 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/process/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/process/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      978 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/model/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/arguments/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/arguments/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/arguments/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      673 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2857 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/methods/convert.py
+-rw-rw-rw-   0 root         (0) root         (0)      587 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/
+-rw-rw-rw-   0 root         (0) root         (0)       84 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      816 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2024-04-03 08:39:08.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/methods/load.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1698 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/action.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/methods/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/methods/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2571 2024-04-03 08:39:08.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/methods/process.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/methods/update.py
+-rw-rw-rw-   0 root         (0) root         (0)      927 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/commands/subparsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      779 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     3064 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/servers/server_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)      777 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/subparsers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/commands/train/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/talisman_tools/commands/train/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/train/action.py
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/commands/train/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/configure/
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/configure/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5626 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/configure/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/configure/wrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.820861 talisman-tools-0.6.3/talisman_tools/configure/wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/configure/wrapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1377 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/configure/wrapper/actions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.824861 talisman-tools-0.6.3/talisman_tools/helper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 08:39:14.000000 talisman-tools-0.6.3/talisman_tools/helper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/helper/concurrency.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-04-03 08:39:08.000000 talisman-tools-0.6.3/talisman_tools/helper/env.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-04-03 08:39:08.000000 talisman-tools-0.6.3/talisman_tools/helper/log_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      660 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/helper/multiprocessing.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/parser_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.824861 talisman-tools-0.6.3/talisman_tools/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     1159 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1840 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/abstract.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      521 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)      669 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)      331 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/kb.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/processor.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/reader.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/trainer.py
+-rw-rw-rw-   0 root         (0) root         (0)      337 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/wrapper.py
+-rw-rw-rw-   0 root         (0) root         (0)      942 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/plugin/wrapper_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      796 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/talisman.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-03-26 14:19:14.000000 talisman-tools-0.6.3/talisman_tools/talisman_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:39:21.816861 talisman-tools-0.6.3/talisman_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      713 2024-04-03 08:39:21.000000 talisman-tools-0.6.3/talisman_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4615 2024-04-03 08:39:21.000000 talisman-tools-0.6.3/talisman_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:39:21.000000 talisman-tools-0.6.3/talisman_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2024-04-03 08:39:21.000000 talisman-tools-0.6.3/talisman_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-03 08:39:21.000000 talisman-tools-0.6.3/talisman_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-03 08:39:21.000000 talisman-tools-0.6.3/talisman_tools.egg-info/top_level.txt
```

### Comparing `talisman-tools-0.6.2/PKG-INFO` & `talisman-tools-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-tools
-Version: 0.6.2
+Version: 0.6.3
 Summary: Talisman applications
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-tools-0.6.2/setup.py` & `talisman-tools-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/arguments/domain.py` & `talisman-tools-0.6.3/talisman_tools/arguments/domain.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/arguments/loader.py` & `talisman-tools-0.6.3/talisman_tools/arguments/loader.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/arguments/processor.py` & `talisman-tools-0.6.3/talisman_tools/arguments/processor.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/arguments/reader.py` & `talisman-tools-0.6.3/talisman_tools/arguments/reader.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/arguments/serializer.py` & `talisman-tools-0.6.3/talisman_tools/arguments/serializer.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/dataset/commands/convert/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/dataset/commands/convert/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/dataset/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/dataset/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/check_performance/action.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/check_performance/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/check_performance/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/check_performance/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/configure/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/configure/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/action.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluation.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluation.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/__init__.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/disambiguation_quality.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/disambiguation_quality.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/nerc.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/nerc.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/evaluators/relext.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/evaluators/relext.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/helpers.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/helpers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/metrics.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/metrics.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/evaluate/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/evaluate/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/process/action.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/process/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/process/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/process/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/commands/subparsers.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/model/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/model/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/arguments/server.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/arguments/server.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/action.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/methods/convert.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/methods/convert.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/converter/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/converter/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/action.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/methods/load.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/methods/load.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from logging import Logger
 
 from fastapi import FastAPI, HTTPException, Request
 from tdm import TalismanDocumentModel
 
+from tp_interfaces.domain.manager import DomainManager
 from tp_interfaces.loader.interfaces import Loader
 from tp_interfaces.logging.context import update_log_extras
 
 _logger = logging.getLogger(__name__)
 
 
 def register_load_docs(
@@ -16,14 +17,16 @@
         logger: Logger = _logger
 ):
     cfg_type = loader.config_type
 
     @app.post('/', response_model=str)
     async def load_docs(request: Request, *, message: TalismanDocumentModel, config: cfg_type):
         with update_log_extras(doc_id=message.id):
+            async with DomainManager() as manager:
+                await manager.domain
             doc = message.deserialize()
             try:
                 status = await loader.load_doc_and_bind_facts(doc, config)
             except Exception as e:
                 logger.error("Non handled exception while request processing", exc_info=e)
                 raise HTTPException(status_code=500)
```

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/loader/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/loader/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/action.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/methods/process.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/methods/process.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/methods/update.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/methods/update.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/processor/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/processor/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/commands/subparsers.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/servers/server_helper.py` & `talisman-tools-0.6.3/talisman_tools/commands/servers/server_helper.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/subparsers.py` & `talisman-tools-0.6.3/talisman_tools/commands/subparsers.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/train/action.py` & `talisman-tools-0.6.3/talisman_tools/commands/train/action.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/commands/train/parser.py` & `talisman-tools-0.6.3/talisman_tools/commands/train/parser.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/configure/configure.py` & `talisman-tools-0.6.3/talisman_tools/configure/configure.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/configure/wrapper/actions.py` & `talisman-tools-0.6.3/talisman_tools/configure/wrapper/actions.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/helper/concurrency.py` & `talisman-tools-0.6.3/talisman_tools/helper/concurrency.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/helper/multiprocessing.py` & `talisman-tools-0.6.3/talisman_tools/helper/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/parser_helper.py` & `talisman-tools-0.6.3/talisman_tools/parser_helper.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/plugin/__init__.py` & `talisman-tools-0.6.3/talisman_tools/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/plugin/abstract.py` & `talisman-tools-0.6.3/talisman_tools/plugin/abstract.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/plugin/cli.py` & `talisman-tools-0.6.3/talisman_tools/plugin/cli.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/plugin/domain.py` & `talisman-tools-0.6.3/talisman_tools/plugin/domain.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/plugin/endpoint.py` & `talisman-tools-0.6.3/talisman_tools/plugin/endpoint.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/plugin/reader.py` & `talisman-tools-0.6.3/talisman_tools/plugin/reader.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/plugin/serializer.py` & `talisman-tools-0.6.3/talisman_tools/plugin/serializer.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/plugin/wrapper_actions.py` & `talisman-tools-0.6.3/talisman_tools/plugin/wrapper_actions.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/talisman.py` & `talisman-tools-0.6.3/talisman_tools/talisman.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools/talisman_logging.py` & `talisman-tools-0.6.3/talisman_tools/talisman_logging.py`

 * *Files identical despite different names*

### Comparing `talisman-tools-0.6.2/talisman_tools.egg-info/PKG-INFO` & `talisman-tools-0.6.3/talisman_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: talisman-tools
-Version: 0.6.2
+Version: 0.6.3
 Summary: Talisman applications
 Author: ISPRAS Talisman NLP team
 Author-email: modis@ispras.ru
 Maintainer: Vladimir Mayorov
 Maintainer-email: vmayorov@ispras.ru
 License: Apache Software License
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `talisman-tools-0.6.2/talisman_tools.egg-info/SOURCES.txt` & `talisman-tools-0.6.3/talisman_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

