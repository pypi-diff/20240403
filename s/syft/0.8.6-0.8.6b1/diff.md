# Comparing `tmp/syft-0.8.6.tar.gz` & `tmp/syft-0.8.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.6.tar", last modified: Wed Apr  3 12:16:58 2024, max compression
+gzip compressed data, was "syft-0.8.6b1.tar", last modified: Fri Mar 22 16:28:17 2024, max compression
```

## Comparing `syft-0.8.6.tar` & `syft-0.8.6b1.tar`

### file list

```diff
@@ -1,311 +1,311 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.312889 syft-0.8.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-04-03 12:13:33.000000 syft-0.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-03 12:13:33.000000 syft-0.8.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23099 2024-04-03 12:16:58.312889 syft-0.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18678 2024-04-03 12:14:48.000000 syft-0.8.6/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-03 12:13:33.000000 syft-0.8.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 12:13:33.000000 syft-0.8.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-03 12:16:58.316889 syft-0.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 12:13:33.000000 syft-0.8.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.256889 syft-0.8.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.260889 syft-0.8.6/src/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6305 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.264889 syft-0.8.6/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.264889 syft-0.8.6/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36986 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46083 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/domain_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/enclave_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/gateway_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-04-03 12:16:00.000000 syft-0.8.6/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/syncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.268889 syft-0.8.6/src/syft/custom_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/builder_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/builder_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/builder_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/runner_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/custom_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.268889 syft-0.8.6/src/syft/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/exceptions/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.268889 syft-0.8.6/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.272889 syft-0.8.6/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.272889 syft-0.8.6/src/syft/img/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/img/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.272889 syft-0.8.6/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/enclave.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    60417 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.272889 syft-0.8.6/src/syft/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)    24381 2024-04-03 12:16:00.000000 syft-0.8.6/src/syft/protocol/data_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 12:14:48.000000 syft-0.8.6/src/syft/protocol/protocol_version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.276889 syft-0.8.6/src/syft/protocol/releases/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/protocol/releases/0.8.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/protocol/releases/0.8.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/protocol/releases/0.8.4.json
--rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/protocol/releases/0.8.6.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.276889 syft-0.8.6/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.276889 syft-0.8.6/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.280889 syft-0.8.6/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    71240 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    37785 2024-04-03 12:16:00.000000 syft-0.8.6/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.280889 syft-0.8.6/src/syft/service/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/blob_storage/remote_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/blob_storage/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.284889 syft-0.8.6/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code/status_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-04-03 12:16:00.000000 syft-0.8.6/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    24350 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.284889 syft-0.8.6/src/syft/service/code_history/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code_history/code_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.284889 syft-0.8.6/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.284889 syft-0.8.6/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28883 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.284889 syft-0.8.6/src/syft/service/enclave/
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.284889 syft-0.8.6/src/syft/service/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/job/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22622 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/job/job_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.288889 syft-0.8.6/src/syft/service/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/log/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/log/log_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.288889 syft-0.8.6/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/metadata/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.288889 syft-0.8.6/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.288889 syft-0.8.6/src/syft/service/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notification/email_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notification/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.288889 syft-0.8.6/src/syft/service/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notifier/notifier_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notifier/notifier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notifier/notifier_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/notifier/smtp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.288889 syft-0.8.6/src/syft/service/object_search/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/object_search/migration_state_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/object_search/object_migration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.288889 syft-0.8.6/src/syft/service/output/
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/output/output_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.292889 syft-0.8.6/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27196 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.292889 syft-0.8.6/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-04-03 12:16:00.000000 syft-0.8.6/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.292889 syft-0.8.6/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/queue/queue_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.292889 syft-0.8.6/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49952 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.292889 syft-0.8.6/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/settings/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.296889 syft-0.8.6/src/syft/service/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29637 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/sync/diff_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/sync/sync_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/sync/sync_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/sync/sync_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.296889 syft-0.8.6/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20702 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.296889 syft-0.8.6/src/syft/service/veilid/
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/veilid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/veilid/veilid_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/veilid/veilid_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.300889 syft-0.8.6/src/syft/service/worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/image_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/image_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/image_registry_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/image_registry_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker_image_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker_image_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    25667 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker_pool_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker_pool_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/service/worker/worker_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/stable_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.300889 syft-0.8.6/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.300889 syft-0.8.6/src/syft/store/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25674 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-04-03 12:16:00.000000 syft-0.8.6/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31590 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-04-03 12:16:00.000000 syft-0.8.6/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.304889 syft-0.8.6/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/cache_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/dicttuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/syft_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    36794 2024-04-03 12:16:00.000000 syft-0.8.6/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/syncable_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.308889 syft-0.8.6/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/_std_stream_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.308889 syft-0.8.6/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    28420 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24531 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-03 12:13:33.000000 syft-0.8.6/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:16:58.308889 syft-0.8.6/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23099 2024-04-03 12:16:58.000000 syft-0.8.6/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-04-03 12:16:58.000000 syft-0.8.6/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:16:58.000000 syft-0.8.6/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 12:16:58.000000 syft-0.8.6/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:14:12.000000 syft-0.8.6/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-03 12:16:58.000000 syft-0.8.6/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 12:16:58.000000 syft-0.8.6/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.068658 syft-0.8.6b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-03-22 16:25:00.000000 syft-0.8.6b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-22 16:25:00.000000 syft-0.8.6b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-03-22 16:28:17.068658 syft-0.8.6b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-03-22 16:26:03.000000 syft-0.8.6b1/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17399 2024-03-22 16:25:00.000000 syft-0.8.6b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-22 16:25:00.000000 syft-0.8.6b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-22 16:28:17.072658 syft-0.8.6b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-22 16:25:00.000000 syft-0.8.6b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.004657 syft-0.8.6b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.012657 syft-0.8.6b1/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-22 16:25:31.000000 syft-0.8.6b1/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-03-22 16:25:31.000000 syft-0.8.6b1/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.016657 syft-0.8.6b1/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.016657 syft-0.8.6b1/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36986 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46083 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/domain_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/enclave_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/gateway_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-03-22 16:27:15.000000 syft-0.8.6b1/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/syncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/custom_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/runner_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60531 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)    22541 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/protocol/data_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/protocol_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/protocol/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-03-22 16:27:36.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.028658 syft-0.8.6b1/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.028658 syft-0.8.6b1/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.032657 syft-0.8.6b1/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71240 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37785 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.032657 syft-0.8.6b1/src/syft/service/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/remote_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/status_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24350 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/code_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28883 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/enclave/
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22622 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/job_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/email_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/smtp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/object_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/object_search/migration_state_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/object_search/object_migration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/output/output_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27196 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49952 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29637 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/diff_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.052658 syft-0.8.6b1/src/syft/service/veilid/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/veilid_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/veilid_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.052658 syft-0.8.6b1/src/syft/service/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25667 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/stable_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.056658 syft-0.8.6b1/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.056658 syft-0.8.6b1/src/syft/store/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25674 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31590 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.060658 syft-0.8.6b1/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/cache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/dicttuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syft_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37205 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syncable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/_std_stream_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    28420 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24446 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-03-22 16:28:17.000000 syft-0.8.6b1/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:25:32.000000 syft-0.8.6b1/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.6/LICENSE` & `syft-0.8.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/PKG-INFO` & `syft-0.8.6b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.6
+Version: 0.8.6b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -120,30 +120,30 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.6,<0.8.7")
+sy.requires(">=0.8.5,<0.8.6")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.6,<0.8.7")
+sy.requires(">=0.8.5,<0.8.6")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
 
@@ -233,20 +233,19 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
+`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
 
 Deprecated:
 
-- `0.8.5-post.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5-post.2/notebooks/api/0.8">API</a>
 - `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
```

### Comparing `syft-0.8.6/PYPI.md` & `syft-0.8.6b1/PYPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.6,<0.8.7")
+sy.requires(">=0.8.5,<0.8.6")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.6,<0.8.7")
+sy.requires(">=0.8.5,<0.8.6")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
 
@@ -129,20 +129,19 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
+`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
 
 Deprecated:
 
-- `0.8.5-post.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5-post.2/notebooks/api/0.8">API</a>
 - `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-_o_n_%_2_0_s_l_a_c_k_-
 _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_m_d_b_o_o_k_]
 
 [Syft Logo]Perform data science on `data` that remains in `someone else's`
 server # Quickstart â `Linux` â `macOS` â `Windows` â `Docker` â
 `Podman` â `Kubernetes` ## Install Client ```bash $ pip install -U syft
 [data_science] ``` ## Launch Server ```python # from Jupyter / Python import
-syft as sy sy.requires(">=0.8.6,<0.8.7") node = sy.orchestra.launch(name="my-
+syft as sy sy.requires(">=0.8.5,<0.8.6") node = sy.orchestra.launch(name="my-
 domain", port=8080, dev_mode=True, reset=True) ``` ```bash # or from the
 command line $ syft launch --name=my-domain --port=8080 --reset=True Starting
 syft-node server on 0.0.0.0:8080 ``` ## Launch Client ```python import syft as
-sy sy.requires(">=0.8.6,<0.8.7") domain_client = sy.login(port=8080,
+sy sy.requires(">=0.8.5,<0.8.6") domain_client = sy.login(port=8080,
 email="info@openmined.org", password="changethis") ``` ## PySyft in 10 minutes
 ð _A_P_I_ _E_x_a_m_p_l_e_ _N_o_t_e_b_o_o_k_s - _0_0_-_l_o_a_d_-_d_a_t_a_._i_p_y_n_b - _0_1_-_s_u_b_m_i_t_-_c_o_d_e_._i_p_y_n_b - _0_2_-
 _r_e_v_i_e_w_-_c_o_d_e_-_a_n_d_-_a_p_p_r_o_v_e_._i_p_y_n_b - _0_3_-_d_a_t_a_-_s_c_i_e_n_t_i_s_t_-_d_o_w_n_l_o_a_d_-_r_e_s_u_l_t_._i_p_y_n_b - _0_4_-
 _j_a_x_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-_r_e_q_u_e_s_t_s_._i_p_y_n_b -
 _0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b - _0_9_-_b_l_o_b_-
 _s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-_k_8_s_._i_p_y_n_b ##
 Deploy Kubernetes Helm Chart **Note**: Assuming we have a Kubernetes cluster
@@ -41,45 +41,44 @@
 `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where
 `private data` lives ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k #
 Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run: `pip
 install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires
 ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires: ð `python
 3.10 - 3.12` - Run: `pip install -U syft` - PyGrid Requires: ð³ `docker`,
 ð¦¦ `podman` or â¸ï¸ `kubernetes` - Run: `hagrid launch ...` # Versions
-`0.9.0` - Coming soon... `0.8.7` (Beta) - `dev` branch ðð½ _A_P_I - Coming
-soon... `0.8.6` (Stable) - _A_P_I Deprecated: - `0.8.5-post.2` - _A_P_I - `0.8.4` -
-_A_P_I - `0.8.3` - _A_P_I - `0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` -
-_C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d - `0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix -
-`0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
-match them up where possible. We release weekly betas which can be used in each
-context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
-... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
-`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
-version of `hagrid` is usually the best. # What is Syft? [Syft]`Syft` is
-OpenMined's `open source` stack that provides `secure` and `private` Data
-Science in Python. Syft decouples `private data` from model training, using
-techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
-federated-learning-collaborative.html), [Differential Privacy](https://
-en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
-//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
-like interface and integration with `Deep Learning` frameworks, so that you as
-a `Data Scientist` can maintain your current workflow while using these new
-`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
-`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
-limits` set by the `data owner`, get `answers` to those `questions`, all
-without obtaining a `copy` of the data itself. We call this process `Remote
-Data Science`. It means in a wide variety of `domains` across society, the
-current `risks` of sharing information (`copying` data) with someone such as,
-privacy invasion, IP theft and blackmail will no longer prevent the vast
-`benefits` such as innovation, insights and scientific discovery which secure
-access will provide. No more cold calls to get `access` to a dataset. No more
-weeks of `wait times` to get a `result` on your `query`. It also means `1000x
-more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Terminology
+`0.9.0` - Coming soon... `0.8.6` (Beta) - `dev` branch ðð½ _A_P_I - Coming
+soon... `0.8.5` (Stable) - _A_P_I Deprecated: - `0.8.4` - _A_P_I - `0.8.3` - _A_P_I -
+`0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` - _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d -
+`0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix - `0.2.0` - `0.5.0` PySyft
+and PyGrid use the same `version` and its best to match them up where possible.
+We release weekly betas which can be used in each context: PySyft (Stable):
+`pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest` PySyft
+(Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ... tag=beta`
+HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
+the best. # What is Syft? [Syft]`Syft` is OpenMined's `open source` stack that
+provides `secure` and `private` Data Science in Python. Syft decouples `private
+data` from model training, using techniques like [Federated Learning](https://
+ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential
+Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted
+Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is
+done with a `numpy`-like interface and integration with `Deep Learning`
+frameworks, so that you as a `Data Scientist` can maintain your current
+workflow while using these new `privacy-enhancing techniques`. ### Why should I
+use Syft? `Syft` allows a `Data Scientist` to ask `questions` about a `dataset`
+and, within `privacy limits` set by the `data owner`, get `answers` to those
+`questions`, all without obtaining a `copy` of the data itself. We call this
+process `Remote Data Science`. It means in a wide variety of `domains` across
+society, the current `risks` of sharing information (`copying` data) with
+someone such as, privacy invasion, IP theft and blackmail will no longer
+prevent the vast `benefits` such as innovation, insights and scientific
+discovery which secure access will provide. No more cold calls to get `access`
+to a dataset. No more weeks of `wait times` to get a `result` on your `query`.
+It also means `1000x more data` in every domain. PySyft opens the doors to a
+streamlined Data Scientist `workflow`, all with the individual's `privacy` at
+its heart. # Terminology
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |                  [[IImmaaggee]]             |                 [[IImmaaggee]]              |
 |_ _ _ _ _ _ _ _ _?ð_?_?_?¨_?ð_?_?_?»_?â_?_?_?ð_?_?_?¼_ _DD_aa_tt_aa_ _OO_ww_nn_ee_rr_ss_ _ _ _|_ _ _ _ _ _?ð_?_?_?©_?ð_?_?_?½_?â_?_?_?ð_?_?_?¬_ _DD_aa_tt_aa_ _SS_cc_ii_ee_nn_tt_ii_ss_tt_ss_ _ |
 |Provide `datasets` which they would   |Are end `users` who desire to perform |
 |like to make available for `study` by |`computations` or `answer` a specific |
 |an `outside party` they may or may not|`question` using one or more data     |
 |_`_f_u_l_l_y_ _t_r_u_s_t_`_ _h_a_s_ _g_o_o_d_ _i_n_t_e_n_t_i_o_n_s_._ _ _ _ _|_o_w_n_e_r_s_'_ _`_d_a_t_a_s_e_t_s_`_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
```

### Comparing `syft-0.8.6/README.md` & `syft-0.8.6b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.6,<0.8.7")
+sy.requires(">=0.8.5,<0.8.6")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.6,<0.8.7")
+sy.requires(">=0.8.5,<0.8.6")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="notebooks/api">API Example Notebooks</a>
 
@@ -132,20 +132,19 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
+`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
 
 Deprecated:
 
-- `0.8.5-post.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5-post.2/notebooks/api/0.8">API</a>
 - `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-_o_n_%_2_0_s_l_a_c_k_-
 _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_m_d_b_o_o_k_]
 
 [Syft Logo]Perform data science on `data` that remains in `someone else's`
 server # Quickstart â `Linux` â `macOS` â `Windows` â `Docker` â
 `Podman` â `Kubernetes` ## Install Client ```bash $ pip install -U syft
 [data_science] ``` ## Launch Server ```python # from Jupyter / Python import
-syft as sy sy.requires(">=0.8.6,<0.8.7") node = sy.orchestra.launch(name="my-
+syft as sy sy.requires(">=0.8.5,<0.8.6") node = sy.orchestra.launch(name="my-
 domain", port=8080, dev_mode=True, reset=True) ``` ```bash # or from the
 command line $ syft launch --name=my-domain --port=8080 --reset=True Starting
 syft-node server on 0.0.0.0:8080 ``` ## Launch Client ```python import syft as
-sy sy.requires(">=0.8.6,<0.8.7") domain_client = sy.login(port=8080,
+sy sy.requires(">=0.8.5,<0.8.6") domain_client = sy.login(port=8080,
 email="info@openmined.org", password="changethis") ``` ## PySyft in 10 minutes
 ð _A_P_I_ _E_x_a_m_p_l_e_ _N_o_t_e_b_o_o_k_s - _0_0_-_l_o_a_d_-_d_a_t_a_._i_p_y_n_b - _0_1_-_s_u_b_m_i_t_-_c_o_d_e_._i_p_y_n_b - _0_2_-
 _r_e_v_i_e_w_-_c_o_d_e_-_a_n_d_-_a_p_p_r_o_v_e_._i_p_y_n_b - _0_3_-_d_a_t_a_-_s_c_i_e_n_t_i_s_t_-_d_o_w_n_l_o_a_d_-_r_e_s_u_l_t_._i_p_y_n_b - _0_4_-
 _j_a_x_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-_r_e_q_u_e_s_t_s_._i_p_y_n_b -
 _0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b - _0_9_-_b_l_o_b_-
 _s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-_k_8_s_._i_p_y_n_b ##
 Deploy Kubernetes Helm Chart **Note**: Assuming we have a Kubernetes cluster
@@ -41,45 +41,44 @@
 `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where
 `private data` lives ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k #
 Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run: `pip
 install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires
 ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires: ð `python
 3.10 - 3.12` - Run: `pip install -U syft` - PyGrid Requires: ð³ `docker`,
 ð¦¦ `podman` or â¸ï¸ `kubernetes` - Run: `hagrid launch ...` # Versions
-`0.9.0` - Coming soon... `0.8.7` (Beta) - `dev` branch ðð½ _A_P_I - Coming
-soon... `0.8.6` (Stable) - _A_P_I Deprecated: - `0.8.5-post.2` - _A_P_I - `0.8.4` -
-_A_P_I - `0.8.3` - _A_P_I - `0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` -
-_C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d - `0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix -
-`0.2.0` - `0.5.0` PySyft and PyGrid use the same `version` and its best to
-match them up where possible. We release weekly betas which can be used in each
-context: PySyft (Stable): `pip install -U syft` PyGrid (Stable) `hagrid launch
-... tag=latest` PySyft (Beta): `pip install -U syft --pre` PyGrid (Beta):
-`hagrid launch ... tag=beta` HAGrid is a cli / deployment tool so the latest
-version of `hagrid` is usually the best. # What is Syft? [Syft]`Syft` is
-OpenMined's `open source` stack that provides `secure` and `private` Data
-Science in Python. Syft decouples `private data` from model training, using
-techniques like [Federated Learning](https://ai.googleblog.com/2017/04/
-federated-learning-collaborative.html), [Differential Privacy](https://
-en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
-//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
-like interface and integration with `Deep Learning` frameworks, so that you as
-a `Data Scientist` can maintain your current workflow while using these new
-`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
-`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
-limits` set by the `data owner`, get `answers` to those `questions`, all
-without obtaining a `copy` of the data itself. We call this process `Remote
-Data Science`. It means in a wide variety of `domains` across society, the
-current `risks` of sharing information (`copying` data) with someone such as,
-privacy invasion, IP theft and blackmail will no longer prevent the vast
-`benefits` such as innovation, insights and scientific discovery which secure
-access will provide. No more cold calls to get `access` to a dataset. No more
-weeks of `wait times` to get a `result` on your `query`. It also means `1000x
-more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Terminology
+`0.9.0` - Coming soon... `0.8.6` (Beta) - `dev` branch ðð½ _A_P_I - Coming
+soon... `0.8.5` (Stable) - _A_P_I Deprecated: - `0.8.4` - _A_P_I - `0.8.3` - _A_P_I -
+`0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` - _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d -
+`0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix - `0.2.0` - `0.5.0` PySyft
+and PyGrid use the same `version` and its best to match them up where possible.
+We release weekly betas which can be used in each context: PySyft (Stable):
+`pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest` PySyft
+(Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ... tag=beta`
+HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
+the best. # What is Syft? [Syft]`Syft` is OpenMined's `open source` stack that
+provides `secure` and `private` Data Science in Python. Syft decouples `private
+data` from model training, using techniques like [Federated Learning](https://
+ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential
+Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted
+Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is
+done with a `numpy`-like interface and integration with `Deep Learning`
+frameworks, so that you as a `Data Scientist` can maintain your current
+workflow while using these new `privacy-enhancing techniques`. ### Why should I
+use Syft? `Syft` allows a `Data Scientist` to ask `questions` about a `dataset`
+and, within `privacy limits` set by the `data owner`, get `answers` to those
+`questions`, all without obtaining a `copy` of the data itself. We call this
+process `Remote Data Science`. It means in a wide variety of `domains` across
+society, the current `risks` of sharing information (`copying` data) with
+someone such as, privacy invasion, IP theft and blackmail will no longer
+prevent the vast `benefits` such as innovation, insights and scientific
+discovery which secure access will provide. No more cold calls to get `access`
+to a dataset. No more weeks of `wait times` to get a `result` on your `query`.
+It also means `1000x more data` in every domain. PySyft opens the doors to a
+streamlined Data Scientist `workflow`, all with the individual's `privacy` at
+its heart. # Terminology
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |                  [[IImmaaggee]]             |                 [[IImmaaggee]]              |
 |_ _ _ _ _ _ _ _ _?ð_?_?_?¨_?ð_?_?_?»_?â_?_?_?ð_?_?_?¼_ _DD_aa_tt_aa_ _OO_ww_nn_ee_rr_ss_ _ _ _|_ _ _ _ _ _?ð_?_?_?©_?ð_?_?_?½_?â_?_?_?ð_?_?_?¬_ _DD_aa_tt_aa_ _SS_cc_ii_ee_nn_tt_ii_ss_tt_ss_ _ |
 |Provide `datasets` which they would   |Are end `users` who desire to perform |
 |like to make available for `study` by |`computations` or `answer` a specific |
 |an `outside party` they may or may not|`question` using one or more data     |
 |_`_f_u_l_l_y_ _t_r_u_s_t_`_ _h_a_s_ _g_o_o_d_ _i_n_t_e_n_t_i_o_n_s_._ _ _ _ _|_o_w_n_e_r_s_'_ _`_d_a_t_a_s_e_t_s_`_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
```

### Comparing `syft-0.8.6/setup.cfg` & `syft-0.8.6b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.6"
+version = attr: "0.8.6-beta.1"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: PYPI.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.6/src/syft/VERSION` & `syft-0.8.6b1/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.6"
+__version__ = "0.8.6-beta.1"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.6/src/syft/__init__.py` & `syft-0.8.6b1/src/syft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.6"
+__version__ = "0.8.6-beta.1"
 
 # stdlib
 from collections.abc import Callable
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
```

### Comparing `syft-0.8.6/src/syft/abstract_node.py` & `syft-0.8.6b1/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/api.py` & `syft-0.8.6b1/src/syft/client/api.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/client.py` & `syft-0.8.6b1/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/connection.py` & `syft-0.8.6b1/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/deploy.py` & `syft-0.8.6b1/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/domain_client.py` & `syft-0.8.6b1/src/syft/client/domain_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/enclave_client.py` & `syft-0.8.6b1/src/syft/client/enclave_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/gateway_client.py` & `syft-0.8.6b1/src/syft/client/gateway_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/registry.py` & `syft-0.8.6b1/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/search.py` & `syft-0.8.6b1/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/syncing.py` & `syft-0.8.6b1/src/syft/client/syncing.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/client/user_settings.py` & `syft-0.8.6b1/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/custom_worker/builder.py` & `syft-0.8.6b1/src/syft/custom_worker/builder.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/custom_worker/builder_docker.py` & `syft-0.8.6b1/src/syft/custom_worker/builder_docker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/custom_worker/builder_k8s.py` & `syft-0.8.6b1/src/syft/custom_worker/builder_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/custom_worker/builder_types.py` & `syft-0.8.6b1/src/syft/custom_worker/builder_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/custom_worker/config.py` & `syft-0.8.6b1/src/syft/custom_worker/config.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/custom_worker/k8s.py` & `syft-0.8.6b1/src/syft/custom_worker/k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/custom_worker/runner_k8s.py` & `syft-0.8.6b1/src/syft/custom_worker/runner_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/custom_worker/utils.py` & `syft-0.8.6b1/src/syft/custom_worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/exceptions/exception.py` & `syft-0.8.6b1/src/syft/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/external/__init__.py` & `syft-0.8.6b1/src/syft/external/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/external/oblv/__init__.py` & `syft-0.8.6b1/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/external/oblv/deployment.py` & `syft-0.8.6b1/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/external/oblv/deployment_client.py` & `syft-0.8.6b1/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/external/oblv/exceptions.py` & `syft-0.8.6b1/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.6b1/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.6b1/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/external/oblv/oblv_service.py` & `syft-0.8.6b1/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/gevent_patch.py` & `syft-0.8.6b1/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/img/logo.png` & `syft-0.8.6b1/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.6b1/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/node/credentials.py` & `syft-0.8.6b1/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/node/node.py` & `syft-0.8.6b1/src/syft/node/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 from ..store.sqlite_document_store import SQLiteStoreClientConfig
 from ..store.sqlite_document_store import SQLiteStoreConfig
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
 from ..util.experimental_flags import flags
 from ..util.telemetry import instrument
-from ..util.util import get_dev_mode
 from ..util.util import get_env
 from ..util.util import get_queue_address
 from ..util.util import random_name
 from ..util.util import str_to_bool
 from ..util.util import thread_ident
 from .credentials import SyftSigningKey
 from .credentials import SyftVerifyKey
@@ -175,14 +174,18 @@
     return get_env(DEFAULT_ROOT_USERNAME, "Jane Doe")
 
 
 def get_default_root_password() -> str | None:
     return get_env(DEFAULT_ROOT_PASSWORD, "changethis")  # nosec
 
 
+def get_dev_mode() -> bool:
+    return str_to_bool(get_env("DEV_MODE", "False"))
+
+
 def get_enable_warnings() -> bool:
     return str_to_bool(get_env("ENABLE_WARNINGS", "False"))
 
 
 def get_container_host() -> str | None:
     return get_env("CONTAINER_HOST")
 
@@ -1420,14 +1423,16 @@
 
     def get_unauthed_context(
         self, login_credentials: UserLoginCredentials
     ) -> NodeServiceContext:
         return UnauthedServiceContext(node=self, login_credentials=login_credentials)
 
     def create_initial_settings(self, admin_email: str) -> NodeSettingsV2 | None:
+        if self.name is None:
+            self.name = random_name()
         try:
             settings_stash = SettingsStash(store=self.document_store)
             if self.signing_key is None:
                 print("create_initial_settings failed as there is no signing key")
                 return None
             settings_exists = settings_stash.get_all(self.signing_key.verify_key).ok()
             if settings_exists:
```

### Comparing `syft-0.8.6/src/syft/node/routes.py` & `syft-0.8.6b1/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/node/run.py` & `syft-0.8.6b1/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/node/server.py` & `syft-0.8.6b1/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/node/worker_settings.py` & `syft-0.8.6b1/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/protocol/data_protocol.py` & `syft-0.8.6b1/src/syft/protocol/data_protocol.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,33 +5,29 @@
 from collections.abc import MutableSequence
 import hashlib
 import json
 from operator import itemgetter
 import os
 from pathlib import Path
 import re
-from types import UnionType
-import typing
 from typing import Any
-import warnings
 
 # third party
 from packaging.version import parse
 from result import OkErr
 from result import Result
 
 # relative
 from .. import __version__
 from ..serde.recursive import TYPE_BANK
 from ..service.response import SyftError
 from ..service.response import SyftException
 from ..service.response import SyftSuccess
 from ..types.dicttuple import DictTuple
 from ..types.syft_object import SyftBaseObject
-from ..util.util import get_dev_mode
 
 PROTOCOL_STATE_FILENAME = "protocol_version.json"
 PROTOCOL_TYPE = str | int
 
 
 def natural_key(key: PROTOCOL_TYPE) -> list[int | str | Any]:
     """Define key for natural ordering of strings."""
@@ -53,61 +49,30 @@
     return Path(os.path.abspath(str(Path(__file__).parent)))
 
 
 def protocol_release_dir() -> Path:
     return data_protocol_dir() / "releases"
 
 
-def handle_union_type_klass_name(type_klass_name: str) -> str:
-    if type_klass_name == typing.Union.__name__:
-        return UnionType.__name__
-    return type_klass_name
-
-
-def handle_annotation_repr_(annotation: type) -> str:
-    """Handle typing representation."""
-    origin = typing.get_origin(annotation)
-    args = typing.get_args(annotation)
-    if origin and args:
-        args_repr = ", ".join(getattr(arg, "__name__", str(arg)) for arg in args)
-        origin_repr = getattr(origin, "__name__", str(origin))
-
-        # Handle typing.Union and types.UnionType
-        origin_repr = handle_union_type_klass_name(origin_repr)
-        return f"{origin_repr}: [{args_repr}]"
-    elif args:
-        args_repr = ", ".join(
-            getattr(arg, "__name__", str(arg)) for arg in sorted(args)
-        )
-        return args_repr
-    else:
-        return repr(annotation)
-
-
 class DataProtocol:
-    def __init__(self, filename: str, raise_exception: bool = False) -> None:
+    def __init__(self, filename: str) -> None:
         self.file_path = data_protocol_dir() / filename
-        self.raise_exception = raise_exception
         self.load_state()
 
     def load_state(self) -> None:
         self.protocol_history = self.read_history()
         self.state = self.build_state()
         self.diff, self.current = self.diff_state(self.state)
         self.protocol_support = self.calculate_supported_protocols()
 
     @staticmethod
     def _calculate_object_hash(klass: type[SyftBaseObject]) -> str:
         # TODO: this depends on what is marked as serde
-
-        # Rebuild the model to ensure that the fields are up to date
-        # and any ForwardRef are resolved
-        klass.model_rebuild()
         field_data = {
-            field: handle_annotation_repr_(field_info.rebuild_annotation())
+            field: repr(field_info.annotation)
             for field, field_info in sorted(
                 klass.model_fields.items(), key=itemgetter(0)
             )
         }
         obj_meta_info = {
             "canonical_name": klass.__canonical_name__,
             "version": klass.__version__,
@@ -242,29 +207,22 @@
                         object_diff[canonical_name][str(version)]["version"] = int(
                             version
                         )
                         object_diff[canonical_name][str(version)]["hash"] = hash_str
                         object_diff[canonical_name][str(version)]["action"] = "add"
                         continue
 
-                    error_msg = (
+                    raise Exception(
                         f"{canonical_name} for class {cls.__name__} fqn {cls} "
                         + f"version {version} hash has changed. "
                         + f"{hash_str} not in {versions.values()}. "
                         + "Is a unique __canonical_name__ for this subclass missing? "
                         + "If the class has changed you will need to define a new class with the changes, "
                         + "with same __canonical_name__ and bump the __version__ number."
-                        + f"{cls.model_fields}"
                     )
-
-                    if get_dev_mode() or self.raise_exception:
-                        raise Exception(error_msg)
-                    else:
-                        warnings.warn(error_msg, stacklevel=1, category=UserWarning)
-                        break
                 else:
                     # new object so its an add
                     object_diff[canonical_name][str(version)] = {}
                     object_diff[canonical_name][str(version)]["version"] = int(version)
                     object_diff[canonical_name][str(version)]["hash"] = hash_str
                     object_diff[canonical_name][str(version)]["action"] = "add"
                     continue
@@ -454,15 +412,14 @@
 
         # Delete the current released protocol
         protocol_history.pop(latest_protocol)
         protocol_file_path.unlink()
 
         # Save history
         self.save_history(protocol_history)
-        self.load_state()
 
     def check_protocol(self) -> Result[SyftSuccess, SyftError]:
         if len(self.diff) != 0:
             return SyftError(message="Protocol Changes Unstaged")
         else:
             return SyftSuccess(message="Protocol Stable")
 
@@ -501,34 +458,26 @@
 
     @property
     def has_dev(self) -> bool:
         if "dev" in self.protocol_history.keys():
             return True
         return False
 
-    def reset_dev_protocol(self) -> None:
-        if self.has_dev:
-            del self.protocol_history["dev"]
-            self.save_history(self.protocol_history)
-
 
-def get_data_protocol(raise_exception: bool = False) -> DataProtocol:
-    return DataProtocol(
-        filename=data_protocol_file_name(),
-        raise_exception=raise_exception,
-    )
+def get_data_protocol() -> DataProtocol:
+    return DataProtocol(filename=data_protocol_file_name())
 
 
 def stage_protocol_changes() -> Result[SyftSuccess, SyftError]:
-    data_protocol = get_data_protocol(raise_exception=True)
+    data_protocol = get_data_protocol()
     return data_protocol.stage_protocol_changes()
 
 
 def bump_protocol_version() -> Result[SyftSuccess, SyftError]:
-    data_protocol = get_data_protocol(raise_exception=True)
+    data_protocol = get_data_protocol()
     return data_protocol.bump_protocol_version()
 
 
 def check_or_stage_protocol() -> Result[SyftSuccess, SyftError]:
     data_protocol = get_data_protocol()
     return data_protocol.check_or_stage_protocol()
```

### Comparing `syft-0.8.6/src/syft/protocol/releases/0.8.2.json` & `syft-0.8.6b1/src/syft/protocol/releases/0.8.2.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/protocol/releases/0.8.3.json` & `syft-0.8.6b1/src/syft/protocol/releases/0.8.3.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/protocol/releases/0.8.4.json` & `syft-0.8.6b1/src/syft/protocol/releases/0.8.4.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/protocol/releases/0.8.6.json` & `syft-0.8.6b1/src/syft/protocol/releases/0.8.5.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9948050213675219%*

 * *Differences: {"'4'": "{'object_versions': {'ActionObject': {'3': {'hash': "*

 * *        "'37bb8f0f87b1da2525da8f6873e6257dff4a732f2dba293b62931ad0b85ef9e2'}}, 'AnyActionObject': "*

 * *        "{'3': {'hash': '7c55461e3c6ba36ff999c64eb1b97a65b5a1f27193a973b1355ee2675f14c313'}}, "*

 * *        "'BlobFileOBject': {'2': {'hash': "*

 * *        "'1ab941c7669572a41067a17e0e3f2d9c7056f7a4df8f899e87ae2358d9113b02'}}, 'JobInfo': {'2': "*

 * *        "{'hash': '058a7fc0c63e0bcb399088e7fcde9b8522522e269b00cee2d093d1c890550ce8'}}, "*

 * *        "'ExecutionOu […]*

```diff
@@ -5,15 +5,15 @@
                 "1": {
                     "action": "remove",
                     "hash": "c0e83867b107113e6fed06364ba364c24b2f4af35b15a3869b176318d3be7989",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "1be1f6793478cd2e4a0cc84713426b2d5586969e98058f4e8b91fc19293cf445",
+                    "hash": "1264dca857f7d5c8d1aa92791726a2e17567aba82538b64d357b988d1ae3a8c9",
                     "version": 2
                 }
             },
             "Action": {
                 "1": {
                     "action": "remove",
                     "hash": "5cf71ee35097f17fbb1dd05096f875211d71cf07161205d7f6a9c11fd49d5272",
@@ -22,39 +22,39 @@
                 "2": {
                     "action": "remove",
                     "hash": "a13b50c4d23bd6deb7896e394f2a20e6cef4c33c5e6f4ee30f19eaffab708f21",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "8b9957c26b2fa6513d6a07cdde6a4fab003693cf4b787e8bda0ecc2503ae9d54",
+                    "hash": "18525c0610aea0aa62fe496a739b0ca7fb828617b4fca73840807d3c7b1477a7",
                     "version": 3
                 }
             },
             "ActionDataEmpty": {
                 "1": {
                     "action": "remove",
                     "hash": "89b5912fe5416f922051b8068be6071a03c87a4ab264959de524f1b86e95f028",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "1fd3a1d3b3d97c8fe4ff2e51567c026830e6c1489f82caa4c6e3ca24a11e1da0",
+                    "hash": "2bea14a344a82a10725a9e933bb1838ffbe2d28771ee4f54f40b4d5663840a7c",
                     "version": 2
                 }
             },
             "ActionDataLink": {
                 "1": {
                     "action": "remove",
                     "hash": "10bf94e99637695f1ba283f0b10e70743a4ebcb9ee75aefb1a05e6d6e1d21a71",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "59756e8b5729df61217f8bcf53f54e99c7fcc715594488779e19296dec582951",
+                    "hash": "4551f22ea68af0d0943f9aa239b4fd468cf9f4da43589b536651fc3d27d99f12",
                     "version": 2
                 }
             },
             "ActionObject": {
                 "1": {
                     "action": "remove",
                     "hash": "632446f1415102490c93fafb56dd9eb29d79623bcc5e9f2e6e37c4f63c2c51c3",
@@ -63,15 +63,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "577aa1f010b90194958a18ec38ee21db3718bd96d9e036501c6ddeefabedf432",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "d5303167b1048c1b956781c6daeaa93ec792bea5181c076c93da74dfec0a6127",
+                    "hash": "37bb8f0f87b1da2525da8f6873e6257dff4a732f2dba293b62931ad0b85ef9e2",
                     "version": 3
                 }
             },
             "ActionQueueItem": {
                 "1": {
                     "action": "remove",
                     "hash": "11a43caf9164eb2a5a21f4bcb0ca361d0a5d134bf3c60173f2c502d0d80219de",
@@ -80,39 +80,39 @@
                 "2": {
                     "action": "remove",
                     "hash": "6413ed01e949cac169299a43ce40651f9bf8053e408b6942853f8afa8a693b3d",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "5bcda9c7df78ded9ea4b53710191f37054d3046ea01125b755afc8c30dd9eed2",
+                    "hash": "4159d6ea45bc82577828bc19d668196422ff29bb8cc298b84623e6f4f476aaf3",
                     "version": 3
                 }
             },
             "ActionStoreChange": {
                 "1": {
                     "action": "remove",
                     "hash": "17b865e75eb3fb2693924fb00ba87a25260be45d55a4eb2184c4ead22d787cbe",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0d97c83b6a355eaa6c351cd50c36ba58c0f0e08e63e16af1c44cba76c61af834",
+                    "hash": "3a1c8f10afb4c4d10a4096a1371e4780b2cb40bb2253193bfced6c250d3e8547",
                     "version": 2
                 }
             },
             "AnswerProjectPoll": {
                 "1": {
                     "action": "remove",
                     "hash": "ff2e1ac7bb764c99d646b96eb3ebfbf9311599b7e3be07aa4a4eb4810bb6dd12",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "7467766e01c8afadb1b2dbe548c9f540a7d6869fed4e98db96c2705bb6f3f3c2",
+                    "hash": "fff1a7e5ca30b76132cf8b6225cb576467d9727349b9dc54d4131fede03c10f3",
                     "version": 2
                 }
             },
             "AnyActionObject": {
                 "1": {
                     "action": "remove",
                     "hash": "bcb31f847907edc9c95d2d120dc5427854604f40940e3f41cd0474a1820ac65e",
@@ -121,75 +121,75 @@
                 "2": {
                     "action": "remove",
                     "hash": "002d8be821140befebbc0503e6bc1ef8779094e24e46305e5da5af6eecb56b13",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "22568b8c3d700b7eaa3291b9f3d014dda3d6dbe20f1f8eab87210ccb2f035bbc",
+                    "hash": "7c55461e3c6ba36ff999c64eb1b97a65b5a1f27193a973b1355ee2675f14c313",
                     "version": 3
                 }
             },
             "Asset": {
                 "1": {
                     "action": "remove",
                     "hash": "24350b8d9597df49999918ad42e0eece1328ea30389311f1e0a420be8f39b8a1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b5ce972e6b0341da041f457660eca873bd9bb4f93e73158767f951cb93b53d10",
+                    "hash": "64661b3bc84a2df81ce631641a0fe3f0d969618b6855971f5e51e5770c278bba",
                     "version": 2
                 }
             },
             "AzureRemoteConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "c05c6caa27db4e385c642536d4b0ecabc0c71e91220d2e6ce21a2761ca68a673",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "56ab4455e8182d3c300efb31ae019a2211ecb9e579ec1a41a087c98ee8e9f317",
+                    "hash": "2f820aa55e6476b455fec7774346a4c0dad212bde1400f1f53f42c8864b7ded4",
                     "version": 2
                 }
             },
             "AzureSecureFilePathLocation": {
                 "1": {
                     "action": "remove",
                     "hash": "1bb15f3f9d7082779f1c9f58de94011487924cb8a8c9c2ec18fd7c161c27fd0e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b05c5b759d43d9aa13e2a11087d13ff78cbec946768e3ff130fcac83a4216117",
+                    "hash": "29a0c01a59d8632037c6d18d6fce1512b651e1aa8493b302746ff294c7bd331d",
                     "version": 2
                 }
             },
             "BaseConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "4e5257080ce615aa4122b02bad8487e4c7d6d0f171ff77abbc9e8cd3e33df89a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "383d9ce8873520c9224e00797a96d6dc2e64f054795e3b1de2ac7cd8ce68df86",
+                    "hash": "45e4480e6fbb5183e36cbe3bd18e21d65c43cc5809028a13ab49270e0a565da6",
                     "version": 2
                 }
             },
             "BlobDeposit": {
                 "1": {
                     "action": "remove",
                     "hash": "c98e6da658a3be01ead4ea6ee6a4c10046879f0ce0f5fc5f946346671579b229",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "7b0709298f6a6bd1e33244f655dc4f3bb95645f9e474f2de331869071e3ab384",
+                    "hash": "87dd601b58f31ccf8e3001e8723d8d251f84bd7ab9a2f87ff7c6cf05b074d41f",
                     "version": 2
                 }
             },
             "BlobFile": {
                 "1": {
                     "action": "remove",
                     "hash": "47ed55183d619c6c624e35412360a41de42833e2c24223c1de1ad12a84fdafc2",
@@ -198,27 +198,27 @@
                 "3": {
                     "action": "remove",
                     "hash": "8f1710c754bb3b39f546b97fd69c4826291398b247976bbc41fa873af431bca9",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "c74d6f9899d928430a38bd4585069b557de8e985a13f82f166479bd7f32d5a85",
+                    "hash": "05ef86582c6b8967499eb0f57d048676e15390ce74891409fada522226563754",
                     "version": 4
                 }
             },
             "BlobFileOBject": {
                 "1": {
                     "action": "remove",
                     "hash": "8da2c80ced4f0414c671313c4b63d05846df1e397c763d99d803be86c29755bb",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f8d75c274f7ae4138e85bb936c3f27241cc0f7dd011ba237396733c53e5a1b0d",
+                    "hash": "1ab941c7669572a41067a17e0e3f2d9c7056f7a4df8f899e87ae2358d9113b02",
                     "version": 2
                 }
             },
             "BlobRetrieval": {
                 "1": {
                     "action": "remove",
                     "hash": "a8d7e1d6483e7a9b5a130e837fa398862aa6cbb316cc5f4470450d835755fdd9",
@@ -227,27 +227,27 @@
                 "2": {
                     "action": "remove",
                     "hash": "4c4fbdb6df5bb9fcbe914a9890bd1c1b6a1b3f382a04cbc8752a5a1b03130111",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "609daef405c4606f61b76df23c91ae75a97788a4e99f3e1ee7faa5a35eab8748",
+                    "hash": "ab0f1f06c57b3cd8bd362514d662b170a888a2487dbb1e9f880f611ce47a2b2c",
                     "version": 3
                 }
             },
             "BlobRetrievalByURL": {
                 "3": {
                     "action": "remove",
                     "hash": "0b664100ea08413ca4ef04665ca910c2cf9535539617ea4ba33687d05cdfe747",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "3a82ec6220eda51289931689db2f598e5e44a610b0a229113c4695f897cc9f2b",
+                    "hash": "3fadedaf8e4ba97db9d4ddf1cf954338113cbb88d016253c008b11f0dfe19c59",
                     "version": 4
                 }
             },
             "BlobStorageEntry": {
                 "1": {
                     "action": "remove",
                     "hash": "9f1b027cce390ee6f71c7a81e7420bb71a477b29c6c62ba74e781a97bc5434e6",
@@ -256,15 +256,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "5472bdd5bdce6d0b561543a6bac70d47bf0c05c141a21450751460cc538d6b55",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "0a5cf4058b330727a2d617a99d56070a7a6977b7d10f532fbb35cd4fe97b7678",
+                    "hash": "136b0fb4908eb0c065a7ba6644ff5377a3c22ce8d97b3e48de1eb241101d4806",
                     "version": 3
                 }
             },
             "BlobStorageMetadata": {
                 "1": {
                     "action": "remove",
                     "hash": "6888943be3f97186190dd26d7eefbdf29b15c6f2fa459e13608065ebcdb799e2",
@@ -273,322 +273,322 @@
                 "2": {
                     "action": "remove",
                     "hash": "674f4c52a8444289d5ef389b919008860e2b0e7acbaafa774d58e492d5b6741a",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "b4b222dc8a994b5ff6d685818973516d89b615e2321d122edc28d1c30479a9fb",
+                    "hash": "643065504ecfabd283c736c794cfb41fb85156879940488d6ea851bb2ac3c16a",
                     "version": 3
                 }
             },
             "Change": {
                 "1": {
                     "action": "remove",
                     "hash": "aefebd1601cf5bfd4817b0db75300a78299cc4949ead735a90873cbd22c8d4bc",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "9784905430b48d60be31b89d5fdbf559f8f7cc0a3be3428a3ba4b17b0db06330",
+                    "hash": "b661753ae9187feb92751edb4a38066c9c14aba73e3639d44ac5fe7aee8b2ab9",
                     "version": 2
                 }
             },
             "ChangeStatus": {
                 "1": {
                     "action": "remove",
                     "hash": "627f6f8e42cc285336aa6fd4916285d796140f4ff901487b7cb3907ef0f116a6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "37e33e685081a3e45155ffe8f02371a5dde82841ebb3d1b60c0ff06031622ccd",
+                    "hash": "8a62d5bcde312e7b9efd1d0b26cab6de7affa1e3ffe9182f8598137340408084",
                     "version": 2
                 }
             },
             "CodeHistoriesDict": {
                 "1": {
                     "action": "remove",
                     "hash": "95288411cd5843834f3273a2fd66a7df2e603e980f4ab1d329f9ab17d5d2f643",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "9ebf38ad3f12b1ec397bd977cf1013fb8703e02562a6e74b7d17ea2debfcb4a1",
+                    "hash": "36175742343fdb2c9ea54809c08857cf1f30451245ebdca45b13020f6c7c0e2e",
                     "version": 2
                 }
             },
             "CodeHistory": {
                 "1": {
                     "action": "remove",
                     "hash": "a7baae93862ae0aa67675f1617574e31aafb15a9ebff633eb817278a3a867161",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f9a3e33bb89c72612b2c5ea501ca16bdbac832a94af1f373c76458f2a5a96614",
+                    "hash": "54793b2909c70303c58fb720e431752547e29e56a616e544b6a103b2bfd2f73b",
                     "version": 2
                 }
             },
             "CodeHistoryView": {
                 "1": {
                     "action": "remove",
                     "hash": "0ed1a2a04a962ecbcfa38b0b8a03c1e51e8946a4b80f6bf2557148ce658671ce",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "91f1c8b4d9f8e8be517cda487615ae2e3a9df6fd4bdd2c7be51836b851f429f0",
+                    "hash": "3d5f79f8367c229f163ab746ef8c7069bec5a1478a19812dbac735fc333e41c3",
                     "version": 2
                 }
             },
             "Contributor": {
                 "1": {
                     "action": "remove",
                     "hash": "d1d4f25bb87e59c0414501d3335097de66815c164c9ed5a7850ff8bec69fbcdc",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "7beef331ac6ea90632adc81a96bd99a656467ab8f2334007c624c64ea8a4b886",
+                    "hash": "55259f1e4f1b9da4ac83b032adb86eb4a1322a06584790d1300131777212dbaa",
                     "version": 2
                 }
             },
             "CreateAsset": {
                 "1": {
                     "action": "remove",
                     "hash": "1b4c71569b8da64258672483bd36dc4aa99a32d4cb519659241d15bc898041a6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "954da64a48165139f585e9e5a9526aa43a73a0709c1c1bf58e937e8c3e0f184f",
+                    "hash": "93c75b45b9b74c69243cc2f2ef2d661e11eef5c23ecf71692ffdbd467d11efe6",
                     "version": 2
                 }
             },
             "CreateBlobStorageEntry": {
                 "1": {
                     "action": "remove",
                     "hash": "61a373336e83645f1b6d78a320323d9ea4ee91b3d87b730cb0608fbfa0072262",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b252fe14bd22f92866c20bfffbdab1a839c8648c7b2cda81500cbeb9a5d85c57",
+                    "hash": "9046843fba39e5700aeb8c442a7e4ac5e772b12f6ac502367b2e5decbb26761f",
                     "version": 2
                 }
             },
             "CreateCustomImageChange": {
                 "1": {
                     "action": "remove",
                     "hash": "bc09dca7995938f3b3a2bd9c8b3c2feffc8484df466144a425cb69cadb2ab635",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "91d2333291eb43c9814eb1d3ad1f736d5c1ccb9370de6734e506f0463fa92159",
+                    "hash": "6569fb11bccd100cd4b6050084656e7e7c46b9405ff76589b870402b26a6927b",
                     "version": 2
                 }
             },
             "CreateCustomWorkerPoolChange": {
                 "1": {
                     "action": "remove",
                     "hash": "86894f8ccc037de61f44f9698fd113ba02c3cf3870a3048c00a46e15dcd1941c",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "84cb18e884dfb1509d78d8775110314278444af2b2dd5370cb2621d28f8d1aaa",
+                    "hash": "e2a223a65461b502f097f06453f878b54175b4055dad3ec9b09c1eb9458a575e",
                     "version": 2
                 }
             },
             "CreateDataset": {
                 "1": {
                     "action": "remove",
                     "hash": "3b020d9b8928cbd7e91f41c749ab4c932e19520696a183f2c7cd1312ebb640d1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "67d45b8e93be3c95cdc5c5c2ff8d7e181e0c3200badc279d56be4f51f5e78ce7",
+                    "hash": "83c6142c99da6667260e0d6df258b6e173beb18e399d60209b6ffccb5547f1e7",
                     "version": 2
                 }
             },
             "CreateNotification": {
                 "1": {
                     "action": "remove",
                     "hash": "b1f459de374fe674f873a4a5f3fb8a8aabe0d83faad84a933f0a77dd1141159a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "657edc0de0b93399006f9c911de2cd212244acc192ff052abf7215bb41fe83aa",
+                    "hash": "32d046bda4d978fb8e839e2c2c4994b86a60843311b74330e307e6e3e422176f",
                     "version": 2
                 }
             },
             "DataSubject": {
                 "1": {
                     "action": "remove",
                     "hash": "0b8b049d4627727b444c419f5d6a97b7cb97a433088ebf744c854b6a470dadf1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "4385b12c582d711cfadf08f6d9254d2b95652d8aeedbeb350c5dcbf57dab1fea",
+                    "hash": "6d9d65d2723aed8cc4cfce9b5ee4a005ab84f8a24372dc47ce856cb6516835a9",
                     "version": 2
                 }
             },
             "DataSubjectCreate": {
                 "1": {
                     "action": "remove",
                     "hash": "5a94f9fcba75c50d78d71222f0235c5fd4d8003ae0db4d74bdbc4d56a99de3aa",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f33811ae53332a54323cd64772776d0fdf95623f5ee7e3f5759dd36ba9e0397d",
+                    "hash": "b35897295822f061fbc70522ca8967cd2be53a5c01b19e24c587cd7b0c4aa3e8",
                     "version": 2
                 }
             },
             "DataSubjectMemberRelationship": {
                 "1": {
                     "action": "remove",
                     "hash": "0a820edc9f1a87387acc3c611fe852752fcb3dab7608058f2bc48211be7bfbd2",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6f03ee3c35cd02973210c25ce99f50effdaa6156211329bddf763272d9d32585",
+                    "hash": "159d4e4f2463b213a65082b270acbb57ae84c5f0dbc897fda75486290b3148f1",
                     "version": 2
                 }
             },
             "Dataset": {
                 "1": {
                     "action": "remove",
                     "hash": "99ca2fa3e46fd9810222d269fac6accb546f632e94d5d57529016ba5e55af5a8",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "5e108228813bda478de1d6496fffc888f2f1bbaa7ae11ccce100987ee935c5ce",
+                    "hash": "0bbae6e3665e61e97eeb328400efc678dfb26409616c66bf48f3f34bbf102721",
                     "version": 2
                 }
             },
             "DatasetPageView": {
                 "1": {
                     "action": "remove",
                     "hash": "b1de14bb9b6a259648dfc59b6a48fa526116afe50a689c24b8bb36fd0e6a97f8",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f7652573278f762788f4ec3d39c3ec14179061429589714ff49210b015d57d0f",
+                    "hash": "c7494afa0ae27326c4521a918eb234ba74eb2c0494ea448255ff310201a16c88",
                     "version": 2
                 }
             },
             "DateTime": {
                 "1": {
                     "action": "remove",
                     "hash": "7e9d89309a10d2110a7ae4f97d8f25a7914853269e8fa0c531630790c1253f17",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "92daa79cc211b880d7c492e32b22fa4b7cce78ef1606a9be4461324f68fb8cd3",
+                    "hash": "c353b8edfa13250507942a3134f0ec9db8fb1d85f4f7a029fe4ad5665614bf5a",
                     "version": 2
                 }
             },
             "DictStoreConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "256e9c623ce0becd555ddd2a55a0c15514e162786b1549388cef98a92a9b18c9",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "071e31e8bf4fdf894b03e0490549be4c40fcb0f0cdecff34866c5d2eded2944f",
+                    "hash": "6cef5c61f567c75c969827fabaf5bd4f4409a399f33b6b2623fbed3c7a597a41",
                     "version": 2
                 }
             },
             "EnclaveMetadata": {
                 "1": {
                     "action": "remove",
                     "hash": "39f85e475015e6f860ddcc5fea819423eba2db8f4b7d8e004c05a44d6f8444c6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6dcc26695abc6a9ecd9d7d1e6507a9f1a92cc5ccd10987e92419bf984245f9a1",
+                    "hash": "5103272305abd2bcf23c616bd9014be986a92c40dc37b6238680114036451852",
                     "version": 2
                 }
             },
             "EnumMutation": {
                 "1": {
                     "action": "remove",
                     "hash": "4c02f956ec9b973064972cc57fc8dd9c525e683f93f804642b4e1bfee1b62e57",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "13275f41942fa8eaa359fe3b0d5ba9f7c8c73564dad6d661441c29beef19a049",
+                    "hash": "6d2e2f64c00dcda74a2545c77abbcf1630c56c26014987038feab174d15bd9d7",
                     "version": 2
                 }
             },
             "ExactMatch": {
                 "1": {
                     "action": "remove",
                     "hash": "e497e2e2380db72766c5e219e8afd13136d8953933d6f1eaf83b14001e887cde",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "8767689e0b6acdc42ed558645ce641098e63094300225e2c8b9e4758abf80104",
+                    "hash": "f752dfdec6b30e1c849e483ac88ab6f0c71a286199415e4f7bc33c8c2502fc1f",
                     "version": 2
                 }
             },
             "ExecutionOutput": {
                 "1": {
                     "action": "add",
-                    "hash": "c2337099eba14767ead75fcc1b1fa265c1898461ede0b5e7758a0e8d11d1757d",
+                    "hash": "201c8abcb6595a64140ad0c3b058557229c7790a25fb55ed229ae0efcb63ad07",
                     "version": 1
                 }
             },
             "HTTPConnection": {
                 "1": {
                     "action": "remove",
                     "hash": "5ee19eaf55ecbe7945ea45924c036ec0f500114a2f64176620961a8c2ec94cdb",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "68409295f8916ceb22a8cf4abf89f5e4bcff0d75dc37e16ede37250ada28df59",
+                    "hash": "c05bfaf9ca6b5f47cd20c52fd7961bf9f372196713c2333fc9bfed8e0383acf1",
                     "version": 2
                 }
             },
             "HTTPNodeRoute": {
                 "1": {
                     "action": "remove",
                     "hash": "1901b9f53f9970ce2bd8307ba9f7cafc0e7eba1d2ec82e4014c6120e605e3741",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "2134ea812f7c6ea41522727ae087245c4b1195ffbad554db638070861cd9eb1c",
+                    "hash": "b7ee63d7b47d2fab46a62d8e7d8277c03f872524457f4fe128cc9759eac72795",
                     "version": 2
                 }
             },
             "JobInfo": {
                 "1": {
                     "action": "remove",
                     "hash": "cf26eeac3d9254dfa439917493b816341f8a379a77d182bbecba3b7ed2c1d00a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "89dbd4a810586b49498be1f5299b565a19871487e14a120433b0a4cf607b6dee",
+                    "hash": "058a7fc0c63e0bcb399088e7fcde9b8522522e269b00cee2d093d1c890550ce8",
                     "version": 2
                 }
             },
             "JobItem": {
                 "1": {
                     "action": "remove",
                     "hash": "7b8723861837b0b7e948b2cf9244159d232185f3407dd6bef108346f941ddf6e",
@@ -602,87 +602,87 @@
                 "3": {
                     "action": "remove",
                     "hash": "5b93a59e28574691339d22826d5650969336a2e930b93d6b3fe6d5409ca0cfc4",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "6a7cc7c2bb4dd234c1508b0af4d3b403cd3b7b427578a775bf80dc36891923ed",
+                    "hash": "dae431b87cadacfd30613519b5dd25d2e4ff59d2a971e21a31d56901103b9420",
                     "version": 4
                 }
             },
             "LibConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "c6ff229aea16874c5d9ae4d1f9e500d13f5cf984bbcee7abd16c5841707a2f78",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "48924a4e5c9dfbc22ef7f2449ca82c7c8d6ae6f6eae070b87747e8a971bd1cb4",
+                    "hash": "0fc4586bc939a15426ba2315f2457c77eea262c9d34756f0ee6b0198c001cf47",
                     "version": 2
                 }
             },
             "LibEndpoint": {
                 "1": {
                     "action": "remove",
                     "hash": "153eac6d8990774eebfffaa75a9895e7c4e1a0e09465d5da0baf4c3a3b03369d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "74916f7c9bbca213b70fcdb5212eae9eb5d3c9fddf4aa35e1fb9a7158fd2d97f",
+                    "hash": "c845900e729bef87be1a0efe69a7059055199eb5a5b9b9e8bd730dd16e18ed7a",
                     "version": 2
                 }
             },
             "LinkedObject": {
                 "1": {
                     "action": "remove",
                     "hash": "824567c6933c095d0e2f6995c8de3581c0fbd2e9e4ead35c8159f7964709c28e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "08ba9bab178011c723f84bdc64ea879a369f4e6fb32d60020ae123e64b19ec42",
+                    "hash": "0c52ad9a259358652f7c78f73ab041185a59b24534cee9f0802313ff4b4d4781",
                     "version": 2
                 }
             },
             "MarkdownDescription": {
                 "1": {
                     "action": "remove",
                     "hash": "519328a3952049f57004013e4fb00840695b24b8575cad983056412c9c9d9ba6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3c4990cee7cc0b9e86c4b1aa6120476d3d7154d4047d8f4a80a10b6ad1415be4",
+                    "hash": "3416f899b925ba0636edd1ac01bf5c6f4f5533eae4f0a825f112bbf89dcd232a",
                     "version": 2
                 }
             },
             "MongoDict": {
                 "1": {
                     "action": "remove",
                     "hash": "640734396edae801e1601fe7777710e67685e552acb0244ad8b4f689599baca9",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "47da755ee2c572f719f9c4624120142f0e3c411aeb03278a9eea5fdd92ad2bad",
+                    "hash": "c83245be5997362196ee7fe2afd2b7ec7a2cf67aed5efe4bde16c7e83dc530b0",
                     "version": 2
                 }
             },
             "MongoStoreConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "e52aa382e300b0b69aaa2d80aadb4e3a9a3c02b3c741b71d56f959c4d3891ce5",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "ab2a664a0b3c6f5e0d8323aa26c399c7810462f1a8178f5e5f5021b95a40570c",
+                    "hash": "f27e70c1c074de2d921f8f0cca02bec90d359cf0a1f255fe77d84455e5daa966",
                     "version": 2
                 }
             },
             "NodeMetadata": {
                 "1": {
                     "action": "remove",
                     "hash": "6bee018894dfdf697ea624740d0bf051750e0b0d8470ced59646f6d8812068ac",
@@ -696,39 +696,39 @@
                 "3": {
                     "action": "remove",
                     "hash": "3cc67abf394a805066a88aef0bea15bde609b9ecbe7ec15172eac5e7a0b7ef7c",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "6d0dd9f388728bb8532ca775587cc7eb9889e111bad8f0b4ba17464140479f9f",
+                    "hash": "9501017d54d67c987bf62a37891e9e2ceaa0f741ff6cc502ea1db7bdf26b98da",
                     "version": 4
                 }
             },
             "NodeMetadataUpdate": {
                 "1": {
                     "action": "remove",
                     "hash": "569d124c23590360bda240c19b53314ccc6204c5d1ab0d2898976a028e002191",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "520ae8ffc0c057ffa827cb7b267a19fb6b92e3cf3c0a3666ac34e271b6dd0aed",
+                    "hash": "cfe5400a5440de50e9a413f84c2aa05bad33135f46b16d21496534973145e93c",
                     "version": 2
                 }
             },
             "NodePeer": {
                 "1": {
                     "action": "remove",
                     "hash": "7b88de7e38490e2d69f31295137673e7ddabc16ab0e2272ff491f6cea1835d63",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "840d11498095c02d3de9bfe48ea8960c81017c4af45cb8af7e12dc9a18ebd2da",
+                    "hash": "14cf8b9bb7c95c20caec8606ae5dddb882832f00fba2326352e7a0f2444dbc9f",
                     "version": 2
                 }
             },
             "NodeSettings": {
                 "1": {
                     "action": "remove",
                     "hash": "b662047bb278f4f5db77c102f94b733c3a929839271b3d6b82ea174a60e2aaf0",
@@ -737,53 +737,53 @@
                 "2": {
                     "action": "remove",
                     "hash": "29a82afcb006a044b6ae04c6ea8a067d145d28b4210bb038ea9fa86ebde108c8",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "2d5f6e79f074f75b5cfc2357eac7cf635b8f083421009a513240b4dbbd5a0fc1",
+                    "hash": "ea0a9336358fc24988e2e157912f1898a9f770d9520b73a34ce2320b0565f99c",
                     "version": 3
                 }
             },
             "NodeSettingsUpdate": {
                 "1": {
                     "action": "remove",
                     "hash": "b6ddc66ff270a3c2c4760e31e1a55d72ed04ccae2d0115ebe2fba6f2bf9bd119",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "e1dc9d2f30c4aae1f7359eb3fd44de5537788cd3c69be5f30c36fb019f07c261",
+                    "hash": "3f66c4c8a21d63b6dba2ad27c452a01aae6b827ca5c161580312dfb850a0d821",
                     "version": 2
                 }
             },
             "Notification": {
                 "1": {
                     "action": "remove",
                     "hash": "d13981f721fe2b3e2717640ee07dc716c596e4ecd442461665c3fdab0b85bf0e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "848bdbdbfc655c8cbb6274d3158fad7d3fcdaf77bf0389031dff0d8cedcdbd24",
+                    "hash": "3814065d869d10444d7413302101c720bc6dd1a105dd7c29eccf38f32351e322",
                     "version": 2
                 }
             },
             "NotificationPreferences": {
                 "1": {
                     "action": "add",
-                    "hash": "e0be3fb928a3e05ba309fc4d59e8eba1e61c6ea09aeb68f25230a5e9446cfcfd",
+                    "hash": "127206b9c72d353d9f1b73fb10d8ecd57f28f9bfbfdc2f7648894cb0d2ad2522",
                     "version": 1
                 }
             },
             "NotifierSettings": {
                 "1": {
                     "action": "add",
-                    "hash": "efa20280a24d48f583d1e21875a9c195466c7df1239cebbce6016fd6c15c02ad",
+                    "hash": "8505ded16432d1741ee16b0eada22da7c6e36ae7b414cfb59168ac846f3e9f54",
                     "version": 1
                 }
             },
             "NumpyArrayObject": {
                 "1": {
                     "action": "remove",
                     "hash": "dcc7b44fa5ad22ae0bc576948f856c172dac1e9de2bc8e2a302e428f3309a278",
@@ -792,15 +792,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "2c631121d9211006edab5620b214dea83e2398bee92244d822227ee316647e22",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "ff3e9e57df17d6027581ae1aa177199751d8685a3b0cb4359e7e55ace3514041",
+                    "hash": "709dc84a946267444a3f9968acf4a5e9807d6aa5143626c3fb635c9282108cc1",
                     "version": 3
                 }
             },
             "NumpyBoolObject": {
                 "1": {
                     "action": "remove",
                     "hash": "a5c822a6a3ca9eefd6a2b68f7fd0bc614fba7995f6bcc30bdc9dc882296b9b16",
@@ -809,15 +809,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "24839ba1c88ed833a134124750d5f299abcdf318670315028ed87b254f4578b3",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "808a042ea9bca5b621417296824bf2a0b170e66c1f714f91ec3feccace41e2a3",
+                    "hash": "bf936c1923ceee4def4cded06d41766998ea472322b0738bade7b85298e469da",
                     "version": 3
                 }
             },
             "NumpyScalarObject": {
                 "1": {
                     "action": "remove",
                     "hash": "5c1b6b6e8ba88bc79e76646d621489b889fe8f9b9fd59f117d594be18a409633",
@@ -826,87 +826,87 @@
                 "2": {
                     "action": "remove",
                     "hash": "0d5d81b9d45c140f6e07b43ed68d31e0ef060d6b4d0431c9b4795997bb35c69d",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "9cc5eca915280827de912d66fbb345f43f80787de309613f3fc53130df5fa7d8",
+                    "hash": "5e84c9905a1816d51c0dfb1eedbfb4d831095ca6c89956c6fe200c2a193cbb8f",
                     "version": 3
                 }
             },
             "ObjectMutation": {
                 "1": {
                     "action": "remove",
                     "hash": "0ee3dd38d6df0fe9a19d848e8f3aaaf13a6ba86afe3406c239caed6da185651a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "4d77ee2650ea29a50e60cf0dcb6cac932b7e6f1aa1e8a927a791ca088e1d07d0",
+                    "hash": "24b7c302f9821afe073534d4ed02c377bd4f7cb691f66ca92b94c38c92dc78c2",
                     "version": 2
                 }
             },
             "ObjectNotReady": {
                 "1": {
                     "action": "remove",
                     "hash": "88207988639b11eaca686b6e079616d9caecc3dbc2a8112258e0f39ee5c3e113",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "07cad6b7fbf4dc9f02ec5857dd4ab4c224fc2da540062a55835eb85df31e7fe8",
+                    "hash": "be7001fea1c819ced4c14e6b3a32b59ee11f773d8b23cf42c2f228e782b631b8",
                     "version": 2
                 }
             },
             "OnDiskBlobDeposit": {
                 "1": {
                     "action": "remove",
                     "hash": "5efc230c1ee65c4626d334aa69ed458c796c45265e546a333844c6c2bcd0e6b0",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6f8f03f6bf76407b8f34aba12970d037c2a59ec3858feee8f8a3234ebe3a744d",
+                    "hash": "adc890e6c70334b46f49fff6b4f22d6aa9f13981b4f6ecd16a0f2910ed69da1b",
                     "version": 2
                 }
             },
             "OutputHistory": {
                 "1": {
                     "action": "remove",
                     "hash": "4ec6e6efd86a972b474251885151bdfe4ef262562174605e8ab6a8abba1aa867",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b6e3d6ca02441af981df1c83bb3ccf05e8221e8da3fb369596190c32ee547f12",
+                    "hash": "425ad1c14348e51a2ec0eb82f1ef86b8fbc63e282e4c511023d6c2d644e3bd83",
                     "version": 2
                 }
             },
             "OutputPolicyExecuteCount": {
                 "1": {
                     "action": "remove",
                     "hash": "6bb24b3b35e19564c43b838ca3f46ccdeadb6596511917f2d220681a378e439d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "124e48961e0a2ffe9b8ce2aca7244e5c87d3a31debaedfc03c4edc721bb1a86c",
+                    "hash": "5bce0120ba3b7cbbe08b28bb92bf035215e66232c36899637b8a3f84300747e3",
                     "version": 2
                 }
             },
             "OutputPolicyExecuteOnce": {
                 "1": {
                     "action": "remove",
                     "hash": "32a40fc9966b277528eebc61c01041f3a5447417731954abdaffbb14dabc76bb",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "429110a31e6a1b91e228e1ce9006607bf6ca3e8ce4c4005c82754b089492ec80",
+                    "hash": "11e2ed5f7fc4bfc701c592352c5377911b0496454c42995c428333ca7ce635c5",
                     "version": 2
                 }
             },
             "PandasDataframeObject": {
                 "1": {
                     "action": "remove",
                     "hash": "35058924b3de2e0a604a92f91f4dd2e3cc0dac80c219d34f360e7cedd52f5f4c",
@@ -915,15 +915,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "66729d4ba7a92210d45c5a5c24fbdb4c8e58138a515a7bdb71ac8f6e8b868544",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "30e79bc3df2f7d99d8bca7e58f2d93ab24fc766ce723d985142cf7adee4cc57a",
+                    "hash": "daf3629fb7d26f41f96cd7f9200d7327a4b74d800b3e02afa75454d11bd47d78",
                     "version": 3
                 }
             },
             "PandasSeriesObject": {
                 "1": {
                     "action": "remove",
                     "hash": "2a0d8a55f1c27bd8fccd276cbe01bf272c40cab10417d7027273983fed423caa",
@@ -932,147 +932,147 @@
                 "2": {
                     "action": "remove",
                     "hash": "cb05a714f75b1140a943f56a3622fcc0477b3a1f504cd545a98510959ffe1528",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "96942949c5a7be48891f84f95b046148bf3e5213b586012071f637c488115ac0",
+                    "hash": "4747a220d1587e99e6ac076496a2aa7217e2700205ac80fc24fe4768a313da78",
                     "version": 3
                 }
             },
             "PartialSyftObject": {
                 "1": {
                     "action": "remove",
                     "hash": "008917584d8e1c09015cdbef02f59c0622f48e0618877c1b44425c8846befc13",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "1254e629e855f017511f60a10f249bd266a018c446b8533b58fcbbb7bb63c29e",
+                    "hash": "385ef254e4a0c9e68fd750f2bb47f8f9c46dbd2ac9f00f535f843f19f1cf6032",
                     "version": 2
                 }
             },
             "Plan": {
                 "1": {
                     "action": "remove",
                     "hash": "a0bba2b7792c9e08c453e9e256f0ac6e6185610726566bcd50b057ae83b42d9a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f8e623e1887df2c0051caf9e06820e6603148e8ae688460e10a6f4b2dd405e9d",
+                    "hash": "67be9b8933b5bec20090727a7b1a03216f874dcc254975481ac62a5a1e9c0c1e",
                     "version": 2
                 }
             },
             "Project": {
                 "1": {
                     "action": "remove",
                     "hash": "ec5b7ac1c92808e266f06b175c6ebcd50be81777ad120c02ce8c6074d0004788",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "7a874f5d00996d9781f1e448c1a6fb766aa236fb9b468e8f0f5fdee76a047791",
+                    "hash": "4b7f5d0bec9a1ba7863679b85425f1918745e9dad21476078c19f7257d5f38a3",
                     "version": 2
                 }
             },
             "ProjectMessage": {
                 "1": {
                     "action": "remove",
                     "hash": "55a3a5171b6949372b4125cc461bf39bc998565e07703804fca6c7ef99695ae4",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "283dd47bd664db581928ffe33e7f93d81100351461976a7d662541837b8490b9",
+                    "hash": "086513fa450d185b5040b75dc034f4e219c3214677674efa4b4263fda140ce2a",
                     "version": 2
                 }
             },
             "ProjectPoll": {
                 "1": {
                     "action": "remove",
                     "hash": "b0ac8f1d9c06997374ddbc33fdf1d0af0da15fdb6899f52d91a8574106558964",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "900f51fcd1cdac2b34f74038a33229273446e211a310138f8af7ac3683094e92",
+                    "hash": "90522301ab056881d79a066d824dcce6d7836f2555ac4182bbafe75bea5a5fa7",
                     "version": 2
                 }
             },
             "ProjectRequest": {
                 "1": {
                     "action": "remove",
                     "hash": "514d189df335c68869eea36befcdcafec74bdc682eaf18871fe879e26da4dbb6",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "4051700e64dd28f6a928fd3e4cbaf989abf0e2345b7c086f3aa8917e30c756b2",
+                    "hash": "7d7f74f39333bef10ac37f49b5783dc9ba9b5783d2bec814d7de2d2025bcce01",
                     "version": 2
                 }
             },
             "ProjectRequestResponse": {
                 "1": {
                     "action": "remove",
                     "hash": "d4c360e845697a0b24695143d0781626cd344cfde43162c90ae90fe67e00ae21",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "31c346849ab131d6eddb109054a19118c6937b20586fe54f5c7a0a50ecc017e4",
+                    "hash": "b29309054cd9f9e6a3f00724453f90510076de0bf03ff300fc83670a1721b272",
                     "version": 2
                 }
             },
             "ProjectSubmit": {
                 "1": {
                     "action": "remove",
                     "hash": "0374b37779497d7e0b2ffeabc38d35bfbae2ee762a7674a5a8af75e7c5545e61",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "70fa24856ecb0df109736e0cb8478cac335801413ca191aa9ced34f5ea3e5189",
+                    "hash": "0af1abb9ac899c0bc133971f75d17be8260b80a2df9fe191965db431bb6fd910",
                     "version": 2
                 }
             },
             "ProjectThreadMessage": {
                 "1": {
                     "action": "remove",
                     "hash": "1118e935792e8e54103dbf91fa33edbf192a7767d2b1d4526dfa7d4a643cde2e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "a7454aace740674583226e4f1c1e48284d4ffbc125c196c919d449e2fe8b52a7",
+                    "hash": "319007e1173c1558917cbdf25171da70514fe0afaae49c7d099aca6f2ec87015",
                     "version": 2
                 }
             },
             "PythonConnection": {
                 "1": {
                     "action": "remove",
                     "hash": "011946fc9af0a6987f5c7bc9b0208b2fae9d65217531430bced7ba542788da1a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "eb479c671fc112b2acbedb88bc5624dfdc9592856c04c22c66410f6c863e1708",
+                    "hash": "b7bb677f60333d3ab1e927d0be44725667ce75620c2861c706cbca022cfae1fc",
                     "version": 2
                 }
             },
             "PythonNodeRoute": {
                 "1": {
                     "action": "remove",
                     "hash": "15711e6e7a1ef726c8e8b5c35a6cb2d30b56ba5213cba489524bf63489e136cf",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "3eca5767ae4a8fbe67744509e58c6d9fb78f38fa0a0f7fcf5960ab4250acc1f0",
+                    "hash": "375b36756047fa0e926e5461320960a5c48546ef8cc0c6bb4ff620c7084dc4fc",
                     "version": 2
                 }
             },
             "QueueItem": {
                 "1": {
                     "action": "remove",
                     "hash": "5aa94681d9d0715d5b605f9625a54e114927271378cf2ea7245f85c488035e0b",
@@ -1086,87 +1086,87 @@
                 "3": {
                     "action": "remove",
                     "hash": "3495f406d2c97050ce86be80c230f49b6b846c63b9a9230cbd6631952f2bad0f",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "96b0ab4ae935558cd391b86e923f8c7e172b3c27b288c0133197bdc41bd7e19f",
+                    "hash": "c37bc1c6303c467050ce4f8faa088a2f66ef1781437ffe34f15aadf5477ac25b",
                     "version": 4
                 }
             },
             "RemoteConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "ad7bc4780a8ad52e14ce68601852c93d2fe07bda489809cad7cae786d2461754",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0269311d0a524c1f2c565ffd1c9d0da4a4cb4880f98b44cb7d3b76312f5c9f98",
+                    "hash": "9d6b8ddb258815b5660f2288164a3a87f68a0e6849493eb48c87da1509b6ab27",
                     "version": 2
                 }
             },
             "ReplyNotification": {
                 "1": {
                     "action": "remove",
                     "hash": "34b2ad522f7406c2486573467d9c7acef5c1063a0d9f2177c3bda2d8c4f87572",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "bc3a15f754ea23a1b6dfe1612ee47a361864c820c507b5644b3fada92bd266e7",
+                    "hash": "7bea00170bce350ea1c3a1a16cfb31264e70da9da2fd6f2128852c479e793b60",
                     "version": 2
                 }
             },
             "Request": {
                 "1": {
                     "action": "remove",
                     "hash": "e054307eeb7f13683cde9ce7613d5ca2925a13fff7c345b1c9f729a12c955f90",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "b8be498ac1e0a7df5e683540ed2a62778faff11404f45f660b3e092e9ed0e37d",
+                    "hash": "72bb2fcf520d8ca31fc5fd9b1730a8839648b7f446bcc9f2b6d80e4c635feb59",
                     "version": 2
                 }
             },
             "RequestInfo": {
                 "1": {
                     "action": "remove",
                     "hash": "b76075c138afc0563ce9ac7f6b1131f048951f7486cd516c02736dc1a2a23639",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "836d768fe0d3d5e134dbcafdff8542a97242ded1b4df1c76dff2ca0f87b28d71",
+                    "hash": "fd127bb4f64b4d04122d31b27b46f712a6f3c9518b2e6df0b140247bab115789",
                     "version": 2
                 }
             },
             "RequestInfoFilter": {
                 "1": {
                     "action": "remove",
                     "hash": "7103abdc464ae71bb746410f5730f55dd8ed82268aa32bbb0a69e0070488a669",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "8dabbabdac26c5223579dabe54f7b1b4220b0e49fa6e401fdb09768bca6b49d5",
+                    "hash": "c8773edca83f068b5a7b7ebe7f5e70ff8df65915564cead695b4528203f750a3",
                     "version": 2
                 }
             },
             "SQLiteStoreConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "b656b26c14cf4e97aba702dd62a0927aec7f860c12eed512c2c688e1b7109aa5",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "194391d5e90030ad2fe46e7a810ee55dddaa9a1f831667bcdad6e2363c1996fa",
+                    "hash": "e2027eacb8db772fadc506e5bbe797a3fd24175c18b98f79f412cc86ee300f2e",
                     "version": 2
                 }
             },
             "SeaweedFSBlobDeposit": {
                 "1": {
                     "action": "remove",
                     "hash": "382a9ac178deed2a9591e1ebbb39f265cbe67027fb93a420d473a4c26b7fda11",
@@ -1175,15 +1175,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "07d84a95324d95d9c868cd7d1c33c908f77aa468671d76c144586aab672bcbb5",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "05e61e6328b085b738e5d41c0781d87852d44d218894cb3008f5be46e337f6d8",
+                    "hash": "ba3715305ea320413ca5a8780d0d02aeeb5cf3be2445aa274496c539ac787425",
                     "version": 3
                 }
             },
             "SeaweedSecureFilePathLocation": {
                 "1": {
                     "action": "remove",
                     "hash": "5724a38b1a92b8a55da3d9cc34a720365a6d0c32683acda630fc44067173e201",
@@ -1192,75 +1192,75 @@
                 "2": {
                     "action": "remove",
                     "hash": "5fd63fed2a4efba8c2b6c7a7b5e9b5939181781c331230896aa130b6fd558739",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "12547e03e48b48c44f13720792db9302726c92f33ecc5374bd92ff6f2d733adf",
+                    "hash": "a986f0e990db9c7ada326b2cca828fa146349a303e674fa48ee4b45702bedc14",
                     "version": 3
                 }
             },
             "SecureFilePathLocation": {
                 "1": {
                     "action": "remove",
                     "hash": "7febc066e2ee5a3a4a891720afede3f5c155cacc0557662ac4d04bf67b964c6d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "e4e18e793f25c1ba8eb32849dafc3b85aa1572ebd9a7339ea8776452777d5b7c",
+                    "hash": "f1a9510992d60e037c0016574225b8f61433b87bb65bc3320800b1c70e54982c",
                     "version": 2
                 }
             },
             "ServiceConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "ca91f59bf045d949d82860f7d52655bfbede4cf6bdc5bae8f847f08a16f05d74",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "4c79a399bbbd8571b712bdb957ff3bc4903aae59cc06bd584c248860dfdab9fe",
+                    "hash": "5945f4f7347baeae0a7f5386d71982a16d6be8ab0c1caa2b10c28d282e66b1ea",
                     "version": 2
                 }
             },
             "SignedSyftAPICall": {
                 "1": {
                     "action": "remove",
                     "hash": "e66a116de2fa44ebdd0d4c2d7d5a047dedb555fd201a0f431cd8017d9d33a61d",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "7a3bdede247c347196d5ced8217d2d3849e91a02dc5fd1c98c4a8bcac98480e4",
+                    "hash": "6cd89ed24027ed94b3e2bb7a07e8932060e07e481ceb35eb7ee4d2d0b6e34f43",
                     "version": 2
                 }
             },
             "StoreConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "17de8875cf590311ddb042140347ffc79d4a85028e504dad178ca4e1237ec861",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "6df61455f637affc477cf7ded7206009b414269b497a586b5d3374368e9ea602",
+                    "hash": "3f6c9a967a43557bf88caab87e5d1b9b14ea240bfd5bd6a1a313798e4ee2552b",
                     "version": 2
                 }
             },
             "SubmitRequest": {
                 "1": {
                     "action": "remove",
                     "hash": "96b4ec12beafd9d8a7c97399cb8a23dade4db16d8f521be3fe7b8fec99db5161",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "33c6aa318e2d7f3d56897e61c7370a5483bf5a37f25cfa0041ff3bf84949aee2",
+                    "hash": "796b297342793995b8dd87e8feb420e8601dee3b704b7a21a93326661b227ea8",
                     "version": 2
                 }
             },
             "SubmitUserCode": {
                 "2": {
                     "action": "remove",
                     "hash": "9b29e060973a3de8d3564a2b7d2bb5c53745aa445bf257576994b613505d7194",
@@ -1269,75 +1269,75 @@
                 "3": {
                     "action": "remove",
                     "hash": "a29160c16d2e2620800d42cdcd9f3637d063a570c477a5d05217a2e64b4bb396",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "3c5c8627e4f7cca64c1249eea52e7c46171fd4882f76c83e9fa8a1ea7e828b9c",
+                    "hash": "755721313ee8a7148c513c1d0b85324cfcbec14297887daf84ac4c0c5f468a4f",
                     "version": 4
                 }
             },
             "SubmitUserPolicy": {
                 "1": {
                     "action": "remove",
                     "hash": "96f7f39279fadc70c569b8d48ed4d6420a8132db51e37466d272fda19953554b",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "354df4734594f6bc3b58b26c0b60592f454c750e49c00781fc15448dd65a4fb4",
+                    "hash": "971f4aa69bf68e7a876b0b1cb85ba7d4213212baf7eeaa24bab0a70f18841497",
                     "version": 2
                 }
             },
             "SyftAPI": {
                 "1": {
                     "action": "remove",
                     "hash": "2bba1d9fcf677a58e35bf903de3da22ee4913af138aa3012af9c46b3609579cd",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "8d24945c5d62c9a910dbe6b925064532db4f351ab7f3eabf1fb454a9e460f7ab",
+                    "hash": "8f3ff426794df07cbeab441ff545fb896f27897df88b11ec949ec05726a41747",
                     "version": 2
                 }
             },
             "SyftAPICall": {
                 "1": {
                     "action": "remove",
                     "hash": "014bd1d0933f6070888a313edba239170759de24eae49bf2374c1be4dbe2b4d7",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "f18183e178a0b5709a2800a7d88f9eef25afefe64d6c646938fec6c5aacd296f",
+                    "hash": "bc686b6399e058b21472d61fe56df1f0de0785219f52c7306dd5ab8bae863d89",
                     "version": 2
                 }
             },
             "SyftAPIData": {
                 "1": {
                     "action": "remove",
                     "hash": "db101a75227e34750d7056785a1e87bb2e8ad6604f19c372d0cb6aa437243bf5",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "931f6019fe66e35eebfe2e0b3c20d7354e2222b4e51a7b60ae9a54c581a77d6e",
+                    "hash": "b303d322c7e6da6e003e5d92a27d86acce512228a9dd62c1ab48824702055bf0",
                     "version": 2
                 }
             },
             "SyftImageRegistry": {
                 "1": {
                     "action": "remove",
                     "hash": "dc83910c91947e3d9eaa3e6f8592237448f0408668c7cca80450b5fcd54722e1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "862410fcf514a41ee13273d9540a245ed79e26bb82a0acfe2ad48accc3af1bef",
+                    "hash": "3ceacaa164246323be86ccde0881dd42ee6275684e147095e1d0de7b007ae066",
                     "version": 2
                 }
             },
             "SyftLog": {
                 "1": {
                     "action": "remove",
                     "hash": "bd3f62b8fe4b2718a6380c8f05a93c5c40169fc4ab174db291929298e588429e",
@@ -1346,27 +1346,27 @@
                 "2": {
                     "action": "remove",
                     "hash": "d3ce45794da2e6c4b0cef63b98a553525af50c5d9db42d3d64caef3e7d22b4a9",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "8964d48238672e0e5d5db6b932cda4ee8eb77581949ab3f7a38a05b1efec13b7",
+                    "hash": "6417108288ab4cf090ee2d548fb44b7de7f60b20a33876e5333ab4cabcc5b5df",
                     "version": 3
                 }
             },
             "SyftObjectMigrationState": {
                 "1": {
                     "action": "remove",
                     "hash": "d3c8126bc15dae4dd243bb035530e3f56cd9e433d403dd6b5f3b45face6d281f",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0b00b9236ae35820733041dc0f4f3956d85d75108a94dba0653aa5948436bd8a",
+                    "hash": "187e6b6619f56fdaf2fbe150a0ec561b1d6a7dbfbc6132257951844206319c79",
                     "version": 2
                 }
             },
             "SyftObjectRetrieval": {
                 "2": {
                     "action": "remove",
                     "hash": "d9d7a7e1b8843145c9687fd013c9223700285886073547734267e91ac53e0996",
@@ -1375,77 +1375,77 @@
                 "3": {
                     "action": "remove",
                     "hash": "952958e9afae007bef3cb89aa15be95dddc4c310e3a8ce4191576f90ac6fcbc8",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "fe151e6fceaafc71c9189d07aed077dc0477bea6a8d7f3c3ace9098ed3161f6b",
+                    "hash": "dd6527e200e7d21e5f4166b2874daf6aeb0b41fafeb8f07f96b675c8625d4cf7",
                     "version": 4
                 }
             },
             "SyftWorker": {
                 "1": {
                     "action": "remove",
                     "hash": "0d5b367162f3ce55ab090cc1b49bd30e50d4eb144e8431eadc679bd0e743aa70",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "ad19971aabbdf6d032fba708357eb0f0d0bd59f993c58b3e36a1b7ca04332453",
+                    "hash": "257395af556b1b2972089150c0e3280479a5ba12779d012651eee2f6870e7133",
                     "version": 2
                 }
             },
             "SyftWorkerImage": {
                 "1": {
                     "action": "remove",
                     "hash": "2a9585b6a286e24f1a9f3f943d0128730cf853edc549184dc1809d19e1eec54b",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "1063e826436e24707eef3f37dbc15f8008ca038fc3f02ad489a49248c8666ba3",
+                    "hash": "4a6169ba1f50fdb73ac45500dd02b9d164ef239f13800c0da0ed5f8aed7cde1a",
                     "version": 2
                 }
             },
             "SyncState": {
                 "1": {
                     "action": "add",
-                    "hash": "a0616775ec8ef0629e2d91e0df9cc4237ea3674727eda1ce367f1897ee35767d",
+                    "hash": "b91ed9a9eb8ac7e2fadafd9376d8adefc83845d2f29939b30e95ebe94dc78cd9",
                     "version": 1
                 }
             },
             "SyncStateItem": {
                 "1": {
                     "action": "add",
-                    "hash": "4dbfa0813f5a3f7be0b36249ff2d67e395ad7c9e138c5a122fc7342b8dcc4b92",
+                    "hash": "cde09be2cfeca4246d001f3f28c00d8647a4506641104e5dc647f136a64fd06e",
                     "version": 1
                 }
             },
             "TwinObject": {
                 "1": {
                     "action": "remove",
                     "hash": "c42455586b43724a7421becd99122b787a129798daf6081e96954ecaea228099",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "c863c24d4ec1989ce2a0547f9b9152a2a61b24386b38ccd37f0aeae91ce80e41",
+                    "hash": "937fded2210d9b792cbe7a99879180e396902fe7b684cd6a14a651db8b9ca2c9",
                     "version": 2
                 }
             },
             "User": {
                 "2": {
                     "action": "remove",
                     "hash": "ded970c92f202716ed33a2117cf541789f35fad66bd4b1db39da5026b1d7d0e7",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "ac5179da4b09332cade6aeedd1c59b506ddfe932ee79b9bb2c087dca24391342",
+                    "hash": "7f5e148674564f2c9c75e19fd2ea17001fbef9e2ba5e49a7e92a8b8b6098f340",
                     "version": 3
                 }
             },
             "UserCode": {
                 "1": {
                     "action": "remove",
                     "hash": "e14c22686cdc7d1fb2b0d01c0aebdea37e62a61b051677c1d30234214f05cd42",
@@ -1459,34 +1459,34 @@
                 "3": {
                     "action": "remove",
                     "hash": "90fcae0f556f375ba1e91d2e345f57241660695c6e2b84c8e311df89d09e6c66",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "0a7181cd5f76800b6566175ffa7276d0cf38c4ddc5110114430147dfc8bfdb2a",
+                    "hash": "84ef96946a18e2028d71e125a7a4b8bed2c9cba3c5a2612634509790506e5b9c",
                     "version": 4
                 }
             },
             "UserCodeExecutionOutput": {
                 "1": {
                     "action": "add",
-                    "hash": "deafafb72d07d724690aaa2fe742379f8e9b3531d9c33f6a8683ee90b462e353",
+                    "hash": "d20e83362df8a5d2d2e7eb26a2c5723739f9cfbe4c0272d3ae7e37a34bbe5317",
                     "version": 1
                 }
             },
             "UserCodeExecutionResult": {
                 "1": {
                     "action": "remove",
                     "hash": "49c32e85e78b7b189a7f13b7e26115ef94fcb0b60b578adcbe2b95e289f63a6e",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "0f4b96ae01b360b7b5ba99f6bd34aaf2da368ff56075bee8137d8c9a82bcec02",
+                    "hash": "05c457f502f7a257a4d5287633d18bbd3cb4ba565afb6a69ac0822c55408a55e",
                     "version": 2
                 }
             },
             "UserCodeStatusChange": {
                 "1": {
                     "action": "remove",
                     "hash": "4f5b405cc2b3976ed8f7018df82e873435d9187dff15fa5a23bc85a738969f3f",
@@ -1495,144 +1495,144 @@
                 "2": {
                     "action": "remove",
                     "hash": "d83e0905ae882c824ba8fbbf455cd3881906bf8b2ebbfff07bcf471ef869cedc",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "6a743ac25193006491f53e0ab697a1391a8f19441d6fa6d6b67d4d5745808b12",
+                    "hash": "dd79f0f4d8cc7c95120911a0a5d9264cc6e65813bd4ad39f81b756b40c1463e9",
                     "version": 3
                 }
             },
             "UserCodeStatusCollection": {
                 "1": {
                     "action": "add",
-                    "hash": "07481d543ec3131e759822710ab1714d525c0a16b20ebe4a2119f558ba22c125",
+                    "hash": "8d8bae10ee1733464272031e7de6fc783668885206fa448c9f7cd8e8cfc7486a",
                     "version": 1
                 }
             },
             "UserCreate": {
                 "2": {
                     "action": "remove",
                     "hash": "2540188c5aaea866914dccff459df6e0f4727108a503414bb1567ff6297d4646",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "70a0d3a701aca47f58009d48c94e314adc464e5429af6794b5770a1163ddfdda",
+                    "hash": "26f9467d60b9b642e0a754e9fc028c66a139925fa7d9fac52e5a1e9afdf1387b",
                     "version": 3
                 }
             },
             "UserPolicy": {
                 "1": {
                     "action": "remove",
                     "hash": "c69b17b1d96cace8b45da6d9639165f2da4aa7ff156b6fd922ac217bf7856d8a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "9a5ef3d6ece1321ad59c20f2dda08564696e1dd8d017b268ffd70c2958671cad",
+                    "hash": "6f201caff6457bd036e614a58aedb9fad6a3947b7d4d7965ccfdb788b6385262",
                     "version": 2
                 }
             },
             "UserPrivateKey": {
                 "1": {
                     "action": "remove",
                     "hash": "7cb196587887f0f3bffb298dd9f3b88509e9b2748792bf8dc03bdd0d6b98714a",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "7e99d928122dd7546c94893314f393956c29b8c8d605f62bc99429972f2ffd8e",
+                    "hash": "0917d22c7cbd3531be6365570952557aed054332d1ec89720213f218e4202ae0",
                     "version": 2
                 }
             },
             "UserSearch": {
                 "1": {
                     "action": "remove",
                     "hash": "69d1e10b81c8a4143cf70e4f911d8562732af2458ebbc455ca64542f11373dd1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "78d4149c8b1af8510755341fc369eae83d7f67c6b771b50af7f9b3c9b6e7b7aa",
+                    "hash": "6fd7bc05cfad5724d81b1122ddf70c6ea09e6fa77fa374c0b68e0d42e0781088",
                     "version": 2
                 }
             },
             "UserUpdate": {
                 "2": {
                     "action": "remove",
                     "hash": "32cba8fbd786c575f92e26c31384d282e68e3ebfe5c4b0a0e793820b1228d246",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "a7333af6252bf92ccd913bb23ddc4c0b0c63f8838277d7ebad406be92fa019d2",
+                    "hash": "fd73429a86cc4fe4db51198ae380a18b9a7e42885701efad42bc2ef1b28c04de",
                     "version": 3
                 }
             },
             "UserView": {
                 "2": {
                     "action": "remove",
                     "hash": "e410de583bb15bc5af57acef7be55ea5fc56b5b0fc169daa3869f4203c4d7473",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "ac21f70f7bcbc6cadd7b07949e66b66bca31aa5c1fb28196ae38d22dc05eb444",
+                    "hash": "4487e0e96c6cdef771d751bca4e14afac48a17ba7aa03d956521e3d757ab95f5",
                     "version": 3
                 }
             },
             "UserViewPage": {
                 "1": {
                     "action": "remove",
                     "hash": "16dac6209b19a934d286ef1efa874379e0040c324e71023c57d1bc6d2d367171",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "1383d83f202e53490d03049685c1052385ecde4ea6d4b34d4917d08749e02e44",
+                    "hash": "0f9d54e606f9a4af73249dd4012baa11fcb7c1e60cce70c01ee48bb63411d6fe",
                     "version": 2
                 }
             },
             "UsersCodeHistoriesDict": {
                 "1": {
                     "action": "remove",
                     "hash": "5e1f389c4565ee8558386dd5c934d81e0c68ab1434f86bb9065976b587ef44d1",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "863280e2a39de8f50293d54dd9798a0568a2204418fe0bd776b5ea3dcc43e99a",
+                    "hash": "9cb9a7e1e5c5e294cd019bdb9824180fa399810e7d57db285823157c91ee7d76",
                     "version": 2
                 }
             },
             "VeilidConnection": {
                 "1": {
                     "action": "add",
-                    "hash": "c1796e7b01c9eae0dbf59cfd5c2c2f0e7eba593e0cea615717246572b27aae4b",
+                    "hash": "c5ed1cfa9b7b146dbce7f1057f6e81e89715b5addfd4d4c4d53c415e450373a5",
                     "version": 1
                 }
             },
             "VeilidNodeRoute": {
                 "1": {
                     "action": "add",
-                    "hash": "eadf99eac62574cdda61290c44c564a3ba22faebf27a661da4fc4a2643760376",
+                    "hash": "4797413e3144fce7bccc290db64f1750e8c09f75d5e1aba6e19d29f921a21074",
                     "version": 1
                 }
             },
             "WorkerPool": {
                 "1": {
                     "action": "remove",
                     "hash": "250699eb4c452fc427995353d5c5ad6245fb3e9fdac8814f8348784816a0733b",
                     "version": 1
                 },
                 "2": {
                     "action": "add",
-                    "hash": "1b81621b7c03eacfe8369c30bbc97967acef6b5d29a3c67d5f8ad81b49556dac",
+                    "hash": "3fa999bb789b9557939dea820ddcb6c68224822581971a3c3861da3b781d6c25",
                     "version": 2
                 }
             },
             "WorkerSettings": {
                 "1": {
                     "action": "remove",
                     "hash": "0dcd95422ec8a7c74e45ee68a125084c08f898dc94a13d25fe5a5fd0e4fc5027",
@@ -1641,15 +1641,15 @@
                 "2": {
                     "action": "remove",
                     "hash": "d623a8a0d6c83b26ba49686bd8be10eccb126f54626fef334a85396c3b8a8ed6",
                     "version": 2
                 },
                 "3": {
                     "action": "add",
-                    "hash": "20c9e19d8084a87130e173d09d3e9ebaecd3127c455702471eac764d37912a43",
+                    "hash": "d42ed88ba674e8e1ceefa61b0f9fd76400d965e52ab000b2c7f0ae5f9d26d109",
                     "version": 3
                 }
             },
             "ZMQClientConfig": {
                 "1": {
                     "action": "remove",
                     "hash": "e6054969b495791569caaf33239039beae3d116e1fe74e9575467c48b9007c45",
@@ -1658,14 +1658,14 @@
                 "3": {
                     "action": "remove",
                     "hash": "91ce5953cced58e12c576aa5174d5ca0c91981b01cf42edd5283d347baa3390b",
                     "version": 3
                 },
                 "4": {
                     "action": "add",
-                    "hash": "d8761747473ef2af59a7889ab0ea0f69f78a841a9f0cf9fad8260e9c570211d5",
+                    "hash": "94f4243442d5aa7d2eb48e661a2cbf9d7c1d6a22035a3783977bdfae4a571142",
                     "version": 4
                 }
             }
         }
     }
 }
```

### Comparing `syft-0.8.6/src/syft/serde/array.py` & `syft-0.8.6b1/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/arrow.py` & `syft-0.8.6b1/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/deserialize.py` & `syft-0.8.6b1/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/lib_permissions.py` & `syft-0.8.6b1/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/lib_service_registry.py` & `syft-0.8.6b1/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/mock.py` & `syft-0.8.6b1/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/recursive.py` & `syft-0.8.6b1/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/recursive_primitives.py` & `syft-0.8.6b1/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/serializable.py` & `syft-0.8.6b1/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/signature.py` & `syft-0.8.6b1/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/serde/third_party.py` & `syft-0.8.6b1/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/action_data_empty.py` & `syft-0.8.6b1/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/action_graph.py` & `syft-0.8.6b1/src/syft/service/action/action_graph.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/action_graph_service.py` & `syft-0.8.6b1/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/action_object.py` & `syft-0.8.6b1/src/syft/service/action/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/action_permissions.py` & `syft-0.8.6b1/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/action_service.py` & `syft-0.8.6b1/src/syft/service/action/action_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/action_store.py` & `syft-0.8.6b1/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/action_types.py` & `syft-0.8.6b1/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/numpy.py` & `syft-0.8.6b1/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/pandas.py` & `syft-0.8.6b1/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/plan.py` & `syft-0.8.6b1/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/action/verification.py` & `syft-0.8.6b1/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/blob_storage/remote_profile.py` & `syft-0.8.6b1/src/syft/service/blob_storage/remote_profile.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/blob_storage/service.py` & `syft-0.8.6b1/src/syft/service/blob_storage/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/blob_storage/stash.py` & `syft-0.8.6b1/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code/code_parse.py` & `syft-0.8.6b1/src/syft/service/code/code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code/status_service.py` & `syft-0.8.6b1/src/syft/service/code/status_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code/user_code.py` & `syft-0.8.6b1/src/syft/service/code/user_code.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code/user_code_parse.py` & `syft-0.8.6b1/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code/user_code_service.py` & `syft-0.8.6b1/src/syft/service/code/user_code_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code/user_code_stash.py` & `syft-0.8.6b1/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code/utils.py` & `syft-0.8.6b1/src/syft/service/code/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code_history/code_history.py` & `syft-0.8.6b1/src/syft/service/code_history/code_history.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code_history/code_history_service.py` & `syft-0.8.6b1/src/syft/service/code_history/code_history_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.6b1/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/context.py` & `syft-0.8.6b1/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/data_subject/data_subject.py` & `syft-0.8.6b1/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.6b1/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.6b1/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.6b1/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/dataset/dataset.py` & `syft-0.8.6b1/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/dataset/dataset_service.py` & `syft-0.8.6b1/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.6b1/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/enclave/enclave_service.py` & `syft-0.8.6b1/src/syft/service/enclave/enclave_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/job/job_service.py` & `syft-0.8.6b1/src/syft/service/job/job_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/job/job_stash.py` & `syft-0.8.6b1/src/syft/service/job/job_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/log/log.py` & `syft-0.8.6b1/src/syft/service/log/log.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/log/log_service.py` & `syft-0.8.6b1/src/syft/service/log/log_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/log/log_stash.py` & `syft-0.8.6b1/src/syft/service/log/log_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/metadata/metadata_service.py` & `syft-0.8.6b1/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/metadata/migrations.py` & `syft-0.8.6b1/src/syft/service/metadata/migrations.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/metadata/node_metadata.py` & `syft-0.8.6b1/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/network/network_service.py` & `syft-0.8.6b1/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/network/node_peer.py` & `syft-0.8.6b1/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/network/routes.py` & `syft-0.8.6b1/src/syft/service/network/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/notification/email_templates.py` & `syft-0.8.6b1/src/syft/service/notification/email_templates.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/notification/notification_service.py` & `syft-0.8.6b1/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/notification/notification_stash.py` & `syft-0.8.6b1/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/notification/notifications.py` & `syft-0.8.6b1/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/notifier/notifier.py` & `syft-0.8.6b1/src/syft/service/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/notifier/notifier_service.py` & `syft-0.8.6b1/src/syft/service/notifier/notifier_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/notifier/notifier_stash.py` & `syft-0.8.6b1/src/syft/service/notifier/notifier_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/notifier/smtp_client.py` & `syft-0.8.6b1/src/syft/service/notifier/smtp_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/object_search/migration_state_service.py` & `syft-0.8.6b1/src/syft/service/object_search/migration_state_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/object_search/object_migration_state.py` & `syft-0.8.6b1/src/syft/service/object_search/object_migration_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/output/output_service.py` & `syft-0.8.6b1/src/syft/service/output/output_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/policy/policy.py` & `syft-0.8.6b1/src/syft/service/policy/policy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/policy/policy_service.py` & `syft-0.8.6b1/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.6b1/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/project/project.py` & `syft-0.8.6b1/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/project/project_service.py` & `syft-0.8.6b1/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/project/project_stash.py` & `syft-0.8.6b1/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/queue/base_queue.py` & `syft-0.8.6b1/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/queue/queue.py` & `syft-0.8.6b1/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/queue/queue_service.py` & `syft-0.8.6b1/src/syft/service/queue/queue_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/queue/queue_stash.py` & `syft-0.8.6b1/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/queue/zmq_queue.py` & `syft-0.8.6b1/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/request/request.py` & `syft-0.8.6b1/src/syft/service/request/request.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/request/request_service.py` & `syft-0.8.6b1/src/syft/service/request/request_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/request/request_stash.py` & `syft-0.8.6b1/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/response.py` & `syft-0.8.6b1/src/syft/service/response.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/service.py` & `syft-0.8.6b1/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/settings/settings.py` & `syft-0.8.6b1/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/settings/settings_service.py` & `syft-0.8.6b1/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/settings/settings_stash.py` & `syft-0.8.6b1/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/sync/diff_state.py` & `syft-0.8.6b1/src/syft/service/sync/diff_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/sync/sync_service.py` & `syft-0.8.6b1/src/syft/service/sync/sync_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/sync/sync_stash.py` & `syft-0.8.6b1/src/syft/service/sync/sync_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/sync/sync_state.py` & `syft-0.8.6b1/src/syft/service/sync/sync_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/user/user.py` & `syft-0.8.6b1/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/user/user_roles.py` & `syft-0.8.6b1/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/user/user_service.py` & `syft-0.8.6b1/src/syft/service/user/user_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
             else:
                 return SyftError(
                     message=f"As a {context.role}, you are not allowed to edit {user.role} to {user_update.role}"
                 )
 
         edits_non_role_attrs = any(
             getattr(user_update, attr) is not Empty
-            for attr in user_update.to_dict()
+            for attr in user_update.dict()
             if attr != "role"
         )
 
         if (
             edits_non_role_attrs
             and user.verify_key != context.credentials
             and ServiceRoleCapability.CAN_MANAGE_USERS not in context.capabilities()
```

### Comparing `syft-0.8.6/src/syft/service/user/user_stash.py` & `syft-0.8.6b1/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/veilid/veilid_service.py` & `syft-0.8.6b1/src/syft/service/veilid/veilid_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/warnings.py` & `syft-0.8.6b1/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/image_identifier.py` & `syft-0.8.6b1/src/syft/service/worker/image_identifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/image_registry.py` & `syft-0.8.6b1/src/syft/service/worker/image_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/image_registry_service.py` & `syft-0.8.6b1/src/syft/service/worker/image_registry_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/image_registry_stash.py` & `syft-0.8.6b1/src/syft/service/worker/image_registry_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/utils.py` & `syft-0.8.6b1/src/syft/service/worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker.py` & `syft-0.8.6b1/src/syft/service/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker_image.py` & `syft-0.8.6b1/src/syft/service/worker/worker_image.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker_image_service.py` & `syft-0.8.6b1/src/syft/service/worker/worker_image_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker_image_stash.py` & `syft-0.8.6b1/src/syft/service/worker/worker_image_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker_pool.py` & `syft-0.8.6b1/src/syft/service/worker/worker_pool.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker_pool_service.py` & `syft-0.8.6b1/src/syft/service/worker/worker_pool_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker_pool_stash.py` & `syft-0.8.6b1/src/syft/service/worker/worker_pool_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker_service.py` & `syft-0.8.6b1/src/syft/service/worker/worker_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/service/worker/worker_stash.py` & `syft-0.8.6b1/src/syft/service/worker/worker_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/blob_storage/__init__.py` & `syft-0.8.6b1/src/syft/store/blob_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.6b1/src/syft/store/blob_storage/on_disk.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.6b1/src/syft/store/blob_storage/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/dict_document_store.py` & `syft-0.8.6b1/src/syft/store/dict_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/document_store.py` & `syft-0.8.6b1/src/syft/store/document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/kv_document_store.py` & `syft-0.8.6b1/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/linked_obj.py` & `syft-0.8.6b1/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/locks.py` & `syft-0.8.6b1/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/mongo_client.py` & `syft-0.8.6b1/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/mongo_codecs.py` & `syft-0.8.6b1/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/mongo_document_store.py` & `syft-0.8.6b1/src/syft/store/mongo_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/store/sqlite_document_store.py` & `syft-0.8.6b1/src/syft/store/sqlite_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/blob_storage.py` & `syft-0.8.6b1/src/syft/types/blob_storage.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/datetime.py` & `syft-0.8.6b1/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/dicttuple.py` & `syft-0.8.6b1/src/syft/types/dicttuple.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/grid_url.py` & `syft-0.8.6b1/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/identity.py` & `syft-0.8.6b1/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/syft_metaclass.py` & `syft-0.8.6b1/src/syft/types/syft_metaclass.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # stdlib
 from typing import Any
+from typing import TypeVar
 from typing import final
 
 # third party
 from pydantic import BaseModel
 from pydantic._internal._model_construction import ModelMetaclass
 
 # relative
 from ..serde.serializable import serializable
 
+_T = TypeVar("_T", bound=BaseModel)
+
 
 class EmptyType(type):
     def __repr__(self) -> str:
         return self.__name__
 
     def __bool__(self) -> bool:
         return False
@@ -21,26 +24,16 @@
 @serializable()
 @final
 class Empty(metaclass=EmptyType):
     pass
 
 
 class PartialModelMetaclass(ModelMetaclass):
-    def __new__(
-        mcs,
-        cls_name: str,
-        bases: tuple[type[Any], ...],
-        namespace: dict[str, Any],
-        *args: Any,
-        **kwargs: Any,
-    ) -> type:
-        cls = super().__new__(mcs, cls_name, bases, namespace, *args, **kwargs)
-
-        if issubclass(cls, BaseModel):
-            for field_info in cls.model_fields.values():
-                if field_info.annotation is not None and field_info.is_required():
-                    field_info.annotation = field_info.annotation | EmptyType
-                    field_info.default = Empty
+    def __call__(cls: type[_T], *args: Any, **kwargs: Any) -> _T:
+        for field_info in cls.model_fields.values():
+            if field_info.annotation is not None and field_info.is_required():
+                field_info.annotation = field_info.annotation | EmptyType
+                field_info.default = Empty
 
-            cls.model_rebuild(force=True)
+        cls.model_rebuild(force=True)
 
-        return cls
+        return super().__call__(*args, **kwargs)  # type: ignore[misc]
```

### Comparing `syft-0.8.6/src/syft/types/syft_migration.py` & `syft-0.8.6b1/src/syft/types/syft_migration.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/syft_object.py` & `syft-0.8.6b1/src/syft/types/syft_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from typing import Any
 from typing import ClassVar
 from typing import Optional
 from typing import TYPE_CHECKING
 from typing import Union
 from typing import get_args
 from typing import get_origin
+import warnings
 
 # third party
 import pandas as pd
 import pydantic
 from pydantic import ConfigDict
 from pydantic import EmailStr
 from pydantic import Field
@@ -549,25 +550,33 @@
         # 🟡 TODO 19: Could we do an mro style inheritence conversion? Risky?
         transform = SyftObjectRegistry.get_transform(type(self), projection)
         return transform(self, context)
 
     def to_dict(
         self, exclude_none: bool = False, exclude_empty: bool = False
     ) -> dict[str, Any]:
-        new_dict = {}
-        for k, v in dict(self).items():
-            # exclude dynamically added syft attributes
-            if k in DYNAMIC_SYFT_ATTRIBUTES:
-                continue
-            if exclude_empty and v is Empty:
-                continue
-            if exclude_none and v is None:
-                continue
-            new_dict[k] = v
-        return new_dict
+        warnings.warn(
+            "`SyftObject.to_dict` is deprecated and will be removed in a future version",
+            PendingDeprecationWarning,
+            stacklevel=2,
+        )
+        # 🟡 TODO 18: Remove to_dict and replace usage with transforms etc
+        if not exclude_none and not exclude_empty:
+            return self.dict()
+        else:
+            new_dict = {}
+            for k, v in dict(self).items():
+                # exclude dynamically added syft attributes
+                if k in DYNAMIC_SYFT_ATTRIBUTES:
+                    continue
+                if exclude_empty and v is not Empty:
+                    new_dict[k] = v
+                if exclude_none and v is not None:
+                    new_dict[k] = v
+            return new_dict
 
     def __post_init__(self) -> None:
         pass
 
     def _syft_set_validate_private_attrs_(self, **kwargs: Any) -> None:
         if not self.__validate_private_attrs__:
             return
```

### Comparing `syft-0.8.6/src/syft/types/syncable_object.py` & `syft-0.8.6b1/src/syft/types/syncable_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/transforms.py` & `syft-0.8.6b1/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/twin_object.py` & `syft-0.8.6b1/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/types/uid.py` & `syft-0.8.6b1/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/_std_stream_capture.py` & `syft-0.8.6b1/src/syft/util/_std_stream_capture.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/autoreload.py` & `syft-0.8.6b1/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/decorators.py` & `syft-0.8.6b1/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/experimental_flags.py` & `syft-0.8.6b1/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/filterwarnings.py` & `syft-0.8.6b1/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/fonts.py` & `syft-0.8.6b1/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/logger.py` & `syft-0.8.6b1/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/markdown.py` & `syft-0.8.6b1/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.6b1/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/schema.py` & `syft-0.8.6b1/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/telemetry.py` & `syft-0.8.6b1/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/trace_decorator.py` & `syft-0.8.6b1/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft/util/util.py` & `syft-0.8.6b1/src/syft/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -906,11 +906,7 @@
 
     container_host = os.getenv("CONTAINER_HOST", None)
     if container_host == "k8s":
         return f"tcp://backend:{port}"
     elif container_host == "docker":
         return f"tcp://{socket.gethostname()}:{port}"
     return f"tcp://localhost:{port}"
-
-
-def get_dev_mode() -> bool:
-    return str_to_bool(os.getenv("DEV_MODE", "False"))
```

### Comparing `syft-0.8.6/src/syft/util/version_compare.py` & `syft-0.8.6b1/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.6/src/syft.egg-info/PKG-INFO` & `syft-0.8.6b1/src/syft.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.6
+Version: 0.8.6b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -120,30 +120,30 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.6,<0.8.7")
+sy.requires(">=0.8.5,<0.8.6")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.6,<0.8.7")
+sy.requires(">=0.8.5,<0.8.6")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
 
@@ -233,20 +233,19 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.7` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.6` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8">API</a>
+`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
 
 Deprecated:
 
-- `0.8.5-post.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5-post.2/notebooks/api/0.8">API</a>
 - `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
```

### Comparing `syft-0.8.6/src/syft.egg-info/SOURCES.txt` & `syft-0.8.6b1/src/syft.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 src/syft/node/worker.py
 src/syft/node/worker_settings.py
 src/syft/protocol/data_protocol.py
 src/syft/protocol/protocol_version.json
 src/syft/protocol/releases/0.8.2.json
 src/syft/protocol/releases/0.8.3.json
 src/syft/protocol/releases/0.8.4.json
-src/syft/protocol/releases/0.8.6.json
+src/syft/protocol/releases/0.8.5.json
 src/syft/serde/__init__.py
 src/syft/serde/array.py
 src/syft/serde/arrow.py
 src/syft/serde/capnp.py
 src/syft/serde/deserialize.py
 src/syft/serde/lib_permissions.py
 src/syft/serde/lib_service_registry.py
```

### Comparing `syft-0.8.6/src/syft.egg-info/requires.txt` & `syft-0.8.6b1/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

