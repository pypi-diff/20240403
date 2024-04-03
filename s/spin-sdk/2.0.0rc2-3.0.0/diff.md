# Comparing `tmp/spin-sdk-2.0.0rc2.tar.gz` & `tmp/spin-sdk-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spin-sdk-2.0.0rc2.tar", last modified: Tue Feb 13 21:33:08 2024, max compression
+gzip compressed data, was "spin-sdk-3.0.0.tar", last modified: Wed Apr  3 21:43:43 2024, max compression
```

## Comparing `spin-sdk-2.0.0rc2.tar` & `spin-sdk-3.0.0.tar`

### file list

```diff
@@ -1,103 +1,106 @@
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.063237 spin-sdk-2.0.0rc2/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    11602 2024-02-12 17:37:12.000000 spin-sdk-2.0.0rc2/LICENSE
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)       53 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/MANIFEST.in
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    16575 2024-02-13 21:33:08.062984 spin-sdk-2.0.0rc2/PKG-INFO
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2750 2024-02-12 17:37:15.000000 spin-sdk-2.0.0rc2/README.md
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      660 2024-02-13 21:32:35.000000 spin-sdk-2.0.0rc2/pyproject.toml
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)       38 2024-02-13 21:33:08.063279 spin-sdk-2.0.0rc2/setup.cfg
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.048215 spin-sdk-2.0.0rc2/src/
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.051274 spin-sdk-2.0.0rc2/src/spin_sdk/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      282 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/__init__.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)       39 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/componentize-py.toml
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.052096 spin-sdk-2.0.0rc2/src/spin_sdk/http/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     7420 2024-02-13 21:31:38.000000 spin-sdk-2.0.0rc2/src/spin_sdk/http/__init__.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    12290 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/http/poll_loop.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1808 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/key_value.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2225 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/llm.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      557 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/mysql.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      570 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/postgres.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)        0 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/py.typed
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      790 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/redis.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1358 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/sqlite.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      109 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/variables.py
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.054084 spin-sdk-2.0.0rc2/src/spin_sdk/wit/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      363 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/__init__.py
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.048865 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.055144 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)       77 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/command.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      709 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/environment.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      107 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/exit.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      445 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/imports.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)       66 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/run.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      316 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/stdio.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1677 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/terminal.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.055550 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/clocks/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1525 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/clocks/monotonic-clock.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1674 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/clocks/wall-clock.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)       97 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/clocks/world.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.056161 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/filesystem/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      213 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/filesystem/preopens.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    27621 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/filesystem/types.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)       89 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/filesystem/world.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.056581 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/http/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1807 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/http/handler.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1439 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/http/proxy.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    24187 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/http/types.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.057451 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/io/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1444 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/io/error.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1590 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/io/poll.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    12096 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/io/streams.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)       79 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/io/world.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.057986 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/random/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1104 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/random/insecure-seed.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      863 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/random/insecure.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1149 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/random/random.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      112 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/random/world.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.059387 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      222 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/instance-network.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2603 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/ip-name-lookup.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     4175 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/network.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1487 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/tcp-create-socket.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    20199 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/tcp.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1477 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/udp-create-socket.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    15189 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/udp.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      215 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/world.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.059772 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/spin@unversioned/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      191 2024-02-12 17:37:21.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/spin@unversioned/inbound-redis.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      462 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/spin@unversioned/redis-types.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.060142 spin-sdk-2.0.0rc2/src/spin_sdk/wit/exports/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1402 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/exports/__init__.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      253 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/exports/inbound_redis.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      393 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/exports/incoming_handler.py
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.062569 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)        0 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/__init__.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1878 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/error.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2750 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/key_value.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2011 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/llm.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1479 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/monotonic_clock.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1483 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/mysql.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1150 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/outgoing_handler.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2142 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/poll.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1458 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/postgres.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     3386 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/rdbms_types.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     4475 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/redis.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      963 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/redis_types.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2341 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/sqlite.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    12938 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/streams.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    33152 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/types.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      897 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/variables.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1644 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/key-value.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2313 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/llm.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      556 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/mysql.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      537 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/postgres.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1462 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/rdbms-types.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2452 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/redis.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      451 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/spin.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     1600 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/sqlite.wit
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      471 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/types.py
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)      658 2024-01-29 17:46:20.000000 spin-sdk-2.0.0rc2/src/spin_sdk/wit/variables.wit
-drwxr-xr-x   0 karthik_ganeshram   (501) staff       (20)        0 2024-02-13 21:33:08.062749 spin-sdk-2.0.0rc2/src/spin_sdk.egg-info/
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)    16575 2024-02-13 21:33:08.000000 spin-sdk-2.0.0rc2/src/spin_sdk.egg-info/PKG-INFO
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)     2944 2024-02-13 21:33:08.000000 spin-sdk-2.0.0rc2/src/spin_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)        1 2024-02-13 21:33:08.000000 spin-sdk-2.0.0rc2/src/spin_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 karthik_ganeshram   (501) staff       (20)        9 2024-02-13 21:33:08.000000 spin-sdk-2.0.0rc2/src/spin_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.637630 spin-sdk-3.0.0/
+-rw-r--r--   0 dicej      (501) staff       (20)    11602 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/LICENSE
+-rw-r--r--   0 dicej      (501) staff       (20)       53 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/MANIFEST.in
+-rw-r--r--   0 dicej      (501) staff       (20)    16202 2024-04-03 21:43:43.637439 spin-sdk-3.0.0/PKG-INFO
+-rw-r--r--   0 dicej      (501) staff       (20)     2380 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/README.md
+-rw-r--r--   0 dicej      (501) staff       (20)      657 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/pyproject.toml
+-rw-r--r--   0 dicej      (501) staff       (20)       38 2024-04-03 21:43:43.637662 spin-sdk-3.0.0/setup.cfg
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.624387 spin-sdk-3.0.0/src/
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.627451 spin-sdk-3.0.0/src/spin_sdk/
+-rw-r--r--   0 dicej      (501) staff       (20)      282 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/__init__.py
+-rw-r--r--   0 dicej      (501) staff       (20)       39 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/componentize-py.toml
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.628326 spin-sdk-3.0.0/src/spin_sdk/http/
+-rw-r--r--   0 dicej      (501) staff       (20)     7459 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/http/__init__.py
+-rw-r--r--   0 dicej      (501) staff       (20)    12299 2024-04-03 21:21:04.000000 spin-sdk-3.0.0/src/spin_sdk/http/poll_loop.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1816 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/key_value.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2222 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/llm.py
+-rw-r--r--   0 dicej      (501) staff       (20)      989 2024-04-03 21:41:05.000000 spin-sdk-3.0.0/src/spin_sdk/mqtt.py
+-rw-r--r--   0 dicej      (501) staff       (20)      561 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/mysql.py
+-rw-r--r--   0 dicej      (501) staff       (20)      573 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/postgres.py
+-rw-r--r--   0 dicej      (501) staff       (20)        0 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/py.typed
+-rw-r--r--   0 dicej      (501) staff       (20)      795 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/redis.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1416 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/sqlite.py
+-rw-r--r--   0 dicej      (501) staff       (20)      195 2024-02-28 16:52:28.000000 spin-sdk-3.0.0/src/spin_sdk/variables.py
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.630327 spin-sdk-3.0.0/src/spin_sdk/wit/
+-rw-r--r--   0 dicej      (501) staff       (20)      356 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/__init__.py
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.625069 spin-sdk-3.0.0/src/spin_sdk/wit/deps/
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.631348 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/
+-rw-r--r--   0 dicej      (501) staff       (20)       77 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/command.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      709 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/environment.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      107 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/exit.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      445 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/imports.wit
+-rw-r--r--   0 dicej      (501) staff       (20)       66 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/run.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      316 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/stdio.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1677 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/terminal.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.631710 spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/
+-rw-r--r--   0 dicej      (501) staff       (20)     1525 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/monotonic-clock.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1674 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/wall-clock.wit
+-rw-r--r--   0 dicej      (501) staff       (20)       97 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.632108 spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/
+-rw-r--r--   0 dicej      (501) staff       (20)      213 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/preopens.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    27621 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/types.wit
+-rw-r--r--   0 dicej      (501) staff       (20)       89 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.632469 spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/
+-rw-r--r--   0 dicej      (501) staff       (20)     1807 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/handler.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1439 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/proxy.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    24187 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/types.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.633232 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/
+-rw-r--r--   0 dicej      (501) staff       (20)     1444 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/error.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1590 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/poll.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    12096 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/streams.wit
+-rw-r--r--   0 dicej      (501) staff       (20)       79 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.633717 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/
+-rw-r--r--   0 dicej      (501) staff       (20)     1104 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/insecure-seed.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      863 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/insecure.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1149 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/random.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      112 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.634743 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/
+-rw-r--r--   0 dicej      (501) staff       (20)      222 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/instance-network.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     2603 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/ip-name-lookup.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     4175 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/network.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1487 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/tcp-create-socket.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    20199 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/tcp.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1477 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/udp-create-socket.wit
+-rw-r--r--   0 dicej      (501) staff       (20)    15189 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/udp.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      215 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/world.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.635021 spin-sdk-3.0.0/src/spin_sdk/wit/deps/spin@unversioned/
+-rw-r--r--   0 dicej      (501) staff       (20)      191 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/spin@unversioned/inbound-redis.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      462 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/deps/spin@unversioned/redis-types.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.635337 spin-sdk-3.0.0/src/spin_sdk/wit/exports/
+-rw-r--r--   0 dicej      (501) staff       (20)     1395 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/exports/__init__.py
+-rw-r--r--   0 dicej      (501) staff       (20)      246 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/exports/inbound_redis.py
+-rw-r--r--   0 dicej      (501) staff       (20)      386 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/exports/incoming_handler.py
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.637075 spin-sdk-3.0.0/src/spin_sdk/wit/imports/
+-rw-r--r--   0 dicej      (501) staff       (20)        0 2024-04-02 19:59:36.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/__init__.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1871 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/error.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2751 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/key_value.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2010 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/llm.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1472 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/monotonic_clock.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1621 2024-04-03 21:41:05.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/mqtt.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1476 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/mysql.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1143 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/outgoing_handler.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2135 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/poll.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1451 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/postgres.py
+-rw-r--r--   0 dicej      (501) staff       (20)     3447 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/rdbms_types.py
+-rw-r--r--   0 dicej      (501) staff       (20)     4488 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/redis.py
+-rw-r--r--   0 dicej      (501) staff       (20)      968 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/redis_types.py
+-rw-r--r--   0 dicej      (501) staff       (20)     2354 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/sqlite.py
+-rw-r--r--   0 dicej      (501) staff       (20)    12935 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/streams.py
+-rw-r--r--   0 dicej      (501) staff       (20)    33255 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/types.py
+-rw-r--r--   0 dicej      (501) staff       (20)      898 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/imports/variables.py
+-rw-r--r--   0 dicej      (501) staff       (20)     1644 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/key-value.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     2313 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/llm.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      916 2024-04-03 21:41:05.000000 spin-sdk-3.0.0/src/spin_sdk/wit/mqtt.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      556 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/mysql.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      537 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/postgres.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1462 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/rdbms-types.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     2452 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/redis.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      466 2024-04-03 21:41:05.000000 spin-sdk-3.0.0/src/spin_sdk/wit/spin.wit
+-rw-r--r--   0 dicej      (501) staff       (20)     1600 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/sqlite.wit
+-rw-r--r--   0 dicej      (501) staff       (20)      452 2024-04-03 21:20:56.000000 spin-sdk-3.0.0/src/spin_sdk/wit/types.py
+-rw-r--r--   0 dicej      (501) staff       (20)      658 2024-02-16 14:45:39.000000 spin-sdk-3.0.0/src/spin_sdk/wit/variables.wit
+drwxr-xr-x   0 dicej      (501) staff       (20)        0 2024-04-03 21:43:43.637240 spin-sdk-3.0.0/src/spin_sdk.egg-info/
+-rw-r--r--   0 dicej      (501) staff       (20)    16202 2024-04-03 21:43:43.000000 spin-sdk-3.0.0/src/spin_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dicej      (501) staff       (20)     3024 2024-04-03 21:43:43.000000 spin-sdk-3.0.0/src/spin_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dicej      (501) staff       (20)        1 2024-04-03 21:43:43.000000 spin-sdk-3.0.0/src/spin_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dicej      (501) staff       (20)        9 2024-04-03 21:43:43.000000 spin-sdk-3.0.0/src/spin_sdk.egg-info/top_level.txt
```

### Comparing `spin-sdk-2.0.0rc2/LICENSE` & `spin-sdk-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/PKG-INFO` & `spin-sdk-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-sdk
-Version: 2.0.0rc2
+Version: 3.0.0
 Summary: Experimental SDK for Spin and Componentize-Py
 Author-email: Fermyon Engineering <engineering@fermyon.com>
 Maintainer-email: Fermyon Engineering <engineering@fermyon.com>
 License:                               Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
@@ -230,38 +230,35 @@
 
 # Spin Python SDK
 
 This is an SDK for creating [Spin](https://github.com/fermyon/spin) apps using Python.
 
 Note that this SDK supersedes an earlier, experimental version, which may be
 found in the [old-sdk](https://github.com/fermyon/spin-python-sdk/tree/old-sdk)
-branch. _(The old template remains on `main` temporarily to preserve compatibility for some
-inbound links; it will be removed or replaced.)_
+branch.
 
 ## [API Documentation](https://fermyon.github.io/spin-python-sdk/index.html)
 
 ## Example
 
 ### Prerequisites
 
 - [Python 3.10 or later and pip](https://www.python.org/downloads/)
 - [componentize-py](https://pypi.org/project/componentize-py/)
 - [spin-sdk](https://pypi.org/project/spin-sdk/)
-- [MyPy](https://pypi.org/project/mypy/)
-    - This is optional, but useful for during development.
 - [Spin](https://github.com/fermyon/spin) 2.2 or later.
-    - As of this writing Spin 2.2 has not yet been released, so we must use the `main` branch of Spin for the time being. You can find pre-built binaries [here](https://github.com/fermyon/spin/releases/tag/canary).
+- [MyPy](https://pypi.org/project/mypy/) -- This is optional, but useful for during development.
 
 Once you have Python and pip installed, you can use the latter to create and
 enter a virtual environment and then install the desired packages
 
 ```shell
 python -m venv .venv
 source .venv/bin/activate
-pip install componentize-py==0.11.0 spin-sdk==2.0.0rc1 mypy==1.8.0
+pip install componentize-py==0.13.1 spin-sdk==3.0.0 mypy==1.8.0
 ```
 
 ### Hello, World
 
 A minimal app requires two files: a `spin.toml` and a Python script, which we'll
 name `app.py`:
 
@@ -283,18 +280,18 @@
 [component.hello.build]
 command = "componentize-py -w spin-http componentize app -o app.wasm"
 EOF
 ```
 
 ```shell
 cat >app.py <<EOF
-from spin_sdk.http import simple
-from spin_sdk.http.simple import Request, Response
+from spin_sdk import http
+from spin_sdk.http import Request, Response
 
-class IncomingHandler(simple.IncomingHandler):
+class IncomingHandler(http.IncomingHandler):
     def handle_request(self, request: Request) -> Response:
         return Response(
             200,
             {"content-type": "text/plain"},
             bytes("Hello from Python!", "utf-8")
         )
 EOF
```

### Comparing `spin-sdk-2.0.0rc2/README.md` & `spin-sdk-3.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # Spin Python SDK
 
 This is an SDK for creating [Spin](https://github.com/fermyon/spin) apps using Python.
 
 Note that this SDK supersedes an earlier, experimental version, which may be
 found in the [old-sdk](https://github.com/fermyon/spin-python-sdk/tree/old-sdk)
-branch. _(The old template remains on `main` temporarily to preserve compatibility for some
-inbound links; it will be removed or replaced.)_
+branch.
 
 ## [API Documentation](https://fermyon.github.io/spin-python-sdk/index.html)
 
 ## Example
 
 ### Prerequisites
 
 - [Python 3.10 or later and pip](https://www.python.org/downloads/)
 - [componentize-py](https://pypi.org/project/componentize-py/)
 - [spin-sdk](https://pypi.org/project/spin-sdk/)
-- [MyPy](https://pypi.org/project/mypy/)
-    - This is optional, but useful for during development.
 - [Spin](https://github.com/fermyon/spin) 2.2 or later.
-    - As of this writing Spin 2.2 has not yet been released, so we must use the `main` branch of Spin for the time being. You can find pre-built binaries [here](https://github.com/fermyon/spin/releases/tag/canary).
+- [MyPy](https://pypi.org/project/mypy/) -- This is optional, but useful for during development.
 
 Once you have Python and pip installed, you can use the latter to create and
 enter a virtual environment and then install the desired packages
 
 ```shell
 python -m venv .venv
 source .venv/bin/activate
-pip install componentize-py==0.11.0 spin-sdk==2.0.0rc1 mypy==1.8.0
+pip install componentize-py==0.13.1 spin-sdk==3.0.0 mypy==1.8.0
 ```
 
 ### Hello, World
 
 A minimal app requires two files: a `spin.toml` and a Python script, which we'll
 name `app.py`:
 
@@ -53,18 +50,18 @@
 [component.hello.build]
 command = "componentize-py -w spin-http componentize app -o app.wasm"
 EOF
 ```
 
 ```shell
 cat >app.py <<EOF
-from spin_sdk.http import simple
-from spin_sdk.http.simple import Request, Response
+from spin_sdk import http
+from spin_sdk.http import Request, Response
 
-class IncomingHandler(simple.IncomingHandler):
+class IncomingHandler(http.IncomingHandler):
     def handle_request(self, request: Request) -> Response:
         return Response(
             200,
             {"content-type": "text/plain"},
             bytes("Hello from Python!", "utf-8")
         )
 EOF
```

### Comparing `spin-sdk-2.0.0rc2/pyproject.toml` & `spin-sdk-3.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spin-sdk"
-version = "2.0.0rc2"
+version = "3.0.0"
 description = "Experimental SDK for Spin and Componentize-Py"
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [ { name = "Fermyon Engineering", email = "engineering@fermyon.com" } ]
 maintainers = [ { name = "Fermyon Engineering", email = "engineering@fermyon.com" } ]
 keywords = [ "webassembly", "wasm", "component", "spin" ]
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/http/__init__.py` & `spin-sdk-3.0.0/src/spin_sdk/http/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import traceback
 
 from spin_sdk.wit import exports
 from spin_sdk.wit.types import Ok, Err
 from spin_sdk.wit.imports import types, outgoing_handler
 from spin_sdk.wit.imports.types import (
-    Method, MethodGet, MethodHead, MethodPost, MethodPut, MethodDelete, MethodConnect, MethodOptions, MethodTrace,
-    MethodPatch, MethodOther, IncomingRequest, IncomingBody, ResponseOutparam, OutgoingResponse, Fields, Scheme,
-    SchemeHttp, SchemeHttps, SchemeOther, OutgoingRequest, OutgoingBody
+    Method, Method_Get, Method_Head, Method_Post, Method_Put, Method_Delete, Method_Connect, Method_Options,
+    Method_Trace, Method_Patch, Method_Other, IncomingRequest, IncomingBody, ResponseOutparam, OutgoingResponse,
+    Fields, Scheme, Scheme_Http, Scheme_Https, Scheme_Other, OutgoingRequest, OutgoingBody
 )
-from spin_sdk.wit.imports.streams import StreamErrorClosed
+from spin_sdk.wit.imports.streams import StreamError_Closed
 from dataclasses import dataclass
 from collections.abc import Mapping
 from typing import Optional
 from urllib import parse
 
 @dataclass
 class Request:
@@ -37,45 +37,45 @@
     def handle_request(self, request: Request) -> Response:
         """Handle an incoming HTTP request and return a response or raise an error"""
         raise NotImplementedError
     
     def handle(self, request: IncomingRequest, response_out: ResponseOutparam):
         method = request.method()
 
-        if isinstance(method, MethodGet):
+        if isinstance(method, Method_Get):
             method_str = "GET"
-        elif isinstance(method, MethodHead):
+        elif isinstance(method, Method_Head):
             method_str = "HEAD"
-        elif isinstance(method, MethodPost):
+        elif isinstance(method, Method_Post):
             method_str = "POST"
-        elif isinstance(method, MethodPut):
+        elif isinstance(method, Method_Put):
             method_str = "PUT"
-        elif isinstance(method, MethodDelete):
+        elif isinstance(method, Method_Delete):
             method_str = "DELETE"
-        elif isinstance(method, MethodConnect):
+        elif isinstance(method, Method_Connect):
             method_str = "CONNECT"
-        elif isinstance(method, MethodOptions):
+        elif isinstance(method, Method_Options):
             method_str = "OPTIONS"
-        elif isinstance(method, MethodTrace):
+        elif isinstance(method, Method_Trace):
             method_str = "TRACE"
-        elif isinstance(method, MethodPatch):
+        elif isinstance(method, Method_Patch):
             method_str = "PATCH"
-        elif isinstance(method, MethodOther):
+        elif isinstance(method, Method_Other):
             method_str = method.value
         else:
             raise AssertionError
 
         request_body = request.consume()
         request_stream = request_body.stream()
         body = bytearray()
         while True:
             try:
                 body += request_stream.blocking_read(16 * 1024)
             except Err as e:
-                if isinstance(e.value, StreamErrorClosed):
+                if isinstance(e.value, StreamError_Closed):
                     request_stream.__exit__()
                     IncomingBody.finish(request_body)
                     break
                 else:
                     raise e
 
         request_uri = request.path_with_query()
@@ -118,43 +118,43 @@
         OutgoingBody.finish(response_body, None)
     
 def send(request: Request) -> Response:
     """Send an HTTP request and return a response or raise an error"""
 
     match request.method:
         case "GET":
-            method: Method = MethodGet()
+            method: Method = Method_Get()
         case "HEAD":
-            method = MethodHead()
+            method = Method_Head()
         case "POST":
-            method = MethodPost()
+            method = Method_Post()
         case "PUT":
-            method = MethodPut()
+            method = Method_Put()
         case "DELETE":
-            method = MethodDelete()
+            method = Method_Delete()
         case "CONNECT":
-            method = MethodConnect()
+            method = Method_Connect()
         case "OPTIONS":
-            method = MethodOptions()
+            method = Method_Options()
         case "TRACE":
-            method = MethodTrace()
+            method = Method_Trace()
         case "PATCH":
-            method = MethodPatch()
+            method = Method_Patch()
         case _:
-            method = MethodOther(request.method)
+            method = Method_Other(request.method)
     
     url_parsed = parse.urlparse(request.uri)
 
     match url_parsed.scheme:
         case "http":
-            scheme: Scheme = SchemeHttp()
+            scheme: Scheme = Scheme_Http()
         case "https":
-            scheme = SchemeHttps()
+            scheme = Scheme_Https()
         case _:
-            scheme = SchemeOther(url_parsed.scheme)
+            scheme = Scheme_Other(url_parsed.scheme)
 
     outgoing_request = OutgoingRequest(Fields.from_list(list(map(
         lambda pair: (pair[0], bytes(pair[1], "utf-8")),
         request.headers.items()
     ))))
     outgoing_request.set_method(method)
     outgoing_request.set_scheme(scheme)
@@ -181,15 +181,15 @@
                     response_body = response_value.consume()
                     response_stream = response_body.stream()
                     body = bytearray()
                     while True:
                         try:
                             body += response_stream.blocking_read(16 * 1024)
                         except Err as e:
-                            if isinstance(e.value, StreamErrorClosed):
+                            if isinstance(e.value, StreamError_Closed):
                                 response_stream.__exit__()
                                 IncomingBody.finish(response_body)
                                 simple_response = Response(
                                     response_value.status(),
                                     dict(map(
                                         lambda pair: (pair[0], str(pair[1], "utf-8")),
                                         response_value.headers().entries()
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/http/poll_loop.py` & `spin-sdk-3.0.0/src/spin_sdk/http/poll_loop.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import asyncio
 import socket
 import subprocess
 
 from spin_sdk.wit.types import Ok, Err
 from spin_sdk.wit.imports import types, streams, poll, outgoing_handler
 from spin_sdk.wit.imports.types import IncomingBody, OutgoingBody, OutgoingRequest, IncomingResponse
-from spin_sdk.wit.imports.streams import StreamErrorClosed, InputStream
+from spin_sdk.wit.imports.streams import StreamError_Closed, InputStream
 from spin_sdk.wit.imports.poll import Pollable
 from typing import Optional, cast
 
 # Maximum number of bytes to read at a time
 READ_SIZE: int = 16 * 1024
 
 async def send(request: OutgoingRequest) -> IncomingResponse:
@@ -59,15 +59,15 @@
                 else:
                     buffer = self.stream.read(READ_SIZE)
                     if len(buffer) == 0:
                         await register(cast(PollLoop, asyncio.get_event_loop()), self.stream.subscribe())
                     else:
                         return buffer
             except Err as e:
-                if isinstance(e.value, StreamErrorClosed):
+                if isinstance(e.value, StreamError_Closed):
                     if self.stream is not None:
                         self.stream.__exit__()
                         self.stream = None
                     if self.body is not None:
                         IncomingBody.finish(self.body)
                         self.body = None
                 else:
@@ -148,15 +148,15 @@
                         new_wakers.append((pollable, waker))
 
                 self.wakers = new_wakers
 
             if self.exception is not None:
                 raise self.exception
             
-        future.result()
+        return future.result()
 
     def is_running(self):
         return self.running
 
     def is_closed(self):
         return not self.running
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/key_value.py` & `spin-sdk-3.0.0/src/spin_sdk/key_value.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,33 +6,33 @@
     """
     Open the store with the specified name.
   
     If `name` is "default", the default store is opened.  Otherwise, `name` must
     refer to a store defined and configured in a runtime configuration file
     supplied with the application.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.ErrorNoSuchStore)` will be raised if the `name` is not recognized.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.Error_NoSuchStore)` will be raised if the `name` is not recognized.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.ErrorAccessDenied)` will be raised if the requesting component does not have
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.Error_AccessDenied)` will be raised if the requesting component does not have
     access to the specified store.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.ErrorStoreTableFull)` will be raised if too many stores have been opened simultaneously.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.Error_StoreTableFull)` will be raised if too many stores have been opened simultaneously.
     Closing one or more previously opened stores might address this using the `__exit__` method.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.ErrorOther(str))` will be raised if some implementation specific error has occured (e.g I/O)
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.Error_Other(str))` will be raised if some implementation specific error has occured (e.g I/O)
     """
     return Store.open(name)
 
 def open_default() -> Store:
     """
     Open the default store.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.ErrorAccessDenied)`
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.Error_AccessDenied)`
     will be raised if the requesting component does not have access to the
     default store.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.ErrorStoreTableFull)` will be raised if too many stores have been opened simultaneously.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.Error_StoreTableFull)` will be raised if too many stores have been opened simultaneously.
     Closing one or more previously opened stores might address this using the `__exit__` method.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.ErrorOther(str))` will be raised if some implementation specific error has occured (e.g I/O)
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.key_value.Error_Other(str))` will be raised if some implementation specific error has occured (e.g I/O)
     """
-    return Store.open("default")
+    return Store.open("default")
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/llm.py` & `spin-sdk-3.0.0/src/spin_sdk/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 """Module for working with the Spin large language model API"""
 
 from dataclasses import dataclass
 from typing import Optional, Sequence
 from spin_sdk.wit.imports import llm as spin_llm
 
 @dataclass
-class LLMInferencingParams:
+class InferencingParams:
     max_tokens: int = 100
     repeat_penalty: float = 1.1
     repeat_penalty_last_n_token_count: int = 64
     temperature: float = 0.8
     top_k: int = 40
     top_p: float = 0.9
     
 
 def generate_embeddings(model: str, text: Sequence[str]) -> spin_llm.EmbeddingsResult:
     """
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorModelNotSupported)` will be raised if the component does not have access to the specified model.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_ModelNotSupported)` will be raised if the component does not have access to the specified model.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorRuntimeError(str))` will be raised if there are any runtime errors.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_RuntimeError(str))` will be raised if there are any runtime errors.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorInvalidInput(str))` will be raised if an invalid input is provided.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_InvalidInput(str))` will be raised if an invalid input is provided.
     """
     return spin_llm.generate_embeddings(model, text)
 
-def infer_with_options(model: str, prompt: str, options: Optional[LLMInferencingParams]) -> spin_llm.InferencingResult:
+def infer_with_options(model: str, prompt: str, options: Optional[InferencingParams]) -> spin_llm.InferencingResult:
     """
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorModelNotSupported)` will be raised if the component does not have access to the specified model.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_ModelNotSupported)` will be raised if the component does not have access to the specified model.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorRuntimeError(str))` will be raised if there are any runtime errors.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_RuntimeError(str))` will be raised if there are any runtime errors.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorInvalidInput(str))` will be raised if an invalid input is provided.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_InvalidInput(str))` will be raised if an invalid input is provided.
     """
-    options = options or LLMInferencingParams
+    options = options or InferencingParams
     return spin_llm.infer(model, prompt, options)
 
 def infer(model: str, prompt: str) -> spin_llm.InferencingResult:
     """
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorModelNotSupported)` will be raised if the component does not have access to the specified model.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_ModelNotSupported)` will be raised if the component does not have access to the specified model.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorRuntimeError(str))` will be raised if there are any runtime errors.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_RuntimeError(str))` will be raised if there are any runtime errors.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.ErrorInvalidInput(str))` will be raised if an invalid input is provided.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.llm.Error_InvalidInput(str))` will be raised if an invalid input is provided.
     """
-    options = LLMInferencingParams
+    options = InferencingParams
     return spin_llm.infer(model, prompt, options)
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/mysql.py` & `spin-sdk-3.0.0/src/spin_sdk/postgres.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Module for interacting with a MySQL database"""
+"""Module for interacting with a Postgres database"""
 
-from spin_sdk.wit.imports.mysql import Connection
+from spin_sdk.wit.imports.postgres import Connection
 
 def open(connection_string: str) -> Connection:
     """
-    Open a connection with a MySQL database.
+    Open a connection with a Postgres database.
     
-    The connection_string is the MySQL URL connection string.
+    The connection_string is the Postgres URL connection string.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.rdbms_types.ErrorConnectionFailed(str))` when a connection fails.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.rdbms_types.Error_ConnectionFailed(str))` when a connection fails.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.import.rdbms_types.ErrorOther(str))` when some other error occurs.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.rdbms_types.Error_Other(str))` when some other error occurs.
     """
-    return Connection.open(connection_string)
+    return Connection.open(connection_string)
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/postgres.py` & `spin-sdk-3.0.0/src/spin_sdk/mysql.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-"""Module for interacting with a Postgres database"""
+"""Module for interacting with a MySQL database"""
 
-from spin_sdk.wit.imports.postgres import Connection
+from spin_sdk.wit.imports.mysql import Connection
 
 def open(connection_string: str) -> Connection:
     """
-    Open a connection with a Postgres database.
+    Open a connection with a MySQL database.
     
-    The connection_string is the Postgres URL connection string.
+    The connection_string is the MySQL URL connection string.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.rdbms_types.ErrorConnectionFailed(str))` when a connection fails.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.rdbms_types.Error_ConnectionFailed(str))` when a connection fails.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.rdbms_types.ErrorOther(str))` when some other error occurs.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.rdbms_types.Error_Other(str))` when some other error occurs.
     """
-    return Connection.open(connection_string)
+    return Connection.open(connection_string)
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/redis.py` & `spin-sdk-3.0.0/src/spin_sdk/mqtt.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-"""Module for interacting with a Redis database"""
+"""Module for utilizing Spin Outbound MQTT"""
 
-from spin_sdk.wit.imports.redis import Connection 
+from enum import Enum
+from spin_sdk.wit.imports.mqtt import Connection, Qos as Qos 
 
-def open(connection_string: str) -> Connection:
+def open(address: str, username: str, password: str, keep_alive_interval_in_secs: int) -> Connection:
     """
-    Open a connection with a Redis database.
+    Open a connection to the Mqtt instance at `address`.
     
-    The connection_string is the Redis URL to connect to.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.mqtt.Error_InvalidAddress)` will be raised if the connection string is invalid.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.redis.ErrorInvalidAddress)` will be raised if the connection string is invalid.
-
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.redis.ErrorTooManyConnection)` will be raised if there are too many open connections. Closing one or more previously opened connection using the `__exit__` method might help.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.mqtt.Error_TooManyConnections)` will be raised if there are too many open connections. Closing one or more previously opened connection using the `__exit__` method might help.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.redis.ErrorOther(str))` when some other error occurs.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.mqtt.Error_ConnectionFailed)` will be raised if the connection failed.
+
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.mqtt.Error_Other(str))` when some other error occurs.
     """
-    return Connection.open(connection_string)
+    return Connection.open(address, username, password, keep_alive_interval_in_secs)
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/sqlite.py` & `spin-sdk-3.0.0/src/spin_sdk/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """Module for interacting with an SQLite database"""
 
 from typing import List
-from spin_sdk.wit.imports.sqlite import Connection
+from spin_sdk.wit.imports.sqlite import Connection, Value_Integer, Value_Real, Value_Text, Value_Blob
 
 def open(name: str) -> Connection:
     """Open a connection to a named database instance.
 
     If `database` is "default", the default instance is opened.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.ErrorAccessDenied)` will be raised when the component does not have access to the specified database.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.Error_AccessDenied)` will be raised when the component does not have access to the specified database.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.ErrorNoSuchDatabase)` will be raised when the host does not recognize the database name requested.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.Error_NoSuchDatabase)` will be raised when the host does not recognize the database name requested.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.ErrorInvalidConnection)` will be raised when the provided connection string is not valid.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.Error_InvalidConnection)` will be raised when the provided connection string is not valid.
     
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.ErrorIo(str))` will be raised when implementation-specific error occured (e.g. I/O)
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.Error_Io(str))` will be raised when implementation-specific error occured (e.g. I/O)
     """
     return Connection.open(name)
 
 def open_default() -> Connection:
     """Open the default store.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.ErrorAccessDenied)` will be raised when the component does not have access to the default database.
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.Error_AccessDenied)` will be raised when the component does not have access to the default database.
 
-    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.ErrorIo(str))` will be raised when implementation-specific error occured (e.g. I/O)
+    A `spin_sdk.wit.types.Err(spin_sdk.wit.imports.sqlite.Error_Io(str))` will be raised when implementation-specific error occured (e.g. I/O)
     """
-    return Connection.open("default")
+    return Connection.open("default")
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/environment.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/environment.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/cli/terminal.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/cli/terminal.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/clocks/monotonic-clock.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/monotonic-clock.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/clocks/wall-clock.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/clocks/wall-clock.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/filesystem/types.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/filesystem/types.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/http/handler.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/handler.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/http/proxy.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/proxy.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/http/types.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/http/types.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/io/error.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/error.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/io/poll.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/poll.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/io/streams.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/io/streams.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/random/insecure-seed.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/insecure-seed.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/random/insecure.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/insecure.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/random/random.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/random/random.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/ip-name-lookup.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/ip-name-lookup.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/network.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/network.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/tcp-create-socket.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/tcp-create-socket.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/tcp.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/tcp.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/udp-create-socket.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/udp-create-socket.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/deps/sockets/udp.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/deps/sockets/udp.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/exports/__init__.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/exports/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 from ..imports import types
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/error.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/error.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/key_value.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/key_value.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 
 
 
 @dataclass
-class ErrorStoreTableFull:
+class Error_StoreTableFull:
     pass
 
 
 @dataclass
-class ErrorNoSuchStore:
+class Error_NoSuchStore:
     pass
 
 
 @dataclass
-class ErrorAccessDenied:
+class Error_AccessDenied:
     pass
 
 
 @dataclass
-class ErrorOther:
+class Error_Other:
     value: str
 
 
-Error = Union[ErrorStoreTableFull, ErrorNoSuchStore, ErrorAccessDenied, ErrorOther]
+Error = Union[Error_StoreTableFull, Error_NoSuchStore, Error_AccessDenied, Error_Other]
 """
 The set of errors which may be raised by functions in this interface
 """
 
 
 class Store:
     """
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/llm.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/llm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 A WASI interface dedicated to performing inferencing for Large Language Models.
 """
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 
@@ -20,29 +20,29 @@
     repeat_penalty_last_n_token_count: int
     temperature: float
     top_k: int
     top_p: float
 
 
 @dataclass
-class ErrorModelNotSupported:
+class Error_ModelNotSupported:
     pass
 
 
 @dataclass
-class ErrorRuntimeError:
+class Error_RuntimeError:
     value: str
 
 
 @dataclass
-class ErrorInvalidInput:
+class Error_InvalidInput:
     value: str
 
 
-Error = Union[ErrorModelNotSupported, ErrorRuntimeError, ErrorInvalidInput]
+Error = Union[Error_ModelNotSupported, Error_RuntimeError, Error_InvalidInput]
 """
 The set of errors which may be raised by functions in this interface
 """
 
 
 @dataclass
 class InferencingUsage:
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/monotonic_clock.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/monotonic_clock.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Windows.
 
 A monotonic clock is a clock which has an unspecified initial value, and
 successive reads of the clock will produce non-decreasing values.
 
 It is intended for measuring elapsed time.
 """
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 from ..imports import poll
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/mysql.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/mysql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 from ..imports import rdbms_types
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/outgoing_handler.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/outgoing_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This interface defines a handler of outgoing HTTP Requests. It should be
 imported by components which wish to make HTTP Requests.
 """
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 from ..imports import types
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/poll.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/poll.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 A poll API intended to let users wait for I/O events on multiple handles
 at once.
 """
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/postgres.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/postgres.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 from ..imports import rdbms_types
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/redis.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/redis.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 
 
 
 @dataclass
-class ErrorInvalidAddress:
+class Error_InvalidAddress:
     pass
 
 
 @dataclass
-class ErrorTooManyConnections:
+class Error_TooManyConnections:
     pass
 
 
 @dataclass
-class ErrorTypeError:
+class Error_TypeError:
     pass
 
 
 @dataclass
-class ErrorOther:
+class Error_Other:
     value: str
 
 
-Error = Union[ErrorInvalidAddress, ErrorTooManyConnections, ErrorTypeError, ErrorOther]
+Error = Union[Error_InvalidAddress, Error_TooManyConnections, Error_TypeError, Error_Other]
 """
 Errors related to interacting with Redis
 """
 
 
 
 @dataclass
-class RedisParameterInt64:
+class RedisParameter_Int64:
     value: int
 
 
 @dataclass
-class RedisParameterBinary:
+class RedisParameter_Binary:
     value: bytes
 
 
-RedisParameter = Union[RedisParameterInt64, RedisParameterBinary]
+RedisParameter = Union[RedisParameter_Int64, RedisParameter_Binary]
 """
 A parameter type for the general-purpose `execute` function.
 """
 
 
 
 @dataclass
-class RedisResultNil:
+class RedisResult_Nil:
     pass
 
 
 @dataclass
-class RedisResultStatus:
+class RedisResult_Status:
     value: str
 
 
 @dataclass
-class RedisResultInt64:
+class RedisResult_Int64:
     value: int
 
 
 @dataclass
-class RedisResultBinary:
+class RedisResult_Binary:
     value: bytes
 
 
-RedisResult = Union[RedisResultNil, RedisResultStatus, RedisResultInt64, RedisResultBinary]
+RedisResult = Union[RedisResult_Nil, RedisResult_Status, RedisResult_Int64, RedisResult_Binary]
 """
 A return type for the general-purpose `execute` function.
 """
 
 
 class Connection:
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/redis_types.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/redis_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 
@@ -12,50 +12,50 @@
     General purpose error.
     """
     SUCCESS = 0
     ERROR = 1
 
 
 @dataclass
-class RedisParameterInt64:
+class RedisParameter_Int64:
     value: int
 
 
 @dataclass
-class RedisParameterBinary:
+class RedisParameter_Binary:
     value: bytes
 
 
-RedisParameter = Union[RedisParameterInt64, RedisParameterBinary]
+RedisParameter = Union[RedisParameter_Int64, RedisParameter_Binary]
 """
 A parameter type for the general-purpose `execute` function.
 """
 
 
 
 @dataclass
-class RedisResultNil:
+class RedisResult_Nil:
     pass
 
 
 @dataclass
-class RedisResultStatus:
+class RedisResult_Status:
     value: str
 
 
 @dataclass
-class RedisResultInt64:
+class RedisResult_Int64:
     value: int
 
 
 @dataclass
-class RedisResultBinary:
+class RedisResult_Binary:
     value: bytes
 
 
-RedisResult = Union[RedisResultNil, RedisResultStatus, RedisResultInt64, RedisResultBinary]
+RedisResult = Union[RedisResult_Nil, RedisResult_Status, RedisResult_Int64, RedisResult_Binary]
 """
 A return type for the general-purpose `execute` function.
 """
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/sqlite.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/sqlite.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,75 +1,75 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 
 
 
 @dataclass
-class ErrorNoSuchDatabase:
+class Error_NoSuchDatabase:
     pass
 
 
 @dataclass
-class ErrorAccessDenied:
+class Error_AccessDenied:
     pass
 
 
 @dataclass
-class ErrorInvalidConnection:
+class Error_InvalidConnection:
     pass
 
 
 @dataclass
-class ErrorDatabaseFull:
+class Error_DatabaseFull:
     pass
 
 
 @dataclass
-class ErrorIo:
+class Error_Io:
     value: str
 
 
-Error = Union[ErrorNoSuchDatabase, ErrorAccessDenied, ErrorInvalidConnection, ErrorDatabaseFull, ErrorIo]
+Error = Union[Error_NoSuchDatabase, Error_AccessDenied, Error_InvalidConnection, Error_DatabaseFull, Error_Io]
 """
 The set of errors which may be raised by functions in this interface
 """
 
 
 
 @dataclass
-class ValueInteger:
+class Value_Integer:
     value: int
 
 
 @dataclass
-class ValueReal:
+class Value_Real:
     value: float
 
 
 @dataclass
-class ValueText:
+class Value_Text:
     value: str
 
 
 @dataclass
-class ValueBlob:
+class Value_Blob:
     value: bytes
 
 
 @dataclass
-class ValueNull:
+class Value_Null:
     pass
 
 
-Value = Union[ValueInteger, ValueReal, ValueText, ValueBlob, ValueNull]
+Value = Union[Value_Integer, Value_Real, Value_Text, Value_Blob, Value_Null]
 """
 A single column's result from a database query
 """
 
 
 @dataclass
 class RowResult:
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/streams.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """
 WASI I/O is an I/O abstraction API which is currently focused on providing
 stream types.
 
 In the future, the component model is expected to add built-in stream types;
 when it does, they are expected to subsume this API.
 """
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
-from ..imports import poll
 from ..imports import error
+from ..imports import poll
 
 
 @dataclass
-class StreamErrorLastOperationFailed:
+class StreamError_LastOperationFailed:
     value: error.Error
 
 
 @dataclass
-class StreamErrorClosed:
+class StreamError_Closed:
     pass
 
 
-StreamError = Union[StreamErrorLastOperationFailed, StreamErrorClosed]
+StreamError = Union[StreamError_LastOperationFailed, StreamError_Closed]
 """
 An error for input-stream and output-stream operations.
 """
 
 
 class InputStream:
     """
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/types.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 """
 This interface defines all of the types and methods for implementing
 HTTP Requests and Responses, both incoming and outgoing, as well as
 their headers, trailers, and bodies.
 """
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 from ..imports import poll
 from ..imports import streams
 from ..imports import error
 
 
 @dataclass
-class MethodGet:
+class Method_Get:
     pass
 
 
 @dataclass
-class MethodHead:
+class Method_Head:
     pass
 
 
 @dataclass
-class MethodPost:
+class Method_Post:
     pass
 
 
 @dataclass
-class MethodPut:
+class Method_Put:
     pass
 
 
 @dataclass
-class MethodDelete:
+class Method_Delete:
     pass
 
 
 @dataclass
-class MethodConnect:
+class Method_Connect:
     pass
 
 
 @dataclass
-class MethodOptions:
+class Method_Options:
     pass
 
 
 @dataclass
-class MethodTrace:
+class Method_Trace:
     pass
 
 
 @dataclass
-class MethodPatch:
+class Method_Patch:
     pass
 
 
 @dataclass
-class MethodOther:
+class Method_Other:
     value: str
 
 
-Method = Union[MethodGet, MethodHead, MethodPost, MethodPut, MethodDelete, MethodConnect, MethodOptions, MethodTrace, MethodPatch, MethodOther]
+Method = Union[Method_Get, Method_Head, Method_Post, Method_Put, Method_Delete, Method_Connect, Method_Options, Method_Trace, Method_Patch, Method_Other]
 """
 This type corresponds to HTTP standard Methods.
 """
 
 
 
 @dataclass
-class SchemeHttp:
+class Scheme_Http:
     pass
 
 
 @dataclass
-class SchemeHttps:
+class Scheme_Https:
     pass
 
 
 @dataclass
-class SchemeOther:
+class Scheme_Other:
     value: str
 
 
-Scheme = Union[SchemeHttp, SchemeHttps, SchemeOther]
+Scheme = Union[Scheme_Http, Scheme_Https, Scheme_Other]
 """
 This type corresponds to HTTP standard Related Schemes.
 """
 
 
 @dataclass
 class DnsErrorPayload:
@@ -115,232 +115,232 @@
     Defines the case payload type for `HTTP-response-{header,trailer}-size` above:
     """
     field_name: Optional[str]
     field_size: Optional[int]
 
 
 @dataclass
-class ErrorCodeDnsTimeout:
+class ErrorCode_DnsTimeout:
     pass
 
 
 @dataclass
-class ErrorCodeDnsError:
+class ErrorCode_DnsError:
     value: DnsErrorPayload
 
 
 @dataclass
-class ErrorCodeDestinationNotFound:
+class ErrorCode_DestinationNotFound:
     pass
 
 
 @dataclass
-class ErrorCodeDestinationUnavailable:
+class ErrorCode_DestinationUnavailable:
     pass
 
 
 @dataclass
-class ErrorCodeDestinationIpProhibited:
+class ErrorCode_DestinationIpProhibited:
     pass
 
 
 @dataclass
-class ErrorCodeDestinationIpUnroutable:
+class ErrorCode_DestinationIpUnroutable:
     pass
 
 
 @dataclass
-class ErrorCodeConnectionRefused:
+class ErrorCode_ConnectionRefused:
     pass
 
 
 @dataclass
-class ErrorCodeConnectionTerminated:
+class ErrorCode_ConnectionTerminated:
     pass
 
 
 @dataclass
-class ErrorCodeConnectionTimeout:
+class ErrorCode_ConnectionTimeout:
     pass
 
 
 @dataclass
-class ErrorCodeConnectionReadTimeout:
+class ErrorCode_ConnectionReadTimeout:
     pass
 
 
 @dataclass
-class ErrorCodeConnectionWriteTimeout:
+class ErrorCode_ConnectionWriteTimeout:
     pass
 
 
 @dataclass
-class ErrorCodeConnectionLimitReached:
+class ErrorCode_ConnectionLimitReached:
     pass
 
 
 @dataclass
-class ErrorCodeTlsProtocolError:
+class ErrorCode_TlsProtocolError:
     pass
 
 
 @dataclass
-class ErrorCodeTlsCertificateError:
+class ErrorCode_TlsCertificateError:
     pass
 
 
 @dataclass
-class ErrorCodeTlsAlertReceived:
+class ErrorCode_TlsAlertReceived:
     value: TlsAlertReceivedPayload
 
 
 @dataclass
-class ErrorCodeHttpRequestDenied:
+class ErrorCode_HttpRequestDenied:
     pass
 
 
 @dataclass
-class ErrorCodeHttpRequestLengthRequired:
+class ErrorCode_HttpRequestLengthRequired:
     pass
 
 
 @dataclass
-class ErrorCodeHttpRequestBodySize:
+class ErrorCode_HttpRequestBodySize:
     value: Optional[int]
 
 
 @dataclass
-class ErrorCodeHttpRequestMethodInvalid:
+class ErrorCode_HttpRequestMethodInvalid:
     pass
 
 
 @dataclass
-class ErrorCodeHttpRequestUriInvalid:
+class ErrorCode_HttpRequestUriInvalid:
     pass
 
 
 @dataclass
-class ErrorCodeHttpRequestUriTooLong:
+class ErrorCode_HttpRequestUriTooLong:
     pass
 
 
 @dataclass
-class ErrorCodeHttpRequestHeaderSectionSize:
+class ErrorCode_HttpRequestHeaderSectionSize:
     value: Optional[int]
 
 
 @dataclass
-class ErrorCodeHttpRequestHeaderSize:
+class ErrorCode_HttpRequestHeaderSize:
     value: Optional[FieldSizePayload]
 
 
 @dataclass
-class ErrorCodeHttpRequestTrailerSectionSize:
+class ErrorCode_HttpRequestTrailerSectionSize:
     value: Optional[int]
 
 
 @dataclass
-class ErrorCodeHttpRequestTrailerSize:
+class ErrorCode_HttpRequestTrailerSize:
     value: FieldSizePayload
 
 
 @dataclass
-class ErrorCodeHttpResponseIncomplete:
+class ErrorCode_HttpResponseIncomplete:
     pass
 
 
 @dataclass
-class ErrorCodeHttpResponseHeaderSectionSize:
+class ErrorCode_HttpResponseHeaderSectionSize:
     value: Optional[int]
 
 
 @dataclass
-class ErrorCodeHttpResponseHeaderSize:
+class ErrorCode_HttpResponseHeaderSize:
     value: FieldSizePayload
 
 
 @dataclass
-class ErrorCodeHttpResponseBodySize:
+class ErrorCode_HttpResponseBodySize:
     value: Optional[int]
 
 
 @dataclass
-class ErrorCodeHttpResponseTrailerSectionSize:
+class ErrorCode_HttpResponseTrailerSectionSize:
     value: Optional[int]
 
 
 @dataclass
-class ErrorCodeHttpResponseTrailerSize:
+class ErrorCode_HttpResponseTrailerSize:
     value: FieldSizePayload
 
 
 @dataclass
-class ErrorCodeHttpResponseTransferCoding:
+class ErrorCode_HttpResponseTransferCoding:
     value: Optional[str]
 
 
 @dataclass
-class ErrorCodeHttpResponseContentCoding:
+class ErrorCode_HttpResponseContentCoding:
     value: Optional[str]
 
 
 @dataclass
-class ErrorCodeHttpResponseTimeout:
+class ErrorCode_HttpResponseTimeout:
     pass
 
 
 @dataclass
-class ErrorCodeHttpUpgradeFailed:
+class ErrorCode_HttpUpgradeFailed:
     pass
 
 
 @dataclass
-class ErrorCodeHttpProtocolError:
+class ErrorCode_HttpProtocolError:
     pass
 
 
 @dataclass
-class ErrorCodeLoopDetected:
+class ErrorCode_LoopDetected:
     pass
 
 
 @dataclass
-class ErrorCodeConfigurationError:
+class ErrorCode_ConfigurationError:
     pass
 
 
 @dataclass
-class ErrorCodeInternalError:
+class ErrorCode_InternalError:
     value: Optional[str]
 
 
-ErrorCode = Union[ErrorCodeDnsTimeout, ErrorCodeDnsError, ErrorCodeDestinationNotFound, ErrorCodeDestinationUnavailable, ErrorCodeDestinationIpProhibited, ErrorCodeDestinationIpUnroutable, ErrorCodeConnectionRefused, ErrorCodeConnectionTerminated, ErrorCodeConnectionTimeout, ErrorCodeConnectionReadTimeout, ErrorCodeConnectionWriteTimeout, ErrorCodeConnectionLimitReached, ErrorCodeTlsProtocolError, ErrorCodeTlsCertificateError, ErrorCodeTlsAlertReceived, ErrorCodeHttpRequestDenied, ErrorCodeHttpRequestLengthRequired, ErrorCodeHttpRequestBodySize, ErrorCodeHttpRequestMethodInvalid, ErrorCodeHttpRequestUriInvalid, ErrorCodeHttpRequestUriTooLong, ErrorCodeHttpRequestHeaderSectionSize, ErrorCodeHttpRequestHeaderSize, ErrorCodeHttpRequestTrailerSectionSize, ErrorCodeHttpRequestTrailerSize, ErrorCodeHttpResponseIncomplete, ErrorCodeHttpResponseHeaderSectionSize, ErrorCodeHttpResponseHeaderSize, ErrorCodeHttpResponseBodySize, ErrorCodeHttpResponseTrailerSectionSize, ErrorCodeHttpResponseTrailerSize, ErrorCodeHttpResponseTransferCoding, ErrorCodeHttpResponseContentCoding, ErrorCodeHttpResponseTimeout, ErrorCodeHttpUpgradeFailed, ErrorCodeHttpProtocolError, ErrorCodeLoopDetected, ErrorCodeConfigurationError, ErrorCodeInternalError]
+ErrorCode = Union[ErrorCode_DnsTimeout, ErrorCode_DnsError, ErrorCode_DestinationNotFound, ErrorCode_DestinationUnavailable, ErrorCode_DestinationIpProhibited, ErrorCode_DestinationIpUnroutable, ErrorCode_ConnectionRefused, ErrorCode_ConnectionTerminated, ErrorCode_ConnectionTimeout, ErrorCode_ConnectionReadTimeout, ErrorCode_ConnectionWriteTimeout, ErrorCode_ConnectionLimitReached, ErrorCode_TlsProtocolError, ErrorCode_TlsCertificateError, ErrorCode_TlsAlertReceived, ErrorCode_HttpRequestDenied, ErrorCode_HttpRequestLengthRequired, ErrorCode_HttpRequestBodySize, ErrorCode_HttpRequestMethodInvalid, ErrorCode_HttpRequestUriInvalid, ErrorCode_HttpRequestUriTooLong, ErrorCode_HttpRequestHeaderSectionSize, ErrorCode_HttpRequestHeaderSize, ErrorCode_HttpRequestTrailerSectionSize, ErrorCode_HttpRequestTrailerSize, ErrorCode_HttpResponseIncomplete, ErrorCode_HttpResponseHeaderSectionSize, ErrorCode_HttpResponseHeaderSize, ErrorCode_HttpResponseBodySize, ErrorCode_HttpResponseTrailerSectionSize, ErrorCode_HttpResponseTrailerSize, ErrorCode_HttpResponseTransferCoding, ErrorCode_HttpResponseContentCoding, ErrorCode_HttpResponseTimeout, ErrorCode_HttpUpgradeFailed, ErrorCode_HttpProtocolError, ErrorCode_LoopDetected, ErrorCode_ConfigurationError, ErrorCode_InternalError]
 """
 These cases are inspired by the IANA HTTP Proxy Error Types:
 https://www.iana.org/assignments/http-proxy-status/http-proxy-status.xhtml#table-http-proxy-error-types
 """
 
 
 
 @dataclass
-class HeaderErrorInvalidSyntax:
+class HeaderError_InvalidSyntax:
     pass
 
 
 @dataclass
-class HeaderErrorForbidden:
+class HeaderError_Forbidden:
     pass
 
 
 @dataclass
-class HeaderErrorImmutable:
+class HeaderError_Immutable:
     pass
 
 
-HeaderError = Union[HeaderErrorInvalidSyntax, HeaderErrorForbidden, HeaderErrorImmutable]
+HeaderError = Union[HeaderError_InvalidSyntax, HeaderError_Forbidden, HeaderError_Immutable]
 """
 This type enumerates the different kinds of errors that may occur when
 setting or appending to a `fields` resource.
 """
 
 
 class Fields:
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/imports/variables.py` & `spin-sdk-3.0.0/src/spin_sdk/wit/imports/variables.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from typing import TypeVar, Generic, Union, Optional, Union, Protocol, Tuple, List, Any, Self
+from typing import TypeVar, Generic, Union, Optional, Protocol, Tuple, List, Any, Self
 from enum import Flag, Enum, auto
 from dataclasses import dataclass
 from abc import abstractmethod
 import weakref
 
 from ..types import Result, Ok, Err, Some
 
 
 
 @dataclass
-class ErrorInvalidName:
+class Error_InvalidName:
     value: str
 
 
 @dataclass
-class ErrorUndefined:
+class Error_Undefined:
     value: str
 
 
 @dataclass
-class ErrorProvider:
+class Error_Provider:
     value: str
 
 
 @dataclass
-class ErrorOther:
+class Error_Other:
     value: str
 
 
-Error = Union[ErrorInvalidName, ErrorUndefined, ErrorProvider, ErrorOther]
+Error = Union[Error_InvalidName, Error_Undefined, Error_Provider, Error_Other]
 """
 The set of errors which may be raised by functions in this interface.
 """
 
 
 
 def get(name: str) -> str:
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/key-value.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/key-value.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/llm.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/llm.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/mysql.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/mysql.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/postgres.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/postgres.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/rdbms-types.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/rdbms-types.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/redis.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/redis.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/sqlite.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/sqlite.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk/wit/variables.wit` & `spin-sdk-3.0.0/src/spin_sdk/wit/variables.wit`

 * *Files identical despite different names*

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk.egg-info/PKG-INFO` & `spin-sdk-3.0.0/src/spin_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spin-sdk
-Version: 2.0.0rc2
+Version: 3.0.0
 Summary: Experimental SDK for Spin and Componentize-Py
 Author-email: Fermyon Engineering <engineering@fermyon.com>
 Maintainer-email: Fermyon Engineering <engineering@fermyon.com>
 License:                               Apache License
                                 Version 2.0, January 2004
                             http://www.apache.org/licenses/
         
@@ -230,38 +230,35 @@
 
 # Spin Python SDK
 
 This is an SDK for creating [Spin](https://github.com/fermyon/spin) apps using Python.
 
 Note that this SDK supersedes an earlier, experimental version, which may be
 found in the [old-sdk](https://github.com/fermyon/spin-python-sdk/tree/old-sdk)
-branch. _(The old template remains on `main` temporarily to preserve compatibility for some
-inbound links; it will be removed or replaced.)_
+branch.
 
 ## [API Documentation](https://fermyon.github.io/spin-python-sdk/index.html)
 
 ## Example
 
 ### Prerequisites
 
 - [Python 3.10 or later and pip](https://www.python.org/downloads/)
 - [componentize-py](https://pypi.org/project/componentize-py/)
 - [spin-sdk](https://pypi.org/project/spin-sdk/)
-- [MyPy](https://pypi.org/project/mypy/)
-    - This is optional, but useful for during development.
 - [Spin](https://github.com/fermyon/spin) 2.2 or later.
-    - As of this writing Spin 2.2 has not yet been released, so we must use the `main` branch of Spin for the time being. You can find pre-built binaries [here](https://github.com/fermyon/spin/releases/tag/canary).
+- [MyPy](https://pypi.org/project/mypy/) -- This is optional, but useful for during development.
 
 Once you have Python and pip installed, you can use the latter to create and
 enter a virtual environment and then install the desired packages
 
 ```shell
 python -m venv .venv
 source .venv/bin/activate
-pip install componentize-py==0.11.0 spin-sdk==2.0.0rc1 mypy==1.8.0
+pip install componentize-py==0.13.1 spin-sdk==3.0.0 mypy==1.8.0
 ```
 
 ### Hello, World
 
 A minimal app requires two files: a `spin.toml` and a Python script, which we'll
 name `app.py`:
 
@@ -283,18 +280,18 @@
 [component.hello.build]
 command = "componentize-py -w spin-http componentize app -o app.wasm"
 EOF
 ```
 
 ```shell
 cat >app.py <<EOF
-from spin_sdk.http import simple
-from spin_sdk.http.simple import Request, Response
+from spin_sdk import http
+from spin_sdk.http import Request, Response
 
-class IncomingHandler(simple.IncomingHandler):
+class IncomingHandler(http.IncomingHandler):
     def handle_request(self, request: Request) -> Response:
         return Response(
             200,
             {"content-type": "text/plain"},
             bytes("Hello from Python!", "utf-8")
         )
 EOF
```

### Comparing `spin-sdk-2.0.0rc2/src/spin_sdk.egg-info/SOURCES.txt` & `spin-sdk-3.0.0/src/spin_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 src/spin_sdk/__init__.py
 src/spin_sdk/componentize-py.toml
 src/spin_sdk/key_value.py
 src/spin_sdk/llm.py
+src/spin_sdk/mqtt.py
 src/spin_sdk/mysql.py
 src/spin_sdk/postgres.py
 src/spin_sdk/py.typed
 src/spin_sdk/redis.py
 src/spin_sdk/sqlite.py
 src/spin_sdk/variables.py
 src/spin_sdk.egg-info/PKG-INFO
@@ -17,14 +18,15 @@
 src/spin_sdk.egg-info/dependency_links.txt
 src/spin_sdk.egg-info/top_level.txt
 src/spin_sdk/http/__init__.py
 src/spin_sdk/http/poll_loop.py
 src/spin_sdk/wit/__init__.py
 src/spin_sdk/wit/key-value.wit
 src/spin_sdk/wit/llm.wit
+src/spin_sdk/wit/mqtt.wit
 src/spin_sdk/wit/mysql.wit
 src/spin_sdk/wit/postgres.wit
 src/spin_sdk/wit/rdbms-types.wit
 src/spin_sdk/wit/redis.wit
 src/spin_sdk/wit/spin.wit
 src/spin_sdk/wit/sqlite.wit
 src/spin_sdk/wit/types.py
@@ -67,14 +69,15 @@
 src/spin_sdk/wit/exports/inbound_redis.py
 src/spin_sdk/wit/exports/incoming_handler.py
 src/spin_sdk/wit/imports/__init__.py
 src/spin_sdk/wit/imports/error.py
 src/spin_sdk/wit/imports/key_value.py
 src/spin_sdk/wit/imports/llm.py
 src/spin_sdk/wit/imports/monotonic_clock.py
+src/spin_sdk/wit/imports/mqtt.py
 src/spin_sdk/wit/imports/mysql.py
 src/spin_sdk/wit/imports/outgoing_handler.py
 src/spin_sdk/wit/imports/poll.py
 src/spin_sdk/wit/imports/postgres.py
 src/spin_sdk/wit/imports/rdbms_types.py
 src/spin_sdk/wit/imports/redis.py
 src/spin_sdk/wit/imports/redis_types.py
```

