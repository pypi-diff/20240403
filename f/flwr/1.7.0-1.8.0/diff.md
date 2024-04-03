# Comparing `tmp/flwr-1.7.0.tar.gz` & `tmp/flwr-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr-1.7.0.tar", max compression
+gzip compressed data, was "flwr-1.8.0.tar", max compression
```

## Comparing `flwr-1.7.0.tar` & `flwr-1.8.0.tar`

### file list

```diff
@@ -1,144 +1,212 @@
--rw-r--r--   0        0        0    11358 2024-02-05 12:22:46.511682 flwr-1.7.0/LICENSE
--rw-r--r--   0        0        0    12549 2024-02-05 12:22:46.511682 flwr-1.7.0/README.md
--rw-r--r--   0        0        0     5419 2024-02-05 12:22:46.863680 flwr-1.7.0/pyproject.toml
--rw-r--r--   0        0        0      981 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/__init__.py
--rw-r--r--   0        0        0     1111 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    19947 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8210 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     7435 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0     4211 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/flower.py
--rw-r--r--   0        0        0      735 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8226 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     6843 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      719 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     5900 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     4128 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0      874 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/middleware/__init__.py
--rw-r--r--   0        0        0      819 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/middleware/secure_aggregation/__init__.py
--rw-r--r--   0        0        0    20111 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/middleware/secure_aggregation/secaggplus_middleware.py
--rw-r--r--   0        0        0     1281 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/middleware/utils.py
--rw-r--r--   0        0        0     1819 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10310 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    11964 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     1023 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     2884 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     4799 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/configsrecord.py
--rw-r--r--   0        0        0     1263 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1329 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     2004 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2270 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     4135 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0     1847 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4783 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/metricsrecord.py
--rw-r--r--   0        0        0     2095 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     4413 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/parametersrecord.py
--rw-r--r--   0        0        0     2351 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/recordset.py
--rw-r--r--   0        0        0    13730 2024-02-05 12:22:46.871680 flwr-1.7.0/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    10856 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     3546 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     2979 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     1686 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3155 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    19643 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7683 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      667 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      870 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/driver/__init__.py
--rw-r--r--   0        0        0     7268 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/driver/app.py
--rw-r--r--   0        0        0     4009 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/driver/driver.py
--rw-r--r--   0        0        0     6126 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/driver/driver_client_proxy.py
--rw-r--r--   0        0        0     4585 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/driver/grpc_driver.py
--rw-r--r--   0        0        0      786 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/flower/__init__.py
--rw-r--r--   0        0        0      683 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3115 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     4670 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     3852 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     6182 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     7505 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2183 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2272 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     3937 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1377 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    25619 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2234 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0     1061 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      712 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     4553 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5956 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4695 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11779 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     2705 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     2823 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-02-05 12:22:46.875680 flwr-1.7.0/src/py/flwr/server/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     5886 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0     4904 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/history.py
--rw-r--r--   0        0        0    15965 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     1003 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/state/__init__.py
--rw-r--r--   0        0        0     7893 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/state/in_memory_state.py
--rw-r--r--   0        0        0    21203 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/state/sqlite_state.py
--rw-r--r--   0        0        0     5316 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/state/state.py
--rw-r--r--   0        0        0     1654 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/state/state_factory.py
--rw-r--r--   0        0        0     2096 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0     4877 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7217 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11684 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      908 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     4740 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0     1278 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13879 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    17062 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     9429 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     3376 2024-02-05 12:22:46.879680 flwr-1.7.0/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    14791 1970-01-01 00:00:00.000000 flwr-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-03 06:41:59.535801 flwr-1.8.0/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-03 06:41:59.535801 flwr-1.8.0/README.md
+-rw-r--r--   0        0        0     5843 2024-04-03 06:41:59.939810 flwr-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     2184 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0     4675 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/flower_toml.py
+-rw-r--r--   0        0        0      789 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5016 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1173 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      594 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3675 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      269 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/flower.toml.tpl
+-rw-r--r--   0        0        0      408 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      507 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      697 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0       30 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/requirements.numpy.txt.tpl
+-rw-r--r--   0        0        0      106 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/requirements.pytorch.txt.tpl
+-rw-r--r--   0        0        0      209 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/new/templates/app/requirements.tensorflow.txt.tpl
+-rw-r--r--   0        0        0      789 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     2300 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1187 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    26114 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-03 06:41:59.943810 flwr-1.8.0/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8636 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8717 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     8560 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2377 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    14482 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     1006 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2424 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2273 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    12385 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     3016 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11669 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     3546 2024-04-03 06:41:59.947810 flwr-1.8.0/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7782 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3115 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     4670 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4356 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     7571 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     9042 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2491 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    24302 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5271 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3450 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     7344 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      820 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0    10106 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0     4586 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5592 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-03 06:41:59.951810 flwr-1.8.0/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4761 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11818 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3036 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      731 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3273 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     6734 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12454 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0     9586 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    23985 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     6058 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0     2207 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/superlink/state/utils.py
+-rw-r--r--   0        0        0      913 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12547 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29038 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    19367 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-03 06:41:59.955810 flwr-1.8.0/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-03 06:41:59.959810 flwr-1.8.0/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15685 2024-04-03 06:41:59.959810 flwr-1.8.0/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15237 1970-01-01 00:00:00.000000 flwr-1.8.0/PKG-INFO
```

### Comparing `flwr-1.7.0/LICENSE` & `flwr-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/README.md` & `flwr-1.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # Flower: A Friendly Federated Learning Framework
 
 <p align="center">
-  <a href="https://flower.dev/">
-    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />
+  <a href="https://flower.ai/">
+    <img src="https://flower.ai/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />
   </a>
 </p>
 <p align="center">
-    <a href="https://flower.dev/">Website</a> |
-    <a href="https://flower.dev/blog">Blog</a> |
-    <a href="https://flower.dev/docs/">Docs</a> |
-    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |
-    <a href="https://flower.dev/join-slack">Slack</a>
+    <a href="https://flower.ai/">Website</a> |
+    <a href="https://flower.ai/blog">Blog</a> |
+    <a href="https://flower.ai/docs/">Docs</a> |
+    <a href="https://flower.ai/conf/flower-summit-2022">Conference</a> |
+    <a href="https://flower.ai/join-slack">Slack</a>
     <br /><br />
 </p>
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)
 ![Build](https://github.com/adap/flower/actions/workflows/framework.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/badge/flwr)](https://pepy.tech/project/flwr)
-[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)
+[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.ai/join-slack)
 
 Flower (`flwr`) is a framework for building federated learning systems. The
 design of Flower is based on a few guiding principles:
 
 - **Customizable**: Federated learning systems vary wildly from one use case to
   another. Flower allows for a wide range of different configurations depending
   on the needs of each individual use case.
 
 - **Extendable**: Flower originated from a research project at the University of
   Oxford, so it was built with AI research in mind. Many components can be
   extended and overridden to build new state-of-the-art systems.
 
 - **Framework-agnostic**: Different machine learning frameworks have different
   strengths. Flower can be used with any machine learning framework, for
-  example, [PyTorch](https://pytorch.org), [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [MLX](https://ml-explore.github.io/mlx/build/html/index.html), [XGBoost](https://xgboost.readthedocs.io/en/stable/), [Pandas](https://pandas.pydata.org/) for federated analytics, or even raw [NumPy](https://numpy.org/)
+  example, [PyTorch](https://pytorch.org), [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [MONAI](https://docs.monai.io/en/latest/index.html), [fastai](https://www.fast.ai/), [MLX](https://ml-explore.github.io/mlx/build/html/index.html), [XGBoost](https://xgboost.readthedocs.io/en/stable/), [Pandas](https://pandas.pydata.org/) for federated analytics, or even raw [NumPy](https://numpy.org/)
   for users who enjoy computing gradients by hand.
 
 - **Understandable**: Flower is written with maintainability in mind. The
   community is encouraged to both read and contribute to the codebase.
 
-Meet the Flower community on [flower.dev](https://flower.dev)!
+Meet the Flower community on [flower.ai](https://flower.ai)!
 
 ## Federated Learning Tutorial
 
 Flower's goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.
 
 0. **What is Federated Learning?**
 
@@ -69,27 +69,27 @@
 
 ## 30-Minute Federated Learning Tutorial
 
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/flower-in-30-minutes/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/flower-in-30-minutes/tutorial.ipynb))
 
 ## Documentation
 
-[Flower Docs](https://flower.dev/docs):
+[Flower Docs](https://flower.ai/docs):
 
-- [Installation](https://flower.dev/docs/framework/how-to-install-flower.html)
-- [Quickstart (TensorFlow)](https://flower.dev/docs/framework/tutorial-quickstart-tensorflow.html)
-- [Quickstart (PyTorch)](https://flower.dev/docs/framework/tutorial-quickstart-pytorch.html)
-- [Quickstart (Hugging Face)](https://flower.dev/docs/framework/tutorial-quickstart-huggingface.html)
-- [Quickstart (PyTorch Lightning)](https://flower.dev/docs/framework/tutorial-quickstart-pytorch-lightning.html)
-- [Quickstart (Pandas)](https://flower.dev/docs/framework/tutorial-quickstart-pandas.html)
-- [Quickstart (fastai)](https://flower.dev/docs/framework/tutorial-quickstart-fastai.html)
-- [Quickstart (JAX)](https://flower.dev/docs/framework/tutorial-quickstart-jax.html)
-- [Quickstart (scikit-learn)](https://flower.dev/docs/framework/tutorial-quickstart-scikitlearn.html)
-- [Quickstart (Android [TFLite])](https://flower.dev/docs/framework/tutorial-quickstart-android.html)
-- [Quickstart (iOS [CoreML])](https://flower.dev/docs/framework/tutorial-quickstart-ios.html)
+- [Installation](https://flower.ai/docs/framework/how-to-install-flower.html)
+- [Quickstart (TensorFlow)](https://flower.ai/docs/framework/tutorial-quickstart-tensorflow.html)
+- [Quickstart (PyTorch)](https://flower.ai/docs/framework/tutorial-quickstart-pytorch.html)
+- [Quickstart (Hugging Face)](https://flower.ai/docs/framework/tutorial-quickstart-huggingface.html)
+- [Quickstart (PyTorch Lightning)](https://flower.ai/docs/framework/tutorial-quickstart-pytorch-lightning.html)
+- [Quickstart (Pandas)](https://flower.ai/docs/framework/tutorial-quickstart-pandas.html)
+- [Quickstart (fastai)](https://flower.ai/docs/framework/tutorial-quickstart-fastai.html)
+- [Quickstart (JAX)](https://flower.ai/docs/framework/tutorial-quickstart-jax.html)
+- [Quickstart (scikit-learn)](https://flower.ai/docs/framework/tutorial-quickstart-scikitlearn.html)
+- [Quickstart (Android [TFLite])](https://flower.ai/docs/framework/tutorial-quickstart-android.html)
+- [Quickstart (iOS [CoreML])](https://flower.ai/docs/framework/tutorial-quickstart-ios.html)
 
 ## Flower Baselines
 
 Flower Baselines is a collection of community-contributed projects that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas. The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline!
 
 - [DASHA](https://github.com/adap/flower/tree/main/baselines/dasha)
 - [DepthFL](https://github.com/adap/flower/tree/main/baselines/depthfl)
@@ -97,65 +97,68 @@
 - [FedMeta](https://github.com/adap/flower/tree/main/baselines/fedmeta)
 - [FedMLB](https://github.com/adap/flower/tree/main/baselines/fedmlb)
 - [FedPer](https://github.com/adap/flower/tree/main/baselines/fedper)
 - [FedProx](https://github.com/adap/flower/tree/main/baselines/fedprox)
 - [FedNova](https://github.com/adap/flower/tree/main/baselines/fednova)
 - [HeteroFL](https://github.com/adap/flower/tree/main/baselines/heterofl)
 - [FedAvgM](https://github.com/adap/flower/tree/main/baselines/fedavgm)
+- [FedStar](https://github.com/adap/flower/tree/main/baselines/fedstar)
 - [FedWav2vec2](https://github.com/adap/flower/tree/main/baselines/fedwav2vec2)
 - [FjORD](https://github.com/adap/flower/tree/main/baselines/fjord)
 - [MOON](https://github.com/adap/flower/tree/main/baselines/moon)
 - [niid-Bench](https://github.com/adap/flower/tree/main/baselines/niid_bench)
 - [TAMUNA](https://github.com/adap/flower/tree/main/baselines/tamuna)
 - [FedVSSL](https://github.com/adap/flower/tree/main/baselines/fedvssl)
 - [FedXGBoost](https://github.com/adap/flower/tree/main/baselines/hfedxgboost)
 - [FedPara](https://github.com/adap/flower/tree/main/baselines/fedpara)
 - [FedAvg](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/fedavg_mnist)
 - [FedOpt](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/adaptive_federated_optimization)
 
-Please refer to the [Flower Baselines Documentation](https://flower.dev/docs/baselines/) for a detailed categorization of baselines and for additional info including:
-* [How to use Flower Baselines](https://flower.dev/docs/baselines/how-to-use-baselines.html)
-* [How to contribute a new Flower Baseline](https://flower.dev/docs/baselines/how-to-contribute-baselines.html)
+Please refer to the [Flower Baselines Documentation](https://flower.ai/docs/baselines/) for a detailed categorization of baselines and for additional info including:
+* [How to use Flower Baselines](https://flower.ai/docs/baselines/how-to-use-baselines.html)
+* [How to contribute a new Flower Baseline](https://flower.ai/docs/baselines/how-to-contribute-baselines.html)
 
 ## Flower Usage Examples
 
 Several code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).
 
 Quickstart examples:
 
 - [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart-tensorflow)
 - [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart-pytorch)
 - [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart-huggingface)
 - [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart-pytorch-lightning)
 - [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart-fastai)
 - [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart-pandas)
 - [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart-jax)
+- [Quickstart (MONAI)](https://github.com/adap/flower/tree/main/examples/quickstart-monai)
 - [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
-- [Quickstart (XGBoost)](https://github.com/adap/flower/tree/main/examples/xgboost-quickstart)
 - [Quickstart (Android [TFLite])](https://github.com/adap/flower/tree/main/examples/android)
 - [Quickstart (iOS [CoreML])](https://github.com/adap/flower/tree/main/examples/ios)
 - [Quickstart (MLX)](https://github.com/adap/flower/tree/main/examples/quickstart-mlx)
 - [Quickstart (XGBoost)](https://github.com/adap/flower/tree/main/examples/xgboost-quickstart)
 
 Other [examples](https://github.com/adap/flower/tree/main/examples):
 
 - [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded-devices)
 - [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch-from-centralized-to-federated)
 - [Vertical FL](https://github.com/adap/flower/tree/main/examples/vertical-fl)
 - [Federated Finetuning of OpenAI's Whisper](https://github.com/adap/flower/tree/main/examples/whisper-federated-finetuning)
-- [Comprehensive XGBoost](https://github.com/adap/flower/tree/main/examples/xgboost-comprehensive)
+- [Federated Finetuning of Large Language Model](https://github.com/adap/flower/tree/main/examples/fedllm-finetune)
+- [Federated Finetuning of a Vision Transformer](https://github.com/adap/flower/tree/main/examples/vit-finetune)
 - [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced-tensorflow)
 - [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced-pytorch)
 - Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation-pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation-tensorflow))
 - [Comprehensive Flower+XGBoost](https://github.com/adap/flower/tree/main/examples/xgboost-comprehensive)
 - [Flower through Docker Compose and with Grafana dashboard](https://github.com/adap/flower/tree/main/examples/flower-via-docker-compose)
+- [Flower with KaplanMeierFitter from the lifelines library](https://github.com/adap/flower/tree/main/examples/federated-kaplna-meier-fitter)
 
 ## Community
 
-Flower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.
+Flower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.ai/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.
 
 <a href="https://github.com/adap/flower/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=adap/flower" />
 </a>
 
 ## Citation
```

#### html2text {}

```diff
@@ -4,40 +4,40 @@
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
 actions/workflows/framework.yml/badge.svg) [![Downloads](https://
 static.pepy.tech/badge/flwr)](https://pepy.tech/project/flwr) [![Slack](https:/
-/img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack) Flower
+/img.shields.io/badge/Chat-Slack-red)](https://flower.ai/join-slack) Flower
 (`flwr`) is a framework for building federated learning systems. The design of
 Flower is based on a few guiding principles: - **Customizable**: Federated
 learning systems vary wildly from one use case to another. Flower allows for a
 wide range of different configurations depending on the needs of each
 individual use case. - **Extendable**: Flower originated from a research
 project at the University of Oxford, so it was built with AI research in mind.
 Many components can be extended and overridden to build new state-of-the-art
 systems. - **Framework-agnostic**: Different machine learning frameworks have
 different strengths. Flower can be used with any machine learning framework,
 for example, [PyTorch](https://pytorch.org), [TensorFlow](https://
 tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch
 Lightning](https://pytorchlightning.ai/), [scikit-learn](https://scikit-
 learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://
-tensorflow.org/lite/), [fastai](https://www.fast.ai/), [MLX](https://ml-
-explore.github.io/mlx/build/html/index.html), [XGBoost](https://
-xgboost.readthedocs.io/en/stable/), [Pandas](https://pandas.pydata.org/) for
-federated analytics, or even raw [NumPy](https://numpy.org/) for users who
-enjoy computing gradients by hand. - **Understandable**: Flower is written with
-maintainability in mind. The community is encouraged to both read and
-contribute to the codebase. Meet the Flower community on [flower.dev](https://
-flower.dev)! ## Federated Learning Tutorial Flower's goal is to make federated
-learning accessible to everyone. This series of tutorials introduces the
-fundamentals of federated learning and how to implement them in Flower. 0.
-**What is Federated Learning?** [![Open in Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+tensorflow.org/lite/), [MONAI](https://docs.monai.io/en/latest/index.html),
+[fastai](https://www.fast.ai/), [MLX](https://ml-explore.github.io/mlx/build/
+html/index.html), [XGBoost](https://xgboost.readthedocs.io/en/stable/),
+[Pandas](https://pandas.pydata.org/) for federated analytics, or even raw
+[NumPy](https://numpy.org/) for users who enjoy computing gradients by hand. -
+**Understandable**: Flower is written with maintainability in mind. The
+community is encouraged to both read and contribute to the codebase. Meet the
+Flower community on [flower.ai](https://flower.ai)! ## Federated Learning
+Tutorial Flower's goal is to make federated learning accessible to everyone.
+This series of tutorials introduces the fundamentals of federated learning and
+how to implement them in Flower. 0. **What is Federated Learning?** [![Open in
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial-
 series-what-is-federated-learning.ipynb) (or open the [Jupyter Notebook](https:
 //github.com/adap/flower/blob/main/doc/source/tutorial-series-what-is-
 federated-learning.ipynb)) 1. **An Introduction to Federated Learning** [![Open
 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial-
 series-get-started-with-flower-pytorch.ipynb) (or open the [Jupyter Notebook]
@@ -61,102 +61,106 @@
 tutorial-series-customize-the-client-pytorch.ipynb)) Stay tuned, more tutorials
 are coming soon. Topics include **Privacy and Security in Federated Learning**,
 and **Scaling Federated Learning**. ## 30-Minute Federated Learning Tutorial [!
 [Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/github/adap/flower/blob/main/examples/
 flower-in-30-minutes/tutorial.ipynb) (or open the [Jupyter Notebook](https://
 github.com/adap/flower/blob/main/examples/flower-in-30-minutes/tutorial.ipynb))
-## Documentation [Flower Docs](https://flower.dev/docs): - [Installation]
-(https://flower.dev/docs/framework/how-to-install-flower.html) - [Quickstart
-(TensorFlow)](https://flower.dev/docs/framework/tutorial-quickstart-
-tensorflow.html) - [Quickstart (PyTorch)](https://flower.dev/docs/framework/
+## Documentation [Flower Docs](https://flower.ai/docs): - [Installation](https:
+//flower.ai/docs/framework/how-to-install-flower.html) - [Quickstart
+(TensorFlow)](https://flower.ai/docs/framework/tutorial-quickstart-
+tensorflow.html) - [Quickstart (PyTorch)](https://flower.ai/docs/framework/
 tutorial-quickstart-pytorch.html) - [Quickstart (Hugging Face)](https://
-flower.dev/docs/framework/tutorial-quickstart-huggingface.html) - [Quickstart
-(PyTorch Lightning)](https://flower.dev/docs/framework/tutorial-quickstart-
-pytorch-lightning.html) - [Quickstart (Pandas)](https://flower.dev/docs/
+flower.ai/docs/framework/tutorial-quickstart-huggingface.html) - [Quickstart
+(PyTorch Lightning)](https://flower.ai/docs/framework/tutorial-quickstart-
+pytorch-lightning.html) - [Quickstart (Pandas)](https://flower.ai/docs/
 framework/tutorial-quickstart-pandas.html) - [Quickstart (fastai)](https://
-flower.dev/docs/framework/tutorial-quickstart-fastai.html) - [Quickstart (JAX)]
-(https://flower.dev/docs/framework/tutorial-quickstart-jax.html) - [Quickstart
-(scikit-learn)](https://flower.dev/docs/framework/tutorial-quickstart-
-scikitlearn.html) - [Quickstart (Android [TFLite])](https://flower.dev/docs/
+flower.ai/docs/framework/tutorial-quickstart-fastai.html) - [Quickstart (JAX)]
+(https://flower.ai/docs/framework/tutorial-quickstart-jax.html) - [Quickstart
+(scikit-learn)](https://flower.ai/docs/framework/tutorial-quickstart-
+scikitlearn.html) - [Quickstart (Android [TFLite])](https://flower.ai/docs/
 framework/tutorial-quickstart-android.html) - [Quickstart (iOS [CoreML])]
-(https://flower.dev/docs/framework/tutorial-quickstart-ios.html) ## Flower
+(https://flower.ai/docs/framework/tutorial-quickstart-ios.html) ## Flower
 Baselines Flower Baselines is a collection of community-contributed projects
 that reproduce the experiments performed in popular federated learning
 publications. Researchers can build on Flower Baselines to quickly evaluate new
 ideas. The Flower community loves contributions! Make your work more visible
 and enable others to build on it by contributing it as a baseline! - [DASHA]
 (https://github.com/adap/flower/tree/main/baselines/dasha) - [DepthFL](https://
 github.com/adap/flower/tree/main/baselines/depthfl) - [FedBN](https://
 github.com/adap/flower/tree/main/baselines/fedbn) - [FedMeta](https://
 github.com/adap/flower/tree/main/baselines/fedmeta) - [FedMLB](https://
 github.com/adap/flower/tree/main/baselines/fedmlb) - [FedPer](https://
 github.com/adap/flower/tree/main/baselines/fedper) - [FedProx](https://
 github.com/adap/flower/tree/main/baselines/fedprox) - [FedNova](https://
 github.com/adap/flower/tree/main/baselines/fednova) - [HeteroFL](https://
 github.com/adap/flower/tree/main/baselines/heterofl) - [FedAvgM](https://
-github.com/adap/flower/tree/main/baselines/fedavgm) - [FedWav2vec2](https://
+github.com/adap/flower/tree/main/baselines/fedavgm) - [FedStar](https://
+github.com/adap/flower/tree/main/baselines/fedstar) - [FedWav2vec2](https://
 github.com/adap/flower/tree/main/baselines/fedwav2vec2) - [FjORD](https://
 github.com/adap/flower/tree/main/baselines/fjord) - [MOON](https://github.com/
 adap/flower/tree/main/baselines/moon) - [niid-Bench](https://github.com/adap/
 flower/tree/main/baselines/niid_bench) - [TAMUNA](https://github.com/adap/
 flower/tree/main/baselines/tamuna) - [FedVSSL](https://github.com/adap/flower/
 tree/main/baselines/fedvssl) - [FedXGBoost](https://github.com/adap/flower/
 tree/main/baselines/hfedxgboost) - [FedPara](https://github.com/adap/flower/
 tree/main/baselines/fedpara) - [FedAvg](https://github.com/adap/flower/tree/
 main/baselines/flwr_baselines/flwr_baselines/publications/fedavg_mnist) -
 [FedOpt](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
 flwr_baselines/publications/adaptive_federated_optimization) Please refer to
-the [Flower Baselines Documentation](https://flower.dev/docs/baselines/) for a
+the [Flower Baselines Documentation](https://flower.ai/docs/baselines/) for a
 detailed categorization of baselines and for additional info including: * [How
-to use Flower Baselines](https://flower.dev/docs/baselines/how-to-use-
-baselines.html) * [How to contribute a new Flower Baseline](https://flower.dev/
+to use Flower Baselines](https://flower.ai/docs/baselines/how-to-use-
+baselines.html) * [How to contribute a new Flower Baseline](https://flower.ai/
 docs/baselines/how-to-contribute-baselines.html) ## Flower Usage Examples
 Several code examples show different usage scenarios of Flower (in combination
 with popular machine learning frameworks such as PyTorch or TensorFlow).
 Quickstart examples: - [Quickstart (TensorFlow)](https://github.com/adap/
 flower/tree/main/examples/quickstart-tensorflow) - [Quickstart (PyTorch)]
 (https://github.com/adap/flower/tree/main/examples/quickstart-pytorch) -
 [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/
 quickstart-huggingface) - [Quickstart (PyTorch Lightning)](https://github.com/
 adap/flower/tree/main/examples/quickstart-pytorch-lightning) - [Quickstart
 (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart-fastai)
 - [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/
 quickstart-pandas) - [Quickstart (JAX)](https://github.com/adap/flower/tree/
-main/examples/quickstart-jax) - [Quickstart (scikit-learn)](https://github.com/
-adap/flower/tree/main/examples/sklearn-logreg-mnist) - [Quickstart (XGBoost)]
-(https://github.com/adap/flower/tree/main/examples/xgboost-quickstart) -
+main/examples/quickstart-jax) - [Quickstart (MONAI)](https://github.com/adap/
+flower/tree/main/examples/quickstart-monai) - [Quickstart (scikit-learn)]
+(https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist) -
 [Quickstart (Android [TFLite])](https://github.com/adap/flower/tree/main/
 examples/android) - [Quickstart (iOS [CoreML])](https://github.com/adap/flower/
 tree/main/examples/ios) - [Quickstart (MLX)](https://github.com/adap/flower/
 tree/main/examples/quickstart-mlx) - [Quickstart (XGBoost)](https://github.com/
 adap/flower/tree/main/examples/xgboost-quickstart) Other [examples](https://
 github.com/adap/flower/tree/main/examples): - [Raspberry Pi & Nvidia Jetson
 Tutorial](https://github.com/adap/flower/tree/main/examples/embedded-devices) -
 [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/
 main/examples/pytorch-from-centralized-to-federated) - [Vertical FL](https://
 github.com/adap/flower/tree/main/examples/vertical-fl) - [Federated Finetuning
 of OpenAI's Whisper](https://github.com/adap/flower/tree/main/examples/whisper-
-federated-finetuning) - [Comprehensive XGBoost](https://github.com/adap/flower/
-tree/main/examples/xgboost-comprehensive) - [Advanced Flower with TensorFlow/
-Keras](https://github.com/adap/flower/tree/main/examples/advanced-tensorflow) -
-[Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/
-examples/advanced-pytorch) - Single-Machine Simulation of Federated Learning
-Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/
-simulation-pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/
-examples/simulation-tensorflow)) - [Comprehensive Flower+XGBoost](https://
-github.com/adap/flower/tree/main/examples/xgboost-comprehensive) - [Flower
-through Docker Compose and with Grafana dashboard](https://github.com/adap/
-flower/tree/main/examples/flower-via-docker-compose) ## Community Flower is
-built by a wonderful community of researchers and engineers. [Join Slack]
-(https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-
-flower) are welcome. _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_a_d_a_p_/_f_l_o_w_e_r_]## Citation
-If you publish work that uses Flower, please cite Flower as follows: ```bibtex
-@article{beutel2020flower, title={Flower: A Friendly Federated Learning
-Research Framework}, author={Beutel, Daniel J and Topal, Taner and Mathur,
-Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani,
-Lorenzo and Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o, Pedro PB de and
-Lane, Nicholas D}, journal={arXiv preprint arXiv:2007.14390}, year={2020} } ```
-Please also consider adding your publication to the list of Flower-based
-publications in the docs, just open a Pull Request. ## Contributing to Flower
-We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get
-started!
+federated-finetuning) - [Federated Finetuning of Large Language Model](https://
+github.com/adap/flower/tree/main/examples/fedllm-finetune) - [Federated
+Finetuning of a Vision Transformer](https://github.com/adap/flower/tree/main/
+examples/vit-finetune) - [Advanced Flower with TensorFlow/Keras](https://
+github.com/adap/flower/tree/main/examples/advanced-tensorflow) - [Advanced
+Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/
+advanced-pytorch) - Single-Machine Simulation of Federated Learning Systems (
+[PyTorch](https://github.com/adap/flower/tree/main/examples/simulation-
+pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/
+simulation-tensorflow)) - [Comprehensive Flower+XGBoost](https://github.com/
+adap/flower/tree/main/examples/xgboost-comprehensive) - [Flower through Docker
+Compose and with Grafana dashboard](https://github.com/adap/flower/tree/main/
+examples/flower-via-docker-compose) - [Flower with KaplanMeierFitter from the
+lifelines library](https://github.com/adap/flower/tree/main/examples/federated-
+kaplna-meier-fitter) ## Community Flower is built by a wonderful community of
+researchers and engineers. [Join Slack](https://flower.ai/join-slack) to meet
+them, [contributions](#contributing-to-flower) are welcome. _[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_a_d_a_p_/_f_l_o_w_e_r_]## Citation If you publish work that uses
+Flower, please cite Flower as follows: ```bibtex @article{beutel2020flower,
+title={Flower: A Friendly Federated Learning Research Framework}, author=
+{Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and
+Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and
+Parcollet, Titouan and GusmÃ£o, Pedro PB de and Lane, Nicholas D}, journal=
+{arXiv preprint arXiv:2007.14390}, year={2020} } ``` Please also consider
+adding your publication to the list of Flower-based publications in the docs,
+just open a Pull Request. ## Contributing to Flower We welcome contributions.
+Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!
```

### Comparing `flwr-1.7.0/pyproject.toml` & `flwr-1.8.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr"
-version = "1.7.0"
+version = "1.8.0"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
-authors = ["The Flower Authors <hello@flower.dev>"]
+authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
-homepage = "https://flower.dev"
+homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
-documentation = "https://flower.dev"
+documentation = "https://flower.ai"
 keywords = [
     "flower",
     "fl",
     "federated learning",
     "federated analytics",
     "federated evaluation",
     "machine learning",
@@ -48,29 +48,34 @@
     { include = "flwr", from = "src/py" },
 ]
 exclude = [
     "src/py/**/*_test.py",
 ]
 
 [tool.poetry.scripts]
+flwr = "flwr.cli.app:app"
 flower-driver-api = "flwr.server:run_driver_api"
 flower-fleet-api = "flwr.server:run_fleet_api"
-flower-server = "flwr.server:run_server"
-flower-client = "flwr.client:run_client"
+flower-superlink = "flwr.server:run_superlink"
+flower-client-app = "flwr.client:run_client_app"
+flower-server-app = "flwr.server:run_server_app"
+flower-simulation = "flwr.simulation:run_simulation_from_cli"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 # Mandatory dependencies
 numpy = "^1.21.0"
 grpcio = "^1.60.0"
 protobuf = "^4.25.2"
-cryptography = "^41.0.2"
+cryptography = "^42.0.4"
 pycryptodome = "^3.18.0"
 iterators = "^0.0.2"
-# Optional dependencies (VCE)
+typer = { version = "^0.9.0", extras=["all"] }
+tomli = "^2.0.1"
+# Optional dependencies (Simulation Engine)
 ray = { version = "==2.6.3", optional = true }
 pydantic = { version = "<2.0.0", optional = true }
 # Optional dependencies (REST transport layer)
 requests = { version = "^2.31.0", optional = true }
 starlette = { version = "^0.31.0", optional = true }
 uvicorn = { version = "^0.23.0", extras = ["standard"], optional = true }
 
@@ -81,22 +86,22 @@
 [tool.poetry.group.dev.dependencies]
 types-dataclasses = "==0.6.6"
 types-protobuf = "==3.19.18"
 types-requests = "==2.31.0.20240125"
 types-setuptools = "==69.0.0.20240125"
 clang-format = "==17.0.6"
 isort = "==5.13.2"
-black = { version = "==23.10.1", extras = ["jupyter"] }
+black = { version = "==24.2.0", extras = ["jupyter"] }
 docformatter = "==1.7.5"
 mypy = "==1.8.0"
 pylint = "==3.0.3"
 flake8 = "==5.0.4"
 pytest = "==7.4.4"
 pytest-cov = "==4.1.0"
-pytest-watch = "==4.2.0"
+pytest-watcher = "==0.4.1"
 grpcio-tools = "==1.60.0"
 mypy-protobuf = "==3.2.0"
 jupyterlab = "==4.0.12"
 rope = "==1.11.0"
 semver = "==3.0.2"
 sphinx = "==6.2.1"
 sphinx-intl = "==2.1.0"
@@ -118,14 +123,15 @@
 mdformat-myst = "==0.1.5"
 twine = "==4.0.2"
 pyroma = "==4.2"
 check-wheel-contents = "==0.4.0"
 GitPython = "==3.1.32"
 PyGithub = "==2.1.1"
 licensecheck = "==2024"
+pre-commit = "==3.5.0"
 
 [tool.isort]
 line_length = 88
 indent = "    "
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
@@ -142,25 +148,34 @@
 [tool.pytest.ini_options]
 minversion = "6.2"
 addopts = "-qq"
 testpaths = [
     "src/py/flwr",
     "src/py/flwr_tool",
 ]
+filterwarnings = "ignore::DeprecationWarning"
+
+[tool.pytest-watcher]
+now = false
+clear = true
+delay = 0.2
+runner = "pytest"
+runner_args = ["-s", "-vvvvv"]
+patterns = ["*.py"]
+ignore_patterns = []
 
 [tool.mypy]
 plugins = [
     "numpy.typing.mypy_plugin",
 ]
 ignore_missing_imports = true
 strict = true
 
 [[tool.mypy.overrides]]
 module = [
-    "flwr_example.*",
     "flwr_experimental.*",
 ]
 ignore_errors = true
 
 [[tool.mypy.overrides]]
 module = [
     "importlib.metadata.*",
```

### Comparing `flwr-1.7.0/src/py/flwr/__init__.py` & `flwr-1.8.0/src/py/flwr/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,19 +13,17 @@
 # limitations under the License.
 # ==============================================================================
 """Flower main package."""
 
 
 from flwr.common.version import package_version as _package_version
 
-from . import client, common, driver, flower, server, simulation
+from . import client, common, server, simulation
 
 __all__ = [
     "client",
     "common",
-    "driver",
-    "flower",
     "server",
     "simulation",
 ]
 
 __version__ = _package_version
```

### Comparing `flwr-1.7.0/src/py/flwr/client/__init__.py` & `flwr-1.8.0/src/py/flwr/client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client."""
 
 
-from .app import run_client as run_client
+from .app import run_client_app as run_client_app
 from .app import start_client as start_client
 from .app import start_numpy_client as start_numpy_client
 from .client import Client as Client
+from .client_app import ClientApp as ClientApp
 from .numpy_client import NumPyClient as NumPyClient
 from .typing import ClientFn as ClientFn
 
 __all__ = [
     "Client",
+    "ClientApp",
     "ClientFn",
     "NumPyClient",
-    "run_client",
+    "run_client_app",
     "start_client",
     "start_numpy_client",
 ]
```

### Comparing `flwr-1.7.0/src/py/flwr/client/app.py` & `flwr-1.8.0/src/py/flwr/client/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,52 +10,56 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower client app."""
 
-
 import argparse
 import sys
 import time
-from logging import DEBUG, INFO, WARN
+from logging import DEBUG, ERROR, INFO, WARN
 from pathlib import Path
-from typing import Callable, ContextManager, Optional, Tuple, Union
+from typing import Callable, ContextManager, Optional, Tuple, Type, Union
+
+from grpc import RpcError
 
 from flwr.client.client import Client
-from flwr.client.flower import Flower
+from flwr.client.client_app import ClientApp, LoadClientAppError
 from flwr.client.typing import ClientFn
-from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
+from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, Message, event
 from flwr.common.address import parse_address
 from flwr.common.constant import (
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_BIDI,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
     TRANSPORT_TYPES,
+    ErrorCode,
 )
-from flwr.common.logger import log, warn_deprecated_feature, warn_experimental_feature
-from flwr.common.message import Message
+from flwr.common.exit_handlers import register_exit_handlers
+from flwr.common.logger import log, warn_deprecated_feature
+from flwr.common.message import Error
+from flwr.common.object_ref import load_app, validate
+from flwr.common.retry_invoker import RetryInvoker, exponential
 
-from .flower import load_flower_callable
 from .grpc_client.connection import grpc_connection
 from .grpc_rere_client.connection import grpc_request_response
 from .message_handler.message_handler import handle_control_message
 from .node_state import NodeState
 from .numpy_client import NumPyClient
 
 
-def run_client() -> None:
-    """Run Flower client."""
-    event(EventType.RUN_CLIENT_ENTER)
+def run_client_app() -> None:
+    """Run Flower client app."""
+    event(EventType.RUN_CLIENT_APP_ENTER)
 
     log(INFO, "Long-running Flower client starting")
 
-    args = _parse_args_client().parse_args()
+    args = _parse_args_run_client_app().parse_args()
 
     # Obtain certificates
     if args.insecure:
         if args.root_certificates is not None:
             sys.exit(
                 "Conflicting options: The '--insecure' flag disables HTTPS, "
                 "but '--root-certificates' was also specified. Please remove "
@@ -82,45 +86,58 @@
             "with the following certificates: %s.",
             args.server,
             cert_path,
         )
 
     log(
         DEBUG,
-        "The Flower client uses `%s` to execute tasks",
-        args.callable,
+        "Flower will load ClientApp `%s`",
+        getattr(args, "client-app"),
     )
 
-    callable_dir = args.dir
-    if callable_dir is not None:
-        sys.path.insert(0, callable_dir)
+    client_app_dir = args.dir
+    if client_app_dir is not None:
+        sys.path.insert(0, client_app_dir)
+
+    app_ref: str = getattr(args, "client-app")
+    valid, error_msg = validate(app_ref)
+    if not valid and error_msg:
+        raise LoadClientAppError(error_msg) from None
+
+    def _load() -> ClientApp:
+        client_app = load_app(app_ref, LoadClientAppError)
 
-    def _load() -> Flower:
-        flower: Flower = load_flower_callable(args.callable)
-        return flower
+        if not isinstance(client_app, ClientApp):
+            raise LoadClientAppError(
+                f"Attribute {app_ref} is not of type {ClientApp}",
+            ) from None
+
+        return client_app
 
     _start_client_internal(
         server_address=args.server,
-        load_flower_callable_fn=_load,
+        load_client_app_fn=_load,
         transport="rest" if args.rest else "grpc-rere",
         root_certificates=root_certificates,
         insecure=args.insecure,
+        max_retries=args.max_retries,
+        max_wait_time=args.max_wait_time,
     )
-    event(EventType.RUN_CLIENT_LEAVE)
+    register_exit_handlers(event_type=EventType.RUN_CLIENT_APP_LEAVE)
 
 
-def _parse_args_client() -> argparse.ArgumentParser:
-    """Parse command line arguments."""
+def _parse_args_run_client_app() -> argparse.ArgumentParser:
+    """Parse flower-client-app command line arguments."""
     parser = argparse.ArgumentParser(
-        description="Start a long-running Flower client",
+        description="Start a Flower client app",
     )
 
     parser.add_argument(
-        "callable",
-        help="For example: `client:flower` or `project.package.module:wrapper.flower`",
+        "client-app",
+        help="For example: `client:app` or `project.package.module:wrapper.app`",
     )
     parser.add_argument(
         "--insecure",
         action="store_true",
         help="Run the client without HTTPS. By default, the client runs with "
         "HTTPS enabled. Use this flag only if you understand the risks.",
     )
@@ -138,18 +155,34 @@
     )
     parser.add_argument(
         "--server",
         default="0.0.0.0:9092",
         help="Server address",
     )
     parser.add_argument(
+        "--max-retries",
+        type=int,
+        default=None,
+        help="The maximum number of times the client will try to connect to the"
+        "server before giving up in case of a connection error. By default,"
+        "it is set to None, meaning there is no limit to the number of tries.",
+    )
+    parser.add_argument(
+        "--max-wait-time",
+        type=float,
+        default=None,
+        help="The maximum duration before the client stops trying to"
+        "connect to the server in case of connection error. By default, it"
+        "is set to None, meaning there is no limit to the total time.",
+    )
+    parser.add_argument(
         "--dir",
         default="",
         help="Add specified directory to the PYTHONPATH and load Flower "
-        "callable from there."
+        "app from there."
         " Default: current working directory.",
     )
 
     return parser
 
 
 def _check_actionable_client(
@@ -176,14 +209,16 @@
     server_address: str,
     client_fn: Optional[ClientFn] = None,
     client: Optional[Client] = None,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
     insecure: Optional[bool] = None,
     transport: Optional[str] = None,
+    max_retries: Optional[int] = None,
+    max_wait_time: Optional[float] = None,
 ) -> None:
     """Start a Flower client node which connects to a Flower server.
 
     Parameters
     ----------
     server_address : str
         The IPv4 or IPv6 address of the server. If the Flower
@@ -209,14 +244,22 @@
         Starts an insecure gRPC connection when True. Enables HTTPS connection
         when False, using system certificates if `root_certificates` is None.
     transport : Optional[str] (default: None)
         Configure the transport layer. Allowed values:
         - 'grpc-bidi': gRPC, bidirectional streaming
         - 'grpc-rere': gRPC, request-response (experimental)
         - 'rest': HTTP (experimental)
+    max_retries: Optional[int] (default: None)
+        The maximum number of times the client will try to connect to the
+        server before giving up in case of a connection error. If set to None,
+        there is no limit to the number of tries.
+    max_wait_time: Optional[float] (default: None)
+        The maximum duration before the client stops trying to
+        connect to the server in case of connection error.
+        If set to None, there is no limit to the total time.
 
     Examples
     --------
     Starting a gRPC client with an insecure server connection:
 
     >>> start_client(
     >>>     server_address=localhost:8080,
@@ -243,50 +286,54 @@
     >>>     client_fn=client_fn,
     >>>     root_certificates=Path("/crts/root.pem").read_bytes(),
     >>> )
     """
     event(EventType.START_CLIENT_ENTER)
     _start_client_internal(
         server_address=server_address,
-        load_flower_callable_fn=None,
+        load_client_app_fn=None,
         client_fn=client_fn,
         client=client,
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
         insecure=insecure,
         transport=transport,
+        max_retries=max_retries,
+        max_wait_time=max_wait_time,
     )
     event(EventType.START_CLIENT_LEAVE)
 
 
 # pylint: disable=import-outside-toplevel
 # pylint: disable=too-many-branches
 # pylint: disable=too-many-locals
 # pylint: disable=too-many-statements
 def _start_client_internal(
     *,
     server_address: str,
-    load_flower_callable_fn: Optional[Callable[[], Flower]] = None,
+    load_client_app_fn: Optional[Callable[[], ClientApp]] = None,
     client_fn: Optional[ClientFn] = None,
     client: Optional[Client] = None,
     grpc_max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
     insecure: Optional[bool] = None,
     transport: Optional[str] = None,
+    max_retries: Optional[int] = None,
+    max_wait_time: Optional[float] = None,
 ) -> None:
     """Start a Flower client node which connects to a Flower server.
 
     Parameters
     ----------
     server_address : str
         The IPv4 or IPv6 address of the server. If the Flower
         server runs on the same machine on port 8080, then `server_address`
         would be `"[::]:8080"`.
-    load_flower_callable_fn : Optional[Callable[[], Flower]] (default: None)
-        A function that can be used to load a `Flower` callable instance.
+    load_client_app_fn : Optional[Callable[[], ClientApp]] (default: None)
+        A function that can be used to load a `ClientApp` instance.
     client_fn : Optional[ClientFn]
         A callable that instantiates a Client. (default: None)
     client : Optional[flwr.client.Client]
         An implementation of the abstract base
         class `flwr.client.Client` (default: None)
     grpc_max_message_length : int (default: 536_870_912, this equals 512MB)
         The maximum length of gRPC messages that can be exchanged with the
@@ -295,27 +342,35 @@
         value. Note that the Flower server needs to be started with the
         same value (see `flwr.server.start_server`), otherwise it will not
         know about the increased limit and block larger messages.
     root_certificates : Optional[Union[bytes, str]] (default: None)
         The PEM-encoded root certificates as a byte string or a path string.
         If provided, a secure connection using the certificates will be
         established to an SSL-enabled Flower server.
-    insecure : bool (default: True)
+    insecure : Optional[bool] (default: None)
         Starts an insecure gRPC connection when True. Enables HTTPS connection
         when False, using system certificates if `root_certificates` is None.
     transport : Optional[str] (default: None)
         Configure the transport layer. Allowed values:
         - 'grpc-bidi': gRPC, bidirectional streaming
         - 'grpc-rere': gRPC, request-response (experimental)
         - 'rest': HTTP (experimental)
+    max_retries: Optional[int] (default: None)
+        The maximum number of times the client will try to connect to the
+        server before giving up in case of a connection error. If set to None,
+        there is no limit to the number of tries.
+    max_wait_time: Optional[float] (default: None)
+        The maximum duration before the client stops trying to
+        connect to the server in case of connection error.
+        If set to None, there is no limit to the total time.
     """
     if insecure is None:
         insecure = root_certificates is None
 
-    if load_flower_callable_fn is None:
+    if load_client_app_fn is None:
         _check_actionable_client(client, client_fn)
 
         if client_fn is None:
             # Wrap `Client` instance in `client_fn`
             def single_client_factory(
                 cid: str,  # pylint: disable=unused-argument
             ) -> Client:
@@ -323,34 +378,71 @@
                     raise ValueError(
                         "Both `client_fn` and `client` are `None`, but one is required"
                     )
                 return client  # Always return the same instance
 
             client_fn = single_client_factory
 
-        def _load_app() -> Flower:
-            return Flower(client_fn=client_fn)
+        def _load_client_app() -> ClientApp:
+            return ClientApp(client_fn=client_fn)
 
-        load_flower_callable_fn = _load_app
-    else:
-        warn_experimental_feature("`load_flower_callable_fn`")
+        load_client_app_fn = _load_client_app
 
-    # At this point, only `load_flower_callable_fn` should be used
+    # At this point, only `load_client_app_fn` should be used
     # Both `client` and `client_fn` must not be used directly
 
     # Initialize connection context manager
-    connection, address = _init_connection(transport, server_address)
+    connection, address, connection_error_type = _init_connection(
+        transport, server_address
+    )
+
+    retry_invoker = RetryInvoker(
+        wait_gen_factory=exponential,
+        recoverable_exceptions=connection_error_type,
+        max_tries=max_retries,
+        max_time=max_wait_time,
+        on_giveup=lambda retry_state: (
+            log(
+                WARN,
+                "Giving up reconnection after %.2f seconds and %s tries.",
+                retry_state.elapsed_time,
+                retry_state.tries,
+            )
+            if retry_state.tries > 1
+            else None
+        ),
+        on_success=lambda retry_state: (
+            log(
+                INFO,
+                "Connection successful after %.2f seconds and %s tries.",
+                retry_state.elapsed_time,
+                retry_state.tries,
+            )
+            if retry_state.tries > 1
+            else None
+        ),
+        on_backoff=lambda retry_state: (
+            log(WARN, "Connection attempt failed, retrying...")
+            if retry_state.tries == 1
+            else log(
+                DEBUG,
+                "Connection attempt failed, retrying in %.2f seconds",
+                retry_state.actual_wait,
+            )
+        ),
+    )
 
     node_state = NodeState()
 
     while True:
         sleep_duration: int = 0
         with connection(
             address,
             insecure,
+            retry_invoker,
             grpc_max_message_length,
             root_certificates,
         ) as conn:
             receive, send, create_node, delete_node = conn
 
             # Register node
             if create_node is not None:
@@ -359,40 +451,91 @@
             while True:
                 # Receive
                 message = receive()
                 if message is None:
                     time.sleep(3)  # Wait for 3s before asking again
                     continue
 
+                log(INFO, "")
+                log(
+                    INFO,
+                    "[RUN %s, ROUND %s]",
+                    message.metadata.run_id,
+                    message.metadata.group_id,
+                )
+                log(
+                    INFO,
+                    "Received: %s message %s",
+                    message.metadata.message_type,
+                    message.metadata.message_id,
+                )
+
                 # Handle control message
                 out_message, sleep_duration = handle_control_message(message)
                 if out_message:
                     send(out_message)
                     break
 
                 # Register context for this run
                 node_state.register_context(run_id=message.metadata.run_id)
 
                 # Retrieve context for this run
                 context = node_state.retrieve_context(run_id=message.metadata.run_id)
 
-                # Load app
-                app: Flower = load_flower_callable_fn()
-
-                # Handle task message
-                out_message = app(message=message, context=context)
-
-                # Update node state
-                node_state.update_context(
-                    run_id=message.metadata.run_id,
-                    context=context,
+                # Create an error reply message that will never be used to prevent
+                # the used-before-assignment linting error
+                reply_message = message.create_error_reply(
+                    error=Error(code=ErrorCode.UNKNOWN, reason="Unknown")
                 )
 
+                # Handle app loading and task message
+                try:
+                    # Load ClientApp instance
+                    client_app: ClientApp = load_client_app_fn()
+
+                    # Execute ClientApp
+                    reply_message = client_app(message=message, context=context)
+                except Exception as ex:  # pylint: disable=broad-exception-caught
+
+                    # Legacy grpc-bidi
+                    if transport in ["grpc-bidi", None]:
+                        log(ERROR, "Client raised an exception.", exc_info=ex)
+                        # Raise exception, crash process
+                        raise ex
+
+                    # Don't update/change NodeState
+
+                    e_code = ErrorCode.CLIENT_APP_RAISED_EXCEPTION
+                    # Reason example: "<class 'ZeroDivisionError'>:<'division by zero'>"
+                    reason = str(type(ex)) + ":<'" + str(ex) + "'>"
+                    exc_entity = "ClientApp"
+                    if isinstance(ex, LoadClientAppError):
+                        reason = (
+                            "An exception was raised when attempting to load "
+                            "`ClientApp`"
+                        )
+                        e_code = ErrorCode.LOAD_CLIENT_APP_EXCEPTION
+                        exc_entity = "SuperNode"
+
+                    log(ERROR, "%s raised an exception", exc_entity, exc_info=ex)
+
+                    # Create error message
+                    reply_message = message.create_error_reply(
+                        error=Error(code=e_code, reason=reason)
+                    )
+                else:
+                    # No exception, update node state
+                    node_state.update_context(
+                        run_id=message.metadata.run_id,
+                        context=context,
+                    )
+
                 # Send
-                send(out_message)
+                send(reply_message)
+                log(INFO, "Sent reply")
 
             # Unregister node
             if delete_node is not None:
                 delete_node()  # pylint: disable=not-callable
 
         if sleep_duration == 0:
             log(INFO, "Disconnect and shut down")
@@ -503,29 +646,28 @@
         grpc_max_message_length=grpc_max_message_length,
         root_certificates=root_certificates,
         insecure=insecure,
         transport=transport,
     )
 
 
-def _init_connection(
-    transport: Optional[str], server_address: str
-) -> Tuple[
+def _init_connection(transport: Optional[str], server_address: str) -> Tuple[
     Callable[
-        [str, bool, int, Union[bytes, str, None]],
+        [str, bool, RetryInvoker, int, Union[bytes, str, None]],
         ContextManager[
             Tuple[
                 Callable[[], Optional[Message]],
                 Callable[[Message], None],
                 Optional[Callable[[], None]],
                 Optional[Callable[[], None]],
             ]
         ],
     ],
     str,
+    Type[Exception],
 ]:
     # Parse IP address
     parsed_address = parse_address(server_address)
     if not parsed_address:
         sys.exit(f"Server address ({server_address}) cannot be parsed.")
     host, port, is_v6 = parsed_address
     address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
@@ -533,26 +675,28 @@
     # Set the default transport layer
     if transport is None:
         transport = TRANSPORT_TYPE_GRPC_BIDI
 
     # Use either gRPC bidirectional streaming or REST request/response
     if transport == TRANSPORT_TYPE_REST:
         try:
+            from requests.exceptions import ConnectionError as RequestsConnectionError
+
             from .rest_client.connection import http_request_response
         except ModuleNotFoundError:
             sys.exit(MISSING_EXTRA_REST)
         if server_address[:4] != "http":
             sys.exit(
                 "When using the REST API, please provide `https://` or "
                 "`http://` before the server address (e.g. `http://127.0.0.1:8080`)"
             )
-        connection = http_request_response
+        connection, error_type = http_request_response, RequestsConnectionError
     elif transport == TRANSPORT_TYPE_GRPC_RERE:
-        connection = grpc_request_response
+        connection, error_type = grpc_request_response, RpcError
     elif transport == TRANSPORT_TYPE_GRPC_BIDI:
-        connection = grpc_connection
+        connection, error_type = grpc_connection, RpcError
     else:
         raise ValueError(
             f"Unknown transport type: {transport} (possible: {TRANSPORT_TYPES})"
         )
 
-    return connection, address
+    return connection, address, error_type
```

### Comparing `flwr-1.7.0/src/py/flwr/client/client.py` & `flwr-1.8.0/src/py/flwr/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,26 +17,26 @@
 # Needed to `Client` class can return a type of `Client` (not needed in py3.11+)
 from __future__ import annotations
 
 from abc import ABC
 
 from flwr.common import (
     Code,
+    Context,
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
     GetParametersIns,
     GetParametersRes,
     GetPropertiesIns,
     GetPropertiesRes,
     Parameters,
     Status,
 )
-from flwr.common.context import Context
 
 
 class Client(ABC):
     """Abstract base class for Flower clients."""
 
     context: Context
```

### Comparing `flwr-1.7.0/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr-1.8.0/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/client/grpc_client/__init__.py` & `flwr-1.8.0/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/client/grpc_client/connection.py` & `flwr-1.8.0/src/py/flwr/client/grpc_client/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 import uuid
 from contextlib import contextmanager
 from logging import DEBUG
 from pathlib import Path
 from queue import Queue
 from typing import Callable, Iterator, Optional, Tuple, Union, cast
 
-from flwr.common import GRPC_MAX_MESSAGE_LENGTH
+from flwr.common import (
+    DEFAULT_TTL,
+    GRPC_MAX_MESSAGE_LENGTH,
+    ConfigsRecord,
+    Message,
+    Metadata,
+    RecordSet,
+)
 from flwr.common import recordset_compat as compat
 from flwr.common import serde
-from flwr.common.configsrecord import ConfigsRecord
-from flwr.common.constant import (
-    TASK_TYPE_EVALUATE,
-    TASK_TYPE_FIT,
-    TASK_TYPE_GET_PARAMETERS,
-    TASK_TYPE_GET_PROPERTIES,
-)
+from flwr.common.constant import MessageType, MessageTypeLegacy
 from flwr.common.grpc import create_channel
 from flwr.common.logger import log
-from flwr.common.message import Message, Metadata
-from flwr.common.recordset import RecordSet
+from flwr.common.retry_invoker import RetryInvoker
 from flwr.proto.transport_pb2 import (  # pylint: disable=E0611
     ClientMessage,
     Reason,
     ServerMessage,
 )
 from flwr.proto.transport_pb2_grpc import FlowerServiceStub  # pylint: disable=E0611
 
@@ -55,14 +55,15 @@
     log(DEBUG, channel_connectivity)
 
 
 @contextmanager
 def grpc_connection(  # pylint: disable=R0915
     server_address: str,
     insecure: bool,
+    retry_invoker: RetryInvoker,  # pylint: disable=unused-argument
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,
     root_certificates: Optional[Union[bytes, str]] = None,
 ) -> Iterator[
     Tuple[
         Callable[[], Optional[Message]],
         Callable[[Message], None],
         Optional[Callable[[], None]],
@@ -73,14 +74,19 @@
 
     Parameters
     ----------
     server_address : str
         The IPv4 or IPv6 address of the server. If the Flower server runs on the same
         machine on port 8080, then `server_address` would be `"0.0.0.0:8080"` or
         `"[::]:8080"`.
+    insecure : bool
+        Starts an insecure gRPC connection when True. Enables HTTPS connection
+        when False, using system certificates if `root_certificates` is None.
+    retry_invoker: RetryInvoker
+        Unused argument present for compatibilty.
     max_message_length : int
         The maximum length of gRPC messages that can be exchanged with the Flower
         server. The default should be sufficient for most models. Users who train
         very large models might need to increase this value. Note that the Flower
         server needs to be started with the same value
         (see `flwr.server.start_server`), otherwise it will not know about the
         increased limit and block larger messages.
@@ -129,88 +135,93 @@
 
     def receive() -> Message:
         # Receive ServerMessage proto
         proto = next(server_message_iterator)
 
         # ServerMessage proto --> *Ins --> RecordSet
         field = proto.WhichOneof("msg")
-        task_type = ""
+        message_type = ""
         if field == "get_properties_ins":
             recordset = compat.getpropertiesins_to_recordset(
                 serde.get_properties_ins_from_proto(proto.get_properties_ins)
             )
-            task_type = TASK_TYPE_GET_PROPERTIES
+            message_type = MessageTypeLegacy.GET_PROPERTIES
         elif field == "get_parameters_ins":
             recordset = compat.getparametersins_to_recordset(
                 serde.get_parameters_ins_from_proto(proto.get_parameters_ins)
             )
-            task_type = TASK_TYPE_GET_PARAMETERS
+            message_type = MessageTypeLegacy.GET_PARAMETERS
         elif field == "fit_ins":
             recordset = compat.fitins_to_recordset(
                 serde.fit_ins_from_proto(proto.fit_ins), False
             )
-            task_type = TASK_TYPE_FIT
+            message_type = MessageType.TRAIN
         elif field == "evaluate_ins":
             recordset = compat.evaluateins_to_recordset(
                 serde.evaluate_ins_from_proto(proto.evaluate_ins), False
             )
-            task_type = TASK_TYPE_EVALUATE
+            message_type = MessageType.EVALUATE
         elif field == "reconnect_ins":
             recordset = RecordSet()
-            recordset.set_configs(
-                "config", ConfigsRecord({"seconds": proto.reconnect_ins.seconds})
+            recordset.configs_records["config"] = ConfigsRecord(
+                {"seconds": proto.reconnect_ins.seconds}
             )
-            task_type = "reconnect"
+            message_type = "reconnect"
         else:
             raise ValueError(
                 "Unsupported instruction in ServerMessage, "
                 "cannot deserialize from ProtoBuf"
             )
 
         # Construct Message
         return Message(
             metadata=Metadata(
                 run_id=0,
-                task_id=str(uuid.uuid4()),
+                message_id=str(uuid.uuid4()),
+                src_node_id=0,
+                dst_node_id=0,
+                reply_to_message="",
                 group_id="",
-                ttl="",
-                task_type=task_type,
+                ttl=DEFAULT_TTL,
+                message_type=message_type,
             ),
-            message=recordset,
+            content=recordset,
         )
 
     def send(message: Message) -> None:
-        # Retrieve RecordSet and task_type
-        recordset = message.message
-        task_type = message.metadata.task_type
+        # Retrieve RecordSet and message_type
+        recordset = message.content
+        message_type = message.metadata.message_type
 
         # RecordSet --> *Res --> *Res proto -> ClientMessage proto
-        if task_type == TASK_TYPE_GET_PROPERTIES:
+        if message_type == MessageTypeLegacy.GET_PROPERTIES:
             getpropres = compat.recordset_to_getpropertiesres(recordset)
             msg_proto = ClientMessage(
                 get_properties_res=serde.get_properties_res_to_proto(getpropres)
             )
-        elif task_type == TASK_TYPE_GET_PARAMETERS:
+        elif message_type == MessageTypeLegacy.GET_PARAMETERS:
             getparamres = compat.recordset_to_getparametersres(recordset, False)
             msg_proto = ClientMessage(
                 get_parameters_res=serde.get_parameters_res_to_proto(getparamres)
             )
-        elif task_type == TASK_TYPE_FIT:
+        elif message_type == MessageType.TRAIN:
             fitres = compat.recordset_to_fitres(recordset, False)
             msg_proto = ClientMessage(fit_res=serde.fit_res_to_proto(fitres))
-        elif task_type == TASK_TYPE_EVALUATE:
+        elif message_type == MessageType.EVALUATE:
             evalres = compat.recordset_to_evaluateres(recordset)
             msg_proto = ClientMessage(evaluate_res=serde.evaluate_res_to_proto(evalres))
-        elif task_type == "reconnect":
-            reason = cast(Reason.ValueType, recordset.get_configs("config")["reason"])
+        elif message_type == "reconnect":
+            reason = cast(
+                Reason.ValueType, recordset.configs_records["config"]["reason"]
+            )
             msg_proto = ClientMessage(
                 disconnect_res=ClientMessage.DisconnectRes(reason=reason)
             )
         else:
-            raise ValueError(f"Invalid task type: {task_type}")
+            raise ValueError(f"Invalid message type: {message_type}")
 
         # Send ClientMessage proto
         return queue.put(msg_proto, block=False)
 
     try:
         # Yield methods
         yield (receive, send, None, None)
```

### Comparing `flwr-1.7.0/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr-1.8.0/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr-1.8.0/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,53 +11,60 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Contextmanager for a gRPC request-response channel to the Flower server."""
 
 
+import random
+import threading
 from contextlib import contextmanager
+from copy import copy
 from logging import DEBUG, ERROR
 from pathlib import Path
-from typing import Callable, Dict, Iterator, Optional, Tuple, Union, cast
+from typing import Callable, Iterator, Optional, Tuple, Union, cast
 
-from flwr.client.message_handler.task_handler import (
-    configure_task_res,
-    get_task_ins,
-    validate_task_ins,
-    validate_task_res,
-)
+from flwr.client.heartbeat import start_ping_loop
+from flwr.client.message_handler.message_handler import validate_out_message
+from flwr.client.message_handler.task_handler import get_task_ins, validate_task_ins
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
+from flwr.common.constant import (
+    PING_BASE_MULTIPLIER,
+    PING_CALL_TIMEOUT,
+    PING_DEFAULT_INTERVAL,
+    PING_RANDOM_RANGE,
+)
 from flwr.common.grpc import create_channel
-from flwr.common.logger import log, warn_experimental_feature
-from flwr.common.message import Message
+from flwr.common.logger import log
+from flwr.common.message import Message, Metadata
+from flwr.common.retry_invoker import RetryInvoker
 from flwr.common.serde import message_from_taskins, message_to_taskres
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     DeleteNodeRequest,
+    PingRequest,
+    PingResponse,
     PullTaskInsRequest,
     PushTaskResRequest,
 )
 from flwr.proto.fleet_pb2_grpc import FleetStub  # pylint: disable=E0611
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.task_pb2 import TaskIns  # pylint: disable=E0611
 
-KEY_NODE = "node"
-KEY_TASK_INS = "current_task_ins"
-
 
 def on_channel_state_change(channel_connectivity: str) -> None:
     """Log channel connectivity."""
     log(DEBUG, channel_connectivity)
 
 
 @contextmanager
-def grpc_request_response(
+def grpc_request_response(  # pylint: disable=R0914, R0915
     server_address: str,
     insecure: bool,
+    retry_invoker: RetryInvoker,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,  # pylint: disable=W0613
     root_certificates: Optional[Union[bytes, str]] = None,
 ) -> Iterator[
     Tuple[
         Callable[[], Optional[Message]],
         Callable[[Message], None],
         Optional[Callable[[], None]],
@@ -71,127 +78,171 @@
 
     Parameters
     ----------
     server_address : str
         The IPv6 address of the server with `http://` or `https://`.
         If the Flower server runs on the same machine
         on port 8080, then `server_address` would be `"http://[::]:8080"`.
+    insecure : bool
+        Starts an insecure gRPC connection when True. Enables HTTPS connection
+        when False, using system certificates if `root_certificates` is None.
+    retry_invoker: RetryInvoker
+        `RetryInvoker` object that will try to reconnect the client to the server
+        after gRPC errors. If None, the client will only try to
+        reconnect once after a failure.
     max_message_length : int
         Ignored, only present to preserve API-compatibility.
     root_certificates : Optional[Union[bytes, str]] (default: None)
         Path of the root certificate. If provided, a secure
         connection using the certificates will be established to an SSL-enabled
         Flower server. Bytes won't work for the REST API.
 
     Returns
     -------
     receive : Callable
     send : Callable
     create_node : Optional[Callable]
     delete_node : Optional[Callable]
     """
-    warn_experimental_feature("`grpc-rere`")
-
     if isinstance(root_certificates, str):
         root_certificates = Path(root_certificates).read_bytes()
 
     channel = create_channel(
         server_address=server_address,
         insecure=insecure,
         root_certificates=root_certificates,
         max_message_length=max_message_length,
     )
     channel.subscribe(on_channel_state_change)
-    stub = FleetStub(channel)
-
-    # Necessary state to link TaskRes to TaskIns
-    state: Dict[str, Optional[TaskIns]] = {KEY_TASK_INS: None}
 
-    # Enable create_node and delete_node to store node
-    node_store: Dict[str, Optional[Node]] = {KEY_NODE: None}
+    # Shared variables for inner functions
+    stub = FleetStub(channel)
+    metadata: Optional[Metadata] = None
+    node: Optional[Node] = None
+    ping_thread: Optional[threading.Thread] = None
+    ping_stop_event = threading.Event()
 
     ###########################################################################
-    # receive/send functions
+    # ping/create_node/delete_node/receive/send functions
     ###########################################################################
 
+    def ping() -> None:
+        # Get Node
+        if node is None:
+            log(ERROR, "Node instance missing")
+            return
+
+        # Construct the ping request
+        req = PingRequest(node=node, ping_interval=PING_DEFAULT_INTERVAL)
+
+        # Call FleetAPI
+        res: PingResponse = stub.Ping(req, timeout=PING_CALL_TIMEOUT)
+
+        # Check if success
+        if not res.success:
+            raise RuntimeError("Ping failed unexpectedly.")
+
+        # Wait
+        rd = random.uniform(*PING_RANDOM_RANGE)
+        next_interval: float = PING_DEFAULT_INTERVAL - PING_CALL_TIMEOUT
+        next_interval *= PING_BASE_MULTIPLIER + rd
+        if not ping_stop_event.is_set():
+            ping_stop_event.wait(next_interval)
+
     def create_node() -> None:
         """Set create_node."""
-        create_node_request = CreateNodeRequest()
-        create_node_response = stub.CreateNode(
+        # Call FleetAPI
+        create_node_request = CreateNodeRequest(ping_interval=PING_DEFAULT_INTERVAL)
+        create_node_response = retry_invoker.invoke(
+            stub.CreateNode,
             request=create_node_request,
         )
-        node_store[KEY_NODE] = create_node_response.node
+
+        # Remember the node and the ping-loop thread
+        nonlocal node, ping_thread
+        node = cast(Node, create_node_response.node)
+        ping_thread = start_ping_loop(ping, ping_stop_event)
 
     def delete_node() -> None:
         """Set delete_node."""
         # Get Node
-        if node_store[KEY_NODE] is None:
+        nonlocal node
+        if node is None:
             log(ERROR, "Node instance missing")
             return
-        node: Node = cast(Node, node_store[KEY_NODE])
 
+        # Stop the ping-loop thread
+        ping_stop_event.set()
+        if ping_thread is not None:
+            ping_thread.join()
+
+        # Call FleetAPI
         delete_node_request = DeleteNodeRequest(node=node)
-        stub.DeleteNode(request=delete_node_request)
+        retry_invoker.invoke(stub.DeleteNode, request=delete_node_request)
 
-        del node_store[KEY_NODE]
+        # Cleanup
+        node = None
 
     def receive() -> Optional[Message]:
         """Receive next task from server."""
         # Get Node
-        if node_store[KEY_NODE] is None:
+        if node is None:
             log(ERROR, "Node instance missing")
             return None
-        node: Node = cast(Node, node_store[KEY_NODE])
 
         # Request instructions (task) from server
         request = PullTaskInsRequest(node=node)
-        response = stub.PullTaskIns(request=request)
+        response = retry_invoker.invoke(stub.PullTaskIns, request=request)
 
         # Get the current TaskIns
         task_ins: Optional[TaskIns] = get_task_ins(response)
 
         # Discard the current TaskIns if not valid
-        if task_ins is not None and not validate_task_ins(task_ins):
+        if task_ins is not None and not (
+            task_ins.task.consumer.node_id == node.node_id
+            and validate_task_ins(task_ins)
+        ):
             task_ins = None
 
-        # Remember `task_ins` until `task_res` is available
-        state[KEY_TASK_INS] = task_ins
+        # Construct the Message
+        in_message = message_from_taskins(task_ins) if task_ins else None
+
+        # Remember `metadata` of the in message
+        nonlocal metadata
+        metadata = copy(in_message.metadata) if in_message else None
 
         # Return the message if available
-        return message_from_taskins(task_ins) if task_ins is not None else None
+        return in_message
 
     def send(message: Message) -> None:
         """Send task result back to server."""
         # Get Node
-        if node_store[KEY_NODE] is None:
+        if node is None:
             log(ERROR, "Node instance missing")
             return
-        node: Node = cast(Node, node_store[KEY_NODE])
 
-        # Get incoming TaskIns
-        if state[KEY_TASK_INS] is None:
-            log(ERROR, "No current TaskIns")
+        # Get the metadata of the incoming message
+        nonlocal metadata
+        if metadata is None:
+            log(ERROR, "No current message")
+            return
+
+        # Validate out message
+        if not validate_out_message(message, metadata):
+            log(ERROR, "Invalid out message")
             return
-        task_ins: TaskIns = cast(TaskIns, state[KEY_TASK_INS])
 
         # Construct TaskRes
         task_res = message_to_taskres(message)
 
-        # Check if fields to be set are not initialized
-        if not validate_task_res(task_res):
-            state[KEY_TASK_INS] = None
-            log(ERROR, "TaskRes has been initialized accidentally")
-
-        # Configure TaskRes
-        task_res = configure_task_res(task_res, task_ins, node)
-
         # Serialize ProtoBuf to bytes
         request = PushTaskResRequest(task_res_list=[task_res])
-        _ = stub.PushTaskRes(request)
+        _ = retry_invoker.invoke(stub.PushTaskRes, request)
 
-        state[KEY_TASK_INS] = None
+        # Cleanup
+        metadata = None
 
     try:
         # Yield methods
         yield (receive, send, create_node, delete_node)
     except Exception as exc:  # pylint: disable=broad-except
         log(ERROR, exc)
```

### Comparing `flwr-1.7.0/src/py/flwr/client/message_handler/__init__.py` & `flwr-1.8.0/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/client/message_handler/message_handler.py` & `flwr-1.8.0/src/py/flwr/client/message_handler/message_handler.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,33 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Client-side message handler."""
 
 
+from logging import WARN
 from typing import Optional, Tuple, cast
 
 from flwr.client.client import (
     maybe_call_evaluate,
     maybe_call_fit,
     maybe_call_get_parameters,
     maybe_call_get_properties,
 )
+from flwr.client.numpy_client import NumPyClient
 from flwr.client.typing import ClientFn
-from flwr.common.configsrecord import ConfigsRecord
-from flwr.common.constant import (
-    TASK_TYPE_EVALUATE,
-    TASK_TYPE_FIT,
-    TASK_TYPE_GET_PARAMETERS,
-    TASK_TYPE_GET_PROPERTIES,
-)
-from flwr.common.context import Context
-from flwr.common.message import Message, Metadata
-from flwr.common.recordset import RecordSet
+from flwr.common import ConfigsRecord, Context, Message, Metadata, RecordSet, log
+from flwr.common.constant import MessageType, MessageTypeLegacy
 from flwr.common.recordset_compat import (
     evaluateres_to_recordset,
     fitres_to_recordset,
     getparametersres_to_recordset,
     getpropertiesres_to_recordset,
     recordset_to_evaluateins,
     recordset_to_fitins,
@@ -71,105 +65,114 @@
     -------
     message : Optional[Message]
         Message to be sent back to the server. If None, the client should
         continue to process messages from the server.
     sleep_duration : int
         Number of seconds that the client should disconnect from the server.
     """
-    if message.metadata.task_type == "reconnect":
+    if message.metadata.message_type == "reconnect":
         # Retrieve ReconnectIns from recordset
-        recordset = message.message
-        seconds = cast(int, recordset.get_configs("config")["seconds"])
+        recordset = message.content
+        seconds = cast(int, recordset.configs_records["config"]["seconds"])
         # Construct ReconnectIns and call _reconnect
         disconnect_msg, sleep_duration = _reconnect(
             ServerMessage.ReconnectIns(seconds=seconds)
         )
         # Store DisconnectRes in recordset
         reason = cast(int, disconnect_msg.disconnect_res.reason)
         recordset = RecordSet()
-        recordset.set_configs("config", ConfigsRecord({"reason": reason}))
-        out_message = Message(
-            metadata=Metadata(
-                run_id=0,
-                task_id="",
-                group_id="",
-                ttl="",
-                task_type="reconnect",
-            ),
-            message=recordset,
-        )
+        recordset.configs_records["config"] = ConfigsRecord({"reason": reason})
+        out_message = message.create_reply(recordset)
         # Return TaskRes and sleep duration
         return out_message, sleep_duration
 
     # Any other message
     return None, 0
 
 
-def handle_legacy_message_from_tasktype(
+def handle_legacy_message_from_msgtype(
     client_fn: ClientFn, message: Message, context: Context
 ) -> Message:
-    """Handle legacy message in the inner most middleware layer."""
-    client = client_fn("-1")
+    """Handle legacy message in the inner most mod."""
+    client = client_fn(str(message.metadata.partition_id))
+
+    # Check if NumPyClient is returend
+    if isinstance(client, NumPyClient):
+        client = client.to_client()
+        log(
+            WARN,
+            "Deprecation Warning: The `client_fn` function must return an instance "
+            "of `Client`, but an instance of `NumpyClient` was returned. "
+            "Please use `NumPyClient.to_client()` method to convert it to `Client`.",
+        )
 
     client.set_context(context)
 
-    task_type = message.metadata.task_type
+    message_type = message.metadata.message_type
 
     # Handle GetPropertiesIns
-    if task_type == TASK_TYPE_GET_PROPERTIES:
+    if message_type == MessageTypeLegacy.GET_PROPERTIES:
         get_properties_res = maybe_call_get_properties(
             client=client,
-            get_properties_ins=recordset_to_getpropertiesins(message.message),
+            get_properties_ins=recordset_to_getpropertiesins(message.content),
         )
         out_recordset = getpropertiesres_to_recordset(get_properties_res)
     # Handle GetParametersIns
-    elif task_type == TASK_TYPE_GET_PARAMETERS:
+    elif message_type == MessageTypeLegacy.GET_PARAMETERS:
         get_parameters_res = maybe_call_get_parameters(
             client=client,
-            get_parameters_ins=recordset_to_getparametersins(message.message),
+            get_parameters_ins=recordset_to_getparametersins(message.content),
         )
         out_recordset = getparametersres_to_recordset(
             get_parameters_res, keep_input=False
         )
     # Handle FitIns
-    elif task_type == TASK_TYPE_FIT:
+    elif message_type == MessageType.TRAIN:
         fit_res = maybe_call_fit(
             client=client,
-            fit_ins=recordset_to_fitins(message.message, keep_input=True),
+            fit_ins=recordset_to_fitins(message.content, keep_input=True),
         )
         out_recordset = fitres_to_recordset(fit_res, keep_input=False)
     # Handle EvaluateIns
-    elif task_type == TASK_TYPE_EVALUATE:
+    elif message_type == MessageType.EVALUATE:
         evaluate_res = maybe_call_evaluate(
             client=client,
-            evaluate_ins=recordset_to_evaluateins(message.message, keep_input=True),
+            evaluate_ins=recordset_to_evaluateins(message.content, keep_input=True),
         )
         out_recordset = evaluateres_to_recordset(evaluate_res)
     else:
-        raise ValueError(f"Invalid task type: {task_type}")
+        raise ValueError(f"Invalid message type: {message_type}")
 
     # Return Message
-    out_message = Message(
-        metadata=Metadata(
-            run_id=0,  # Non-user defined
-            task_id="",  # Non-user defined
-            group_id="",  # Non-user defined
-            ttl="",
-            task_type=task_type,
-        ),
-        message=out_recordset,
-    )
-    return out_message
+    return message.create_reply(out_recordset)
 
 
 def _reconnect(
     reconnect_msg: ServerMessage.ReconnectIns,
 ) -> Tuple[ClientMessage, int]:
     # Determine the reason for sending DisconnectRes message
     reason = Reason.ACK
     sleep_duration = None
     if reconnect_msg.seconds is not None:
         reason = Reason.RECONNECT
         sleep_duration = reconnect_msg.seconds
     # Build DisconnectRes message
     disconnect_res = ClientMessage.DisconnectRes(reason=reason)
     return ClientMessage(disconnect_res=disconnect_res), sleep_duration
+
+
+def validate_out_message(out_message: Message, in_message_metadata: Metadata) -> bool:
+    """Validate the out message."""
+    out_meta = out_message.metadata
+    in_meta = in_message_metadata
+    if (  # pylint: disable-next=too-many-boolean-expressions
+        out_meta.run_id == in_meta.run_id
+        and out_meta.message_id == ""  # This will be generated by the server
+        and out_meta.src_node_id == in_meta.dst_node_id
+        and out_meta.dst_node_id == in_meta.src_node_id
+        and out_meta.reply_to_message == in_meta.message_id
+        and out_meta.group_id == in_meta.group_id
+        and out_meta.message_type == in_meta.message_type
+        and out_meta.created_at > in_meta.created_at
+    ):
+        return True
+    return False
```

### Comparing `flwr-1.7.0/src/py/flwr/client/middleware/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,15 @@
-# Copyright 2023 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Middleware layers."""
-
-
-from .secure_aggregation.secaggplus_middleware import secaggplus_middleware
-from .utils import make_ffn
-
-__all__ = [
-    "make_ffn",
-    "secaggplus_middleware",
-]
+"""Flower SuperLink."""
```

### Comparing `flwr-1.7.0/src/py/flwr/client/middleware/secure_aggregation/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Copyright 2023 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Secure Aggregation handlers."""
-from .secaggplus_middleware import secaggplus_middleware
+"""Fleet Simulation Engine side."""
+
+from .vce_api import start_vce
 
 __all__ = [
-    "secaggplus_middleware",
+    "start_vce",
 ]
```

### Comparing `flwr-1.7.0/src/py/flwr/client/middleware/secure_aggregation/secaggplus_middleware.py` & `flwr-1.8.0/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,31 +8,35 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Message handler for the SecAgg+ protocol."""
+"""Modifier for the SecAgg+ protocol."""
 
 
 import os
 from dataclasses import dataclass, field
-from logging import INFO, WARNING
-from typing import Any, Callable, Dict, List, Tuple, cast
+from logging import DEBUG, WARNING
+from typing import Any, Dict, List, Tuple, cast
 
-from flwr.client.typing import FlowerCallable
-from flwr.common import ndarray_to_bytes, parameters_to_ndarrays
+from flwr.client.typing import ClientAppCallable
+from flwr.common import (
+    ConfigsRecord,
+    Context,
+    Message,
+    Parameters,
+    RecordSet,
+    ndarray_to_bytes,
+    parameters_to_ndarrays,
+)
 from flwr.common import recordset_compat as compat
-from flwr.common.configsrecord import ConfigsRecord
-from flwr.common.constant import TASK_TYPE_FIT
-from flwr.common.context import Context
+from flwr.common.constant import MessageType
 from flwr.common.logger import log
-from flwr.common.message import Message, Metadata
-from flwr.common.recordset import RecordSet
 from flwr.common.secure_aggregation.crypto.shamir import create_shares
 from flwr.common.secure_aggregation.crypto.symmetric_encryption import (
     bytes_to_private_key,
     bytes_to_public_key,
     decrypt,
     encrypt,
     generate_key_pairs,
@@ -45,62 +49,42 @@
     parameters_addition,
     parameters_mod,
     parameters_multiply,
     parameters_subtraction,
 )
 from flwr.common.secure_aggregation.quantization import quantize
 from flwr.common.secure_aggregation.secaggplus_constants import (
-    KEY_ACTIVE_SECURE_ID_LIST,
-    KEY_CIPHERTEXT_LIST,
-    KEY_CLIPPING_RANGE,
-    KEY_DEAD_SECURE_ID_LIST,
-    KEY_DESTINATION_LIST,
-    KEY_MASKED_PARAMETERS,
-    KEY_MOD_RANGE,
-    KEY_PUBLIC_KEY_1,
-    KEY_PUBLIC_KEY_2,
-    KEY_SAMPLE_NUMBER,
-    KEY_SECURE_ID,
-    KEY_SECURE_ID_LIST,
-    KEY_SHARE_LIST,
-    KEY_SHARE_NUMBER,
-    KEY_SOURCE_LIST,
-    KEY_STAGE,
-    KEY_TARGET_RANGE,
-    KEY_THRESHOLD,
     RECORD_KEY_CONFIGS,
     RECORD_KEY_STATE,
-    STAGE_COLLECT_MASKED_INPUT,
-    STAGE_SETUP,
-    STAGE_SHARE_KEYS,
-    STAGE_UNMASK,
-    STAGES,
+    Key,
+    Stage,
 )
 from flwr.common.secure_aggregation.secaggplus_utils import (
     pseudo_rand_gen,
     share_keys_plaintext_concat,
     share_keys_plaintext_separate,
 )
-from flwr.common.typing import ConfigsRecordValues, FitRes
+from flwr.common.typing import ConfigsRecordValues
 
 
 @dataclass
 # pylint: disable-next=too-many-instance-attributes
 class SecAggPlusState:
     """State of the SecAgg+ protocol."""
 
-    current_stage: str = STAGE_UNMASK
+    current_stage: str = Stage.UNMASK
 
-    sid: int = 0
+    nid: int = 0
     sample_num: int = 0
     share_num: int = 0
     threshold: int = 0
     clipping_range: float = 0.0
     target_range: int = 0
     mod_range: int = 0
+    max_weight: float = 0.0
 
     # Secret key (sk) and public key (pk)
     sk1: bytes = b""
     pk1: bytes = b""
     sk2: bytes = b""
     pk2: bytes = b""
 
@@ -145,241 +129,235 @@
                         v_list.extend(b1_b2)
                     ret[f"{k}:V"] = v_list
                 else:
                     ret[f"{k}:V"] = list(v.values())
         return ret
 
 
-def _get_fit_fn(
-    msg: Message, ctxt: Context, call_next: FlowerCallable
-) -> Callable[[], FitRes]:
-    """Get the fit function."""
-
-    def fit() -> FitRes:
-        out_msg = call_next(msg, ctxt)
-        return compat.recordset_to_fitres(out_msg.message, keep_input=False)
-
-    return fit
-
-
-def secaggplus_middleware(
+def secaggplus_mod(
     msg: Message,
     ctxt: Context,
-    call_next: FlowerCallable,
+    call_next: ClientAppCallable,
 ) -> Message:
     """Handle incoming message and return results, following the SecAgg+ protocol."""
     # Ignore non-fit messages
-    if msg.metadata.task_type != TASK_TYPE_FIT:
+    if msg.metadata.message_type != MessageType.TRAIN:
         return call_next(msg, ctxt)
 
     # Retrieve local state
-    if RECORD_KEY_STATE not in ctxt.state.configs:
-        ctxt.state.set_configs(RECORD_KEY_STATE, ConfigsRecord({}))
-    state_dict = ctxt.state.get_configs(RECORD_KEY_STATE).data
+    if RECORD_KEY_STATE not in ctxt.state.configs_records:
+        ctxt.state.configs_records[RECORD_KEY_STATE] = ConfigsRecord({})
+    state_dict = ctxt.state.configs_records[RECORD_KEY_STATE]
     state = SecAggPlusState(**state_dict)
 
     # Retrieve incoming configs
-    configs = msg.message.get_configs(RECORD_KEY_CONFIGS).data
+    configs = msg.content.configs_records[RECORD_KEY_CONFIGS]
 
     # Check the validity of the next stage
     check_stage(state.current_stage, configs)
 
     # Update the current stage
-    state.current_stage = cast(str, configs.pop(KEY_STAGE))
+    state.current_stage = cast(str, configs.pop(Key.STAGE))
 
     # Check the validity of the configs based on the current stage
     check_configs(state.current_stage, configs)
 
     # Execute
-    if state.current_stage == STAGE_SETUP:
+    out_content = RecordSet()
+    if state.current_stage == Stage.SETUP:
+        state.nid = msg.metadata.dst_node_id
         res = _setup(state, configs)
-    elif state.current_stage == STAGE_SHARE_KEYS:
+    elif state.current_stage == Stage.SHARE_KEYS:
         res = _share_keys(state, configs)
-    elif state.current_stage == STAGE_COLLECT_MASKED_INPUT:
-        fit = _get_fit_fn(msg, ctxt, call_next)
-        res = _collect_masked_input(state, configs, fit)
-    elif state.current_stage == STAGE_UNMASK:
+    elif state.current_stage == Stage.COLLECT_MASKED_VECTORS:
+        out_msg = call_next(msg, ctxt)
+        out_content = out_msg.content
+        fitres = compat.recordset_to_fitres(out_content, keep_input=True)
+        res = _collect_masked_vectors(
+            state, configs, fitres.num_examples, fitres.parameters
+        )
+        for p_record in out_content.parameters_records.values():
+            p_record.clear()
+    elif state.current_stage == Stage.UNMASK:
         res = _unmask(state, configs)
     else:
-        raise ValueError(f"Unknown secagg stage: {state.current_stage}")
+        raise ValueError(f"Unknown SecAgg/SecAgg+ stage: {state.current_stage}")
 
     # Save state
-    ctxt.state.set_configs(RECORD_KEY_STATE, ConfigsRecord(state.to_dict()))
+    ctxt.state.configs_records[RECORD_KEY_STATE] = ConfigsRecord(state.to_dict())
 
     # Return message
-    return Message(
-        metadata=Metadata(0, "", "", "", TASK_TYPE_FIT),
-        message=RecordSet(configs={RECORD_KEY_CONFIGS: ConfigsRecord(res, False)}),
-    )
+    out_content.configs_records[RECORD_KEY_CONFIGS] = ConfigsRecord(res, False)
+    return msg.create_reply(out_content)
 
 
-def check_stage(current_stage: str, configs: Dict[str, ConfigsRecordValues]) -> None:
+def check_stage(current_stage: str, configs: ConfigsRecord) -> None:
     """Check the validity of the next stage."""
-    # Check the existence of KEY_STAGE
-    if KEY_STAGE not in configs:
+    # Check the existence of Config.STAGE
+    if Key.STAGE not in configs:
         raise KeyError(
-            f"The required key '{KEY_STAGE}' is missing from the input `named_values`."
+            f"The required key '{Key.STAGE}' is missing from the ConfigsRecord."
         )
 
-    # Check the value type of the KEY_STAGE
-    next_stage = configs[KEY_STAGE]
+    # Check the value type of the Config.STAGE
+    next_stage = configs[Key.STAGE]
     if not isinstance(next_stage, str):
         raise TypeError(
-            f"The value for the key '{KEY_STAGE}' must be of type {str}, "
+            f"The value for the key '{Key.STAGE}' must be of type {str}, "
             f"but got {type(next_stage)} instead."
         )
 
     # Check the validity of the next stage
-    if next_stage == STAGE_SETUP:
-        if current_stage != STAGE_UNMASK:
+    if next_stage == Stage.SETUP:
+        if current_stage != Stage.UNMASK:
             log(WARNING, "Restart from the setup stage")
     # If stage is not "setup",
-    # the stage from `named_values` should be the expected next stage
+    # the stage from configs should be the expected next stage
     else:
-        expected_next_stage = STAGES[(STAGES.index(current_stage) + 1) % len(STAGES)]
+        stages = Stage.all()
+        expected_next_stage = stages[(stages.index(current_stage) + 1) % len(stages)]
         if next_stage != expected_next_stage:
             raise ValueError(
                 "Abort secure aggregation: "
                 f"expect {expected_next_stage} stage, but receive {next_stage} stage"
             )
 
 
 # pylint: disable-next=too-many-branches
-def check_configs(stage: str, configs: Dict[str, ConfigsRecordValues]) -> None:
+def check_configs(stage: str, configs: ConfigsRecord) -> None:
     """Check the validity of the configs."""
-    # Check `named_values` for the setup stage
-    if stage == STAGE_SETUP:
+    # Check configs for the setup stage
+    if stage == Stage.SETUP:
         key_type_pairs = [
-            (KEY_SAMPLE_NUMBER, int),
-            (KEY_SECURE_ID, int),
-            (KEY_SHARE_NUMBER, int),
-            (KEY_THRESHOLD, int),
-            (KEY_CLIPPING_RANGE, float),
-            (KEY_TARGET_RANGE, int),
-            (KEY_MOD_RANGE, int),
+            (Key.SAMPLE_NUMBER, int),
+            (Key.SHARE_NUMBER, int),
+            (Key.THRESHOLD, int),
+            (Key.CLIPPING_RANGE, float),
+            (Key.TARGET_RANGE, int),
+            (Key.MOD_RANGE, int),
         ]
         for key, expected_type in key_type_pairs:
             if key not in configs:
                 raise KeyError(
-                    f"Stage {STAGE_SETUP}: the required key '{key}' is "
-                    "missing from the input `named_values`."
+                    f"Stage {Stage.SETUP}: the required key '{key}' is "
+                    "missing from the ConfigsRecord."
                 )
             # Bool is a subclass of int in Python,
             # so `isinstance(v, int)` will return True even if v is a boolean.
             # pylint: disable-next=unidiomatic-typecheck
             if type(configs[key]) is not expected_type:
                 raise TypeError(
-                    f"Stage {STAGE_SETUP}: The value for the key '{key}' "
+                    f"Stage {Stage.SETUP}: The value for the key '{key}' "
                     f"must be of type {expected_type}, "
                     f"but got {type(configs[key])} instead."
                 )
-    elif stage == STAGE_SHARE_KEYS:
+    elif stage == Stage.SHARE_KEYS:
         for key, value in configs.items():
             if (
                 not isinstance(value, list)
                 or len(value) != 2
                 or not isinstance(value[0], bytes)
                 or not isinstance(value[1], bytes)
             ):
                 raise TypeError(
-                    f"Stage {STAGE_SHARE_KEYS}: "
+                    f"Stage {Stage.SHARE_KEYS}: "
                     f"the value for the key '{key}' must be a list of two bytes."
                 )
-    elif stage == STAGE_COLLECT_MASKED_INPUT:
+    elif stage == Stage.COLLECT_MASKED_VECTORS:
         key_type_pairs = [
-            (KEY_CIPHERTEXT_LIST, bytes),
-            (KEY_SOURCE_LIST, int),
+            (Key.CIPHERTEXT_LIST, bytes),
+            (Key.SOURCE_LIST, int),
         ]
         for key, expected_type in key_type_pairs:
             if key not in configs:
                 raise KeyError(
-                    f"Stage {STAGE_COLLECT_MASKED_INPUT}: "
+                    f"Stage {Stage.COLLECT_MASKED_VECTORS}: "
                     f"the required key '{key}' is "
-                    "missing from the input `named_values`."
+                    "missing from the ConfigsRecord."
                 )
             if not isinstance(configs[key], list) or any(
                 elm
                 for elm in cast(List[Any], configs[key])
                 # pylint: disable-next=unidiomatic-typecheck
                 if type(elm) is not expected_type
             ):
                 raise TypeError(
-                    f"Stage {STAGE_COLLECT_MASKED_INPUT}: "
+                    f"Stage {Stage.COLLECT_MASKED_VECTORS}: "
                     f"the value for the key '{key}' "
                     f"must be of type List[{expected_type.__name__}]"
                 )
-    elif stage == STAGE_UNMASK:
+    elif stage == Stage.UNMASK:
         key_type_pairs = [
-            (KEY_ACTIVE_SECURE_ID_LIST, int),
-            (KEY_DEAD_SECURE_ID_LIST, int),
+            (Key.ACTIVE_NODE_ID_LIST, int),
+            (Key.DEAD_NODE_ID_LIST, int),
         ]
         for key, expected_type in key_type_pairs:
             if key not in configs:
                 raise KeyError(
-                    f"Stage {STAGE_UNMASK}: "
+                    f"Stage {Stage.UNMASK}: "
                     f"the required key '{key}' is "
-                    "missing from the input `named_values`."
+                    "missing from the ConfigsRecord."
                 )
             if not isinstance(configs[key], list) or any(
                 elm
                 for elm in cast(List[Any], configs[key])
                 # pylint: disable-next=unidiomatic-typecheck
                 if type(elm) is not expected_type
             ):
                 raise TypeError(
-                    f"Stage {STAGE_UNMASK}: "
+                    f"Stage {Stage.UNMASK}: "
                     f"the value for the key '{key}' "
                     f"must be of type List[{expected_type.__name__}]"
                 )
     else:
         raise ValueError(f"Unknown secagg stage: {stage}")
 
 
 def _setup(
-    state: SecAggPlusState, configs: Dict[str, ConfigsRecordValues]
+    state: SecAggPlusState, configs: ConfigsRecord
 ) -> Dict[str, ConfigsRecordValues]:
     # Assigning parameter values to object fields
     sec_agg_param_dict = configs
-    state.sample_num = cast(int, sec_agg_param_dict[KEY_SAMPLE_NUMBER])
-    state.sid = cast(int, sec_agg_param_dict[KEY_SECURE_ID])
-    log(INFO, "Client %d: starting stage 0...", state.sid)
-
-    state.share_num = cast(int, sec_agg_param_dict[KEY_SHARE_NUMBER])
-    state.threshold = cast(int, sec_agg_param_dict[KEY_THRESHOLD])
-    state.clipping_range = cast(float, sec_agg_param_dict[KEY_CLIPPING_RANGE])
-    state.target_range = cast(int, sec_agg_param_dict[KEY_TARGET_RANGE])
-    state.mod_range = cast(int, sec_agg_param_dict[KEY_MOD_RANGE])
+    state.sample_num = cast(int, sec_agg_param_dict[Key.SAMPLE_NUMBER])
+    log(DEBUG, "Node %d: starting stage 0...", state.nid)
 
-    # Dictionaries containing client secure IDs as keys
+    state.share_num = cast(int, sec_agg_param_dict[Key.SHARE_NUMBER])
+    state.threshold = cast(int, sec_agg_param_dict[Key.THRESHOLD])
+    state.clipping_range = cast(float, sec_agg_param_dict[Key.CLIPPING_RANGE])
+    state.target_range = cast(int, sec_agg_param_dict[Key.TARGET_RANGE])
+    state.mod_range = cast(int, sec_agg_param_dict[Key.MOD_RANGE])
+    state.max_weight = cast(float, sec_agg_param_dict[Key.MAX_WEIGHT])
+
+    # Dictionaries containing node IDs as keys
     # and their respective secret shares as values.
     state.rd_seed_share_dict = {}
     state.sk1_share_dict = {}
-    # Dictionary containing client secure IDs as keys
+    # Dictionary containing node IDs as keys
     # and their respective shared secrets (with this client) as values.
     state.ss2_dict = {}
 
     # Create 2 sets private public key pairs
     # One for creating pairwise masks
     # One for encrypting message to distribute shares
     sk1, pk1 = generate_key_pairs()
     sk2, pk2 = generate_key_pairs()
 
     state.sk1, state.pk1 = private_key_to_bytes(sk1), public_key_to_bytes(pk1)
     state.sk2, state.pk2 = private_key_to_bytes(sk2), public_key_to_bytes(pk2)
-    log(INFO, "Client %d: stage 0 completes. uploading public keys...", state.sid)
-    return {KEY_PUBLIC_KEY_1: state.pk1, KEY_PUBLIC_KEY_2: state.pk2}
+    log(DEBUG, "Node %d: stage 0 completes. uploading public keys...", state.nid)
+    return {Key.PUBLIC_KEY_1: state.pk1, Key.PUBLIC_KEY_2: state.pk2}
 
 
 # pylint: disable-next=too-many-locals
 def _share_keys(
-    state: SecAggPlusState, configs: Dict[str, ConfigsRecordValues]
+    state: SecAggPlusState, configs: ConfigsRecord
 ) -> Dict[str, ConfigsRecordValues]:
     named_bytes_tuples = cast(Dict[str, Tuple[bytes, bytes]], configs)
     key_dict = {int(sid): (pk1, pk2) for sid, (pk1, pk2) in named_bytes_tuples.items()}
-    log(INFO, "Client %d: starting stage 1...", state.sid)
+    log(DEBUG, "Node %d: starting stage 1...", state.nid)
     state.public_keys_dict = key_dict
 
     # Check if the size is larger than threshold
     if len(state.public_keys_dict) < state.threshold:
         raise ValueError("Available neighbours number smaller than threshold")
 
     # Check if all public keys are unique
@@ -388,16 +366,16 @@
         pk_list.append(pk1)
         pk_list.append(pk2)
     if len(set(pk_list)) != len(pk_list):
         raise ValueError("Some public keys are identical")
 
     # Check if public keys of this client are correct in the dictionary
     if (
-        state.public_keys_dict[state.sid][0] != state.pk1
-        or state.public_keys_dict[state.sid][1] != state.pk2
+        state.public_keys_dict[state.nid][0] != state.pk1
+        or state.public_keys_dict[state.nid][1] != state.pk2
     ):
         raise ValueError(
             "Own public keys are displayed in dict incorrectly, should not happen!"
         )
 
     # Generate the private mask seed
     state.rd_seed = os.urandom(32)
@@ -405,126 +383,136 @@
     # Create shares for the private mask seed and the first private key
     b_shares = create_shares(state.rd_seed, state.threshold, state.share_num)
     sk1_shares = create_shares(state.sk1, state.threshold, state.share_num)
 
     srcs, dsts, ciphertexts = [], [], []
 
     # Distribute shares
-    for idx, (sid, (_, pk2)) in enumerate(state.public_keys_dict.items()):
-        if sid == state.sid:
-            state.rd_seed_share_dict[state.sid] = b_shares[idx]
-            state.sk1_share_dict[state.sid] = sk1_shares[idx]
+    for idx, (nid, (_, pk2)) in enumerate(state.public_keys_dict.items()):
+        if nid == state.nid:
+            state.rd_seed_share_dict[state.nid] = b_shares[idx]
+            state.sk1_share_dict[state.nid] = sk1_shares[idx]
         else:
             shared_key = generate_shared_key(
                 bytes_to_private_key(state.sk2),
                 bytes_to_public_key(pk2),
             )
-            state.ss2_dict[sid] = shared_key
+            state.ss2_dict[nid] = shared_key
             plaintext = share_keys_plaintext_concat(
-                state.sid, sid, b_shares[idx], sk1_shares[idx]
+                state.nid, nid, b_shares[idx], sk1_shares[idx]
             )
             ciphertext = encrypt(shared_key, plaintext)
-            srcs.append(state.sid)
-            dsts.append(sid)
+            srcs.append(state.nid)
+            dsts.append(nid)
             ciphertexts.append(ciphertext)
 
-    log(INFO, "Client %d: stage 1 completes. uploading key shares...", state.sid)
-    return {KEY_DESTINATION_LIST: dsts, KEY_CIPHERTEXT_LIST: ciphertexts}
+    log(DEBUG, "Node %d: stage 1 completes. uploading key shares...", state.nid)
+    return {Key.DESTINATION_LIST: dsts, Key.CIPHERTEXT_LIST: ciphertexts}
 
 
 # pylint: disable-next=too-many-locals
-def _collect_masked_input(
+def _collect_masked_vectors(
     state: SecAggPlusState,
-    configs: Dict[str, ConfigsRecordValues],
-    fit: Callable[[], FitRes],
+    configs: ConfigsRecord,
+    num_examples: int,
+    updated_parameters: Parameters,
 ) -> Dict[str, ConfigsRecordValues]:
-    log(INFO, "Client %d: starting stage 2...", state.sid)
+    log(DEBUG, "Node %d: starting stage 2...", state.nid)
     available_clients: List[int] = []
-    ciphertexts = cast(List[bytes], configs[KEY_CIPHERTEXT_LIST])
-    srcs = cast(List[int], configs[KEY_SOURCE_LIST])
+    ciphertexts = cast(List[bytes], configs[Key.CIPHERTEXT_LIST])
+    srcs = cast(List[int], configs[Key.SOURCE_LIST])
     if len(ciphertexts) + 1 < state.threshold:
         raise ValueError("Not enough available neighbour clients.")
 
     # Decrypt ciphertexts, verify their sources, and store shares.
     for src, ciphertext in zip(srcs, ciphertexts):
         shared_key = state.ss2_dict[src]
         plaintext = decrypt(shared_key, ciphertext)
         actual_src, dst, rd_seed_share, sk1_share = share_keys_plaintext_separate(
             plaintext
         )
         available_clients.append(src)
         if src != actual_src:
             raise ValueError(
-                f"Client {state.sid}: received ciphertext "
+                f"Node {state.nid}: received ciphertext "
                 f"from {actual_src} instead of {src}."
             )
-        if dst != state.sid:
+        if dst != state.nid:
             raise ValueError(
-                f"Client {state.sid}: received an encrypted message"
-                f"for Client {dst} from Client {src}."
+                f"Node {state.nid}: received an encrypted message"
+                f"for Node {dst} from Node {src}."
             )
         state.rd_seed_share_dict[src] = rd_seed_share
         state.sk1_share_dict[src] = sk1_share
 
-    # Fit client
-    fit_res = fit()
-    parameters_factor = fit_res.num_examples
-    parameters = parameters_to_ndarrays(fit_res.parameters)
+    # Fit
+    ratio = num_examples / state.max_weight
+    if ratio > 1:
+        log(
+            WARNING,
+            "Potential overflow warning: the provided weight (%s) exceeds the specified"
+            " max_weight (%s). This may lead to overflow issues.",
+            num_examples,
+            state.max_weight,
+        )
+    q_ratio = round(ratio * state.target_range)
+    dq_ratio = q_ratio / state.target_range
+
+    parameters = parameters_to_ndarrays(updated_parameters)
+    parameters = parameters_multiply(parameters, dq_ratio)
 
     # Quantize parameter update (vector)
     quantized_parameters = quantize(
         parameters, state.clipping_range, state.target_range
     )
 
-    quantized_parameters = parameters_multiply(quantized_parameters, parameters_factor)
-    quantized_parameters = factor_combine(parameters_factor, quantized_parameters)
+    quantized_parameters = factor_combine(q_ratio, quantized_parameters)
 
     dimensions_list: List[Tuple[int, ...]] = [a.shape for a in quantized_parameters]
 
     # Add private mask
     private_mask = pseudo_rand_gen(state.rd_seed, state.mod_range, dimensions_list)
     quantized_parameters = parameters_addition(quantized_parameters, private_mask)
 
-    for client_id in available_clients:
+    for node_id in available_clients:
         # Add pairwise masks
         shared_key = generate_shared_key(
             bytes_to_private_key(state.sk1),
-            bytes_to_public_key(state.public_keys_dict[client_id][0]),
+            bytes_to_public_key(state.public_keys_dict[node_id][0]),
         )
         pairwise_mask = pseudo_rand_gen(shared_key, state.mod_range, dimensions_list)
-        if state.sid > client_id:
+        if state.nid > node_id:
             quantized_parameters = parameters_addition(
                 quantized_parameters, pairwise_mask
             )
         else:
             quantized_parameters = parameters_subtraction(
                 quantized_parameters, pairwise_mask
             )
 
     # Take mod of final weight update vector and return to server
     quantized_parameters = parameters_mod(quantized_parameters, state.mod_range)
-    log(INFO, "Client %d: stage 2 completes. uploading masked parameters...", state.sid)
+    log(DEBUG, "Node %d: stage 2 completed, uploading masked parameters...", state.nid)
     return {
-        KEY_MASKED_PARAMETERS: [ndarray_to_bytes(arr) for arr in quantized_parameters]
+        Key.MASKED_PARAMETERS: [ndarray_to_bytes(arr) for arr in quantized_parameters]
     }
 
 
 def _unmask(
-    state: SecAggPlusState, configs: Dict[str, ConfigsRecordValues]
+    state: SecAggPlusState, configs: ConfigsRecord
 ) -> Dict[str, ConfigsRecordValues]:
-    log(INFO, "Client %d: starting stage 3...", state.sid)
+    log(DEBUG, "Node %d: starting stage 3...", state.nid)
 
-    active_sids = cast(List[int], configs[KEY_ACTIVE_SECURE_ID_LIST])
-    dead_sids = cast(List[int], configs[KEY_DEAD_SECURE_ID_LIST])
-    # Send private mask seed share for every avaliable client (including itclient)
+    active_nids = cast(List[int], configs[Key.ACTIVE_NODE_ID_LIST])
+    dead_nids = cast(List[int], configs[Key.DEAD_NODE_ID_LIST])
+    # Send private mask seed share for every avaliable client (including itself)
     # Send first private key share for building pairwise mask for every dropped client
-    if len(active_sids) < state.threshold:
+    if len(active_nids) < state.threshold:
         raise ValueError("Available neighbours number smaller than threshold")
 
-    sids, shares = [], []
-    sids += active_sids
-    shares += [state.rd_seed_share_dict[sid] for sid in active_sids]
-    sids += dead_sids
-    shares += [state.sk1_share_dict[sid] for sid in dead_sids]
+    all_nids, shares = [], []
+    all_nids = active_nids + dead_nids
+    shares += [state.rd_seed_share_dict[nid] for nid in active_nids]
+    shares += [state.sk1_share_dict[nid] for nid in dead_nids]
 
-    log(INFO, "Client %d: stage 3 completes. uploading key shares...", state.sid)
-    return {KEY_SECURE_ID_LIST: sids, KEY_SHARE_LIST: shares}
+    log(DEBUG, "Node %d: stage 3 completes. uploading key shares...", state.nid)
+    return {Key.NODE_ID_LIST: all_nids, Key.SHARE_LIST: shares}
```

### Comparing `flwr-1.7.0/src/py/flwr/client/middleware/utils.py` & `flwr-1.8.0/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,30 @@
-# Copyright 2023 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Utility functions for middleware layers."""
+"""Modifier for the SecAgg protocol."""
 
 
-from typing import List
+from flwr.client.typing import ClientAppCallable
+from flwr.common import Context, Message
 
-from flwr.client.typing import FlowerCallable, Layer
-from flwr.common.context import Context
-from flwr.common.message import Message
+from .secaggplus_mod import secaggplus_mod
 
 
-def make_ffn(ffn: FlowerCallable, layers: List[Layer]) -> FlowerCallable:
-    """."""
-
-    def wrap_ffn(_ffn: FlowerCallable, _layer: Layer) -> FlowerCallable:
-        def new_ffn(message: Message, context: Context) -> Message:
-            return _layer(message, context, _ffn)
-
-        return new_ffn
-
-    for layer in reversed(layers):
-        ffn = wrap_ffn(ffn, layer)
-
-    return ffn
+def secagg_mod(
+    msg: Message,
+    ctxt: Context,
+    call_next: ClientAppCallable,
+) -> Message:
+    """Handle incoming message and return results, following the SecAgg protocol."""
+    return secaggplus_mod(msg, ctxt, call_next)
```

### Comparing `flwr-1.7.0/src/py/flwr/client/node_state.py` & `flwr-1.8.0/src/py/flwr/client/node_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """Node state."""
 
 
 from typing import Any, Dict
 
-from flwr.common.context import Context
-from flwr.common.recordset import RecordSet
+from flwr.common import Context, RecordSet
 
 
 class NodeState:
     """State of a node where client nodes execute runs."""
 
     def __init__(self) -> None:
         self._meta: Dict[str, Any] = {}  # holds metadata about the node
```

### Comparing `flwr-1.7.0/src/py/flwr/client/node_state_tests.py` & `flwr-1.8.0/src/py/flwr/client/node_state_tests.py`

 * *Files 19% similar despite different names*

```diff
@@ -11,29 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Node state tests."""
 
 
+from typing import cast
+
 from flwr.client.node_state import NodeState
-from flwr.common.configsrecord import ConfigsRecord
-from flwr.common.context import Context
+from flwr.common import ConfigsRecord, Context
 from flwr.proto.task_pb2 import TaskIns  # pylint: disable=E0611
 
 
 def _run_dummy_task(context: Context) -> Context:
     counter_value: str = "1"
-    if "counter" in context.state.configs.keys():
-        counter_value = context.get_configs("counter")["count"]  # type: ignore
+    if "counter" in context.state.configs_records.keys():
+        counter_value = cast(str, context.state.configs_records["counter"]["count"])
         counter_value += "1"
 
-    context.state.set_configs(
-        name="counter", record=ConfigsRecord({"count": counter_value})
-    )
+    context.state.configs_records["counter"] = ConfigsRecord({"count": counter_value})
 
     return context
 
 
 def test_multirun_in_node_state() -> None:
     """Test basic NodeState logic."""
     # Tasks to perform
@@ -57,8 +56,10 @@
         updated_state = _run_dummy_task(context)
 
         # Update run state
         node_state.update_context(run_id=run_id, context=updated_state)
 
     # Verify values
     for run_id, context in node_state.run_contexts.items():
-        assert context.state.get_configs("counter")["count"] == expected_values[run_id]
+        assert (
+            context.state.configs_records["counter"]["count"] == expected_values[run_id]
+        )
```

### Comparing `flwr-1.7.0/src/py/flwr/client/numpy_client.py` & `flwr-1.8.0/src/py/flwr/client/numpy_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
 from abc import ABC
 from typing import Callable, Dict, Tuple
 
 from flwr.client.client import Client
 from flwr.common import (
     Config,
+    Context,
     NDArrays,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
-from flwr.common.context import Context
 from flwr.common.typing import (
     Code,
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
     GetParametersIns,
```

### Comparing `flwr-1.7.0/src/py/flwr/client/rest_client/__init__.py` & `flwr-1.8.0/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/client/typing.py` & `flwr-1.8.0/src/py/flwr/client/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Custom types for Flower clients."""
 
+
 from typing import Callable
 
-from flwr.common.context import Context
-from flwr.common.message import Message
+from flwr.common import Context, Message
 
 from .client import Client as Client
 
-FlowerCallable = Callable[[Message, Context], Message]
+# Compatibility
 ClientFn = Callable[[str], Client]
-Layer = Callable[[Message, Context, FlowerCallable], Message]
+
+ClientAppCallable = Callable[[Message, Context], Message]
+Mod = Callable[[Message, Context, ClientAppCallable], Message]
```

### Comparing `flwr-1.7.0/src/py/flwr/common/address.py` & `flwr-1.8.0/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/configsrecord.py` & `flwr-1.8.0/src/py/flwr/common/record/configsrecord.py`

 * *Files 26% similar despite different names*

```diff
@@ -11,106 +11,113 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """ConfigsRecord."""
 
 
-from dataclasses import dataclass, field
-from typing import Dict, Optional, get_args
+from typing import Dict, List, Optional, get_args
 
-from .typing import ConfigsRecordValues, ConfigsScalar
+from flwr.common.typing import ConfigsRecordValues, ConfigsScalar
 
+from .typeddict import TypedDict
+
+
+def _check_key(key: str) -> None:
+    """Check if key is of expected type."""
+    if not isinstance(key, str):
+        raise TypeError(f"Key must be of type `str` but `{type(key)}` was passed.")
+
+
+def _check_value(value: ConfigsRecordValues) -> None:
+    def is_valid(__v: ConfigsScalar) -> None:
+        """Check if value is of expected type."""
+        if not isinstance(__v, get_args(ConfigsScalar)):
+            raise TypeError(
+                "Not all values are of valid type."
+                f" Expected `{ConfigsRecordValues}` but `{type(__v)}` was passed."
+            )
+
+    if isinstance(value, list):
+        # If your lists are large (e.g. 1M+ elements) this will be slow
+        # 1s to check 10M element list on a M2 Pro
+        # In such settings, you'd be better of treating such config as
+        # an array and pass it to a ParametersRecord.
+        # Empty lists are valid
+        if len(value) > 0:
+            is_valid(value[0])
+            # all elements in the list must be of the same valid type
+            # this is needed for protobuf
+            value_type = type(value[0])
+            if not all(isinstance(v, value_type) for v in value):
+                raise TypeError(
+                    "All values in a list must be of the same valid type. "
+                    f"One of {ConfigsScalar}."
+                )
+    else:
+        is_valid(value)
 
-@dataclass
-class ConfigsRecord:
-    """Configs record."""
 
-    data: Dict[str, ConfigsRecordValues] = field(default_factory=dict)
+class ConfigsRecord(TypedDict[str, ConfigsRecordValues]):
+    """Configs record."""
 
     def __init__(
         self,
         configs_dict: Optional[Dict[str, ConfigsRecordValues]] = None,
         keep_input: bool = True,
-    ):
+    ) -> None:
         """Construct a ConfigsRecord object.
 
         Parameters
         ----------
         configs_dict : Optional[Dict[str, ConfigsRecordValues]]
             A dictionary that stores basic types (i.e. `str`, `int`, `float`, `bytes` as
             defined in `ConfigsScalar`) and lists of such types (see
             `ConfigsScalarList`).
         keep_input : bool (default: True)
             A boolean indicating whether config passed should be deleted from the input
             dictionary immediately after adding them to the record. When set
             to True, the data is duplicated in memory. If memory is a concern, set
             it to False.
         """
-        self.data = {}
+        super().__init__(_check_key, _check_value)
         if configs_dict:
-            self.set_configs(configs_dict, keep_input=keep_input)
+            for k in list(configs_dict.keys()):
+                self[k] = configs_dict[k]
+                if not keep_input:
+                    del configs_dict[k]
 
-    def set_configs(
-        self, configs_dict: Dict[str, ConfigsRecordValues], keep_input: bool = True
-    ) -> None:
-        """Add configs to the record.
+    def count_bytes(self) -> int:
+        """Return number of Bytes stored in this object.
 
-        Parameters
-        ----------
-        configs_dict : Dict[str, ConfigsRecordValues]
-            A dictionary that stores basic types (i.e. `str`,`int`, `float`, `bytes` as
-            defined in `ConfigsRecordValues`) and list of such types (see
-            `ConfigsScalarList`).
-        keep_input : bool (default: True)
-            A boolean indicating whether config passed should be deleted from the input
-            dictionary immediately after adding them to the record. When set
-            to True, the data is duplicated in memory. If memory is a concern, set
-            it to False.
+        This function counts booleans as occupying 1 Byte.
         """
-        if any(not isinstance(k, str) for k in configs_dict.keys()):
-            raise TypeError(f"Not all keys are of valid type. Expected {str}")
 
-        def is_valid(value: ConfigsScalar) -> None:
-            """Check if value is of expected type."""
-            if not isinstance(value, get_args(ConfigsScalar)):
-                raise TypeError(
-                    "Not all values are of valid type."
-                    f" Expected {ConfigsRecordValues} but you passed {type(value)}."
+        def get_var_bytes(value: ConfigsScalar) -> int:
+            """Return Bytes of value passed."""
+            if isinstance(value, bool):
+                var_bytes = 1
+            elif isinstance(value, (int, float)):
+                var_bytes = (
+                    8  # the profobufing represents int/floats in ConfigRecords as 64bit
                 )
-
-        # Check types of values
-        # Split between those values that are list and those that aren't
-        # then process in the same way
-        for value in configs_dict.values():
-            if isinstance(value, list):
-                # If your lists are large (e.g. 1M+ elements) this will be slow
-                # 1s to check 10M element list on a M2 Pro
-                # In such settings, you'd be better of treating such config as
-                # an array and pass it to a ParametersRecord.
-                # Empty lists are valid
-                if len(value) > 0:
-                    is_valid(value[0])
-                    # all elements in the list must be of the same valid type
-                    # this is needed for protobuf
-                    value_type = type(value[0])
-                    if not all(isinstance(v, value_type) for v in value):
-                        raise TypeError(
-                            "All values in a list must be of the same valid type. "
-                            f"One of {ConfigsScalar}."
-                        )
+            if isinstance(value, (str, bytes)):
+                var_bytes = len(value)
+            return var_bytes
+
+        num_bytes = 0
+
+        for k, v in self.items():
+            if isinstance(v, List):
+                if isinstance(v[0], (bytes, str)):
+                    # not all str are of equal length necessarily
+                    # for both the footprint of each element is 1 Byte
+                    num_bytes += int(sum(len(s) for s in v))  # type: ignore
+                else:
+                    num_bytes += get_var_bytes(v[0]) * len(v)
             else:
-                is_valid(value)
+                num_bytes += get_var_bytes(v)
+
+            # We also count the bytes footprint of the keys
+            num_bytes += len(k)
 
-        # Add configs to record
-        if keep_input:
-            # Copy
-            self.data = configs_dict.copy()
-        else:
-            # Add entries to dataclass without duplicating memory
-            for key in list(configs_dict.keys()):
-                self.data[key] = configs_dict[key]
-                del configs_dict[key]
-
-    def __getitem__(self, key: str) -> ConfigsRecordValues:
-        """Retrieve an element stored in record."""
-        return self.data[key]
+        return num_bytes
```

### Comparing `flwr-1.7.0/src/py/flwr/common/constant.py` & `flwr-1.8.0/src/py/flwr/server/criterion.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,31 +8,21 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower constants."""
+"""Abstract class for criterion sampling."""
 
 
-MISSING_EXTRA_REST = """
-Extra dependencies required for using the REST-based Fleet API are missing.
+from abc import ABC, abstractmethod
 
-To use the REST API, install `flwr` with the `rest` extra:
+from .client_proxy import ClientProxy
 
-    `pip install flwr[rest]`.
-"""
-
-TRANSPORT_TYPE_GRPC_BIDI = "grpc-bidi"
-TRANSPORT_TYPE_GRPC_RERE = "grpc-rere"
-TRANSPORT_TYPE_REST = "rest"
-TRANSPORT_TYPES = [
-    TRANSPORT_TYPE_GRPC_BIDI,
-    TRANSPORT_TYPE_GRPC_RERE,
-    TRANSPORT_TYPE_REST,
-]
-
-TASK_TYPE_GET_PROPERTIES = "get_properties"
-TASK_TYPE_GET_PARAMETERS = "get_parameters"
-TASK_TYPE_FIT = "fit"
-TASK_TYPE_EVALUATE = "evaluate"
+
+class Criterion(ABC):
+    """Abstract class which allows subclasses to implement criterion sampling."""
+
+    @abstractmethod
+    def select(self, client: ClientProxy) -> bool:
+        """Decide whether a client should be eligible for sampling or not."""
```

### Comparing `flwr-1.7.0/src/py/flwr/common/context.py` & `flwr-1.8.0/src/py/flwr/common/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 # limitations under the License.
 # ==============================================================================
 """Context."""
 
 
 from dataclasses import dataclass
 
-from .recordset import RecordSet
+from .record import RecordSet
 
 
 @dataclass
 class Context:
     """State of your run.
 
     Parameters
     ----------
     state : RecordSet
         Holds records added by the entity in a given run and that will stay local.
         This means that the data it holds will never leave the system it's running from.
         This can be used as an intermediate storage or scratchpad when
-        executing middleware layers. It can also be used as a memory to access
+        executing mods. It can also be used as a memory to access
         at different points during the lifecycle of this entity (e.g. across
         multiple rounds)
     """
 
     state: RecordSet
```

### Comparing `flwr-1.7.0/src/py/flwr/common/date.py` & `flwr-1.8.0/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/dp.py` & `flwr-1.8.0/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/grpc.py` & `flwr-1.8.0/src/py/flwr/common/grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Utility functions for gRPC."""
 
 
-from logging import INFO
+from logging import DEBUG
 from typing import Optional
 
 import grpc
 
 from flwr.common.logger import log
 
 GRPC_MAX_MESSAGE_LENGTH: int = 536_870_912  # == 512 * 1024 * 1024
@@ -45,16 +45,16 @@
     channel_options = [
         ("grpc.max_send_message_length", max_message_length),
         ("grpc.max_receive_message_length", max_message_length),
     ]
 
     if insecure:
         channel = grpc.insecure_channel(server_address, options=channel_options)
-        log(INFO, "Opened insecure gRPC connection (no certificates were passed)")
+        log(DEBUG, "Opened insecure gRPC connection (no certificates were passed)")
     else:
         ssl_channel_credentials = grpc.ssl_channel_credentials(root_certificates)
         channel = grpc.secure_channel(
             server_address, ssl_channel_credentials, options=channel_options
         )
-        log(INFO, "Opened secure gRPC connection using certificates")
+        log(DEBUG, "Opened secure gRPC connection using certificates")
 
     return channel
```

### Comparing `flwr-1.7.0/src/py/flwr/common/metricsrecord.py` & `flwr-1.8.0/src/py/flwr/common/record/metricsrecord.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,25 +11,58 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """MetricsRecord."""
 
 
-from dataclasses import dataclass, field
-from typing import Dict, Optional, get_args
+from typing import Dict, List, Optional, get_args
 
-from .typing import MetricsRecordValues, MetricsScalar
+from flwr.common.typing import MetricsRecordValues, MetricsScalar
 
+from .typeddict import TypedDict
+
+
+def _check_key(key: str) -> None:
+    """Check if key is of expected type."""
+    if not isinstance(key, str):
+        raise TypeError(f"Key must be of type `str` but `{type(key)}` was passed.")
+
+
+def _check_value(value: MetricsRecordValues) -> None:
+    def is_valid(__v: MetricsScalar) -> None:
+        """Check if value is of expected type."""
+        if not isinstance(__v, get_args(MetricsScalar)) or isinstance(__v, bool):
+            raise TypeError(
+                "Not all values are of valid type."
+                f" Expected `{MetricsRecordValues}` but `{type(__v)}` was passed."
+            )
+
+    if isinstance(value, list):
+        # If your lists are large (e.g. 1M+ elements) this will be slow
+        # 1s to check 10M element list on a M2 Pro
+        # In such settings, you'd be better of treating such metric as
+        # an array and pass it to a ParametersRecord.
+        # Empty lists are valid
+        if len(value) > 0:
+            is_valid(value[0])
+            # all elements in the list must be of the same valid type
+            # this is needed for protobuf
+            value_type = type(value[0])
+            if not all(isinstance(v, value_type) for v in value):
+                raise TypeError(
+                    "All values in a list must be of the same valid type. "
+                    f"One of {MetricsScalar}."
+                )
+    else:
+        is_valid(value)
 
-@dataclass
-class MetricsRecord:
-    """Metrics record."""
 
-    data: Dict[str, MetricsRecordValues] = field(default_factory=dict)
+class MetricsRecord(TypedDict[str, MetricsRecordValues]):
+    """Metrics record."""
 
     def __init__(
         self,
         metrics_dict: Optional[Dict[str, MetricsRecordValues]] = None,
         keep_input: bool = True,
     ):
         """Construct a MetricsRecord object.
@@ -41,76 +74,29 @@
             in `MetricsScalar`) and list of such types (see `MetricsScalarList`).
         keep_input : bool (default: True)
             A boolean indicating whether metrics should be deleted from the input
             dictionary immediately after adding them to the record. When set
             to True, the data is duplicated in memory. If memory is a concern, set
             it to False.
         """
-        self.data = {}
+        super().__init__(_check_key, _check_value)
         if metrics_dict:
-            self.set_metrics(metrics_dict, keep_input=keep_input)
-
-    def set_metrics(
-        self, metrics_dict: Dict[str, MetricsRecordValues], keep_input: bool = True
-    ) -> None:
-        """Add metrics to the record.
-
-        Parameters
-        ----------
-        metrics_dict : Dict[str, MetricsRecordValues]
-            A dictionary that stores basic types (i.e. `int`, `float` as defined
-            in `MetricsScalar`) and list of such types (see `MetricsScalarList`).
-        keep_input : bool (default: True)
-            A boolean indicating whether metrics should be deleted from the input
-            dictionary immediately after adding them to the record. When set
-            to True, the data is duplicated in memory. If memory is a concern, set
-            it to False.
-        """
-        if any(not isinstance(k, str) for k in metrics_dict.keys()):
-            raise TypeError(f"Not all keys are of valid type. Expected {str}.")
-
-        def is_valid(value: MetricsScalar) -> None:
-            """Check if value is of expected type."""
-            if not isinstance(value, get_args(MetricsScalar)) or isinstance(
-                value, bool
-            ):
-                raise TypeError(
-                    "Not all values are of valid type."
-                    f" Expected {MetricsRecordValues} but you passed {type(value)}."
-                )
-
-        # Check types of values
-        # Split between those values that are list and those that aren't
-        # then process in the same way
-        for value in metrics_dict.values():
-            if isinstance(value, list):
-                # If your lists are large (e.g. 1M+ elements) this will be slow
-                # 1s to check 10M element list on a M2 Pro
-                # In such settings, you'd be better of treating such metric as
-                # an array and pass it to a ParametersRecord.
-                # Empty lists are valid
-                if len(value) > 0:
-                    is_valid(value[0])
-                    # all elements in the list must be of the same valid type
-                    # this is needed for protobuf
-                    value_type = type(value[0])
-                    if not all(isinstance(v, value_type) for v in value):
-                        raise TypeError(
-                            "All values in a list must be of the same valid type. "
-                            f"One of {MetricsScalar}."
-                        )
+            for k in list(metrics_dict.keys()):
+                self[k] = metrics_dict[k]
+                if not keep_input:
+                    del metrics_dict[k]
+
+    def count_bytes(self) -> int:
+        """Return number of Bytes stored in this object."""
+        num_bytes = 0
+
+        for k, v in self.items():
+            if isinstance(v, List):
+                # both int and float normally take 4 bytes
+                # But MetricRecords are mapped to 64bit int/float
+                # during protobuffing
+                num_bytes += 8 * len(v)
             else:
-                is_valid(value)
-
-        # Add metrics to record
-        if keep_input:
-            # Copy
-            self.data = metrics_dict.copy()
-        else:
-            # Add entries to dataclass without duplicating memory
-            for key in list(metrics_dict.keys()):
-                self.data[key] = metrics_dict[key]
-                del metrics_dict[key]
-
-    def __getitem__(self, key: str) -> MetricsRecordValues:
-        """Retrieve an element stored in record."""
-        return self.data[key]
+                num_bytes += 8
+            # We also count the bytes footprint of the keys
+            num_bytes += len(k)
+        return num_bytes
```

### Comparing `flwr-1.7.0/src/py/flwr/common/parameter.py` & `flwr-1.8.0/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/parametersrecord.py` & `flwr-1.8.0/src/py/flwr/common/record/parametersrecord.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """ParametersRecord and Array."""
 
-
-from dataclasses import dataclass, field
-from typing import List, Optional, OrderedDict
+from dataclasses import dataclass
+from io import BytesIO
+from typing import List, Optional, OrderedDict, cast
+
+import numpy as np
+
+from ..constant import SType
+from ..typing import NDArray
+from .typeddict import TypedDict
 
 
 @dataclass
 class Array:
     """Array type.
 
     A dataclass containing serialized data from an array-like or tensor-like object
@@ -45,26 +51,50 @@
     """
 
     dtype: str
     shape: List[int]
     stype: str
     data: bytes
 
+    def numpy(self) -> NDArray:
+        """Return the array as a NumPy array."""
+        if self.stype != SType.NUMPY:
+            raise TypeError(
+                f"Unsupported serialization type for numpy conversion: '{self.stype}'"
+            )
+        bytes_io = BytesIO(self.data)
+        # WARNING: NEVER set allow_pickle to true.
+        # Reason: loading pickled data can execute arbitrary code
+        # Source: https://numpy.org/doc/stable/reference/generated/numpy.load.html
+        ndarray_deserialized = np.load(bytes_io, allow_pickle=False)
+        return cast(NDArray, ndarray_deserialized)
+
+
+def _check_key(key: str) -> None:
+    """Check if key is of expected type."""
+    if not isinstance(key, str):
+        raise TypeError(f"Key must be of type `str` but `{type(key)}` was passed.")
+
+
+def _check_value(value: Array) -> None:
+    if not isinstance(value, Array):
+        raise TypeError(
+            f"Value must be of type `{Array}` but `{type(value)}` was passed."
+        )
+
 
 @dataclass
-class ParametersRecord:
+class ParametersRecord(TypedDict[str, Array]):
     """Parameters record.
 
     A dataclass storing named Arrays in order. This means that it holds entries as an
     OrderedDict[str, Array]. ParametersRecord objects can be viewed as an equivalent to
     PyTorch's state_dict, but holding serialised tensors instead.
     """
 
-    data: OrderedDict[str, Array] = field(default_factory=OrderedDict[str, Array])
-
     def __init__(
         self,
         array_dict: Optional[OrderedDict[str, Array]] = None,
         keep_input: bool = False,
     ) -> None:
         """Construct a ParametersRecord object.
 
@@ -77,41 +107,30 @@
             dictionary immediately after adding them to the record. If False, the
             dictionary passed to `set_parameters()` will be empty once exiting from that
             function. This is the desired behaviour when working with very large
             models/tensors/arrays. However, if you plan to continue working with your
             parameters after adding it to the record, set this flag to True. When set
             to True, the data is duplicated in memory.
         """
-        self.data = OrderedDict()
+        super().__init__(_check_key, _check_value)
         if array_dict:
-            self.set_parameters(array_dict, keep_input=keep_input)
+            for k in list(array_dict.keys()):
+                self[k] = array_dict[k]
+                if not keep_input:
+                    del array_dict[k]
+
+    def count_bytes(self) -> int:
+        """Return number of Bytes stored in this object.
+
+        Note that a small amount of Bytes might also be included in this counting that
+        correspond to metadata of the serialized object (e.g. of NumPy array) needed for
+        deseralization.
+        """
+        num_bytes = 0
 
-    def set_parameters(
-        self, array_dict: OrderedDict[str, Array], keep_input: bool = False
-    ) -> None:
-        """Add parameters to record.
+        for k, v in self.items():
+            num_bytes += len(v.data)
 
-        Parameters
-        ----------
-        array_dict : OrderedDict[str, Array]
-            A dictionary that stores serialized array-like or tensor-like objects.
-        keep_input : bool (default: False)
-            A boolean indicating whether parameters should be deleted from the input
-            dictionary immediately after adding them to the record.
-        """
-        if any(not isinstance(k, str) for k in array_dict.keys()):
-            raise TypeError(f"Not all keys are of valid type. Expected {str}")
-        if any(not isinstance(v, Array) for v in array_dict.values()):
-            raise TypeError(f"Not all values are of valid type. Expected {Array}")
-
-        if keep_input:
-            # Copy
-            self.data = OrderedDict(array_dict)
-        else:
-            # Add entries to dataclass without duplicating memory
-            for key in list(array_dict.keys()):
-                self.data[key] = array_dict[key]
-                del array_dict[key]
-
-    def __getitem__(self, key: str) -> Array:
-        """Retrieve an element stored in record."""
-        return self.data[key]
+            # We also count the bytes footprint of the keys
+            num_bytes += len(k)
+
+        return num_bytes
```

### Comparing `flwr-1.7.0/src/py/flwr/common/recordset_compat.py` & `flwr-1.8.0/src/py/flwr/common/recordset_compat.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,18 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 """RecordSet utilities."""
 
 
 from typing import Dict, Mapping, OrderedDict, Tuple, Union, cast, get_args
 
-from .configsrecord import ConfigsRecord
-from .metricsrecord import MetricsRecord
-from .parametersrecord import Array, ParametersRecord
-from .recordset import RecordSet
+from . import Array, ConfigsRecord, MetricsRecord, ParametersRecord, RecordSet
 from .typing import (
     Code,
     ConfigsRecordValues,
     EvaluateIns,
     EvaluateRes,
     FitIns,
     FitRes,
@@ -57,24 +54,24 @@
         The record to be conveted into Parameters.
     keep_input : bool
         A boolean indicating whether entries in the record should be deleted from the
         input dictionary immediately after adding them to the record.
     """
     parameters = Parameters(tensors=[], tensor_type="")
 
-    for key in list(record.data.keys()):
+    for key in list(record.keys()):
         parameters.tensors.append(record[key].data)
 
         if not parameters.tensor_type:
             # Setting from first array in record. Recall the warning in the docstrings
             # of this function.
             parameters.tensor_type = record[key].stype
 
         if not keep_input:
-            del record.data[key]
+            del record[key]
 
     return parameters
 
 
 def parameters_to_parametersrecord(
     parameters: Parameters, keep_input: bool
 ) -> ParametersRecord:
@@ -91,29 +88,26 @@
     keep_input : bool
         A boolean indicating whether parameters should be deleted from the input
         Parameters object (i.e. a list of serialized NumPy arrays) immediately after
         adding them to the record.
     """
     tensor_type = parameters.tensor_type
 
-    p_record = ParametersRecord()
-
     num_arrays = len(parameters.tensors)
     ordered_dict = OrderedDict()
     for idx in range(num_arrays):
         if keep_input:
             tensor = parameters.tensors[idx]
         else:
             tensor = parameters.tensors.pop(0)
         ordered_dict[str(idx)] = Array(
             data=tensor, dtype="", stype=tensor_type, shape=[]
         )
 
-    p_record.set_parameters(ordered_dict, keep_input=keep_input)
-    return p_record
+    return ParametersRecord(ordered_dict, keep_input=keep_input)
 
 
 def _check_mapping_from_recordscalartype_to_scalar(
     record_data: Mapping[str, Union[ConfigsRecordValues, MetricsRecordValues]]
 ) -> Dict[str, Scalar]:
     """Check mapping `common.*RecordValues` into `common.Scalar` is possible."""
     for value in record_data.values():
@@ -131,61 +125,59 @@
 def _recordset_to_fit_or_evaluate_ins_components(
     recordset: RecordSet,
     ins_str: str,
     keep_input: bool,
 ) -> Tuple[Parameters, Dict[str, Scalar]]:
     """Derive Fit/Evaluate Ins from a RecordSet."""
     # get Array and construct Parameters
-    parameters_record = recordset.get_parameters(f"{ins_str}.parameters")
+    parameters_record = recordset.parameters_records[f"{ins_str}.parameters"]
 
     parameters = parametersrecord_to_parameters(
         parameters_record, keep_input=keep_input
     )
 
     # get config dict
-    config_record = recordset.get_configs(f"{ins_str}.config")
-
-    config_dict = _check_mapping_from_recordscalartype_to_scalar(config_record.data)
+    config_record = recordset.configs_records[f"{ins_str}.config"]
+    # pylint: disable-next=protected-access
+    config_dict = _check_mapping_from_recordscalartype_to_scalar(config_record._data)
 
     return parameters, config_dict
 
 
 def _fit_or_evaluate_ins_to_recordset(
     ins: Union[FitIns, EvaluateIns], keep_input: bool
 ) -> RecordSet:
     recordset = RecordSet()
 
     ins_str = "fitins" if isinstance(ins, FitIns) else "evaluateins"
-    recordset.set_parameters(
-        name=f"{ins_str}.parameters",
-        record=parameters_to_parametersrecord(ins.parameters, keep_input=keep_input),
-    )
+    parametersrecord = parameters_to_parametersrecord(ins.parameters, keep_input)
+    recordset.parameters_records[f"{ins_str}.parameters"] = parametersrecord
 
-    recordset.set_configs(
-        name=f"{ins_str}.config", record=ConfigsRecord(ins.config)  # type: ignore
+    recordset.configs_records[f"{ins_str}.config"] = ConfigsRecord(
+        ins.config  # type: ignore
     )
 
     return recordset
 
 
 def _embed_status_into_recordset(
     res_str: str, status: Status, recordset: RecordSet
 ) -> RecordSet:
     status_dict: Dict[str, ConfigsRecordValues] = {
         "code": int(status.code.value),
         "message": status.message,
     }
     # we add it to a `ConfigsRecord`` because the `status.message`` is a string
     # and `str` values aren't supported in `MetricsRecords`
-    recordset.set_configs(f"{res_str}.status", record=ConfigsRecord(status_dict))
+    recordset.configs_records[f"{res_str}.status"] = ConfigsRecord(status_dict)
     return recordset
 
 
 def _extract_status_from_recordset(res_str: str, recordset: RecordSet) -> Status:
-    status = recordset.get_configs(f"{res_str}.status")
+    status = recordset.configs_records[f"{res_str}.status"]
     code = cast(int, status["code"])
     return Status(code=Code(code), message=str(status["message"]))
 
 
 def recordset_to_fitins(recordset: RecordSet, keep_input: bool) -> FitIns:
     """Derive FitIns from a RecordSet object."""
     parameters, config = _recordset_to_fit_or_evaluate_ins_components(
@@ -202,46 +194,47 @@
     return _fit_or_evaluate_ins_to_recordset(fitins, keep_input)
 
 
 def recordset_to_fitres(recordset: RecordSet, keep_input: bool) -> FitRes:
     """Derive FitRes from a RecordSet object."""
     ins_str = "fitres"
     parameters = parametersrecord_to_parameters(
-        recordset.get_parameters(f"{ins_str}.parameters"), keep_input=keep_input
+        recordset.parameters_records[f"{ins_str}.parameters"], keep_input=keep_input
     )
 
     num_examples = cast(
-        int, recordset.get_metrics(f"{ins_str}.num_examples")["num_examples"]
+        int, recordset.metrics_records[f"{ins_str}.num_examples"]["num_examples"]
     )
-    configs_record = recordset.get_configs(f"{ins_str}.metrics")
-
-    metrics = _check_mapping_from_recordscalartype_to_scalar(configs_record.data)
+    configs_record = recordset.configs_records[f"{ins_str}.metrics"]
+    # pylint: disable-next=protected-access
+    metrics = _check_mapping_from_recordscalartype_to_scalar(configs_record._data)
     status = _extract_status_from_recordset(ins_str, recordset)
 
     return FitRes(
         status=status, parameters=parameters, num_examples=num_examples, metrics=metrics
     )
 
 
 def fitres_to_recordset(fitres: FitRes, keep_input: bool) -> RecordSet:
     """Construct a RecordSet from a FitRes object."""
     recordset = RecordSet()
 
     res_str = "fitres"
 
-    recordset.set_configs(
-        name=f"{res_str}.metrics", record=ConfigsRecord(fitres.metrics)  # type: ignore
+    recordset.configs_records[f"{res_str}.metrics"] = ConfigsRecord(
+        fitres.metrics  # type: ignore
     )
-    recordset.set_metrics(
-        name=f"{res_str}.num_examples",
-        record=MetricsRecord({"num_examples": fitres.num_examples}),
-    )
-    recordset.set_parameters(
-        name=f"{res_str}.parameters",
-        record=parameters_to_parametersrecord(fitres.parameters, keep_input),
+    recordset.metrics_records[f"{res_str}.num_examples"] = MetricsRecord(
+        {"num_examples": fitres.num_examples},
+    )
+    recordset.parameters_records[f"{res_str}.parameters"] = (
+        parameters_to_parametersrecord(
+            fitres.parameters,
+            keep_input,
+        )
     )
 
     # status
     recordset = _embed_status_into_recordset(res_str, fitres.status, recordset)
 
     return recordset
 
@@ -262,90 +255,87 @@
     return _fit_or_evaluate_ins_to_recordset(evaluateins, keep_input)
 
 
 def recordset_to_evaluateres(recordset: RecordSet) -> EvaluateRes:
     """Derive EvaluateRes from a RecordSet object."""
     ins_str = "evaluateres"
 
-    loss = cast(int, recordset.get_metrics(f"{ins_str}.loss")["loss"])
+    loss = cast(int, recordset.metrics_records[f"{ins_str}.loss"]["loss"])
 
     num_examples = cast(
-        int, recordset.get_metrics(f"{ins_str}.num_examples")["num_examples"]
+        int, recordset.metrics_records[f"{ins_str}.num_examples"]["num_examples"]
     )
-    configs_record = recordset.get_configs(f"{ins_str}.metrics")
+    configs_record = recordset.configs_records[f"{ins_str}.metrics"]
 
-    metrics = _check_mapping_from_recordscalartype_to_scalar(configs_record.data)
+    # pylint: disable-next=protected-access
+    metrics = _check_mapping_from_recordscalartype_to_scalar(configs_record._data)
     status = _extract_status_from_recordset(ins_str, recordset)
 
     return EvaluateRes(
         status=status, loss=loss, num_examples=num_examples, metrics=metrics
     )
 
 
 def evaluateres_to_recordset(evaluateres: EvaluateRes) -> RecordSet:
     """Construct a RecordSet from a EvaluateRes object."""
     recordset = RecordSet()
 
     res_str = "evaluateres"
     # loss
-    recordset.set_metrics(
-        name=f"{res_str}.loss",
-        record=MetricsRecord({"loss": evaluateres.loss}),
+    recordset.metrics_records[f"{res_str}.loss"] = MetricsRecord(
+        {"loss": evaluateres.loss},
     )
 
     # num_examples
-    recordset.set_metrics(
-        name=f"{res_str}.num_examples",
-        record=MetricsRecord({"num_examples": evaluateres.num_examples}),
+    recordset.metrics_records[f"{res_str}.num_examples"] = MetricsRecord(
+        {"num_examples": evaluateres.num_examples},
     )
 
     # metrics
-    recordset.set_configs(
-        name=f"{res_str}.metrics",
-        record=ConfigsRecord(evaluateres.metrics),  # type: ignore
+    recordset.configs_records[f"{res_str}.metrics"] = ConfigsRecord(
+        evaluateres.metrics,  # type: ignore
     )
 
     # status
     recordset = _embed_status_into_recordset(
         f"{res_str}", evaluateres.status, recordset
     )
 
     return recordset
 
 
 def recordset_to_getparametersins(recordset: RecordSet) -> GetParametersIns:
     """Derive GetParametersIns from a RecordSet object."""
-    config_record = recordset.get_configs("getparametersins.config")
-
-    config_dict = _check_mapping_from_recordscalartype_to_scalar(config_record.data)
+    config_record = recordset.configs_records["getparametersins.config"]
+    # pylint: disable-next=protected-access
+    config_dict = _check_mapping_from_recordscalartype_to_scalar(config_record._data)
 
     return GetParametersIns(config=config_dict)
 
 
 def getparametersins_to_recordset(getparameters_ins: GetParametersIns) -> RecordSet:
     """Construct a RecordSet from a GetParametersIns object."""
     recordset = RecordSet()
 
-    recordset.set_configs(
-        name="getparametersins.config",
-        record=ConfigsRecord(getparameters_ins.config),  # type: ignore
+    recordset.configs_records["getparametersins.config"] = ConfigsRecord(
+        getparameters_ins.config,  # type: ignore
     )
     return recordset
 
 
 def getparametersres_to_recordset(
     getparametersres: GetParametersRes, keep_input: bool
 ) -> RecordSet:
     """Construct a RecordSet from a GetParametersRes object."""
     recordset = RecordSet()
     res_str = "getparametersres"
     parameters_record = parameters_to_parametersrecord(
         getparametersres.parameters, keep_input=keep_input
     )
-    recordset.set_parameters(f"{res_str}.parameters", parameters_record)
+    recordset.parameters_records[f"{res_str}.parameters"] = parameters_record
 
     # status
     recordset = _embed_status_into_recordset(
         res_str, getparametersres.status, recordset
     )
 
     return recordset
@@ -353,57 +343,57 @@
 
 def recordset_to_getparametersres(
     recordset: RecordSet, keep_input: bool
 ) -> GetParametersRes:
     """Derive GetParametersRes from a RecordSet object."""
     res_str = "getparametersres"
     parameters = parametersrecord_to_parameters(
-        recordset.get_parameters(f"{res_str}.parameters"), keep_input=keep_input
+        recordset.parameters_records[f"{res_str}.parameters"], keep_input=keep_input
     )
 
     status = _extract_status_from_recordset(res_str, recordset)
     return GetParametersRes(status=status, parameters=parameters)
 
 
 def recordset_to_getpropertiesins(recordset: RecordSet) -> GetPropertiesIns:
     """Derive GetPropertiesIns from a RecordSet object."""
-    config_record = recordset.get_configs("getpropertiesins.config")
-    config_dict = _check_mapping_from_recordscalartype_to_scalar(config_record.data)
+    config_record = recordset.configs_records["getpropertiesins.config"]
+    # pylint: disable-next=protected-access
+    config_dict = _check_mapping_from_recordscalartype_to_scalar(config_record._data)
 
     return GetPropertiesIns(config=config_dict)
 
 
 def getpropertiesins_to_recordset(getpropertiesins: GetPropertiesIns) -> RecordSet:
     """Construct a RecordSet from a GetPropertiesRes object."""
     recordset = RecordSet()
-    recordset.set_configs(
-        name="getpropertiesins.config",
-        record=ConfigsRecord(getpropertiesins.config),  # type: ignore
+    recordset.configs_records["getpropertiesins.config"] = ConfigsRecord(
+        getpropertiesins.config,  # type: ignore
     )
     return recordset
 
 
 def recordset_to_getpropertiesres(recordset: RecordSet) -> GetPropertiesRes:
     """Derive GetPropertiesRes from a RecordSet object."""
     res_str = "getpropertiesres"
-    config_record = recordset.get_configs(f"{res_str}.properties")
-    properties = _check_mapping_from_recordscalartype_to_scalar(config_record.data)
+    config_record = recordset.configs_records[f"{res_str}.properties"]
+    # pylint: disable-next=protected-access
+    properties = _check_mapping_from_recordscalartype_to_scalar(config_record._data)
 
     status = _extract_status_from_recordset(res_str, recordset=recordset)
 
     return GetPropertiesRes(status=status, properties=properties)
 
 
 def getpropertiesres_to_recordset(getpropertiesres: GetPropertiesRes) -> RecordSet:
     """Construct a RecordSet from a GetPropertiesRes object."""
     recordset = RecordSet()
     res_str = "getpropertiesres"
-    recordset.set_configs(
-        name=f"{res_str}.properties",
-        record=ConfigsRecord(getpropertiesres.properties),  # type: ignore
+    recordset.configs_records[f"{res_str}.properties"] = ConfigsRecord(
+        getpropertiesres.properties,  # type: ignore
     )
     # status
     recordset = _embed_status_into_recordset(
         res_str, getpropertiesres.status, recordset
     )
 
     return recordset
```

### Comparing `flwr-1.7.0/src/py/flwr/common/retry_invoker.py` & `flwr-1.8.0/src/py/flwr/common/retry_invoker.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 # pylint: disable-next=too-many-instance-attributes
 class RetryInvoker:
     """Wrapper class for retry (with backoff) triggered by exceptions.
 
     Parameters
     ----------
-    wait_factory: Callable[[], Generator[float, None, None]]
+    wait_gen_factory: Callable[[], Generator[float, None, None]]
         A generator yielding successive wait times in seconds. If the generator
         is finite, the giveup event will be triggered when the generator raises
         `StopIteration`.
     recoverable_exceptions: Union[Type[Exception], Tuple[Type[Exception]]]
         An exception type (or tuple of types) that triggers backoff.
     max_tries: Optional[int]
         The maximum number of attempts to make before giving up. Once exhausted,
@@ -125,27 +125,34 @@
         A callable to be executed in the event of success. The parameter is a
         data class object detailing the invocation.
     on_backoff: Optional[Callable[[RetryState], None]] (default: None)
         A callable to be executed in the event of a backoff. The parameter is a
         data class object detailing the invocation.
     on_giveup: Optional[Callable[[RetryState], None]] (default: None)
         A callable to be executed in the event that `max_tries` or `max_time` is
-        exceeded, `should_giveup` returns True, or `wait_factory()` generator raises
+        exceeded, `should_giveup` returns True, or `wait_gen_factory()` generator raises
         `StopInteration`. The parameter is a data class object detailing the
         invocation.
     jitter: Optional[Callable[[float], float]] (default: full_jitter)
-        A function of the value yielded by `wait_factory()` returning the actual time
-        to wait. This function helps distribute wait times stochastically to avoid
+        A function of the value yielded by `wait_gen_factory()` returning the actual
+        time to wait. This function helps distribute wait times stochastically to avoid
         timing collisions across concurrent clients. Wait times are jittered by
         default using the `full_jitter` function. To disable jittering, pass
         `jitter=None`.
     should_giveup: Optional[Callable[[Exception], bool]] (default: None)
         A function accepting an exception instance, returning whether or not
         to give up prematurely before other give-up conditions are evaluated.
         If set to None, the strategy is to never give up prematurely.
+    wait_function: Optional[Callable[[float], None]] (default: None)
+        A function that defines how to wait between retry attempts. It accepts
+        one argument, the wait time in seconds, allowing the use of various waiting
+        mechanisms (e.g., asynchronous waits or event-based synchronization) suitable
+        for different execution environments. If set to `None`, the `wait_function`
+        defaults to `time.sleep`, which is ideal for synchronous operations. Custom
+        functions should manage execution flow to prevent blocking or interference.
 
     Examples
     --------
     Initialize a `RetryInvoker` with exponential backoff and invoke a function:
 
     >>> invoker = RetryInvoker(
     ...     exponential,  # Or use `lambda: exponential(3, 2)` to pass arguments
@@ -155,34 +162,38 @@
     ... )
     >>> invoker.invoke(my_func, arg1, arg2, kw1=kwarg1)
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
-        wait_factory: Callable[[], Generator[float, None, None]],
+        wait_gen_factory: Callable[[], Generator[float, None, None]],
         recoverable_exceptions: Union[Type[Exception], Tuple[Type[Exception], ...]],
         max_tries: Optional[int],
         max_time: Optional[float],
         *,
         on_success: Optional[Callable[[RetryState], None]] = None,
         on_backoff: Optional[Callable[[RetryState], None]] = None,
         on_giveup: Optional[Callable[[RetryState], None]] = None,
         jitter: Optional[Callable[[float], float]] = full_jitter,
         should_giveup: Optional[Callable[[Exception], bool]] = None,
+        wait_function: Optional[Callable[[float], None]] = None,
     ) -> None:
-        self.wait_factory = wait_factory
+        self.wait_gen_factory = wait_gen_factory
         self.recoverable_exceptions = recoverable_exceptions
         self.max_tries = max_tries
         self.max_time = max_time
         self.on_success = on_success
         self.on_backoff = on_backoff
         self.on_giveup = on_giveup
         self.jitter = jitter
         self.should_giveup = should_giveup
+        if wait_function is None:
+            wait_function = time.sleep
+        self.wait_function = wait_function
 
     # pylint: disable-next=too-many-locals
     def invoke(
         self,
         target: Callable[..., Any],
         *args: Any,
         **kwargs: Any,
@@ -208,40 +219,40 @@
         -------
         Any
             The result of the given callable invocation.
 
         Raises
         ------
         Exception
-            If the number of tries exceeds `max_tries`, if the total time
-            exceeds `max_time`, if `wait_factory()` generator raises `StopInteration`,
+            If the number of tries exceeds `max_tries`, if the total time exceeds
+            `max_time`, if `wait_gen_factory()` generator raises `StopInteration`,
             or if the `should_giveup` returns True for a raised exception.
 
         Notes
         -----
-        The time between retries is determined by the provided `wait_factory()`
+        The time between retries is determined by the provided `wait_gen_factory()`
         generator and can optionally be jittered using the `jitter` function.
         The recoverable exceptions that trigger a retry, as well as conditions to
         stop retries, are also determined by the class's initialization parameters.
         """
 
         def try_call_event_handler(
             handler: Optional[Callable[[RetryState], None]]
         ) -> None:
             if handler is not None:
                 handler(cast(RetryState, ref_state[0]))
 
         try_cnt = 0
-        wait_generator = self.wait_factory()
-        start = time.time()
+        wait_generator = self.wait_gen_factory()
+        start = time.monotonic()
         ref_state: List[Optional[RetryState]] = [None]
 
         while True:
             try_cnt += 1
-            elapsed_time = time.time() - start
+            elapsed_time = time.monotonic() - start
             state = RetryState(
                 target=target,
                 args=args,
                 kwargs=kwargs,
                 tries=try_cnt,
                 elapsed_time=elapsed_time,
             )
@@ -278,12 +289,12 @@
                     try_call_event_handler(self.on_giveup)
                     raise err from None
 
                 # Trigger backoff event
                 try_call_event_handler(self.on_backoff)
 
                 # Sleep
-                time.sleep(wait_time)
+                self.wait_function(state.actual_wait)
             else:
                 # Trigger success event
                 try_call_event_handler(self.on_success)
                 return ret
```

### Comparing `flwr-1.7.0/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr-1.8.0/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr-1.8.0/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr-1.8.0/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr-1.8.0/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr-1.8.0/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Utility functions for performing operations on Numpy NDArrays."""
 
 
-from typing import Any, List, Tuple
+from typing import Any, List, Tuple, Union
 
 import numpy as np
 from numpy.typing import DTypeLike, NDArray
 
 
 def factor_combine(factor: int, parameters: List[NDArray[Any]]) -> List[NDArray[Any]]:
     """Combine factor with parameters."""
@@ -64,18 +64,18 @@
     if bin(divisor).count("1") == 1:
         msk = divisor - 1
         return [parameters[idx] & msk for idx in range(len(parameters))]
     return [parameters[idx] % divisor for idx in range(len(parameters))]
 
 
 def parameters_multiply(
-    parameters: List[NDArray[Any]], multiplier: int
+    parameters: List[NDArray[Any]], multiplier: Union[int, float]
 ) -> List[NDArray[Any]]:
-    """Multiply parameters by an integer multiplier."""
+    """Multiply parameters by an integer/float multiplier."""
     return [parameters[idx] * multiplier for idx in range(len(parameters))]
 
 
 def parameters_divide(
-    parameters: List[NDArray[Any]], divisor: int
+    parameters: List[NDArray[Any]], divisor: Union[int, float]
 ) -> List[NDArray[Any]]:
-    """Divide weight by an integer divisor."""
+    """Divide weight by an integer/float divisor."""
     return [parameters[idx] / divisor for idx in range(len(parameters))]
```

### Comparing `flwr-1.7.0/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr-1.8.0/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr-1.8.0/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,38 +19,38 @@
 
 import numpy as np
 
 from flwr.common.typing import NDArrayInt
 
 
 def share_keys_plaintext_concat(
-    source: int, destination: int, b_share: bytes, sk_share: bytes
+    src_node_id: int, dst_node_id: int, b_share: bytes, sk_share: bytes
 ) -> bytes:
     """Combine arguments to bytes.
 
     Parameters
     ----------
-    source : int
-        the secure ID of the source.
-    destination : int
-        the secure ID of the destination.
+    src_node_id : int
+        the node ID of the source.
+    dst_node_id : int
+        the node ID of the destination.
     b_share : bytes
         the private key share of the source sent to the destination.
     sk_share : bytes
         the secret key share of the source sent to the destination.
 
     Returns
     -------
     bytes
         The combined bytes of all the arguments.
     """
     return b"".join(
         [
-            int.to_bytes(source, 4, "little"),
-            int.to_bytes(destination, 4, "little"),
+            int.to_bytes(src_node_id, 8, "little", signed=True),
+            int.to_bytes(dst_node_id, 8, "little", signed=True),
             int.to_bytes(len(b_share), 4, "little"),
             b_share,
             sk_share,
         ]
     )
 
 
@@ -60,29 +60,29 @@
     Parameters
     ----------
     plaintext : bytes
         the bytes containing 4 arguments.
 
     Returns
     -------
-    source : int
-        the secure ID of the source.
-    destination : int
-        the secure ID of the destination.
+    src_node_id : int
+        the node ID of the source.
+    dst_node_id : int
+        the node ID of the destination.
     b_share : bytes
         the private key share of the source sent to the destination.
     sk_share : bytes
         the secret key share of the source sent to the destination.
     """
     src, dst, mark = (
-        int.from_bytes(plaintext[:4], "little"),
-        int.from_bytes(plaintext[4:8], "little"),
-        int.from_bytes(plaintext[8:12], "little"),
+        int.from_bytes(plaintext[:8], "little", signed=True),
+        int.from_bytes(plaintext[8:16], "little", signed=True),
+        int.from_bytes(plaintext[16:20], "little"),
     )
-    ret = (src, dst, plaintext[12 : 12 + mark], plaintext[12 + mark :])
+    ret = (src, dst, plaintext[20 : 20 + mark], plaintext[20 + mark :])
     return ret
 
 
 def pseudo_rand_gen(
     seed: bytes, num_range: int, dimensions_list: List[Tuple[int, ...]]
 ) -> List[NDArrayInt]:
     """Seeded pseudo-random number generator for noise generation with Numpy."""
```

### Comparing `flwr-1.7.0/src/py/flwr/common/serde.py` & `flwr-1.8.0/src/py/flwr/common/serde.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 
 from typing import Any, Dict, List, MutableMapping, OrderedDict, Type, TypeVar, cast
 
 from google.protobuf.message import Message as GrpcMessage
 
 # pylint: disable=E0611
+from flwr.proto.error_pb2 import Error as ProtoError
+from flwr.proto.node_pb2 import Node
 from flwr.proto.recordset_pb2 import Array as ProtoArray
 from flwr.proto.recordset_pb2 import BoolList, BytesList
 from flwr.proto.recordset_pb2 import ConfigsRecord as ProtoConfigsRecord
 from flwr.proto.recordset_pb2 import ConfigsRecordValue as ProtoConfigsRecordValue
 from flwr.proto.recordset_pb2 import DoubleList
 from flwr.proto.recordset_pb2 import MetricsRecord as ProtoMetricsRecord
 from flwr.proto.recordset_pb2 import MetricsRecordValue as ProtoMetricsRecordValue
@@ -38,20 +40,17 @@
     Reason,
     Scalar,
     ServerMessage,
     Status,
 )
 
 # pylint: enable=E0611
-from . import typing
-from .configsrecord import ConfigsRecord
-from .message import Message, Metadata
-from .metricsrecord import MetricsRecord
-from .parametersrecord import Array, ParametersRecord
-from .recordset import RecordSet
+from . import Array, ConfigsRecord, MetricsRecord, ParametersRecord, RecordSet, typing
+from .message import Error, Message, Metadata
+from .record.typeddict import TypedDict
 
 #  === Parameters message ===
 
 
 def parameters_to_proto(parameters: typing.Parameters) -> Parameters:
     """Serialize `Parameters` to ProtoBuf."""
     return Parameters(tensors=parameters.tensors, tensor_type=parameters.tensor_type)
@@ -409,15 +408,17 @@
         value = list(getattr(value_proto, value_field).vals)
     else:
         value = getattr(value_proto, value_field)
     return value
 
 
 def _record_value_dict_to_proto(
-    value_dict: Dict[str, Any], allowed_types: List[type], value_proto_class: Type[T]
+    value_dict: TypedDict[str, Any],
+    allowed_types: List[type],
+    value_proto_class: Type[T],
 ) -> Dict[str, T]:
     """Serialize the record value dict to ProtoBuf.
 
     Note: `bool` MUST be put in the front of allowd_types if it exists.
     """
     # Move bool to the front
     if bool in allowed_types and allowed_types[0] != bool:
@@ -451,16 +452,16 @@
         data=array_proto.data,
     )
 
 
 def parameters_record_to_proto(record: ParametersRecord) -> ProtoParametersRecord:
     """Serialize ParametersRecord to ProtoBuf."""
     return ProtoParametersRecord(
-        data_keys=record.data.keys(),
-        data_values=map(array_to_proto, record.data.values()),
+        data_keys=record.keys(),
+        data_values=map(array_to_proto, record.values()),
     )
 
 
 def parameters_record_from_proto(
     record_proto: ProtoParametersRecord,
 ) -> ParametersRecord:
     """Deserialize ParametersRecord from ProtoBuf."""
@@ -471,17 +472,15 @@
         keep_input=False,
     )
 
 
 def metrics_record_to_proto(record: MetricsRecord) -> ProtoMetricsRecord:
     """Serialize MetricsRecord to ProtoBuf."""
     return ProtoMetricsRecord(
-        data=_record_value_dict_to_proto(
-            record.data, [float, int], ProtoMetricsRecordValue
-        )
+        data=_record_value_dict_to_proto(record, [float, int], ProtoMetricsRecordValue)
     )
 
 
 def metrics_record_from_proto(record_proto: ProtoMetricsRecord) -> MetricsRecord:
     """Deserialize MetricsRecord from ProtoBuf."""
     return MetricsRecord(
         metrics_dict=cast(
@@ -492,15 +491,17 @@
     )
 
 
 def configs_record_to_proto(record: ConfigsRecord) -> ProtoConfigsRecord:
     """Serialize ConfigsRecord to ProtoBuf."""
     return ProtoConfigsRecord(
         data=_record_value_dict_to_proto(
-            record.data, [bool, int, float, str, bytes], ProtoConfigsRecordValue
+            record,
+            [bool, int, float, str, bytes],
+            ProtoConfigsRecordValue,
         )
     )
 
 
 def configs_record_from_proto(record_proto: ProtoConfigsRecord) -> ConfigsRecord:
     """Deserialize ConfigsRecord from ProtoBuf."""
     return ConfigsRecord(
@@ -508,96 +509,165 @@
             Dict[str, typing.ConfigsRecordValues],
             _record_value_dict_from_proto(record_proto.data),
         ),
         keep_input=False,
     )
 
 
+# === Error message ===
+
+
+def error_to_proto(error: Error) -> ProtoError:
+    """Serialize Error to ProtoBuf."""
+    reason = error.reason if error.reason else ""
+    return ProtoError(code=error.code, reason=reason)
+
+
+def error_from_proto(error_proto: ProtoError) -> Error:
+    """Deserialize Error from ProtoBuf."""
+    reason = error_proto.reason if len(error_proto.reason) > 0 else None
+    return Error(code=error_proto.code, reason=reason)
+
+
 # === RecordSet message ===
 
 
 def recordset_to_proto(recordset: RecordSet) -> ProtoRecordSet:
     """Serialize RecordSet to ProtoBuf."""
     return ProtoRecordSet(
         parameters={
-            k: parameters_record_to_proto(v) for k, v in recordset.parameters.items()
+            k: parameters_record_to_proto(v)
+            for k, v in recordset.parameters_records.items()
+        },
+        metrics={
+            k: metrics_record_to_proto(v) for k, v in recordset.metrics_records.items()
+        },
+        configs={
+            k: configs_record_to_proto(v) for k, v in recordset.configs_records.items()
         },
-        metrics={k: metrics_record_to_proto(v) for k, v in recordset.metrics.items()},
-        configs={k: configs_record_to_proto(v) for k, v in recordset.configs.items()},
     )
 
 
 def recordset_from_proto(recordset_proto: ProtoRecordSet) -> RecordSet:
     """Deserialize RecordSet from ProtoBuf."""
     return RecordSet(
-        parameters={
+        parameters_records={
             k: parameters_record_from_proto(v)
             for k, v in recordset_proto.parameters.items()
         },
-        metrics={
+        metrics_records={
             k: metrics_record_from_proto(v) for k, v in recordset_proto.metrics.items()
         },
-        configs={
+        configs_records={
             k: configs_record_from_proto(v) for k, v in recordset_proto.configs.items()
         },
     )
 
 
 # === Message ===
 
 
 def message_to_taskins(message: Message) -> TaskIns:
     """Create a TaskIns from the Message."""
+    md = message.metadata
     return TaskIns(
+        group_id=md.group_id,
+        run_id=md.run_id,
         task=Task(
-            ttl=message.metadata.ttl,
-            task_type=message.metadata.task_type,
-            recordset=recordset_to_proto(message.message),
+            producer=Node(node_id=0, anonymous=True),  # Assume driver node
+            consumer=Node(node_id=md.dst_node_id, anonymous=False),
+            created_at=md.created_at,
+            ttl=md.ttl,
+            ancestry=[md.reply_to_message] if md.reply_to_message != "" else [],
+            task_type=md.message_type,
+            recordset=(
+                recordset_to_proto(message.content) if message.has_content() else None
+            ),
+            error=error_to_proto(message.error) if message.has_error() else None,
         ),
     )
 
 
 def message_from_taskins(taskins: TaskIns) -> Message:
     """Create a Message from the TaskIns."""
     # Retrieve the Metadata
     metadata = Metadata(
         run_id=taskins.run_id,
-        task_id=taskins.task_id,
+        message_id=taskins.task_id,
+        src_node_id=taskins.task.producer.node_id,
+        dst_node_id=taskins.task.consumer.node_id,
+        reply_to_message=taskins.task.ancestry[0] if taskins.task.ancestry else "",
         group_id=taskins.group_id,
         ttl=taskins.task.ttl,
-        task_type=taskins.task.task_type,
+        message_type=taskins.task.task_type,
     )
 
-    # Return the Message
-    return Message(
+    # Construct Message
+    message = Message(
         metadata=metadata,
-        message=recordset_from_proto(taskins.task.recordset),
+        content=(
+            recordset_from_proto(taskins.task.recordset)
+            if taskins.task.HasField("recordset")
+            else None
+        ),
+        error=(
+            error_from_proto(taskins.task.error)
+            if taskins.task.HasField("error")
+            else None
+        ),
     )
+    message.metadata.created_at = taskins.task.created_at
+    return message
 
 
 def message_to_taskres(message: Message) -> TaskRes:
     """Create a TaskRes from the Message."""
+    md = message.metadata
     return TaskRes(
+        task_id="",  # This will be generated by the server
+        group_id=md.group_id,
+        run_id=md.run_id,
         task=Task(
-            ttl=message.metadata.ttl,
-            task_type=message.metadata.task_type,
-            recordset=recordset_to_proto(message.message),
+            producer=Node(node_id=md.src_node_id, anonymous=False),
+            consumer=Node(node_id=0, anonymous=True),  # Assume driver node
+            created_at=md.created_at,
+            ttl=md.ttl,
+            ancestry=[md.reply_to_message] if md.reply_to_message != "" else [],
+            task_type=md.message_type,
+            recordset=(
+                recordset_to_proto(message.content) if message.has_content() else None
+            ),
+            error=error_to_proto(message.error) if message.has_error() else None,
         ),
     )
 
 
 def message_from_taskres(taskres: TaskRes) -> Message:
     """Create a Message from the TaskIns."""
     # Retrieve the MetaData
     metadata = Metadata(
         run_id=taskres.run_id,
-        task_id=taskres.task_id,
+        message_id=taskres.task_id,
+        src_node_id=taskres.task.producer.node_id,
+        dst_node_id=taskres.task.consumer.node_id,
+        reply_to_message=taskres.task.ancestry[0] if taskres.task.ancestry else "",
         group_id=taskres.group_id,
         ttl=taskres.task.ttl,
-        task_type=taskres.task.task_type,
+        message_type=taskres.task.task_type,
     )
 
-    # Return the Message
-    return Message(
+    # Construct the Message
+    message = Message(
         metadata=metadata,
-        message=recordset_from_proto(taskres.task.recordset),
+        content=(
+            recordset_from_proto(taskres.task.recordset)
+            if taskres.task.HasField("recordset")
+            else None
+        ),
+        error=(
+            error_from_proto(taskres.task.error)
+            if taskres.task.HasField("error")
+            else None
+        ),
     )
+    message.metadata.created_at = taskres.task.created_at
+    return message
```

### Comparing `flwr-1.7.0/src/py/flwr/common/telemetry.py` & `flwr-1.8.0/src/py/flwr/common/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from typing import Any, Dict, List, Optional, Union, cast
 
 from flwr.common.version import package_name, package_version
 
 FLWR_TELEMETRY_ENABLED = os.getenv("FLWR_TELEMETRY_ENABLED", "1")
 FLWR_TELEMETRY_LOGGING = os.getenv("FLWR_TELEMETRY_LOGGING", "0")
 
-TELEMETRY_EVENTS_URL = "https://telemetry.flower.dev/api/v1/event"
+TELEMETRY_EVENTS_URL = "https://telemetry.flower.ai/api/v1/event"
 
 LOGGER_NAME = "flwr-telemetry"
 LOGGER_LEVEL = logging.DEBUG
 
 
 def _configure_logger(log_level: int) -> None:
     console_handler = logging.StreamHandler()
@@ -133,32 +133,36 @@
     RUN_DRIVER_API_LEAVE = auto()
 
     # Fleet API
     RUN_FLEET_API_ENTER = auto()
     RUN_FLEET_API_LEAVE = auto()
 
     # Driver API and Fleet API
-    RUN_SERVER_ENTER = auto()
-    RUN_SERVER_LEAVE = auto()
+    RUN_SUPERLINK_ENTER = auto()
+    RUN_SUPERLINK_LEAVE = auto()
 
     # Simulation
     START_SIMULATION_ENTER = auto()
     START_SIMULATION_LEAVE = auto()
 
     # Driver: Driver
     DRIVER_CONNECT = auto()
     DRIVER_DISCONNECT = auto()
 
     # Driver: start_driver
     START_DRIVER_ENTER = auto()
     START_DRIVER_LEAVE = auto()
 
-    # SuperNode: flower-client
-    RUN_CLIENT_ENTER = auto()
-    RUN_CLIENT_LEAVE = auto()
+    # flower-client-app
+    RUN_CLIENT_APP_ENTER = auto()
+    RUN_CLIENT_APP_LEAVE = auto()
+
+    # flower-server-app
+    RUN_SERVER_APP_ENTER = auto()
+    RUN_SERVER_APP_LEAVE = auto()
 
 
 # Use the ThreadPoolExecutor with max_workers=1 to have a queue
 # and also ensure that telemetry calls are not blocking.
 state: Dict[str, Union[Optional[str], Optional[ThreadPoolExecutor]]] = {
     # Will be assigned ThreadPoolExecutor(max_workers=1)
     # in event() the first time it's required
```

### Comparing `flwr-1.7.0/src/py/flwr/common/typing.py` & `flwr-1.8.0/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/common/version.py` & `flwr-1.8.0/src/py/flwr/common/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Flower package version helper."""
 
-
 import importlib.metadata as importlib_metadata
 from typing import Tuple
 
 
 def _check_package(name: str) -> Tuple[str, str]:
     version: str = importlib_metadata.version(name)
     return name, version
```

### Comparing `flwr-1.7.0/src/py/flwr/driver/__init__.py` & `flwr-1.8.0/src/py/flwr/server/driver/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower driver SDK."""
 
 
-from .app import start_driver
 from .driver import Driver
 from .grpc_driver import GrpcDriver
 
 __all__ = [
     "Driver",
     "GrpcDriver",
-    "start_driver",
 ]
```

### Comparing `flwr-1.7.0/src/py/flwr/driver/app.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedavgm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,213 +1,200 @@
-# Copyright 2022 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2020 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower driver app."""
+"""Federated Averaging with Momentum (FedAvgM) [Hsu et al., 2019] strategy.
+
+Paper: arxiv.org/pdf/1909.06335.pdf
+"""
 
 
-import sys
-import threading
-import time
-from logging import INFO
-from pathlib import Path
-from typing import Dict, Optional, Union
+from logging import WARNING
+from typing import Callable, Dict, List, Optional, Tuple, Union
 
-from flwr.common import EventType, event
-from flwr.common.address import parse_address
+from flwr.common import (
+    FitRes,
+    MetricsAggregationFn,
+    NDArrays,
+    Parameters,
+    Scalar,
+    ndarrays_to_parameters,
+    parameters_to_ndarrays,
+)
 from flwr.common.logger import log
-from flwr.proto import driver_pb2  # pylint: disable=E0611
-from flwr.server.app import ServerConfig, init_defaults, run_fl
 from flwr.server.client_manager import ClientManager
-from flwr.server.history import History
-from flwr.server.server import Server
-from flwr.server.strategy import Strategy
-
-from .driver_client_proxy import DriverClientProxy
-from .grpc_driver import GrpcDriver
+from flwr.server.client_proxy import ClientProxy
 
-DEFAULT_SERVER_ADDRESS_DRIVER = "[::]:9091"
+from .aggregate import aggregate
+from .fedavg import FedAvg
 
-ERROR_MESSAGE_DRIVER_NOT_CONNECTED = """
-[Driver] Error: Not connected.
-
-Call `connect()` on the `Driver` instance before calling any of the other `Driver`
-methods.
-"""
 
+# pylint: disable=line-too-long
+class FedAvgM(FedAvg):
+    """Federated Averaging with Momentum strategy.
 
-def start_driver(  # pylint: disable=too-many-arguments, too-many-locals
-    *,
-    server_address: str = DEFAULT_SERVER_ADDRESS_DRIVER,
-    server: Optional[Server] = None,
-    config: Optional[ServerConfig] = None,
-    strategy: Optional[Strategy] = None,
-    client_manager: Optional[ClientManager] = None,
-    root_certificates: Optional[Union[bytes, str]] = None,
-) -> History:
-    """Start a Flower Driver API server.
+    Implementation based on https://arxiv.org/abs/1909.06335
 
     Parameters
     ----------
-    server_address : Optional[str]
-        The IPv4 or IPv6 address of the Driver API server.
-        Defaults to `"[::]:8080"`.
-    server : Optional[flwr.server.Server] (default: None)
-        A server implementation, either `flwr.server.Server` or a subclass
-        thereof. If no instance is provided, then `start_driver` will create
-        one.
-    config : Optional[ServerConfig] (default: None)
-        Currently supported values are `num_rounds` (int, default: 1) and
-        `round_timeout` in seconds (float, default: None).
-    strategy : Optional[flwr.server.Strategy] (default: None).
-        An implementation of the abstract base class
-        `flwr.server.strategy.Strategy`. If no strategy is provided, then
-        `start_server` will use `flwr.server.strategy.FedAvg`.
-    client_manager : Optional[flwr.server.DriverClientManager] (default: None)
-        An implementation of the class `flwr.server.ClientManager`. If no
-        implementation is provided, then `start_driver` will use
-        `flwr.server.SimpleClientManager`.
-    root_certificates : Optional[Union[bytes, str]] (default: None)
-        The PEM-encoded root certificates as a byte string or a path string.
-        If provided, a secure connection using the certificates will be
-        established to an SSL-enabled Flower server.
-
-    Returns
-    -------
-    hist : flwr.server.history.History
-        Object containing training and evaluation metrics.
-
-    Examples
-    --------
-    Starting a driver that connects to an insecure server:
-
-    >>> start_driver()
-
-    Starting a driver that connects to an SSL-enabled server:
-
-    >>> start_driver(
-    >>>     root_certificates=Path("/crts/root.pem").read_bytes()
-    >>> )
+    fraction_fit : float, optional
+        Fraction of clients used during training. Defaults to 1.0.
+    fraction_evaluate : float, optional
+        Fraction of clients used during validation. Defaults to 1.0.
+    min_fit_clients : int, optional
+        Minimum number of clients used during training. Defaults to 2.
+    min_evaluate_clients : int, optional
+        Minimum number of clients used during validation. Defaults to 2.
+    min_available_clients : int, optional
+        Minimum number of total clients in the system. Defaults to 2.
+    evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
+        Optional function used for validation. Defaults to None.
+    on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
+        Function used to configure training. Defaults to None.
+    on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
+        Function used to configure validation. Defaults to None.
+    accept_failures : bool, optional
+        Whether or not accept rounds containing failures. Defaults to True.
+    initial_parameters : Parameters, optional
+        Initial global model parameters.
+    server_learning_rate: float
+        Server-side learning rate used in server-side optimization.
+        Defaults to 1.0.
+    server_momentum: float
+        Server-side momentum factor used for FedAvgM. Defaults to 0.0.
     """
-    event(EventType.START_DRIVER_ENTER)
 
-    # Parse IP address
-    parsed_address = parse_address(server_address)
-    if not parsed_address:
-        sys.exit(f"Server IP address ({server_address}) cannot be parsed.")
-    host, port, is_v6 = parsed_address
-    address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
-
-    # Create the Driver
-    if isinstance(root_certificates, str):
-        root_certificates = Path(root_certificates).read_bytes()
-    driver = GrpcDriver(
-        driver_service_address=address, root_certificates=root_certificates
-    )
-    driver.connect()
-    lock = threading.Lock()
-
-    # Initialize the Driver API server and config
-    initialized_server, initialized_config = init_defaults(
-        server=server,
-        config=config,
-        strategy=strategy,
-        client_manager=client_manager,
-    )
-    log(
-        INFO,
-        "Starting Flower server, config: %s",
-        initialized_config,
-    )
-
-    # Start the thread updating nodes
-    thread = threading.Thread(
-        target=update_client_manager,
-        args=(
-            driver,
-            initialized_server.client_manager(),
-            lock,
-        ),
-    )
-    thread.start()
-
-    # Start training
-    hist = run_fl(
-        server=initialized_server,
-        config=initialized_config,
-    )
-
-    # Stop the Driver API server and the thread
-    with lock:
-        driver.disconnect()
-    thread.join()
-
-    event(EventType.START_SERVER_LEAVE)
-
-    return hist
-
-
-def update_client_manager(
-    driver: GrpcDriver,
-    client_manager: ClientManager,
-    lock: threading.Lock,
-) -> None:
-    """Update the nodes list in the client manager.
-
-    This function periodically communicates with the associated driver to get all
-    node_ids. Each node_id is then converted into a `DriverClientProxy` instance
-    and stored in the `registered_nodes` dictionary with node_id as key.
-
-    New nodes will be added to the ClientManager via `client_manager.register()`,
-    and dead nodes will be removed from the ClientManager via
-    `client_manager.unregister()`.
-    """
-    # Request for run_id
-    run_id = driver.create_run(
-        driver_pb2.CreateRunRequest()  # pylint: disable=E1101
-    ).run_id
-
-    # Loop until the driver is disconnected
-    registered_nodes: Dict[int, DriverClientProxy] = {}
-    while True:
-        with lock:
-            # End the while loop if the driver is disconnected
-            if driver.stub is None:
-                break
-            get_nodes_res = driver.get_nodes(
-                req=driver_pb2.GetNodesRequest(run_id=run_id)  # pylint: disable=E1101
-            )
-        all_node_ids = {node.node_id for node in get_nodes_res.nodes}
-        dead_nodes = set(registered_nodes).difference(all_node_ids)
-        new_nodes = all_node_ids.difference(registered_nodes)
-
-        # Unregister dead nodes
-        for node_id in dead_nodes:
-            client_proxy = registered_nodes[node_id]
-            client_manager.unregister(client_proxy)
-            del registered_nodes[node_id]
-
-        # Register new nodes
-        for node_id in new_nodes:
-            client_proxy = DriverClientProxy(
-                node_id=node_id,
-                driver=driver,
-                anonymous=False,
-                run_id=run_id,
-            )
-            if client_manager.register(client_proxy):
-                registered_nodes[node_id] = client_proxy
-            else:
-                raise RuntimeError("Could not register node.")
+    # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
+    def __init__(
+        self,
+        *,
+        fraction_fit: float = 1.0,
+        fraction_evaluate: float = 1.0,
+        min_fit_clients: int = 2,
+        min_evaluate_clients: int = 2,
+        min_available_clients: int = 2,
+        evaluate_fn: Optional[
+            Callable[
+                [int, NDArrays, Dict[str, Scalar]],
+                Optional[Tuple[float, Dict[str, Scalar]]],
+            ]
+        ] = None,
+        on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
+        on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
+        accept_failures: bool = True,
+        initial_parameters: Optional[Parameters] = None,
+        fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
+        evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
+        server_learning_rate: float = 1.0,
+        server_momentum: float = 0.0,
+    ) -> None:
+        super().__init__(
+            fraction_fit=fraction_fit,
+            fraction_evaluate=fraction_evaluate,
+            min_fit_clients=min_fit_clients,
+            min_evaluate_clients=min_evaluate_clients,
+            min_available_clients=min_available_clients,
+            evaluate_fn=evaluate_fn,
+            on_fit_config_fn=on_fit_config_fn,
+            on_evaluate_config_fn=on_evaluate_config_fn,
+            accept_failures=accept_failures,
+            initial_parameters=initial_parameters,
+            fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
+            evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
+        )
+        self.server_learning_rate = server_learning_rate
+        self.server_momentum = server_momentum
+        self.server_opt: bool = (self.server_momentum != 0.0) or (
+            self.server_learning_rate != 1.0
+        )
+        self.momentum_vector: Optional[NDArrays] = None
+
+    def __repr__(self) -> str:
+        """Compute a string representation of the strategy."""
+        rep = f"FedAvgM(accept_failures={self.accept_failures})"
+        return rep
+
+    def initialize_parameters(
+        self, client_manager: ClientManager
+    ) -> Optional[Parameters]:
+        """Initialize global model parameters."""
+        return self.initial_parameters
+
+    def aggregate_fit(
+        self,
+        server_round: int,
+        results: List[Tuple[ClientProxy, FitRes]],
+        failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
+    ) -> Tuple[Optional[Parameters], Dict[str, Scalar]]:
+        """Aggregate fit results using weighted average."""
+        if not results:
+            return None, {}
+        # Do not aggregate if there are failures and failures are not accepted
+        if not self.accept_failures and failures:
+            return None, {}
+        # Convert results
+        weights_results = [
+            (parameters_to_ndarrays(fit_res.parameters), fit_res.num_examples)
+            for _, fit_res in results
+        ]
+
+        fedavg_result = aggregate(weights_results)
+        # following convention described in
+        # https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
+        if self.server_opt:
+            # You need to initialize the model
+            assert (
+                self.initial_parameters is not None
+            ), "When using server-side optimization, model needs to be initialized."
+            initial_weights = parameters_to_ndarrays(self.initial_parameters)
+
+            # remember that updates are the opposite of gradients
+            pseudo_gradient: NDArrays = [
+                x - y
+                for x, y in zip(
+                    parameters_to_ndarrays(self.initial_parameters), fedavg_result
+                )
+            ]
+            if self.server_momentum > 0.0:
+                if server_round > 1:
+                    assert (
+                        self.momentum_vector
+                    ), "Momentum should have been created on round 1."
+                    self.momentum_vector = [
+                        self.server_momentum * x + y
+                        for x, y in zip(self.momentum_vector, pseudo_gradient)
+                    ]
+                else:
+                    self.momentum_vector = pseudo_gradient
+
+                # No nesterov for now
+                pseudo_gradient = self.momentum_vector
+
+            # SGD
+            fedavg_result = [
+                x - self.server_learning_rate * y
+                for x, y in zip(initial_weights, pseudo_gradient)
+            ]
+            # Update current weights
+            self.initial_parameters = ndarrays_to_parameters(fedavg_result)
+
+        parameters_aggregated = ndarrays_to_parameters(fedavg_result)
+
+        # Aggregate custom metrics if aggregation fn was provided
+        metrics_aggregated = {}
+        if self.fit_metrics_aggregation_fn:
+            fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
+            metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
+        elif server_round == 1:  # Only log this warning once
+            log(WARNING, "No fit_metrics_aggregation_fn provided")
 
-        # Sleep for 3 seconds
-        time.sleep(3)
+        return parameters_aggregated, metrics_aggregated
```

### Comparing `flwr-1.7.0/src/py/flwr/driver/driver.py` & `flwr-1.8.0/src/py/flwr/server/driver/grpc_driver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2023 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,101 +11,119 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower driver service client."""
 
 
-from typing import Iterable, List, Optional, Tuple
+from logging import DEBUG, ERROR, WARNING
+from typing import Optional
 
-from flwr.driver.grpc_driver import DEFAULT_SERVER_ADDRESS_DRIVER, GrpcDriver
+import grpc
+
+from flwr.common import EventType, event
+from flwr.common.grpc import create_channel
+from flwr.common.logger import log
 from flwr.proto.driver_pb2 import (  # pylint: disable=E0611
     CreateRunRequest,
+    CreateRunResponse,
     GetNodesRequest,
+    GetNodesResponse,
     PullTaskResRequest,
+    PullTaskResResponse,
     PushTaskInsRequest,
+    PushTaskInsResponse,
 )
-from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
-from flwr.proto.task_pb2 import TaskIns, TaskRes  # pylint: disable=E0611
+from flwr.proto.driver_pb2_grpc import DriverStub  # pylint: disable=E0611
+
+DEFAULT_SERVER_ADDRESS_DRIVER = "[::]:9091"
 
+ERROR_MESSAGE_DRIVER_NOT_CONNECTED = """
+[Driver] Error: Not connected.
 
-class Driver:
-    """`Driver` class provides an interface to the Driver API.
+Call `connect()` on the `GrpcDriver` instance before calling any of the other
+`GrpcDriver` methods.
+"""
 
-    Parameters
-    ----------
-    driver_service_address : Optional[str]
-        The IPv4 or IPv6 address of the Driver API server.
-        Defaults to `"[::]:9091"`.
-    certificates : bytes (default: None)
-        Tuple containing root certificate, server certificate, and private key
-        to start a secure SSL-enabled server. The tuple is expected to have
-        three bytes elements in the following order:
-
-            * CA certificate.
-            * server certificate.
-            * server private key.
-    """
+
+class GrpcDriver:
+    """`GrpcDriver` provides access to the gRPC Driver API/service."""
 
     def __init__(
         self,
         driver_service_address: str = DEFAULT_SERVER_ADDRESS_DRIVER,
         root_certificates: Optional[bytes] = None,
     ) -> None:
-        self.addr = driver_service_address
+        self.driver_service_address = driver_service_address
         self.root_certificates = root_certificates
-        self.grpc_driver: Optional[GrpcDriver] = None
-        self.run_id: Optional[int] = None
-        self.node = Node(node_id=0, anonymous=True)
-
-    def _get_grpc_driver_and_run_id(self) -> Tuple[GrpcDriver, int]:
-        # Check if the GrpcDriver is initialized
-        if self.grpc_driver is None or self.run_id is None:
-            # Connect and create run
-            self.grpc_driver = GrpcDriver(
-                driver_service_address=self.addr,
-                root_certificates=self.root_certificates,
-            )
-            self.grpc_driver.connect()
-            res = self.grpc_driver.create_run(CreateRunRequest())
-            self.run_id = res.run_id
-
-        return self.grpc_driver, self.run_id
-
-    def get_nodes(self) -> List[Node]:
-        """Get node IDs."""
-        grpc_driver, run_id = self._get_grpc_driver_and_run_id()
-
-        # Call GrpcDriver method
-        res = grpc_driver.get_nodes(GetNodesRequest(run_id=run_id))
-        return list(res.nodes)
-
-    def push_task_ins(self, task_ins_list: List[TaskIns]) -> List[str]:
-        """Schedule tasks."""
-        grpc_driver, run_id = self._get_grpc_driver_and_run_id()
-
-        # Set run_id
-        for task_ins in task_ins_list:
-            task_ins.run_id = run_id
-
-        # Call GrpcDriver method
-        res = grpc_driver.push_task_ins(PushTaskInsRequest(task_ins_list=task_ins_list))
-        return list(res.task_ids)
+        self.channel: Optional[grpc.Channel] = None
+        self.stub: Optional[DriverStub] = None
 
-    def pull_task_res(self, task_ids: Iterable[str]) -> List[TaskRes]:
-        """Get task results."""
-        grpc_driver, _ = self._get_grpc_driver_and_run_id()
-
-        # Call GrpcDriver method
-        res = grpc_driver.pull_task_res(
-            PullTaskResRequest(node=self.node, task_ids=task_ids)
+    def connect(self) -> None:
+        """Connect to the Driver API."""
+        event(EventType.DRIVER_CONNECT)
+        if self.channel is not None or self.stub is not None:
+            log(WARNING, "Already connected")
+            return
+        self.channel = create_channel(
+            server_address=self.driver_service_address,
+            insecure=(self.root_certificates is None),
+            root_certificates=self.root_certificates,
         )
-        return list(res.task_res_list)
+        self.stub = DriverStub(self.channel)
+        log(DEBUG, "[Driver] Connected to %s", self.driver_service_address)
 
-    def __del__(self) -> None:
-        """Disconnect GrpcDriver if connected."""
-        # Check if GrpcDriver is initialized
-        if self.grpc_driver is None:
+    def disconnect(self) -> None:
+        """Disconnect from the Driver API."""
+        event(EventType.DRIVER_DISCONNECT)
+        if self.channel is None or self.stub is None:
+            log(DEBUG, "Already disconnected")
             return
+        channel = self.channel
+        self.channel = None
+        self.stub = None
+        channel.close()
+        log(DEBUG, "[Driver] Disconnected")
+
+    def create_run(self, req: CreateRunRequest) -> CreateRunResponse:
+        """Request for run ID."""
+        # Check if channel is open
+        if self.stub is None:
+            log(ERROR, ERROR_MESSAGE_DRIVER_NOT_CONNECTED)
+            raise ConnectionError("`GrpcDriver` instance not connected")
+
+        # Call Driver API
+        res: CreateRunResponse = self.stub.CreateRun(request=req)
+        return res
+
+    def get_nodes(self, req: GetNodesRequest) -> GetNodesResponse:
+        """Get client IDs."""
+        # Check if channel is open
+        if self.stub is None:
+            log(ERROR, ERROR_MESSAGE_DRIVER_NOT_CONNECTED)
+            raise ConnectionError("`GrpcDriver` instance not connected")
+
+        # Call gRPC Driver API
+        res: GetNodesResponse = self.stub.GetNodes(request=req)
+        return res
 
-        # Disconnect
-        self.grpc_driver.disconnect()
+    def push_task_ins(self, req: PushTaskInsRequest) -> PushTaskInsResponse:
+        """Schedule tasks."""
+        # Check if channel is open
+        if self.stub is None:
+            log(ERROR, ERROR_MESSAGE_DRIVER_NOT_CONNECTED)
+            raise ConnectionError("`GrpcDriver` instance not connected")
+
+        # Call gRPC Driver API
+        res: PushTaskInsResponse = self.stub.PushTaskIns(request=req)
+        return res
+
+    def pull_task_res(self, req: PullTaskResRequest) -> PullTaskResResponse:
+        """Get task results."""
+        # Check if channel is open
+        if self.stub is None:
+            log(ERROR, ERROR_MESSAGE_DRIVER_NOT_CONNECTED)
+            raise ConnectionError("`GrpcDriver` instance not connected")
+
+        # Call Driver API
+        res: PullTaskResResponse = self.stub.PullTaskRes(request=req)
+        return res
```

### Comparing `flwr-1.7.0/src/py/flwr/driver/driver_client_proxy.py` & `flwr-1.8.0/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,27 +15,21 @@
 """Flower ClientProxy implementation for Driver API."""
 
 
 import time
 from typing import List, Optional
 
 from flwr import common
+from flwr.common import DEFAULT_TTL, MessageType, MessageTypeLegacy, RecordSet
 from flwr.common import recordset_compat as compat
 from flwr.common import serde
-from flwr.common.constant import (
-    TASK_TYPE_EVALUATE,
-    TASK_TYPE_FIT,
-    TASK_TYPE_GET_PARAMETERS,
-    TASK_TYPE_GET_PROPERTIES,
-)
-from flwr.common.recordset import RecordSet
 from flwr.proto import driver_pb2, node_pb2, task_pb2  # pylint: disable=E0611
 from flwr.server.client_proxy import ClientProxy
 
-from .grpc_driver import GrpcDriver
+from ..driver.grpc_driver import GrpcDriver
 
 SLEEP_TIME = 1
 
 
 class DriverClientProxy(ClientProxy):
     """Flower client proxy which delegates work using the Driver API."""
 
@@ -43,92 +37,112 @@
         super().__init__(str(node_id))
         self.node_id = node_id
         self.driver = driver
         self.run_id = run_id
         self.anonymous = anonymous
 
     def get_properties(
-        self, ins: common.GetPropertiesIns, timeout: Optional[float]
+        self,
+        ins: common.GetPropertiesIns,
+        timeout: Optional[float],
+        group_id: Optional[int],
     ) -> common.GetPropertiesRes:
         """Return client's properties."""
         # Ins to RecordSet
         out_recordset = compat.getpropertiesins_to_recordset(ins)
         # Fetch response
         in_recordset = self._send_receive_recordset(
-            out_recordset, TASK_TYPE_GET_PROPERTIES, timeout
+            out_recordset, MessageTypeLegacy.GET_PROPERTIES, timeout, group_id
         )
         # RecordSet to Res
         return compat.recordset_to_getpropertiesres(in_recordset)
 
     def get_parameters(
-        self, ins: common.GetParametersIns, timeout: Optional[float]
+        self,
+        ins: common.GetParametersIns,
+        timeout: Optional[float],
+        group_id: Optional[int],
     ) -> common.GetParametersRes:
         """Return the current local model parameters."""
         # Ins to RecordSet
         out_recordset = compat.getparametersins_to_recordset(ins)
         # Fetch response
         in_recordset = self._send_receive_recordset(
-            out_recordset, TASK_TYPE_GET_PARAMETERS, timeout
+            out_recordset, MessageTypeLegacy.GET_PARAMETERS, timeout, group_id
         )
         # RecordSet to Res
         return compat.recordset_to_getparametersres(in_recordset, False)
 
-    def fit(self, ins: common.FitIns, timeout: Optional[float]) -> common.FitRes:
+    def fit(
+        self, ins: common.FitIns, timeout: Optional[float], group_id: Optional[int]
+    ) -> common.FitRes:
         """Train model parameters on the locally held dataset."""
         # Ins to RecordSet
         out_recordset = compat.fitins_to_recordset(ins, keep_input=True)
         # Fetch response
         in_recordset = self._send_receive_recordset(
-            out_recordset, TASK_TYPE_FIT, timeout
+            out_recordset, MessageType.TRAIN, timeout, group_id
         )
         # RecordSet to Res
         return compat.recordset_to_fitres(in_recordset, keep_input=False)
 
     def evaluate(
-        self, ins: common.EvaluateIns, timeout: Optional[float]
+        self, ins: common.EvaluateIns, timeout: Optional[float], group_id: Optional[int]
     ) -> common.EvaluateRes:
         """Evaluate model parameters on the locally held dataset."""
         # Ins to RecordSet
         out_recordset = compat.evaluateins_to_recordset(ins, keep_input=True)
         # Fetch response
         in_recordset = self._send_receive_recordset(
-            out_recordset, TASK_TYPE_EVALUATE, timeout
+            out_recordset, MessageType.EVALUATE, timeout, group_id
         )
         # RecordSet to Res
         return compat.recordset_to_evaluateres(in_recordset)
 
     def reconnect(
-        self, ins: common.ReconnectIns, timeout: Optional[float]
+        self,
+        ins: common.ReconnectIns,
+        timeout: Optional[float],
+        group_id: Optional[int],
     ) -> common.DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
         return common.DisconnectRes(reason="")  # Nothing to do here (yet)
 
     def _send_receive_recordset(
         self,
         recordset: RecordSet,
         task_type: str,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> RecordSet:
         task_ins = task_pb2.TaskIns(  # pylint: disable=E1101
             task_id="",
-            group_id="",
+            group_id=str(group_id) if group_id is not None else "",
             run_id=self.run_id,
             task=task_pb2.Task(  # pylint: disable=E1101
                 producer=node_pb2.Node(  # pylint: disable=E1101
                     node_id=0,
                     anonymous=True,
                 ),
                 consumer=node_pb2.Node(  # pylint: disable=E1101
                     node_id=self.node_id,
                     anonymous=self.anonymous,
                 ),
                 task_type=task_type,
                 recordset=serde.recordset_to_proto(recordset),
+                ttl=DEFAULT_TTL,
             ),
         )
+
+        # This would normally be recorded upon common.Message creation
+        # but this compatibility stack doesn't create Messages,
+        # so we need to inject `created_at` manually (needed for
+        # taskins validation by server.utils.validator)
+        task_ins.task.created_at = time.time()
+
         push_task_ins_req = driver_pb2.PushTaskInsRequest(  # pylint: disable=E1101
             task_ins_list=[task_ins]
         )
 
         # Send TaskIns to Driver API
         push_task_ins_res = self.driver.push_task_ins(req=push_task_ins_req)
 
@@ -152,12 +166,28 @@
             pull_task_res_res = self.driver.pull_task_res(req=pull_task_res_req)
 
             task_res_list: List[task_pb2.TaskRes] = list(  # pylint: disable=E1101
                 pull_task_res_res.task_res_list
             )
             if len(task_res_list) == 1:
                 task_res = task_res_list[0]
+
+                # This will raise an Exception if task_res carries an `error`
+                validate_task_res(task_res=task_res)
+
                 return serde.recordset_from_proto(task_res.task.recordset)
 
             if timeout is not None and time.time() > start_time + timeout:
                 raise RuntimeError("Timeout reached")
             time.sleep(SLEEP_TIME)
+
+
+def validate_task_res(
+    task_res: task_pb2.TaskRes,  # pylint: disable=E1101
+) -> None:
+    """Validate if a TaskRes is empty or not."""
+    if not task_res.HasField("task"):
+        raise ValueError("Invalid TaskRes, field `task` missing")
+    if task_res.task.HasField("error"):
+        raise ValueError("Exception during client-side task execution")
+    if not task_res.task.HasField("recordset"):
+        raise ValueError("Invalid TaskRes, both `recordset` and `error` are missing")
```

### Comparing `flwr-1.7.0/src/py/flwr/flower/__init__.py` & `flwr-1.8.0/src/py/flwr/cli/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,15 @@
-# Copyright 2020 Adap GmbH. All Rights Reserved.
+# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Flower callable package."""
-
-
-from flwr.client.flower import Flower as Flower
-
-__all__ = [
-    "Flower",
-]
+"""Flower command line interface."""
```

### Comparing `flwr-1.7.0/src/py/flwr/proto/__init__.py` & `flwr-1.8.0/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/driver_pb2.py` & `flwr-1.8.0/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/driver_pb2.pyi` & `flwr-1.8.0/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr-1.8.0/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr-1.8.0/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/fleet_pb2.py` & `flwr-1.8.0/src/py/flwr/proto/fleet_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,39 +12,43 @@
 _sym_db = _symbol_database.Default()
 
 
 from flwr.proto import node_pb2 as flwr_dot_proto_dot_node__pb2
 from flwr.proto import task_pb2 as flwr_dot_proto_dot_task__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66lwr/proto/fleet.proto\x12\nflwr.proto\x1a\x15\x66lwr/proto/node.proto\x1a\x15\x66lwr/proto/task.proto\"\x13\n\x11\x43reateNodeRequest\"4\n\x12\x43reateNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"3\n\x11\x44\x65leteNodeRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"\x14\n\x12\x44\x65leteNodeResponse\"F\n\x12PullTaskInsRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x10\n\x08task_ids\x18\x02 \x03(\t\"k\n\x13PullTaskInsResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12*\n\rtask_ins_list\x18\x02 \x03(\x0b\x32\x13.flwr.proto.TaskIns\"@\n\x12PushTaskResRequest\x12*\n\rtask_res_list\x18\x01 \x03(\x0b\x32\x13.flwr.proto.TaskRes\"\xae\x01\n\x13PushTaskResResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12=\n\x07results\x18\x02 \x03(\x0b\x32,.flwr.proto.PushTaskResResponse.ResultsEntry\x1a.\n\x0cResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"\x1e\n\tReconnect\x12\x11\n\treconnect\x18\x01 \x01(\x04\x32\xc9\x02\n\x05\x46leet\x12M\n\nCreateNode\x12\x1d.flwr.proto.CreateNodeRequest\x1a\x1e.flwr.proto.CreateNodeResponse\"\x00\x12M\n\nDeleteNode\x12\x1d.flwr.proto.DeleteNodeRequest\x1a\x1e.flwr.proto.DeleteNodeResponse\"\x00\x12P\n\x0bPullTaskIns\x12\x1e.flwr.proto.PullTaskInsRequest\x1a\x1f.flwr.proto.PullTaskInsResponse\"\x00\x12P\n\x0bPushTaskRes\x12\x1e.flwr.proto.PushTaskResRequest\x1a\x1f.flwr.proto.PushTaskResResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x66lwr/proto/fleet.proto\x12\nflwr.proto\x1a\x15\x66lwr/proto/node.proto\x1a\x15\x66lwr/proto/task.proto\"*\n\x11\x43reateNodeRequest\x12\x15\n\rping_interval\x18\x01 \x01(\x01\"4\n\x12\x43reateNodeResponse\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"3\n\x11\x44\x65leteNodeRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\"\x14\n\x12\x44\x65leteNodeResponse\"D\n\x0bPingRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x15\n\rping_interval\x18\x02 \x01(\x01\"\x1f\n\x0cPingResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"F\n\x12PullTaskInsRequest\x12\x1e\n\x04node\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x10\n\x08task_ids\x18\x02 \x03(\t\"k\n\x13PullTaskInsResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12*\n\rtask_ins_list\x18\x02 \x03(\x0b\x32\x13.flwr.proto.TaskIns\"@\n\x12PushTaskResRequest\x12*\n\rtask_res_list\x18\x01 \x03(\x0b\x32\x13.flwr.proto.TaskRes\"\xae\x01\n\x13PushTaskResResponse\x12(\n\treconnect\x18\x01 \x01(\x0b\x32\x15.flwr.proto.Reconnect\x12=\n\x07results\x18\x02 \x03(\x0b\x32,.flwr.proto.PushTaskResResponse.ResultsEntry\x1a.\n\x0cResultsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\r:\x02\x38\x01\"\x1e\n\tReconnect\x12\x11\n\treconnect\x18\x01 \x01(\x04\x32\x86\x03\n\x05\x46leet\x12M\n\nCreateNode\x12\x1d.flwr.proto.CreateNodeRequest\x1a\x1e.flwr.proto.CreateNodeResponse\"\x00\x12M\n\nDeleteNode\x12\x1d.flwr.proto.DeleteNodeRequest\x1a\x1e.flwr.proto.DeleteNodeResponse\"\x00\x12;\n\x04Ping\x12\x17.flwr.proto.PingRequest\x1a\x18.flwr.proto.PingResponse\"\x00\x12P\n\x0bPullTaskIns\x12\x1e.flwr.proto.PullTaskInsRequest\x1a\x1f.flwr.proto.PullTaskInsResponse\"\x00\x12P\n\x0bPushTaskRes\x12\x1e.flwr.proto.PushTaskResRequest\x1a\x1f.flwr.proto.PushTaskResResponse\"\x00\x62\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flwr.proto.fleet_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._options = None
   _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_options = b'8\001'
   _globals['_CREATENODEREQUEST']._serialized_start=84
-  _globals['_CREATENODEREQUEST']._serialized_end=103
-  _globals['_CREATENODERESPONSE']._serialized_start=105
-  _globals['_CREATENODERESPONSE']._serialized_end=157
-  _globals['_DELETENODEREQUEST']._serialized_start=159
-  _globals['_DELETENODEREQUEST']._serialized_end=210
-  _globals['_DELETENODERESPONSE']._serialized_start=212
-  _globals['_DELETENODERESPONSE']._serialized_end=232
-  _globals['_PULLTASKINSREQUEST']._serialized_start=234
-  _globals['_PULLTASKINSREQUEST']._serialized_end=304
-  _globals['_PULLTASKINSRESPONSE']._serialized_start=306
-  _globals['_PULLTASKINSRESPONSE']._serialized_end=413
-  _globals['_PUSHTASKRESREQUEST']._serialized_start=415
-  _globals['_PUSHTASKRESREQUEST']._serialized_end=479
-  _globals['_PUSHTASKRESRESPONSE']._serialized_start=482
-  _globals['_PUSHTASKRESRESPONSE']._serialized_end=656
-  _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_start=610
-  _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_end=656
-  _globals['_RECONNECT']._serialized_start=658
-  _globals['_RECONNECT']._serialized_end=688
-  _globals['_FLEET']._serialized_start=691
-  _globals['_FLEET']._serialized_end=1020
+  _globals['_CREATENODEREQUEST']._serialized_end=126
+  _globals['_CREATENODERESPONSE']._serialized_start=128
+  _globals['_CREATENODERESPONSE']._serialized_end=180
+  _globals['_DELETENODEREQUEST']._serialized_start=182
+  _globals['_DELETENODEREQUEST']._serialized_end=233
+  _globals['_DELETENODERESPONSE']._serialized_start=235
+  _globals['_DELETENODERESPONSE']._serialized_end=255
+  _globals['_PINGREQUEST']._serialized_start=257
+  _globals['_PINGREQUEST']._serialized_end=325
+  _globals['_PINGRESPONSE']._serialized_start=327
+  _globals['_PINGRESPONSE']._serialized_end=358
+  _globals['_PULLTASKINSREQUEST']._serialized_start=360
+  _globals['_PULLTASKINSREQUEST']._serialized_end=430
+  _globals['_PULLTASKINSRESPONSE']._serialized_start=432
+  _globals['_PULLTASKINSRESPONSE']._serialized_end=539
+  _globals['_PUSHTASKRESREQUEST']._serialized_start=541
+  _globals['_PUSHTASKRESREQUEST']._serialized_end=605
+  _globals['_PUSHTASKRESRESPONSE']._serialized_start=608
+  _globals['_PUSHTASKRESRESPONSE']._serialized_end=782
+  _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_start=736
+  _globals['_PUSHTASKRESRESPONSE_RESULTSENTRY']._serialized_end=782
+  _globals['_RECONNECT']._serialized_start=784
+  _globals['_RECONNECT']._serialized_end=814
+  _globals['_FLEET']._serialized_start=817
+  _globals['_FLEET']._serialized_end=1207
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flwr-1.7.0/src/py/flwr/proto/fleet_pb2.pyi` & `flwr-1.8.0/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -12,16 +12,21 @@
 import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 class CreateNodeRequest(google.protobuf.message.Message):
     """CreateNode messages"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    PING_INTERVAL_FIELD_NUMBER: builtins.int
+    ping_interval: builtins.float
     def __init__(self,
+        *,
+        ping_interval: builtins.float = ...,
         ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["ping_interval",b"ping_interval"]) -> None: ...
 global___CreateNodeRequest = CreateNodeRequest
 
 class CreateNodeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     NODE_FIELD_NUMBER: builtins.int
     @property
     def node(self) -> flwr.proto.node_pb2.Node: ...
@@ -49,14 +54,42 @@
 
 class DeleteNodeResponse(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     def __init__(self,
         ) -> None: ...
 global___DeleteNodeResponse = DeleteNodeResponse
 
+class PingRequest(google.protobuf.message.Message):
+    """Ping messages"""
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    NODE_FIELD_NUMBER: builtins.int
+    PING_INTERVAL_FIELD_NUMBER: builtins.int
+    @property
+    def node(self) -> flwr.proto.node_pb2.Node: ...
+    ping_interval: builtins.float
+    def __init__(self,
+        *,
+        node: typing.Optional[flwr.proto.node_pb2.Node] = ...,
+        ping_interval: builtins.float = ...,
+        ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["node",b"node"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["node",b"node","ping_interval",b"ping_interval"]) -> None: ...
+global___PingRequest = PingRequest
+
+class PingResponse(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    SUCCESS_FIELD_NUMBER: builtins.int
+    success: builtins.bool
+    def __init__(self,
+        *,
+        success: builtins.bool = ...,
+        ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["success",b"success"]) -> None: ...
+global___PingResponse = PingResponse
+
 class PullTaskInsRequest(google.protobuf.message.Message):
     """PullTaskIns messages"""
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     NODE_FIELD_NUMBER: builtins.int
     TASK_IDS_FIELD_NUMBER: builtins.int
     @property
     def node(self) -> flwr.proto.node_pb2.Node: ...
```

### Comparing `flwr-1.7.0/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr-1.8.0/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,14 +20,19 @@
                 response_deserializer=flwr_dot_proto_dot_fleet__pb2.CreateNodeResponse.FromString,
                 )
         self.DeleteNode = channel.unary_unary(
                 '/flwr.proto.Fleet/DeleteNode',
                 request_serializer=flwr_dot_proto_dot_fleet__pb2.DeleteNodeRequest.SerializeToString,
                 response_deserializer=flwr_dot_proto_dot_fleet__pb2.DeleteNodeResponse.FromString,
                 )
+        self.Ping = channel.unary_unary(
+                '/flwr.proto.Fleet/Ping',
+                request_serializer=flwr_dot_proto_dot_fleet__pb2.PingRequest.SerializeToString,
+                response_deserializer=flwr_dot_proto_dot_fleet__pb2.PingResponse.FromString,
+                )
         self.PullTaskIns = channel.unary_unary(
                 '/flwr.proto.Fleet/PullTaskIns',
                 request_serializer=flwr_dot_proto_dot_fleet__pb2.PullTaskInsRequest.SerializeToString,
                 response_deserializer=flwr_dot_proto_dot_fleet__pb2.PullTaskInsResponse.FromString,
                 )
         self.PushTaskRes = channel.unary_unary(
                 '/flwr.proto.Fleet/PushTaskRes',
@@ -47,14 +52,20 @@
 
     def DeleteNode(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def Ping(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def PullTaskIns(self, request, context):
         """Retrieve one or more tasks, if possible
 
         HTTP API path: /api/v1/fleet/pull-task-ins
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
@@ -78,14 +89,19 @@
                     response_serializer=flwr_dot_proto_dot_fleet__pb2.CreateNodeResponse.SerializeToString,
             ),
             'DeleteNode': grpc.unary_unary_rpc_method_handler(
                     servicer.DeleteNode,
                     request_deserializer=flwr_dot_proto_dot_fleet__pb2.DeleteNodeRequest.FromString,
                     response_serializer=flwr_dot_proto_dot_fleet__pb2.DeleteNodeResponse.SerializeToString,
             ),
+            'Ping': grpc.unary_unary_rpc_method_handler(
+                    servicer.Ping,
+                    request_deserializer=flwr_dot_proto_dot_fleet__pb2.PingRequest.FromString,
+                    response_serializer=flwr_dot_proto_dot_fleet__pb2.PingResponse.SerializeToString,
+            ),
             'PullTaskIns': grpc.unary_unary_rpc_method_handler(
                     servicer.PullTaskIns,
                     request_deserializer=flwr_dot_proto_dot_fleet__pb2.PullTaskInsRequest.FromString,
                     response_serializer=flwr_dot_proto_dot_fleet__pb2.PullTaskInsResponse.SerializeToString,
             ),
             'PushTaskRes': grpc.unary_unary_rpc_method_handler(
                     servicer.PushTaskRes,
@@ -133,14 +149,31 @@
         return grpc.experimental.unary_unary(request, target, '/flwr.proto.Fleet/DeleteNode',
             flwr_dot_proto_dot_fleet__pb2.DeleteNodeRequest.SerializeToString,
             flwr_dot_proto_dot_fleet__pb2.DeleteNodeResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def Ping(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/flwr.proto.Fleet/Ping',
+            flwr_dot_proto_dot_fleet__pb2.PingRequest.SerializeToString,
+            flwr_dot_proto_dot_fleet__pb2.PingResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def PullTaskIns(request,
             target,
             options=(),
             channel_credentials=None,
             call_credentials=None,
             insecure=False,
             compression=None,
```

### Comparing `flwr-1.7.0/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr-1.8.0/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,18 @@
         flwr.proto.fleet_pb2.CreateNodeRequest,
         flwr.proto.fleet_pb2.CreateNodeResponse]
 
     DeleteNode: grpc.UnaryUnaryMultiCallable[
         flwr.proto.fleet_pb2.DeleteNodeRequest,
         flwr.proto.fleet_pb2.DeleteNodeResponse]
 
+    Ping: grpc.UnaryUnaryMultiCallable[
+        flwr.proto.fleet_pb2.PingRequest,
+        flwr.proto.fleet_pb2.PingResponse]
+
     PullTaskIns: grpc.UnaryUnaryMultiCallable[
         flwr.proto.fleet_pb2.PullTaskInsRequest,
         flwr.proto.fleet_pb2.PullTaskInsResponse]
     """Retrieve one or more tasks, if possible
 
     HTTP API path: /api/v1/fleet/pull-task-ins
     """
@@ -43,14 +47,20 @@
     @abc.abstractmethod
     def DeleteNode(self,
         request: flwr.proto.fleet_pb2.DeleteNodeRequest,
         context: grpc.ServicerContext,
     ) -> flwr.proto.fleet_pb2.DeleteNodeResponse: ...
 
     @abc.abstractmethod
+    def Ping(self,
+        request: flwr.proto.fleet_pb2.PingRequest,
+        context: grpc.ServicerContext,
+    ) -> flwr.proto.fleet_pb2.PingResponse: ...
+
+    @abc.abstractmethod
     def PullTaskIns(self,
         request: flwr.proto.fleet_pb2.PullTaskInsRequest,
         context: grpc.ServicerContext,
     ) -> flwr.proto.fleet_pb2.PullTaskInsResponse:
         """Retrieve one or more tasks, if possible
 
         HTTP API path: /api/v1/fleet/pull-task-ins
```

### Comparing `flwr-1.7.0/src/py/flwr/proto/node_pb2.py` & `flwr-1.8.0/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/node_pb2.pyi` & `flwr-1.8.0/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/recordset_pb2.py` & `flwr-1.8.0/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/recordset_pb2.pyi` & `flwr-1.8.0/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/task_pb2.py` & `flwr-1.8.0/src/py/flwr/proto/task_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,23 +11,24 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from flwr.proto import node_pb2 as flwr_dot_proto_dot_node__pb2
 from flwr.proto import recordset_pb2 as flwr_dot_proto_dot_recordset__pb2
 from flwr.proto import transport_pb2 as flwr_dot_proto_dot_transport__pb2
+from flwr.proto import error_pb2 as flwr_dot_proto_dot_error__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x66lwr/proto/task.proto\x12\nflwr.proto\x1a\x15\x66lwr/proto/node.proto\x1a\x1a\x66lwr/proto/recordset.proto\x1a\x1a\x66lwr/proto/transport.proto\"\xd4\x01\n\x04Task\x12\"\n\x08producer\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\"\n\x08\x63onsumer\x18\x02 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x12\n\ncreated_at\x18\x03 \x01(\t\x12\x14\n\x0c\x64\x65livered_at\x18\x04 \x01(\t\x12\x0b\n\x03ttl\x18\x05 \x01(\t\x12\x10\n\x08\x61ncestry\x18\x06 \x03(\t\x12\x11\n\ttask_type\x18\x07 \x01(\t\x12(\n\trecordset\x18\x08 \x01(\x0b\x32\x15.flwr.proto.RecordSet\"\\\n\x07TaskIns\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x10\n\x08group_id\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\x12\x12\x1e\n\x04task\x18\x04 \x01(\x0b\x32\x10.flwr.proto.Task\"\\\n\x07TaskRes\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x10\n\x08group_id\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\x12\x12\x1e\n\x04task\x18\x04 \x01(\x0b\x32\x10.flwr.proto.Taskb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15\x66lwr/proto/task.proto\x12\nflwr.proto\x1a\x15\x66lwr/proto/node.proto\x1a\x1a\x66lwr/proto/recordset.proto\x1a\x1a\x66lwr/proto/transport.proto\x1a\x16\x66lwr/proto/error.proto\"\x89\x02\n\x04Task\x12\"\n\x08producer\x18\x01 \x01(\x0b\x32\x10.flwr.proto.Node\x12\"\n\x08\x63onsumer\x18\x02 \x01(\x0b\x32\x10.flwr.proto.Node\x12\x12\n\ncreated_at\x18\x03 \x01(\x01\x12\x14\n\x0c\x64\x65livered_at\x18\x04 \x01(\t\x12\x11\n\tpushed_at\x18\x05 \x01(\x01\x12\x0b\n\x03ttl\x18\x06 \x01(\x01\x12\x10\n\x08\x61ncestry\x18\x07 \x03(\t\x12\x11\n\ttask_type\x18\x08 \x01(\t\x12(\n\trecordset\x18\t \x01(\x0b\x32\x15.flwr.proto.RecordSet\x12 \n\x05\x65rror\x18\n \x01(\x0b\x32\x11.flwr.proto.Error\"\\\n\x07TaskIns\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x10\n\x08group_id\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\x12\x12\x1e\n\x04task\x18\x04 \x01(\x0b\x32\x10.flwr.proto.Task\"\\\n\x07TaskRes\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x10\n\x08group_id\x18\x02 \x01(\t\x12\x0e\n\x06run_id\x18\x03 \x01(\x12\x12\x1e\n\x04task\x18\x04 \x01(\x0b\x32\x10.flwr.proto.Taskb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'flwr.proto.task_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
-  _globals['_TASK']._serialized_start=117
-  _globals['_TASK']._serialized_end=329
-  _globals['_TASKINS']._serialized_start=331
-  _globals['_TASKINS']._serialized_end=423
-  _globals['_TASKRES']._serialized_start=425
-  _globals['_TASKRES']._serialized_end=517
+  _globals['_TASK']._serialized_start=141
+  _globals['_TASK']._serialized_end=406
+  _globals['_TASKINS']._serialized_start=408
+  _globals['_TASKINS']._serialized_end=500
+  _globals['_TASKRES']._serialized_start=502
+  _globals['_TASKRES']._serialized_end=594
 # @@protoc_insertion_point(module_scope)
```

### Comparing `flwr-1.7.0/src/py/flwr/proto/task_pb2.pyi` & `flwr-1.8.0/src/py/flwr/proto/task_pb2.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 @generated by mypy-protobuf.  Do not edit manually!
 isort:skip_file
 """
 import builtins
+import flwr.proto.error_pb2
 import flwr.proto.node_pb2
 import flwr.proto.recordset_pb2
 import google.protobuf.descriptor
 import google.protobuf.internal.containers
 import google.protobuf.message
 import typing
 import typing_extensions
@@ -15,43 +16,50 @@
 
 class Task(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     PRODUCER_FIELD_NUMBER: builtins.int
     CONSUMER_FIELD_NUMBER: builtins.int
     CREATED_AT_FIELD_NUMBER: builtins.int
     DELIVERED_AT_FIELD_NUMBER: builtins.int
+    PUSHED_AT_FIELD_NUMBER: builtins.int
     TTL_FIELD_NUMBER: builtins.int
     ANCESTRY_FIELD_NUMBER: builtins.int
     TASK_TYPE_FIELD_NUMBER: builtins.int
     RECORDSET_FIELD_NUMBER: builtins.int
+    ERROR_FIELD_NUMBER: builtins.int
     @property
     def producer(self) -> flwr.proto.node_pb2.Node: ...
     @property
     def consumer(self) -> flwr.proto.node_pb2.Node: ...
-    created_at: typing.Text
+    created_at: builtins.float
     delivered_at: typing.Text
-    ttl: typing.Text
+    pushed_at: builtins.float
+    ttl: builtins.float
     @property
     def ancestry(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[typing.Text]: ...
     task_type: typing.Text
     @property
     def recordset(self) -> flwr.proto.recordset_pb2.RecordSet: ...
+    @property
+    def error(self) -> flwr.proto.error_pb2.Error: ...
     def __init__(self,
         *,
         producer: typing.Optional[flwr.proto.node_pb2.Node] = ...,
         consumer: typing.Optional[flwr.proto.node_pb2.Node] = ...,
-        created_at: typing.Text = ...,
+        created_at: builtins.float = ...,
         delivered_at: typing.Text = ...,
-        ttl: typing.Text = ...,
+        pushed_at: builtins.float = ...,
+        ttl: builtins.float = ...,
         ancestry: typing.Optional[typing.Iterable[typing.Text]] = ...,
         task_type: typing.Text = ...,
         recordset: typing.Optional[flwr.proto.recordset_pb2.RecordSet] = ...,
+        error: typing.Optional[flwr.proto.error_pb2.Error] = ...,
         ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["consumer",b"consumer","producer",b"producer","recordset",b"recordset"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ancestry",b"ancestry","consumer",b"consumer","created_at",b"created_at","delivered_at",b"delivered_at","producer",b"producer","recordset",b"recordset","task_type",b"task_type","ttl",b"ttl"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["consumer",b"consumer","error",b"error","producer",b"producer","recordset",b"recordset"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["ancestry",b"ancestry","consumer",b"consumer","created_at",b"created_at","delivered_at",b"delivered_at","error",b"error","producer",b"producer","pushed_at",b"pushed_at","recordset",b"recordset","task_type",b"task_type","ttl",b"ttl"]) -> None: ...
 global___Task = Task
 
 class TaskIns(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
     TASK_ID_FIELD_NUMBER: builtins.int
     GROUP_ID_FIELD_NUMBER: builtins.int
     RUN_ID_FIELD_NUMBER: builtins.int
```

### Comparing `flwr-1.7.0/src/py/flwr/proto/transport_pb2.py` & `flwr-1.8.0/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/transport_pb2.pyi` & `flwr-1.8.0/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr-1.8.0/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr-1.8.0/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/__init__.py` & `flwr-1.8.0/src/py/flwr/server/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,29 +12,41 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower server."""
 
 
 from . import strategy
-from .app import ServerConfig as ServerConfig
+from . import workflow as workflow
 from .app import run_driver_api as run_driver_api
 from .app import run_fleet_api as run_fleet_api
-from .app import run_server as run_server
+from .app import run_superlink as run_superlink
 from .app import start_server as start_server
 from .client_manager import ClientManager as ClientManager
 from .client_manager import SimpleClientManager as SimpleClientManager
+from .compat import LegacyContext as LegacyContext
+from .compat import start_driver as start_driver
+from .driver import Driver as Driver
 from .history import History as History
+from .run_serverapp import run_server_app as run_server_app
 from .server import Server as Server
+from .server_app import ServerApp as ServerApp
+from .server_config import ServerConfig as ServerConfig
 
 __all__ = [
     "ClientManager",
+    "Driver",
     "History",
+    "LegacyContext",
     "run_driver_api",
     "run_fleet_api",
-    "run_server",
+    "run_server_app",
+    "run_superlink",
     "Server",
+    "ServerApp",
     "ServerConfig",
     "SimpleClientManager",
+    "start_driver",
     "start_server",
     "strategy",
+    "workflow",
 ]
```

### Comparing `flwr-1.7.0/src/py/flwr/server/app.py` & `flwr-1.8.0/src/py/flwr/server/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,75 +10,62 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower server app."""
 
-
 import argparse
+import asyncio
 import importlib.util
 import sys
 import threading
-from dataclasses import dataclass
 from logging import ERROR, INFO, WARN
 from os.path import isfile
 from pathlib import Path
-from signal import SIGINT, SIGTERM, signal
-from types import FrameType
 from typing import List, Optional, Tuple
 
 import grpc
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH, EventType, event
 from flwr.common.address import parse_address
 from flwr.common.constant import (
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
+    TRANSPORT_TYPE_VCE,
 )
+from flwr.common.exit_handlers import register_exit_handlers
 from flwr.common.logger import log
-from flwr.proto.driver_pb2_grpc import (  # pylint: disable=E0611
-    add_DriverServicer_to_server,
-)
 from flwr.proto.fleet_pb2_grpc import (  # pylint: disable=E0611
     add_FleetServicer_to_server,
 )
-from flwr.server.client_manager import ClientManager, SimpleClientManager
-from flwr.server.driver.driver_servicer import DriverServicer
-from flwr.server.fleet.grpc_bidi.grpc_server import (
+
+from .client_manager import ClientManager
+from .history import History
+from .server import Server, init_defaults, run_fl
+from .server_config import ServerConfig
+from .strategy import Strategy
+from .superlink.driver.driver_grpc import run_driver_api_grpc
+from .superlink.fleet.grpc_bidi.grpc_server import (
     generic_create_grpc_server,
     start_grpc_server,
 )
-from flwr.server.fleet.grpc_rere.fleet_servicer import FleetServicer
-from flwr.server.history import History
-from flwr.server.server import Server
-from flwr.server.state import StateFactory
-from flwr.server.strategy import FedAvg, Strategy
+from .superlink.fleet.grpc_rere.fleet_servicer import FleetServicer
+from .superlink.fleet.vce import start_vce
+from .superlink.state import StateFactory
 
 ADDRESS_DRIVER_API = "0.0.0.0:9091"
 ADDRESS_FLEET_API_GRPC_RERE = "0.0.0.0:9092"
 ADDRESS_FLEET_API_GRPC_BIDI = "[::]:8080"  # IPv6 to keep start_server compatible
 ADDRESS_FLEET_API_REST = "0.0.0.0:9093"
 
 DATABASE = ":flwr-in-memory-state:"
 
 
-@dataclass
-class ServerConfig:
-    """Flower server config.
-
-    All attributes have default values which allows users to configure just the ones
-    they care about.
-    """
-
-    num_rounds: int = 1
-    round_timeout: Optional[float] = None
-
-
 def start_server(  # pylint: disable=too-many-arguments,too-many-locals
     *,
     server_address: str = ADDRESS_FLEET_API_GRPC_BIDI,
     server: Optional[Server] = None,
     config: Optional[ServerConfig] = None,
     strategy: Optional[Strategy] = None,
     client_manager: Optional[ClientManager] = None,
@@ -190,60 +177,19 @@
     grpc_server.stop(grace=1)
 
     event(EventType.START_SERVER_LEAVE)
 
     return hist
 
 
-def init_defaults(
-    server: Optional[Server],
-    config: Optional[ServerConfig],
-    strategy: Optional[Strategy],
-    client_manager: Optional[ClientManager],
-) -> Tuple[Server, ServerConfig]:
-    """Create server instance if none was given."""
-    if server is None:
-        if client_manager is None:
-            client_manager = SimpleClientManager()
-        if strategy is None:
-            strategy = FedAvg()
-        server = Server(client_manager=client_manager, strategy=strategy)
-    elif strategy is not None:
-        log(WARN, "Both server and strategy were provided, ignoring strategy")
-
-    # Set default config values
-    if config is None:
-        config = ServerConfig()
-
-    return server, config
-
-
-def run_fl(
-    server: Server,
-    config: ServerConfig,
-) -> History:
-    """Train a model on the given server and return the History object."""
-    hist = server.fit(num_rounds=config.num_rounds, timeout=config.round_timeout)
-    log(INFO, "app_fit: losses_distributed %s", str(hist.losses_distributed))
-    log(INFO, "app_fit: metrics_distributed_fit %s", str(hist.metrics_distributed_fit))
-    log(INFO, "app_fit: metrics_distributed %s", str(hist.metrics_distributed))
-    log(INFO, "app_fit: losses_centralized %s", str(hist.losses_centralized))
-    log(INFO, "app_fit: metrics_centralized %s", str(hist.metrics_centralized))
-
-    # Graceful shutdown
-    server.disconnect_all_clients(timeout=config.round_timeout)
-
-    return hist
-
-
 def run_driver_api() -> None:
     """Run Flower server (Driver API)."""
     log(INFO, "Starting Flower server (Driver API)")
     event(EventType.RUN_DRIVER_API_ENTER)
-    args = _parse_args_driver().parse_args()
+    args = _parse_args_run_driver_api().parse_args()
 
     # Parse IP address
     parsed_address = parse_address(args.driver_api_address)
     if not parsed_address:
         sys.exit(f"Driver IP address ({args.driver_api_address}) cannot be parsed.")
     host, port, is_v6 = parsed_address
     address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
@@ -251,36 +197,36 @@
     # Obtain certificates
     certificates = _try_obtain_certificates(args)
 
     # Initialize StateFactory
     state_factory = StateFactory(args.database)
 
     # Start server
-    grpc_server: grpc.Server = _run_driver_api_grpc(
+    grpc_server: grpc.Server = run_driver_api_grpc(
         address=address,
         state_factory=state_factory,
         certificates=certificates,
     )
 
     # Graceful shutdown
-    _register_exit_handlers(
+    register_exit_handlers(
+        event_type=EventType.RUN_DRIVER_API_LEAVE,
         grpc_servers=[grpc_server],
         bckg_threads=[],
-        event_type=EventType.RUN_DRIVER_API_LEAVE,
     )
 
     # Block
     grpc_server.wait_for_termination()
 
 
 def run_fleet_api() -> None:
     """Run Flower server (Fleet API)."""
     log(INFO, "Starting Flower server (Fleet API)")
     event(EventType.RUN_FLEET_API_ENTER)
-    args = _parse_args_fleet().parse_args()
+    args = _parse_args_run_fleet_api().parse_args()
 
     # Obtain certificates
     certificates = _try_obtain_certificates(args)
 
     # Initialize StateFactory
     state_factory = StateFactory(args.database)
 
@@ -326,33 +272,33 @@
             certificates=certificates,
         )
         grpc_servers.append(fleet_server)
     else:
         raise ValueError(f"Unknown fleet_api_type: {args.fleet_api_type}")
 
     # Graceful shutdown
-    _register_exit_handlers(
+    register_exit_handlers(
+        event_type=EventType.RUN_FLEET_API_LEAVE,
         grpc_servers=grpc_servers,
         bckg_threads=bckg_threads,
-        event_type=EventType.RUN_FLEET_API_LEAVE,
     )
 
     # Block
     if len(grpc_servers) > 0:
         grpc_servers[0].wait_for_termination()
     elif len(bckg_threads) > 0:
         bckg_threads[0].join()
 
 
 # pylint: disable=too-many-branches, too-many-locals, too-many-statements
-def run_server() -> None:
+def run_superlink() -> None:
     """Run Flower server (Driver API and Fleet API)."""
     log(INFO, "Starting Flower server")
-    event(EventType.RUN_SERVER_ENTER)
-    args = _parse_args_server().parse_args()
+    event(EventType.RUN_SUPERLINK_ENTER)
+    args = _parse_args_run_superlink().parse_args()
 
     # Parse IP address
     parsed_address = parse_address(args.driver_api_address)
     if not parsed_address:
         sys.exit(f"Driver IP address ({args.driver_api_address}) cannot be parsed.")
     host, port, is_v6 = parsed_address
     address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
@@ -360,15 +306,15 @@
     # Obtain certificates
     certificates = _try_obtain_certificates(args)
 
     # Initialize StateFactory
     state_factory = StateFactory(args.database)
 
     # Start Driver API
-    driver_server: grpc.Server = _run_driver_api_grpc(
+    driver_server: grpc.Server = run_driver_api_grpc(
         address=address,
         state_factory=state_factory,
         certificates=certificates,
     )
 
     grpc_servers = [driver_server]
     bckg_threads = []
@@ -408,22 +354,33 @@
         address = f"[{host}]:{port}" if is_v6 else f"{host}:{port}"
         fleet_server = _run_fleet_api_grpc_rere(
             address=address,
             state_factory=state_factory,
             certificates=certificates,
         )
         grpc_servers.append(fleet_server)
+    elif args.fleet_api_type == TRANSPORT_TYPE_VCE:
+        f_stop = asyncio.Event()  # Does nothing
+        _run_fleet_api_vce(
+            num_supernodes=args.num_supernodes,
+            client_app_attr=args.client_app,
+            backend_name=args.backend,
+            backend_config_json_stream=args.backend_config,
+            app_dir=args.app_dir,
+            state_factory=state_factory,
+            f_stop=f_stop,
+        )
     else:
         raise ValueError(f"Unknown fleet_api_type: {args.fleet_api_type}")
 
     # Graceful shutdown
-    _register_exit_handlers(
+    register_exit_handlers(
+        event_type=EventType.RUN_SUPERLINK_LEAVE,
         grpc_servers=grpc_servers,
         bckg_threads=bckg_threads,
-        event_type=EventType.RUN_SERVER_LEAVE,
     )
 
     # Block
     while True:
         if bckg_threads:
             for thread in bckg_threads:
                 if not thread.is_alive():
@@ -450,84 +407,14 @@
             "Certificates are required unless running in insecure mode. "
             "Please provide certificate paths with '--certificates' or run the server "
             "in insecure mode using '--insecure' if you understand the risks."
         )
     return certificates
 
 
-def _register_exit_handlers(
-    grpc_servers: List[grpc.Server],
-    bckg_threads: List[threading.Thread],
-    event_type: EventType,
-) -> None:
-    default_handlers = {
-        SIGINT: None,
-        SIGTERM: None,
-    }
-
-    def graceful_exit_handler(  # type: ignore
-        signalnum,
-        frame: FrameType,  # pylint: disable=unused-argument
-    ) -> None:
-        """Exit handler to be registered with signal.signal.
-
-        When called will reset signal handler to original signal handler from
-        default_handlers.
-        """
-        # Reset to default handler
-        signal(signalnum, default_handlers[signalnum])
-
-        event_res = event(event_type=event_type)
-
-        for grpc_server in grpc_servers:
-            grpc_server.stop(grace=1)
-
-        for bckg_thread in bckg_threads:
-            bckg_thread.join()
-
-        # Ensure event has happend
-        event_res.result()
-
-        # Setup things for graceful exit
-        sys.exit(0)
-
-    default_handlers[SIGINT] = signal(  # type: ignore
-        SIGINT,
-        graceful_exit_handler,  # type: ignore
-    )
-    default_handlers[SIGTERM] = signal(  # type: ignore
-        SIGTERM,
-        graceful_exit_handler,  # type: ignore
-    )
-
-
-def _run_driver_api_grpc(
-    address: str,
-    state_factory: StateFactory,
-    certificates: Optional[Tuple[bytes, bytes, bytes]],
-) -> grpc.Server:
-    """Run Driver API (gRPC, request-response)."""
-    # Create Driver API gRPC server
-    driver_servicer: grpc.Server = DriverServicer(
-        state_factory=state_factory,
-    )
-    driver_add_servicer_to_server_fn = add_DriverServicer_to_server
-    driver_grpc_server = generic_create_grpc_server(
-        servicer_and_add_fn=(driver_servicer, driver_add_servicer_to_server_fn),
-        server_address=address,
-        max_message_length=GRPC_MAX_MESSAGE_LENGTH,
-        certificates=certificates,
-    )
-
-    log(INFO, "Flower ECE: Starting Driver API (gRPC-rere) on %s", address)
-    driver_grpc_server.start()
-
-    return driver_grpc_server
-
-
 def _run_fleet_api_grpc_rere(
     address: str,
     state_factory: StateFactory,
     certificates: Optional[Tuple[bytes, bytes, bytes]],
 ) -> grpc.Server:
     """Run Fleet API (gRPC, request-response)."""
     # Create Fleet API gRPC server
@@ -544,28 +431,51 @@
 
     log(INFO, "Flower ECE: Starting Fleet API (gRPC-rere) on %s", address)
     fleet_grpc_server.start()
 
     return fleet_grpc_server
 
 
+# pylint: disable=too-many-arguments
+def _run_fleet_api_vce(
+    num_supernodes: int,
+    client_app_attr: str,
+    backend_name: str,
+    backend_config_json_stream: str,
+    app_dir: str,
+    state_factory: StateFactory,
+    f_stop: asyncio.Event,
+) -> None:
+    log(INFO, "Flower VCE: Starting Fleet API (VirtualClientEngine)")
+
+    start_vce(
+        num_supernodes=num_supernodes,
+        client_app_attr=client_app_attr,
+        backend_name=backend_name,
+        backend_config_json_stream=backend_config_json_stream,
+        state_factory=state_factory,
+        app_dir=app_dir,
+        f_stop=f_stop,
+    )
+
+
 # pylint: disable=import-outside-toplevel,too-many-arguments
 def _run_fleet_api_rest(
     host: str,
     port: int,
     ssl_keyfile: Optional[str],
     ssl_certfile: Optional[str],
     state_factory: StateFactory,
     workers: int,
 ) -> None:
     """Run Driver API (REST-based)."""
     try:
         import uvicorn
 
-        from flwr.server.fleet.rest_rere.rest_api import app as fast_api_app
+        from flwr.server.superlink.fleet.rest_rere.rest_api import app as fast_api_app
     except ModuleNotFoundError:
         sys.exit(MISSING_EXTRA_REST)
     if workers != 1:
         raise ValueError(
             f"The supported number of workers for the Fleet API (REST server) is "
             f"1. Instead given {workers}. The functionality of >1 workers will be "
             f"added in the future releases."
@@ -580,15 +490,15 @@
     )
     if any(validation_exceptions):
         # Starting with 3.11 we can use ExceptionGroup but for now
         # this seems to be the reasonable approach.
         raise ValueError(validation_exceptions)
 
     uvicorn.run(
-        app="flwr.server.fleet.rest_rere.rest_api:app",
+        app="flwr.server.superlink.fleet.rest_rere.rest_api:app",
         port=port,
         host=host,
         reload=False,
         access_log=True,
         ssl_keyfile=ssl_keyfile,
         ssl_certfile=ssl_certfile,
         workers=workers,
@@ -617,15 +527,15 @@
         )
         log(ERROR, msg)
         validation_exceptions.append(ValueError(msg))
 
     return validation_exceptions
 
 
-def _parse_args_driver() -> argparse.ArgumentParser:
+def _parse_args_run_driver_api() -> argparse.ArgumentParser:
     """Parse command line arguments for Driver API."""
     parser = argparse.ArgumentParser(
         description="Start a Flower Driver API server. "
         "This server will be responsible for "
         "receiving TaskIns from the Driver script and "
         "sending them to the Fleet API. Once the client nodes "
         "are done, they will send the TaskRes back to this Driver API server (through"
@@ -634,15 +544,15 @@
 
     _add_args_common(parser=parser)
     _add_args_driver_api(parser=parser)
 
     return parser
 
 
-def _parse_args_fleet() -> argparse.ArgumentParser:
+def _parse_args_run_fleet_api() -> argparse.ArgumentParser:
     """Parse command line arguments for Fleet API."""
     parser = argparse.ArgumentParser(
         description="Start a Flower Fleet API server."
         "This server will be responsible for "
         "sending TaskIns (received from the Driver API) to the client nodes "
         "and of receiving TaskRes sent back from those same client nodes once "
         "they are done. Then, this Fleet API server can send those "
@@ -651,15 +561,15 @@
 
     _add_args_common(parser=parser)
     _add_args_fleet_api(parser=parser)
 
     return parser
 
 
-def _parse_args_server() -> argparse.ArgumentParser:
+def _parse_args_run_superlink() -> argparse.ArgumentParser:
     """Parse command line arguments for both Driver API and Fleet API."""
     parser = argparse.ArgumentParser(
         description="This will start a Flower server "
         "(meaning, a Driver API and a Fleet API), "
         "that clients will be able to connect to.",
     )
 
@@ -721,14 +631,22 @@
         "--rest",
         action="store_const",
         dest="fleet_api_type",
         const=TRANSPORT_TYPE_REST,
         help="Start a Fleet API server (REST, experimental)",
     )
 
+    ex_group.add_argument(
+        "--vce",
+        action="store_const",
+        dest="fleet_api_type",
+        const=TRANSPORT_TYPE_VCE,
+        help="Start a Fleet API server (VirtualClientEngine)",
+    )
+
     # Fleet API gRPC-rere options
     grpc_rere_group = parser.add_argument_group(
         "Fleet API (gRPC-rere) server options", ""
     )
     grpc_rere_group.add_argument(
         "--grpc-rere-fleet-api-address",
         help="Fleet API (gRPC-rere) server address (IPv4, IPv6, or a domain name)",
@@ -756,7 +674,40 @@
     )
     rest_group.add_argument(
         "--rest-fleet-api-workers",
         help="Set the number of concurrent workers for the Fleet API REST server.",
         type=int,
         default=1,
     )
+
+    # Fleet API VCE options
+    vce_group = parser.add_argument_group("Fleet API (VCE) server options", "")
+    vce_group.add_argument(
+        "--client-app",
+        help="For example: `client:app` or `project.package.module:wrapper.app`.",
+    )
+    vce_group.add_argument(
+        "--num-supernodes",
+        type=int,
+        help="Number of simulated SuperNodes.",
+    )
+    vce_group.add_argument(
+        "--backend",
+        default="ray",
+        type=str,
+        help="Simulation backend that executes the ClientApp.",
+    )
+    vce_group.add_argument(
+        "--backend-config",
+        type=str,
+        default='{"client_resources": {"num_cpus":1, "num_gpus":0.0}, "tensorflow": 0}',
+        help='A JSON formatted stream, e.g \'{"<keyA>":<value>, "<keyB>":<value>}\' to '
+        "configure a backend. Values supported in <value> are those included by "
+        "`flwr.common.typing.ConfigsRecordValues`. ",
+    )
+    parser.add_argument(
+        "--app-dir",
+        default="",
+        help="Add specified directory to the PYTHONPATH and load"
+        "ClientApp from there."
+        " Default: current working directory.",
+    )
```

### Comparing `flwr-1.7.0/src/py/flwr/server/client_manager.py` & `flwr-1.8.0/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/client_proxy.py` & `flwr-1.8.0/src/py/flwr/server/client_proxy.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,41 +43,46 @@
         self.properties: Properties = {}
 
     @abstractmethod
     def get_properties(
         self,
         ins: GetPropertiesIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> GetPropertiesRes:
         """Return the client's properties."""
 
     @abstractmethod
     def get_parameters(
         self,
         ins: GetParametersIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> GetParametersRes:
         """Return the current local model parameters."""
 
     @abstractmethod
     def fit(
         self,
         ins: FitIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> FitRes:
         """Refine the provided parameters using the locally held dataset."""
 
     @abstractmethod
     def evaluate(
         self,
         ins: EvaluateIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> EvaluateRes:
         """Evaluate the provided parameters using the locally held dataset."""
 
     @abstractmethod
     def reconnect(
         self,
         ins: ReconnectIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
```

### Comparing `flwr-1.7.0/src/py/flwr/server/criterion.py` & `flwr-1.8.0/src/py/flwr/cli/run/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-# Copyright 2020 Flower Labs GmbH. All Rights Reserved.
+# Copyright 2024 Flower Labs GmbH. All Rights Reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Abstract class for criterion sampling."""
+"""Flower command line interface `run` command."""
 
+from .run import run as run
 
-from abc import ABC, abstractmethod
-
-from .client_proxy import ClientProxy
-
-
-class Criterion(ABC):
-    """Abstract class which allows subclasses to implement criterion sampling."""
-
-    @abstractmethod
-    def select(self, client: ClientProxy) -> bool:
-        """Decide whether a client should be eligible for sampling or not."""
+__all__ = [
+    "run",
+]
```

### Comparing `flwr-1.7.0/src/py/flwr/server/driver/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/driver/driver_servicer.py` & `flwr-1.8.0/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Driver API servicer."""
 
 
-from logging import INFO
+import time
+from logging import DEBUG, INFO
 from typing import List, Optional, Set
 from uuid import UUID
 
 import grpc
 
 from flwr.common.logger import log
 from flwr.proto import driver_pb2_grpc  # pylint: disable=E0611
@@ -31,29 +32,29 @@
     PullTaskResRequest,
     PullTaskResResponse,
     PushTaskInsRequest,
     PushTaskInsResponse,
 )
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.task_pb2 import TaskRes  # pylint: disable=E0611
-from flwr.server.state import State, StateFactory
+from flwr.server.superlink.state import State, StateFactory
 from flwr.server.utils.validator import validate_task_ins_or_res
 
 
 class DriverServicer(driver_pb2_grpc.DriverServicer):
     """Driver API servicer."""
 
     def __init__(self, state_factory: StateFactory) -> None:
         self.state_factory = state_factory
 
     def GetNodes(
         self, request: GetNodesRequest, context: grpc.ServicerContext
     ) -> GetNodesResponse:
         """Get available nodes."""
-        log(INFO, "DriverServicer.GetNodes")
+        log(DEBUG, "DriverServicer.GetNodes")
         state: State = self.state_factory.state()
         all_ids: Set[int] = state.get_nodes(request.run_id)
         nodes: List[Node] = [
             Node(node_id=node_id, anonymous=False) for node_id in all_ids
         ]
         return GetNodesResponse(nodes=nodes)
 
@@ -66,15 +67,20 @@
         run_id = state.create_run()
         return CreateRunResponse(run_id=run_id)
 
     def PushTaskIns(
         self, request: PushTaskInsRequest, context: grpc.ServicerContext
     ) -> PushTaskInsResponse:
         """Push a set of TaskIns."""
-        log(INFO, "DriverServicer.PushTaskIns")
+        log(DEBUG, "DriverServicer.PushTaskIns")
+
+        # Set pushed_at (timestamp in seconds)
+        pushed_at = time.time()
+        for task_ins in request.task_ins_list:
+            task_ins.task.pushed_at = pushed_at
 
         # Validate request
         _raise_if(len(request.task_ins_list) == 0, "`task_ins_list` must not be empty")
         for task_ins in request.task_ins_list:
             validation_errors = validate_task_ins_or_res(task_ins)
             _raise_if(bool(validation_errors), ", ".join(validation_errors))
 
@@ -91,25 +97,25 @@
             task_ids=[str(task_id) if task_id else "" for task_id in task_ids]
         )
 
     def PullTaskRes(
         self, request: PullTaskResRequest, context: grpc.ServicerContext
     ) -> PullTaskResResponse:
         """Pull a set of TaskRes."""
-        log(INFO, "DriverServicer.PullTaskRes")
+        log(DEBUG, "DriverServicer.PullTaskRes")
 
         # Convert each task_id str to UUID
         task_ids: Set[UUID] = {UUID(task_id) for task_id in request.task_ids}
 
         # Init state
         state: State = self.state_factory.state()
 
         # Register callback
         def on_rpc_done() -> None:
-            log(INFO, "DriverServicer.PullTaskRes callback: delete TaskIns/TaskRes")
+            log(DEBUG, "DriverServicer.PullTaskRes callback: delete TaskIns/TaskRes")
 
             if context.is_active():
                 return
             if context.code() != grpc.StatusCode.OK:
                 return
 
             # Delete delivered TaskIns and TaskRes
```

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/flower_service_servicer.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,20 @@
 
 from flwr.proto import transport_pb2_grpc  # pylint: disable=E0611
 from flwr.proto.transport_pb2 import (  # pylint: disable=E0611
     ClientMessage,
     ServerMessage,
 )
 from flwr.server.client_manager import ClientManager
-from flwr.server.fleet.grpc_bidi.grpc_bridge import GrpcBridge, InsWrapper, ResWrapper
-from flwr.server.fleet.grpc_bidi.grpc_client_proxy import GrpcClientProxy
+from flwr.server.superlink.fleet.grpc_bidi.grpc_bridge import (
+    GrpcBridge,
+    InsWrapper,
+    ResWrapper,
+)
+from flwr.server.superlink.fleet.grpc_bidi.grpc_client_proxy import GrpcClientProxy
 
 
 def default_bridge_factory() -> GrpcBridge:
     """Return GrpcBridge instance."""
     return GrpcBridge()
```

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/grpc_bridge.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,19 @@
 from flwr import common
 from flwr.common import serde
 from flwr.proto.transport_pb2 import (  # pylint: disable=E0611
     ClientMessage,
     ServerMessage,
 )
 from flwr.server.client_proxy import ClientProxy
-from flwr.server.fleet.grpc_bidi.grpc_bridge import GrpcBridge, InsWrapper, ResWrapper
+from flwr.server.superlink.fleet.grpc_bidi.grpc_bridge import (
+    GrpcBridge,
+    InsWrapper,
+    ResWrapper,
+)
 
 
 class GrpcClientProxy(ClientProxy):
     """Flower ClientProxy that uses gRPC to delegate tasks over the network."""
 
     def __init__(
         self,
@@ -38,14 +42,15 @@
         super().__init__(cid)
         self.bridge = bridge
 
     def get_properties(
         self,
         ins: common.GetPropertiesIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> common.GetPropertiesRes:
         """Request client's set of internal properties."""
         get_properties_msg = serde.get_properties_ins_to_proto(ins)
         res_wrapper: ResWrapper = self.bridge.request(
             ins_wrapper=InsWrapper(
                 server_message=ServerMessage(get_properties_ins=get_properties_msg),
                 timeout=timeout,
@@ -57,14 +62,15 @@
         )
         return get_properties_res
 
     def get_parameters(
         self,
         ins: common.GetParametersIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> common.GetParametersRes:
         """Return the current local model parameters."""
         get_parameters_msg = serde.get_parameters_ins_to_proto(ins)
         res_wrapper: ResWrapper = self.bridge.request(
             ins_wrapper=InsWrapper(
                 server_message=ServerMessage(get_parameters_ins=get_parameters_msg),
                 timeout=timeout,
@@ -76,14 +82,15 @@
         )
         return get_parameters_res
 
     def fit(
         self,
         ins: common.FitIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> common.FitRes:
         """Refine the provided parameters using the locally held dataset."""
         fit_ins_msg = serde.fit_ins_to_proto(ins)
 
         res_wrapper: ResWrapper = self.bridge.request(
             ins_wrapper=InsWrapper(
                 server_message=ServerMessage(fit_ins=fit_ins_msg),
@@ -94,14 +101,15 @@
         fit_res = serde.fit_res_from_proto(client_msg.fit_res)
         return fit_res
 
     def evaluate(
         self,
         ins: common.EvaluateIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> common.EvaluateRes:
         """Evaluate the provided parameters using the locally held dataset."""
         evaluate_msg = serde.evaluate_ins_to_proto(ins)
         res_wrapper: ResWrapper = self.bridge.request(
             ins_wrapper=InsWrapper(
                 server_message=ServerMessage(evaluate_ins=evaluate_msg),
                 timeout=timeout,
@@ -111,14 +119,15 @@
         evaluate_res = serde.evaluate_res_from_proto(client_msg.evaluate_res)
         return evaluate_res
 
     def reconnect(
         self,
         ins: common.ReconnectIns,
         timeout: Optional[float],
+        group_id: Optional[int],
     ) -> common.DisconnectRes:
         """Disconnect and (optionally) reconnect later."""
         reconnect_ins_msg = serde.reconnect_ins_to_proto(ins)
         res_wrapper: ResWrapper = self.bridge.request(
             ins_wrapper=InsWrapper(
                 server_message=ServerMessage(reconnect_ins=reconnect_ins_msg),
                 timeout=timeout,
```

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/grpc_bidi/grpc_server.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
 from flwr.common.logger import log
 from flwr.proto.transport_pb2_grpc import (  # pylint: disable=E0611
     add_FlowerServiceServicer_to_server,
 )
 from flwr.server.client_manager import ClientManager
-from flwr.server.driver.driver_servicer import DriverServicer
-from flwr.server.fleet.grpc_bidi.flower_service_servicer import FlowerServiceServicer
-from flwr.server.fleet.grpc_rere.fleet_servicer import FleetServicer
+from flwr.server.superlink.driver.driver_servicer import DriverServicer
+from flwr.server.superlink.fleet.grpc_bidi.flower_service_servicer import (
+    FlowerServiceServicer,
+)
+from flwr.server.superlink.fleet.grpc_rere.fleet_servicer import FleetServicer
 
 INVALID_CERTIFICATES_ERR_MSG = """
     When setting any of root_certificate, certificate, or private_key,
     all of them need to be set.
 """
 
 AddServicerToServerFn = Callable[..., Any]
```

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/grpc_rere/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/grpc_rere/fleet_servicer.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,32 +11,34 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Fleet API gRPC request-response servicer."""
 
 
-from logging import INFO
+from logging import DEBUG, INFO
 
 import grpc
 
 from flwr.common.logger import log
 from flwr.proto import fleet_pb2_grpc  # pylint: disable=E0611
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     CreateNodeResponse,
     DeleteNodeRequest,
     DeleteNodeResponse,
+    PingRequest,
+    PingResponse,
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
 )
-from flwr.server.fleet.message_handler import message_handler
-from flwr.server.state import StateFactory
+from flwr.server.superlink.fleet.message_handler import message_handler
+from flwr.server.superlink.state import StateFactory
 
 
 class FleetServicer(fleet_pb2_grpc.FleetServicer):
     """Fleet API servicer."""
 
     def __init__(self, state_factory: StateFactory) -> None:
         self.state_factory = state_factory
@@ -57,14 +59,22 @@
         """."""
         log(INFO, "FleetServicer.DeleteNode")
         return message_handler.delete_node(
             request=request,
             state=self.state_factory.state(),
         )
 
+    def Ping(self, request: PingRequest, context: grpc.ServicerContext) -> PingResponse:
+        """."""
+        log(DEBUG, "FleetServicer.Ping")
+        return message_handler.ping(
+            request=request,
+            state=self.state_factory.state(),
+        )
+
     def PullTaskIns(
         self, request: PullTaskInsRequest, context: grpc.ServicerContext
     ) -> PullTaskInsResponse:
         """Pull TaskIns."""
         log(INFO, "FleetServicer.PullTaskIns")
         return message_handler.pull_task_ins(
             request=request,
```

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/message_handler/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/message_handler/message_handler.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,54 +11,66 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Fleet API message handlers."""
 
 
+import time
 from typing import List, Optional
 from uuid import UUID
 
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     CreateNodeResponse,
     DeleteNodeRequest,
     DeleteNodeResponse,
+    PingRequest,
+    PingResponse,
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
     Reconnect,
 )
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.task_pb2 import TaskIns, TaskRes  # pylint: disable=E0611
-from flwr.server.state import State
+from flwr.server.superlink.state import State
 
 
 def create_node(
     request: CreateNodeRequest,  # pylint: disable=unused-argument
     state: State,
 ) -> CreateNodeResponse:
     """."""
     # Create node
-    node_id = state.create_node()
+    node_id = state.create_node(ping_interval=request.ping_interval)
     return CreateNodeResponse(node=Node(node_id=node_id, anonymous=False))
 
 
 def delete_node(request: DeleteNodeRequest, state: State) -> DeleteNodeResponse:
     """."""
     # Validate node_id
-    if request.node.anonymous or request.node.node_id <= 0:
+    if request.node.anonymous or request.node.node_id == 0:
         return DeleteNodeResponse()
 
     # Update state
     state.delete_node(node_id=request.node.node_id)
     return DeleteNodeResponse()
 
 
+def ping(
+    request: PingRequest,  # pylint: disable=unused-argument
+    state: State,  # pylint: disable=unused-argument
+) -> PingResponse:
+    """."""
+    res = state.acknowledge_ping(request.node.node_id, request.ping_interval)
+    return PingResponse(success=res)
+
+
 def pull_task_ins(request: PullTaskInsRequest, state: State) -> PullTaskInsResponse:
     """Pull TaskIns handler."""
     # Get node_id if client node is not anonymous
     node = request.node  # pylint: disable=no-member
     node_id: Optional[int] = None if node.anonymous else node.node_id
 
     # Retrieve TaskIns from State
@@ -73,14 +85,17 @@
 
 def push_task_res(request: PushTaskResRequest, state: State) -> PushTaskResResponse:
     """Push TaskRes handler."""
     # pylint: disable=no-member
     task_res: TaskRes = request.task_res_list[0]
     # pylint: enable=no-member
 
+    # Set pushed_at (timestamp in seconds)
+    task_res.task.pushed_at = time.time()
+
     # Store TaskRes in State
     task_id: Optional[UUID] = state.store_task_res(task_res=task_res)
 
     # Build response
     response = PushTaskResResponse(
         reconnect=Reconnect(reconnect=5),
         results={str(task_id): 0},
```

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/rest_rere/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/fleet/rest_rere/rest_api.py` & `flwr-1.8.0/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,19 +17,20 @@
 
 import sys
 
 from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     DeleteNodeRequest,
+    PingRequest,
     PullTaskInsRequest,
     PushTaskResRequest,
 )
-from flwr.server.fleet.message_handler import message_handler
-from flwr.server.state import State
+from flwr.server.superlink.fleet.message_handler import message_handler
+from flwr.server.superlink.state import State
 
 try:
     from starlette.applications import Starlette
     from starlette.datastructures import Headers
     from starlette.exceptions import HTTPException
     from starlette.requests import Request
     from starlette.responses import Response
@@ -148,19 +149,46 @@
     return Response(
         status_code=200,
         content=push_task_res_response_bytes,
         headers={"Content-Type": "application/protobuf"},
     )
 
 
+async def ping(request: Request) -> Response:
+    """Ping."""
+    _check_headers(request.headers)
+
+    # Get the request body as raw bytes
+    ping_request_bytes: bytes = await request.body()
+
+    # Deserialize ProtoBuf
+    ping_request_proto = PingRequest()
+    ping_request_proto.ParseFromString(ping_request_bytes)
+
+    # Get state from app
+    state: State = app.state.STATE_FACTORY.state()
+
+    # Handle message
+    ping_response_proto = message_handler.ping(request=ping_request_proto, state=state)
+
+    # Return serialized ProtoBuf
+    ping_response_bytes = ping_response_proto.SerializeToString()
+    return Response(
+        status_code=200,
+        content=ping_response_bytes,
+        headers={"Content-Type": "application/protobuf"},
+    )
+
+
 routes = [
     Route("/api/v0/fleet/create-node", create_node, methods=["POST"]),
     Route("/api/v0/fleet/delete-node", delete_node, methods=["POST"]),
     Route("/api/v0/fleet/pull-task-ins", pull_task_ins, methods=["POST"]),
     Route("/api/v0/fleet/push-task-res", push_task_res, methods=["POST"]),
+    Route("/api/v0/fleet/ping", ping, methods=["POST"]),
 ]
 
 app: Starlette = Starlette(
     debug=False,
     routes=routes,
 )
```

### Comparing `flwr-1.7.0/src/py/flwr/server/history.py` & `flwr-1.8.0/src/py/flwr/server/history.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Training history."""
 
 
+import pprint
 from functools import reduce
 from typing import Dict, List, Tuple
 
 from flwr.common.typing import Scalar
 
 
 class History:
@@ -86,33 +87,39 @@
         Returns
         -------
         representation : str
             The string representation of the history object.
         """
         rep = ""
         if self.losses_distributed:
-            rep += "History (loss, distributed):\n" + reduce(
-                lambda a, b: a + b,
-                [
-                    f"\tround {server_round}: {loss}\n"
-                    for server_round, loss in self.losses_distributed
-                ],
+            rep += "History (loss, distributed):\n" + pprint.pformat(
+                reduce(
+                    lambda a, b: a + b,
+                    [
+                        f"\tround {server_round}: {loss}\n"
+                        for server_round, loss in self.losses_distributed
+                    ],
+                )
             )
         if self.losses_centralized:
-            rep += "History (loss, centralized):\n" + reduce(
-                lambda a, b: a + b,
-                [
-                    f"\tround {server_round}: {loss}\n"
-                    for server_round, loss in self.losses_centralized
-                ],
+            rep += "History (loss, centralized):\n" + pprint.pformat(
+                reduce(
+                    lambda a, b: a + b,
+                    [
+                        f"\tround {server_round}: {loss}\n"
+                        for server_round, loss in self.losses_centralized
+                    ],
+                )
             )
         if self.metrics_distributed_fit:
-            rep += "History (metrics, distributed, fit):\n" + str(
+            rep += "History (metrics, distributed, fit):\n" + pprint.pformat(
                 self.metrics_distributed_fit
             )
         if self.metrics_distributed:
-            rep += "History (metrics, distributed, evaluate):\n" + str(
+            rep += "History (metrics, distributed, evaluate):\n" + pprint.pformat(
                 self.metrics_distributed
             )
         if self.metrics_centralized:
-            rep += "History (metrics, centralized):\n" + str(self.metrics_centralized)
+            rep += "History (metrics, centralized):\n" + pprint.pformat(
+                self.metrics_centralized
+            )
         return rep
```

### Comparing `flwr-1.7.0/src/py/flwr/server/server.py` & `flwr-1.8.0/src/py/flwr/server/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,16 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Flower server."""
 
 
 import concurrent.futures
+import io
 import timeit
-from logging import DEBUG, INFO
+from logging import INFO, WARN
 from typing import Dict, List, Optional, Tuple, Union
 
 from flwr.common import (
     Code,
     DisconnectRes,
     EvaluateIns,
     EvaluateRes,
@@ -29,19 +30,21 @@
     FitRes,
     Parameters,
     ReconnectIns,
     Scalar,
 )
 from flwr.common.logger import log
 from flwr.common.typing import GetParametersIns
-from flwr.server.client_manager import ClientManager
+from flwr.server.client_manager import ClientManager, SimpleClientManager
 from flwr.server.client_proxy import ClientProxy
 from flwr.server.history import History
 from flwr.server.strategy import FedAvg, Strategy
 
+from .server_config import ServerConfig
+
 FitResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, FitRes]],
     List[Union[Tuple[ClientProxy, FitRes], BaseException]],
 ]
 EvaluateResultsAndFailures = Tuple[
     List[Tuple[ClientProxy, EvaluateRes]],
     List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]],
@@ -77,38 +80,39 @@
         self.strategy = strategy
 
     def client_manager(self) -> ClientManager:
         """Return ClientManager."""
         return self._client_manager
 
     # pylint: disable=too-many-locals
-    def fit(self, num_rounds: int, timeout: Optional[float]) -> History:
+    def fit(self, num_rounds: int, timeout: Optional[float]) -> Tuple[History, float]:
         """Run federated averaging for a number of rounds."""
         history = History()
 
         # Initialize parameters
-        log(INFO, "Initializing global parameters")
-        self.parameters = self._get_initial_parameters(timeout=timeout)
-        log(INFO, "Evaluating initial parameters")
+        log(INFO, "[INIT]")
+        self.parameters = self._get_initial_parameters(server_round=0, timeout=timeout)
+        log(INFO, "Evaluating initial global parameters")
         res = self.strategy.evaluate(0, parameters=self.parameters)
         if res is not None:
             log(
                 INFO,
                 "initial parameters (loss, other metrics): %s, %s",
                 res[0],
                 res[1],
             )
             history.add_loss_centralized(server_round=0, loss=res[0])
             history.add_metrics_centralized(server_round=0, metrics=res[1])
 
         # Run federated learning for num_rounds
-        log(INFO, "FL starting")
         start_time = timeit.default_timer()
 
         for current_round in range(1, num_rounds + 1):
+            log(INFO, "")
+            log(INFO, "[ROUND %s]", current_round)
             # Train model and replace previous global model
             res_fit = self.fit_round(
                 server_round=current_round,
                 timeout=timeout,
             )
             if res_fit is not None:
                 parameters_prime, fit_metrics, _ = res_fit  # fit_metrics_aggregated
@@ -146,16 +150,15 @@
                     history.add_metrics_distributed(
                         server_round=current_round, metrics=evaluate_metrics_fed
                     )
 
         # Bookkeeping
         end_time = timeit.default_timer()
         elapsed = end_time - start_time
-        log(INFO, "FL finished in %s", elapsed)
-        return history
+        return history, elapsed
 
     def evaluate_round(
         self,
         server_round: int,
         timeout: Optional[float],
     ) -> Optional[
         Tuple[Optional[float], Dict[str, Scalar], EvaluateResultsAndFailures]
@@ -164,34 +167,33 @@
         # Get clients and their respective instructions from strategy
         client_instructions = self.strategy.configure_evaluate(
             server_round=server_round,
             parameters=self.parameters,
             client_manager=self._client_manager,
         )
         if not client_instructions:
-            log(INFO, "evaluate_round %s: no clients selected, cancel", server_round)
+            log(INFO, "configure_evaluate: no clients selected, skipping evaluation")
             return None
         log(
-            DEBUG,
-            "evaluate_round %s: strategy sampled %s clients (out of %s)",
-            server_round,
+            INFO,
+            "configure_evaluate: strategy sampled %s clients (out of %s)",
             len(client_instructions),
             self._client_manager.num_available(),
         )
 
         # Collect `evaluate` results from all clients participating in this round
         results, failures = evaluate_clients(
             client_instructions,
             max_workers=self.max_workers,
             timeout=timeout,
+            group_id=server_round,
         )
         log(
-            DEBUG,
-            "evaluate_round %s received %s results and %s failures",
-            server_round,
+            INFO,
+            "aggregate_evaluate: received %s results and %s failures",
             len(results),
             len(failures),
         )
 
         # Aggregate the evaluation results
         aggregated_result: Tuple[
             Optional[float],
@@ -213,34 +215,33 @@
         client_instructions = self.strategy.configure_fit(
             server_round=server_round,
             parameters=self.parameters,
             client_manager=self._client_manager,
         )
 
         if not client_instructions:
-            log(INFO, "fit_round %s: no clients selected, cancel", server_round)
+            log(INFO, "configure_fit: no clients selected, cancel")
             return None
         log(
-            DEBUG,
-            "fit_round %s: strategy sampled %s clients (out of %s)",
-            server_round,
+            INFO,
+            "configure_fit: strategy sampled %s clients (out of %s)",
             len(client_instructions),
             self._client_manager.num_available(),
         )
 
         # Collect `fit` results from all clients participating in this round
         results, failures = fit_clients(
             client_instructions=client_instructions,
             max_workers=self.max_workers,
             timeout=timeout,
+            group_id=server_round,
         )
         log(
-            DEBUG,
-            "fit_round %s received %s results and %s failures",
-            server_round,
+            INFO,
+            "aggregate_fit: received %s results and %s failures",
             len(results),
             len(failures),
         )
 
         # Aggregate training results
         aggregated_result: Tuple[
             Optional[Parameters],
@@ -258,29 +259,33 @@
         client_instructions = [(client_proxy, instruction) for client_proxy in clients]
         _ = reconnect_clients(
             client_instructions=client_instructions,
             max_workers=self.max_workers,
             timeout=timeout,
         )
 
-    def _get_initial_parameters(self, timeout: Optional[float]) -> Parameters:
+    def _get_initial_parameters(
+        self, server_round: int, timeout: Optional[float]
+    ) -> Parameters:
         """Get initial parameters from one of the available clients."""
         # Server-side parameter initialization
         parameters: Optional[Parameters] = self.strategy.initialize_parameters(
             client_manager=self._client_manager
         )
         if parameters is not None:
-            log(INFO, "Using initial parameters provided by strategy")
+            log(INFO, "Using initial global parameters provided by strategy")
             return parameters
 
         # Get initial parameters from one of the clients
         log(INFO, "Requesting initial parameters from one random client")
         random_client = self._client_manager.sample(1)[0]
         ins = GetParametersIns(config={})
-        get_parameters_res = random_client.get_parameters(ins=ins, timeout=timeout)
+        get_parameters_res = random_client.get_parameters(
+            ins=ins, timeout=timeout, group_id=server_round
+        )
         log(INFO, "Received initial parameters from one random client")
         return get_parameters_res.parameters
 
 
 def reconnect_clients(
     client_instructions: List[Tuple[ClientProxy, ReconnectIns]],
     max_workers: Optional[int],
@@ -315,27 +320,29 @@
     reconnect: ReconnectIns,
     timeout: Optional[float],
 ) -> Tuple[ClientProxy, DisconnectRes]:
     """Instruct client to disconnect and (optionally) reconnect later."""
     disconnect = client.reconnect(
         reconnect,
         timeout=timeout,
+        group_id=None,
     )
     return client, disconnect
 
 
 def fit_clients(
     client_instructions: List[Tuple[ClientProxy, FitIns]],
     max_workers: Optional[int],
     timeout: Optional[float],
+    group_id: int,
 ) -> FitResultsAndFailures:
     """Refine parameters concurrently on all selected clients."""
     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
         submitted_fs = {
-            executor.submit(fit_client, client_proxy, ins, timeout)
+            executor.submit(fit_client, client_proxy, ins, timeout, group_id)
             for client_proxy, ins in client_instructions
         }
         finished_fs, _ = concurrent.futures.wait(
             fs=submitted_fs,
             timeout=None,  # Handled in the respective communication stack
         )
 
@@ -346,18 +353,18 @@
         _handle_finished_future_after_fit(
             future=future, results=results, failures=failures
         )
     return results, failures
 
 
 def fit_client(
-    client: ClientProxy, ins: FitIns, timeout: Optional[float]
+    client: ClientProxy, ins: FitIns, timeout: Optional[float], group_id: int
 ) -> Tuple[ClientProxy, FitRes]:
     """Refine parameters on a single client."""
-    fit_res = client.fit(ins, timeout=timeout)
+    fit_res = client.fit(ins, timeout=timeout, group_id=group_id)
     return client, fit_res
 
 
 def _handle_finished_future_after_fit(
     future: concurrent.futures.Future,  # type: ignore
     results: List[Tuple[ClientProxy, FitRes]],
     failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
@@ -382,19 +389,20 @@
     failures.append(result)
 
 
 def evaluate_clients(
     client_instructions: List[Tuple[ClientProxy, EvaluateIns]],
     max_workers: Optional[int],
     timeout: Optional[float],
+    group_id: int,
 ) -> EvaluateResultsAndFailures:
     """Evaluate parameters concurrently on all selected clients."""
     with concurrent.futures.ThreadPoolExecutor(max_workers=max_workers) as executor:
         submitted_fs = {
-            executor.submit(evaluate_client, client_proxy, ins, timeout)
+            executor.submit(evaluate_client, client_proxy, ins, timeout, group_id)
             for client_proxy, ins in client_instructions
         }
         finished_fs, _ = concurrent.futures.wait(
             fs=submitted_fs,
             timeout=None,  # Handled in the respective communication stack
         )
 
@@ -408,17 +416,18 @@
     return results, failures
 
 
 def evaluate_client(
     client: ClientProxy,
     ins: EvaluateIns,
     timeout: Optional[float],
+    group_id: int,
 ) -> Tuple[ClientProxy, EvaluateRes]:
     """Evaluate parameters on a single client."""
-    evaluate_res = client.evaluate(ins, timeout=timeout)
+    evaluate_res = client.evaluate(ins, timeout=timeout, group_id=group_id)
     return client, evaluate_res
 
 
 def _handle_finished_future_after_evaluate(
     future: concurrent.futures.Future,  # type: ignore
     results: List[Tuple[ClientProxy, EvaluateRes]],
     failures: List[Union[Tuple[ClientProxy, EvaluateRes], BaseException]],
@@ -437,7 +446,55 @@
     # Check result status code
     if res.status.code == Code.OK:
         results.append(result)
         return
 
     # Not successful, client returned a result where the status code is not OK
     failures.append(result)
+
+
+def init_defaults(
+    server: Optional[Server],
+    config: Optional[ServerConfig],
+    strategy: Optional[Strategy],
+    client_manager: Optional[ClientManager],
+) -> Tuple[Server, ServerConfig]:
+    """Create server instance if none was given."""
+    if server is None:
+        if client_manager is None:
+            client_manager = SimpleClientManager()
+        if strategy is None:
+            strategy = FedAvg()
+        server = Server(client_manager=client_manager, strategy=strategy)
+    elif strategy is not None:
+        log(WARN, "Both server and strategy were provided, ignoring strategy")
+
+    # Set default config values
+    if config is None:
+        config = ServerConfig()
+
+    return server, config
+
+
+def run_fl(
+    server: Server,
+    config: ServerConfig,
+) -> History:
+    """Train a model on the given server and return the History object."""
+    hist, elapsed_time = server.fit(
+        num_rounds=config.num_rounds, timeout=config.round_timeout
+    )
+
+    log(INFO, "")
+    log(INFO, "[SUMMARY]")
+    log(INFO, "Run finished %s rounds in %.2fs", config.num_rounds, elapsed_time)
+    for idx, line in enumerate(io.StringIO(str(hist))):
+        if idx == 0:
+            log(INFO, "%s", line.strip("\n"))
+        else:
+            log(INFO, "\t%s", line.strip("\n"))
+    log(INFO, "")
+
+    # Graceful shutdown
+    server.disconnect_all_clients(timeout=config.round_timeout)
+
+    return hist
```

### Comparing `flwr-1.7.0/src/py/flwr/server/state/__init__.py` & `flwr-1.8.0/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/state/sqlite_state.py` & `flwr-1.8.0/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,33 +14,40 @@
 # ==============================================================================
 """SQLite based implemenation of server state."""
 
 
 import os
 import re
 import sqlite3
-from datetime import datetime, timedelta
+import time
 from logging import DEBUG, ERROR
 from typing import Any, Dict, List, Optional, Set, Tuple, Union, cast
 from uuid import UUID, uuid4
 
 from flwr.common import log, now
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.recordset_pb2 import RecordSet  # pylint: disable=E0611
 from flwr.proto.task_pb2 import Task, TaskIns, TaskRes  # pylint: disable=E0611
 from flwr.server.utils.validator import validate_task_ins_or_res
 
 from .state import State
+from .utils import make_node_unavailable_taskres
 
 SQL_CREATE_TABLE_NODE = """
 CREATE TABLE IF NOT EXISTS node(
-    node_id INTEGER UNIQUE
+    node_id         INTEGER UNIQUE,
+    online_until    REAL,
+    ping_interval   REAL
 );
 """
 
+SQL_CREATE_INDEX_ONLINE_UNTIL = """
+CREATE INDEX IF NOT EXISTS idx_online_until ON node (online_until);
+"""
+
 SQL_CREATE_TABLE_RUN = """
 CREATE TABLE IF NOT EXISTS run(
     run_id INTEGER UNIQUE
 );
 """
 
 SQL_CREATE_TABLE_TASK_INS = """
@@ -48,17 +55,18 @@
     task_id                 TEXT UNIQUE,
     group_id                TEXT,
     run_id                  INTEGER,
     producer_anonymous      BOOLEAN,
     producer_node_id        INTEGER,
     consumer_anonymous      BOOLEAN,
     consumer_node_id        INTEGER,
-    created_at              TEXT,
+    created_at              REAL,
     delivered_at            TEXT,
-    ttl                     TEXT,
+    pushed_at               REAL,
+    ttl                     REAL,
     ancestry                TEXT,
     task_type               TEXT,
     recordset               BLOB,
     FOREIGN KEY(run_id) REFERENCES run(run_id)
 );
 """
 
@@ -68,25 +76,26 @@
     task_id                 TEXT UNIQUE,
     group_id                TEXT,
     run_id                  INTEGER,
     producer_anonymous      BOOLEAN,
     producer_node_id        INTEGER,
     consumer_anonymous      BOOLEAN,
     consumer_node_id        INTEGER,
-    created_at              TEXT,
+    created_at              REAL,
     delivered_at            TEXT,
-    ttl                     TEXT,
+    pushed_at               REAL,
+    ttl                     REAL,
     ancestry                TEXT,
     task_type               TEXT,
     recordset               BLOB,
     FOREIGN KEY(run_id) REFERENCES run(run_id)
 );
 """
 
-DictOrTuple = Union[Tuple[Any], Dict[str, Any]]
+DictOrTuple = Union[Tuple[Any, ...], Dict[str, Any]]
 
 
 class SqliteState(State):
     """SQLite-based state implementation."""
 
     def __init__(
         self,
@@ -119,14 +128,15 @@
         cur = self.conn.cursor()
 
         # Create each table if not exists queries
         cur.execute(SQL_CREATE_TABLE_RUN)
         cur.execute(SQL_CREATE_TABLE_TASK_INS)
         cur.execute(SQL_CREATE_TABLE_TASK_RES)
         cur.execute(SQL_CREATE_TABLE_NODE)
+        cur.execute(SQL_CREATE_INDEX_ONLINE_UNTIL)
         res = cur.execute("SELECT name FROM sqlite_schema;")
 
         return res.fetchall()
 
     def query(
         self,
         query: str,
@@ -181,23 +191,19 @@
         """
         # Validate task
         errors = validate_task_ins_or_res(task_ins)
         if any(errors):
             log(ERROR, errors)
             return None
 
-        # Create task_id, created_at and ttl
+        # Create task_id
         task_id = uuid4()
-        created_at: datetime = now()
-        ttl: datetime = created_at + timedelta(hours=24)
 
         # Store TaskIns
         task_ins.task_id = str(task_id)
-        task_ins.task.created_at = created_at.isoformat()
-        task_ins.task.ttl = ttl.isoformat()
         data = (task_ins_to_dict(task_ins),)
         columns = ", ".join([f":{key}" for key in data[0]])
         query = f"INSERT INTO task_ins VALUES({columns});"
 
         # Only invalid run_id can trigger IntegrityError.
         # This may need to be changed in the future version with more integrity checks.
         try:
@@ -316,37 +322,34 @@
         """
         # Validate task
         errors = validate_task_ins_or_res(task_res)
         if any(errors):
             log(ERROR, errors)
             return None
 
-        # Create task_id, created_at and ttl
+        # Create task_id
         task_id = uuid4()
-        created_at: datetime = now()
-        ttl: datetime = created_at + timedelta(hours=24)
 
         # Store TaskIns
         task_res.task_id = str(task_id)
-        task_res.task.created_at = created_at.isoformat()
-        task_res.task.ttl = ttl.isoformat()
         data = (task_res_to_dict(task_res),)
         columns = ", ".join([f":{key}" for key in data[0]])
         query = f"INSERT INTO task_res VALUES({columns});"
 
         # Only invalid run_id can trigger IntegrityError.
         # This may need to be changed in the future version with more integrity checks.
         try:
             self.query(query, data)
         except sqlite3.IntegrityError:
             log(ERROR, "`run` is invalid")
             return None
 
         return task_id
 
+    # pylint: disable-next=R0914
     def get_task_res(self, task_ids: Set[UUID], limit: Optional[int]) -> List[TaskRes]:
         """Get TaskRes for task_ids.
 
         Usually, the Driver API calls this method to get results for instructions it has
         previously scheduled.
 
         Retrieves all TaskRes for the given `task_ids` and returns and empty list if
@@ -369,15 +372,15 @@
         query = f"""
             SELECT *
             FROM task_res
             WHERE ancestry IN ({placeholders})
             AND delivered_at = ""
         """
 
-        data: Dict[str, Union[str, int]] = {}
+        data: Dict[str, Union[str, float, int]] = {}
 
         if limit is not None:
             query += " LIMIT :limit"
             data["limit"] = limit
 
         query += ";"
 
@@ -403,14 +406,62 @@
             for index, task_id in enumerate(found_task_ids):
                 data[f"id_{index}"] = str(task_id)
 
             # Run query
             rows = self.query(query, data)
 
         result = [dict_to_task_res(row) for row in rows]
+
+        # 1. Query: Fetch consumer_node_id of remaining task_ids
+        # Assume the ancestry field only contains one element
+        data.clear()
+        replied_task_ids: Set[UUID] = {UUID(str(row["ancestry"])) for row in rows}
+        remaining_task_ids = task_ids - replied_task_ids
+        placeholders = ",".join([f":id_{i}" for i in range(len(remaining_task_ids))])
+        query = f"""
+            SELECT consumer_node_id
+            FROM task_ins
+            WHERE task_id IN ({placeholders});
+        """
+        for index, task_id in enumerate(remaining_task_ids):
+            data[f"id_{index}"] = str(task_id)
+        node_ids = [int(row["consumer_node_id"]) for row in self.query(query, data)]
+
+        # 2. Query: Select offline nodes
+        placeholders = ",".join([f":id_{i}" for i in range(len(node_ids))])
+        query = f"""
+            SELECT node_id
+            FROM node
+            WHERE node_id IN ({placeholders})
+            AND online_until < :time;
+        """
+        data = {f"id_{i}": str(node_id) for i, node_id in enumerate(node_ids)}
+        data["time"] = time.time()
+        offline_node_ids = [int(row["node_id"]) for row in self.query(query, data)]
+
+        # 3. Query: Select TaskIns for offline nodes
+        placeholders = ",".join([f":id_{i}" for i in range(len(offline_node_ids))])
+        query = f"""
+            SELECT *
+            FROM task_ins
+            WHERE consumer_node_id IN ({placeholders});
+        """
+        data = {f"id_{i}": str(node_id) for i, node_id in enumerate(offline_node_ids)}
+        task_ins_rows = self.query(query, data)
+
+        # Make TaskRes containing node unavailabe error
+        for row in task_ins_rows:
+            if limit and len(result) == limit:
+                break
+            task_ins = dict_to_task_ins(row)
+            err_taskres = make_node_unavailable_taskres(
+                ref_taskins=task_ins,
+            )
+            result.append(err_taskres)
+
         return result
 
     def num_task_ins(self) -> int:
         """Calculate the number of task_ins in store.
 
         This includes delivered but not yet deleted task_ins.
         """
@@ -463,22 +514,25 @@
 
         with self.conn:
             self.conn.execute(query_1, data)
             self.conn.execute(query_2, data)
 
         return None
 
-    def create_node(self) -> int:
+    def create_node(self, ping_interval: float) -> int:
         """Create, store in state, and return `node_id`."""
         # Sample a random int64 as node_id
         node_id: int = int.from_bytes(os.urandom(8), "little", signed=True)
 
-        query = "INSERT INTO node VALUES(:node_id);"
+        query = (
+            "INSERT INTO node (node_id, online_until, ping_interval) VALUES (?, ?, ?)"
+        )
+
         try:
-            self.query(query, {"node_id": node_id})
+            self.query(query, (node_id, time.time() + ping_interval, ping_interval))
         except sqlite3.IntegrityError:
             log(ERROR, "Unexpected node registration failure.")
             return 0
         return node_id
 
     def delete_node(self, node_id: int) -> None:
         """Delete a client node."""
@@ -495,16 +549,16 @@
         """
         # Validate run ID
         query = "SELECT COUNT(*) FROM run WHERE run_id = ?;"
         if self.query(query, (run_id,))[0]["COUNT(*)"] == 0:
             return set()
 
         # Get nodes
-        query = "SELECT * FROM node;"
-        rows = self.query(query)
+        query = "SELECT node_id FROM node WHERE online_until > ?;"
+        rows = self.query(query, (time.time(),))
         result: Set[int] = {row["node_id"] for row in rows}
         return result
 
     def create_run(self) -> int:
         """Create one run and store it in state."""
         # Sample a random int64 as run_id
         run_id: int = int.from_bytes(os.urandom(8), "little", signed=True)
@@ -515,14 +569,25 @@
         if self.query(query, (run_id,))[0]["COUNT(*)"] == 0:
             query = "INSERT INTO run VALUES(:run_id);"
             self.query(query, {"run_id": run_id})
             return run_id
         log(ERROR, "Unexpected run creation failure.")
         return 0
 
+    def acknowledge_ping(self, node_id: int, ping_interval: float) -> bool:
+        """Acknowledge a ping received from a node, serving as a heartbeat."""
+        # Update `online_until` and `ping_interval` for the given `node_id`
+        query = "UPDATE node SET online_until = ?, ping_interval = ? WHERE node_id = ?;"
+        try:
+            self.query(query, (time.time() + ping_interval, ping_interval, node_id))
+            return True
+        except sqlite3.IntegrityError:
+            log(ERROR, "`node_id` does not exist.")
+            return False
+
 
 def dict_factory(
     cursor: sqlite3.Cursor,
     row: sqlite3.Row,
 ) -> Dict[str, Any]:
     """Turn SQLite results into dicts.
 
@@ -540,14 +605,15 @@
         "run_id": task_msg.run_id,
         "producer_anonymous": task_msg.task.producer.anonymous,
         "producer_node_id": task_msg.task.producer.node_id,
         "consumer_anonymous": task_msg.task.consumer.anonymous,
         "consumer_node_id": task_msg.task.consumer.node_id,
         "created_at": task_msg.task.created_at,
         "delivered_at": task_msg.task.delivered_at,
+        "pushed_at": task_msg.task.pushed_at,
         "ttl": task_msg.task.ttl,
         "ancestry": ",".join(task_msg.task.ancestry),
         "task_type": task_msg.task.task_type,
         "recordset": task_msg.task.recordset.SerializeToString(),
     }
     return result
 
@@ -560,14 +626,15 @@
         "run_id": task_msg.run_id,
         "producer_anonymous": task_msg.task.producer.anonymous,
         "producer_node_id": task_msg.task.producer.node_id,
         "consumer_anonymous": task_msg.task.consumer.anonymous,
         "consumer_node_id": task_msg.task.consumer.node_id,
         "created_at": task_msg.task.created_at,
         "delivered_at": task_msg.task.delivered_at,
+        "pushed_at": task_msg.task.pushed_at,
         "ttl": task_msg.task.ttl,
         "ancestry": ",".join(task_msg.task.ancestry),
         "task_type": task_msg.task.task_type,
         "recordset": task_msg.task.recordset.SerializeToString(),
     }
     return result
 
@@ -588,14 +655,15 @@
             ),
             consumer=Node(
                 node_id=task_dict["consumer_node_id"],
                 anonymous=task_dict["consumer_anonymous"],
             ),
             created_at=task_dict["created_at"],
             delivered_at=task_dict["delivered_at"],
+            pushed_at=task_dict["pushed_at"],
             ttl=task_dict["ttl"],
             ancestry=task_dict["ancestry"].split(","),
             task_type=task_dict["task_type"],
             recordset=recordset,
         ),
     )
     return result
@@ -617,14 +685,15 @@
             ),
             consumer=Node(
                 node_id=task_dict["consumer_node_id"],
                 anonymous=task_dict["consumer_anonymous"],
             ),
             created_at=task_dict["created_at"],
             delivered_at=task_dict["delivered_at"],
+            pushed_at=task_dict["pushed_at"],
             ttl=task_dict["ttl"],
             ancestry=task_dict["ancestry"].split(","),
             task_type=task_dict["task_type"],
             recordset=recordset,
         ),
     )
     return result
```

### Comparing `flwr-1.7.0/src/py/flwr/server/state/state.py` & `flwr-1.8.0/src/py/flwr/server/superlink/state/state.py`

 * *Files 7% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         """
 
     @abc.abstractmethod
     def delete_tasks(self, task_ids: Set[UUID]) -> None:
         """Delete all delivered TaskIns/TaskRes pairs."""
 
     @abc.abstractmethod
-    def create_node(self) -> int:
+    def create_node(self, ping_interval: float) -> int:
         """Create, store in state, and return `node_id`."""
 
     @abc.abstractmethod
     def delete_node(self, node_id: int) -> None:
         """Remove `node_id` from state."""
 
     @abc.abstractmethod
@@ -148,7 +148,26 @@
         If the provided `run_id` does not exist or has no matching nodes,
         an empty `Set` MUST be returned.
         """
 
     @abc.abstractmethod
     def create_run(self) -> int:
         """Create one run."""
+
+    @abc.abstractmethod
+    def acknowledge_ping(self, node_id: int, ping_interval: float) -> bool:
+        """Acknowledge a ping received from a node, serving as a heartbeat.
+
+        Parameters
+        ----------
+        node_id : int
+            The `node_id` from which the ping was received.
+        ping_interval : float
+            The interval (in seconds) from the current timestamp within which the next
+            ping from this node must be received. This acts as a hard deadline to ensure
+            an accurate assessment of the node's availability.
+
+        Returns
+        -------
+        is_acknowledged : bool
+            True if the ping is successfully acknowledged; otherwise, False.
+        """
```

### Comparing `flwr-1.7.0/src/py/flwr/server/state/state_factory.py` & `flwr-1.8.0/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/aggregate.py` & `flwr-1.8.0/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/bulyan.py` & `flwr-1.8.0/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr-1.8.0/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr-1.8.0/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,17 +100,17 @@
             A list of tuples. Each tuple in the list identifies a `ClientProxy` and the
             `FitIns` for this particular `ClientProxy`. If a particular `ClientProxy`
             is not included in this list, it means that this `ClientProxy`
             will not participate in the next round of federated learning.
         """
         additional_config = {"dpfedavg_clip_norm": self.clip_norm}
         if not self.server_side_noising:
-            additional_config[
-                "dpfedavg_noise_stddev"
-            ] = self._calc_client_noise_stddev()
+            additional_config["dpfedavg_noise_stddev"] = (
+                self._calc_client_noise_stddev()
+            )
 
         client_instructions = self.strategy.configure_fit(
             server_round, parameters, client_manager
         )
 
         for _, fit_ins in client_instructions:
             fit_ins.config.update(additional_config)
```

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedadagrad.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedadam.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedavg.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedavg.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         Whether or not accept rounds containing failures. Defaults to True.
     initial_parameters : Parameters, optional
         Initial global model parameters.
     fit_metrics_aggregation_fn : Optional[MetricsAggregationFn]
         Metrics aggregation function, optional.
     evaluate_metrics_aggregation_fn : Optional[MetricsAggregationFn]
         Metrics aggregation function, optional.
+    inplace : bool (default: True)
+        Enable (True) or disable (False) in-place aggregation of model updates.
     """
 
     # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
```

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedavg_android.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedavgm.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedyogi.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,76 +8,85 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Federated Averaging with Momentum (FedAvgM) [Hsu et al., 2019] strategy.
+"""Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al., 2020] strategy.
 
-Paper: arxiv.org/pdf/1909.06335.pdf
+Paper: arxiv.org/abs/2003.00295
 """
 
 
-from logging import WARNING
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
+import numpy as np
+
 from flwr.common import (
     FitRes,
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
-from flwr.common.logger import log
-from flwr.server.client_manager import ClientManager
 from flwr.server.client_proxy import ClientProxy
 
-from .aggregate import aggregate
-from .fedavg import FedAvg
+from .fedopt import FedOpt
 
 
 # pylint: disable=line-too-long
-class FedAvgM(FedAvg):
-    """Federated Averaging with Momentum strategy.
+class FedYogi(FedOpt):
+    """FedYogi [Reddi et al., 2020] strategy.
 
-    Implementation based on https://arxiv.org/abs/1909.06335
+    Implementation based on https://arxiv.org/abs/2003.00295v5
 
     Parameters
     ----------
     fraction_fit : float, optional
         Fraction of clients used during training. Defaults to 1.0.
     fraction_evaluate : float, optional
         Fraction of clients used during validation. Defaults to 1.0.
     min_fit_clients : int, optional
         Minimum number of clients used during training. Defaults to 2.
     min_evaluate_clients : int, optional
         Minimum number of clients used during validation. Defaults to 2.
     min_available_clients : int, optional
         Minimum number of total clients in the system. Defaults to 2.
-    evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
+    evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[
+    Tuple[float, Dict[str, Scalar]]]]]
         Optional function used for validation. Defaults to None.
     on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
         Function used to configure training. Defaults to None.
     on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
         Function used to configure validation. Defaults to None.
     accept_failures : bool, optional
         Whether or not accept rounds containing failures. Defaults to True.
-    initial_parameters : Parameters, optional
+    initial_parameters : Parameters
         Initial global model parameters.
-    server_learning_rate: float
-        Server-side learning rate used in server-side optimization.
-        Defaults to 1.0.
-    server_momentum: float
-        Server-side momentum factor used for FedAvgM. Defaults to 0.0.
+    fit_metrics_aggregation_fn : Optional[MetricsAggregationFn]
+        Metrics aggregation function, optional.
+    evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn]
+        Metrics aggregation function, optional.
+    eta : float, optional
+        Server-side learning rate. Defaults to 1e-2.
+    eta_l : float, optional
+        Client-side learning rate. Defaults to 0.0316.
+    beta_1 : float, optional
+        Momentum parameter. Defaults to 0.9.
+    beta_2 : float, optional
+        Second moment parameter. Defaults to 0.99.
+    tau : float, optional
+        Controls the algorithm's degree of adaptability.
+        Defaults to 1e-3.
     """
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes, line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals, line-too-long
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
@@ -87,114 +96,85 @@
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         accept_failures: bool = True,
-        initial_parameters: Optional[Parameters] = None,
+        initial_parameters: Parameters,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
-        server_learning_rate: float = 1.0,
-        server_momentum: float = 0.0,
+        eta: float = 1e-2,
+        eta_l: float = 0.0316,
+        beta_1: float = 0.9,
+        beta_2: float = 0.99,
+        tau: float = 1e-3,
     ) -> None:
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
+            eta=eta,
+            eta_l=eta_l,
+            beta_1=beta_1,
+            beta_2=beta_2,
+            tau=tau,
         )
-        self.server_learning_rate = server_learning_rate
-        self.server_momentum = server_momentum
-        self.server_opt: bool = (self.server_momentum != 0.0) or (
-            self.server_learning_rate != 1.0
-        )
-        self.momentum_vector: Optional[NDArrays] = None
 
     def __repr__(self) -> str:
         """Compute a string representation of the strategy."""
-        rep = f"FedAvgM(accept_failures={self.accept_failures})"
+        rep = f"FedYogi(accept_failures={self.accept_failures})"
         return rep
 
-    def initialize_parameters(
-        self, client_manager: ClientManager
-    ) -> Optional[Parameters]:
-        """Initialize global model parameters."""
-        return self.initial_parameters
-
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
         failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
     ) -> Tuple[Optional[Parameters], Dict[str, Scalar]]:
         """Aggregate fit results using weighted average."""
-        if not results:
-            return None, {}
-        # Do not aggregate if there are failures and failures are not accepted
-        if not self.accept_failures and failures:
+        fedavg_parameters_aggregated, metrics_aggregated = super().aggregate_fit(
+            server_round=server_round, results=results, failures=failures
+        )
+        if fedavg_parameters_aggregated is None:
             return None, {}
-        # Convert results
-        weights_results = [
-            (parameters_to_ndarrays(fit_res.parameters), fit_res.num_examples)
-            for _, fit_res in results
+
+        fedavg_weights_aggregate = parameters_to_ndarrays(fedavg_parameters_aggregated)
+
+        # Yogi
+        delta_t: NDArrays = [
+            x - y for x, y in zip(fedavg_weights_aggregate, self.current_weights)
         ]
 
-        fedavg_result = aggregate(weights_results)
-        # following convention described in
-        # https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
-        if self.server_opt:
-            # You need to initialize the model
-            assert (
-                self.initial_parameters is not None
-            ), "When using server-side optimization, model needs to be initialized."
-            initial_weights = parameters_to_ndarrays(self.initial_parameters)
-
-            # remember that updates are the opposite of gradients
-            pseudo_gradient: NDArrays = [
-                x - y
-                for x, y in zip(
-                    parameters_to_ndarrays(self.initial_parameters), fedavg_result
-                )
-            ]
-            if self.server_momentum > 0.0:
-                if server_round > 1:
-                    assert (
-                        self.momentum_vector
-                    ), "Momentum should have been created on round 1."
-                    self.momentum_vector = [
-                        self.server_momentum * x + y
-                        for x, y in zip(self.momentum_vector, pseudo_gradient)
-                    ]
-                else:
-                    self.momentum_vector = pseudo_gradient
-
-                # No nesterov for now
-                pseudo_gradient = self.momentum_vector
-
-            # SGD
-            fedavg_result = [
-                x - self.server_learning_rate * y
-                for x, y in zip(initial_weights, pseudo_gradient)
-            ]
-            # Update current weights
-            self.initial_parameters = ndarrays_to_parameters(fedavg_result)
+        # m_t
+        if not self.m_t:
+            self.m_t = [np.zeros_like(x) for x in delta_t]
+        self.m_t = [
+            np.multiply(self.beta_1, x) + (1 - self.beta_1) * y
+            for x, y in zip(self.m_t, delta_t)
+        ]
 
-        parameters_aggregated = ndarrays_to_parameters(fedavg_result)
+        # v_t
+        if not self.v_t:
+            self.v_t = [np.zeros_like(x) for x in delta_t]
+        self.v_t = [
+            x - (1.0 - self.beta_2) * np.multiply(y, y) * np.sign(x - np.multiply(y, y))
+            for x, y in zip(self.v_t, delta_t)
+        ]
+
+        new_weights = [
+            x + self.eta * y / (np.sqrt(z) + self.tau)
+            for x, y, z in zip(self.current_weights, self.m_t, self.v_t)
+        ]
 
-        # Aggregate custom metrics if aggregation fn was provided
-        metrics_aggregated = {}
-        if self.fit_metrics_aggregation_fn:
-            fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
-            metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
-        elif server_round == 1:  # Only log this warning once
-            log(WARNING, "No fit_metrics_aggregation_fn provided")
+        self.current_weights = new_weights
 
-        return parameters_aggregated, metrics_aggregated
+        return ndarrays_to_parameters(self.current_weights), metrics_aggregated
```

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedmedian.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedopt.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedprox.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr-1.8.0/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/fedyogi.py` & `flwr-1.8.0/src/py/flwr/server/strategy/krum.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,173 +8,148 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-"""Adaptive Federated Optimization using Yogi (FedYogi) [Reddi et al., 2020] strategy.
+"""Machine Learning with Adversaries: Byzantine Tolerant Gradient Descent.
 
-Paper: arxiv.org/abs/2003.00295
+[Blanchard et al., 2017].
+
+Paper: proceedings.neurips.cc/paper/2017/file/f4b9ec30ad9f68f89b29639786cb62ef-Paper.pdf
 """
 
 
+from logging import WARNING
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
-import numpy as np
-
 from flwr.common import (
     FitRes,
     MetricsAggregationFn,
     NDArrays,
     Parameters,
     Scalar,
     ndarrays_to_parameters,
     parameters_to_ndarrays,
 )
+from flwr.common.logger import log
 from flwr.server.client_proxy import ClientProxy
 
-from .fedopt import FedOpt
+from .aggregate import aggregate_krum
+from .fedavg import FedAvg
 
 
 # pylint: disable=line-too-long
-class FedYogi(FedOpt):
-    """FedYogi [Reddi et al., 2020] strategy.
+class Krum(FedAvg):
+    """Krum [Blanchard et al., 2017] strategy.
 
-    Implementation based on https://arxiv.org/abs/2003.00295v5
+    Implementation based on https://arxiv.org/abs/1703.02757
 
     Parameters
     ----------
     fraction_fit : float, optional
         Fraction of clients used during training. Defaults to 1.0.
     fraction_evaluate : float, optional
         Fraction of clients used during validation. Defaults to 1.0.
     min_fit_clients : int, optional
         Minimum number of clients used during training. Defaults to 2.
     min_evaluate_clients : int, optional
         Minimum number of clients used during validation. Defaults to 2.
     min_available_clients : int, optional
         Minimum number of total clients in the system. Defaults to 2.
-    evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[
-    Tuple[float, Dict[str, Scalar]]]]]
+    num_malicious_clients : int, optional
+        Number of malicious clients in the system. Defaults to 0.
+    num_clients_to_keep : int, optional
+        Number of clients to keep before averaging (MultiKrum). Defaults to 0, in
+        that case classical Krum is applied.
+    evaluate_fn : Optional[Callable[[int, NDArrays, Dict[str, Scalar]], Optional[Tuple[float, Dict[str, Scalar]]]]]
         Optional function used for validation. Defaults to None.
     on_fit_config_fn : Callable[[int], Dict[str, Scalar]], optional
         Function used to configure training. Defaults to None.
     on_evaluate_config_fn : Callable[[int], Dict[str, Scalar]], optional
         Function used to configure validation. Defaults to None.
     accept_failures : bool, optional
         Whether or not accept rounds containing failures. Defaults to True.
-    initial_parameters : Parameters
+    initial_parameters : Parameters, optional
         Initial global model parameters.
-    fit_metrics_aggregation_fn : Optional[MetricsAggregationFn]
-        Metrics aggregation function, optional.
-    evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn]
-        Metrics aggregation function, optional.
-    eta : float, optional
-        Server-side learning rate. Defaults to 1e-2.
-    eta_l : float, optional
-        Client-side learning rate. Defaults to 0.0316.
-    beta_1 : float, optional
-        Momentum parameter. Defaults to 0.9.
-    beta_2 : float, optional
-        Second moment parameter. Defaults to 0.99.
-    tau : float, optional
-        Controls the algorithm's degree of adaptability.
-        Defaults to 1e-3.
     """
 
-    # pylint: disable=too-many-arguments,too-many-instance-attributes,too-many-locals, line-too-long
+    # pylint: disable=too-many-arguments,too-many-instance-attributes
     def __init__(
         self,
         *,
         fraction_fit: float = 1.0,
         fraction_evaluate: float = 1.0,
         min_fit_clients: int = 2,
         min_evaluate_clients: int = 2,
         min_available_clients: int = 2,
+        num_malicious_clients: int = 0,
+        num_clients_to_keep: int = 0,
         evaluate_fn: Optional[
             Callable[
                 [int, NDArrays, Dict[str, Scalar]],
                 Optional[Tuple[float, Dict[str, Scalar]]],
             ]
         ] = None,
         on_fit_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         on_evaluate_config_fn: Optional[Callable[[int], Dict[str, Scalar]]] = None,
         accept_failures: bool = True,
-        initial_parameters: Parameters,
+        initial_parameters: Optional[Parameters] = None,
         fit_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
         evaluate_metrics_aggregation_fn: Optional[MetricsAggregationFn] = None,
-        eta: float = 1e-2,
-        eta_l: float = 0.0316,
-        beta_1: float = 0.9,
-        beta_2: float = 0.99,
-        tau: float = 1e-3,
     ) -> None:
         super().__init__(
             fraction_fit=fraction_fit,
             fraction_evaluate=fraction_evaluate,
             min_fit_clients=min_fit_clients,
             min_evaluate_clients=min_evaluate_clients,
             min_available_clients=min_available_clients,
             evaluate_fn=evaluate_fn,
             on_fit_config_fn=on_fit_config_fn,
             on_evaluate_config_fn=on_evaluate_config_fn,
             accept_failures=accept_failures,
             initial_parameters=initial_parameters,
             fit_metrics_aggregation_fn=fit_metrics_aggregation_fn,
             evaluate_metrics_aggregation_fn=evaluate_metrics_aggregation_fn,
-            eta=eta,
-            eta_l=eta_l,
-            beta_1=beta_1,
-            beta_2=beta_2,
-            tau=tau,
         )
+        self.num_malicious_clients = num_malicious_clients
+        self.num_clients_to_keep = num_clients_to_keep
 
     def __repr__(self) -> str:
         """Compute a string representation of the strategy."""
-        rep = f"FedYogi(accept_failures={self.accept_failures})"
+        rep = f"Krum(accept_failures={self.accept_failures})"
         return rep
 
     def aggregate_fit(
         self,
         server_round: int,
         results: List[Tuple[ClientProxy, FitRes]],
         failures: List[Union[Tuple[ClientProxy, FitRes], BaseException]],
     ) -> Tuple[Optional[Parameters], Dict[str, Scalar]]:
-        """Aggregate fit results using weighted average."""
-        fedavg_parameters_aggregated, metrics_aggregated = super().aggregate_fit(
-            server_round=server_round, results=results, failures=failures
-        )
-        if fedavg_parameters_aggregated is None:
+        """Aggregate fit results using Krum."""
+        if not results:
+            return None, {}
+        # Do not aggregate if there are failures and failures are not accepted
+        if not self.accept_failures and failures:
             return None, {}
 
-        fedavg_weights_aggregate = parameters_to_ndarrays(fedavg_parameters_aggregated)
-
-        # Yogi
-        delta_t: NDArrays = [
-            x - y for x, y in zip(fedavg_weights_aggregate, self.current_weights)
-        ]
-
-        # m_t
-        if not self.m_t:
-            self.m_t = [np.zeros_like(x) for x in delta_t]
-        self.m_t = [
-            np.multiply(self.beta_1, x) + (1 - self.beta_1) * y
-            for x, y in zip(self.m_t, delta_t)
-        ]
-
-        # v_t
-        if not self.v_t:
-            self.v_t = [np.zeros_like(x) for x in delta_t]
-        self.v_t = [
-            x - (1.0 - self.beta_2) * np.multiply(y, y) * np.sign(x - np.multiply(y, y))
-            for x, y in zip(self.v_t, delta_t)
-        ]
-
-        new_weights = [
-            x + self.eta * y / (np.sqrt(z) + self.tau)
-            for x, y, z in zip(self.current_weights, self.m_t, self.v_t)
+        # Convert results
+        weights_results = [
+            (parameters_to_ndarrays(fit_res.parameters), fit_res.num_examples)
+            for _, fit_res in results
         ]
+        parameters_aggregated = ndarrays_to_parameters(
+            aggregate_krum(
+                weights_results, self.num_malicious_clients, self.num_clients_to_keep
+            )
+        )
 
-        self.current_weights = new_weights
+        # Aggregate custom metrics if aggregation fn was provided
+        metrics_aggregated = {}
+        if self.fit_metrics_aggregation_fn:
+            fit_metrics = [(res.num_examples, res.metrics) for _, res in results]
+            metrics_aggregated = self.fit_metrics_aggregation_fn(fit_metrics)
+        elif server_round == 1:  # Only log this warning once
+            log(WARNING, "No fit_metrics_aggregation_fn provided")
 
-        return ndarrays_to_parameters(self.current_weights), metrics_aggregated
+        return parameters_aggregated, metrics_aggregated
```

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/qfedavg.py` & `flwr-1.8.0/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/strategy/strategy.py` & `flwr-1.8.0/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/utils/__init__.py` & `flwr-1.8.0/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/utils/tensorboard.py` & `flwr-1.8.0/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/server/utils/validator.py` & `flwr-1.8.0/src/py/flwr/server/utils/validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,21 +27,29 @@
 
     if tasks_ins_res.task_id != "":
         validation_errors.append("non-empty `task_id`")
 
     if not tasks_ins_res.HasField("task"):
         validation_errors.append("`task` does not set field `task`")
 
-    # Created/delivered/TTL
-    if tasks_ins_res.task.created_at != "":
-        validation_errors.append("`created_at` must be an empty str")
+    # Created/delivered/TTL/Pushed
+    if (
+        tasks_ins_res.task.created_at < 1711497600.0
+    ):  # unix timestamp of 27 March 2024 00h:00m:00s UTC
+        validation_errors.append(
+            "`created_at` must be a float that records the unix timestamp "
+            "in seconds when the message was created."
+        )
     if tasks_ins_res.task.delivered_at != "":
         validation_errors.append("`delivered_at` must be an empty str")
-    if tasks_ins_res.task.ttl != "":
-        validation_errors.append("`ttl` must be an empty str")
+    if tasks_ins_res.task.ttl <= 0:
+        validation_errors.append("`ttl` must be higher than zero")
+    if tasks_ins_res.task.pushed_at < 1711497600.0:
+        # unix timestamp of 27 March 2024 00h:00m:00s UTC
+        validation_errors.append("`pushed_at` is not a recent timestamp")
 
     # TaskIns specific
     if isinstance(tasks_ins_res, TaskIns):
         # Task producer
         if not tasks_ins_res.task.HasField("producer"):
             validation_errors.append("`producer` does not set field `producer`")
         if tasks_ins_res.task.producer.node_id != 0:
@@ -62,16 +70,19 @@
             and tasks_ins_res.task.consumer.node_id == 0
         ):
             validation_errors.append("non-anonymous consumer MUST provide a `node_id`")
 
         # Content check
         if tasks_ins_res.task.task_type == "":
             validation_errors.append("`task_type` MUST be set")
-        if not tasks_ins_res.task.HasField("recordset"):
-            validation_errors.append("`recordset` MUST be set")
+        if not (
+            tasks_ins_res.task.HasField("recordset")
+            ^ tasks_ins_res.task.HasField("error")
+        ):
+            validation_errors.append("Either `recordset` or `error` MUST be set")
 
         # Ancestors
         if len(tasks_ins_res.task.ancestry) != 0:
             validation_errors.append("`ancestry` is not empty")
 
     # TaskRes specific
     if isinstance(tasks_ins_res, TaskRes):
@@ -102,15 +113,18 @@
             and tasks_ins_res.task.consumer.node_id == 0
         ):
             validation_errors.append("non-anonymous consumer MUST provide a `node_id`")
 
         # Content check
         if tasks_ins_res.task.task_type == "":
             validation_errors.append("`task_type` MUST be set")
-        if not tasks_ins_res.task.HasField("recordset"):
-            validation_errors.append("`recordset` MUST be set")
+        if not (
+            tasks_ins_res.task.HasField("recordset")
+            ^ tasks_ins_res.task.HasField("error")
+        ):
+            validation_errors.append("Either `recordset` or `error` MUST be set")
 
         # Ancestors
         if len(tasks_ins_res.task.ancestry) == 0:
             validation_errors.append("`ancestry` is empty")
 
     return validation_errors
```

### Comparing `flwr-1.7.0/src/py/flwr/simulation/__init__.py` & `flwr-1.8.0/src/py/flwr/simulation/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # limitations under the License.
 # ==============================================================================
 """Flower simulation."""
 
 
 import importlib
 
+from flwr.simulation.run_simulation import run_simulation, run_simulation_from_cli
+
 is_ray_installed = importlib.util.find_spec("ray") is not None
 
 if is_ray_installed:
     from flwr.simulation.app import start_simulation
 else:
     RAY_IMPORT_ERROR: str = """Unable to import module `ray`.
 
@@ -30,10 +32,8 @@
 """
 
     def start_simulation(*args, **kwargs):  # type: ignore
         """Log error stating that module `ray` could not be imported."""
         raise ImportError(RAY_IMPORT_ERROR)
 
 
-__all__ = [
-    "start_simulation",
-]
+__all__ = ["start_simulation", "run_simulation_from_cli", "run_simulation"]
```

### Comparing `flwr-1.7.0/src/py/flwr/simulation/app.py` & `flwr-1.8.0/src/py/flwr/simulation/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,21 +24,21 @@
 
 import ray
 from ray.util.scheduling_strategies import NodeAffinitySchedulingStrategy
 
 from flwr.client import ClientFn
 from flwr.common import EventType, event
 from flwr.common.logger import log
-from flwr.server import Server
-from flwr.server.app import ServerConfig, init_defaults, run_fl
 from flwr.server.client_manager import ClientManager
 from flwr.server.history import History
+from flwr.server.server import Server, init_defaults, run_fl
+from flwr.server.server_config import ServerConfig
 from flwr.server.strategy import Strategy
 from flwr.simulation.ray_transport.ray_actor import (
-    DefaultActor,
+    ClientAppActor,
     VirtualClientEngineActor,
     VirtualClientEngineActorPool,
     pool_size_from_resources,
 )
 from flwr.simulation.ray_transport.ray_client_proxy import RayActorClientProxy
 
 INVALID_ARGUMENTS_START_SIMULATION = """
@@ -78,15 +78,15 @@
     client_resources: Optional[Dict[str, float]] = None,
     server: Optional[Server] = None,
     config: Optional[ServerConfig] = None,
     strategy: Optional[Strategy] = None,
     client_manager: Optional[ClientManager] = None,
     ray_init_args: Optional[Dict[str, Any]] = None,
     keep_initialised: Optional[bool] = False,
-    actor_type: Type[VirtualClientEngineActor] = DefaultActor,
+    actor_type: Type[VirtualClientEngineActor] = ClientAppActor,
     actor_kwargs: Optional[Dict[str, Any]] = None,
     actor_scheduling: Union[str, NodeAffinitySchedulingStrategy] = "DEFAULT",
 ) -> History:
     """Start a Ray-based Flower simulation server.
 
     Parameters
     ----------
@@ -134,18 +134,18 @@
         { "ignore_reinit_error": True, "include_dashboard": False }
 
         An empty dictionary can be used (ray_init_args={}) to prevent any
         arguments from being passed to ray.init.
     keep_initialised: Optional[bool] (default: False)
         Set to True to prevent `ray.shutdown()` in case `ray.is_initialized()=True`.
 
-    actor_type: VirtualClientEngineActor (default: DefaultActor)
+    actor_type: VirtualClientEngineActor (default: ClientAppActor)
         Optionally specify the type of actor to use. The actor object, which
         persists throughout the simulation, will be the process in charge of
-        running the clients' jobs (i.e. their `fit()` method).
+        executing a ClientApp wrapping input argument `client_fn`.
 
     actor_kwargs: Optional[Dict[str, Any]] (default: None)
         If you want to create your own Actor classes, you might need to pass
         some input argument. You can use this dictionary for such purpose.
 
     actor_scheduling: Optional[Union[str, NodeAffinitySchedulingStrategy]]
         (default: "DEFAULT")
@@ -215,15 +215,15 @@
         "Flower VCE: Ray initialized with resources: %s",
         cluster_resources,
     )
 
     log(
         INFO,
         "Optimize your simulation with Flower VCE: "
-        "https://flower.dev/docs/framework/how-to-run-simulations.html",
+        "https://flower.ai/docs/framework/how-to-run-simulations.html",
     )
 
     # Log the resources that a single client will be able to use
     if client_resources is None:
         log(
             INFO,
             "No `client_resources` specified. Using minimal resources for clients.",
@@ -333,15 +333,15 @@
             "recover from it. Try launching your simulation with more generous "
             "`client_resources` setting (i.e. it seems %s is "
             "not enough for your run). Use fewer concurrent actors. "
             "\n\t\t - You were running a multi-node simulation and all worker nodes "
             "disconnected. The head node might still be alive but cannot accommodate "
             "any actor with resources: %s."
             "\nTake a look at the Flower simulation examples for guidance "
-            "<https://flower.dev/docs/framework/how-to-run-simulations.html>.",
+            "<https://flower.ai/docs/framework/how-to-run-simulations.html>.",
             client_resources,
             client_resources,
         )
         raise RuntimeError("Simulation crashed.") from ex
 
     finally:
         # Stop time monitoring resources in cluster
```

### Comparing `flwr-1.7.0/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr-1.8.0/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr-1.7.0/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr-1.8.0/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,94 +10,68 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Ray-based Flower Actor and ActorPool implementation."""
 
-
+import asyncio
 import threading
-import traceback
 from abc import ABC
-from logging import ERROR, WARNING
+from logging import DEBUG, ERROR, WARNING
 from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union
 
 import ray
 from ray import ObjectRef
 from ray.util.actor_pool import ActorPool
 
-from flwr import common
-from flwr.client import Client, ClientFn
-from flwr.common.context import Context
+from flwr.client.client_app import ClientApp, ClientAppException, LoadClientAppError
+from flwr.common import Context, Message
 from flwr.common.logger import log
-from flwr.simulation.ray_transport.utils import check_clientfn_returns_client
 
-# All possible returns by a client
-ClientRes = Union[
-    common.GetPropertiesRes, common.GetParametersRes, common.FitRes, common.EvaluateRes
-]
-# A function to be executed by a client to obtain some results
-JobFn = Callable[[Client], ClientRes]
-
-
-class ClientException(Exception):
-    """Raised when client side logic crashes with an exception."""
-
-    def __init__(self, message: str):
-        div = ">" * 7
-        self.message = "\n" + div + "A ClientException occurred." + message
-        super().__init__(self.message)
+ClientAppFn = Callable[[], ClientApp]
 
 
 class VirtualClientEngineActor(ABC):
     """Abstract base class for VirtualClientEngine Actors."""
 
     def terminate(self) -> None:
         """Manually terminate Actor object."""
-        log(WARNING, "Manually terminating %s}", self.__class__.__name__)
+        log(WARNING, "Manually terminating %s", self.__class__.__name__)
         ray.actor.exit_actor()
 
     def run(
         self,
-        client_fn: ClientFn,
-        job_fn: JobFn,
+        client_app_fn: ClientAppFn,
+        message: Message,
         cid: str,
         context: Context,
-    ) -> Tuple[str, ClientRes, Context]:
+    ) -> Tuple[str, Message, Context]:
         """Run a client run."""
-        # Execute tasks and return result
+        # Pass message through ClientApp and return a message
         # return also cid which is needed to ensure results
         # from the pool are correctly assigned to each ClientProxy
         try:
-            # Instantiate client (check 'Client' type is returned)
-            client = check_clientfn_returns_client(client_fn(cid))
-            # Inject context
-            client.set_context(context)
-            # Run client job
-            job_results = job_fn(client)
-            # Retrieve context (potentially updated)
-            updated_context = client.get_context()
+            # Load app
+            app: ClientApp = client_app_fn()
+
+            # Handle task message
+            out_message = app(message=message, context=context)
+
+        except LoadClientAppError as load_ex:
+            raise load_ex
+
         except Exception as ex:
-            client_trace = traceback.format_exc()
-            message = (
-                "\n\tSomething went wrong when running your client run."
-                "\n\tClient "
-                + cid
-                + " crashed when the "
-                + self.__class__.__name__
-                + " was running its run."
-                "\n\tException triggered on the client side: " + client_trace,
-            )
-            raise ClientException(str(message)) from ex
+            raise ClientAppException(str(ex)) from ex
 
-        return cid, job_results, updated_context
+        return cid, out_message, context
 
 
 @ray.remote
-class DefaultActor(VirtualClientEngineActor):
+class ClientAppActor(VirtualClientEngineActor):
     """A Ray Actor class that runs client runs.
 
     Parameters
     ----------
     on_actor_init_fn: Optional[Callable[[], None]] (default: None)
         A function to execute upon actor initialization.
     """
@@ -233,33 +207,33 @@
         your Ray cluster (e.g. you add a new node).
         """
         with self.lock:
             new_actors = [self.create_actor_fn() for _ in range(num_actors)]
             self._idle_actors.extend(new_actors)
             self.num_actors += num_actors
 
-    def submit(self, fn: Any, value: Tuple[ClientFn, JobFn, str, Context]) -> None:
-        """Take idle actor and assign it a client run.
+    def submit(self, fn: Any, value: Tuple[ClientAppFn, Message, str, Context]) -> None:
+        """Take an idle actor and assign it to run a client app and Message.
 
         Submit a job to an actor by first removing it from the list of idle actors, then
-        check if this actor was flagged to be removed from the pool
+        check if this actor was flagged to be removed from the pool.
         """
-        client_fn, job_fn, cid, context = value
+        app_fn, mssg, cid, context = value
         actor = self._idle_actors.pop()
         if self._check_and_remove_actor_from_pool(actor):
-            future = fn(actor, client_fn, job_fn, cid, context)
+            future = fn(actor, app_fn, mssg, cid, context)
             future_key = tuple(future) if isinstance(future, List) else future
             self._future_to_actor[future_key] = (self._next_task_index, actor, cid)
             self._next_task_index += 1
 
             # Update with future
             self._cid_to_future[cid]["future"] = future_key
 
     def submit_client_job(
-        self, actor_fn: Any, job: Tuple[ClientFn, JobFn, str, Context]
+        self, actor_fn: Any, job: Tuple[ClientAppFn, Message, str, Context]
     ) -> None:
         """Submit a job while tracking client ids."""
         _, _, cid, _ = job
 
         # We need to put this behind a lock since .submit() involves
         # removing and adding elements from a dictionary. Which creates
         # issues in multi-threaded settings
@@ -291,25 +265,25 @@
             # With the current ClientProxy<-->ActorPool interaction
             # we should never be hitting this condition.
             log(WARNING, "This shouldn't be happening")
             return False
 
         return self._cid_to_future[cid]["ready"]  # type: ignore
 
-    def _fetch_future_result(self, cid: str) -> Tuple[ClientRes, Context]:
+    def _fetch_future_result(self, cid: str) -> Tuple[Message, Context]:
         """Fetch result and updated context for a VirtualClient from Object Store.
 
         The job submitted by the ClientProxy interfacing with client with cid=cid is
         ready. Here we fetch it from the object store and return.
         """
         try:
             future: ObjectRef[Any] = self._cid_to_future[cid]["future"]  # type: ignore
-            res_cid, res, updated_context = ray.get(
+            res_cid, out_mssg, updated_context = ray.get(
                 future
-            )  # type: (str, ClientRes, Context)
+            )  # type: (str, Message, Context)
         except ray.exceptions.RayActorError as ex:
             log(ERROR, ex)
             if hasattr(ex, "actor_id"):
                 # RayActorError only contains the actor_id attribute
                 # if the actor won't be restarted again.
                 self._flag_actor_for_removal(ex.actor_id)
             raise ex
@@ -318,15 +292,15 @@
         assert res_cid == cid, log(
             ERROR, "The VirtualClient %s got result from client %s", cid, res_cid
         )
 
         # Reset mapping
         self._reset_cid_to_future_dict(cid)
 
-        return res, updated_context
+        return out_mssg, updated_context
 
     def _flag_actor_for_removal(self, actor_id_hex: str) -> None:
         """Flag actor that should be removed from pool."""
         with self.lock:
             self.actor_to_remove.add(actor_id_hex)
             log(WARNING, "Actor(%s) will be remove from pool.", actor_id_hex)
 
@@ -405,21 +379,112 @@
                 else:
                     # The actor doesn't fit in the pool anymore.
                     # Manually terminate the actor
                     actor.terminate.remote()
 
     def get_client_result(
         self, cid: str, timeout: Optional[float]
-    ) -> Tuple[ClientRes, Context]:
+    ) -> Tuple[Message, Context]:
         """Get result from VirtualClient with specific cid."""
         # Loop until all jobs submitted to the pool are completed. Break early
         # if the result for the ClientProxy calling this method is ready
         while self.has_next() and not self._is_future_ready(cid):  # type: ignore
             try:
                 self.process_unordered_future(timeout=timeout)
             except StopIteration:
                 # There are no pending jobs in the pool
                 break
 
         # Fetch result belonging to the VirtualClient calling this method
         # Return both result from tasks and (potentially) updated run context
         return self._fetch_future_result(cid)
+
+
+def init_ray(*args: Any, **kwargs: Any) -> None:
+    """Intialises Ray if not already initialised."""
+    if not ray.is_initialized():
+        ray.init(*args, **kwargs)
+
+
+class BasicActorPool:
+    """A basic actor pool."""
+
+    def __init__(
+        self,
+        actor_type: Type[VirtualClientEngineActor],
+        client_resources: Dict[str, Union[int, float]],
+        actor_kwargs: Dict[str, Any],
+    ):
+        self.client_resources = client_resources
+
+        # Queue of idle actors
+        self.pool: "asyncio.Queue[Type[VirtualClientEngineActor]]" = asyncio.Queue(
+            maxsize=1024
+        )
+        self.num_actors = 0
+
+        # Resolve arguments to pass during actor init
+        actor_args = {} if actor_kwargs is None else actor_kwargs
+
+        # A function that creates an actor
+        self.create_actor_fn = lambda: actor_type.options(  # type: ignore
+            **client_resources
+        ).remote(**actor_args)
+
+        # Figure out how many actors can be created given the cluster resources
+        # and the resources the user indicates each VirtualClient will need
+        self.actors_capacity = pool_size_from_resources(client_resources)
+        self._future_to_actor: Dict[Any, Type[VirtualClientEngineActor]] = {}
+
+    def is_actor_available(self) -> bool:
+        """Return true if there is an idle actor."""
+        return self.pool.qsize() > 0
+
+    async def add_actors_to_pool(self, num_actors: int) -> None:
+        """Add actors to the pool.
+
+        This method may be executed also if new resources are added to your Ray cluster
+        (e.g. you add a new node).
+        """
+        for _ in range(num_actors):
+            await self.pool.put(self.create_actor_fn())  # type: ignore
+        self.num_actors += num_actors
+
+    async def terminate_all_actors(self) -> None:
+        """Terminate actors in pool."""
+        num_terminated = 0
+        while self.pool.qsize():
+            actor = await self.pool.get()
+            actor.terminate.remote()  # type: ignore
+            num_terminated += 1
+
+        log(DEBUG, "Terminated %i actors", num_terminated)
+
+    async def submit(
+        self, actor_fn: Any, job: Tuple[ClientAppFn, Message, str, Context]
+    ) -> Any:
+        """On idle actor, submit job and return future."""
+        # Remove idle actor from pool
+        actor = await self.pool.get()
+        # Submit job to actor
+        app_fn, mssg, cid, context = job
+        future = actor_fn(actor, app_fn, mssg, cid, context)
+        # Keep track of future:actor (so we can fetch the actor upon job completion
+        # and add it back to the pool)
+        self._future_to_actor[future] = actor
+        return future
+
+    async def add_actor_back_to_pool(self, future: Any) -> None:
+        """Ad actor assigned to run future back into the pool."""
+        actor = self._future_to_actor.pop(future)
+        await self.pool.put(actor)
+
+    async def fetch_result_and_return_actor_to_pool(
+        self, future: Any
+    ) -> Tuple[Message, Context]:
+        """Pull result given a future and add actor back to pool."""
+        # Get actor that ran job
+        await self.add_actor_back_to_pool(future)
+        # Retrieve result for object store
+        # Instead of doing ray.get(future) we await it
+        _, out_mssg, updated_context = await future
+        return out_mssg, updated_context
```

### Comparing `flwr-1.7.0/src/py/flwr/simulation/ray_transport/utils.py` & `flwr-1.8.0/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # ==============================================================================
 """Utilities for Actors in the Virtual Client Engine."""
 
 import traceback
 import warnings
 from logging import ERROR
 
-from flwr.client import Client
 from flwr.common.logger import log
 
 try:
     import tensorflow as TF
 except ModuleNotFoundError:
     TF = None
 
@@ -56,29 +55,7 @@
             for gpu in gpus:
                 TF.config.experimental.set_memory_growth(gpu, True)
         except RuntimeError as ex:
             # Memory growth must be set before GPUs have been initialized
             log(ERROR, traceback.format_exc())
             log(ERROR, ex)
             raise ex
-
-
-def check_clientfn_returns_client(client: Client) -> Client:
-    """Warn once that clients returned in `clinet_fn` should be of type Client.
-
-    This is here for backwards compatibility. If a ClientFn is provided returning
-    a different type of client (e.g. NumPyClient) we'll warn the user but convert
-    the client internally to `Client` by calling `.to_client()`.
-    """
-    if not isinstance(client, Client):
-        mssg = (
-            " Ensure your client is of type `flwr.client.Client`. Please convert it"
-            " using the `.to_client()` method before returning it"
-            " in the `client_fn` you pass to `start_simulation`."
-            " We have applied this conversion on your behalf."
-            " Not returning a `Client` might trigger an error in future"
-            " versions of Flower."
-        )
-
-        warnings.warn(mssg, DeprecationWarning, stacklevel=2)
-        client = client.to_client()
-    return client
```

### Comparing `flwr-1.7.0/PKG-INFO` & `flwr-1.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,100 @@
 Metadata-Version: 2.1
 Name: flwr
-Version: 1.7.0
+Version: 1.8.0
 Summary: Flower: A Friendly Federated Learning Framework
-Home-page: https://flower.dev
+Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
-Author-email: hello@flower.dev
+Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Provides-Extra: rest
 Provides-Extra: simulation
-Requires-Dist: cryptography (>=41.0.2,<42.0.0)
+Requires-Dist: cryptography (>=42.0.4,<43.0.0)
 Requires-Dist: grpcio (>=1.60.0,<2.0.0)
 Requires-Dist: iterators (>=0.0.2,<0.0.3)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Requires-Dist: protobuf (>=4.25.2,<5.0.0)
 Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: pydantic (<2.0.0) ; extra == "simulation"
 Requires-Dist: ray (==2.6.3) ; extra == "simulation"
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "rest"
 Requires-Dist: starlette (>=0.31.0,<0.32.0) ; extra == "rest"
+Requires-Dist: tomli (>=2.0.1,<3.0.0)
+Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: uvicorn[standard] (>=0.23.0,<0.24.0) ; extra == "rest"
-Project-URL: Documentation, https://flower.dev
+Project-URL: Documentation, https://flower.ai
 Project-URL: Repository, https://github.com/adap/flower
 Description-Content-Type: text/markdown
 
 # Flower: A Friendly Federated Learning Framework
 
 <p align="center">
-  <a href="https://flower.dev/">
-    <img src="https://flower.dev/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />
+  <a href="https://flower.ai/">
+    <img src="https://flower.ai/_next/image/?url=%2F_next%2Fstatic%2Fmedia%2Fflower_white_border.c2012e70.png&w=640&q=75" width="140px" alt="Flower Website" />
   </a>
 </p>
 <p align="center">
-    <a href="https://flower.dev/">Website</a> |
-    <a href="https://flower.dev/blog">Blog</a> |
-    <a href="https://flower.dev/docs/">Docs</a> |
-    <a href="https://flower.dev/conf/flower-summit-2022">Conference</a> |
-    <a href="https://flower.dev/join-slack">Slack</a>
+    <a href="https://flower.ai/">Website</a> |
+    <a href="https://flower.ai/blog">Blog</a> |
+    <a href="https://flower.ai/docs/">Docs</a> |
+    <a href="https://flower.ai/conf/flower-summit-2022">Conference</a> |
+    <a href="https://flower.ai/join-slack">Slack</a>
     <br /><br />
 </p>
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://github.com/adap/flower/blob/main/LICENSE)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/flower/blob/main/CONTRIBUTING.md)
 ![Build](https://github.com/adap/flower/actions/workflows/framework.yml/badge.svg)
 [![Downloads](https://static.pepy.tech/badge/flwr)](https://pepy.tech/project/flwr)
-[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack)
+[![Slack](https://img.shields.io/badge/Chat-Slack-red)](https://flower.ai/join-slack)
 
 Flower (`flwr`) is a framework for building federated learning systems. The
 design of Flower is based on a few guiding principles:
 
 - **Customizable**: Federated learning systems vary wildly from one use case to
   another. Flower allows for a wide range of different configurations depending
   on the needs of each individual use case.
 
 - **Extendable**: Flower originated from a research project at the University of
   Oxford, so it was built with AI research in mind. Many components can be
   extended and overridden to build new state-of-the-art systems.
 
 - **Framework-agnostic**: Different machine learning frameworks have different
   strengths. Flower can be used with any machine learning framework, for
-  example, [PyTorch](https://pytorch.org), [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [fastai](https://www.fast.ai/), [MLX](https://ml-explore.github.io/mlx/build/html/index.html), [XGBoost](https://xgboost.readthedocs.io/en/stable/), [Pandas](https://pandas.pydata.org/) for federated analytics, or even raw [NumPy](https://numpy.org/)
+  example, [PyTorch](https://pytorch.org), [TensorFlow](https://tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch Lightning](https://pytorchlightning.ai/), [scikit-learn](https://scikit-learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://tensorflow.org/lite/), [MONAI](https://docs.monai.io/en/latest/index.html), [fastai](https://www.fast.ai/), [MLX](https://ml-explore.github.io/mlx/build/html/index.html), [XGBoost](https://xgboost.readthedocs.io/en/stable/), [Pandas](https://pandas.pydata.org/) for federated analytics, or even raw [NumPy](https://numpy.org/)
   for users who enjoy computing gradients by hand.
 
 - **Understandable**: Flower is written with maintainability in mind. The
   community is encouraged to both read and contribute to the codebase.
 
-Meet the Flower community on [flower.dev](https://flower.dev)!
+Meet the Flower community on [flower.ai](https://flower.ai)!
 
 ## Federated Learning Tutorial
 
 Flower's goal is to make federated learning accessible to everyone. This series of tutorials introduces the fundamentals of federated learning and how to implement them in Flower.
 
 0. **What is Federated Learning?**
 
@@ -118,27 +120,27 @@
 
 ## 30-Minute Federated Learning Tutorial
 
 [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/adap/flower/blob/main/examples/flower-in-30-minutes/tutorial.ipynb) (or open the [Jupyter Notebook](https://github.com/adap/flower/blob/main/examples/flower-in-30-minutes/tutorial.ipynb))
 
 ## Documentation
 
-[Flower Docs](https://flower.dev/docs):
+[Flower Docs](https://flower.ai/docs):
 
-- [Installation](https://flower.dev/docs/framework/how-to-install-flower.html)
-- [Quickstart (TensorFlow)](https://flower.dev/docs/framework/tutorial-quickstart-tensorflow.html)
-- [Quickstart (PyTorch)](https://flower.dev/docs/framework/tutorial-quickstart-pytorch.html)
-- [Quickstart (Hugging Face)](https://flower.dev/docs/framework/tutorial-quickstart-huggingface.html)
-- [Quickstart (PyTorch Lightning)](https://flower.dev/docs/framework/tutorial-quickstart-pytorch-lightning.html)
-- [Quickstart (Pandas)](https://flower.dev/docs/framework/tutorial-quickstart-pandas.html)
-- [Quickstart (fastai)](https://flower.dev/docs/framework/tutorial-quickstart-fastai.html)
-- [Quickstart (JAX)](https://flower.dev/docs/framework/tutorial-quickstart-jax.html)
-- [Quickstart (scikit-learn)](https://flower.dev/docs/framework/tutorial-quickstart-scikitlearn.html)
-- [Quickstart (Android [TFLite])](https://flower.dev/docs/framework/tutorial-quickstart-android.html)
-- [Quickstart (iOS [CoreML])](https://flower.dev/docs/framework/tutorial-quickstart-ios.html)
+- [Installation](https://flower.ai/docs/framework/how-to-install-flower.html)
+- [Quickstart (TensorFlow)](https://flower.ai/docs/framework/tutorial-quickstart-tensorflow.html)
+- [Quickstart (PyTorch)](https://flower.ai/docs/framework/tutorial-quickstart-pytorch.html)
+- [Quickstart (Hugging Face)](https://flower.ai/docs/framework/tutorial-quickstart-huggingface.html)
+- [Quickstart (PyTorch Lightning)](https://flower.ai/docs/framework/tutorial-quickstart-pytorch-lightning.html)
+- [Quickstart (Pandas)](https://flower.ai/docs/framework/tutorial-quickstart-pandas.html)
+- [Quickstart (fastai)](https://flower.ai/docs/framework/tutorial-quickstart-fastai.html)
+- [Quickstart (JAX)](https://flower.ai/docs/framework/tutorial-quickstart-jax.html)
+- [Quickstart (scikit-learn)](https://flower.ai/docs/framework/tutorial-quickstart-scikitlearn.html)
+- [Quickstart (Android [TFLite])](https://flower.ai/docs/framework/tutorial-quickstart-android.html)
+- [Quickstart (iOS [CoreML])](https://flower.ai/docs/framework/tutorial-quickstart-ios.html)
 
 ## Flower Baselines
 
 Flower Baselines is a collection of community-contributed projects that reproduce the experiments performed in popular federated learning publications. Researchers can build on Flower Baselines to quickly evaluate new ideas. The Flower community loves contributions! Make your work more visible and enable others to build on it by contributing it as a baseline!
 
 - [DASHA](https://github.com/adap/flower/tree/main/baselines/dasha)
 - [DepthFL](https://github.com/adap/flower/tree/main/baselines/depthfl)
@@ -146,65 +148,68 @@
 - [FedMeta](https://github.com/adap/flower/tree/main/baselines/fedmeta)
 - [FedMLB](https://github.com/adap/flower/tree/main/baselines/fedmlb)
 - [FedPer](https://github.com/adap/flower/tree/main/baselines/fedper)
 - [FedProx](https://github.com/adap/flower/tree/main/baselines/fedprox)
 - [FedNova](https://github.com/adap/flower/tree/main/baselines/fednova)
 - [HeteroFL](https://github.com/adap/flower/tree/main/baselines/heterofl)
 - [FedAvgM](https://github.com/adap/flower/tree/main/baselines/fedavgm)
+- [FedStar](https://github.com/adap/flower/tree/main/baselines/fedstar)
 - [FedWav2vec2](https://github.com/adap/flower/tree/main/baselines/fedwav2vec2)
 - [FjORD](https://github.com/adap/flower/tree/main/baselines/fjord)
 - [MOON](https://github.com/adap/flower/tree/main/baselines/moon)
 - [niid-Bench](https://github.com/adap/flower/tree/main/baselines/niid_bench)
 - [TAMUNA](https://github.com/adap/flower/tree/main/baselines/tamuna)
 - [FedVSSL](https://github.com/adap/flower/tree/main/baselines/fedvssl)
 - [FedXGBoost](https://github.com/adap/flower/tree/main/baselines/hfedxgboost)
 - [FedPara](https://github.com/adap/flower/tree/main/baselines/fedpara)
 - [FedAvg](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/fedavg_mnist)
 - [FedOpt](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/flwr_baselines/publications/adaptive_federated_optimization)
 
-Please refer to the [Flower Baselines Documentation](https://flower.dev/docs/baselines/) for a detailed categorization of baselines and for additional info including:
-* [How to use Flower Baselines](https://flower.dev/docs/baselines/how-to-use-baselines.html)
-* [How to contribute a new Flower Baseline](https://flower.dev/docs/baselines/how-to-contribute-baselines.html)
+Please refer to the [Flower Baselines Documentation](https://flower.ai/docs/baselines/) for a detailed categorization of baselines and for additional info including:
+* [How to use Flower Baselines](https://flower.ai/docs/baselines/how-to-use-baselines.html)
+* [How to contribute a new Flower Baseline](https://flower.ai/docs/baselines/how-to-contribute-baselines.html)
 
 ## Flower Usage Examples
 
 Several code examples show different usage scenarios of Flower (in combination with popular machine learning frameworks such as PyTorch or TensorFlow).
 
 Quickstart examples:
 
 - [Quickstart (TensorFlow)](https://github.com/adap/flower/tree/main/examples/quickstart-tensorflow)
 - [Quickstart (PyTorch)](https://github.com/adap/flower/tree/main/examples/quickstart-pytorch)
 - [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/quickstart-huggingface)
 - [Quickstart (PyTorch Lightning)](https://github.com/adap/flower/tree/main/examples/quickstart-pytorch-lightning)
 - [Quickstart (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart-fastai)
 - [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/quickstart-pandas)
 - [Quickstart (JAX)](https://github.com/adap/flower/tree/main/examples/quickstart-jax)
+- [Quickstart (MONAI)](https://github.com/adap/flower/tree/main/examples/quickstart-monai)
 - [Quickstart (scikit-learn)](https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist)
-- [Quickstart (XGBoost)](https://github.com/adap/flower/tree/main/examples/xgboost-quickstart)
 - [Quickstart (Android [TFLite])](https://github.com/adap/flower/tree/main/examples/android)
 - [Quickstart (iOS [CoreML])](https://github.com/adap/flower/tree/main/examples/ios)
 - [Quickstart (MLX)](https://github.com/adap/flower/tree/main/examples/quickstart-mlx)
 - [Quickstart (XGBoost)](https://github.com/adap/flower/tree/main/examples/xgboost-quickstart)
 
 Other [examples](https://github.com/adap/flower/tree/main/examples):
 
 - [Raspberry Pi & Nvidia Jetson Tutorial](https://github.com/adap/flower/tree/main/examples/embedded-devices)
 - [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/main/examples/pytorch-from-centralized-to-federated)
 - [Vertical FL](https://github.com/adap/flower/tree/main/examples/vertical-fl)
 - [Federated Finetuning of OpenAI's Whisper](https://github.com/adap/flower/tree/main/examples/whisper-federated-finetuning)
-- [Comprehensive XGBoost](https://github.com/adap/flower/tree/main/examples/xgboost-comprehensive)
+- [Federated Finetuning of Large Language Model](https://github.com/adap/flower/tree/main/examples/fedllm-finetune)
+- [Federated Finetuning of a Vision Transformer](https://github.com/adap/flower/tree/main/examples/vit-finetune)
 - [Advanced Flower with TensorFlow/Keras](https://github.com/adap/flower/tree/main/examples/advanced-tensorflow)
 - [Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/advanced-pytorch)
 - Single-Machine Simulation of Federated Learning Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/simulation-pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/simulation-tensorflow))
 - [Comprehensive Flower+XGBoost](https://github.com/adap/flower/tree/main/examples/xgboost-comprehensive)
 - [Flower through Docker Compose and with Grafana dashboard](https://github.com/adap/flower/tree/main/examples/flower-via-docker-compose)
+- [Flower with KaplanMeierFitter from the lifelines library](https://github.com/adap/flower/tree/main/examples/federated-kaplna-meier-fitter)
 
 ## Community
 
-Flower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.
+Flower is built by a wonderful community of researchers and engineers. [Join Slack](https://flower.ai/join-slack) to meet them, [contributions](#contributing-to-flower) are welcome.
 
 <a href="https://github.com/adap/flower/graphs/contributors">
   <img src="https://contrib.rocks/image?repo=adap/flower" />
 </a>
 
 ## Citation
```

#### html2text {}

```diff
@@ -1,73 +1,74 @@
-Metadata-Version: 2.1 Name: flwr Version: 1.7.0 Summary: Flower: A Friendly
-Federated Learning Framework Home-page: https://flower.dev License: Apache-2.0
+Metadata-Version: 2.1 Name: flwr Version: 1.8.0 Summary: Flower: A Friendly
+Federated Learning Framework Home-page: https://flower.ai License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated
 evaluation,machine learning Author: The Flower Authors Author-email:
-hello@flower.dev Requires-Python: >=3.8,<4.0 Classifier: Development Status ::
-5 - Production/Stable Classifier: Intended Audience :: Developers Classifier:
+hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
-Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.12
+Python :: 3.12 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
 Engineering :: Artificial Intelligence Classifier: Topic :: Scientific/
 Engineering :: Mathematics Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Typing :: Typed
 Provides-Extra: rest Provides-Extra: simulation Requires-Dist: cryptography
-(>=41.0.2,<42.0.0) Requires-Dist: grpcio (>=1.60.0,<2.0.0) Requires-Dist:
+(>=42.0.4,<43.0.0) Requires-Dist: grpcio (>=1.60.0,<2.0.0) Requires-Dist:
 iterators (>=0.0.2,<0.0.3) Requires-Dist: numpy (>=1.21.0,<2.0.0) Requires-
 Dist: protobuf (>=4.25.2,<5.0.0) Requires-Dist: pycryptodome (>=3.18.0,<4.0.0)
 Requires-Dist: pydantic (<2.0.0) ; extra == "simulation" Requires-Dist: ray
 (==2.6.3) ; extra == "simulation" Requires-Dist: requests (>=2.31.0,<3.0.0) ;
 extra == "rest" Requires-Dist: starlette (>=0.31.0,<0.32.0) ; extra == "rest"
-Requires-Dist: uvicorn[standard] (>=0.23.0,<0.24.0) ; extra == "rest" Project-
-URL: Documentation, https://flower.dev Project-URL: Repository, https://
-github.com/adap/flower Description-Content-Type: text/markdown # Flower: A
-Friendly Federated Learning Framework
+Requires-Dist: tomli (>=2.0.1,<3.0.0) Requires-Dist: typer[all]
+(>=0.9.0,<0.10.0) Requires-Dist: uvicorn[standard] (>=0.23.0,<0.24.0) ; extra
+== "rest" Project-URL: Documentation, https://flower.ai Project-URL:
+Repository, https://github.com/adap/flower Description-Content-Type: text/
+markdown # Flower: A Friendly Federated Learning Framework
                                _[_F_l_o_w_e_r_ _W_e_b_s_i_t_e_]
                   _W_e_b_s_i_t_e | _B_l_o_g | _D_o_c_s | _C_o_n_f_e_r_e_n_c_e | _S_l_a_c_k
 
 [![GitHub license](https://img.shields.io/github/license/adap/flower)](https://
 github.com/adap/flower/blob/main/LICENSE) [![PRs Welcome](https://
 img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/adap/
 flower/blob/main/CONTRIBUTING.md) ![Build](https://github.com/adap/flower/
 actions/workflows/framework.yml/badge.svg) [![Downloads](https://
 static.pepy.tech/badge/flwr)](https://pepy.tech/project/flwr) [![Slack](https:/
-/img.shields.io/badge/Chat-Slack-red)](https://flower.dev/join-slack) Flower
+/img.shields.io/badge/Chat-Slack-red)](https://flower.ai/join-slack) Flower
 (`flwr`) is a framework for building federated learning systems. The design of
 Flower is based on a few guiding principles: - **Customizable**: Federated
 learning systems vary wildly from one use case to another. Flower allows for a
 wide range of different configurations depending on the needs of each
 individual use case. - **Extendable**: Flower originated from a research
 project at the University of Oxford, so it was built with AI research in mind.
 Many components can be extended and overridden to build new state-of-the-art
 systems. - **Framework-agnostic**: Different machine learning frameworks have
 different strengths. Flower can be used with any machine learning framework,
 for example, [PyTorch](https://pytorch.org), [TensorFlow](https://
 tensorflow.org), [Hugging Face Transformers](https://huggingface.co/), [PyTorch
 Lightning](https://pytorchlightning.ai/), [scikit-learn](https://scikit-
 learn.org/), [JAX](https://jax.readthedocs.io/), [TFLite](https://
-tensorflow.org/lite/), [fastai](https://www.fast.ai/), [MLX](https://ml-
-explore.github.io/mlx/build/html/index.html), [XGBoost](https://
-xgboost.readthedocs.io/en/stable/), [Pandas](https://pandas.pydata.org/) for
-federated analytics, or even raw [NumPy](https://numpy.org/) for users who
-enjoy computing gradients by hand. - **Understandable**: Flower is written with
-maintainability in mind. The community is encouraged to both read and
-contribute to the codebase. Meet the Flower community on [flower.dev](https://
-flower.dev)! ## Federated Learning Tutorial Flower's goal is to make federated
-learning accessible to everyone. This series of tutorials introduces the
-fundamentals of federated learning and how to implement them in Flower. 0.
-**What is Federated Learning?** [![Open in Colab](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
+tensorflow.org/lite/), [MONAI](https://docs.monai.io/en/latest/index.html),
+[fastai](https://www.fast.ai/), [MLX](https://ml-explore.github.io/mlx/build/
+html/index.html), [XGBoost](https://xgboost.readthedocs.io/en/stable/),
+[Pandas](https://pandas.pydata.org/) for federated analytics, or even raw
+[NumPy](https://numpy.org/) for users who enjoy computing gradients by hand. -
+**Understandable**: Flower is written with maintainability in mind. The
+community is encouraged to both read and contribute to the codebase. Meet the
+Flower community on [flower.ai](https://flower.ai)! ## Federated Learning
+Tutorial Flower's goal is to make federated learning accessible to everyone.
+This series of tutorials introduces the fundamentals of federated learning and
+how to implement them in Flower. 0. **What is Federated Learning?** [![Open in
+Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial-
 series-what-is-federated-learning.ipynb) (or open the [Jupyter Notebook](https:
 //github.com/adap/flower/blob/main/doc/source/tutorial-series-what-is-
 federated-learning.ipynb)) 1. **An Introduction to Federated Learning** [![Open
 in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/github/adap/flower/blob/main/doc/source/tutorial-
 series-get-started-with-flower-pytorch.ipynb) (or open the [Jupyter Notebook]
@@ -91,102 +92,106 @@
 tutorial-series-customize-the-client-pytorch.ipynb)) Stay tuned, more tutorials
 are coming soon. Topics include **Privacy and Security in Federated Learning**,
 and **Scaling Federated Learning**. ## 30-Minute Federated Learning Tutorial [!
 [Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)]
 (https://colab.research.google.com/github/adap/flower/blob/main/examples/
 flower-in-30-minutes/tutorial.ipynb) (or open the [Jupyter Notebook](https://
 github.com/adap/flower/blob/main/examples/flower-in-30-minutes/tutorial.ipynb))
-## Documentation [Flower Docs](https://flower.dev/docs): - [Installation]
-(https://flower.dev/docs/framework/how-to-install-flower.html) - [Quickstart
-(TensorFlow)](https://flower.dev/docs/framework/tutorial-quickstart-
-tensorflow.html) - [Quickstart (PyTorch)](https://flower.dev/docs/framework/
+## Documentation [Flower Docs](https://flower.ai/docs): - [Installation](https:
+//flower.ai/docs/framework/how-to-install-flower.html) - [Quickstart
+(TensorFlow)](https://flower.ai/docs/framework/tutorial-quickstart-
+tensorflow.html) - [Quickstart (PyTorch)](https://flower.ai/docs/framework/
 tutorial-quickstart-pytorch.html) - [Quickstart (Hugging Face)](https://
-flower.dev/docs/framework/tutorial-quickstart-huggingface.html) - [Quickstart
-(PyTorch Lightning)](https://flower.dev/docs/framework/tutorial-quickstart-
-pytorch-lightning.html) - [Quickstart (Pandas)](https://flower.dev/docs/
+flower.ai/docs/framework/tutorial-quickstart-huggingface.html) - [Quickstart
+(PyTorch Lightning)](https://flower.ai/docs/framework/tutorial-quickstart-
+pytorch-lightning.html) - [Quickstart (Pandas)](https://flower.ai/docs/
 framework/tutorial-quickstart-pandas.html) - [Quickstart (fastai)](https://
-flower.dev/docs/framework/tutorial-quickstart-fastai.html) - [Quickstart (JAX)]
-(https://flower.dev/docs/framework/tutorial-quickstart-jax.html) - [Quickstart
-(scikit-learn)](https://flower.dev/docs/framework/tutorial-quickstart-
-scikitlearn.html) - [Quickstart (Android [TFLite])](https://flower.dev/docs/
+flower.ai/docs/framework/tutorial-quickstart-fastai.html) - [Quickstart (JAX)]
+(https://flower.ai/docs/framework/tutorial-quickstart-jax.html) - [Quickstart
+(scikit-learn)](https://flower.ai/docs/framework/tutorial-quickstart-
+scikitlearn.html) - [Quickstart (Android [TFLite])](https://flower.ai/docs/
 framework/tutorial-quickstart-android.html) - [Quickstart (iOS [CoreML])]
-(https://flower.dev/docs/framework/tutorial-quickstart-ios.html) ## Flower
+(https://flower.ai/docs/framework/tutorial-quickstart-ios.html) ## Flower
 Baselines Flower Baselines is a collection of community-contributed projects
 that reproduce the experiments performed in popular federated learning
 publications. Researchers can build on Flower Baselines to quickly evaluate new
 ideas. The Flower community loves contributions! Make your work more visible
 and enable others to build on it by contributing it as a baseline! - [DASHA]
 (https://github.com/adap/flower/tree/main/baselines/dasha) - [DepthFL](https://
 github.com/adap/flower/tree/main/baselines/depthfl) - [FedBN](https://
 github.com/adap/flower/tree/main/baselines/fedbn) - [FedMeta](https://
 github.com/adap/flower/tree/main/baselines/fedmeta) - [FedMLB](https://
 github.com/adap/flower/tree/main/baselines/fedmlb) - [FedPer](https://
 github.com/adap/flower/tree/main/baselines/fedper) - [FedProx](https://
 github.com/adap/flower/tree/main/baselines/fedprox) - [FedNova](https://
 github.com/adap/flower/tree/main/baselines/fednova) - [HeteroFL](https://
 github.com/adap/flower/tree/main/baselines/heterofl) - [FedAvgM](https://
-github.com/adap/flower/tree/main/baselines/fedavgm) - [FedWav2vec2](https://
+github.com/adap/flower/tree/main/baselines/fedavgm) - [FedStar](https://
+github.com/adap/flower/tree/main/baselines/fedstar) - [FedWav2vec2](https://
 github.com/adap/flower/tree/main/baselines/fedwav2vec2) - [FjORD](https://
 github.com/adap/flower/tree/main/baselines/fjord) - [MOON](https://github.com/
 adap/flower/tree/main/baselines/moon) - [niid-Bench](https://github.com/adap/
 flower/tree/main/baselines/niid_bench) - [TAMUNA](https://github.com/adap/
 flower/tree/main/baselines/tamuna) - [FedVSSL](https://github.com/adap/flower/
 tree/main/baselines/fedvssl) - [FedXGBoost](https://github.com/adap/flower/
 tree/main/baselines/hfedxgboost) - [FedPara](https://github.com/adap/flower/
 tree/main/baselines/fedpara) - [FedAvg](https://github.com/adap/flower/tree/
 main/baselines/flwr_baselines/flwr_baselines/publications/fedavg_mnist) -
 [FedOpt](https://github.com/adap/flower/tree/main/baselines/flwr_baselines/
 flwr_baselines/publications/adaptive_federated_optimization) Please refer to
-the [Flower Baselines Documentation](https://flower.dev/docs/baselines/) for a
+the [Flower Baselines Documentation](https://flower.ai/docs/baselines/) for a
 detailed categorization of baselines and for additional info including: * [How
-to use Flower Baselines](https://flower.dev/docs/baselines/how-to-use-
-baselines.html) * [How to contribute a new Flower Baseline](https://flower.dev/
+to use Flower Baselines](https://flower.ai/docs/baselines/how-to-use-
+baselines.html) * [How to contribute a new Flower Baseline](https://flower.ai/
 docs/baselines/how-to-contribute-baselines.html) ## Flower Usage Examples
 Several code examples show different usage scenarios of Flower (in combination
 with popular machine learning frameworks such as PyTorch or TensorFlow).
 Quickstart examples: - [Quickstart (TensorFlow)](https://github.com/adap/
 flower/tree/main/examples/quickstart-tensorflow) - [Quickstart (PyTorch)]
 (https://github.com/adap/flower/tree/main/examples/quickstart-pytorch) -
 [Quickstart (Hugging Face)](https://github.com/adap/flower/tree/main/examples/
 quickstart-huggingface) - [Quickstart (PyTorch Lightning)](https://github.com/
 adap/flower/tree/main/examples/quickstart-pytorch-lightning) - [Quickstart
 (fastai)](https://github.com/adap/flower/tree/main/examples/quickstart-fastai)
 - [Quickstart (Pandas)](https://github.com/adap/flower/tree/main/examples/
 quickstart-pandas) - [Quickstart (JAX)](https://github.com/adap/flower/tree/
-main/examples/quickstart-jax) - [Quickstart (scikit-learn)](https://github.com/
-adap/flower/tree/main/examples/sklearn-logreg-mnist) - [Quickstart (XGBoost)]
-(https://github.com/adap/flower/tree/main/examples/xgboost-quickstart) -
+main/examples/quickstart-jax) - [Quickstart (MONAI)](https://github.com/adap/
+flower/tree/main/examples/quickstart-monai) - [Quickstart (scikit-learn)]
+(https://github.com/adap/flower/tree/main/examples/sklearn-logreg-mnist) -
 [Quickstart (Android [TFLite])](https://github.com/adap/flower/tree/main/
 examples/android) - [Quickstart (iOS [CoreML])](https://github.com/adap/flower/
 tree/main/examples/ios) - [Quickstart (MLX)](https://github.com/adap/flower/
 tree/main/examples/quickstart-mlx) - [Quickstart (XGBoost)](https://github.com/
 adap/flower/tree/main/examples/xgboost-quickstart) Other [examples](https://
 github.com/adap/flower/tree/main/examples): - [Raspberry Pi & Nvidia Jetson
 Tutorial](https://github.com/adap/flower/tree/main/examples/embedded-devices) -
 [PyTorch: From Centralized to Federated](https://github.com/adap/flower/tree/
 main/examples/pytorch-from-centralized-to-federated) - [Vertical FL](https://
 github.com/adap/flower/tree/main/examples/vertical-fl) - [Federated Finetuning
 of OpenAI's Whisper](https://github.com/adap/flower/tree/main/examples/whisper-
-federated-finetuning) - [Comprehensive XGBoost](https://github.com/adap/flower/
-tree/main/examples/xgboost-comprehensive) - [Advanced Flower with TensorFlow/
-Keras](https://github.com/adap/flower/tree/main/examples/advanced-tensorflow) -
-[Advanced Flower with PyTorch](https://github.com/adap/flower/tree/main/
-examples/advanced-pytorch) - Single-Machine Simulation of Federated Learning
-Systems ([PyTorch](https://github.com/adap/flower/tree/main/examples/
-simulation-pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/
-examples/simulation-tensorflow)) - [Comprehensive Flower+XGBoost](https://
-github.com/adap/flower/tree/main/examples/xgboost-comprehensive) - [Flower
-through Docker Compose and with Grafana dashboard](https://github.com/adap/
-flower/tree/main/examples/flower-via-docker-compose) ## Community Flower is
-built by a wonderful community of researchers and engineers. [Join Slack]
-(https://flower.dev/join-slack) to meet them, [contributions](#contributing-to-
-flower) are welcome. _[_h_t_t_p_s_:_/_/_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_a_d_a_p_/_f_l_o_w_e_r_]## Citation
-If you publish work that uses Flower, please cite Flower as follows: ```bibtex
-@article{beutel2020flower, title={Flower: A Friendly Federated Learning
-Research Framework}, author={Beutel, Daniel J and Topal, Taner and Mathur,
-Akhil and Qiu, Xinchi and Fernandez-Marques, Javier and Gao, Yan and Sani,
-Lorenzo and Kwing, Hei Li and Parcollet, Titouan and GusmÃ£o, Pedro PB de and
-Lane, Nicholas D}, journal={arXiv preprint arXiv:2007.14390}, year={2020} } ```
-Please also consider adding your publication to the list of Flower-based
-publications in the docs, just open a Pull Request. ## Contributing to Flower
-We welcome contributions. Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get
-started!
+federated-finetuning) - [Federated Finetuning of Large Language Model](https://
+github.com/adap/flower/tree/main/examples/fedllm-finetune) - [Federated
+Finetuning of a Vision Transformer](https://github.com/adap/flower/tree/main/
+examples/vit-finetune) - [Advanced Flower with TensorFlow/Keras](https://
+github.com/adap/flower/tree/main/examples/advanced-tensorflow) - [Advanced
+Flower with PyTorch](https://github.com/adap/flower/tree/main/examples/
+advanced-pytorch) - Single-Machine Simulation of Federated Learning Systems (
+[PyTorch](https://github.com/adap/flower/tree/main/examples/simulation-
+pytorch)) ([Tensorflow](https://github.com/adap/flower/tree/main/examples/
+simulation-tensorflow)) - [Comprehensive Flower+XGBoost](https://github.com/
+adap/flower/tree/main/examples/xgboost-comprehensive) - [Flower through Docker
+Compose and with Grafana dashboard](https://github.com/adap/flower/tree/main/
+examples/flower-via-docker-compose) - [Flower with KaplanMeierFitter from the
+lifelines library](https://github.com/adap/flower/tree/main/examples/federated-
+kaplna-meier-fitter) ## Community Flower is built by a wonderful community of
+researchers and engineers. [Join Slack](https://flower.ai/join-slack) to meet
+them, [contributions](#contributing-to-flower) are welcome. _[_h_t_t_p_s_:_/_/
+_c_o_n_t_r_i_b_._r_o_c_k_s_/_i_m_a_g_e_?_r_e_p_o_=_a_d_a_p_/_f_l_o_w_e_r_]## Citation If you publish work that uses
+Flower, please cite Flower as follows: ```bibtex @article{beutel2020flower,
+title={Flower: A Friendly Federated Learning Research Framework}, author=
+{Beutel, Daniel J and Topal, Taner and Mathur, Akhil and Qiu, Xinchi and
+Fernandez-Marques, Javier and Gao, Yan and Sani, Lorenzo and Kwing, Hei Li and
+Parcollet, Titouan and GusmÃ£o, Pedro PB de and Lane, Nicholas D}, journal=
+{arXiv preprint arXiv:2007.14390}, year={2020} } ``` Please also consider
+adding your publication to the list of Flower-based publications in the docs,
+just open a Pull Request. ## Contributing to Flower We welcome contributions.
+Please see [CONTRIBUTING.md](CONTRIBUTING.md) to get started!
```

