# Comparing `tmp/linuxnet-qos-3.3.4.tar.gz` & `tmp/linuxnet-qos-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/panos/dvl/gitlab/qos/linuxnet-qos/dist/tmp_egeoisk/linuxnet-qos-3.3.4.tar", last modified: Sat Apr  8 20:38:41 2023, max compression
+gzip compressed data, was "linuxnet-qos-3.3.6.tar", last modified: Wed Apr  3 17:30:52 2024, max compression
```

## Comparing `linuxnet-qos-3.3.4.tar` & `linuxnet-qos-3.3.6.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/actions/
--rw-r--r--   0 panos     (1001) users      (100)      937 2023-04-08 20:07:35.000000 linuxnet-qos-3.3.4/docs/actions/mirred.rst
--rw-r--r--   0 panos     (1001) users      (100)      992 2023-04-08 20:07:36.000000 linuxnet-qos-3.3.4/docs/actions/police.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/extend/
--rw-r--r--   0 panos     (1001) users      (100)     2279 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.4/docs/extend/filter.rst
--rw-r--r--   0 panos     (1001) users      (100)     2653 2023-04-08 20:07:32.000000 linuxnet-qos-3.3.4/docs/extend/parsing.rst
--rw-r--r--   0 panos     (1001) users      (100)     9505 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.4/docs/extend/qdisc.rst
--rw-r--r--   0 panos     (1001) users      (100)     1070 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.4/docs/extend/util.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/filters/
--rw-r--r--   0 panos     (1001) users      (100)      923 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.4/docs/filters/fwfilter.rst
--rw-r--r--   0 panos     (1001) users      (100)     2582 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.4/docs/filters/u32filter.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/docs/qdiscs/
--rw-r--r--   0 panos     (1001) users      (100)     1133 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.4/docs/qdiscs/fifo.rst
--rw-r--r--   0 panos     (1001) users      (100)     1371 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.4/docs/qdiscs/fq_codel.rst
--rw-r--r--   0 panos     (1001) users      (100)     1279 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.4/docs/qdiscs/htb.rst
--rw-r--r--   0 panos     (1001) users      (100)     1282 2023-04-08 20:07:35.000000 linuxnet-qos-3.3.4/docs/qdiscs/ingress.rst
--rw-r--r--   0 panos     (1001) users      (100)     1343 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.4/docs/qdiscs/multiqueue.rst
--rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.4/docs/qdiscs/netem.rst
--rw-r--r--   0 panos     (1001) users      (100)     1311 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.4/docs/qdiscs/prio.rst
--rw-r--r--   0 panos     (1001) users      (100)     1351 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.4/docs/qdiscs/sfq.rst
--rw-r--r--   0 panos     (1001) users      (100)      905 2023-02-20 19:38:13.000000 linuxnet-qos-3.3.4/docs/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     2819 2023-02-20 19:39:24.000000 linuxnet-qos-3.3.4/docs/conf.py
--rw-r--r--   0 panos     (1001) users      (100)     1079 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.4/docs/config.rst
--rw-r--r--   0 panos     (1001) users      (100)     1454 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.4/docs/exceptions.rst
--rw-r--r--   0 panos     (1001) users      (100)     1223 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.4/docs/extensibility.rst
--rw-r--r--   0 panos     (1001) users      (100)     2151 2023-02-22 07:01:57.000000 linuxnet-qos-3.3.4/docs/index.rst
--rw-r--r--   0 panos     (1001) users      (100)      977 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.4/docs/qdisc.rst
--rw-r--r--   0 panos     (1001) users      (100)     1789 2023-04-08 20:07:33.000000 linuxnet-qos-3.3.4/docs/qos_api.rst
--rw-r--r--   0 panos     (1001) users      (100)     1341 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.4/docs/stats.rst
--rw-r--r--   0 panos     (1001) users      (100)     2065 2023-04-08 20:07:36.000000 linuxnet-qos-3.3.4/docs/traffic_actions.rst
--rw-r--r--   0 panos     (1001) users      (100)     1279 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.4/docs/traffic_filters.rst
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/qos/
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/
--rw-r--r--   0 panos     (1001) users      (100)      816 2023-04-08 20:07:34.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     2816 2023-04-08 20:07:34.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/action.py
--rw-r--r--   0 panos     (1001) users      (100)     5141 2023-04-08 20:07:35.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/mirred.py
--rw-r--r--   0 panos     (1001) users      (100)     5066 2023-04-08 20:07:34.000000 linuxnet-qos-3.3.4/linuxnet/qos/actions/police.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/
--rw-r--r--   0 panos     (1001) users      (100)     1160 2023-02-22 06:09:39.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     8006 2023-04-08 20:07:30.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/filter.py
--rw-r--r--   0 panos     (1001) users      (100)     5939 2023-04-08 20:07:30.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/fwfilter.py
--rw-r--r--   0 panos     (1001) users      (100)    31301 2023-04-08 20:07:30.000000 linuxnet-qos-3.3.4/linuxnet/qos/filters/u32filter.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/
--rw-r--r--   0 panos     (1001) users      (100)     1029 2023-02-22 06:09:36.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)     5501 2023-04-08 20:07:28.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/fifo.py
--rw-r--r--   0 panos     (1001) users      (100)    13821 2023-04-08 20:07:28.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/fq_codel.py
--rw-r--r--   0 panos     (1001) users      (100)    20192 2023-02-22 06:09:37.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/htb.py
--rw-r--r--   0 panos     (1001) users      (100)     2357 2023-04-08 20:07:33.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/ingress.py
--rw-r--r--   0 panos     (1001) users      (100)     3581 2023-02-22 06:09:37.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/multiqueue.py
--rw-r--r--   0 panos     (1001) users      (100)    11373 2023-04-08 20:07:29.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/netem.py
--rw-r--r--   0 panos     (1001) users      (100)     7519 2023-04-08 20:07:28.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/prio.py
--rw-r--r--   0 panos     (1001) users      (100)    25418 2023-04-08 20:07:29.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/qdisc.py
--rw-r--r--   0 panos     (1001) users      (100)     5779 2023-04-08 20:07:29.000000 linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/sfq.py
--rw-r--r--   0 panos     (1001) users      (100)     1322 2023-04-08 20:07:31.000000 linuxnet-qos-3.3.4/linuxnet/qos/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    26352 2023-04-08 20:07:31.000000 linuxnet-qos-3.3.4/linuxnet/qos/config.py
--rw-r--r--   0 panos     (1001) users      (100)      907 2023-02-22 06:09:40.000000 linuxnet-qos-3.3.4/linuxnet/qos/deps.py
--rw-r--r--   0 panos     (1001) users      (100)     4430 2023-04-08 20:07:31.000000 linuxnet-qos-3.3.4/linuxnet/qos/exceptions.py
--rw-r--r--   0 panos     (1001) users      (100)     1636 2023-02-22 06:09:40.000000 linuxnet-qos-3.3.4/linuxnet/qos/extension.py
--rw-r--r--   0 panos     (1001) users      (100)     5369 2023-02-22 06:09:34.000000 linuxnet-qos-3.3.4/linuxnet/qos/handle.py
--rw-r--r--   0 panos     (1001) users      (100)      893 2023-04-08 20:07:32.000000 linuxnet-qos-3.3.4/linuxnet/qos/metadata.py
--rw-r--r--   0 panos     (1001) users      (100)    36970 2023-04-08 20:07:30.000000 linuxnet-qos-3.3.4/linuxnet/qos/parsers.py
--rw-r--r--   0 panos     (1001) users      (100)     4148 2023-02-22 06:09:36.000000 linuxnet-qos-3.3.4/linuxnet/qos/tcunit.py
--rw-r--r--   0 panos     (1001) users      (100)     2968 2023-02-22 06:09:36.000000 linuxnet-qos-3.3.4/linuxnet/qos/util.py
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-02-20 19:27:55.000000 linuxnet-qos-3.3.4/linuxnet/__init__.py
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/
--rw-r--r--   0 panos     (1001) users      (100)     2374 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)     1632 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/SOURCES.txt
--rw-r--r--   0 panos     (1001) users      (100)        1 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/dependency_links.txt
--rw-r--r--   0 panos     (1001) users      (100)        9 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/linuxnet_qos.egg-info/top_level.txt
-drwxr-sr-x   0 panos     (1001) users      (100)        0 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/tests/
--rw-r--r--   0 panos     (1001) users      (100)        0 2023-02-22 06:58:21.000000 linuxnet-qos-3.3.4/tests/__init__.py
--rw-r--r--   0 panos     (1001) users      (100)    31223 2023-04-08 20:07:32.000000 linuxnet-qos-3.3.4/tests/qos_test.py
--rw-r--r--   0 panos     (1001) users      (100)    18811 2023-02-20 19:37:02.000000 linuxnet-qos-3.3.4/.pylintrc
--rw-r--r--   0 panos     (1001) users      (100)      244 2023-04-08 20:11:06.000000 linuxnet-qos-3.3.4/CHANGELOG.md
--rw-r--r--   0 panos     (1001) users      (100)    32387 2023-02-20 19:31:11.000000 linuxnet-qos-3.3.4/LICENSE
--rw-r--r--   0 panos     (1001) users      (100)      271 2023-02-20 19:36:39.000000 linuxnet-qos-3.3.4/MANIFEST.in
--rw-r--r--   0 panos     (1001) users      (100)     5135 2023-02-20 19:36:02.000000 linuxnet-qos-3.3.4/Makefile
--rw-r--r--   0 panos     (1001) users      (100)     1477 2023-02-22 07:01:39.000000 linuxnet-qos-3.3.4/README.md
--rw-r--r--   0 panos     (1001) users      (100)     4993 2023-02-22 06:57:50.000000 linuxnet-qos-3.3.4/setup.py
--rw-r--r--   0 panos     (1001) users      (100)     2374 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/PKG-INFO
--rw-r--r--   0 panos     (1001) users      (100)       38 2023-04-08 20:38:41.000000 linuxnet-qos-3.3.4/setup.cfg
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.329644 linuxnet-qos-3.3.6/
+-rw-r--r--   0 panos     (1001) users      (100)    18811 2023-02-20 19:37:02.000000 linuxnet-qos-3.3.6/.pylintrc
+-rw-r--r--   0 panos     (1001) users      (100)      439 2024-04-03 15:11:05.000000 linuxnet-qos-3.3.6/CHANGELOG.md
+-rw-r--r--   0 panos     (1001) users      (100)    32387 2023-02-20 19:31:11.000000 linuxnet-qos-3.3.6/LICENSE
+-rw-r--r--   0 panos     (1001) users      (100)      271 2023-02-20 19:36:39.000000 linuxnet-qos-3.3.6/MANIFEST.in
+-rw-r--r--   0 panos     (1001) users      (100)     5135 2023-02-20 19:36:02.000000 linuxnet-qos-3.3.6/Makefile
+-rw-r--r--   0 panos     (1001) users      (100)     2354 2024-04-03 17:30:52.328644 linuxnet-qos-3.3.6/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     1477 2023-02-22 07:01:39.000000 linuxnet-qos-3.3.6/README.md
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.314644 linuxnet-qos-3.3.6/docs/
+-rw-r--r--   0 panos     (1001) users      (100)      905 2023-02-20 19:38:13.000000 linuxnet-qos-3.3.6/docs/Makefile
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.314644 linuxnet-qos-3.3.6/docs/actions/
+-rw-r--r--   0 panos     (1001) users      (100)      937 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/docs/actions/mirred.rst
+-rw-r--r--   0 panos     (1001) users      (100)      992 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/docs/actions/police.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2819 2023-02-20 19:39:24.000000 linuxnet-qos-3.3.6/docs/conf.py
+-rw-r--r--   0 panos     (1001) users      (100)     1079 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.6/docs/config.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1454 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.6/docs/exceptions.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.315644 linuxnet-qos-3.3.6/docs/extend/
+-rw-r--r--   0 panos     (1001) users      (100)     2279 2023-02-22 06:09:41.000000 linuxnet-qos-3.3.6/docs/extend/filter.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2653 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/docs/extend/parsing.rst
+-rw-r--r--   0 panos     (1001) users      (100)     9505 2024-04-03 04:18:52.000000 linuxnet-qos-3.3.6/docs/extend/qdisc.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1117 2024-04-03 04:18:52.000000 linuxnet-qos-3.3.6/docs/extend/util.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1223 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.6/docs/extensibility.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.315644 linuxnet-qos-3.3.6/docs/filters/
+-rw-r--r--   0 panos     (1001) users      (100)      923 2023-02-22 06:09:42.000000 linuxnet-qos-3.3.6/docs/filters/fwfilter.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2582 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.6/docs/filters/u32filter.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2151 2023-02-22 07:01:57.000000 linuxnet-qos-3.3.6/docs/index.rst
+-rw-r--r--   0 panos     (1001) users      (100)      977 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.6/docs/qdisc.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.316644 linuxnet-qos-3.3.6/docs/qdiscs/
+-rw-r--r--   0 panos     (1001) users      (100)     1133 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.6/docs/qdiscs/fifo.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1371 2023-02-22 06:09:43.000000 linuxnet-qos-3.3.6/docs/qdiscs/fq_codel.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1279 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.6/docs/qdiscs/htb.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1282 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/docs/qdiscs/ingress.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1343 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.6/docs/qdiscs/multiqueue.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1129 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.6/docs/qdiscs/netem.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1311 2023-02-22 06:09:44.000000 linuxnet-qos-3.3.6/docs/qdiscs/prio.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1351 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.6/docs/qdiscs/sfq.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1789 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/docs/qos_api.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1341 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.6/docs/stats.rst
+-rw-r--r--   0 panos     (1001) users      (100)     2065 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/docs/traffic_actions.rst
+-rw-r--r--   0 panos     (1001) users      (100)     1279 2023-02-22 06:09:45.000000 linuxnet-qos-3.3.6/docs/traffic_filters.rst
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.317644 linuxnet-qos-3.3.6/linuxnet/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-02-20 19:27:55.000000 linuxnet-qos-3.3.6/linuxnet/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.319644 linuxnet-qos-3.3.6/linuxnet/qos/
+-rw-r--r--   0 panos     (1001) users      (100)     1322 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/__init__.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.320644 linuxnet-qos-3.3.6/linuxnet/qos/actions/
+-rw-r--r--   0 panos     (1001) users      (100)      816 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/actions/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     2816 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/actions/action.py
+-rw-r--r--   0 panos     (1001) users      (100)     5141 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/actions/mirred.py
+-rw-r--r--   0 panos     (1001) users      (100)     5066 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/actions/police.py
+-rw-r--r--   0 panos     (1001) users      (100)    26352 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/config.py
+-rw-r--r--   0 panos     (1001) users      (100)      907 2023-02-22 06:09:40.000000 linuxnet-qos-3.3.6/linuxnet/qos/deps.py
+-rw-r--r--   0 panos     (1001) users      (100)     4430 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/exceptions.py
+-rw-r--r--   0 panos     (1001) users      (100)     1665 2024-04-03 04:18:52.000000 linuxnet-qos-3.3.6/linuxnet/qos/extension.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.321644 linuxnet-qos-3.3.6/linuxnet/qos/filters/
+-rw-r--r--   0 panos     (1001) users      (100)     1160 2023-02-22 06:09:39.000000 linuxnet-qos-3.3.6/linuxnet/qos/filters/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     8006 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/filters/filter.py
+-rw-r--r--   0 panos     (1001) users      (100)     5939 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/filters/fwfilter.py
+-rw-r--r--   0 panos     (1001) users      (100)    31774 2024-04-03 04:18:52.000000 linuxnet-qos-3.3.6/linuxnet/qos/filters/u32filter.py
+-rw-r--r--   0 panos     (1001) users      (100)     5369 2023-02-22 06:09:34.000000 linuxnet-qos-3.3.6/linuxnet/qos/handle.py
+-rw-r--r--   0 panos     (1001) users      (100)      899 2024-04-03 04:18:52.000000 linuxnet-qos-3.3.6/linuxnet/qos/metadata.py
+-rw-r--r--   0 panos     (1001) users      (100)    36970 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/parsers.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.325644 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/
+-rw-r--r--   0 panos     (1001) users      (100)     1029 2023-02-22 06:09:36.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)     5501 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/fifo.py
+-rw-r--r--   0 panos     (1001) users      (100)    13821 2024-04-03 04:18:51.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/fq_codel.py
+-rw-r--r--   0 panos     (1001) users      (100)    20192 2024-04-03 04:18:51.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/htb.py
+-rw-r--r--   0 panos     (1001) users      (100)     2357 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/ingress.py
+-rw-r--r--   0 panos     (1001) users      (100)     3581 2023-02-22 06:09:37.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/multiqueue.py
+-rw-r--r--   0 panos     (1001) users      (100)    11373 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/netem.py
+-rw-r--r--   0 panos     (1001) users      (100)     7519 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/prio.py
+-rw-r--r--   0 panos     (1001) users      (100)    25418 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/qdisc.py
+-rw-r--r--   0 panos     (1001) users      (100)     5779 2024-04-03 04:18:51.000000 linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/sfq.py
+-rw-r--r--   0 panos     (1001) users      (100)     4461 2024-04-03 04:18:52.000000 linuxnet-qos-3.3.6/linuxnet/qos/tcunit.py
+-rw-r--r--   0 panos     (1001) users      (100)     2968 2023-02-22 06:09:36.000000 linuxnet-qos-3.3.6/linuxnet/qos/util.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.327644 linuxnet-qos-3.3.6/linuxnet_qos.egg-info/
+-rw-r--r--   0 panos     (1001) users      (100)     2354 2024-04-03 17:30:52.000000 linuxnet-qos-3.3.6/linuxnet_qos.egg-info/PKG-INFO
+-rw-r--r--   0 panos     (1001) users      (100)     1632 2024-04-03 17:30:52.000000 linuxnet-qos-3.3.6/linuxnet_qos.egg-info/SOURCES.txt
+-rw-r--r--   0 panos     (1001) users      (100)        1 2024-04-03 17:30:52.000000 linuxnet-qos-3.3.6/linuxnet_qos.egg-info/dependency_links.txt
+-rw-r--r--   0 panos     (1001) users      (100)        9 2024-04-03 17:30:52.000000 linuxnet-qos-3.3.6/linuxnet_qos.egg-info/top_level.txt
+-rw-r--r--   0 panos     (1001) users      (100)       38 2024-04-03 17:30:52.329644 linuxnet-qos-3.3.6/setup.cfg
+-rw-r--r--   0 panos     (1001) users      (100)     4993 2023-02-22 06:57:50.000000 linuxnet-qos-3.3.6/setup.py
+drwxr-sr-x   0 panos     (1001) users      (100)        0 2024-04-03 17:30:52.327644 linuxnet-qos-3.3.6/tests/
+-rw-r--r--   0 panos     (1001) users      (100)        0 2023-02-22 06:58:21.000000 linuxnet-qos-3.3.6/tests/__init__.py
+-rw-r--r--   0 panos     (1001) users      (100)    31223 2023-04-08 20:39:35.000000 linuxnet-qos-3.3.6/tests/qos_test.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `linuxnet-qos-3.3.4/docs/actions/mirred.rst` & `linuxnet-qos-3.3.6/docs/actions/mirred.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/actions/police.rst` & `linuxnet-qos-3.3.6/docs/actions/police.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/extend/filter.rst` & `linuxnet-qos-3.3.6/docs/extend/filter.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/extend/parsing.rst` & `linuxnet-qos-3.3.6/docs/extend/parsing.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/extend/qdisc.rst` & `linuxnet-qos-3.3.6/docs/extend/qdisc.rst`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 Supporting a new queuing discipline
 -----------------------------------
 
 The following example illustrates how to add support for the ``pfifo``
 queuing discipline::
 
-    from linuxnet.qos.extension import (QDisc, unitstr2num,
+    from linuxnet.qos.extension import (QDisc, unitstr2int,
                                         QDiscParser, QDiscOutput)
 
     class PFifoQDisc(QDisc):
         """The new Python class must be a child of QDisc
         """
         def __init__(self, handle, parent_handle, packet_limit=None):
             super().__init__(handle, parent_handle)
@@ -65,15 +65,15 @@
             """
             field_iter = qdisc_output.get_field_iter()
             packet_limit = None
             for field in field_iter:
                 if field == 'limit':
                     limitstr = next(field_iter)
                     # limit value should have 'p' suffix
-                    packet_limit = unitstr2num(limitstr, 'p')
+                    packet_limit = unitstr2int(limitstr, 'p')
             return PFifoQDisc(qdisc_output.get_handle(),
                                     qdisc_output.get_parent_handle(),
                                     packet_limit)
 
     #
     # Register the new queueing discipline with the parser.
     #
```

### Comparing `linuxnet-qos-3.3.4/docs/extend/util.rst` & `linuxnet-qos-3.3.6/docs/extend/util.rst`

 * *Files 16% similar despite different names*

```diff
@@ -28,12 +28,16 @@
 
 --------------
 
 .. autofunction:: datastr2int
 
 --------------
 
+.. autofunction:: unitstr2int
+
+--------------
+
 .. autofunction:: timestr2float
 
 --------------
 
 .. autofunction:: rate2str
```

### Comparing `linuxnet-qos-3.3.4/docs/filters/fwfilter.rst` & `linuxnet-qos-3.3.6/docs/filters/fwfilter.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/filters/u32filter.rst` & `linuxnet-qos-3.3.6/docs/filters/u32filter.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdiscs/fifo.rst` & `linuxnet-qos-3.3.6/docs/qdiscs/fifo.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdiscs/fq_codel.rst` & `linuxnet-qos-3.3.6/docs/qdiscs/fq_codel.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdiscs/htb.rst` & `linuxnet-qos-3.3.6/docs/qdiscs/htb.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdiscs/ingress.rst` & `linuxnet-qos-3.3.6/docs/qdiscs/ingress.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdiscs/multiqueue.rst` & `linuxnet-qos-3.3.6/docs/qdiscs/multiqueue.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdiscs/netem.rst` & `linuxnet-qos-3.3.6/docs/qdiscs/netem.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdiscs/prio.rst` & `linuxnet-qos-3.3.6/docs/qdiscs/prio.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdiscs/sfq.rst` & `linuxnet-qos-3.3.6/docs/qdiscs/sfq.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/Makefile` & `linuxnet-qos-3.3.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/conf.py` & `linuxnet-qos-3.3.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/config.rst` & `linuxnet-qos-3.3.6/docs/config.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/exceptions.rst` & `linuxnet-qos-3.3.6/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/extensibility.rst` & `linuxnet-qos-3.3.6/docs/extensibility.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/index.rst` & `linuxnet-qos-3.3.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qdisc.rst` & `linuxnet-qos-3.3.6/docs/qdisc.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/qos_api.rst` & `linuxnet-qos-3.3.6/docs/qos_api.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/stats.rst` & `linuxnet-qos-3.3.6/docs/stats.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/traffic_actions.rst` & `linuxnet-qos-3.3.6/docs/traffic_actions.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/docs/traffic_filters.rst` & `linuxnet-qos-3.3.6/docs/traffic_filters.rst`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/actions/__init__.py` & `linuxnet-qos-3.3.6/linuxnet/qos/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/actions/action.py` & `linuxnet-qos-3.3.6/linuxnet/qos/actions/action.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/actions/mirred.py` & `linuxnet-qos-3.3.6/linuxnet/qos/actions/mirred.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/actions/police.py` & `linuxnet-qos-3.3.6/linuxnet/qos/actions/police.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/filters/__init__.py` & `linuxnet-qos-3.3.6/linuxnet/qos/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/filters/filter.py` & `linuxnet-qos-3.3.6/linuxnet/qos/filters/filter.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/filters/fwfilter.py` & `linuxnet-qos-3.3.6/linuxnet/qos/filters/fwfilter.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/filters/u32filter.py` & `linuxnet-qos-3.3.6/linuxnet/qos/filters/u32filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2021, 2022, 2023, Panagiotis Tsirigotis
+# Copyright (c) 2021, 2022, 2023, 2024, Panagiotis Tsirigotis
 
 # This file is part of linuxnet-qos.
 #
 # linuxnet-qos is free software: you can redistribute it and/or
 # modify it under the terms of version 3 of the GNU Affero General Public
 # License as published by the Free Software Foundation.
 #
@@ -699,14 +699,22 @@
         #
         # Other forms are possible, e.g.
         #
         #   fh 801::800 order 2048 key ht 801 bkt 0 link 1:
         #
         # These will be ignored with a log warning.
         #
+        # The 'flowid' may be prefixed by '*'.
+        # The semantics of this are unclear.
+        # The tc command in the iproute-tc-6.2.0-5.el8_9.x86_64 RPM will
+        # display it; previous versions did not. This appears to be
+        # a regression that has since been fixed upstream:
+        # https://patchwork.kernel.org/project/netdevbpf/patch/20230228034955.1215122-1-liuhangbin@gmail.com/
+        # RHEL8 has not yet picked it up.
+        #
         class_handle = None
         filter_handle = None
         is_terminal = False
         for filter_line in filt_output.filter_lines_iter():
             filter_handle = None
             field_iter = iter(filter_line)
             for field in field_iter:
@@ -737,15 +745,15 @@
                         _ = int(next(field_iter), 16)
                         field = next(field_iter)
                         if field != 'bkt':
                             raise TcParsingError(
                                         f"expecting 'bkt', found '{field}'",
                                         line=str(filter_line))
                         _ = int(next(field_iter))
-                    elif field == 'flowid':
+                    elif field in ('flowid', '*flowid'):
                         if not is_terminal:
                             class_handle = Handle.create_from_string(
                                                         next(field_iter),
                                                         default_major=0)
                     elif field == 'terminal':
                         is_terminal = True
                     elif field == 'not_in_hw':
```

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/__init__.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/fifo.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/fifo.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/fq_codel.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/fq_codel.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import re
 
 from typing import List, Optional, TextIO
 
 from ..deps import get_logger
 from ..exceptions import TcParsingError
 from ..handle import Handle
-from ..tcunit import datastr2int, timestr2float, unitstr2num
+from ..tcunit import datastr2int, timestr2float, unitstr2int
 from ..parsers import QDiscParser
 
 from .qdisc import QDisc, QStats
 
 _logger = get_logger("linuxnet.qos.qdiscs.fq_codel")
 
 
@@ -345,15 +345,15 @@
         interval = None
         memory_limit = None
         ecn = None
         drop_batch = None
         try:
             for field in field_iter:
                 if field == 'limit':
-                    limit = unitstr2num(next(field_iter), 'p')
+                    limit = unitstr2int(next(field_iter), 'p')
                 elif field == 'flows':
                     flows = int(next(field_iter))
                 elif field == 'quantum':
                     quantum = int(next(field_iter))
                 elif field == 'target':
                     target = timestr2float(next(field_iter))
                 elif field == 'interval':
```

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/htb.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/htb.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 import re
 
 from typing import List, Optional, TextIO
 
 from ..deps import get_logger
 from ..exceptions import TcParsingError, TcBandwidthError
 from ..handle import Handle
-from ..tcunit import rate2str, bwstr2int, unitstr2num
+from ..tcunit import rate2str, bwstr2int, unitstr2int
 from ..parsers import QDiscParser, QClassParser
 
 from .qdisc import QDisc, QClass, QStats
 
 _logger = get_logger("linuxnet.qos.qdiscs.htb")
 
 
@@ -424,17 +424,17 @@
                 if field == 'prio':
                     prio = int(next(field_iter))
                 elif field == 'rate':
                     rate = bwstr2int(next(field_iter))
                 elif field == 'ceil':
                     ceil = bwstr2int(next(field_iter))
                 elif field == 'burst':
-                    burst = unitstr2num(next(field_iter), 'b')
+                    burst = unitstr2int(next(field_iter), 'b')
                 elif field == 'cburst':
-                    cburst = unitstr2num(next(field_iter), 'b')
+                    cburst = unitstr2int(next(field_iter), 'b')
                 else:
                     raise TcParsingError(f"unknown field '{field}'")
             htb_class = HTBQClass(qclass_output.get_handle(),
                                     qclass_output.get_parent_handle(),
                                     rate=rate,
                                     ceil=ceil, prio=prio,
                                     burst=burst, cburst=cburst)
```

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/ingress.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/ingress.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/multiqueue.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/multiqueue.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/netem.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/netem.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/prio.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/prio.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/qdisc.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/qdisc.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/qdiscs/sfq.py` & `linuxnet-qos-3.3.6/linuxnet/qos/qdiscs/sfq.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 """This module provides access to the SFQ queueing discipline
 """
 
 from typing import List, Optional, TextIO
 
 from ..exceptions import TcParsingError
 from ..handle import Handle
-from ..tcunit import unitstr2num, datastr2int
+from ..tcunit import unitstr2int, datastr2int
 from ..parsers import QDiscParser
 
 from .qdisc import QDisc, QStats
 
 
 class SFQQDiscStats(QStats):
     """SFQDisc stats
@@ -151,15 +151,15 @@
         for field in field_iter:
             if field == 'limit':
                 #
                 # 'limit' is not documented in tc-sfq(8), so we ignore it.
                 #
                 _ = next(field_iter)
             elif field == 'perturb':
-                perturb = unitstr2num(next(field_iter), 'sec')
+                perturb = unitstr2int(next(field_iter), 'sec')
             elif field == 'quantum':
                 quantum = datastr2int(next(field_iter))
             elif field == 'depth':
                 _ = next(field_iter)
             elif field == 'divisor':
                 _ = next(field_iter)
             else:
```

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/__init__.py` & `linuxnet-qos-3.3.6/linuxnet/qos/__init__.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/config.py` & `linuxnet-qos-3.3.6/linuxnet/qos/config.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/deps.py` & `linuxnet-qos-3.3.6/linuxnet/qos/deps.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/exceptions.py` & `linuxnet-qos-3.3.6/linuxnet/qos/exceptions.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/extension.py` & `linuxnet-qos-3.3.6/linuxnet/qos/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,10 +44,11 @@
                 FilterOutputLine,
                 LineGroupIterator,
                 )
 
 from .tcunit import (
                 bwstr2int,
                 datastr2int,
+                unitstr2int,
                 timestr2float,
                 rate2str,
                 )
```

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/handle.py` & `linuxnet-qos-3.3.6/linuxnet/qos/handle.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/metadata.py` & `linuxnet-qos-3.3.6/linuxnet/qos/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, 2023, Panagiotis Tsirigotis
+# Copyright (c) 2022, 2023, 2024, Panagiotis Tsirigotis
 
 # This file is part of linuxnet-qos.
 #
 # linuxnet-qos is free software: you can redistribute it and/or
 # modify it under the terms of version 3 of the GNU Affero General Public
 # License as published by the Free Software Foundation.
 #
@@ -18,10 +18,10 @@
 """
 Metadata information intended to be used by setup.py and the
 Sphinx conf.py
 """
 
 # pylint: disable=invalid-name
 
-_version_ = "3.3.4"
+_version_ = "3.3.6"
 _author_ = "Panagiotis (Panos) Tsirigotis"
 _package_ = "linuxnet.qos"
```

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/parsers.py` & `linuxnet-qos-3.3.6/linuxnet/qos/parsers.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/tcunit.py` & `linuxnet-qos-3.3.6/linuxnet/qos/tcunit.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def bwstr2int(bwstr: str) -> int:
     """Convert a string of the form
 
         * 500000bit
         * 500000Kbit
         * 500000Mbit
 
-    to the corresponding number.
+    to the corresponding number. The unit of the return value is bits/sec.
     """
     match = _int_unit_expr.match(bwstr)
     if match is None:
         raise TcParsingError(f'not a valid bandwidth string: {bwstr}')
     numstr = match.group(1)
     unit = match.group(2)
     if unit == 'bit':
@@ -55,14 +55,15 @@
     """Convert a string of the form
 
         * 500000b
         * 500000Kb
         * 500000Mb
 
     to the corresponding number.  'b' stands for 'byte'.
+    The unit of the return value is bytes.
     """
     match = _int_unit_expr.match(datastr)
     if match is None:
         raise TcParsingError(f'not a valid data string: {datastr}')
     numstr = match.group(1)
     unit = match.group(2)
     if unit == 'b':
@@ -98,20 +99,27 @@
     elif unit == 'us':
         multiplier = 0.001
     else:
         raise TcParsingError(f'unknown time unit: {unit}')
     return float(numstr) * multiplier
 
 
-def unitstr2num(bytestr: str, suffix: str) -> int:
-    """Convert a string of the form '1600b' to the corresponding number
+def unitstr2int(unitstr: str, suffix: str) -> int:
+    """Convert a string with an expected suffix to a number,
+    e.g. ``unitstr2int("20sec", "sec")`` returns ``20``.
+
+    :param unitstr: a string of the form ``<num><suffix>``
+    :param suffix: expected suffix
+
+    A :exc:`ValueError` will be raised if ``unitstr`` does not end
+    in ``suffix``.
     """
-    if not bytestr.endswith(suffix):
-        raise ValueError(f"missing suffix '{suffix}': " + bytestr)
-    return int(bytestr[:-len(suffix)])
+    if not unitstr.endswith(suffix):
+        raise ValueError(f"missing suffix '{suffix}': " + unitstr)
+    return int(unitstr[:-len(suffix)])
 
 
 class _TcBandwidthUnit(enum.IntEnum):
     """This class uses units as reported by the tc(8) command.
         kbit means kilobit per second
         mbit means megabit per second
         bps means bytes per second
```

### Comparing `linuxnet-qos-3.3.4/linuxnet/qos/util.py` & `linuxnet-qos-3.3.6/linuxnet/qos/util.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/linuxnet_qos.egg-info/PKG-INFO` & `linuxnet-qos-3.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: linuxnet-qos
-Version: 3.3.4
+Version: 3.3.6
 Summary: programmatic access to the Linux queuing disciplines
 Home-page: https://gitlab.com/panos-tools/linuxnet-qos
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-qos
 Project-URL: Documentation, https://linuxnet-qos.readthedocs.io/en/latest/index.html
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Networking
@@ -73,9 +72,7 @@
 
 Available `Makefile` targets can be listed by invoking `make` with no arguments.
 
 `make install` will install the package.
 
 `make test` runs the unit tests.
 
-
-
```

### Comparing `linuxnet-qos-3.3.4/linuxnet_qos.egg-info/SOURCES.txt` & `linuxnet-qos-3.3.6/linuxnet_qos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/tests/qos_test.py` & `linuxnet-qos-3.3.6/tests/qos_test.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/.pylintrc` & `linuxnet-qos-3.3.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/LICENSE` & `linuxnet-qos-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/Makefile` & `linuxnet-qos-3.3.6/Makefile`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/README.md` & `linuxnet-qos-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/setup.py` & `linuxnet-qos-3.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `linuxnet-qos-3.3.4/PKG-INFO` & `linuxnet-qos-3.3.6/linuxnet_qos.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: linuxnet-qos
-Version: 3.3.4
+Version: 3.3.6
 Summary: programmatic access to the Linux queuing disciplines
 Home-page: https://gitlab.com/panos-tools/linuxnet-qos
 Author: Panagiotis (Panos) Tsirigotis
 Author-email: ptsirigotis01@gmail.com
 License: AGPLv3
 Project-URL: Source, https://gitlab.com/panos-tools/linuxnet-qos
 Project-URL: Documentation, https://linuxnet-qos.readthedocs.io/en/latest/index.html
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Networking
@@ -73,9 +72,7 @@
 
 Available `Makefile` targets can be listed by invoking `make` with no arguments.
 
 `make install` will install the package.
 
 `make test` runs the unit tests.
 
-
-
```

