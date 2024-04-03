# Comparing `tmp/pulumiverse_buildkite-3.1.5.tar.gz` & `tmp/pulumiverse_buildkite-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumiverse_buildkite-3.1.5.tar", last modified: Wed Mar 27 00:37:40 2024, max compression
+gzip compressed data, was "pulumiverse_buildkite-3.1.6.tar", last modified: Wed Apr  3 00:26:05 2024, max compression
```

## Comparing `pulumiverse_buildkite-3.1.5.tar` & `pulumiverse_buildkite-3.1.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.148776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.148776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/agent/
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/agent/agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/cluster_agent_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/cluster_default_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/cluster_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/get_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/get_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/organization/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/organization/banner.py
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/organization/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/organization/organization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19294 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/get_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/get_signed_steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/get_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    17437 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    54496 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/team/
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/team/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/team/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/team/member.py
--rw-r--r--   0 runner    (1001) docker     (127)    20844 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/team/team.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/testsuite/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/testsuite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/testsuite/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/testsuite/test_suite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 00:37:40.148776 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-03-27 00:37:40.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-03-27 00:37:40.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 00:37:40.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 00:37:40.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-27 00:37:40.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-27 00:37:40.000000 pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 00:37:40.152776 pulumiverse_buildkite-3.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-27 00:37:39.000000 pulumiverse_buildkite-3.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.676772 pulumiverse_buildkite-3.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-03 00:26:05.676772 pulumiverse_buildkite-3.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5889 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.672772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.672772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8792 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/agent/agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.672772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16838 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17101 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/cluster_agent_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12130 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/cluster_default_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14551 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/cluster_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/get_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.672772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/get_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.676772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8857 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/organization/banner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/organization/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11872 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/organization/organization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.676772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19294 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/get_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8581 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/get_signed_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17437 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54496 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23969 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13308 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15694 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13438 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.676772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/team/
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/team/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/team/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12954 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/team/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20844 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/team/team.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.676772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/testsuite/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/testsuite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14400 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/testsuite/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14044 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/testsuite/test_suite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:26:05.672772 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:26:05.676772 pulumiverse_buildkite-3.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-03 00:26:05.000000 pulumiverse_buildkite-3.1.6/setup.py
```

### Comparing `pulumiverse_buildkite-3.1.5/PKG-INFO` & `pulumiverse_buildkite-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse_buildkite
-Version: 3.1.5
+Version: 3.1.6
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/pulumiverse/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_buildkite-3.1.5/README.md` & `pulumiverse_buildkite-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/__init__.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/_inputs.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/_utilities.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/agent/agent_token.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/agent/agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/cluster.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/cluster_agent_token.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/cluster_agent_token.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/cluster_default_queue.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/cluster_default_queue.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/cluster_queue.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/cluster_queue.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/cluster/get_cluster.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/cluster/get_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/config/outputs.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/config/vars.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/get_meta.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/get_meta.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/organization/banner.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/organization/banner.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/organization/get_organization.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/organization/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/organization/organization.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/organization/organization.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/_inputs.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/get_pipeline.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/get_pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/get_signed_steps.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/get_signed_steps.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/get_template.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/get_template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/outputs.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/pipeline.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/schedule.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/team.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/pipeline/template.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/pipeline/template.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/provider.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/provider.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/team/get_team.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/team/get_team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/team/member.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/team/member.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/team/team.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/team/team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/testsuite/team.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/testsuite/team.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite/testsuite/test_suite.py` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite/testsuite/test_suite.py`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/PKG-INFO` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumiverse-buildkite
-Version: 3.1.5
+Version: 3.1.6
 Summary: A Pulumi package for creating and managing Buildkite resources.
 Home-page: https://github.com/pulumiverse/pulumi-buildkite
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumiverse/pulumi-buildkite
 Keywords: pulumi buildkite
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumiverse_buildkite-3.1.5/pulumiverse_buildkite.egg-info/SOURCES.txt` & `pulumiverse_buildkite-3.1.6/pulumiverse_buildkite.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumiverse_buildkite-3.1.5/setup.py` & `pulumiverse_buildkite-3.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # coding=utf-8
 # *** WARNING: this file was generated by the Pulumi Terraform Bridge (tfgen) Tool. ***
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 import errno
-import os
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.1.5"
+VERSION = "3.1.6"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "buildkite Pulumi Package - Development Version"
```

