# Comparing `tmp/chainlib-eth-0.6.0.tar.gz` & `tmp/chainlib-eth-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlib-eth-0.6.0.tar", last modified: Tue Apr  2 11:11:37 2024, max compression
+gzip compressed data, was "chainlib-eth-0.6.1.tar", last modified: Wed Apr  3 14:06:56 2024, max compression
```

## Comparing `chainlib-eth-0.6.0.tar` & `chainlib-eth-0.6.1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.606249 chainlib-eth-0.6.0/
--rw-r--r--   0 lash      (1000) lash      (1000)     3710 2023-10-29 10:06:21.000000 chainlib-eth-0.6.0/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:13:49.000000 chainlib-eth-0.6.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      111 2023-06-03 11:38:52.000000 chainlib-eth-0.6.0/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)     2928 2024-04-02 11:11:37.606249 chainlib-eth-0.6.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1961 2023-06-03 11:38:17.000000 chainlib-eth-0.6.0/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      872 2022-11-14 07:16:48.000000 chainlib-eth-0.6.0/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:16:57.000000 chainlib-eth-0.6.0/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.596249 chainlib-eth-0.6.0/chainlib/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.599583 chainlib-eth-0.6.0/chainlib/eth/
--rw-r--r--   0 lash      (1000) lash      (1000)     1029 2022-02-27 09:47:47.000000 chainlib-eth-0.6.0/chainlib/eth/address.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4651 2024-04-02 10:34:52.000000 chainlib-eth-0.6.0/chainlib/eth/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      420 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.599583 chainlib-eth-0.6.0/chainlib/eth/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)       94 2021-10-18 11:32:11.000000 chainlib-eth-0.6.0/chainlib/eth/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      601 2023-02-07 06:18:34.000000 chainlib-eth-0.6.0/chainlib/eth/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1144 2023-02-12 08:11:49.000000 chainlib-eth-0.6.0/chainlib/eth/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)      515 2022-11-06 10:28:58.000000 chainlib-eth-0.6.0/chainlib/eth/cli/decode.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2801 2023-10-29 10:31:10.000000 chainlib-eth-0.6.0/chainlib/eth/cli/encode.py
--rw-r--r--   0 lash      (1000) lash      (1000)       41 2022-10-13 13:18:24.000000 chainlib-eth-0.6.0/chainlib/eth/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2512 2023-02-13 06:36:33.000000 chainlib-eth-0.6.0/chainlib/eth/cli/rpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)      629 2022-10-13 13:18:24.000000 chainlib-eth-0.6.0/chainlib/eth/cli/wallet.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7796 2021-12-21 14:52:18.000000 chainlib-eth-0.6.0/chainlib/eth/connection.py
--rw-r--r--   0 lash      (1000) lash      (1000)      248 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/constant.py
--rw-r--r--   0 lash      (1000) lash      (1000)    17638 2023-05-08 05:03:13.000000 chainlib-eth-0.6.0/chainlib/eth/contract.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.596249 chainlib-eth-0.6.0/chainlib/eth/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.599583 chainlib-eth-0.6.0/chainlib/eth/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)      291 2023-10-29 10:06:21.000000 chainlib-eth-0.6.0/chainlib/eth/data/config/config.ini
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.599583 chainlib-eth-0.6.0/chainlib/eth/dialect/
--rw-r--r--   0 lash      (1000) lash      (1000)      671 2023-10-29 10:06:21.000000 chainlib-eth-0.6.0/chainlib/eth/dialect/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      486 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/dialect/openethereum.py
--rw-r--r--   0 lash      (1000) lash      (1000)      578 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9041 2021-12-21 14:52:18.000000 chainlib-eth-0.6.0/chainlib/eth/gas.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-10 10:08:49.000000 chainlib-eth-0.6.0/chainlib/eth/jsonrpc.py
--rw-r--r--   0 lash      (1000) lash      (1000)      726 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3659 2022-10-13 13:18:24.000000 chainlib-eth-0.6.0/chainlib/eth/nonce.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.602916 chainlib-eth-0.6.0/chainlib/eth/pytest/
--rw-r--r--   0 lash      (1000) lash      (1000)       95 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/pytest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      296 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/pytest/fixtures_chain.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2535 2021-12-21 14:52:18.000000 chainlib-eth-0.6.0/chainlib/eth/pytest/fixtures_ethtester.py
--rw-r--r--   0 lash      (1000) lash      (1000)      310 2021-12-21 14:52:18.000000 chainlib-eth-0.6.0/chainlib/eth/pytest/fixtures_signer.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.602916 chainlib-eth-0.6.0/chainlib/eth/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2815 2022-11-04 07:29:23.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/balance.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4562 2023-10-29 10:06:21.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      694 2022-11-04 07:29:23.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/checksum.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2364 2022-11-04 07:29:23.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/count.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2367 2023-02-10 16:44:27.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/decode.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7307 2024-04-02 09:54:14.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/encode.py
--rw-r--r--   0 lash      (1000) lash      (1000)      996 2022-11-12 13:31:10.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/flags.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6095 2023-02-10 16:44:27.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/gas.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4730 2023-10-29 10:06:21.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/get.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5328 2023-03-01 22:45:39.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/info.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5572 2022-11-06 10:28:58.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/raw.py
--rw-r--r--   0 lash      (1000) lash      (1000)      303 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/subscribe.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4102 2022-11-06 10:28:58.000000 chainlib-eth-0.6.0/chainlib/eth/runnable/wait.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5717 2023-06-03 06:59:28.000000 chainlib-eth-0.6.0/chainlib/eth/settings.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1833 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/chainlib/eth/sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1209 2022-11-04 07:29:23.000000 chainlib-eth-0.6.0/chainlib/eth/src.py
--rw-r--r--   0 lash      (1000) lash      (1000)    25912 2023-10-29 10:06:21.000000 chainlib-eth-0.6.0/chainlib/eth/tx.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.602916 chainlib-eth-0.6.0/chainlib/eth/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)     6361 2021-12-21 14:52:18.000000 chainlib-eth-0.6.0/chainlib/eth/unittest/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2705 2023-05-13 09:04:30.000000 chainlib-eth-0.6.0/chainlib/eth/unittest/ethtester.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.606249 chainlib-eth-0.6.0/chainlib_eth.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)     2928 2024-04-02 11:11:37.000000 chainlib-eth-0.6.0/chainlib_eth.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     2029 2024-04-02 11:11:37.000000 chainlib-eth-0.6.0/chainlib_eth.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-02 11:11:37.000000 chainlib-eth-0.6.0/chainlib_eth.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      556 2024-04-02 11:11:37.000000 chainlib-eth-0.6.0/chainlib_eth.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      109 2024-04-02 11:11:37.000000 chainlib-eth-0.6.0/chainlib_eth.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        9 2024-04-02 11:11:37.000000 chainlib-eth-0.6.0/chainlib_eth.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.599583 chainlib-eth-0.6.0/man/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.602916 chainlib-eth-0.6.0/man/build/
--rw-r--r--   0 lash      (1000) lash      (1000)     3349 2023-05-08 06:23:52.000000 chainlib-eth-0.6.0/man/build/eth-balance.1
--rw-r--r--   0 lash      (1000) lash      (1000)     4585 2023-05-08 06:23:50.000000 chainlib-eth-0.6.0/man/build/eth-count.1
--rw-r--r--   0 lash      (1000) lash      (1000)     4012 2023-05-08 06:23:50.000000 chainlib-eth-0.6.0/man/build/eth-decode.1
--rw-r--r--   0 lash      (1000) lash      (1000)     9745 2023-05-08 06:23:50.000000 chainlib-eth-0.6.0/man/build/eth-encode.1
--rw-r--r--   0 lash      (1000) lash      (1000)    11012 2023-05-08 06:23:49.000000 chainlib-eth-0.6.0/man/build/eth-gas.1
--rw-r--r--   0 lash      (1000) lash      (1000)     4333 2023-05-08 06:23:49.000000 chainlib-eth-0.6.0/man/build/eth-get.1
--rw-r--r--   0 lash      (1000) lash      (1000)     4230 2023-05-08 06:23:49.000000 chainlib-eth-0.6.0/man/build/eth-info.1
--rw-r--r--   0 lash      (1000) lash      (1000)     7965 2023-05-08 06:23:51.000000 chainlib-eth-0.6.0/man/build/eth-raw.1
--rw-r--r--   0 lash      (1000) lash      (1000)     5024 2023-05-08 06:23:51.000000 chainlib-eth-0.6.0/man/build/eth-wait.1
--rw-r--r--   0 lash      (1000) lash      (1000)      109 2024-04-02 11:09:37.000000 chainlib-eth-0.6.0/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1463 2024-04-02 11:11:37.606249 chainlib-eth-0.6.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      974 2023-06-03 12:08:30.000000 chainlib-eth-0.6.0/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       63 2024-04-02 10:12:01.000000 chainlib-eth-0.6.0/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:11:37.606249 chainlib-eth-0.6.0/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     7080 2023-03-29 08:49:49.000000 chainlib-eth-0.6.0/tests/test_abi.py
--rw-r--r--   0 lash      (1000) lash      (1000)      978 2022-05-04 18:10:33.000000 chainlib-eth-0.6.0/tests/test_address.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2244 2023-02-03 09:18:31.000000 chainlib-eth-0.6.0/tests/test_block.py
--rw-r--r--   0 lash      (1000) lash      (1000)     8184 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/tests/test_bloom.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1196 2022-10-13 13:18:24.000000 chainlib-eth-0.6.0/tests/test_cli.py
--rw-r--r--   0 lash      (1000) lash      (1000)      896 2023-03-29 09:08:32.000000 chainlib-eth-0.6.0/tests/test_event.py
--rw-r--r--   0 lash      (1000) lash      (1000)      620 2021-10-10 10:18:45.000000 chainlib-eth-0.6.0/tests/test_nonce.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3466 2021-12-21 14:52:18.000000 chainlib-eth-0.6.0/tests/test_sign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1607 2022-10-13 13:18:24.000000 chainlib-eth-0.6.0/tests/test_stat.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6621 2022-10-13 13:18:24.000000 chainlib-eth-0.6.0/tests/test_tx.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.959953 chainlib-eth-0.6.1/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3710 2023-10-29 10:06:21.000000 chainlib-eth-0.6.1/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:13:49.000000 chainlib-eth-0.6.1/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      111 2023-06-03 11:38:52.000000 chainlib-eth-0.6.1/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)     2928 2024-04-03 14:06:56.959953 chainlib-eth-0.6.1/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1961 2023-06-03 11:38:17.000000 chainlib-eth-0.6.1/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      872 2022-11-14 07:16:48.000000 chainlib-eth-0.6.1/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:16:57.000000 chainlib-eth-0.6.1/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.953287 chainlib-eth-0.6.1/chainlib/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.956620 chainlib-eth-0.6.1/chainlib/eth/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1029 2022-02-27 09:47:47.000000 chainlib-eth-0.6.1/chainlib/eth/address.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4851 2024-04-03 14:03:40.000000 chainlib-eth-0.6.1/chainlib/eth/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      420 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.956620 chainlib-eth-0.6.1/chainlib/eth/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)       94 2021-10-18 11:32:11.000000 chainlib-eth-0.6.1/chainlib/eth/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      601 2023-02-07 06:18:34.000000 chainlib-eth-0.6.1/chainlib/eth/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1144 2023-02-12 08:11:49.000000 chainlib-eth-0.6.1/chainlib/eth/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      515 2022-11-06 10:28:58.000000 chainlib-eth-0.6.1/chainlib/eth/cli/decode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2801 2023-10-29 10:31:10.000000 chainlib-eth-0.6.1/chainlib/eth/cli/encode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       41 2022-10-13 13:18:24.000000 chainlib-eth-0.6.1/chainlib/eth/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2512 2023-02-13 06:36:33.000000 chainlib-eth-0.6.1/chainlib/eth/cli/rpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      629 2022-10-13 13:18:24.000000 chainlib-eth-0.6.1/chainlib/eth/cli/wallet.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7796 2021-12-21 14:52:18.000000 chainlib-eth-0.6.1/chainlib/eth/connection.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      248 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/constant.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    17638 2023-05-08 05:03:13.000000 chainlib-eth-0.6.1/chainlib/eth/contract.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.953287 chainlib-eth-0.6.1/chainlib/eth/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.956620 chainlib-eth-0.6.1/chainlib/eth/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)      291 2023-10-29 10:06:21.000000 chainlib-eth-0.6.1/chainlib/eth/data/config/config.ini
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.956620 chainlib-eth-0.6.1/chainlib/eth/dialect/
+-rw-r--r--   0 lash      (1000) lash      (1000)      671 2023-10-29 10:06:21.000000 chainlib-eth-0.6.1/chainlib/eth/dialect/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      486 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/dialect/openethereum.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      578 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9041 2021-12-21 14:52:18.000000 chainlib-eth-0.6.1/chainlib/eth/gas.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2080 2022-12-10 10:08:49.000000 chainlib-eth-0.6.1/chainlib/eth/jsonrpc.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      726 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3659 2022-10-13 13:18:24.000000 chainlib-eth-0.6.1/chainlib/eth/nonce.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.956620 chainlib-eth-0.6.1/chainlib/eth/pytest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       95 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/pytest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      296 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/pytest/fixtures_chain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2535 2021-12-21 14:52:18.000000 chainlib-eth-0.6.1/chainlib/eth/pytest/fixtures_ethtester.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      310 2021-12-21 14:52:18.000000 chainlib-eth-0.6.1/chainlib/eth/pytest/fixtures_signer.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.956620 chainlib-eth-0.6.1/chainlib/eth/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2815 2022-11-04 07:29:23.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/balance.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4562 2024-04-03 13:58:08.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      694 2022-11-04 07:29:23.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/checksum.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2364 2022-11-04 07:29:23.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/count.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2367 2023-02-10 16:44:27.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/decode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7307 2024-04-02 09:54:14.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/encode.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      996 2022-11-12 13:31:10.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/flags.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6095 2023-02-10 16:44:27.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/gas.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4730 2023-10-29 10:06:21.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/get.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5328 2023-03-01 22:45:39.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/info.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5572 2022-11-06 10:28:58.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/raw.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      303 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/subscribe.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4102 2022-11-06 10:28:58.000000 chainlib-eth-0.6.1/chainlib/eth/runnable/wait.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5717 2023-06-03 06:59:28.000000 chainlib-eth-0.6.1/chainlib/eth/settings.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1833 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/chainlib/eth/sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1209 2022-11-04 07:29:23.000000 chainlib-eth-0.6.1/chainlib/eth/src.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    25912 2024-04-03 13:54:32.000000 chainlib-eth-0.6.1/chainlib/eth/tx.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.956620 chainlib-eth-0.6.1/chainlib/eth/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)     6361 2021-12-21 14:52:18.000000 chainlib-eth-0.6.1/chainlib/eth/unittest/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2705 2023-05-13 09:04:30.000000 chainlib-eth-0.6.1/chainlib/eth/unittest/ethtester.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.959953 chainlib-eth-0.6.1/chainlib_eth.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2928 2024-04-03 14:06:56.000000 chainlib-eth-0.6.1/chainlib_eth.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     2029 2024-04-03 14:06:56.000000 chainlib-eth-0.6.1/chainlib_eth.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-03 14:06:56.000000 chainlib-eth-0.6.1/chainlib_eth.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      556 2024-04-03 14:06:56.000000 chainlib-eth-0.6.1/chainlib_eth.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      109 2024-04-03 14:06:56.000000 chainlib-eth-0.6.1/chainlib_eth.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        9 2024-04-03 14:06:56.000000 chainlib-eth-0.6.1/chainlib_eth.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.953287 chainlib-eth-0.6.1/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.956620 chainlib-eth-0.6.1/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3349 2023-05-08 06:23:52.000000 chainlib-eth-0.6.1/man/build/eth-balance.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     4585 2023-05-08 06:23:50.000000 chainlib-eth-0.6.1/man/build/eth-count.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     4012 2023-05-08 06:23:50.000000 chainlib-eth-0.6.1/man/build/eth-decode.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     9745 2023-05-08 06:23:50.000000 chainlib-eth-0.6.1/man/build/eth-encode.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    11012 2023-05-08 06:23:49.000000 chainlib-eth-0.6.1/man/build/eth-gas.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     4333 2023-05-08 06:23:49.000000 chainlib-eth-0.6.1/man/build/eth-get.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     4230 2023-05-08 06:23:49.000000 chainlib-eth-0.6.1/man/build/eth-info.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     7965 2023-05-08 06:23:51.000000 chainlib-eth-0.6.1/man/build/eth-raw.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     5024 2023-05-08 06:23:51.000000 chainlib-eth-0.6.1/man/build/eth-wait.1
+-rw-r--r--   0 lash      (1000) lash      (1000)      109 2024-04-02 11:19:36.000000 chainlib-eth-0.6.1/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1463 2024-04-03 14:06:56.959953 chainlib-eth-0.6.1/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      974 2023-06-03 12:08:30.000000 chainlib-eth-0.6.1/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       63 2024-04-02 11:19:36.000000 chainlib-eth-0.6.1/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-03 14:06:56.959953 chainlib-eth-0.6.1/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     7080 2023-03-29 08:49:49.000000 chainlib-eth-0.6.1/tests/test_abi.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      978 2022-05-04 18:10:33.000000 chainlib-eth-0.6.1/tests/test_address.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2244 2023-02-03 09:18:31.000000 chainlib-eth-0.6.1/tests/test_block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     8184 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/tests/test_bloom.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1196 2022-10-13 13:18:24.000000 chainlib-eth-0.6.1/tests/test_cli.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      896 2023-03-29 09:08:32.000000 chainlib-eth-0.6.1/tests/test_event.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      620 2021-10-10 10:18:45.000000 chainlib-eth-0.6.1/tests/test_nonce.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3466 2021-12-21 14:52:18.000000 chainlib-eth-0.6.1/tests/test_sign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1607 2022-10-13 13:18:24.000000 chainlib-eth-0.6.1/tests/test_stat.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6621 2022-10-13 13:18:24.000000 chainlib-eth-0.6.1/tests/test_tx.py
```

### Comparing `chainlib-eth-0.6.0/CHANGELOG` & `chainlib-eth-0.6.1/CHANGELOG`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/LICENSE` & `chainlib-eth-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/PKG-INFO` & `chainlib-eth-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlib-eth
-Version: 0.6.0
+Version: 0.6.1
 Summary: Ethereum implementation of the chainlib interface
 Home-page: https://git.defalslfy.org/chainlib-eth
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainlib-eth-0.6.0/README.md` & `chainlib-eth-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/WAIVER` & `chainlib-eth-0.6.1/WAIVER`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/WAIVER.asc` & `chainlib-eth-0.6.1/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/address.py` & `chainlib-eth-0.6.1/chainlib/eth/address.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/block.py` & `chainlib-eth-0.6.1/chainlib/eth/block.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,24 @@
             i += 1
         if idx == -1:
             raise AttributeError('tx {} not found in block {}'.format(tx_hash, self.hash))
         return idx
 
 
     def to_human(self):
+        try:
+            self.fee_limit = hex_to_int(self.fee_limit)
+        except TypeError:
+            pass
+
+        try:
+            self.fee_cost = hex_to_int(self.fee_cost)
+        except TypeError:
+            pass
+
         s = """hash: {}
 number: {}
 parent: {}
 timestamp: {}
 time: {}
 author: {}
 gas_limit: {}
@@ -172,14 +182,14 @@
 """.format(
     self.hash,
     self.number,
     self.parent_hash,
     self.timestamp,
     datetime.datetime.fromtimestamp(self.timestamp),
     self.author,
-    hex_to_int(self.fee_limit),
-    hex_to_int(self.fee_cost),
+    self.fee_limit,
+    self.fee_cost,
     len(self.txs),
         )
 
         return s
```

### Comparing `chainlib-eth-0.6.0/chainlib/eth/cli/arg.py` & `chainlib-eth-0.6.1/chainlib/eth/cli/arg.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/cli/config.py` & `chainlib-eth-0.6.1/chainlib/eth/cli/config.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/cli/decode.py` & `chainlib-eth-0.6.1/chainlib/eth/cli/decode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/cli/encode.py` & `chainlib-eth-0.6.1/chainlib/eth/cli/encode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/cli/rpc.py` & `chainlib-eth-0.6.1/chainlib/eth/cli/rpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/cli/wallet.py` & `chainlib-eth-0.6.1/chainlib/eth/cli/wallet.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/connection.py` & `chainlib-eth-0.6.1/chainlib/eth/connection.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/contract.py` & `chainlib-eth-0.6.1/chainlib/eth/contract.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/dialect/__init__.py` & `chainlib-eth-0.6.1/chainlib/eth/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/error.py` & `chainlib-eth-0.6.1/chainlib/eth/error.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/gas.py` & `chainlib-eth-0.6.1/chainlib/eth/gas.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/jsonrpc.py` & `chainlib-eth-0.6.1/chainlib/eth/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/log.py` & `chainlib-eth-0.6.1/chainlib/eth/log.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/nonce.py` & `chainlib-eth-0.6.1/chainlib/eth/nonce.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/pytest/fixtures_ethtester.py` & `chainlib-eth-0.6.1/chainlib/eth/pytest/fixtures_ethtester.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/balance.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/balance.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/block.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/block.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/checksum.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/checksum.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/count.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/count.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/decode.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/decode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/encode.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/encode.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/flags.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/flags.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/gas.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/gas.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/get.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/get.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/info.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/info.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/raw.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/raw.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/runnable/wait.py` & `chainlib-eth-0.6.1/chainlib/eth/runnable/wait.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/settings.py` & `chainlib-eth-0.6.1/chainlib/eth/settings.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/sign.py` & `chainlib-eth-0.6.1/chainlib/eth/sign.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/src.py` & `chainlib-eth-0.6.1/chainlib/eth/src.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/tx.py` & `chainlib-eth-0.6.1/chainlib/eth/tx.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/unittest/base.py` & `chainlib-eth-0.6.1/chainlib/eth/unittest/base.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib/eth/unittest/ethtester.py` & `chainlib-eth-0.6.1/chainlib/eth/unittest/ethtester.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib_eth.egg-info/PKG-INFO` & `chainlib-eth-0.6.1/chainlib_eth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlib-eth
-Version: 0.6.0
+Version: 0.6.1
 Summary: Ethereum implementation of the chainlib interface
 Home-page: https://git.defalslfy.org/chainlib-eth
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `chainlib-eth-0.6.0/chainlib_eth.egg-info/SOURCES.txt` & `chainlib-eth-0.6.1/chainlib_eth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/chainlib_eth.egg-info/entry_points.txt` & `chainlib-eth-0.6.1/chainlib_eth.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-balance.1` & `chainlib-eth-0.6.1/man/build/eth-balance.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-count.1` & `chainlib-eth-0.6.1/man/build/eth-count.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-decode.1` & `chainlib-eth-0.6.1/man/build/eth-decode.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-encode.1` & `chainlib-eth-0.6.1/man/build/eth-encode.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-gas.1` & `chainlib-eth-0.6.1/man/build/eth-gas.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-get.1` & `chainlib-eth-0.6.1/man/build/eth-get.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-info.1` & `chainlib-eth-0.6.1/man/build/eth-info.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-raw.1` & `chainlib-eth-0.6.1/man/build/eth-raw.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/man/build/eth-wait.1` & `chainlib-eth-0.6.1/man/build/eth-wait.1`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/setup.cfg` & `chainlib-eth-0.6.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = chainlib-eth
-version = 0.6.0
+version = 0.6.1
 description = Ethereum implementation of the chainlib interface
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalslfy.org/chainlib-eth
 keywords = 
 	dlt
 	blockchain
```

### Comparing `chainlib-eth-0.6.0/setup.py` & `chainlib-eth-0.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_abi.py` & `chainlib-eth-0.6.1/tests/test_abi.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_address.py` & `chainlib-eth-0.6.1/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_block.py` & `chainlib-eth-0.6.1/tests/test_block.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_bloom.py` & `chainlib-eth-0.6.1/tests/test_bloom.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_cli.py` & `chainlib-eth-0.6.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_event.py` & `chainlib-eth-0.6.1/tests/test_event.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_nonce.py` & `chainlib-eth-0.6.1/tests/test_nonce.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_sign.py` & `chainlib-eth-0.6.1/tests/test_sign.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_stat.py` & `chainlib-eth-0.6.1/tests/test_stat.py`

 * *Files identical despite different names*

### Comparing `chainlib-eth-0.6.0/tests/test_tx.py` & `chainlib-eth-0.6.1/tests/test_tx.py`

 * *Files identical despite different names*

