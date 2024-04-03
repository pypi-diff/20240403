# Comparing `tmp/aesir-0.4.0.tar.gz` & `tmp/aesir-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aesir-0.4.0.tar", max compression
+gzip compressed data, was "aesir-0.4.1.tar", max compression
```

## Comparing `aesir-0.4.0.tar` & `aesir-0.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1078 2023-11-30 23:46:55.435688 aesir-0.4.0/LICENSE
--rw-r--r--   0        0        0    11531 2024-02-29 08:21:34.054800 aesir-0.4.0/README.md
--rw-r--r--   0        0        0     2226 2024-02-29 08:20:26.711478 aesir-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1025 2024-02-29 08:20:17.173695 aesir-0.4.0/src/aesir/__init__.py
--rw-r--r--   0        0        0      849 2024-02-29 08:20:17.173733 aesir-0.4.0/src/aesir/commands/__init__.py
--rw-r--r--   0        0        0     2692 2024-02-29 08:20:17.214476 aesir-0.4.0/src/aesir/commands/build.py
--rw-r--r--   0        0        0     1835 2024-02-29 08:20:17.173678 aesir-0.4.0/src/aesir/commands/clean.py
--rw-r--r--   0        0        0     6981 2024-02-29 08:20:17.173705 aesir-0.4.0/src/aesir/commands/deploy.py
--rw-r--r--   0        0        0     1334 2024-02-29 08:20:17.173647 aesir-0.4.0/src/aesir/commands/flush.py
--rw-r--r--   0        0        0     5920 2024-02-29 08:20:17.174398 aesir-0.4.0/src/aesir/commands/mine.py
--rw-r--r--   0        0        0     1804 2024-02-29 08:20:17.173656 aesir-0.4.0/src/aesir/commands/nodekeys.py
--rw-r--r--   0        0        0     4811 2024-02-29 08:20:17.173670 aesir-0.4.0/src/aesir/commands/ping_pong.py
--rw-r--r--   0        0        0     2475 2024-02-29 08:20:17.173687 aesir-0.4.0/src/aesir/commands/pull.py
--rw-r--r--   0        0        0     1728 2024-02-29 08:20:17.173638 aesir-0.4.0/src/aesir/configs.py
--rw-r--r--   0        0        0      849 2024-02-29 08:20:17.173623 aesir-0.4.0/src/aesir/core.py
--rw-r--r--   0        0        0     8770 2024-02-29 08:07:05.474286 aesir-0.4.0/src/aesir/schemas.yml
--rw-r--r--   0        0        0     1152 2024-02-29 08:20:17.217943 aesir-0.4.0/src/aesir/types/__init__.py
--rw-r--r--   0        0        0      584 2024-02-29 08:20:17.218095 aesir-0.4.0/src/aesir/types/blockchain_info.py
--rw-r--r--   0        0        0      657 2024-02-29 08:20:17.218136 aesir-0.4.0/src/aesir/types/build.py
--rw-r--r--   0        0        0      474 2024-02-29 08:20:17.218170 aesir-0.4.0/src/aesir/types/cluster_enum.py
--rw-r--r--   0        0        0      581 2024-02-29 08:20:17.173722 aesir-0.4.0/src/aesir/types/image.py
--rw-r--r--   0        0        0      633 2024-02-29 08:20:17.218041 aesir-0.4.0/src/aesir/types/lnd_info.py
--rw-r--r--   0        0        0     1463 2024-02-29 08:20:17.173749 aesir-0.4.0/src/aesir/types/mutex_option.py
--rw-r--r--   0        0        0      499 2024-02-29 08:20:17.173714 aesir-0.4.0/src/aesir/types/new_address.py
--rw-r--r--   0        0        0      507 2024-02-29 08:20:17.173742 aesir-0.4.0/src/aesir/types/open_channel.py
--rw-r--r--   0        0        0      523 2024-02-29 08:20:17.217927 aesir-0.4.0/src/aesir/types/peripheral_enum.py
--rw-r--r--   0        0        0      911 2024-02-29 08:20:17.218006 aesir-0.4.0/src/aesir/types/service.py
--rw-r--r--   0        0        0    13351 1970-01-01 00:00:00.000000 aesir-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-11-30 23:46:55.435688 aesir-0.4.1/LICENSE
+-rw-r--r--   0        0        0    11639 2024-04-03 08:15:27.643829 aesir-0.4.1/README.md
+-rw-r--r--   0        0        0     2226 2024-04-03 08:15:06.612241 aesir-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1025 2024-04-03 08:15:00.233412 aesir-0.4.1/src/aesir/__init__.py
+-rw-r--r--   0        0        0      849 2024-04-03 08:15:00.237568 aesir-0.4.1/src/aesir/commands/__init__.py
+-rw-r--r--   0        0        0     2692 2024-04-03 08:15:00.248245 aesir-0.4.1/src/aesir/commands/build.py
+-rw-r--r--   0        0        0     1835 2024-04-03 08:15:00.243176 aesir-0.4.1/src/aesir/commands/clean.py
+-rw-r--r--   0        0        0     6981 2024-04-03 08:15:00.256654 aesir-0.4.1/src/aesir/commands/deploy.py
+-rw-r--r--   0        0        0     1334 2024-04-03 08:15:00.227278 aesir-0.4.1/src/aesir/commands/flush.py
+-rw-r--r--   0        0        0     5920 2024-04-03 08:15:00.256923 aesir-0.4.1/src/aesir/commands/mine.py
+-rw-r--r--   0        0        0     1804 2024-04-03 08:15:00.226990 aesir-0.4.1/src/aesir/commands/nodekeys.py
+-rw-r--r--   0        0        0     4811 2024-04-03 08:15:00.237834 aesir-0.4.1/src/aesir/commands/ping_pong.py
+-rw-r--r--   0        0        0     2475 2024-04-03 08:15:00.248313 aesir-0.4.1/src/aesir/commands/pull.py
+-rw-r--r--   0        0        0     1728 2024-04-03 08:15:00.227155 aesir-0.4.1/src/aesir/configs.py
+-rw-r--r--   0        0        0      849 2024-04-03 08:15:00.233307 aesir-0.4.1/src/aesir/core.py
+-rw-r--r--   0        0        0     8770 2024-04-03 08:14:08.893090 aesir-0.4.1/src/aesir/schemas.yml
+-rw-r--r--   0        0        0     1152 2024-04-03 08:15:00.256706 aesir-0.4.1/src/aesir/types/__init__.py
+-rw-r--r--   0        0        0      584 2024-04-03 08:15:00.256737 aesir-0.4.1/src/aesir/types/blockchain_info.py
+-rw-r--r--   0        0        0      657 2024-04-03 08:15:00.256759 aesir-0.4.1/src/aesir/types/build.py
+-rw-r--r--   0        0        0      474 2024-04-03 08:15:00.256677 aesir-0.4.1/src/aesir/types/cluster_enum.py
+-rw-r--r--   0        0        0      581 2024-04-03 08:15:00.251470 aesir-0.4.1/src/aesir/types/image.py
+-rw-r--r--   0        0        0      633 2024-04-03 08:15:00.256800 aesir-0.4.1/src/aesir/types/lnd_info.py
+-rw-r--r--   0        0        0     1463 2024-04-03 08:15:00.256599 aesir-0.4.1/src/aesir/types/mutex_option.py
+-rw-r--r--   0        0        0      499 2024-04-03 08:15:00.248379 aesir-0.4.1/src/aesir/types/new_address.py
+-rw-r--r--   0        0        0      507 2024-04-03 08:15:00.248352 aesir-0.4.1/src/aesir/types/open_channel.py
+-rw-r--r--   0        0        0      523 2024-04-03 08:15:00.256692 aesir-0.4.1/src/aesir/types/peripheral_enum.py
+-rw-r--r--   0        0        0      911 2024-04-03 08:15:00.256718 aesir-0.4.1/src/aesir/types/service.py
+-rw-r--r--   0        0        0    13459 1970-01-01 00:00:00.000000 aesir-0.4.1/PKG-INFO
```

### Comparing `aesir-0.4.0/LICENSE` & `aesir-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aesir-0.4.0/README.md` & `aesir-0.4.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,16 @@
 ### Cluster types
 
 Currently there are two supported cluster-types in this project. Specified by flags,
 `--duo` (default), or `--uno` with the following set-up:
 
 | Type | Description                                                                |
 | ---- | -------------------------------------------------------------------------- |
-|  duo | Contains two LND nodes named `aesir-ping` and `aesir-pong` unified by <br> one single `aesir-bitcoind` service. 
+|  duo | Contains two LND nodes named `aesir-ping` and `aesir-pong` unified by <br> one single `aesir-bitcoind` service. |
+|  ohm | Only has `aesir-bitcoind` without any Lightning nodes. |
 |  uno | Only has one LND node named `aesir-lnd` connected to `aesir-bitcoind`. |
 
 ### Peripheral containers
 
 This project also helps you setup peripheral services to make development process easier, too.
 For example, if you want to deploy a duo-cluster with attached postgres database, run the following:
 
@@ -141,14 +142,15 @@
 * **0.3.4** Simplify deployment workflows and 
 * **0.3.5** Restructure project so that when installed, `src` folder will not be created
 * **0.3.6** Breakdown "setup" command into "build" and "pull"
 * **0.3.7** Lightning cluster now with [ord](https://github.com/ordinals/ord)
 * **0.3.8** Rename "ord" to "ord-server" to avoid confusion with cli
 * **0.3.9** Remove intermediate containers
 * **0.4.0** Resist electricity with "ohm" mode
+* **0.4.1** Remove Ordinals' spiked ball
 
 ## Roadmap
 
 * Make image versioning a little bit more intuitive.
 * Add `aesir-tesla-ball` peripheral service using [tesla-ball](https://github.com/krutt/tesla-ball)
 * Write [click](https://click.palletsprojects.com) tests.
 * Use [joblib](https://github.com/joblib/joblib) to speed up deployment with parallelization.
@@ -176,15 +178,15 @@
 > Package operations: 33 installs, 0 updates, 0 removals
 >
 >   • ...
 >   • ...
 >   • ...
 >   • ...
 >
-> Installing the current project: aesir (0.4.0)
+> Installing the current project: aesir (0.4.1)
 ```
 
 ### Known issues
 
 You may run into this setback when first running this project. This is a
 [docker-py](https://github.com/docker/docker-py/issues/3059) issue widely known as of October 2022.
```

### Comparing `aesir-0.4.0/pyproject.toml` & `aesir-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 ]
 keywords = ['anonymous', 'bitcoin', 'cashu', 'chaum', 'chaumian', 'cli', 'ecash', 'lightning']
 license = 'MIT'
 name = 'aesir'
 packages = [{from='src', include='aesir'}]
 readme = 'README.md'
 repository = 'https://github.com/krutt/aesir'
-version = '0.4.0'
+version = '0.4.1'
 
 
 [tool.poetry.dependencies]
 APScheduler = '^3.10.4'
 click = '^8.1.7'
 docker = '^6.1.3'
 pydantic = '^2.5.2'
```

### Comparing `aesir-0.4.0/src/aesir/__init__.py` & `aesir-0.4.1/src/aesir/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/__init__.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION: https://www.w3docs.com/snippets/python/what-is-init-py-for.html
 #
 # HISTORY:
 # *************************************************************
 
@@ -47,8 +47,8 @@
   "flush",
   "mine",
   "nodekeys",
   "ping_pong",
   "pull",
 ]
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
```

### Comparing `aesir-0.4.0/src/aesir/commands/__init__.py` & `aesir-0.4.1/src/aesir/commands/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/__init__.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION: https://www.w3docs.com/snippets/python/what-is-init-py-for.html
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/commands/build.py` & `aesir-0.4.1/src/aesir/commands/build.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/build.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2024-02-27 23:52
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/commands/clean.py` & `aesir-0.4.1/src/aesir/commands/clean.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/clean.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/commands/deploy.py` & `aesir-0.4.1/src/aesir/commands/deploy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/deploy.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/commands/flush.py` & `aesir-0.4.1/src/aesir/commands/flush.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/flush.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 06:24
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/commands/mine.py` & `aesir-0.4.1/src/aesir/commands/mine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/mine.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR:      Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/commands/nodekeys.py` & `aesir-0.4.1/src/aesir/commands/nodekeys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/nodekeys.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/commands/ping_pong.py` & `aesir-0.4.1/src/aesir/commands/ping_pong.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/ping_pong.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 06:18
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/commands/pull.py` & `aesir-0.4.1/src/aesir/commands/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/commands/pull.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 06:18
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/configs.py` & `aesir-0.4.1/src/aesir/configs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/configs.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/core.py` & `aesir-0.4.1/src/aesir/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/core.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 02:20
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/schemas.yml` & `aesir-0.4.1/src/aesir/schemas.yml`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         - -server=1
         - -regtest=1
         - -rpcauth=aesir:0a17eed40accdd0f2271a548547ec9bb$b269b686f2ad7ccf0b5ea3450e0687dc1a90846d3828811ad0d570de83b65f4c
         - -debug=1
         - -zmqpubrawblock=tcp://0.0.0.0:28334
         - -zmqpubrawtx=tcp://0.0.0.0:28335
         - -zmqpubhashblock=tcp://0.0.0.0:28336
-        - -txindex=0
+        - -txindex=1
         - -dnsseed=0
         - -upnp=0
         - -rpcbind=0.0.0.0
         - -rpcallowip=0.0.0.0/0
         - -rpcport=18443
         - -rpcworkqueue=128
         - -rest
@@ -133,15 +133,15 @@
         - -server=1
         - -regtest=1
         - -rpcauth=aesir:0a17eed40accdd0f2271a548547ec9bb$b269b686f2ad7ccf0b5ea3450e0687dc1a90846d3828811ad0d570de83b65f4c
         - -debug=1
         - -zmqpubrawblock=tcp://0.0.0.0:28334
         - -zmqpubrawtx=tcp://0.0.0.0:28335
         - -zmqpubhashblock=tcp://0.0.0.0:28336
-        - -txindex=0
+        - -txindex=1
         - -dnsseed=0
         - -upnp=0
         - -rpcbind=0.0.0.0
         - -rpcallowip=0.0.0.0/0
         - -rpcport=18443
         - -rpcworkqueue=128
         - -rest
@@ -163,15 +163,15 @@
         - -server=1
         - -regtest=1
         - -rpcauth=aesir:0a17eed40accdd0f2271a548547ec9bb$b269b686f2ad7ccf0b5ea3450e0687dc1a90846d3828811ad0d570de83b65f4c
         - -debug=1
         - -zmqpubrawblock=tcp://0.0.0.0:28334
         - -zmqpubrawtx=tcp://0.0.0.0:28335
         - -zmqpubhashblock=tcp://0.0.0.0:28336
-        - -txindex=0
+        - -txindex=1
         - -dnsseed=0
         - -upnp=0
         - -rpcbind=0.0.0.0
         - -rpcallowip=0.0.0.0/0
         - -rpcport=18443
         - -rpcworkqueue=128
         - -rest
```

### Comparing `aesir-0.4.0/src/aesir/types/__init__.py` & `aesir-0.4.1/src/aesir/types/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/types/__init__.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION: https://www.w3docs.com/snippets/python/what-is-init-py-for.html
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/types/blockchain_info.py` & `aesir-0.4.1/src/aesir/types/blockchain_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/types/blockchain_info.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/types/build.py` & `aesir-0.4.1/src/aesir/types/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/types/build_enum.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-06 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/types/image.py` & `aesir-0.4.1/src/aesir/types/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/types/image.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/types/lnd_info.py` & `aesir-0.4.1/src/aesir/types/lnd_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/types/lnd_info.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/types/mutex_option.py` & `aesir-0.4.1/src/aesir/types/mutex_option.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/types/mutex_option.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/types/peripheral_enum.py` & `aesir-0.4.1/src/aesir/types/peripheral_enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/types/peripheral_enum.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-03 01:11
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/src/aesir/types/service.py` & `aesir-0.4.1/src/aesir/types/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3.8
 # coding:utf-8
 # Copyright (C) 2022-2024 All rights reserved.
 # FILENAME:    ~~/src/aesir/types/service.py
-# VERSION: 	   0.4.0
+# VERSION: 	   0.4.1
 # CREATED: 	   2023-12-01 05:31
 # AUTHOR: 	   Sitt Guruvanich <aekasitt.g+github@siamintech.co.th>
 # DESCRIPTION:
 #
 # HISTORY:
 # *************************************************************
```

### Comparing `aesir-0.4.0/PKG-INFO` & `aesir-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aesir
-Version: 0.4.0
+Version: 0.4.1
 Summary: Command line interface used for generating local Lightning test environment
 Home-page: https://github.com/krutt/aesir
 License: MIT
 Keywords: anonymous,bitcoin,cashu,chaum,chaumian,cli,ecash,lightning
 Author: Sitt Guruvanich
 Author-email: aekasitt.g+github@siamintech.co.th
 Requires-Python: >=3.8,<4.0
@@ -122,15 +122,16 @@
 ### Cluster types
 
 Currently there are two supported cluster-types in this project. Specified by flags,
 `--duo` (default), or `--uno` with the following set-up:
 
 | Type | Description                                                                |
 | ---- | -------------------------------------------------------------------------- |
-|  duo | Contains two LND nodes named `aesir-ping` and `aesir-pong` unified by <br> one single `aesir-bitcoind` service. 
+|  duo | Contains two LND nodes named `aesir-ping` and `aesir-pong` unified by <br> one single `aesir-bitcoind` service. |
+|  ohm | Only has `aesir-bitcoind` without any Lightning nodes. |
 |  uno | Only has one LND node named `aesir-lnd` connected to `aesir-bitcoind`. |
 
 ### Peripheral containers
 
 This project also helps you setup peripheral services to make development process easier, too.
 For example, if you want to deploy a duo-cluster with attached postgres database, run the following:
 
@@ -183,14 +184,15 @@
 * **0.3.4** Simplify deployment workflows and 
 * **0.3.5** Restructure project so that when installed, `src` folder will not be created
 * **0.3.6** Breakdown "setup" command into "build" and "pull"
 * **0.3.7** Lightning cluster now with [ord](https://github.com/ordinals/ord)
 * **0.3.8** Rename "ord" to "ord-server" to avoid confusion with cli
 * **0.3.9** Remove intermediate containers
 * **0.4.0** Resist electricity with "ohm" mode
+* **0.4.1** Remove Ordinals' spiked ball
 
 ## Roadmap
 
 * Make image versioning a little bit more intuitive.
 * Add `aesir-tesla-ball` peripheral service using [tesla-ball](https://github.com/krutt/tesla-ball)
 * Write [click](https://click.palletsprojects.com) tests.
 * Use [joblib](https://github.com/joblib/joblib) to speed up deployment with parallelization.
@@ -218,15 +220,15 @@
 > Package operations: 33 installs, 0 updates, 0 removals
 >
 >   • ...
 >   • ...
 >   • ...
 >   • ...
 >
-> Installing the current project: aesir (0.4.0)
+> Installing the current project: aesir (0.4.1)
 ```
 
 ### Known issues
 
 You may run into this setback when first running this project. This is a
 [docker-py](https://github.com/docker/docker-py/issues/3059) issue widely known as of October 2022.
```

