# Comparing `tmp/super-ide-1.4.6.tar.gz` & `tmp/super-ide-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "super-ide-1.4.6.tar", last modified: Wed Mar 27 15:26:00 2024, max compression
+gzip compressed data, was "super-ide-1.4.7.tar", last modified: Wed Apr  3 15:56:45 2024, max compression
```

## Comparing `super-ide-1.4.6.tar` & `super-ide-1.4.7.tar`

### file list

```diff
@@ -1,117 +1,112 @@
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/
--rw-r--r--   0 xukun     (1000) xukun     (1000)    34520 2024-02-28 18:17:14.000000 super-ide-1.4.6/LICENSE
--rw-r--r--   0 xukun     (1000) xukun     (1000)      111 2024-02-28 18:17:14.000000 super-ide-1.4.6/MANIFEST.in
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2724 2024-03-27 15:26:00.841113 super-ide-1.4.6/PKG-INFO
--rw-r--r--   0 xukun     (1000) xukun     (1000)      790 2024-02-28 18:17:14.000000 super-ide-1.4.6/README.rst
--rw-r--r--   0 xukun     (1000) xukun     (1000)       38 2024-03-27 15:26:00.841113 super-ide-1.4.6/setup.cfg
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3436 2024-02-28 18:17:14.000000 super-ide-1.4.6/setup.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/super_ide.egg-info/
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2724 2024-03-27 15:26:00.000000 super-ide-1.4.6/super_ide.egg-info/PKG-INFO
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2689 2024-03-27 15:26:00.000000 super-ide-1.4.6/super_ide.egg-info/SOURCES.txt
--rw-r--r--   0 xukun     (1000) xukun     (1000)        1 2024-03-27 15:26:00.000000 super-ide-1.4.6/super_ide.egg-info/dependency_links.txt
--rw-r--r--   0 xukun     (1000) xukun     (1000)      161 2024-03-27 15:26:00.000000 super-ide-1.4.6/super_ide.egg-info/entry_points.txt
--rw-r--r--   0 xukun     (1000) xukun     (1000)      284 2024-03-27 15:26:00.000000 super-ide-1.4.6/super_ide.egg-info/requires.txt
--rw-r--r--   0 xukun     (1000) xukun     (1000)        9 2024-03-27 15:26:00.000000 super-ide-1.4.6/super_ide.egg-info/top_level.txt
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2027 2024-03-27 15:23:03.000000 super-ide-1.4.6/superide/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     4449 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/__main__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     8340 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/app.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/boards/
--rw-r--r--   0 xukun     (1000) xukun     (1000)        0 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/boards/__init__.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/boards/__pycache__/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      146 2024-03-07 11:47:38.000000 super-ide-1.4.6/superide/boards/__pycache__/__init__.cpython-312.pyc
--rw-r--r--   0 xukun     (1000) xukun     (1000)     4174 2024-03-21 05:41:57.000000 super-ide-1.4.6/superide/boards/__pycache__/cli.cpython-312.pyc
--rw-r--r--   0 xukun     (1000) xukun     (1000)      207 2024-03-27 14:50:19.000000 super-ide-1.4.6/superide/boards/boards.json
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2937 2024-03-21 05:41:49.000000 super-ide-1.4.6/superide/boards/cli.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     5203 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/cache.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3277 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/cli.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3553 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/compat.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/debug/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      610 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     6135 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/cli.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/debug/config/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      610 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     8965 2024-03-14 04:54:14.000000 super-ide-1.4.6/superide/debug/config/base.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2068 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/blackmagic.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     1742 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/factory.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)      969 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/generic.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     1161 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/jlink.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)      921 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/mspdebug.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)      962 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/native.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)      962 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/qemu.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     1156 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/config/renode.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     1195 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/exception.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     5085 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/helpers.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/debug/process/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      610 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/process/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     4891 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/process/base.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3449 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/process/client.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     7014 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/process/gdb.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     5727 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/debug/process/server.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2972 2024-03-27 09:26:23.000000 super-ide-1.4.6/superide/exception.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     6701 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/fs.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/home/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3986 2024-03-27 09:42:58.000000 super-ide-1.4.6/superide/home/app.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3208 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/cli.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/home/rpc/
--rw-r--r--   0 xukun     (1000) xukun     (1000)        0 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/rpc/__init__.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/home/rpc/handlers/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/rpc/handlers/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2839 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/rpc/handlers/app.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)      603 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/rpc/handlers/base.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2928 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/rpc/handlers/ide.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     6430 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/rpc/handlers/os.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)    16695 2024-03-08 05:56:05.000000 super-ide-1.4.6/superide/home/rpc/handlers/project.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     1202 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/rpc/handlers/registry.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)      627 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/runServer.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.831113 super-ide-1.4.6/superide/home/static/
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/superide/home/static/assets/
--rw-r--r--   0 xukun     (1000) xukun     (1000)    15406 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/home/static/assets/favicon.ico
--rw-r--r--   0 xukun     (1000) xukun     (1000)   107097 2024-03-27 15:20:23.000000 super-ide-1.4.6/superide/home/static/assets/index-6fed80ed.css
--rw-r--r--   0 xukun     (1000) xukun     (1000)   439260 2024-03-27 15:20:23.000000 super-ide-1.4.6/superide/home/static/assets/index-d2bbbc6e.js
--rw-r--r--   0 xukun     (1000) xukun     (1000)      529 2024-03-27 15:21:50.000000 super-ide-1.4.6/superide/home/static/index.html
--rw-r--r--   0 xukun     (1000) xukun     (1000)     7468 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/http.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3522 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/lockfile.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)    10459 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/maintenance.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     6432 2024-03-07 14:58:41.000000 super-ide-1.4.6/superide/proc.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/superide/project/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/project/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)      960 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/project/cli.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/superide/project/commands/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/project/commands/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3253 2024-03-14 04:54:14.000000 super-ide-1.4.6/superide/project/commands/config.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     5446 2024-03-14 04:54:14.000000 super-ide-1.4.6/superide/project/commands/init.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2833 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/project/commands/metadata.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)    18874 2024-03-14 04:54:14.000000 super-ide-1.4.6/superide/project/config.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     1846 2024-03-14 04:54:14.000000 super-ide-1.4.6/superide/project/exception.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     6607 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/project/helpers.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)    31369 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/project/options.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3084 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/project/savedeps.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     8513 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/project/vcsclient.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     1392 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/public.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/superide/registry/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/registry/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2900 2024-03-14 04:54:14.000000 super-ide-1.4.6/superide/registry/cli.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     8683 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/registry/client.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3690 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/registry/mirror.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/superide/run/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/run/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     9493 2024-03-14 04:54:14.000000 super-ide-1.4.6/superide/run/cli.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     1600 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/run/helpers.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     6718 2024-03-27 09:26:23.000000 super-ide-1.4.6/superide/run/processor.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/superide/system/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/system/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)      971 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/system/cli.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/superide/system/commands/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/system/commands/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2448 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/system/commands/completion.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     2933 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/system/commands/info.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3242 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/system/completion.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)    10925 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/telemetry.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/superide/toolchain/
--rw-r--r--   0 xukun     (1000) xukun     (1000)      560 2024-03-14 04:54:14.000000 super-ide-1.4.6/superide/toolchain/__init__.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     4186 2024-03-27 09:26:23.000000 super-ide-1.4.6/superide/toolchain/toolchain.py
--rw-r--r--   0 xukun     (1000) xukun     (1000)     5895 2024-02-28 18:17:14.000000 super-ide-1.4.6/superide/util.py
-drwxr-xr-x   0 xukun     (1000) xukun     (1000)        0 2024-03-27 15:26:00.841113 super-ide-1.4.6/tests/
--rw-r--r--   0 xukun     (1000) xukun     (1000)     3437 2024-02-28 18:17:14.000000 super-ide-1.4.6/tests/test_examples.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.699095 super-ide-1.4.7/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    34520 2024-04-03 15:40:53.000000 super-ide-1.4.7/LICENSE
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      111 2024-04-03 15:40:53.000000 super-ide-1.4.7/MANIFEST.in
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2206 2024-04-03 15:56:45.695076 super-ide-1.4.7/PKG-INFO
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      790 2024-04-03 15:40:53.000000 super-ide-1.4.7/README.rst
+-rwxrwxrwx   0 denk      (1000) denk      (1000)       38 2024-04-03 15:56:45.701098 super-ide-1.4.7/setup.cfg
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3436 2024-04-03 15:40:53.000000 super-ide-1.4.7/setup.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:35.453491 super-ide-1.4.7/super_ide.egg-info/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2206 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/PKG-INFO
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2565 2024-04-03 15:56:34.000000 super-ide-1.4.7/super_ide.egg-info/SOURCES.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        1 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/dependency_links.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      162 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/entry_points.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      284 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/requires.txt
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        9 2024-04-03 15:56:33.000000 super-ide-1.4.7/super_ide.egg-info/top_level.txt
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:35.900990 super-ide-1.4.7/superide/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2026 2024-04-03 15:46:41.000000 super-ide-1.4.7/superide/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     4449 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/__main__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8340 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/app.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:36.009641 super-ide-1.4.7/superide/boards/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/boards/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      207 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/boards/boards.json
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2937 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/boards/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5203 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/cache.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3277 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3553 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/compat.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:36.184642 super-ide-1.4.7/superide/debug/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6135 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:41.617090 super-ide-1.4.7/superide/debug/config/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8965 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2068 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/blackmagic.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1742 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/factory.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      969 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/generic.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1161 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/jlink.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      921 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/mspdebug.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      962 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/native.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      962 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/qemu.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1156 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/config/renode.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1195 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5085 2024-04-03 15:40:53.000000 super-ide-1.4.7/superide/debug/helpers.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:42.211835 super-ide-1.4.7/superide/debug/process/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      610 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/debug/process/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     4891 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/debug/process/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3449 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/debug/process/client.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     7087 2024-04-03 15:46:34.000000 super-ide-1.4.7/superide/debug/process/gdb.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5727 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/debug/process/server.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3197 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6701 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/fs.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:42.577465 super-ide-1.4.7/superide/home/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/home/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3986 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/home/app.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3208 2024-04-03 15:40:54.000000 super-ide-1.4.7/superide/home/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:42.666453 super-ide-1.4.7/superide/home/rpc/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/__init__.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:43.538758 super-ide-1.4.7/superide/home/rpc/handlers/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2839 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/app.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      603 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/base.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2928 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/ide.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6430 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/os.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    16695 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/project.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1202 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/rpc/handlers/registry.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      627 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/runServer.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:43.639614 super-ide-1.4.7/superide/home/static/
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:44.106059 super-ide-1.4.7/superide/home/static/assets/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    15406 2024-04-03 15:41:00.000000 super-ide-1.4.7/superide/home/static/assets/favicon.ico
+-rwxrwxrwx   0 denk      (1000) denk      (1000)   107097 2024-04-03 15:41:01.000000 super-ide-1.4.7/superide/home/static/assets/index-6fed80ed.css
+-rwxrwxrwx   0 denk      (1000) denk      (1000)   439260 2024-04-03 15:41:02.000000 super-ide-1.4.7/superide/home/static/assets/index-d2bbbc6e.js
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      529 2024-04-03 15:41:04.000000 super-ide-1.4.7/superide/home/static/index.html
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     7468 2024-04-03 15:41:05.000000 super-ide-1.4.7/superide/http.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3522 2024-04-03 15:41:05.000000 super-ide-1.4.7/superide/lockfile.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    10459 2024-04-03 15:41:05.000000 super-ide-1.4.7/superide/maintenance.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6432 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/proc.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:44.635321 super-ide-1.4.7/superide/project/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      960 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:44.935488 super-ide-1.4.7/superide/project/commands/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/commands/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3253 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/commands/config.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5446 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/commands/init.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2833 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/commands/metadata.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    18874 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/config.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1846 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/exception.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6607 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/helpers.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    31369 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/options.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3084 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/savedeps.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8513 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/project/vcsclient.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1392 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/public.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.096112 super-ide-1.4.7/superide/registry/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/registry/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2900 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/registry/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     8683 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/registry/client.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3690 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/registry/mirror.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.240996 super-ide-1.4.7/superide/run/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/run/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     9493 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/run/cli.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     1600 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/run/helpers.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     6718 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/run/processor.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.408798 super-ide-1.4.7/superide/system/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/system/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      971 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/system/cli.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.605661 super-ide-1.4.7/superide/system/commands/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:06.000000 super-ide-1.4.7/superide/system/commands/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2448 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/system/commands/completion.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     2933 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/system/commands/info.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3242 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/system/completion.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)    10925 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/telemetry.py
+drwxrwxrwx   0 denk      (1000) denk      (1000)        0 2024-04-03 15:56:45.666665 super-ide-1.4.7/superide/toolchain/
+-rwxrwxrwx   0 denk      (1000) denk      (1000)      560 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/toolchain/__init__.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     3569 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/toolchain/toolchain.py
+-rwxrwxrwx   0 denk      (1000) denk      (1000)     5895 2024-04-03 15:41:07.000000 super-ide-1.4.7/superide/util.py
```

### Comparing `super-ide-1.4.6/LICENSE` & `super-ide-1.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/README.rst` & `super-ide-1.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/setup.py` & `super-ide-1.4.7/setup.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/super_ide.egg-info/SOURCES.txt` & `super-ide-1.4.7/super_ide.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,14 @@
 superide/proc.py
 superide/public.py
 superide/telemetry.py
 superide/util.py
 superide/boards/__init__.py
 superide/boards/boards.json
 superide/boards/cli.py
-superide/boards/__pycache__/__init__.cpython-312.pyc
-superide/boards/__pycache__/cli.cpython-312.pyc
 superide/debug/__init__.py
 superide/debug/cli.py
 superide/debug/exception.py
 superide/debug/helpers.py
 superide/debug/config/__init__.py
 superide/debug/config/base.py
 superide/debug/config/blackmagic.py
@@ -86,9 +84,8 @@
 superide/system/__init__.py
 superide/system/cli.py
 superide/system/completion.py
 superide/system/commands/__init__.py
 superide/system/commands/completion.py
 superide/system/commands/info.py
 superide/toolchain/__init__.py
-superide/toolchain/toolchain.py
-tests/test_examples.py
+superide/toolchain/toolchain.py
```

### Comparing `super-ide-1.4.6/superide/__init__.py` & `super-ide-1.4.7/superide/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #    https://www.gnu.org/licenses/agpl-3.0.txt
 #
 # THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
 # PURPOSE.
 # See the AGPL-3.0 for more details.
 
-VERSION = (1, 4, 6)
+VERSION = (1, 4, 7)
 __version__ = ".".join([str(s) for s in VERSION])
 
 __title__ = "super-ide"
 __description__ = (
     "A professional Cross-platform IDE. "
     "Cross-platform IDE and Unified Debugger. "
     "Static Code Analyzer and Remote Unit Testing. "
@@ -52,9 +52,9 @@
     "185.199.110.153",  # Github.com
     "88.198.170.159",  # mengning.com.cn
     "github.com",
 ] + __registry_mirror_hosts__
 
 __configfile__ = "SuperIDE.ini"
 
-__container_engine__ = "docker"
+__container_engine__ = "isula"
```

### Comparing `super-ide-1.4.6/superide/__main__.py` & `super-ide-1.4.7/superide/__main__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/app.py` & `super-ide-1.4.7/superide/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/boards/cli.py` & `super-ide-1.4.7/superide/boards/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/cache.py` & `super-ide-1.4.7/superide/cache.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/cli.py` & `super-ide-1.4.7/superide/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/compat.py` & `super-ide-1.4.7/superide/compat.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/__init__.py` & `super-ide-1.4.7/superide/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/cli.py` & `super-ide-1.4.7/superide/debug/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/__init__.py` & `super-ide-1.4.7/superide/debug/config/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/base.py` & `super-ide-1.4.7/superide/debug/config/base.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/blackmagic.py` & `super-ide-1.4.7/superide/debug/config/blackmagic.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/factory.py` & `super-ide-1.4.7/superide/debug/config/factory.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/generic.py` & `super-ide-1.4.7/superide/debug/config/generic.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/jlink.py` & `super-ide-1.4.7/superide/debug/config/jlink.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/mspdebug.py` & `super-ide-1.4.7/superide/debug/config/mspdebug.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/native.py` & `super-ide-1.4.7/superide/debug/config/native.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/qemu.py` & `super-ide-1.4.7/superide/debug/config/qemu.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/config/renode.py` & `super-ide-1.4.7/superide/debug/config/renode.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/exception.py` & `super-ide-1.4.7/superide/debug/exception.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/helpers.py` & `super-ide-1.4.7/superide/debug/helpers.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/process/__init__.py` & `super-ide-1.4.7/superide/debug/process/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/process/base.py` & `super-ide-1.4.7/superide/debug/process/base.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/process/client.py` & `super-ide-1.4.7/superide/debug/process/client.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/debug/process/gdb.py` & `super-ide-1.4.7/superide/debug/process/gdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,21 +32,24 @@
         self._target_is_running = False
         self._errors_buffer = b""
 
     async def run(self, extra_args):  # pylint: disable=arguments-differ
         await super().run()
 
         self.generate_init_script(os.path.join(self.working_dir, self.PIO_SRC_NAME))
-        gdb_path = self.debug_config.client_executable_path or "gdb"
+        gdb_path = self.debug_config.client_executable_path or "docker"
         # start GDB client
         args = [
             gdb_path,
-            "-q",
-            "--directory",
-            self.working_dir,
+            'exec',
+            '-i',
+            'boring_cray',
+            'gdb-multiarch',
+            '-q',
+            '--interpreter=mi2',
             "--directory",
             self.project_dir,
             "-l",
             "10",
         ]
         args.extend(list(extra_args or []))
         gdb_data_dir = self._get_data_dir(gdb_path)
```

### Comparing `super-ide-1.4.6/superide/debug/process/server.py` & `super-ide-1.4.7/superide/debug/process/server.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/exception.py` & `super-ide-1.4.7/superide/exception.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #
 #    https://www.gnu.org/licenses/agpl-3.0.txt
 #
 # THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND, EITHER EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT, MERCHANTABILITY OR FIT FOR A PARTICULAR
 # PURPOSE.
 # See the AGPL-3.0 for more details.
+from superide import __container_engine__
 
 
 class SuperIDEException(Exception):
     MESSAGE = None
 
     def __str__(self):  # pragma: no cover
         if self.MESSAGE:
@@ -31,17 +32,21 @@
     pass
 
 
 class AbortedByUser(UserSideException):
     MESSAGE = "Aborted by user"
 
 class ContainerEngineNotFound(UserSideException):
-    MESSAGE = "ContainerEngine not to be found"
+    MESSAGE = f"ContainerEngine({__container_engine__}) not to be found"
 
+class ImageNotGet(UserSideException):
+    MESSAGE = "Failed to get image."
 
+class InitProjectError(UserSideException):
+    MESSAGE = "Failed to init project."
 #
 # UDEV Rules
 #
 
 
 class InvalidUdevRules(UserSideException):
     pass
```

### Comparing `super-ide-1.4.6/superide/fs.py` & `super-ide-1.4.7/superide/fs.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/__init__.py` & `super-ide-1.4.7/superide/home/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/app.py` & `super-ide-1.4.7/superide/home/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/cli.py` & `super-ide-1.4.7/superide/home/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/rpc/handlers/__init__.py` & `super-ide-1.4.7/superide/home/rpc/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/rpc/handlers/app.py` & `super-ide-1.4.7/superide/home/rpc/handlers/app.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/rpc/handlers/base.py` & `super-ide-1.4.7/superide/home/rpc/handlers/base.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/rpc/handlers/ide.py` & `super-ide-1.4.7/superide/home/rpc/handlers/ide.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/rpc/handlers/os.py` & `super-ide-1.4.7/superide/home/rpc/handlers/os.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/rpc/handlers/project.py` & `super-ide-1.4.7/superide/home/rpc/handlers/project.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/rpc/handlers/registry.py` & `super-ide-1.4.7/superide/home/rpc/handlers/registry.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/runServer.py` & `super-ide-1.4.7/superide/home/runServer.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/static/assets/favicon.ico` & `super-ide-1.4.7/superide/home/static/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/static/assets/index-6fed80ed.css` & `super-ide-1.4.7/superide/home/static/assets/index-6fed80ed.css`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/static/assets/index-d2bbbc6e.js` & `super-ide-1.4.7/superide/home/static/assets/index-d2bbbc6e.js`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/home/static/index.html` & `super-ide-1.4.7/superide/home/static/index.html`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/http.py` & `super-ide-1.4.7/superide/http.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/lockfile.py` & `super-ide-1.4.7/superide/lockfile.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/maintenance.py` & `super-ide-1.4.7/superide/maintenance.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/proc.py` & `super-ide-1.4.7/superide/proc.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/__init__.py` & `super-ide-1.4.7/superide/project/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/cli.py` & `super-ide-1.4.7/superide/project/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/commands/__init__.py` & `super-ide-1.4.7/superide/project/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/commands/config.py` & `super-ide-1.4.7/superide/project/commands/config.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/commands/init.py` & `super-ide-1.4.7/superide/project/commands/init.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/commands/metadata.py` & `super-ide-1.4.7/superide/project/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/config.py` & `super-ide-1.4.7/superide/project/config.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/exception.py` & `super-ide-1.4.7/superide/project/exception.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/helpers.py` & `super-ide-1.4.7/superide/project/helpers.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/options.py` & `super-ide-1.4.7/superide/project/options.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/savedeps.py` & `super-ide-1.4.7/superide/project/savedeps.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/project/vcsclient.py` & `super-ide-1.4.7/superide/project/vcsclient.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/public.py` & `super-ide-1.4.7/superide/public.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/registry/__init__.py` & `super-ide-1.4.7/superide/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/registry/cli.py` & `super-ide-1.4.7/superide/registry/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/registry/client.py` & `super-ide-1.4.7/superide/registry/client.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/registry/mirror.py` & `super-ide-1.4.7/superide/registry/mirror.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/run/__init__.py` & `super-ide-1.4.7/superide/run/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/run/cli.py` & `super-ide-1.4.7/superide/run/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/run/helpers.py` & `super-ide-1.4.7/superide/run/helpers.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/run/processor.py` & `super-ide-1.4.7/superide/run/processor.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/system/__init__.py` & `super-ide-1.4.7/superide/system/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/system/cli.py` & `super-ide-1.4.7/superide/system/cli.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/system/commands/__init__.py` & `super-ide-1.4.7/superide/system/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/system/commands/completion.py` & `super-ide-1.4.7/superide/system/commands/completion.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/system/commands/info.py` & `super-ide-1.4.7/superide/system/commands/info.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/system/completion.py` & `super-ide-1.4.7/superide/system/completion.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/telemetry.py` & `super-ide-1.4.7/superide/telemetry.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/toolchain/__init__.py` & `super-ide-1.4.7/superide/toolchain/__init__.py`

 * *Files identical despite different names*

### Comparing `super-ide-1.4.6/superide/toolchain/toolchain.py` & `super-ide-1.4.7/superide/toolchain/toolchain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,53 @@
 import json
 import subprocess
 import os
-import shutil
-import sys
-from superide import __container_engine__
+from superide import __container_engine__, exception
 
 class Toolchain:
+    check_image_flag = False
+
     def __init__(self, image_name, project_directory):
         check_container_engine_availability()
         self.image_name = image_name
         self.project_directory = project_directory
         self.contain_project_directory = "/app/project"
         self.check_image()
         
         
     def check_image(self):
+        if(Toolchain.check_image_flag):
+            return
         try:
-            output = subprocess.check_output([__container_engine__, "images", "-q", self.image_name])
-            if output:
-                return
-            else:
-                print(f"The image '{self.image_name}' does not exist locally, will be pulled.")
-                # 拉取镜像
-                subprocess.run([__container_engine__, 'pull', self.image_name])
-
+            print('check image...')
+            if(__container_engine__ == 'docker'):
+                output = subprocess.check_output(["docker", "images", "-q", self.image_name])
+                if output:
+                    Toolchain.check_image_flag = True
+                    return
+            subprocess.run([__container_engine__, 'pull', self.image_name], stderr=subprocess.DEVNULL)
+            Toolchain.check_image_flag = True
         except subprocess.CalledProcessError:
-            print("Failed to get image.")
-            sys.exit(1)
+            raise exception.ImageNotGet()
 
     def init_project(self):
         # 文件夹非空则不能创建项目
         if(len(os.listdir(self.project_directory)) != 0):
             print("can't init project in Non empty folder")
-            sys.exit(1)
-        container_name = 'CopyExampleProjectDemo'
-        source_path = '/app/ExampleProject'
-        destination_path = self.project_directory
+            raise exception.InitProjectError()
+        
+        source_path = '/app/ExampleProject/.'
+        destination_path = self.contain_project_directory
         try:
-            # 创建容器
-            create_command = [__container_engine__, 'create', '--name', container_name, self.image_name]
-            subprocess.run(create_command)
-
-            # 复制文件
-            copy_command = [__container_engine__, 'cp', f'{container_name}:{source_path}', destination_path]
-            subprocess.run(copy_command)
-
-            # 删除容器（可选）
-            delete_command = [__container_engine__, 'rm', container_name]
-            subprocess.run(delete_command)
-
-            # 移动到项目目录
-            source_path = destination_path + '/ExampleProject/'
-            for file in os.listdir(source_path):
-                src_file = os.path.join(source_path, file)
-                dst_file = os.path.join(destination_path, file)
-                shutil.move(src_file, dst_file)
-            clear_command = ['rm', '-rf', source_path]
-            subprocess.run(clear_command)
+            command = [__container_engine__, "run","-it","--rm", "-v", self.project_directory+":"+self.contain_project_directory, self.image_name, 
+                       'cp', '-r', source_path, destination_path];
+            subprocess.run(command)
         except Exception:
             print("init project failed")
-            sys.exit(1)
+            raise exception.InitProjectError()
 
     def _get_tools(self):
         with open(f'{self.project_directory}/.vscode/tasks.json') as file:
             config = json.load(file)
         for task in config['tasks']:
             if task['label'] == 'Build':
                 self.build_task = task
@@ -100,12 +84,10 @@
 
 def check_container_engine_availability():
     path = get_container_engine_path()
     if path:
         try:
             subprocess.run([path, '--version'], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
         except subprocess.CalledProcessError:
-            print(f"{__container_engine__} is not available.")
-            sys.exit(1)
+            raise exception.ContainerEngineNotFound()
     else:
-        print(f"{__container_engine__} not found on the system.")
-        sys.exit(1)
+        raise exception.ContainerEngineNotFound()
```

### Comparing `super-ide-1.4.6/superide/util.py` & `super-ide-1.4.7/superide/util.py`

 * *Files identical despite different names*

