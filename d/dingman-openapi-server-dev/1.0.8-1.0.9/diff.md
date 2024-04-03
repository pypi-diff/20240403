# Comparing `tmp/dingman-openapi-server-dev-1.0.8.tar.gz` & `tmp/dingman-openapi-server-dev-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dingman-openapi-server-dev-1.0.8.tar", last modified: Tue Aug 15 22:05:58 2023, max compression
+gzip compressed data, was "dist/dingman-openapi-server-dev-1.0.9.tar", last modified: Wed Aug 16 21:19:56 2023, max compression
```

## Comparing `dingman-openapi-server-dev-1.0.8.tar` & `dingman-openapi-server-dev-1.0.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      274 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      902 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/dingman_openapi_server_dev.egg-info/
--rw-r--r--   0 root         (0) root         (0)      274 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/dingman_openapi_server_dev.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3459 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/dingman_openapi_server_dev.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/dingman_openapi_server_dev.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/dingman_openapi_server_dev.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/dingman_openapi_server_dev.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/openapi_server/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/__init__.py
--rw-r--r--   0 root         (0) root         (0)      393 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/openapi_server/controllers/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/controllers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5687 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/controllers/deploy_resources_controller.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/controllers/security_controller_.py
--rw-r--r--   0 root         (0) root         (0)      608 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/encoder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/
--rw-r--r--   0 root         (0) root         (0)     4321 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3753 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/affinity.py
--rw-r--r--   0 root         (0) root         (0)     1913 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/base_model_.py
--rw-r--r--   0 root         (0) root         (0)     4943 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/config.py
--rw-r--r--   0 root         (0) root         (0)     2700 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/config_templates.py
--rw-r--r--   0 root         (0) root         (0)    16535 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/container.py
--rw-r--r--   0 root         (0) root         (0)     2639 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/container_life_cycle.py
--rw-r--r--   0 root         (0) root         (0)     3654 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/container_port.py
--rw-r--r--   0 root         (0) root         (0)     5435 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/container_sec_context.py
--rw-r--r--   0 root         (0) root         (0)     2568 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/container_sec_context_capabilities.py
--rw-r--r--   0 root         (0) root         (0)     2567 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/custom_manifest.py
--rw-r--r--   0 root         (0) root         (0)    10247 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/deploy_platform_resource.py
--rw-r--r--   0 root         (0) root         (0)    12200 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/deploy_resources.py
--rw-r--r--   0 root         (0) root         (0)     3963 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/dingman_error.py
--rw-r--r--   0 root         (0) root         (0)     2425 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/dingman_response.py
--rw-r--r--   0 root         (0) root         (0)    10477 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/endpoint.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/env_from_source.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/env_var.py
--rw-r--r--   0 root         (0) root         (0)     1827 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/env_var_source.py
--rw-r--r--   0 root         (0) root         (0)     4682 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/http_get.py
--rw-r--r--   0 root         (0) root         (0)     4413 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/http_ingress_path.py
--rw-r--r--   0 root         (0) root         (0)     5643 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress.py
--rw-r--r--   0 root         (0) root         (0)     1821 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress_backend.py
--rw-r--r--   0 root         (0) root         (0)     2446 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress_backend_service.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress_rule.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress_tls.py
--rw-r--r--   0 root         (0) root         (0)     3561 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/life_cycle_handler.py
--rw-r--r--   0 root         (0) root         (0)     4613 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/node_affinity.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/node_selector.py
--rw-r--r--   0 root         (0) root         (0)     3199 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/node_selector_term.py
--rw-r--r--   0 root         (0) root         (0)     2827 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/object_field_selector.py
--rw-r--r--   0 root         (0) root         (0)     9740 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)    13340 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/pod.py
--rw-r--r--   0 root         (0) root         (0)     4649 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/pod_affinity.py
--rw-r--r--   0 root         (0) root         (0)     3664 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/pod_affinity_term.py
--rw-r--r--   0 root         (0) root         (0)     4713 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/pod_anti_affinity.py
--rw-r--r--   0 root         (0) root         (0)     3682 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/pod_sec_context.py
--rw-r--r--   0 root         (0) root         (0)     2623 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/preferred_scheduling_term.py
--rw-r--r--   0 root         (0) root         (0)     7480 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/probe.py
--rw-r--r--   0 root         (0) root         (0)     3138 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/rbac_role_ref.py
--rw-r--r--   0 root         (0) root         (0)     3577 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/rbac_rule.py
--rw-r--r--   0 root         (0) root         (0)     3598 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/ref_volume_source.py
--rw-r--r--   0 root         (0) root         (0)     6245 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/relabel_config.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/resource_requirements.py
--rw-r--r--   0 root         (0) root         (0)     4812 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/role.py
--rw-r--r--   0 root         (0) root         (0)     6130 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/role_binding.py
--rw-r--r--   0 root         (0) root         (0)     3185 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/role_binding_subject.py
--rw-r--r--   0 root         (0) root         (0)     4141 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/secret.py
--rw-r--r--   0 root         (0) root         (0)     8819 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/service.py
--rw-r--r--   0 root         (0) root         (0)     2533 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/service_account.py
--rw-r--r--   0 root         (0) root         (0)     7583 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/service_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3055 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/service_monitor_namespace_selector.py
--rw-r--r--   0 root         (0) root         (0)     6369 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/service_port.py
--rw-r--r--   0 root         (0) root         (0)     2189 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/sysctl.py
--rw-r--r--   0 root         (0) root         (0)     2413 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/tcp_socket.py
--rw-r--r--   0 root         (0) root         (0)     5341 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/toleration.py
--rw-r--r--   0 root         (0) root         (0)     5905 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/topology_spread_constraint.py
--rw-r--r--   0 root         (0) root         (0)     3521 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/update_strategy.py
--rw-r--r--   0 root         (0) root         (0)     4965 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/update_strategy_rolling_update_config.py
--rw-r--r--   0 root         (0) root         (0)     6189 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/volume.py
--rw-r--r--   0 root         (0) root         (0)     3553 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_device.py
--rw-r--r--   0 root         (0) root         (0)     2767 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_empty_dir.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_host_path.py
--rw-r--r--   0 root         (0) root         (0)     4139 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_mount.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)     2769 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/weighted_pod_affinity_term.py
--rw-r--r--   0 root         (0) root         (0)    13077 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/models/workload.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/openapi_server/openapi/
--rw-r--r--   0 root         (0) root         (0)   193428 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/openapi/openapi.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/openapi_server/test/
--rw-r--r--   0 root         (0) root         (0)      437 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)   143371 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/test/test_deploy_resources_controller.py
--rw-r--r--   0 root         (0) root         (0)      809 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/typing_utils.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_server/util.py
--rw-r--r--   0 root         (0) root         (0)        7 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/openapi_version
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-15 22:05:58.000000 dingman-openapi-server-dev-1.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      903 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/setup.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-08-15 22:05:50.000000 dingman-openapi-server-dev-1.0.8/update_dev_pkg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      274 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      902 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/dingman_openapi_server_dev.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/dingman_openapi_server_dev.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3459 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/dingman_openapi_server_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/dingman_openapi_server_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/dingman_openapi_server_dev.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/dingman_openapi_server_dev.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/openapi_server/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      393 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/openapi_server/controllers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5687 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/controllers/deploy_resources_controller.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/controllers/security_controller_.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/encoder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/
+-rw-r--r--   0 root         (0) root         (0)     4321 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3753 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/affinity.py
+-rw-r--r--   0 root         (0) root         (0)     1913 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/base_model_.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/config.py
+-rw-r--r--   0 root         (0) root         (0)     2700 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/config_templates.py
+-rw-r--r--   0 root         (0) root         (0)    16535 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/container.py
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/container_life_cycle.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/container_port.py
+-rw-r--r--   0 root         (0) root         (0)     5435 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/container_sec_context.py
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/container_sec_context_capabilities.py
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/custom_manifest.py
+-rw-r--r--   0 root         (0) root         (0)    10247 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/deploy_platform_resource.py
+-rw-r--r--   0 root         (0) root         (0)    12200 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/deploy_resources.py
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/dingman_error.py
+-rw-r--r--   0 root         (0) root         (0)     2425 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/dingman_response.py
+-rw-r--r--   0 root         (0) root         (0)    10477 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/endpoint.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/env_from_source.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/env_var.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/env_var_source.py
+-rw-r--r--   0 root         (0) root         (0)     4682 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/http_get.py
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/http_ingress_path.py
+-rw-r--r--   0 root         (0) root         (0)     5643 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress.py
+-rw-r--r--   0 root         (0) root         (0)     1821 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress_backend.py
+-rw-r--r--   0 root         (0) root         (0)     2446 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress_backend_service.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress_tls.py
+-rw-r--r--   0 root         (0) root         (0)     3561 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/life_cycle_handler.py
+-rw-r--r--   0 root         (0) root         (0)     4613 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/node_affinity.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/node_selector.py
+-rw-r--r--   0 root         (0) root         (0)     3199 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/node_selector_term.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/object_field_selector.py
+-rw-r--r--   0 root         (0) root         (0)     9740 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)    13340 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/pod.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/pod_affinity.py
+-rw-r--r--   0 root         (0) root         (0)     3664 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/pod_affinity_term.py
+-rw-r--r--   0 root         (0) root         (0)     4713 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/pod_anti_affinity.py
+-rw-r--r--   0 root         (0) root         (0)     3682 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/pod_sec_context.py
+-rw-r--r--   0 root         (0) root         (0)     2623 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/preferred_scheduling_term.py
+-rw-r--r--   0 root         (0) root         (0)     7480 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/probe.py
+-rw-r--r--   0 root         (0) root         (0)     3138 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/rbac_role_ref.py
+-rw-r--r--   0 root         (0) root         (0)     3577 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/rbac_rule.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/ref_volume_source.py
+-rw-r--r--   0 root         (0) root         (0)     6245 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/relabel_config.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/resource_requirements.py
+-rw-r--r--   0 root         (0) root         (0)     4812 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/role.py
+-rw-r--r--   0 root         (0) root         (0)     6130 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/role_binding.py
+-rw-r--r--   0 root         (0) root         (0)     3185 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/role_binding_subject.py
+-rw-r--r--   0 root         (0) root         (0)     4141 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/secret.py
+-rw-r--r--   0 root         (0) root         (0)     8819 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/service.py
+-rw-r--r--   0 root         (0) root         (0)     2533 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/service_account.py
+-rw-r--r--   0 root         (0) root         (0)     7583 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/service_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3055 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/service_monitor_namespace_selector.py
+-rw-r--r--   0 root         (0) root         (0)     6369 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/service_port.py
+-rw-r--r--   0 root         (0) root         (0)     2189 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/sysctl.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/tcp_socket.py
+-rw-r--r--   0 root         (0) root         (0)     5341 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/toleration.py
+-rw-r--r--   0 root         (0) root         (0)     5905 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/topology_spread_constraint.py
+-rw-r--r--   0 root         (0) root         (0)     3521 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/update_strategy.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/update_strategy_rolling_update_config.py
+-rw-r--r--   0 root         (0) root         (0)     6189 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/volume.py
+-rw-r--r--   0 root         (0) root         (0)     3553 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_device.py
+-rw-r--r--   0 root         (0) root         (0)     2767 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_empty_dir.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_host_path.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_mount.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     2769 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/weighted_pod_affinity_term.py
+-rw-r--r--   0 root         (0) root         (0)    13077 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/models/workload.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/openapi_server/openapi/
+-rw-r--r--   0 root         (0) root         (0)   193428 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/openapi/openapi.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/openapi_server/test/
+-rw-r--r--   0 root         (0) root         (0)      437 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   143371 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/test/test_deploy_resources_controller.py
+-rw-r--r--   0 root         (0) root         (0)      809 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/typing_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_server/util.py
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/openapi_version
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-16 21:19:56.000000 dingman-openapi-server-dev-1.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      903 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-08-16 21:19:48.000000 dingman-openapi-server-dev-1.0.9/update_dev_pkg.py
```

### Comparing `dingman-openapi-server-dev-1.0.8/README.md` & `dingman-openapi-server-dev-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/dingman_openapi_server_dev.egg-info/SOURCES.txt` & `dingman-openapi-server-dev-1.0.9/dingman_openapi_server_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/controllers/deploy_resources_controller.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/controllers/deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/controllers/security_controller_.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/controllers/security_controller_.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/encoder.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/encoder.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/__init__.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/affinity.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/affinity.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/base_model_.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/base_model_.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/config.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/config.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/config_templates.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/config_templates.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/container.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/container.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/container_life_cycle.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/container_life_cycle.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/container_port.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/container_port.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/container_sec_context.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/container_sec_context.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/container_sec_context_capabilities.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/container_sec_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/custom_manifest.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/custom_manifest.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/deploy_platform_resource.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/deploy_platform_resource.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/deploy_resources.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/deploy_resources.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/dingman_error.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/dingman_error.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/dingman_response.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/dingman_response.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/endpoint.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/env_from_source.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/env_from_source.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/env_var.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/env_var.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/env_var_source.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/env_var_source.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/http_get.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/http_get.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/http_ingress_path.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/http_ingress_path.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress_backend.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress_backend.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress_backend_service.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress_backend_service.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress_rule.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress_rule.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/ingress_tls.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/ingress_tls.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/life_cycle_handler.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/life_cycle_handler.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/node_affinity.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/node_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/node_selector.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/node_selector.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/node_selector_term.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/node_selector_term.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/object_field_selector.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/object_field_selector.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/persistent_volume_claim.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/pod.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/pod.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/pod_affinity.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/pod_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/pod_affinity_term.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/pod_anti_affinity.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/pod_sec_context.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/pod_sec_context.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/preferred_scheduling_term.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/preferred_scheduling_term.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/probe.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/probe.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/rbac_role_ref.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/rbac_role_ref.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/rbac_rule.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/rbac_rule.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/ref_volume_source.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/ref_volume_source.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/relabel_config.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/relabel_config.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/resource_requirements.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/resource_requirements.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/role.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/role.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/role_binding.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/role_binding.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/role_binding_subject.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/role_binding_subject.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/secret.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/secret.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/service.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/service.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/service_account.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/service_account.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/service_monitor.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/service_monitor.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/service_monitor_namespace_selector.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/service_monitor_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/service_port.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/service_port.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/sysctl.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/sysctl.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/tcp_socket.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/toleration.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/toleration.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/topology_spread_constraint.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/topology_spread_constraint.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/update_strategy.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/update_strategy.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/update_strategy_rolling_update_config.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/update_strategy_rolling_update_config.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/volume.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/volume.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_device.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_device.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_empty_dir.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_empty_dir.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_host_path.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_host_path.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_mount.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_mount.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/volume_persistent_volume_claim.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/volume_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/weighted_pod_affinity_term.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/weighted_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/models/workload.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/models/workload.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/openapi/openapi.yaml` & `dingman-openapi-server-dev-1.0.9/openapi_server/openapi/openapi.yaml`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/test/test_deploy_resources_controller.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/test/test_deploy_resources_controller.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/typing_utils.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/typing_utils.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/openapi_server/util.py` & `dingman-openapi-server-dev-1.0.9/openapi_server/util.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/setup.py` & `dingman-openapi-server-dev-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dingman-openapi-server-dev-1.0.8/update_dev_pkg.py` & `dingman-openapi-server-dev-1.0.9/update_dev_pkg.py`

 * *Files identical despite different names*

