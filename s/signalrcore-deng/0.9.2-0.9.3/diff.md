# Comparing `tmp/signalrcore-deng-0.9.2.tar.gz` & `tmp/signalrcore-deng-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "signalrcore-deng-0.9.2.tar", last modified: Tue Jul 26 12:36:09 2022, max compression
+gzip compressed data, was "signalrcore-deng-0.9.3.tar", last modified: Wed Apr  3 02:35:31 2024, max compression
```

## Comparing `signalrcore-deng-0.9.2.tar` & `signalrcore-deng-0.9.3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:09.001752 signalrcore-deng-0.9.2/
--rw-rw-rw-   0        0        0     1101 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/LICENSE
--rw-rw-rw-   0        0        0       17 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/MANIFEST.in
--rw-rw-rw-   0        0        0    11150 2022-07-26 12:36:09.000752 signalrcore-deng-0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0    10262 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/README.md
--rw-rw-rw-   0        0        0       42 2022-07-26 12:36:09.001752 signalrcore-deng-0.9.2/setup.cfg
--rw-rw-rw-   0        0        0     1258 2022-07-26 12:35:18.000000 signalrcore-deng-0.9.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.955315 signalrcore-deng-0.9.2/signalrcore/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/__init__.py
--rw-rw-rw-   0        0        0     2855 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/helpers.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.959404 signalrcore-deng-0.9.2/signalrcore/hub/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/hub/__init__.py
--rw-rw-rw-   0        0        0      989 2021-11-11 03:30:19.000000 signalrcore-deng-0.9.2/signalrcore/hub/auth_hub_connection.py
--rw-rw-rw-   0        0        0     8934 2021-11-11 03:30:19.000000 signalrcore-deng-0.9.2/signalrcore/hub/base_hub_connection.py
--rw-rw-rw-   0        0        0      176 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/hub/errors.py
--rw-rw-rw-   0        0        0     1979 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/hub/handlers.py
--rw-rw-rw-   0        0        0     9934 2021-11-11 03:44:49.000000 signalrcore-deng-0.9.2/signalrcore/hub_connection_builder.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.969406 signalrcore-deng-0.9.2/signalrcore/messages/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/__init__.py
--rw-rw-rw-   0        0        0      447 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/base_message.py
--rw-rw-rw-   0        0        0      647 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/cancel_invocation_message.py
--rw-rw-rw-   0        0        0      716 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/close_message.py
--rw-rw-rw-   0        0        0     1952 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/completion_message.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.972407 signalrcore-deng-0.9.2/signalrcore/messages/handshake/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/handshake/__init__.py
--rw-rw-rw-   0        0        0      152 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/handshake/request.py
--rw-rw-rw-   0        0        0      103 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/handshake/response.py
--rw-rw-rw-   0        0        0     2086 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/invocation_message.py
--rw-rw-rw-   0        0        0      234 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/message_type.py
--rw-rw-rw-   0        0        0      403 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/ping_message.py
--rw-rw-rw-   0        0        0     1189 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/stream_invocation_message.py
--rw-rw-rw-   0        0        0      786 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/messages/stream_item_message.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.975908 signalrcore-deng-0.9.2/signalrcore/protocol/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/protocol/__init__.py
--rw-rw-rw-   0        0        0     2991 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/protocol/base_hub_protocol.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.976909 signalrcore-deng-0.9.2/signalrcore/protocol/handshake/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/protocol/handshake/__init__.py
--rw-rw-rw-   0        0        0     1704 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/protocol/json_hub_protocol.py
--rw-rw-rw-   0        0        0     6419 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/protocol/messagepack_protocol.py
--rw-rw-rw-   0        0        0     2180 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/subject.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.978907 signalrcore-deng-0.9.2/signalrcore/transport/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/transport/__init__.py
--rw-rw-rw-   0        0        0      997 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/transport/base_transport.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.982039 signalrcore-deng-0.9.2/signalrcore/transport/websockets/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/transport/websockets/__init__.py
--rw-rw-rw-   0        0        0      140 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/transport/websockets/connection.py
--rw-rw-rw-   0        0        0     2680 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/signalrcore/transport/websockets/reconnection.py
--rw-rw-rw-   0        0        0     9408 2021-11-11 03:44:49.000000 signalrcore-deng-0.9.2/signalrcore/transport/websockets/websocket_transport.py
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.991274 signalrcore-deng-0.9.2/signalrcore_deng.egg-info/
--rw-rw-rw-   0        0        0    11150 2022-07-26 12:36:08.000000 signalrcore-deng-0.9.2/signalrcore_deng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1762 2022-07-26 12:36:08.000000 signalrcore-deng-0.9.2/signalrcore_deng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-26 12:36:08.000000 signalrcore-deng-0.9.2/signalrcore_deng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2022-07-26 12:36:08.000000 signalrcore-deng-0.9.2/signalrcore_deng.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2022-07-26 12:36:08.000000 signalrcore-deng-0.9.2/signalrcore_deng.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-07-26 12:36:08.999752 signalrcore-deng-0.9.2/test/
--rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/__init__.py
--rw-rw-rw-   0        0        0     1892 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/base_test_case.py
--rw-rw-rw-   0        0        0     1033 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/client_streaming_test.py
--rw-rw-rw-   0        0        0     2225 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/configuration_test.py
--rw-rw-rw-   0        0        0     1629 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/open_close_test.py
--rw-rw-rw-   0        0        0     4131 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/reconnection_test.py
--rw-rw-rw-   0        0        0     1893 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/send_auth_errors_test.py
--rw-rw-rw-   0        0        0     2819 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/send_auth_test.py
--rw-rw-rw-   0        0        0     5354 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/send_test.py
--rw-rw-rw-   0        0        0     2044 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.2/test/streaming_test.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.273171 signalrcore-deng-0.9.3/
+-rw-rw-rw-   0        0        0     1101 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/LICENSE
+-rw-rw-rw-   0        0        0       17 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    11254 2024-04-03 02:35:31.271655 signalrcore-deng-0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10262 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 02:35:31.273171 signalrcore-deng-0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     1258 2024-04-03 02:33:34.000000 signalrcore-deng-0.9.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.196879 signalrcore-deng-0.9.3/signalrcore/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/__init__.py
+-rw-rw-rw-   0        0        0     2855 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/helpers.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.203451 signalrcore-deng-0.9.3/signalrcore/hub/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/hub/__init__.py
+-rw-rw-rw-   0        0        0      989 2021-11-11 03:30:19.000000 signalrcore-deng-0.9.3/signalrcore/hub/auth_hub_connection.py
+-rw-rw-rw-   0        0        0     8934 2021-11-11 03:30:19.000000 signalrcore-deng-0.9.3/signalrcore/hub/base_hub_connection.py
+-rw-rw-rw-   0        0        0      176 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/hub/errors.py
+-rw-rw-rw-   0        0        0     1979 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/hub/handlers.py
+-rw-rw-rw-   0        0        0     9934 2021-11-11 03:44:49.000000 signalrcore-deng-0.9.3/signalrcore/hub_connection_builder.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.220714 signalrcore-deng-0.9.3/signalrcore/messages/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/__init__.py
+-rw-rw-rw-   0        0        0      447 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/base_message.py
+-rw-rw-rw-   0        0        0      647 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/cancel_invocation_message.py
+-rw-rw-rw-   0        0        0      716 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/close_message.py
+-rw-rw-rw-   0        0        0     1952 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/completion_message.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.225978 signalrcore-deng-0.9.3/signalrcore/messages/handshake/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/handshake/__init__.py
+-rw-rw-rw-   0        0        0      152 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/handshake/request.py
+-rw-rw-rw-   0        0        0      103 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/handshake/response.py
+-rw-rw-rw-   0        0        0     2086 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/invocation_message.py
+-rw-rw-rw-   0        0        0      234 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/message_type.py
+-rw-rw-rw-   0        0        0      403 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/ping_message.py
+-rw-rw-rw-   0        0        0     1189 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/stream_invocation_message.py
+-rw-rw-rw-   0        0        0      786 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/messages/stream_item_message.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.232105 signalrcore-deng-0.9.3/signalrcore/protocol/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/protocol/__init__.py
+-rw-rw-rw-   0        0        0     2991 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/protocol/base_hub_protocol.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.234191 signalrcore-deng-0.9.3/signalrcore/protocol/handshake/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/protocol/handshake/__init__.py
+-rw-rw-rw-   0        0        0     1704 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/protocol/json_hub_protocol.py
+-rw-rw-rw-   0        0        0     6419 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/protocol/messagepack_protocol.py
+-rw-rw-rw-   0        0        0     2180 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/subject.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.237356 signalrcore-deng-0.9.3/signalrcore/transport/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/transport/__init__.py
+-rw-rw-rw-   0        0        0      997 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/transport/base_transport.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.243494 signalrcore-deng-0.9.3/signalrcore/transport/websockets/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/transport/websockets/__init__.py
+-rw-rw-rw-   0        0        0      140 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/transport/websockets/connection.py
+-rw-rw-rw-   0        0        0     2680 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/signalrcore/transport/websockets/reconnection.py
+-rw-rw-rw-   0        0        0     9582 2024-04-03 02:35:16.000000 signalrcore-deng-0.9.3/signalrcore/transport/websockets/websocket_transport.py
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.269618 signalrcore-deng-0.9.3/signalrcore_deng.egg-info/
+-rw-rw-rw-   0        0        0    11254 2024-04-03 02:35:31.000000 signalrcore-deng-0.9.3/signalrcore_deng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1762 2024-04-03 02:35:31.000000 signalrcore-deng-0.9.3/signalrcore_deng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 02:35:31.000000 signalrcore-deng-0.9.3/signalrcore_deng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-03 02:35:31.000000 signalrcore-deng-0.9.3/signalrcore_deng.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-03 02:35:31.000000 signalrcore-deng-0.9.3/signalrcore_deng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 02:35:31.268066 signalrcore-deng-0.9.3/test/
+-rw-rw-rw-   0        0        0        0 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/__init__.py
+-rw-rw-rw-   0        0        0     1892 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/base_test_case.py
+-rw-rw-rw-   0        0        0     1033 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/client_streaming_test.py
+-rw-rw-rw-   0        0        0     2225 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/configuration_test.py
+-rw-rw-rw-   0        0        0     1629 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/open_close_test.py
+-rw-rw-rw-   0        0        0     4131 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/reconnection_test.py
+-rw-rw-rw-   0        0        0     1893 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/send_auth_errors_test.py
+-rw-rw-rw-   0        0        0     2819 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/send_auth_test.py
+-rw-rw-rw-   0        0        0     5354 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/send_test.py
+-rw-rw-rw-   0        0        0     2044 2021-11-11 02:32:24.000000 signalrcore-deng-0.9.3/test/streaming_test.py
```

### Comparing `signalrcore-deng-0.9.2/LICENSE` & `signalrcore-deng-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/PKG-INFO` & `signalrcore-deng-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: signalrcore-deng
-Version: 0.9.2
+Version: 0.9.3
 Summary: 修改说明：1、fork原库，在原库的基础上修复了一些多线程相关的BUG；2、支持设置网络代码，方便fiddler等软件抓包；（仅项目自用，其余用途建议直接使用原库signalrcore的最新版）
 Home-page: https://github.com/mandrewcito/signalrcore
 Author: mandrewcito
 Author-email: anbaalo@gmail.com
 Keywords: signalr core client 3.1
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.22.0
+Requires-Dist: websocket-client==1.0.0
+Requires-Dist: msgpack==1.0.2
 
 # SignalR core client
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/mandrewcito/1)
 ![Pypi](https://img.shields.io/pypi/v/signalrcore.svg)
 [![Downloads](https://pepy.tech/badge/signalrcore/month)](https://pepy.tech/project/signalrcore/month)
 [![Downloads](https://pepy.tech/badge/signalrcore)](https://pepy.tech/project/signalrcore)
 ![Issues](https://img.shields.io/github/issues/mandrewcito/signalrcore.svg)
```

### Comparing `signalrcore-deng-0.9.2/README.md` & `signalrcore-deng-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/setup.py` & `signalrcore-deng-0.9.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="signalrcore-deng",
-    version="0.9.2",
+    version="0.9.3",
     author="mandrewcito",
     author_email="anbaalo@gmail.com",
     description="修改说明：1、fork原库，在原库的基础上修复了一些多线程相关的BUG；2、支持设置网络代码，方便fiddler等软件抓包；（仅项目自用，其余用途建议直接使用原库signalrcore的最新版）",
     keywords="signalr core client 3.1",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license_file="LICENSE",
```

### Comparing `signalrcore-deng-0.9.2/signalrcore/helpers.py` & `signalrcore-deng-0.9.3/signalrcore/helpers.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/hub/auth_hub_connection.py` & `signalrcore-deng-0.9.3/signalrcore/hub/auth_hub_connection.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/hub/base_hub_connection.py` & `signalrcore-deng-0.9.3/signalrcore/hub/base_hub_connection.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/hub/handlers.py` & `signalrcore-deng-0.9.3/signalrcore/hub/handlers.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/hub_connection_builder.py` & `signalrcore-deng-0.9.3/signalrcore/hub_connection_builder.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/messages/cancel_invocation_message.py` & `signalrcore-deng-0.9.3/signalrcore/messages/cancel_invocation_message.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/messages/close_message.py` & `signalrcore-deng-0.9.3/signalrcore/messages/close_message.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/messages/completion_message.py` & `signalrcore-deng-0.9.3/signalrcore/messages/completion_message.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/messages/invocation_message.py` & `signalrcore-deng-0.9.3/signalrcore/messages/invocation_message.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/messages/stream_invocation_message.py` & `signalrcore-deng-0.9.3/signalrcore/messages/stream_invocation_message.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/messages/stream_item_message.py` & `signalrcore-deng-0.9.3/signalrcore/messages/stream_item_message.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/protocol/base_hub_protocol.py` & `signalrcore-deng-0.9.3/signalrcore/protocol/base_hub_protocol.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/protocol/json_hub_protocol.py` & `signalrcore-deng-0.9.3/signalrcore/protocol/json_hub_protocol.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/protocol/messagepack_protocol.py` & `signalrcore-deng-0.9.3/signalrcore/protocol/messagepack_protocol.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/subject.py` & `signalrcore-deng-0.9.3/signalrcore/subject.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/transport/base_transport.py` & `signalrcore-deng-0.9.3/signalrcore/transport/base_transport.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/transport/websockets/reconnection.py` & `signalrcore-deng-0.9.3/signalrcore/transport/websockets/reconnection.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/signalrcore/transport/websockets/websocket_transport.py` & `signalrcore-deng-0.9.3/signalrcore/transport/websockets/websocket_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,24 +86,31 @@
             self.url,
             header=self.headers,
             on_message=self.on_message,
             on_error=self.on_socket_error,
             on_close=self.on_close,
             on_open=self.on_open,
             )
-            
+
         self._thread = threading.Thread(
             target=lambda: self._ws.run_forever(
-                sslopt={"cert_reqs": ssl.CERT_NONE} if not self.verify_ssl else {},
+                sslopt={
+                    "cert_reqs": ssl.CERT_NONE,
+                    "check_hostname": False,
+                    "ciphers": "DEFAULT:@SECLEVEL=0",
+                }
+                if not self.verify_ssl
+                else {},
                 ping_interval=self.ping_interval,
                 proxy_type=self.proxy_type,
                 http_proxy_host=self.http_proxy_host,
                 http_proxy_port=self.http_proxy_port,
                 skip_utf8_validation=self.skip_utf8_validation,
-            ))
+            )
+        )
         self._thread.daemon = True
         self._thread.start()
         return True
 
     def negotiate(self):
         negotiate_url = Helpers.get_negotiate_url(self.url)
         self.logger.debug("Negotiate url:{0}".format(negotiate_url))
```

### Comparing `signalrcore-deng-0.9.2/signalrcore_deng.egg-info/PKG-INFO` & `signalrcore-deng-0.9.3/signalrcore_deng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 Metadata-Version: 2.1
 Name: signalrcore-deng
-Version: 0.9.2
+Version: 0.9.3
 Summary: 修改说明：1、fork原库，在原库的基础上修复了一些多线程相关的BUG；2、支持设置网络代码，方便fiddler等软件抓包；（仅项目自用，其余用途建议直接使用原库signalrcore的最新版）
 Home-page: https://github.com/mandrewcito/signalrcore
 Author: mandrewcito
 Author-email: anbaalo@gmail.com
 Keywords: signalr core client 3.1
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: requests>=2.22.0
+Requires-Dist: websocket-client==1.0.0
+Requires-Dist: msgpack==1.0.2
 
 # SignalR core client
 [![Donate](https://img.shields.io/badge/Donate-PayPal-green.svg?logo=paypal&style=flat-square)](https://www.paypal.me/mandrewcito/1)
 ![Pypi](https://img.shields.io/pypi/v/signalrcore.svg)
 [![Downloads](https://pepy.tech/badge/signalrcore/month)](https://pepy.tech/project/signalrcore/month)
 [![Downloads](https://pepy.tech/badge/signalrcore)](https://pepy.tech/project/signalrcore)
 ![Issues](https://img.shields.io/github/issues/mandrewcito/signalrcore.svg)
```

### Comparing `signalrcore-deng-0.9.2/signalrcore_deng.egg-info/SOURCES.txt` & `signalrcore-deng-0.9.3/signalrcore_deng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/base_test_case.py` & `signalrcore-deng-0.9.3/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/client_streaming_test.py` & `signalrcore-deng-0.9.3/test/client_streaming_test.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/configuration_test.py` & `signalrcore-deng-0.9.3/test/configuration_test.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/open_close_test.py` & `signalrcore-deng-0.9.3/test/open_close_test.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/reconnection_test.py` & `signalrcore-deng-0.9.3/test/reconnection_test.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/send_auth_errors_test.py` & `signalrcore-deng-0.9.3/test/send_auth_errors_test.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/send_auth_test.py` & `signalrcore-deng-0.9.3/test/send_auth_test.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/send_test.py` & `signalrcore-deng-0.9.3/test/send_test.py`

 * *Files identical despite different names*

### Comparing `signalrcore-deng-0.9.2/test/streaming_test.py` & `signalrcore-deng-0.9.3/test/streaming_test.py`

 * *Files identical despite different names*

