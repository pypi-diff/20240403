# Comparing `tmp/runtimepy-3.8.0.tar.gz` & `tmp/runtimepy-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runtimepy-3.8.0.tar", last modified: Sat Feb 24 17:24:09 2024, max compression
+gzip compressed data, was "runtimepy-3.9.0.tar", last modified: Mon Feb 26 03:24:13 2024, max compression
```

## Comparing `runtimepy-3.8.0.tar` & `runtimepy-3.9.0.tar`

### file list

```diff
@@ -1,215 +1,219 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.423551 runtimepy-3.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-24 17:22:20.000000 runtimepy-3.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-02-24 17:24:09.423551 runtimepy-3.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-02-24 17:22:20.000000 runtimepy-3.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-02-24 17:22:20.000000 runtimepy-3.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.395551 runtimepy-3.8.0/runtimepy/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.395551 runtimepy-3.8.0/runtimepy/channel/
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.399551 runtimepy-3.8.0/runtimepy/channel/environment/
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/environment/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/environment/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.399551 runtimepy-3.8.0/runtimepy/channel/environment/command/
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/environment/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/environment/command/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/environment/command/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/environment/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/environment/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/channel/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.399551 runtimepy-3.8.0/runtimepy/codec/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/codec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.399551 runtimepy-3.8.0/runtimepy/codec/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/codec/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/codec/protocol/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/codec/protocol/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.399551 runtimepy-3.8.0/runtimepy/codec/system/
--rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/codec/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.399551 runtimepy-3.8.0/runtimepy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/commands/arbiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/commands/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/commands/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/commands/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/commands/tui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.399551 runtimepy-3.8.0/runtimepy/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/factories.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.403551 runtimepy-3.8.0/runtimepy/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/BitFields.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/Channel.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/ChannelCommand.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/ChannelRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/EnumRegistry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/FindFile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/RuntimeEnum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/TaskConfig.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/has_factory.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/has_name.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/data/schemas/has_request_flag.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.403551 runtimepy-3.8.0/runtimepy/enum/
--rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/enum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/enum/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/enum/type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.403551 runtimepy-3.8.0/runtimepy/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/metrics/channel.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/metrics/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/metrics/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.403551 runtimepy-3.8.0/runtimepy/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/mixins/async_command.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/mixins/enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/mixins/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/mixins/finalize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/mixins/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/mixins/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.407551 runtimepy-3.8.0/runtimepy/net/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.407551 runtimepy-3.8.0/runtimepy/net/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.407551 runtimepy-3.8.0/runtimepy/net/arbiter/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.407551 runtimepy-3.8.0/runtimepy/net/arbiter/factory/
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/factory/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/factory/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.407551 runtimepy-3.8.0/runtimepy/net/arbiter/housekeeping/
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/housekeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/imports.py
--rw-r--r--   0 runner    (1001) docker     (127)     5517 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/result.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.407551 runtimepy-3.8.0/runtimepy/net/arbiter/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/tcp/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/udp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/arbiter/websocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.407551 runtimepy-3.8.0/runtimepy/net/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/factories/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.411551 runtimepy-3.8.0/runtimepy/net/http/
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/http/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/http/header.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/http/request_target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/http/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/http/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/http/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.411551 runtimepy-3.8.0/runtimepy/net/server/
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/server/html.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/server/json.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.411551 runtimepy-3.8.0/runtimepy/net/stream/
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/stream/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.411551 runtimepy-3.8.0/runtimepy/net/stream/json/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/stream/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/stream/json/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/stream/json/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/stream/json/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/stream/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.411551 runtimepy-3.8.0/runtimepy/net/tcp/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/tcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/tcp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/tcp/create.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.411551 runtimepy-3.8.0/runtimepy/net/tcp/http/
--rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/tcp/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/tcp/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.411551 runtimepy-3.8.0/runtimepy/net/tcp/telnet/
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/tcp/telnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/tcp/telnet/codes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.411551 runtimepy-3.8.0/runtimepy/net/udp/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/udp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/udp/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/udp/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/udp/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.415551 runtimepy-3.8.0/runtimepy/net/websocket/
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/net/websocket/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.415551 runtimepy-3.8.0/runtimepy/primitives/
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.415551 runtimepy-3.8.0/runtimepy/primitives/array/
--rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7561 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/byte_order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.415551 runtimepy-3.8.0/runtimepy/primitives/field/
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/field/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.415551 runtimepy-3.8.0/runtimepy/primitives/field/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/field/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/field/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/int.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/scaling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.415551 runtimepy-3.8.0/runtimepy/primitives/serializable/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/serializable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/serializable/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/serializable/fixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/serializable/prefixed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/string.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.415551 runtimepy-3.8.0/runtimepy/primitives/type/
--rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/type/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/type/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/type/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/type/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/type/float.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/primitives/type/int.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/runtimepy/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/registry/bool.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/registry/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/registry/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/runtimepy/task/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/task/asynchronous.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/runtimepy/task/basic/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/task/basic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/task/basic/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/task/basic/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/runtimepy/task/trig/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/task/trig/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/runtimepy/telemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/runtimepy/tui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/tui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/runtimepy/tui/channels/
--rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/tui/channels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/tui/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/tui/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/tui/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/tui/task.py
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-24 17:22:20.000000 runtimepy-3.8.0/runtimepy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/runtimepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-02-24 17:24:09.000000 runtimepy-3.8.0/runtimepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-02-24 17:24:09.000000 runtimepy-3.8.0/runtimepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-24 17:24:09.000000 runtimepy-3.8.0/runtimepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-24 17:24:09.000000 runtimepy-3.8.0/runtimepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-24 17:24:09.000000 runtimepy-3.8.0/runtimepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-24 17:24:09.000000 runtimepy-3.8.0/runtimepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-24 17:24:09.423551 runtimepy-3.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-24 17:22:20.000000 runtimepy-3.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-24 17:24:09.419551 runtimepy-3.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-24 17:22:20.000000 runtimepy-3.8.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-24 17:22:20.000000 runtimepy-3.8.0/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-24 17:22:20.000000 runtimepy-3.8.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.596395 runtimepy-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-02-26 03:21:58.000000 runtimepy-3.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-02-26 03:24:13.592395 runtimepy-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-02-26 03:21:58.000000 runtimepy-3.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-02-26 03:21:58.000000 runtimepy-3.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.568395 runtimepy-3.9.0/runtimepy/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/channel/
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/channel/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3481 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/channel/environment/command/
+-rw-r--r--   0 runner    (1001) docker     (127)     8144 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/command/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/command/processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/command/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5004 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7034 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/environment/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/channel/event/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/event/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5703 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/channel/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/codec/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/codec/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9041 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/protocol/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4257 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/protocol/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/codec/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     6950 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/codec/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/arbiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/commands/tui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.572395 runtimepy-3.9.0/runtimepy/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/factories.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   362870 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.576395 runtimepy-3.9.0/runtimepy/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/BitFields.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/Channel.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ChannelCommand.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ChannelRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ClientConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/EnumRegistry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/FindFile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/RuntimeEnum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/ServerConnectionConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/TaskConfig.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/has_factory.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/has_name.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/data/schemas/has_request_flag.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.576395 runtimepy-3.9.0/runtimepy/enum/
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/enum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/enum/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/enum/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.576395 runtimepy-3.9.0/runtimepy/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/metrics/channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/metrics/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/metrics/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1686 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/async_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/finalize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/mixins/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11954 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8457 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/arbiter/factory/
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/factory/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/factory/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/arbiter/housekeeping/
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/housekeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/imports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/arbiter/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/tcp/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/udp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/arbiter/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11292 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.580395 runtimepy-3.9.0/runtimepy/net/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/factories/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/request_target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/http/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/server/html.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/server/json.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/stream/
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/stream/json/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/json/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3754 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/json/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/json/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/stream/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/tcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6911 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/create.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/tcp/http/
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/tcp/telnet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/telnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/tcp/telnet/codes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.584395 runtimepy-3.9.0/runtimepy/net/udp/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/udp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7560 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/udp/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/udp/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/udp/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/net/websocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/net/websocket/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/array/
+-rw-r--r--   0 runner    (1001) docker     (127)     8311 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7561 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/byte_order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/field/
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6620 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/field/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/field/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     2668 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/field/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6130 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/field/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/scaling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/serializable/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/serializable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/serializable/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/serializable/fixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/serializable/prefixed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/string.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.588395 runtimepy-3.9.0/runtimepy/primitives/type/
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/float.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/primitives/type/int.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/registry/bool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/registry/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/registry/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/task/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/asynchronous.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/task/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/basic/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/basic/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/task/trig/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/task/trig/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy/tui/channels/
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/channels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/tui/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-02-26 03:21:58.000000 runtimepy-3.9.0/runtimepy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/runtimepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6941 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-26 03:24:13.000000 runtimepy-3.9.0/runtimepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 03:24:13.596395 runtimepy-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-02-26 03:21:58.000000 runtimepy-3.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 03:24:13.592395 runtimepy-3.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-02-26 03:21:58.000000 runtimepy-3.9.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-26 03:21:58.000000 runtimepy-3.9.0/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-02-26 03:21:58.000000 runtimepy-3.9.0/tests/test_resources.py
```

### Comparing `runtimepy-3.8.0/LICENSE` & `runtimepy-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/PKG-INFO` & `runtimepy-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 3.8.0
+Version: 3.9.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,17 +13,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: svgen>=0.5.0
 Requires-Dist: vcorelib>=3.2.0
 Requires-Dist: websockets
-Requires-Dist: svgen>=0.5.0
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -37,19 +37,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=d0656a2e337796f56cdb520895ea2f08
+    hash=c7bfaabcb235afbdae1921e1defa2f1a
     =====================================
 -->
 
-# runtimepy ([3.8.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([3.9.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-3.8.0/README.md` & `runtimepy-3.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=d0656a2e337796f56cdb520895ea2f08
+    hash=c7bfaabcb235afbdae1921e1defa2f1a
     =====================================
 -->
 
-# runtimepy ([3.8.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([3.9.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-3.8.0/pyproject.toml` & `runtimepy-3.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "runtimepy"
-version = "3.8.0"
+version = "3.9.0"
 description = "A framework for implementing Python services."
 readme = "README.md"
 requires-python = ">=3.11"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `runtimepy-3.8.0/runtimepy/app.py` & `runtimepy-3.9.0/runtimepy/app.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/channel/__init__.py` & `runtimepy-3.9.0/runtimepy/channel/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from typing import Union as _Union
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 
 # internal
+from runtimepy.channel.event import PrimitiveEvent
 from runtimepy.mixins.enum import EnumMixin as _EnumMixin
 from runtimepy.primitives import T as _T
 from runtimepy.primitives import normalize as _normalize
 from runtimepy.primitives.bool import Bool as _Bool
 from runtimepy.primitives.float import Double as _Double
 from runtimepy.primitives.float import Float as _Float
 from runtimepy.primitives.int import Int8 as _Int8
@@ -55,14 +56,17 @@
 
         # Whether or not this channel should accept commands.
         self.commandable: bool = _cast(bool, data["commandable"])
 
         # A key to this channel's enumeration in the enumeration registry.
         self._enum = _cast(str, data.get("enum"))
 
+        # An event-streaming interface.
+        self.event = PrimitiveEvent(self.raw, self.id)
+
     def asdict(self) -> _JsonObject:
         """Obtain a dictionary representing this instance."""
 
         result = {
             "id": self.id,
             "type": str(self.type),
             "commandable": self.commandable,
```

### Comparing `runtimepy-3.8.0/runtimepy/channel/environment/__init__.py` & `runtimepy-3.9.0/runtimepy/channel/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/channel/environment/array.py` & `runtimepy-3.9.0/runtimepy/channel/environment/array.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/channel/environment/base.py` & `runtimepy-3.9.0/runtimepy/channel/environment/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/channel/environment/command/__init__.py` & `runtimepy-3.9.0/runtimepy/channel/environment/command/processor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-A module implementing UI command processing.
+A module implementing a channel-command processing interface.
 """
 
 # built-in
 from argparse import Namespace
 from typing import Any, Callable, Optional, cast
 
 # third-party
@@ -19,25 +19,14 @@
 from runtimepy.channel.environment.command.result import SUCCESS, CommandResult
 from runtimepy.mixins.environment import ChannelEnvironmentMixin
 from runtimepy.primitives.bool import Bool
 from runtimepy.primitives.field import BitField
 
 CommandHook = Callable[[Namespace, Optional[FieldOrChannel]], None]
 
-# Declared so we re-export FieldOrChannel after moving where it's declared.
-__all__ = [
-    "CommandHook",
-    "FieldOrChannel",
-    "ChannelCommandProcessor",
-    "EnvironmentMap",
-    "ENVIRONMENTS",
-    "clear_env",
-    "register_env",
-]
-
 
 class ChannelCommandProcessor(ChannelEnvironmentMixin):
     """A command processing interface for channel environments."""
 
     def __init__(
         self, env: ChannelEnvironment, logger: LoggerType, **kwargs
     ) -> None:
@@ -190,27 +179,7 @@
             assert args is not None
             result = self.handle_command(args)
 
         return result
 
 
 EnvironmentMap = dict[str, ChannelCommandProcessor]
-ENVIRONMENTS: EnvironmentMap = {}
-
-
-def clear_env() -> None:
-    """Reset the global environment mapping."""
-    ENVIRONMENTS.clear()
-
-
-def env_json_data() -> dict[str, Any]:
-    """Get JSON data for each environment."""
-    return {key: cmd.env.export_json for key, cmd in ENVIRONMENTS.items()}
-
-
-def register_env(name: str, env: ChannelCommandProcessor) -> None:
-    """Register a channel environment globally."""
-
-    assert (
-        name not in ENVIRONMENTS or ENVIRONMENTS[name] is env
-    ), f"Can't register environment '{name}'!"
-    ENVIRONMENTS[name] = env
```

### Comparing `runtimepy-3.8.0/runtimepy/channel/environment/command/parser.py` & `runtimepy-3.9.0/runtimepy/channel/environment/command/parser.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/channel/environment/command/result.py` & `runtimepy-3.9.0/runtimepy/channel/environment/command/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/channel/environment/create.py` & `runtimepy-3.9.0/runtimepy/channel/environment/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/channel/environment/file.py` & `runtimepy-3.9.0/runtimepy/channel/environment/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,17 @@
     """A class integrating file-system operations with channel environments."""
 
     def export_json(
         self, resolve_enum: bool = True
     ) -> _Dict[str, _JsonObject]:
         """Get this channel environment as a single dictionary."""
 
+        # Only allow exporting finalized environments.
+        self.finalize(strict=False)
+
         return {
             CHANNELS_KEY: self.channels.asdict(),
             ENUMS_KEY: self.enums.asdict(),
             FIELDS_KEY: self.fields.asdict(),
             NAMES_KEY: {
                 CHANNELS_KEY: _cast(_JsonValue, self.channels.names.asdict()),
                 ENUMS_KEY: _cast(_JsonValue, self.enums.names.asdict()),
@@ -75,14 +78,17 @@
         fields: _Pathlike = FIELDS_FILE,
         names: _Pathlike = NAMES_FILE,
         resolve_enum: bool = True,
         **kwargs,
     ) -> None:
         """Write channel and enum registries to disk."""
 
+        # Only allow exporting finalized environments.
+        self.finalize(strict=False)
+
         self.channels.encode(channels, **kwargs)
         self.enums.encode(enums, **kwargs)
         self.fields.encode(fields, **kwargs)
 
         # Keep track of name-to-identifier mappings for all such mappings.
         _ARBITER.encode(
             names,
@@ -116,43 +122,53 @@
             fields=path.joinpath(FIELDS_FILE),
             names=path.joinpath(NAMES_FILE),
             resolve_enum=resolve_enum,
             **kwargs,
         )
 
     @classmethod
-    def load_json(cls: _Type[T], data: _Dict[str, _JsonObject]) -> T:
+    def load_json(
+        cls: _Type[T], data: _Dict[str, _JsonObject], finalize: bool = True
+    ) -> T:
         """Load a channel environment from JSON data."""
 
         chan_reg = _ChannelRegistry.create(data[CHANNELS_KEY])
         enum_reg = _EnumRegistry.create(data[ENUMS_KEY])
 
         # Handle name data.
         chan_reg.names.load_name_to_key(
             _cast(_NameToKey[int], data[NAMES_KEY][CHANNELS_KEY])
         )
         enum_reg.names.load_name_to_key(
             _cast(_NameToKey[int], data[NAMES_KEY][ENUMS_KEY])
         )
 
-        return cls(
+        result = cls(
             channels=chan_reg,
             enums=enum_reg,
             values=_cast(_Optional[_ValueMap], data.get(VALUES_KEY)),
             fields=_fields_from_dict(data[FIELDS_KEY]),
         )
 
+        # Typically, externally loaded environments should be final at load
+        # time.
+        if finalize:
+            result.finalize()
+
+        return result
+
     @classmethod
     def load(
         cls: _Type[T],
         channels: _Pathlike = CHANNELS_FILE,
         enums: _Pathlike = ENUMS_FILE,
         values: _Pathlike = VALUES_FILE,
         fields: _Pathlike = FIELDS_FILE,
         names: _Pathlike = NAMES_FILE,
+        finalize: bool = True,
     ) -> T:
         """Load a channel environment from a pair of files."""
 
         value_map: _Optional[_ValueMap] = None
 
         # Load the value map if it's present.
         values = _normalize(values)
@@ -170,27 +186,37 @@
         chan_reg.names.load_name_to_key(
             _cast(_NameToKey[int], name_data[CHANNELS_KEY])
         )
         enum_reg.names.load_name_to_key(
             _cast(_NameToKey[int], name_data[ENUMS_KEY])
         )
 
-        return cls(
+        result = cls(
             channels=chan_reg,
             enums=enum_reg,
             values=value_map,
             fields=_fields_from_file(fields),
         )
 
+        # Typically, externally loaded environments should be final at load
+        # time.
+        if finalize:
+            result.finalize()
+
+        return result
+
     @classmethod
-    def load_directory(cls: _Type[T], path: _Pathlike) -> T:
+    def load_directory(
+        cls: _Type[T], path: _Pathlike, finalize: bool = True
+    ) -> T:
         """Load a channel environment from a directory."""
 
         path = _normalize(path, require=True)
         assert path.is_dir(), f"'{path}' is not a directory!"
         return cls.load(
             channels=path.joinpath(CHANNELS_FILE),
             enums=path.joinpath(ENUMS_FILE),
             values=path.joinpath(VALUES_FILE),
             fields=path.joinpath(FIELDS_FILE),
             names=path.joinpath(NAMES_FILE),
+            finalize=finalize,
         )
```

### Comparing `runtimepy-3.8.0/runtimepy/codec/protocol/__init__.py` & `runtimepy-3.9.0/runtimepy/codec/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/codec/protocol/base.py` & `runtimepy-3.9.0/runtimepy/codec/protocol/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/codec/protocol/json.py` & `runtimepy-3.9.0/runtimepy/codec/protocol/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/codec/system/__init__.py` & `runtimepy-3.9.0/runtimepy/codec/system/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/commands/all.py` & `runtimepy-3.9.0/runtimepy/commands/all.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/commands/arbiter.py` & `runtimepy-3.9.0/runtimepy/commands/arbiter.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/commands/common.py` & `runtimepy-3.9.0/runtimepy/commands/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/commands/server.py` & `runtimepy-3.9.0/runtimepy/commands/server.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/commands/task.py` & `runtimepy-3.9.0/runtimepy/commands/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/commands/tui.py` & `runtimepy-3.9.0/runtimepy/commands/tui.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/data/factories.yaml` & `runtimepy-3.9.0/runtimepy/data/factories.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/data/favicon.ico` & `runtimepy-3.9.0/runtimepy/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/data/schemas/BitFields.yaml` & `runtimepy-3.9.0/runtimepy/data/schemas/BitFields.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml` & `runtimepy-3.9.0/runtimepy/data/schemas/ConnectionArbiterConfig.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/data/schemas/FindFile.yaml` & `runtimepy-3.9.0/runtimepy/data/schemas/FindFile.yaml`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/entry.py` & `runtimepy-3.9.0/runtimepy/entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/enum/__init__.py` & `runtimepy-3.9.0/runtimepy/enum/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/enum/registry.py` & `runtimepy-3.9.0/runtimepy/enum/registry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/enum/type.py` & `runtimepy-3.9.0/runtimepy/enum/type.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/mapping.py` & `runtimepy-3.9.0/runtimepy/mapping.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 A module implementing a generic, two-way mapping interface.
 """
 
 # built-in
+import re
 from typing import Dict as _Dict
 from typing import Generic as _Generic
-from typing import Iterator as _Iterator
+from typing import Iterable, Iterator
 from typing import List as _List
 from typing import MutableMapping as _MutableMapping
 from typing import Optional as _Optional
 from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import Union as _Union
 from typing import cast as _cast
@@ -34,14 +35,27 @@
 BoolMappingData = _MutableMapping[MappingKey[bool], MappingKey[bool]]
 EnumMappingData = _Union[
     IntMappingData,
     BoolMappingData,
     _MutableMapping[str, bool],
     _MutableMapping[str, int],
 ]
+DEFAULT_PATTERN = ".*"
+
+
+def name_search(
+    names: Iterable[str], pattern: str, exact: bool = False
+) -> Iterator[str]:
+    """A simple name searching method."""
+
+    compiled = re.compile(pattern)
+    for name in names:
+        if compiled.search(name) is not None:
+            if not exact or name == pattern:
+                yield name
 
 
 class TwoWayNameMapping(_RegexMixin, LoggerMixin, _Generic[T]):
     """A class interface for managing two-way mappings."""
 
     def __init__(
         self,
@@ -108,18 +122,17 @@
         if isinstance(key, str):
             if key in self._reverse:
                 return key
 
         return self._mapping.get(_cast(T, key))
 
     @property
-    def names(self) -> _Iterator[str]:
+    def names(self) -> Iterator[str]:
         """Iterate over names."""
-        for name in self._reverse:
-            yield name
+        yield from self._reverse
 
     def asdict(self) -> _Dict[str, T]:
         """Provide a dictionary representation."""
         return self._reverse
 
     @classmethod
     def int_from_dict(
@@ -138,14 +151,18 @@
             if isinstance(key, str):
                 reverse[key] = int(value)
             else:
                 mapping[key] = str(value)
 
         return cls(mapping=mapping, reverse=reverse)
 
+    def search(self, pattern: str, exact: bool = False) -> Iterator[str]:
+        """Get names in this mapping based on a pattern."""
+        yield from name_search(self.names, pattern, exact=exact)
+
     @classmethod
     def bool_from_dict(
         cls: _Type[BoolMapping], data: BoolMappingData
     ) -> BoolMapping:
         """
         Create a boolean-to-name mapping from a dictionary with arbitrary data.
         """
```

### Comparing `runtimepy-3.8.0/runtimepy/metrics/channel.py` & `runtimepy-3.9.0/runtimepy/metrics/channel.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/metrics/connection.py` & `runtimepy-3.9.0/runtimepy/metrics/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/metrics/task.py` & `runtimepy-3.9.0/runtimepy/metrics/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/mixins/async_command.py` & `runtimepy-3.9.0/runtimepy/mixins/async_command.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 import asyncio
 from typing import Optional
 
 # third-party
 from vcorelib.logging import LoggerMixin
 
 # internal
-from runtimepy.channel.environment.command import (
+from runtimepy.channel.environment.command import FieldOrChannel
+from runtimepy.channel.environment.command.processor import (
     ChannelCommandProcessor,
-    FieldOrChannel,
 )
 
 ChannelCommandParams = tuple[Namespace, Optional[FieldOrChannel]]
 
 
 class AsyncCommandProcessingMixin(LoggerMixin, ABC):
     """A class mixin for handling asynchronous commands."""
```

### Comparing `runtimepy-3.8.0/runtimepy/mixins/enum.py` & `runtimepy-3.9.0/runtimepy/mixins/enum.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/mixins/environment.py` & `runtimepy-3.9.0/runtimepy/mixins/environment.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/mixins/finalize.py` & `runtimepy-3.9.0/runtimepy/mixins/finalize.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/mixins/logging.py` & `runtimepy-3.9.0/runtimepy/mixins/logging.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/mixins/regex.py` & `runtimepy-3.9.0/runtimepy/mixins/regex.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/__init__.py` & `runtimepy-3.9.0/runtimepy/net/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/apps/__init__.py` & `runtimepy-3.9.0/runtimepy/net/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/__init__.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/base.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/config.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/config.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/factory/connection.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/factory/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/factory/task.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/factory/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/housekeeping/__init__.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/housekeeping/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/imports.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/imports.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/info.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/info.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,25 @@
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.logging import LoggerType as _LoggerType
 from vcorelib.namespace import Namespace as _Namespace
 
 # internal
+from runtimepy.mapping import DEFAULT_PATTERN
 from runtimepy.net.arbiter.result import OverallResult, results
 from runtimepy.net.connection import Connection as _Connection
 from runtimepy.net.manager import ConnectionManager
 from runtimepy.task import PeriodicTask, PeriodicTaskManager
 from runtimepy.tui.mixin import TuiMixin
 
 ConnectionMap = _MutableMapping[str, _Connection]
 T = _TypeVar("T", bound=_Connection)
 V = _TypeVar("V", bound=PeriodicTask)
 
-DEFAULT_PATTERN = ".*"
-
 
 @dataclass
 class AppInfo:
     """References provided to network applications."""
 
     # A logger for applications to use.
     logger: _LoggerType
```

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/result.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/result.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/task.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/tcp/__init__.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/tcp/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/tcp/json.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/tcp/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/udp.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/udp.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/arbiter/websocket.py` & `runtimepy-3.9.0/runtimepy/net/arbiter/websocket.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/backoff.py` & `runtimepy-3.9.0/runtimepy/net/backoff.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/connection.py` & `runtimepy-3.9.0/runtimepy/net/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 # third-party
 from vcorelib.asyncio import log_exceptions as _log_exceptions
 from vcorelib.logging import LoggerType as _LoggerType
 
 # internal
 from runtimepy.channel.environment import ChannelEnvironment
-from runtimepy.channel.environment.command import ChannelCommandProcessor
+from runtimepy.channel.environment.command.processor import (
+    ChannelCommandProcessor,
+)
 from runtimepy.metrics import ConnectionMetrics
 from runtimepy.mixins.environment import ChannelEnvironmentMixin
 from runtimepy.mixins.logging import LoggerMixinLevelControl
 from runtimepy.net.backoff import ExponentialBackoff
 from runtimepy.primitives import Bool, Uint8
 from runtimepy.primitives.byte_order import DEFAULT_BYTE_ORDER, ByteOrder
```

### Comparing `runtimepy-3.8.0/runtimepy/net/factories/__init__.py` & `runtimepy-3.9.0/runtimepy/net/factories/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/http/__init__.py` & `runtimepy-3.9.0/runtimepy/net/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/http/common.py` & `runtimepy-3.9.0/runtimepy/net/http/common.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/http/header.py` & `runtimepy-3.9.0/runtimepy/net/http/header.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/http/request_target.py` & `runtimepy-3.9.0/runtimepy/net/http/request_target.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/http/response.py` & `runtimepy-3.9.0/runtimepy/net/http/response.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/http/state.py` & `runtimepy-3.9.0/runtimepy/net/http/state.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/http/version.py` & `runtimepy-3.9.0/runtimepy/net/http/version.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/manager.py` & `runtimepy-3.9.0/runtimepy/net/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/mixin.py` & `runtimepy-3.9.0/runtimepy/net/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/server/__init__.py` & `runtimepy-3.9.0/runtimepy/net/server/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/server/html.py` & `runtimepy-3.9.0/runtimepy/net/server/html.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/server/json.py` & `runtimepy-3.9.0/runtimepy/net/server/json.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/stream/__init__.py` & `runtimepy-3.9.0/runtimepy/net/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/stream/base.py` & `runtimepy-3.9.0/runtimepy/net/stream/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/stream/json/base.py` & `runtimepy-3.9.0/runtimepy/net/stream/json/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         """Register connection-specific command handlers."""
 
         # Extra handlers.
         self.typed_handler("find_file", FindFile, find_file_request_handler)
         self.typed_handler(
             "channel_command",
             ChannelCommand,
-            channel_env_handler(ENVIRONMENTS, self.command),
+            channel_env_handler(ENVIRONMENTS.data, self.command),
         )
 
     def init(self) -> None:
         """Initialize this instance."""
 
         super().init()
         self._setup_async_commands()
```

### Comparing `runtimepy-3.8.0/runtimepy/net/stream/json/handlers.py` & `runtimepy-3.9.0/runtimepy/net/stream/json/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 # third-party
 from vcorelib.dict import MergeStrategy
 from vcorelib.dict.codec import BasicDictCodec
 from vcorelib.io import ARBITER
 from vcorelib.paths import find_file
 
 # internal
-from runtimepy.channel.environment.command import ChannelCommandProcessor
+from runtimepy.channel.environment.command.processor import (
+    ChannelCommandProcessor,
+)
 from runtimepy.net.stream.json.types import JsonMessage, TypedHandler
 from runtimepy.schemas import RuntimepyDictCodec
 
 
 class ChannelCommand(RuntimepyDictCodec, BasicDictCodec):
     """A schema-validated find-file request."""
```

### Comparing `runtimepy-3.8.0/runtimepy/net/stream/json/types.py` & `runtimepy-3.9.0/runtimepy/net/stream/json/types.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/stream/string.py` & `runtimepy-3.9.0/runtimepy/net/stream/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/tcp/connection.py` & `runtimepy-3.9.0/runtimepy/net/tcp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/tcp/create.py` & `runtimepy-3.9.0/runtimepy/net/tcp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/tcp/http/__init__.py` & `runtimepy-3.9.0/runtimepy/net/tcp/http/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/tcp/protocol.py` & `runtimepy-3.9.0/runtimepy/net/tcp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/tcp/telnet/__init__.py` & `runtimepy-3.9.0/runtimepy/net/tcp/telnet/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/tcp/telnet/codes.py` & `runtimepy-3.9.0/runtimepy/net/tcp/telnet/codes.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/udp/connection.py` & `runtimepy-3.9.0/runtimepy/net/udp/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/udp/create.py` & `runtimepy-3.9.0/runtimepy/net/udp/create.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/udp/protocol.py` & `runtimepy-3.9.0/runtimepy/net/udp/protocol.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/util.py` & `runtimepy-3.9.0/runtimepy/net/util.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/net/websocket/connection.py` & `runtimepy-3.9.0/runtimepy/net/websocket/connection.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/__init__.py` & `runtimepy-3.9.0/runtimepy/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/array/__init__.py` & `runtimepy-3.9.0/runtimepy/primitives/array/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/base.py` & `runtimepy-3.9.0/runtimepy/primitives/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -103,29 +103,29 @@
 
     @value.setter
     def value(self, value: T) -> None:
         """Obtain the underlying value."""
 
         curr: T = self.raw.value  # type: ignore
 
+        self.raw.value = value
+        self.last_updated_ns = default_time_ns()
+
         # Call callbacks if the value has changed.
         if self.callbacks and curr != value:
             to_remove = []
             for ident, (callback, once) in self.callbacks.items():
                 callback(curr, value)
                 if once:
                     to_remove.append(ident)
 
             # Remove one-time callbacks.
             for item in to_remove:
                 self.remove_callback(item)
 
-        self.last_updated_ns = default_time_ns()
-        self.raw.value = value
-
     @property
     def scaled(self) -> Numeric:
         """Get this primitive as a scaled value."""
         return apply(self.value, scaling=self.scaling)
 
     @scaled.setter
     def scaled(self, value: T) -> None:
```

### Comparing `runtimepy-3.8.0/runtimepy/primitives/bool.py` & `runtimepy-3.9.0/runtimepy/primitives/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/byte_order.py` & `runtimepy-3.9.0/runtimepy/primitives/byte_order.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/field/__init__.py` & `runtimepy-3.9.0/runtimepy/primitives/field/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/field/fields.py` & `runtimepy-3.9.0/runtimepy/primitives/field/fields.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/field/manager/__init__.py` & `runtimepy-3.9.0/runtimepy/primitives/field/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/field/manager/base.py` & `runtimepy-3.9.0/runtimepy/primitives/field/manager/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/float.py` & `runtimepy-3.9.0/runtimepy/primitives/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/int.py` & `runtimepy-3.9.0/runtimepy/primitives/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/scaling.py` & `runtimepy-3.9.0/runtimepy/primitives/scaling.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/serializable/base.py` & `runtimepy-3.9.0/runtimepy/primitives/serializable/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/serializable/fixed.py` & `runtimepy-3.9.0/runtimepy/primitives/serializable/fixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/serializable/prefixed.py` & `runtimepy-3.9.0/runtimepy/primitives/serializable/prefixed.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/string.py` & `runtimepy-3.9.0/runtimepy/primitives/string.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/type/__init__.py` & `runtimepy-3.9.0/runtimepy/primitives/type/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/type/base.py` & `runtimepy-3.9.0/runtimepy/primitives/type/base.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/type/bool.py` & `runtimepy-3.9.0/runtimepy/primitives/type/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/type/bounds.py` & `runtimepy-3.9.0/runtimepy/primitives/type/bounds.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 
 class IntegerBounds(NamedTuple):
     """A container for integer bounds."""
 
     min: int
     max: int
 
+    def validate(self, val: int) -> bool:
+        """Determine if the value is within bounds."""
+        return self.min <= val <= self.max
+
     def clamp(self, val: int) -> int:
         """
         Ensure that 'val' is between min and max, use the min or max value
         instead of the provided value if it exceeds these bounds.
         """
 
         return max(self.min, min(val, self.max))
```

### Comparing `runtimepy-3.8.0/runtimepy/primitives/type/float.py` & `runtimepy-3.9.0/runtimepy/primitives/type/float.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/primitives/type/int.py` & `runtimepy-3.9.0/runtimepy/primitives/type/int.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/registry/__init__.py` & `runtimepy-3.9.0/runtimepy/registry/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 integer identifier.
 """
 
 # built-in
 from abc import abstractmethod as _abstractmethod
 from typing import Dict as _Dict
 from typing import Generic as _Generic
+from typing import Iterator
 from typing import Optional as _Optional
+from typing import Tuple
 from typing import Type as _Type
 from typing import TypeVar as _TypeVar
 from typing import cast as _cast
 
 # third-party
 from vcorelib.io.types import JsonObject as _JsonObject
 from vcorelib.io.types import JsonValue as _JsonValue
@@ -45,14 +47,22 @@
         }
 
         # Create the name registry.
         self.names = self.name_registry(
             reverse={name: item.id for name, item in self.items.items()}
         )
 
+    def search(
+        self, pattern: str, exact: bool = False
+    ) -> Iterator[Tuple[str, T]]:
+        """Search for items in the registry by name."""
+
+        for name in self.names.search(pattern, exact=exact):
+            yield name, self.items[name]
+
     def asdict(self) -> _JsonObject:
         """Get this registry as a dictionary."""
 
         return {
             name: _cast(_JsonValue, item.asdict())
             for name, item in self.items.items()
         }
```

### Comparing `runtimepy-3.8.0/runtimepy/registry/bool.py` & `runtimepy-3.9.0/runtimepy/registry/bool.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/registry/item.py` & `runtimepy-3.9.0/runtimepy/registry/item.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/registry/name.py` & `runtimepy-3.9.0/runtimepy/registry/name.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/schemas.py` & `runtimepy-3.9.0/runtimepy/schemas.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/task/asynchronous.py` & `runtimepy-3.9.0/runtimepy/task/asynchronous.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/task/basic/manager.py` & `runtimepy-3.9.0/runtimepy/task/basic/manager.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/task/basic/periodic.py` & `runtimepy-3.9.0/runtimepy/task/basic/periodic.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
 from vcorelib.math import DEFAULT_DEPTH as _DEFAULT_DEPTH
 from vcorelib.math import MovingAverage as _MovingAverage
 from vcorelib.math import RateTracker as _RateTracker
 from vcorelib.math import rate_str as _rate_str
 
 # internal
 from runtimepy.channel.environment import ChannelEnvironment
-from runtimepy.channel.environment.command import ChannelCommandProcessor
+from runtimepy.channel.environment.command.processor import (
+    ChannelCommandProcessor,
+)
 from runtimepy.metrics import PeriodicTaskMetrics
 from runtimepy.mixins.environment import ChannelEnvironmentMixin
 from runtimepy.mixins.logging import LoggerMixinLevelControl
 from runtimepy.primitives import Bool as _Bool
 from runtimepy.primitives import Double as _Double
 from runtimepy.primitives import Float as _Float
```

### Comparing `runtimepy-3.8.0/runtimepy/task/trig/__init__.py` & `runtimepy-3.9.0/runtimepy/task/trig/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/tui/channels/__init__.py` & `runtimepy-3.9.0/runtimepy/tui/channels/__init__.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/tui/cursor.py` & `runtimepy-3.9.0/runtimepy/tui/cursor.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/tui/mixin.py` & `runtimepy-3.9.0/runtimepy/tui/mixin.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/tui/mock.py` & `runtimepy-3.9.0/runtimepy/tui/mock.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy/tui/task.py` & `runtimepy-3.9.0/runtimepy/tui/task.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/runtimepy.egg-info/PKG-INFO` & `runtimepy-3.9.0/runtimepy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runtimepy
-Version: 3.8.0
+Version: 3.9.0
 Summary: A framework for implementing Python services.
 Home-page: https://github.com/vkottler/runtimepy
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,17 +13,17 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: svgen>=0.5.0
 Requires-Dist: vcorelib>=3.2.0
 Requires-Dist: websockets
-Requires-Dist: svgen>=0.5.0
 Provides-Extra: test
 Requires-Dist: pylint; extra == "test"
 Requires-Dist: flake8; extra == "test"
 Requires-Dist: black; extra == "test"
 Requires-Dist: ruff; extra == "test"
 Requires-Dist: mypy; extra == "test"
 Requires-Dist: isort; extra == "test"
@@ -37,19 +37,19 @@
 Requires-Dist: types-setuptools; extra == "test"
 Requires-Dist: uvloop; (sys_platform != "win32" and sys_platform != "cygwin") and extra == "test"
 
 <!--
     =====================================
     generator=datazen
     version=3.1.4
-    hash=d0656a2e337796f56cdb520895ea2f08
+    hash=c7bfaabcb235afbdae1921e1defa2f1a
     =====================================
 -->
 
-# runtimepy ([3.8.0](https://pypi.org/project/runtimepy/))
+# runtimepy ([3.9.0](https://pypi.org/project/runtimepy/))
 
 [![python](https://img.shields.io/pypi/pyversions/runtimepy.svg)](https://pypi.org/project/runtimepy/)
 ![Build Status](https://github.com/vkottler/runtimepy/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/runtimepy/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/runtimepy)
 ![PyPI - Status](https://img.shields.io/pypi/status/runtimepy)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/runtimepy)
```

### Comparing `runtimepy-3.8.0/runtimepy.egg-info/SOURCES.txt` & `runtimepy-3.9.0/runtimepy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,18 @@
 runtimepy/channel/environment/__init__.py
 runtimepy/channel/environment/array.py
 runtimepy/channel/environment/base.py
 runtimepy/channel/environment/create.py
 runtimepy/channel/environment/file.py
 runtimepy/channel/environment/command/__init__.py
 runtimepy/channel/environment/command/parser.py
+runtimepy/channel/environment/command/processor.py
 runtimepy/channel/environment/command/result.py
+runtimepy/channel/event/__init__.py
+runtimepy/channel/event/header.py
 runtimepy/codec/__init__.py
 runtimepy/codec/protocol/__init__.py
 runtimepy/codec/protocol/base.py
 runtimepy/codec/protocol/json.py
 runtimepy/codec/system/__init__.py
 runtimepy/commands/__init__.py
 runtimepy/commands/all.py
```

### Comparing `runtimepy-3.8.0/setup.py` & `runtimepy-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/tests/test_entry.py` & `runtimepy-3.9.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `runtimepy-3.8.0/tests/test_mapping.py` & `runtimepy-3.9.0/tests/test_mapping.py`

 * *Files identical despite different names*

