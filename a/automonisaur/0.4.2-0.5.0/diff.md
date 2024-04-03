# Comparing `tmp/automonisaur-0.4.2.tar.gz` & `tmp/automonisaur-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automonisaur-0.4.2.tar", last modified: Tue Feb  6 22:13:37 2024, max compression
+gzip compressed data, was "automonisaur-0.5.0.tar", last modified: Wed Apr  3 01:55:20 2024, max compression
```

## Comparing `automonisaur-0.4.2.tar` & `automonisaur-0.5.0.tar`

### file list

```diff
@@ -1,367 +1,411 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.082552 automonisaur-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-06 22:13:34.000000 automonisaur-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-02-06 22:13:37.082552 automonisaur-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4168 2024-02-06 22:13:34.000000 automonisaur-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.042552 automonisaur-0.4.2/automon/
--rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/healthcheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/
--rwxr-xr-x   0 runner    (1001) docker     (127)      155 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/assertions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/asyncioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/asyncioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/asyncioWrapper/loop.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/cryptography/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/cryptography/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/cryptography/hashing.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/cryptography/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/dates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/grok/
--rw-r--r--   0 runner    (1001) docker     (127)    11169 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/grok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/httpWrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/mathWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/mathWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/mathWrapper/file_size.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/nest_asyncioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/nest_asyncioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/nest_asyncioWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/osWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/osWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/osWrapper/environ.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1796 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/regex.py
--rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/sanitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/sleeper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/subprocessWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/subprocessWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/subprocessWrapper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/subprocessWrapper/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.046552 automonisaur-0.4.2/automon/helpers/subprocessWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/subprocessWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/subprocessWrapper/tests/test_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/subprocessWrapper/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/subprocessWrapper/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/subprocessWrapper/tests/test_sanitize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_sanitation.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_sleeper.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/tests/test_sleeper_async.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/helpers/threadingWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/threadingWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/threadingWrapper/initialize_threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/helpers/threadingWrapper/worker_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/integrations/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/integrations/beautifulsoupWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/beautifulsoupWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/beautifulsoupWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/integrations/cryptocurrency/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/cryptocurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/cryptocurrency/accounting.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/cryptocurrency/coinbase.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/cryptocurrency/other.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/cryptocurrency/robinhood.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/integrations/cryptocurrency/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/cryptocurrency/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/cryptocurrency/tests/test_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/integrations/datascience/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/datascience/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/integrations/datascience/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/datascience/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/datascience/pandas/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/datascience/pandas/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/datascience/pandas/series.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.050552 automonisaur-0.4.2/automon/integrations/datascience/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/datascience/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/datascience/tests/test_datascience.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/jvm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/snapshots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/elasticsearch/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/tests/test_elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/facebook/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/facebook/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/facebook/groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/flaskWrapper/
--rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/flaskWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/flaskWrapper/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/flaskWrapper/auth_creds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/flaskWrapper/boilerplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/flaskWrapper/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/flaskWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/flaskWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/flaskWrapper/tests/test_flask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/geoip/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/geoip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/geoip/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/geoip/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/geoip/tests/test_geoip.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/google/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/auth/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/auth/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/google/auth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/auth/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/auth/tests/test_config_Credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/auth/tests/test_google_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.054552 automonisaur-0.4.2/automon/integrations/google/gmail/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/gmail/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.058552 automonisaur-0.4.2/automon/integrations/google/gmail/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/gmail/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/gmail/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/gmail/v1/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.058552 automonisaur-0.4.2/automon/integrations/google/people/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.058552 automonisaur-0.4.2/automon/integrations/google/people/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/tests/test_google_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/tests/test_google_contacts_neo4j.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/people/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.058552 automonisaur-0.4.2/automon/integrations/google/sheets/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/sheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/sheets/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/sheets/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.058552 automonisaur-0.4.2/automon/integrations/google/sheets/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/sheets/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/sheets/tests/test_google_sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/sheets/tests/test_google_sheets_clear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.058552 automonisaur-0.4.2/automon/integrations/google/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/tests/test_google_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/google/tests/test_google_contacts_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.058552 automonisaur-0.4.2/automon/integrations/instagram/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/client_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/stories.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/instagram/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/tests/test_instagram.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/tests/test_instagram_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/tests/test_instagram_browser_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/tests/test_instagram_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/instagram/xpaths.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/ldap/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/ldap/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/ldap/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/mac/
--rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/mac/airport/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/airport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/airport/airport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/airport/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/airport/ssid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/mac/airport/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/airport/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/airport/tests/test_airport.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/airport/tests/test_airport_neo4j.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/mac/macchanger/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/macchanger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/macchanger/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/mac/macchanger/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/macchanger/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/macchanger/tests/test_macchanger.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/mac/macchanger/tests/test_set_mac_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/minioWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/assertions.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/object.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.062552 automonisaur-0.4.2/automon/integrations/minioWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/tests/test_minio_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/tests/test_minio_client_public.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/minioWrapper/tests/test_minio_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.066552 automonisaur-0.4.2/automon/integrations/neo4jWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/cypher.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.066552 automonisaur-0.4.2/automon/integrations/neo4jWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.066552 automonisaur-0.4.2/automon/integrations/nmap/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/nmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/nmap/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/nmap/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/nmap/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.066552 automonisaur-0.4.2/automon/integrations/nmap/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/nmap/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/nmap/tests/test_nmap_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/nmap/tests/test_nmap_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.066552 automonisaur-0.4.2/automon/integrations/openvpn/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/openvpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/openvpn/openvpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.066552 automonisaur-0.4.2/automon/integrations/requestsWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/requestsWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/requestsWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/requestsWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/requestsWrapper/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.066552 automonisaur-0.4.2/automon/integrations/requestsWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/requestsWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/requestsWrapper/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/requestsWrapper/tests/test_rest.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.066552 automonisaur-0.4.2/automon/integrations/scrapyWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/scrapyWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/scrapyWrapper/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.070552 automonisaur-0.4.2/automon/integrations/seleniumWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/actions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/browser_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/browser_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/config_window_size.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.070552 automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_new_browser.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_user_agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/user_agents.py
--rw-r--r--   0 runner    (1001) docker     (127)    12505 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/seleniumWrapper/webdriver_chrome.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.070552 automonisaur-0.4.2/automon/integrations/sentryio/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/sentryio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/sentryio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/sentryio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.070552 automonisaur-0.4.2/automon/integrations/sentryio/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/sentryio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/sentryio/tests/test_sentryio.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/sentryio/tests/test_sentryio_callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.070552 automonisaur-0.4.2/automon/integrations/shodan/
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/shodan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.070552 automonisaur-0.4.2/automon/integrations/shodan/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/shodan/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/shodan/tests/test_shodan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.074552 automonisaur-0.4.2/automon/integrations/slackWrapper/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/bots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/clientAsync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/slack_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    11075 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/slack_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.074552 automonisaur-0.4.2/automon/integrations/slackWrapper/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/slackWrapper/tests/test_slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.074552 automonisaur-0.4.2/automon/integrations/snmp/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/snmp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/snmp/generate_maps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.074552 automonisaur-0.4.2/automon/integrations/splunk/
--rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.074552 automonisaur-0.4.2/automon/integrations/splunk/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk/tests/test_splunk_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk/tests/test_splunk_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.074552 automonisaur-0.4.2/automon/integrations/splunk_soar/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/action_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    25552 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/container.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.074552 automonisaur-0.4.2/automon/integrations/splunk_soar/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.078552 automonisaur-0.4.2/automon/integrations/splunk_soar/integration/servicenow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/integration/servicenow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/integration/servicenow/ticket.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/phantom_unittest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.078552 automonisaur-0.4.2/automon/integrations/splunk_soar/rest/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/rest/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.078552 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   899665 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/dino.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_uat.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      590 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/splunk_soar/vault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.082552 automonisaur-0.4.2/automon/integrations/swift/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/swift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/swift/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/swift/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/swift/error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/swift/iterables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.082552 automonisaur-0.4.2/automon/integrations/swift/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/swift/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/swift/tests/test_swift.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.082552 automonisaur-0.4.2/automon/integrations/vds/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/vds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/vds/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/vds/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.082552 automonisaur-0.4.2/automon/integrations/vds/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/vds/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/integrations/vds/tests/test_vds.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/liveliness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.082552 automonisaur-0.4.2/automon/log/
--rwxr-xr-x   0 runner    (1001) docker     (127)      317 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/log/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.082552 automonisaur-0.4.2/automon/log/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/log/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-02-06 22:13:34.000000 automonisaur-0.4.2/automon/log/tests/test_logger_builtin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 22:13:37.082552 automonisaur-0.4.2/automonisaur.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-02-06 22:13:37.000000 automonisaur-0.4.2/automonisaur.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13726 2024-02-06 22:13:37.000000 automonisaur-0.4.2/automonisaur.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 22:13:37.000000 automonisaur-0.4.2/automonisaur.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-06 22:13:37.000000 automonisaur-0.4.2/automonisaur.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 22:13:37.082552 automonisaur-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-06 22:13:34.000000 automonisaur-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.327974 automonisaur-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 01:55:17.000000 automonisaur-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-03 01:55:20.327974 automonisaur-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4332 2024-04-03 01:55:17.000000 automonisaur-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.283974 automonisaur-0.5.0/automon/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       48 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/healthcheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.283974 automonisaur-0.5.0/automon/helpers/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      190 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1257 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/assertions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.283974 automonisaur-0.5.0/automon/helpers/asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/asyncioWrapper/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/helpers/cryptography/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/cryptography/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/cryptography/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/cryptography/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/httpWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/helpers/mathWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/mathWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/mathWrapper/file_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/helpers/osWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/osWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/osWrapper/environ.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      338 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4412 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4396 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/sleeper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/helpers/subprocessWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/subprocessWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/subprocessWrapper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6055 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/subprocessWrapper/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/helpers/subprocessWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/subprocessWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/subprocessWrapper/tests/test_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/subprocessWrapper/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/subprocessWrapper/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/subprocessWrapper/tests/test_sanitize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/test_assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/test_healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/test_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/test_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/test_sanitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/test_sleeper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/tests/test_sleeper_async.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/helpers/threadingWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/threadingWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/threadingWrapper/initialize_threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/helpers/threadingWrapper/worker_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/integrations/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.287974 automonisaur-0.5.0/automon/integrations/beautifulsoupWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/beautifulsoupWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/beautifulsoupWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/cryptocurrency/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/cryptocurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1764 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/cryptocurrency/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/cryptocurrency/coinbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/cryptocurrency/other.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/cryptocurrency/robinhood.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/cryptocurrency/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/cryptocurrency/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/cryptocurrency/tests/test_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/datadogWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/datadogWrapper/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/api/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/api/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/datadogWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datadogWrapper/tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/datascience/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datascience/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/datascience/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datascience/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datascience/pandas/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datascience/pandas/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datascience/pandas/series.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/datascience/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datascience/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/datascience/tests/test_datascience.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.291974 automonisaur-0.5.0/automon/integrations/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2948 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/jvm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5915 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/snapshots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/elasticsearch/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/tests/test_elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/tests/test_elasticsearch_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/tests/test_elasticsearch_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/facebook/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/facebook/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22290 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/facebook/groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/flaskWrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       42 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/flaskWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4360 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/flaskWrapper/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/flaskWrapper/auth_creds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/flaskWrapper/boilerplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/flaskWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/flaskWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/flaskWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/flaskWrapper/tests/test_flask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/geoip/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/geoip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/geoip/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/geoip/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/geoip/tests/test_geoip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/google/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/auth/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/auth/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/google/auth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/auth/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/auth/tests/test_config_Credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/auth/tests/test_google_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.295974 automonisaur-0.5.0/automon/integrations/google/gmail/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/gmail/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.299974 automonisaur-0.5.0/automon/integrations/google/gmail/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/gmail/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/gmail/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/gmail/v1/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.299974 automonisaur-0.5.0/automon/integrations/google/people/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7329 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10867 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.299974 automonisaur-0.5.0/automon/integrations/google/people/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/tests/test_google_contacts_neo4j.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/people/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.299974 automonisaur-0.5.0/automon/integrations/google/sheets/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/sheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/sheets/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/sheets/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.299974 automonisaur-0.5.0/automon/integrations/google/sheets/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/sheets/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11260 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/sheets/tests/test_google_sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/sheets/tests/test_google_sheets_clear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.299974 automonisaur-0.5.0/automon/integrations/google/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/tests/test_google_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/google/tests/test_google_contacts_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.299974 automonisaur-0.5.0/automon/integrations/grok/
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/grok/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.299974 automonisaur-0.5.0/automon/integrations/grok/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/grok/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/grok/tests/test_grok.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/instagram/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/client_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7666 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/stories.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/instagram/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/tests/test_instagram.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/tests/test_instagram_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/tests/test_instagram_browser_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/tests/test_instagram_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/instagram/xpaths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/ldap/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/ldap/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3523 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/ldap/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/mac/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       64 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/mac/airport/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/airport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/airport/airport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/airport/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/airport/ssid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/mac/airport/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/airport/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/airport/tests/test_airport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/airport/tests/test_airport_neo4j.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/mac/macchanger/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/macchanger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/macchanger/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/mac/macchanger/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/macchanger/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/macchanger/tests/test_macchanger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/mac/macchanger/tests/test_set_mac_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.303974 automonisaur-0.5.0/automon/integrations/minioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/minioWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/tests/test_minio_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/tests/test_minio_client_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/minioWrapper/tests/test_minio_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/neo4jWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11026 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/cypher.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/neo4jWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/nest_asyncioWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nest_asyncioWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nest_asyncioWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/nmap/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nmap/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nmap/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4631 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nmap/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/nmap/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nmap/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nmap/tests/test_nmap_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/nmap/tests/test_nmap_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/test/test_client_ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/test/test_memory_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.307974 automonisaur-0.5.0/automon/integrations/openvpn/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openvpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/openvpn/openvpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.311974 automonisaur-0.5.0/automon/integrations/psutilWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/psutilWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/psutilWrapper/cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.311974 automonisaur-0.5.0/automon/integrations/requestsWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/requestsWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6549 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/requestsWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/requestsWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/requestsWrapper/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.311974 automonisaur-0.5.0/automon/integrations/requestsWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/requestsWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/requestsWrapper/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/requestsWrapper/tests/test_rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/requestsWrapper/tests/test_rest_inherit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.311974 automonisaur-0.5.0/automon/integrations/scrapyWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/scrapyWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/scrapyWrapper/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.311974 automonisaur-0.5.0/automon/integrations/seleniumWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17113 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/browser_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/browser_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/config_window_size.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.311974 automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_browser_headless.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_new_browser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/user_agents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12519 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/seleniumWrapper/webdriver_chrome.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/sentryio/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/sentryio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/sentryio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/sentryio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/sentryio/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/sentryio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/sentryio/tests/test_sentryio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/sentryio/tests/test_sentryio_callback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/shodan/
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/shodan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/shodan/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/shodan/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/shodan/tests/test_shodan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/slackWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/bots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/clientAsync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/slack_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11080 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/slack_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/slackWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/slackWrapper/tests/test_slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/snmp/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/snmp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16073 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/snmp/generate_maps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/splunk/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       66 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.315974 automonisaur-0.5.0/automon/integrations/splunk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk/tests/test_splunk_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk/tests/test_splunk_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.319974 automonisaur-0.5.0/automon/integrations/splunk_soar/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/action_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25563 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.319974 automonisaur-0.5.0/automon/integrations/splunk_soar/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.319974 automonisaur-0.5.0/automon/integrations/splunk_soar/integration/servicenow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/integration/servicenow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/integration/servicenow/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/integration/servicenow/ticket.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1731 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/phantom_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.319974 automonisaur-0.5.0/automon/integrations/splunk_soar/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/rest/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.323974 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   899665 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/dino.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_filter_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_get_action_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_by_playbook_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_list_app_run_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_list_vault.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_uat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      590 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/splunk_soar/vault.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.323974 automonisaur-0.5.0/automon/integrations/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17203 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swift/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swift/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swift/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swift/iterables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.323974 automonisaur-0.5.0/automon/integrations/swift/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swift/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swift/tests/test_swift.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.323974 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.323974 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/api/v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7694 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.323974 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_library_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/swimlaneWrapper/tests/test_rest_workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.327974 automonisaur-0.5.0/automon/integrations/vds/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/vds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/vds/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/vds/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.327974 automonisaur-0.5.0/automon/integrations/vds/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/vds/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/integrations/vds/tests/test_vds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/liveliness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.327974 automonisaur-0.5.0/automon/log/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      317 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/log/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.327974 automonisaur-0.5.0/automon/log/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/log/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 01:55:17.000000 automonisaur-0.5.0/automon/log/tests/test_logger_builtin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 01:55:20.327974 automonisaur-0.5.0/automonisaur.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-03 01:55:20.000000 automonisaur-0.5.0/automonisaur.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-04-03 01:55:20.000000 automonisaur-0.5.0/automonisaur.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 01:55:20.000000 automonisaur-0.5.0/automonisaur.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 01:55:20.000000 automonisaur-0.5.0/automonisaur.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 01:55:20.327974 automonisaur-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-03 01:55:17.000000 automonisaur-0.5.0/setup.py
```

### Comparing `automonisaur-0.4.2/LICENSE` & `automonisaur-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/PKG-INFO` & `automonisaur-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.4.2
+Version: 0.5.0
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -57,17 +57,19 @@
 | API             | flask                                                       |
 | Chat            | slack                                                       |
 | Data Scraping   | beautifulsoup<br/>facebook groups<br/>instagram<br/>scrapy  |
 | Databases       | elasticsearch<br/>neo4j<br/>splunk                          |
 | Data Store      | minio<br/>swift                                             |
 | Devices         | snmp                                                        |
 | Google Cloud    | google auth api<br/>google people api<br/>google sheets api |
+| Helpers         | os<br/>subprocess<br/>threading<br/>socket<br/>datetime     |
 | Logging         | sentryio                                                    |
-| macOS           | airport<br/>macchanger                                      |
+| MacOS           | airport<br/>macchanger                                      |
 | Python          | logging<br/>requests                                        |
+| SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
 
 - python >= 3.8
```

### Comparing `automonisaur-0.4.2/README.md` & `automonisaur-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,19 @@
 | API             | flask                                                       |
 | Chat            | slack                                                       |
 | Data Scraping   | beautifulsoup<br/>facebook groups<br/>instagram<br/>scrapy  |
 | Databases       | elasticsearch<br/>neo4j<br/>splunk                          |
 | Data Store      | minio<br/>swift                                             |
 | Devices         | snmp                                                        |
 | Google Cloud    | google auth api<br/>google people api<br/>google sheets api |
+| Helpers         | os<br/>subprocess<br/>threading<br/>socket<br/>datetime     |
 | Logging         | sentryio                                                    |
-| macOS           | airport<br/>macchanger                                      |
+| MacOS           | airport<br/>macchanger                                      |
 | Python          | logging<br/>requests                                        |
+| SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
 
 - python >= 3.8
```

### Comparing `automonisaur-0.4.2/automon/helpers/assertions.py` & `automonisaur-0.5.0/automon/helpers/assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/markdown.py` & `automonisaur-0.5.0/automon/helpers/markdown.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/nest_asyncioWrapper/client.py` & `automonisaur-0.5.0/automon/integrations/nest_asyncioWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/networking.py` & `automonisaur-0.5.0/automon/helpers/networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/osWrapper/environ.py` & `automonisaur-0.5.0/automon/helpers/osWrapper/environ.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/sanitation.py` & `automonisaur-0.5.0/automon/helpers/sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/sleeper.py` & `automonisaur-0.5.0/automon/helpers/sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/subprocessWrapper/run.py` & `automonisaur-0.5.0/automon/helpers/subprocessWrapper/run.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/subprocessWrapper/tests/test_runner.py` & `automonisaur-0.5.0/automon/helpers/subprocessWrapper/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/tests/test_assertions.py` & `automonisaur-0.5.0/automon/helpers/tests/test_assertions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/tests/test_networking.py` & `automonisaur-0.5.0/automon/helpers/tests/test_networking.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/tests/test_sanitation.py` & `automonisaur-0.5.0/automon/helpers/tests/test_sanitation.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/tests/test_sleeper.py` & `automonisaur-0.5.0/automon/helpers/tests/test_sleeper.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/threadingWrapper/initialize_threading.py` & `automonisaur-0.5.0/automon/helpers/threadingWrapper/initialize_threading.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/helpers/threadingWrapper/worker_thread.py` & `automonisaur-0.5.0/automon/helpers/threadingWrapper/worker_thread.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/beautifulsoupWrapper/client.py` & `automonisaur-0.5.0/automon/integrations/beautifulsoupWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/cryptocurrency/accounting.py` & `automonisaur-0.5.0/automon/integrations/cryptocurrency/accounting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/cryptocurrency/coinbase.py` & `automonisaur-0.5.0/automon/integrations/cryptocurrency/coinbase.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/cryptocurrency/other.py` & `automonisaur-0.5.0/automon/integrations/cryptocurrency/other.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/cryptocurrency/tests/test_crypto.py` & `automonisaur-0.5.0/automon/integrations/cryptocurrency/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/datascience/pandas/pandas.py` & `automonisaur-0.5.0/automon/integrations/datascience/pandas/pandas.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/datascience/tests/test_datascience.py` & `automonisaur-0.5.0/automon/integrations/datascience/tests/test_datascience.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/cleanup.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/cleanup.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/client.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/config.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/jvm.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/jvm.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/metrics.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/metrics.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/snapshots.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/snapshots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/tests/test_elasticsearch.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/tests/test_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/tests/test_elasticsearch_JvmMonitor.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py` & `automonisaur-0.5.0/automon/integrations/elasticsearch/tests/test_elasticsearch_snapshot.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/facebook/groups.py` & `automonisaur-0.5.0/automon/integrations/facebook/groups.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/flaskWrapper/auth.py` & `automonisaur-0.5.0/automon/integrations/flaskWrapper/auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/flaskWrapper/boilerplate.py` & `automonisaur-0.5.0/automon/integrations/flaskWrapper/boilerplate.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/flaskWrapper/config.py` & `automonisaur-0.5.0/automon/integrations/flaskWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/flaskWrapper/tests/test_flask.py` & `automonisaur-0.5.0/automon/integrations/flaskWrapper/tests/test_flask.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/auth/client.py` & `automonisaur-0.5.0/automon/integrations/google/auth/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/auth/config.py` & `automonisaur-0.5.0/automon/integrations/google/auth/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/gmail/v1/client.py` & `automonisaur-0.5.0/automon/integrations/google/gmail/v1/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/gmail/v1/config.py` & `automonisaur-0.5.0/automon/integrations/google/gmail/v1/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/people/client.py` & `automonisaur-0.5.0/automon/integrations/google/people/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/people/config.py` & `automonisaur-0.5.0/automon/integrations/google/people/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/people/person.py` & `automonisaur-0.5.0/automon/integrations/google/people/person.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/people/results.py` & `automonisaur-0.5.0/automon/integrations/google/people/results.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/people/urls.py` & `automonisaur-0.5.0/automon/integrations/google/people/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/sheets/client.py` & `automonisaur-0.5.0/automon/integrations/google/sheets/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/sheets/config.py` & `automonisaur-0.5.0/automon/integrations/google/sheets/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/sheets/tests/test_google_sheets.py` & `automonisaur-0.5.0/automon/integrations/google/sheets/tests/test_google_sheets.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py` & `automonisaur-0.5.0/automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/google/sheets/tests/test_google_sheets_clear.py` & `automonisaur-0.5.0/automon/integrations/google/sheets/tests/test_google_sheets_clear.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/instagram/client.py` & `automonisaur-0.5.0/automon/integrations/instagram/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/instagram/client_browser.py` & `automonisaur-0.5.0/automon/integrations/instagram/client_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/instagram/config.py` & `automonisaur-0.5.0/automon/integrations/instagram/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/instagram/stories.py` & `automonisaur-0.5.0/automon/integrations/instagram/stories.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/instagram/tests/test_instagram_browser.py` & `automonisaur-0.5.0/automon/integrations/instagram/tests/test_instagram_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/instagram/tests/test_instagram_browser_auth.py` & `automonisaur-0.5.0/automon/integrations/instagram/tests/test_instagram_browser_auth.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/instagram/xpaths.py` & `automonisaur-0.5.0/automon/integrations/instagram/xpaths.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/ldap/client.py` & `automonisaur-0.5.0/automon/integrations/ldap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/mac/airport/airport.py` & `automonisaur-0.5.0/automon/integrations/mac/airport/airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/mac/airport/scan.py` & `automonisaur-0.5.0/automon/integrations/mac/airport/scan.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/mac/airport/ssid.py` & `automonisaur-0.5.0/automon/integrations/mac/airport/ssid.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/mac/airport/tests/test_airport.py` & `automonisaur-0.5.0/automon/integrations/mac/airport/tests/test_airport.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/mac/airport/tests/test_airport_neo4j.py` & `automonisaur-0.5.0/automon/integrations/mac/airport/tests/test_airport_neo4j.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/mac/macchanger/client.py` & `automonisaur-0.5.0/automon/integrations/mac/macchanger/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/mac/macchanger/tests/test_macchanger.py` & `automonisaur-0.5.0/automon/integrations/mac/macchanger/tests/test_macchanger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/minioWrapper/client.py` & `automonisaur-0.5.0/automon/integrations/minioWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/minioWrapper/config.py` & `automonisaur-0.5.0/automon/integrations/minioWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/minioWrapper/object.py` & `automonisaur-0.5.0/automon/integrations/minioWrapper/object.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/minioWrapper/tests/test_minio_client.py` & `automonisaur-0.5.0/automon/integrations/minioWrapper/tests/test_minio_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/minioWrapper/tests/test_minio_client_public.py` & `automonisaur-0.5.0/automon/integrations/minioWrapper/tests/test_minio_client_public.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py` & `automonisaur-0.5.0/automon/integrations/minioWrapper/tests/test_minio_client_public_clear_bucket.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/neo4jWrapper/client.py` & `automonisaur-0.5.0/automon/integrations/neo4jWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/neo4jWrapper/clientAsync.py` & `automonisaur-0.5.0/automon/integrations/neo4jWrapper/clientAsync.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/neo4jWrapper/config.py` & `automonisaur-0.5.0/automon/integrations/neo4jWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/neo4jWrapper/cypher.py` & `automonisaur-0.5.0/automon/integrations/neo4jWrapper/cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/neo4jWrapper/results.py` & `automonisaur-0.5.0/automon/integrations/neo4jWrapper/results.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py` & `automonisaur-0.5.0/automon/integrations/neo4jWrapper/tests/test_neo4j_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py` & `automonisaur-0.5.0/automon/integrations/neo4jWrapper/tests/test_neo4j_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py` & `automonisaur-0.5.0/automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/nmap/client.py` & `automonisaur-0.5.0/automon/integrations/nmap/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/nmap/config.py` & `automonisaur-0.5.0/automon/integrations/nmap/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/nmap/output.py` & `automonisaur-0.5.0/automon/integrations/nmap/output.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/nmap/tests/test_nmap_client.py` & `automonisaur-0.5.0/automon/integrations/nmap/tests/test_nmap_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/openvpn/openvpn.py` & `automonisaur-0.5.0/automon/integrations/openvpn/openvpn.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/requestsWrapper/client.py` & `automonisaur-0.5.0/automon/integrations/requestsWrapper/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -15,51 +15,48 @@
 
         self.config = config or RequestsConfig()
 
         self.url = url
         self.data = data
         self.errors = None
         self.headers = headers
-        self.results = None
+        self.response = None
         self.requests = requests
-
-        if url:
-            self.url = url
-            self.get(url=self.url, data=self.data, headers=self.headers)
+        self.session = self.requests.Session()
 
     def __repr__(self):
         return f'{self.__dict__}'
 
     def __len__(self):
         if self.content:
             len(self.content)
 
-    def _log_result(self):
-        if self.results.status_code == 200:
+    async def _log_result(self):
+        if self.status_code == 200:
             msg = [
-                self.results.request.method,
-                self.results.url,
-                f'{round(len(self.results.content) / 1024, 2)} KB',
-                self.results.status_code,
+                self.response.request.method,
+                self.response.url,
+                f'{round(len(self.content) / 1024, 2)} KB',
+                self.status_code,
             ]
             msg = ' '.join(msg)
             return logger.debug(msg)
 
         msg = [
-            self.results.request.method,
-            self.results.url,
-            f'{round(len(self.results.content) / 1024, 2)} KB',
-            self.results.status_code,
-            self.results.content
+            self.response.request.method,
+            self.response.url,
+            f'{round(len(self.content) / 1024, 2)} KB',
+            self.status_code,
+            self.content
         ]
 
         msg = ' '.join(msg)
         return logger.error(msg)
 
-    def _params(self, url, data, headers):
+    async def _params(self, url, data, headers):
         if url is None:
             url = self.url
 
         if data is None:
             data = self.data
 
         if headers is None:
@@ -68,131 +65,188 @@
         self.url = url
         self.data = data
         self.headers = headers
         return url, data, headers
 
     @property
     def content(self):
-        if self.results:
-            return self.results.content
+        if 'content' in dir(self.response):
+            return self.response.content
 
-    @property
-    def text(self):
-        if self.results:
-            return self.results.text
+    async def content_to_dict(self):
+        return await self.to_dict()
 
-    def delete(self,
-               url: str = None,
-               data: dict = None,
-               headers: dict = None, **kwargs) -> bool:
+    async def delete(
+            self,
+            url: str = None,
+            data: dict = None,
+            headers: dict = None,
+            **kwargs
+    ) -> bool:
         """requests.delete"""
 
-        url, data, headers = self._params(url, data, headers)
+        url, data, headers = await self._params(url, data, headers)
 
         try:
-            self.results = requests.delete(url=url, data=data, headers=headers, **kwargs)
-            self._log_result()
-            return True
+            self.response = self.session.delete(url=url, data=data, headers=headers, **kwargs)
+            await self._log_result()
+
+            if self.status_code == 200:
+                return True
+
+            return False
         except Exception as e:
             self.errors = e
             logger.error(f'delete failed. {e}')
         return False
 
-    def get(self,
+    async def get(
+            self,
             url: str = None,
             data: dict = None,
-            headers: dict = None, **kwargs) -> bool:
+            headers: dict = None,
+            **kwargs
+    ) -> bool:
         """requests.get"""
 
-        url, data, headers = self._params(url, data, headers)
+        url, data, headers = await self._params(url, data, headers)
 
         try:
-            self.results = requests.get(url=url, data=data, headers=headers, **kwargs)
+            self.response = self.session.get(url=url, data=data, headers=headers, **kwargs)
 
             logger.debug(
-                f'{self.results.url} '
-                f'{round(len(self.results.content) / 1024, 2)} KB '
-                f'{self.results.status_code}'
+                f'{self.response.url} '
+                f'{round(len(self.content) / 1024, 2)} KB '
+                f'{self.status_code}'
             )
 
-            return True
+            if self.status_code == 200:
+                return True
+
+            return False
         except Exception as e:
             self.errors = e
             logger.error(f'{e}')
         return False
 
-    def patch(self,
-              url: str = None,
-              data: dict = None,
-              headers: dict = None, **kwargs) -> bool:
+    async def patch(
+            self,
+            url: str = None,
+            data: dict = None,
+            headers: dict = None,
+            **kwargs
+    ) -> bool:
         """requests.patch"""
 
-        url, data, headers = self._params(url, data, headers)
+        url, data, headers = await self._params(url, data, headers)
 
         try:
-            self.results = requests.patch(url=url, data=data, headers=headers, **kwargs)
+            self.response = self.session.patch(url=url, data=data, headers=headers, **kwargs)
 
             logger.debug(
-                f'{self.results.url} '
-                f'{round(len(self.results.content) / 1024, 2)} KB '
-                f'{self.results.status_code}'
+                f'{self.response.url} '
+                f'{round(len(self.content) / 1024, 2)} KB '
+                f'{self.status_code}'
             )
 
-            return True
+            if self.status_code == 200:
+                return True
+
+            return False
         except Exception as e:
             self.errors = e
             logger.error(f'patch failed. {e}')
         return False
 
-    def post(self,
-             url: str = None,
-             data: dict = None,
-             headers: dict = None, **kwargs) -> bool:
+    async def post(
+            self,
+            url: str = None,
+            data: dict = None,
+            headers: dict = None,
+            **kwargs
+    ) -> bool:
         """requests.post"""
 
-        url, data, headers = self._params(url, data, headers)
+        url, data, headers = await self._params(url, data, headers)
 
         try:
-            self.results = requests.post(url=url, data=data, headers=headers, **kwargs)
+            self.response = self.session.post(url=url, data=data, headers=headers, **kwargs)
 
             logger.debug(
-                f'{self.results.url} '
-                f'{round(len(self.results.content) / 1024, 2)} KB '
-                f'{self.results.status_code}'
+                f'{self.response.url} '
+                f'{round(len(self.content) / 1024, 2)} KB '
+                f'{self.status_code}'
             )
 
-            return True
+            if self.status_code == 200:
+                return True
+
+            return False
         except Exception as e:
             self.errors = e
             logger.error(f'post failed. {e}')
         return False
 
-    def put(self,
+    async def put(
+            self,
             url: str = None,
             data: dict = None,
-            headers: dict = None, **kwargs) -> bool:
+            headers: dict = None,
+            **kwargs
+    ) -> bool:
         """requests.put"""
 
-        url, data, headers = self._params(url, data, headers)
+        url, data, headers = await self._params(url, data, headers)
 
         try:
-            self.results = requests.put(url=url, data=data, headers=headers, **kwargs)
+            self.response = self.session.put(url=url, data=data, headers=headers, **kwargs)
 
             logger.debug(
-                f'{self.results.url} '
-                f'{round(len(self.results.content) / 1024, 2)} KB '
-                f'{self.results.status_code}'
+                f'{self.response.url} '
+                f'{round(len(self.content) / 1024, 2)} KB '
+                f'{self.status_code}'
             )
 
-            return True
+            if self.status_code == 200:
+                return True
+
+            return False
         except Exception as e:
             self.errors = e
             logger.error(f'put failed. {e}')
         return False
 
-    def to_dict(self):
-        if self.results is not None:
-            return json.loads(self.results.content)
+    @property
+    def reason(self):
+        if 'reason' in dir(self.response):
+            return self.response.reason
+
+    @property
+    def status_code(self):
+        if 'status_code' in dir(self.response):
+            return self.response.status_code
+
+    @property
+    def text(self):
+        if self.response:
+            return self.response.text
+
+    async def to_dict(self):
+        if self.response is not None:
+            try:
+                return json.loads(self.content)
+            except Exception as error:
+                logger.error(error)
+
+    async def to_json(self):
+        if self.content:
+            try:
+                return json.dumps(json.loads(self.content))
+            except Exception as error:
+                logger.error(error)
+
+    async def update_headers(self, headers: dict):
+        return self.session.headers.update(headers)
 
 
 class Requests(RequestsClient):
     pass
```

### Comparing `automonisaur-0.4.2/automon/integrations/requestsWrapper/rest.py` & `automonisaur-0.5.0/automon/integrations/requestsWrapper/rest.py`

 * *Files 23% similar despite different names*

```diff
@@ -16,21 +16,21 @@
         self.requests = RequestsClient()
 
     def isConnected(self):
         if self.config.is_ready:
             return True
         return False
 
-    def get(self, url: str, data: str = None, headers: dict = None) -> bool:
-        return self.requests.get(url=url, data=data, headers=headers)
+    async def get(self, url: str, data: str = None, headers: dict = None) -> bool:
+        return await self.requests.get(url=url, data=data, headers=headers)
 
-    def post(self, url: str, data: str = None, headers: dict = None) -> bool:
-        return self.requests.post(url=url, data=data, headers=headers)
+    async def post(self, url: str, data: str = None, headers: dict = None) -> bool:
+        return await self.requests.post(url=url, data=data, headers=headers)
 
-    def delete(self, url: str, data: str = None, headers: dict = None) -> bool:
-        return self.requests.delete(url=url, data=data, headers=headers)
+    async def delete(self, url: str, data: str = None, headers: dict = None) -> bool:
+        return await self.requests.delete(url=url, data=data, headers=headers)
 
-    def patch(self, url: str, data: str = None, headers: dict = None) -> bool:
-        return self.requests.patch(url=url, data=data, headers=headers)
+    async def patch(self, url: str, data: str = None, headers: dict = None) -> bool:
+        return await self.requests.patch(url=url, data=data, headers=headers)
 
     def __repr__(self):
         return f'{self.__dict__}'
```

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/actions.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/actions.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/browser.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/browser.py`

 * *Files 1% similar despite different names*

```diff
@@ -323,14 +323,18 @@
             current_url=self.current_url,
             value=value,
         )))
         return self.find_element(value=value, by=by, **kwargs)
 
     async def get(self, url: str, **kwargs) -> bool:
         """get url"""
+        if not self.webdriver:
+            logger.error(f'missing webdriver')
+            raise Exception(f'missing webdriver')
+
         try:
             if self.webdriver.get(url, **kwargs) is None:
                 logger.info(str(dict(
                     url=url,
                     current_url=self.current_url,
                     kwargs=kwargs
                 )))
```

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/browser_types.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/browser_types.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/config.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/config_window_size.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/config_window_size.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_browser.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_browser.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_browser_headless.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_browser_useragent.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,30 +3,22 @@
 from automon.integrations.seleniumWrapper import SeleniumBrowser, ChromeWrapper
 
 browser = SeleniumBrowser()
 browser.config.webdriver_wrapper = ChromeWrapper()
 browser.config.webdriver_wrapper.enable_defaults()
 browser.config.webdriver_wrapper.enable_headless()
 
+agent = 'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:112.0) Gecko/20100101 Firefox/112.0'
 
-class SeleniumClientTest(unittest.TestCase):
+browser.config.webdriver_wrapper.set_user_agent(agent)
 
-    async def test(self):
-        if browser.run():
-            await browser.set_window_size(device_type='web-large')
-            while True:
-
-                try:
-                    if await browser.get('http://bing.com'):
-                        self.assertTrue(await browser.save_screenshot())
-                        self.assertTrue(await browser.save_screenshot())
-                        self.assertTrue(await browser.save_screenshot(folder='./'))
 
-                    await browser.quit()
-                    break
+class SeleniumClientTest(unittest.TestCase):
+    async def test_user_agent(self):
+        if await browser.run():
+            self.assertEqual(browser.user_agent, agent)
 
-                except:
-                    pass
+            await browser.quit()
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/tests/test_user_agent.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/tests/test_user_agent.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/user_agents.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/user_agents.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/seleniumWrapper/webdriver_chrome.py` & `automonisaur-0.5.0/automon/integrations/seleniumWrapper/webdriver_chrome.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
                 logger.debug(str(dict(
                     SELENIUM_CHROMEDRIVER_PATH=path,
                     PATH=os.environ['PATH']
                 )))
 
                 return True
 
-        logger.error(f'not found: {path}')
+        logger.error(f'chrome driver not found: {path}')
 
     async def quit(self):
         """quit
 
         """
         result = self.webdriver.quit()
         logger.info(f'{result}')
```

### Comparing `automonisaur-0.4.2/automon/integrations/sentryio/client.py` & `automonisaur-0.5.0/automon/integrations/sentryio/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/sentryio/config.py` & `automonisaur-0.5.0/automon/integrations/sentryio/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/sentryio/tests/test_sentryio.py` & `automonisaur-0.5.0/automon/integrations/sentryio/tests/test_sentryio.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/sentryio/tests/test_sentryio_callback.py` & `automonisaur-0.5.0/automon/integrations/sentryio/tests/test_sentryio_callback.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/shodan/__init__.py` & `automonisaur-0.5.0/automon/integrations/shodan/__init__.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/slackWrapper/bots.py` & `automonisaur-0.5.0/automon/integrations/slackWrapper/bots.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/slackWrapper/client.py` & `automonisaur-0.5.0/automon/integrations/slackWrapper/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/slackWrapper/clientAsync.py` & `automonisaur-0.5.0/automon/integrations/slackWrapper/clientAsync.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import slack
 import random
 import asyncio
 
 from automon import log
-from automon.helpers.nest_asyncioWrapper import AsyncStarter
+from automon.integrations.nest_asyncioWrapper import AsyncStarter
 
 from .config import ConfigSlack
 from .bots import BotInfo
 from .error import SlackError
 
 logger = log.logging.getLogger(__name__)
 logger.setLevel(log.ERROR)
```

### Comparing `automonisaur-0.4.2/automon/integrations/slackWrapper/config.py` & `automonisaur-0.5.0/automon/integrations/slackWrapper/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/slackWrapper/error.py` & `automonisaur-0.5.0/automon/integrations/slackWrapper/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/slackWrapper/slack_formatting.py` & `automonisaur-0.5.0/automon/integrations/slackWrapper/slack_formatting.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/slackWrapper/slack_logger.py` & `automonisaur-0.5.0/automon/integrations/slackWrapper/slack_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import traceback
 
 from json import dumps
 from asyncio import sleep
 
-from automon.helpers.nest_asyncioWrapper import AsyncStarter
+from automon.integrations.nest_asyncioWrapper import AsyncStarter
 from automon.integrations.slackWrapper.client import SlackClient
 
 from automon.integrations.slackWrapper.slack_formatting import Emoji, Chat, Format
 from automon import log
 from automon.log import INFO, ERROR, WARN, CRITICAL, DEBUG, TEST
 
 logger = log.logging.getLogger(__name__)
```

### Comparing `automonisaur-0.4.2/automon/integrations/slackWrapper/tests/test_slack.py` & `automonisaur-0.5.0/automon/integrations/slackWrapper/tests/test_slack.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/snmp/generate_maps.py` & `automonisaur-0.5.0/automon/integrations/snmp/generate_maps.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk/client.py` & `automonisaur-0.5.0/automon/integrations/splunk/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk/config.py` & `automonisaur-0.5.0/automon/integrations/splunk/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk/helpers.py` & `automonisaur-0.5.0/automon/integrations/splunk/helpers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk/tests/test_splunk_client.py` & `automonisaur-0.5.0/automon/integrations/splunk/tests/test_splunk_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk/tests/test_splunk_config.py` & `automonisaur-0.5.0/automon/integrations/splunk/tests/test_splunk_config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/client.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,16 +52,16 @@
         self.playbook_run = None
 
     def __repr__(self) -> str:
         return f'{self.__dict__}'
 
     def _content(self) -> bytes:
         """get result"""
-        if self.client.results:
-            return self.client.results.content
+        if self.client.response:
+            return self.client.response.content
         return b''
 
     def _content_dict(self) -> dict:
         """convert request.content to dict"""
         if self._content():
             return json.loads(self._content())
         return {}
@@ -91,15 +91,15 @@
         return self.client.post(url=url, headers=self.client.headers, data=data)
 
     @_is_connected
     def close_container(self, container_id: int, **kwargs) -> Optional[CloseContainerResponse]:
         """Set container status to closed"""
         data = dict(status='closed')
         if self._post(Urls.container(identifier=container_id, **kwargs), data=json.dumps(data)):
-            if self.client.results.status_code == 200:
+            if self.client.response.status_code == 200:
                 response = CloseContainerResponse(self._content_dict())
                 logger.info(f'container closed: {response}')
                 return response
 
         logger.error(msg=f'close failed. {self.client.to_dict()}')
 
     @_is_connected
@@ -108,15 +108,15 @@
             playbook_run_id: int = None,
             cancel: bool = True, **kwargs) -> CancelPlaybookResponse:
         """Cancel playbook run"""
         data = dict(cancel=cancel)
         data = json.dumps(data)
 
         if self._post(Urls.playbook_run(identifier=playbook_run_id, **kwargs), data=data):
-            if self.client.results.status_code == 200:
+            if self.client.response.status_code == 200:
                 response = CancelPlaybookResponse(self._content_dict())
                 logger.info(f'cancel playbook run: {response}')
                 return response
 
         logger.error(f'cancel failed: {playbook_run_id} {self.client.to_dict()}')
 
     @_is_connected
@@ -159,15 +159,15 @@
                  source_data_identifier=source_data_identifier,
                  start_time=start_time,
                  tags=tags,
                  type=type)
         )
 
         if self._post(Urls.artifact(*args, **kwargs), data=artifact.to_json()):
-            if self.client.results.status_code == 200:
+            if self.client.response.status_code == 200:
                 id = self.client.to_dict()['id']
                 logger.info(f'artifact created. {artifact} {self.client.to_dict()}')
                 return self.get_artifact(artifact_id=id)
             else:
                 existing_artifact_id = self.client.to_dict()['existing_artifact_id']
                 logger.info(f'artifact exists. {artifact} {self.client.to_dict()}')
                 return self.get_artifact(artifact_id=existing_artifact_id)
@@ -233,15 +233,15 @@
                  tenant_id=tenant_id,
                  container_type=container_type,
                  template_id=template_id,
                  authorized_users=authorized_users)
         )
 
         if self._post(Urls.container(*args, **kwargs), data=container.to_json()):
-            if self.client.results.status_code == 200:
+            if self.client.response.status_code == 200:
                 response = CreateContainerResponse(self.client.to_dict())
                 logger.info(f'container created. {container} {response}')
                 return response
         logger.error(f'create container. {self.client.to_dict()}')
         return False
 
     @staticmethod
@@ -305,27 +305,27 @@
 
     @_is_connected
     def delete_container(self, container_id, *args, **kwargs):
         """Delete containers"""
         assert isinstance(container_id, int)
 
         if self._delete(Urls.container(identifier=container_id, *args, **kwargs)):
-            if self.client.results.status_code == 200:
+            if self.client.response.status_code == 200:
                 logger.info(f'container deleted: {container_id}')
                 return True
         logger.error(f'delete container: {container_id}. {self.client.to_dict()}')
         return False
 
     def is_connected(self) -> bool:
         """check if client can connect"""
         if self.config.is_ready:
             if self._get(Urls.container(page_size=1)):
                 logger.info(f'client connected '
                             f'{self.config.host} '
-                            f'[{self.client.results.status_code}] ')
+                            f'[{self.client.response.status_code}] ')
                 return True
 
         else:
             logger.warning(f'client not connected')
         return False
 
     @_is_connected
@@ -422,15 +422,15 @@
 
         logger.error(f'playbook failed: {self.client.errors}')
 
     @_is_connected
     def get_vault(self, vault_id: int, **kwargs) -> Optional[Vault]:
         """Get vault object"""
         if self._get(Urls.vault(identifier=vault_id, **kwargs)):
-            if self.client.results.status_code == 200:
+            if self.client.response.status_code == 200:
                 response = Vault(self._content_dict())
                 logger.info(msg=f'get vault: {response}')
                 return response
 
         logger.error(msg=f'get vault failed: {self.client.to_dict()}')
 
     @_is_connected
@@ -726,15 +726,15 @@
         """Update playbook active state"""
         data = dict(
             active=active,
             cancel_runs=cancel_runs
         )
         data = json.dumps(data)
         if self._post(Urls.playbook(identifier=playbook_id, **kwargs), data=data):
-            if self.client.results.status_code == 200:
+            if self.client.response.status_code == 200:
                 response = UpdatePlaybookResponse(self._content_dict())
                 logger.info(f'update playbook: {data}')
                 return response
 
         logger.error(f'update failed: {self.client.to_dict()}')
 
     @_is_connected
@@ -750,13 +750,13 @@
             container_id=container_id,
             playbook_id=playbook_id,
             scope=scope,
             run=run
         )
         data = json.dumps(data)
         if self._post(Urls.playbook_run(**kwargs), data=data):
-            if self.client.results.status_code == 200:
+            if self.client.response.status_code == 200:
                 response = RunPlaybookResponse(self._content_dict())
                 logger.info(f'run playbook: {data}')
                 return response
 
         logger.error(f'run failed: {self.client.to_dict()}')
```

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/config.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/datatypes.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/datatypes.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/integration/servicenow/ticket.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/integration/servicenow/ticket.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/phantom_unittest.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/phantom_unittest.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/responses.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/responses.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/rest/urls.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/rest/urls.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/rules.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/rules.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/tests/dino.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/tests/dino.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_create_container_attachment.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_client_list_containers.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_uat.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_uat.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_uat_run_playbook.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/tests/test_soar_uat_update_playbook.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/splunk_soar/vault.py` & `automonisaur-0.5.0/automon/integrations/splunk_soar/vault.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/swift/client.py` & `automonisaur-0.5.0/automon/integrations/swift/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/swift/config.py` & `automonisaur-0.5.0/automon/integrations/swift/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/swift/error.py` & `automonisaur-0.5.0/automon/integrations/swift/error.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/swift/iterables.py` & `automonisaur-0.5.0/automon/integrations/swift/iterables.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/swift/tests/test_swift.py` & `automonisaur-0.5.0/automon/integrations/swift/tests/test_swift.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/vds/client.py` & `automonisaur-0.5.0/automon/integrations/vds/client.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/integrations/vds/config.py` & `automonisaur-0.5.0/automon/integrations/vds/config.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/log/attributes.py` & `automonisaur-0.5.0/automon/log/attributes.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/log/logger.py` & `automonisaur-0.5.0/automon/log/logger.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automon/log/tests/test_logger_builtin.py` & `automonisaur-0.5.0/automon/log/tests/test_logger_builtin.py`

 * *Files identical despite different names*

### Comparing `automonisaur-0.4.2/automonisaur.egg-info/PKG-INFO` & `automonisaur-0.5.0/automonisaur.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automonisaur
-Version: 0.4.2
+Version: 0.5.0
 Summary: Core libraries for automonisaur
 Home-page: https://github.com/TheShellLand/automonisaur
 Author: naisanza
 Author-email: naisanza@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -57,17 +57,19 @@
 | API             | flask                                                       |
 | Chat            | slack                                                       |
 | Data Scraping   | beautifulsoup<br/>facebook groups<br/>instagram<br/>scrapy  |
 | Databases       | elasticsearch<br/>neo4j<br/>splunk                          |
 | Data Store      | minio<br/>swift                                             |
 | Devices         | snmp                                                        |
 | Google Cloud    | google auth api<br/>google people api<br/>google sheets api |
+| Helpers         | os<br/>subprocess<br/>threading<br/>socket<br/>datetime     |
 | Logging         | sentryio                                                    |
-| macOS           | airport<br/>macchanger                                      |
+| MacOS           | airport<br/>macchanger                                      |
 | Python          | logging<br/>requests                                        |
+| SOAR            | swimlane<br/>splunk soar                                    |
 | Recon           | nmap                                                        |
 | Test Automation | selenium                                                    |
 
 #### Requires
 
 - python >= 3.8
```

### Comparing `automonisaur-0.4.2/automonisaur.egg-info/SOURCES.txt` & `automonisaur-0.5.0/automonisaur.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,45 +2,40 @@
 README.md
 setup.py
 automon/__init__.py
 automon/healthcheck.py
 automon/liveliness.py
 automon/helpers/__init__.py
 automon/helpers/assertions.py
-automon/helpers/cpu.py
 automon/helpers/dates.py
 automon/helpers/httpWrapper.py
 automon/helpers/markdown.py
 automon/helpers/networking.py
 automon/helpers/regex.py
 automon/helpers/sanitation.py
 automon/helpers/sleeper.py
 automon/helpers/asyncioWrapper/__init__.py
 automon/helpers/asyncioWrapper/loop.py
 automon/helpers/cryptography/__init__.py
 automon/helpers/cryptography/hashing.py
 automon/helpers/cryptography/secret.py
-automon/helpers/grok/__init__.py
 automon/helpers/mathWrapper/__init__.py
 automon/helpers/mathWrapper/file_size.py
-automon/helpers/nest_asyncioWrapper/__init__.py
-automon/helpers/nest_asyncioWrapper/client.py
 automon/helpers/osWrapper/__init__.py
 automon/helpers/osWrapper/environ.py
 automon/helpers/subprocessWrapper/__init__.py
 automon/helpers/subprocessWrapper/exceptions.py
 automon/helpers/subprocessWrapper/run.py
 automon/helpers/subprocessWrapper/tests/__init__.py
 automon/helpers/subprocessWrapper/tests/test_pipe.py
 automon/helpers/subprocessWrapper/tests/test_run.py
 automon/helpers/subprocessWrapper/tests/test_runner.py
 automon/helpers/subprocessWrapper/tests/test_sanitize.py
 automon/helpers/tests/__init__.py
 automon/helpers/tests/test_assertions.py
-automon/helpers/tests/test_grok.py
 automon/helpers/tests/test_healthcheck.py
 automon/helpers/tests/test_helpers.py
 automon/helpers/tests/test_liveliness.py
 automon/helpers/tests/test_networking.py
 automon/helpers/tests/test_sanitation.py
 automon/helpers/tests/test_sleeper.py
 automon/helpers/tests/test_sleeper_async.py
@@ -53,14 +48,23 @@
 automon/integrations/cryptocurrency/__init__.py
 automon/integrations/cryptocurrency/accounting.py
 automon/integrations/cryptocurrency/coinbase.py
 automon/integrations/cryptocurrency/other.py
 automon/integrations/cryptocurrency/robinhood.py
 automon/integrations/cryptocurrency/tests/__init__.py
 automon/integrations/cryptocurrency/tests/test_crypto.py
+automon/integrations/datadogWrapper/__init__.py
+automon/integrations/datadogWrapper/client.py
+automon/integrations/datadogWrapper/config.py
+automon/integrations/datadogWrapper/api/__init__.py
+automon/integrations/datadogWrapper/api/v1.py
+automon/integrations/datadogWrapper/api/v2.py
+automon/integrations/datadogWrapper/tests/__init__.py
+automon/integrations/datadogWrapper/tests/test_auth.py
+automon/integrations/datadogWrapper/tests/test_log.py
 automon/integrations/datascience/__init__.py
 automon/integrations/datascience/pandas/__init__.py
 automon/integrations/datascience/pandas/dataframe.py
 automon/integrations/datascience/pandas/pandas.py
 automon/integrations/datascience/pandas/series.py
 automon/integrations/datascience/tests/__init__.py
 automon/integrations/datascience/tests/test_datascience.py
@@ -115,14 +119,17 @@
 automon/integrations/google/sheets/tests/__init__.py
 automon/integrations/google/sheets/tests/test_google_sheets.py
 automon/integrations/google/sheets/tests/test_google_sheets_AUDIT.py
 automon/integrations/google/sheets/tests/test_google_sheets_clear.py
 automon/integrations/google/tests/__init__.py
 automon/integrations/google/tests/test_google_contacts.py
 automon/integrations/google/tests/test_google_contacts_neo4j.py
+automon/integrations/grok/__init__.py
+automon/integrations/grok/tests/__init__.py
+automon/integrations/grok/tests/test_grok.py
 automon/integrations/instagram/__init__.py
 automon/integrations/instagram/client.py
 automon/integrations/instagram/client_browser.py
 automon/integrations/instagram/config.py
 automon/integrations/instagram/stories.py
 automon/integrations/instagram/urls.py
 automon/integrations/instagram/xpaths.py
@@ -163,23 +170,34 @@
 automon/integrations/neo4jWrapper/config.py
 automon/integrations/neo4jWrapper/cypher.py
 automon/integrations/neo4jWrapper/results.py
 automon/integrations/neo4jWrapper/tests/__init__.py
 automon/integrations/neo4jWrapper/tests/test_neo4j_client.py
 automon/integrations/neo4jWrapper/tests/test_neo4j_config.py
 automon/integrations/neo4jWrapper/tests/test_neo4j_cypher.py
+automon/integrations/nest_asyncioWrapper/__init__.py
+automon/integrations/nest_asyncioWrapper/client.py
 automon/integrations/nmap/__init__.py
 automon/integrations/nmap/client.py
 automon/integrations/nmap/config.py
 automon/integrations/nmap/output.py
 automon/integrations/nmap/tests/__init__.py
 automon/integrations/nmap/tests/test_nmap_client.py
 automon/integrations/nmap/tests/test_nmap_config.py
+automon/integrations/openTelemetryWrapper/__init__.py
+automon/integrations/openTelemetryWrapper/client.py
+automon/integrations/openTelemetryWrapper/config.py
+automon/integrations/openTelemetryWrapper/test/__init__.py
+automon/integrations/openTelemetryWrapper/test/test_client_ready.py
+automon/integrations/openTelemetryWrapper/test/test_memory_trace.py
+automon/integrations/openTelemetryWrapper/test/test_pop_finished_spans.py
 automon/integrations/openvpn/__init__.py
 automon/integrations/openvpn/openvpn.py
+automon/integrations/psutilWrapper/__init__.py
+automon/integrations/psutilWrapper/cpu.py
 automon/integrations/requestsWrapper/__init__.py
 automon/integrations/requestsWrapper/client.py
 automon/integrations/requestsWrapper/config.py
 automon/integrations/requestsWrapper/rest.py
 automon/integrations/requestsWrapper/tests/__init__.py
 automon/integrations/requestsWrapper/tests/test_requests.py
 automon/integrations/requestsWrapper/tests/test_rest.py
@@ -267,14 +285,30 @@
 automon/integrations/swift/__init__.py
 automon/integrations/swift/client.py
 automon/integrations/swift/config.py
 automon/integrations/swift/error.py
 automon/integrations/swift/iterables.py
 automon/integrations/swift/tests/__init__.py
 automon/integrations/swift/tests/test_swift.py
+automon/integrations/swimlaneWrapper/__init__.py
+automon/integrations/swimlaneWrapper/client.py
+automon/integrations/swimlaneWrapper/config.py
+automon/integrations/swimlaneWrapper/api/__init__.py
+automon/integrations/swimlaneWrapper/api/v2.py
+automon/integrations/swimlaneWrapper/tests/__init__.py
+automon/integrations/swimlaneWrapper/tests/test_library_record_create.py
+automon/integrations/swimlaneWrapper/tests/test_rest_app.py
+automon/integrations/swimlaneWrapper/tests/test_rest_auth.py
+automon/integrations/swimlaneWrapper/tests/test_rest_auth_token.py
+automon/integrations/swimlaneWrapper/tests/test_rest_logging.py
+automon/integrations/swimlaneWrapper/tests/test_rest_record.py
+automon/integrations/swimlaneWrapper/tests/test_rest_record_create.py
+automon/integrations/swimlaneWrapper/tests/test_rest_record_delete_all.py
+automon/integrations/swimlaneWrapper/tests/test_rest_record_resolve_fields.py
+automon/integrations/swimlaneWrapper/tests/test_rest_workspace.py
 automon/integrations/vds/__init__.py
 automon/integrations/vds/client.py
 automon/integrations/vds/config.py
 automon/integrations/vds/tests/__init__.py
 automon/integrations/vds/tests/test_vds.py
 automon/log/__init__.py
 automon/log/attributes.py
```

### Comparing `automonisaur-0.4.2/setup.py` & `automonisaur-0.5.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="automonisaur",
-    version="0.4.2",
+    version="0.5.0",
     author="naisanza",
     author_email="naisanza@gmail.com",
     description="Core libraries for automonisaur",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheShellLand/automonisaur",
     packages=setuptools.find_packages(),
```

